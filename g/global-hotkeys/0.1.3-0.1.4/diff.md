# Comparing `tmp/global_hotkeys-0.1.3.tar.gz` & `tmp/global_hotkeys-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.3.tar", last modified: Mon May 29 03:26:01 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.4.tar", last modified: Wed Jun 21 13:10:57 2023, max compression
```

## Comparing `global_hotkeys-0.1.3.tar` & `global_hotkeys-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/
--rw-rw-rw-   0        0        0     1403 2023-05-29 03:25:19.000000 global_hotkeys-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8921 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6984 2023-05-28 21:39:05.000000 global_hotkeys-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.927352 global_hotkeys-0.1.3/global_hotkeys/
--rw-rw-rw-   0        0        0     3486 2023-05-29 03:21:04.000000 global_hotkeys-0.1.3/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0    10334 2023-05-28 21:25:45.000000 global_hotkeys-0.1.3/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.3/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.944145 global_hotkeys-0.1.3/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     8921 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-29 03:23:27.000000 global_hotkeys-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.958145 global_hotkeys-0.1.3/tests/
--rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.3/tests/_t.py
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.3/tests/global_snippets.py
--rw-rw-rw-   0        0        0     1381 2023-05-29 03:22:24.000000 global_hotkeys-0.1.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/
+-rw-rw-rw-   0        0        0     1403 2023-05-29 03:25:19.000000 global_hotkeys-0.1.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9662 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7725 2023-06-21 13:08:54.000000 global_hotkeys-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.665789 global_hotkeys-0.1.4/global_hotkeys/
+-rw-rw-rw-   0        0        0     4320 2023-06-21 12:57:14.000000 global_hotkeys-0.1.4/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0    10304 2023-06-21 12:58:55.000000 global_hotkeys-0.1.4/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.4/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.679529 global_hotkeys-0.1.4/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     9662 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 13:10:57.000000 global_hotkeys-0.1.4/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:10:57.694508 global_hotkeys-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-06-21 13:09:57.000000 global_hotkeys-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:10:57.692528 global_hotkeys-0.1.4/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.4/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.4/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     2091 2023-06-21 13:05:55.000000 global_hotkeys-0.1.4/tests/test.py
```

### Comparing `global_hotkeys-0.1.3/CHANGELOG.txt` & `global_hotkeys-0.1.4/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.3/LICENSE.txt` & `global_hotkeys-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.3/PKG-INFO` & `global_hotkeys-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 ## Example usage
 
 ```python
 from global_hotkeys import *
 
 import time
 
-# Flag to indicate the program whether should continue running.
+# Flag to indicate whether the program should continue running.
 is_alive = True
 
 def print_hello():
     print("Hello")
 
 def print_world():
     print("World")
@@ -46,36 +46,52 @@
 
 def print_bar():
     print("Bar")
 
 def print_with_params(params):
     print(params["test"])
 
+def press_with_params(params):
+    print(params["press_param"])
+
+def release_with_params(params):
+    print(params["release_param"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    
-    # We can even use a dict format now for our bindings as well:
+    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
 
     },
+    # dict style with differentiating params for press and release callbacks
+    {
+        "hotkey": "control + 9",
+        "on_press_callback": press_with_params,
+        "on_release_callback": release_with_params,
+        "actuate_on_partial_release": False,
+        "press_callback_params": {"press_param":"ctrl+9 pressed!"},
+        "release_callback_params": {"release_param": "ctrl+9 released!"},
+
+    },
 
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
@@ -85,15 +101,17 @@
 #
 # Or in explicit dict format:
 # {
 #     "hotkey": <binding>,
 #     "on_press_callback": <press_callback>,
 #     "on_release_callback": <release_callback>,
 #     "actuate_on_partial_release": False | True,
-#     "callback_params": <a variable or expression can go here>)
+#     "callback_params": <a variable or expression can go here>  <-- This applies to both callbacks.
+#     "press_callback_params": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
 # }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
@@ -166,30 +184,30 @@
 enter
 shift
 control
 alt
 pause
 caps_lock
 escape
-space   <-- a literal space character (' ') can be used as well.
+space
 page_up
 page_down
 left_window
 right_window
 window
 end
 home
 left
 up
 right
 down
 select
 print
 execute
-enter": win32con.VK_
+enter
 print_screen
 insert
 delete
 help
 0
 1
 2
```

