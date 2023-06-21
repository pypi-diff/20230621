# Comparing `tmp/ltchiptool_terminal-1.0.0.tar.gz` & `tmp/ltchiptool_terminal-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool_terminal-1.0.0.tar", max compression
+gzip compressed data, was "ltchiptool_terminal-1.1.0.tar", max compression
```

## Comparing `ltchiptool_terminal-1.0.0.tar` & `ltchiptool_terminal-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/README.md
--rw-r--r--   0        0        0      648 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/ltctplugin/terminal/__init__.py
--rw-r--r--   0        0        0    12740 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/ltctplugin/terminal/gui.py
--rw-r--r--   0        0        0     4217 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/ltctplugin/terminal/terminal.wxui
--rw-r--r--   0        0        0     5485 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/ltctplugin/terminal/terminal.xrc
--rw-r--r--   0        0        0     3744 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/ltctplugin/terminal/work.py
--rw-r--r--   0        0        0      491 2023-06-15 18:44:17.339450 ltchiptool_terminal-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 ltchiptool_terminal-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/README.md
+-rw-r--r--   0        0        0      648 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/__init__.py
+-rw-r--r--   0        0        0    13754 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/gui.py
+-rw-r--r--   0        0        0     4217 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.wxui
+-rw-r--r--   0        0        0     5485 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.xrc
+-rw-r--r--   0        0        0     3744 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/work.py
+-rw-r--r--   0        0        0      491 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 ltchiptool_terminal-1.1.0/PKG-INFO
```

### Comparing `ltchiptool_terminal-1.0.0/ltctplugin/terminal/__init__.py` & `ltchiptool_terminal-1.1.0/ltctplugin/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.0.0/ltctplugin/terminal/gui.py` & `ltchiptool_terminal-1.1.0/ltctplugin/terminal/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,33 @@
     def open_real_terminal(self):
         ...
 
     def close_real_terminal(self):
         ...
 
 
+class SerialHook:
+    def on_serial_receive(self, data: bytes) -> bool | None:
+        pass
+
+    def on_serial_open(self, port: str) -> None:
+        pass
+
+    def on_serial_close(self, port: str) -> None:
+        pass
+
+
 class TerminalPanel(BasePanel):
     Flash: FlashPanel = None
     FlashPortsUpdated: Callable[[list[tuple[str, bool, str]]], None] = None
     FlashWorkStopped: Callable[[BaseThread], None] = None
     delayed_port: str | None = None
     ports_busy: set[str]
     serial: SerialMixin = None
+    hooks: list[SerialHook] = None
     newlines = {
         (False, False): b"",
         (False, True): b"\n",
         (True, False): b"\r",
         (True, True): b"\r\n",
     }
     newline: bytes = b""
@@ -65,14 +77,15 @@
         self.BoxEcho = self.BindCheckBox("checkbox_echo")
         self.Text: wx.TextCtrl = self.FindWindowByName("text_console", self)
         self.Text.SetDefaultStyle(wx.TextAttr(wx.WHITE))
         self.Text.Bind(wx.EVT_CHAR, self.OnKeyEvent)
 
         # noinspection PyTypeChecker
         self.serial = Serial()
+        self.hooks = []
         ColorPalette.get().apply(self.Text)
         self.Text.SetDefaultStyle(wx.TextAttr(ColorPalette.get()[self.fg]))
 
     def GetSettings(self) -> dict:
         return dict(
             port=self.port,
             baudrate=self.baudrate,
@@ -206,14 +219,16 @@
         if self.serial.is_open or real_port in self.ports_busy:
             # don't open twice, ignore busy ports
             return
         try:
             self.serial.port = self.real_port
             self.serial.baudrate = self.baudrate
             self.serial.open_real_terminal()
+            for hook in self.hooks:
+                hook.on_serial_open(self.serial.port)
             self.DoUpdate()
             self.StartWork(
                 TerminalThread(
                     s=self.serial,
                     on_serial_data=self.OnSerialData,
                     on_control_data=self.OnControlData,
                 ),
@@ -222,18 +237,36 @@
         except Exception as e:
             LoggingHandler.get().emit_exception(e, msg=f"Couldn't open {self.port}")
             self.PortClose()
 
     def PortClose(self) -> None:
         self.StopWork(TerminalThread)
         self.serial.close_real_terminal()
+        for hook in self.hooks:
+            hook.on_serial_close(self.serial.port)
         # this freezes the app
         # self.DoUpdate()
         self.Port.Enable(True)
 
+    def PortWrite(self, data: bytes) -> None:
+        if not self.serial.is_open:
+            return
+        self.serial.write(data)
+
+    def PortIsOpen(self) -> bool:
+        return self.serial.is_open
+
+    def PortAddHook(self, hook: SerialHook) -> None:
+        if hook not in self.hooks:
+            self.hooks.append(hook)
+
+    def PortRemoveHook(self, hook: SerialHook) -> None:
+        if hook in self.hooks:
+            self.hooks.remove(hook)
+
     def OnPortsUpdated(self, ports: list[tuple[str, bool, str]]) -> None:
         user_port = self.port or self.delayed_port
         if self.FlashPortsUpdated:
             self.FlashPortsUpdated(ports)
         items: list[str] = self.Flash.Port.GetStrings()
         items.insert(0, "Same as for flashing")
         self.Port.Set(items)
@@ -260,14 +293,17 @@
             text = chr(key)
             if self.echo:
                 self.Text.AppendText(text)
             text = text.encode("utf-8", "ignore")
         self.serial.write(text)
 
     def OnSerialData(self, data: bytes) -> None:
+        for hook in self.hooks:
+            if hook.on_serial_receive(data) is True:
+                return
         data = data.replace(b"\r\n", b"\n")
         data = data.replace(b"\r", b"")
         text = data.decode("utf-8", errors="replace")
         self.Text.AppendText(text)
 
     def OnControlData(self, data: bytes) -> None:
         if not (data.startswith(b"\x1B[") and data.endswith(b"m")):
```

### Comparing `ltchiptool_terminal-1.0.0/ltctplugin/terminal/terminal.wxui` & `ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.0.0/ltctplugin/terminal/terminal.xrc` & `ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.0.0/ltctplugin/terminal/work.py` & `ltchiptool_terminal-1.1.0/ltctplugin/terminal/work.py`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.0.0/PKG-INFO` & `ltchiptool_terminal-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool-terminal
-Version: 1.0.0
+Version: 1.1.0
 Summary: Serial terminal plugin for ltchiptool
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