### Comparing `global_hotkeys-0.1.3/README.md` & `global_hotkeys-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## Example usage
 
 ```python
 from global_hotkeys import *
 
 import time
 
-# Flag to indicate the program whether should continue running.
+# Flag to indicate whether the program should continue running.
 is_alive = True
 
 def print_hello():
     print("Hello")
 
 def print_world():
     print("World")
@@ -29,36 +29,52 @@
 
 def print_bar():
     print("Bar")
 
 def print_with_params(params):
     print(params["test"])
 
+def press_with_params(params):
+    print(params["press_param"])
+
+def release_with_params(params):
+    print(params["release_param"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    
-    # We can even use a dict format now for our bindings as well:
+    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
 
     },
+    # dict style with differentiating params for press and release callbacks
+    {
+        "hotkey": "control + 9",
+        "on_press_callback": press_with_params,
+        "on_release_callback": release_with_params,
+        "actuate_on_partial_release": False,
+        "press_callback_params": {"press_param":"ctrl+9 pressed!"},
+        "release_callback_params": {"release_param": "ctrl+9 released!"},
+
+    },
 
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
@@ -68,15 +84,17 @@
 #
 # Or in explicit dict format:
 # {
 #     "hotkey": <binding>,
 #     "on_press_callback": <press_callback>,
 #     "on_release_callback": <release_callback>,
 #     "actuate_on_partial_release": False | True,
-#     "callback_params": <a variable or expression can go here>)
+#     "callback_params": <a variable or expression can go here>  <-- This applies to both callbacks.
+#     "press_callback_params": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
 # }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
@@ -149,30 +167,30 @@
 enter
 shift
 control
 alt
 pause
 caps_lock
 escape
-space   <-- a literal space character (' ') can be used as well.
+space
 page_up
 page_down
 left_window
 right_window
 window
 end
 home
 left
 up
 right
 down
 select
 print
 execute
-enter": win32con.VK_
+enter
 print_screen
 insert
 delete
 help
 0
 1
 2
```

### Comparing `global_hotkeys-0.1.3/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.4/global_hotkeys/hotkey_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         return True
 
     def _reset_binding_press_state(self, hotkey_id):
         for i in range(0, len(self.hotkey_actions[hotkey_id][2])):
             self.hotkey_actions[hotkey_id][2][i] = 0
 
-    def register_hotkey(self, binding, press_callback, release_callback, actuate_on_partial_release, callback_params):
+    def register_hotkey(self, binding, press_callback, release_callback, actuate_on_partial_release, press_callback_params, release_callback_params):
         self._is_valid_binding(binding)
         
         self.hotkey_counter += 1
         id = self.hotkey_counter
 
         hotkey_id = self._find_hotkey_id(binding)
         if hotkey_id != None:
@@ -110,20 +110,15 @@
             )
             return False
 
         # we want to track how far along the binding's chording sequence we've progressed.
         binding_press_state = [0 for i in range(0, len(binding))]
 
         self.hotkeys[id] = binding
-        self.hotkey_actions[id] = [press_callback, release_callback, binding_press_state, actuate_on_partial_release, callback_params]
-
-        # print(f"id: {id}")
-        # print(str(self.hotkeys))
-        # print(str(self.hotkey_actions))
-        # print("------")
+        self.hotkey_actions[id] = [press_callback, release_callback, binding_press_state, actuate_on_partial_release, press_callback_params, release_callback_params]
 
         return True
     
     def _find_index_of_first_item_not_matching_in_list(self, _list, target):
         for i in range(0, len(_list)):
             if _list[i] != target:
                 return i
@@ -191,15 +186,15 @@
             time.sleep(0.02)
             # Exit out if the main thread has terminated.
             if not main_thread().is_alive():
                 break
 
             for id in id_list:
                 hotkey = self.hotkeys[id]
-                press_callback, release_callback, binding_press_state, actuate_on_partial_release, callback_params = self.hotkey_actions[id]
+                press_callback, release_callback, binding_press_state, actuate_on_partial_release, press_callback_params, release_callback_params = self.hotkey_actions[id]
                 key_state_id = self._find_index_of_first_item_not_matching_in_list(binding_press_state, 2)
                 if(key_state_id is None):
                     raise Exception("binding_press_state was not reset after completion!")
                     continue
                 key_state = binding_press_state[key_state_id]
                 chord = [_to_virtualkey(key) if key != "window" else "window" for key in hotkey[key_state_id]]
 
@@ -229,27 +224,27 @@
                     pressed = self._are_all_keys_not_pressed_in_chord(non_allowed_modifiers)
 
                 if pressed:
                     this_is_the_last_chord = key_state_id == len(hotkey) - 1
                     self.hotkey_actions[id][2][key_state_id] = 1
                     if (key_state != 1) and (this_is_the_last_chord):
                         if press_callback != None:
-                            if callback_params != None:
-                                press_callback(callback_params)
+                            if press_callback_params != None:
+                                press_callback(press_callback_params)
                             else:
-                                press_callback(callback_params)
+                                press_callback()
                 else:
                     this_is_the_last_chord = key_state_id == len(hotkey) - 1
                     #self.hotkey_actions[id][2] = False
                     if (key_state == 1):
                         if this_is_the_last_chord:
                             if fully_not_pressed or actuate_on_partial_release:
                                 self._reset_binding_press_state(id)
                                 if release_callback != None:
-                                    if callback_params != None:
-                                        release_callback(callback_params)
+                                    if release_callback_params != None:
+                                        release_callback(release_callback_params)
                                     else:
                                         release_callback()
                         else:
                             self.hotkey_actions[id][2][key_state_id] = 2
 
-hotkey_checker = HotkeyChecker()
+hotkey_checker = HotkeyChecker()
```

### Comparing `global_hotkeys-0.1.3/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.4/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.3/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.4/global_hotkeys.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 ## Example usage
 
 ```python
 from global_hotkeys import *
 
 import time
 
-# Flag to indicate the program whether should continue running.
+# Flag to indicate whether the program should continue running.
 is_alive = True
 
 def print_hello():
     print("Hello")
 
 def print_world():
     print("World")
@@ -46,36 +46,52 @@
 
 def print_bar():
     print("Bar")
 
 def print_with_params(params):
     print(params["test"])
 
+def press_with_params(params):
+    print(params["press_param"])
+
+def release_with_params(params):
+    print(params["release_param"])
+
 def exit_application():
     global is_alive
     print("exiting")
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
     ["control + 5", None, print_hello, False],
     ["control + 6", None, print_with_params, False, {"test":5}],
-    
-    # We can even use a dict format now for our bindings as well:
+    ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
+    # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
         "actuate_on_partial_release": False,
         "callback_params": {"test": "testing"},
 
     },
+    # dict style with differentiating params for press and release callbacks
+    {
+        "hotkey": "control + 9",
+        "on_press_callback": press_with_params,
+        "on_release_callback": release_with_params,
+        "actuate_on_partial_release": False,
+        "press_callback_params": {"press_param":"ctrl+9 pressed!"},
+        "release_callback_params": {"release_param": "ctrl+9 released!"},
+
+    },
 
     ["window + 1", None, print_foo, False],
     ["t,m", None, print_bar, False],
     ["control + Q", None, exit_application, False],
 ]
 
 # Bindings take on the form of:
@@ -85,15 +101,17 @@
 #
 # Or in explicit dict format:
 # {
 #     "hotkey": <binding>,
 #     "on_press_callback": <press_callback>,
 #     "on_release_callback": <release_callback>,
 #     "actuate_on_partial_release": False | True,
-#     "callback_params": <a variable or expression can go here>)
+#     "callback_params": <a variable or expression can go here>  <-- This applies to both callbacks.
+#     "press_callback_params": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
 # }
 
 # It's useful to have 'actuate_on_partial_release_flag' set to False, 
 # so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
 
 # Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
 # and additional key chords are separated by commas. Spaces are ignored.
@@ -166,30 +184,30 @@
 enter
 shift
 control
 alt
 pause
 caps_lock
 escape
-space   <-- a literal space character (' ') can be used as well.
+space
 page_up
 page_down
 left_window
 right_window
 window
 end
 home
 left
 up
 right
 down
 select
 print
 execute
-enter": win32con.VK_
+enter
 print_screen
 insert
 delete
 help
 0
 1
 2
```

### Comparing `global_hotkeys-0.1.3/setup.py` & `global_hotkeys-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.3',
+  version='0.1.4',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
```

### Comparing `global_hotkeys-0.1.3/tests/global_snippets.py` & `global_hotkeys-0.1.4/tests/global_snippets.py`

 * *Files identical despite different names*

