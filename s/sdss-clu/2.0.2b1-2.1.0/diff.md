# Comparing `tmp/sdss_clu-2.0.2b1.tar.gz` & `tmp/sdss_clu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.0.2b1.tar", max compression
+gzip compressed data, was "sdss_clu-2.1.0.tar", max compression
```

## Comparing `sdss_clu-2.0.2b1.tar` & `sdss_clu-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1504 2023-05-23 18:42:10.362267 sdss_clu-2.0.2b1/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-05-23 18:42:10.362498 sdss_clu-2.0.2b1/README.rst
--rw-r--r--   0        0        0     2644 2023-05-23 18:42:10.376156 sdss_clu-2.0.2b1/pyproject.toml
--rw-r--r--   0        0        0      889 2023-05-23 18:42:10.376648 sdss_clu-2.0.2b1/python/clu/__init__.py
--rwxr-xr-x   0        0        0     7260 2023-05-23 18:42:10.377014 sdss_clu-2.0.2b1/python/clu/__main__.py
--rw-r--r--   0        0        0    13555 2023-05-23 18:42:10.377447 sdss_clu-2.0.2b1/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-05-23 18:42:10.377898 sdss_clu-2.0.2b1/python/clu/base.py
--rw-r--r--   0        0        0    14596 2023-05-23 18:42:10.378353 sdss_clu-2.0.2b1/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-05-23 18:42:10.378854 sdss_clu-2.0.2b1/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-05-23 18:42:10.421280 sdss_clu-2.0.2b1/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-05-23 18:42:10.502589 sdss_clu-2.0.2b1/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-05-23 18:42:10.502970 sdss_clu-2.0.2b1/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-05-23 18:42:10.503291 sdss_clu-2.0.2b1/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-05-23 18:42:10.503623 sdss_clu-2.0.2b1/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-05-23 18:42:10.503839 sdss_clu-2.0.2b1/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-05-23 18:42:10.504088 sdss_clu-2.0.2b1/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-05-23 18:42:10.504395 sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-05-23 18:42:10.504711 sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-05-23 18:42:10.505080 sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-05-23 18:42:10.505376 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-05-23 18:42:10.505775 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-05-23 18:42:10.506167 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-05-23 18:42:10.506647 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-05-23 18:42:10.507599 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-05-23 18:42:10.508114 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-05-23 18:42:10.508442 sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-05-23 18:42:10.508900 sdss_clu-2.0.2b1/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11758 2023-05-23 18:42:10.509180 sdss_clu-2.0.2b1/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-05-23 18:42:10.509537 sdss_clu-2.0.2b1/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-05-23 18:42:10.509825 sdss_clu-2.0.2b1/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-05-23 18:42:10.510042 sdss_clu-2.0.2b1/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-05-23 18:42:10.510306 sdss_clu-2.0.2b1/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-05-23 18:42:10.510527 sdss_clu-2.0.2b1/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-05-23 18:42:10.510746 sdss_clu-2.0.2b1/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-05-23 18:42:10.511034 sdss_clu-2.0.2b1/python/clu/tools.py
--rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 sdss_clu-2.0.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-06-21 19:00:04.136605 sdss_clu-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-06-21 19:00:04.136911 sdss_clu-2.1.0/README.rst
+-rw-r--r--   0        0        0     2774 2023-06-21 19:00:04.150234 sdss_clu-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-06-21 19:00:04.150625 sdss_clu-2.1.0/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     9074 2023-06-21 19:00:04.150900 sdss_clu-2.1.0/python/clu/__main__.py
+-rw-r--r--   0        0        0    13555 2023-06-21 19:00:04.151167 sdss_clu-2.1.0/python/clu/actor.py
+-rw-r--r--   0        0        0    19832 2023-06-21 19:00:04.151454 sdss_clu-2.1.0/python/clu/base.py
+-rw-r--r--   0        0        0    14705 2023-06-21 19:00:04.151738 sdss_clu-2.1.0/python/clu/client.py
+-rw-r--r--   0        0        0    20069 2023-06-21 19:00:04.152048 sdss_clu-2.1.0/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-06-21 19:00:04.152368 sdss_clu-2.1.0/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-06-21 19:00:04.152584 sdss_clu-2.1.0/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-06-21 19:00:04.152890 sdss_clu-2.1.0/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    17892 2023-06-21 19:00:04.153192 sdss_clu-2.1.0/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-06-21 19:00:04.153573 sdss_clu-2.1.0/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-06-21 19:00:04.153821 sdss_clu-2.1.0/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-06-21 19:00:04.154044 sdss_clu-2.1.0/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-06-21 19:00:04.154344 sdss_clu-2.1.0/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-06-21 19:00:04.154681 sdss_clu-2.1.0/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-06-21 19:00:04.154939 sdss_clu-2.1.0/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-06-21 19:00:04.155211 sdss_clu-2.1.0/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-06-21 19:00:04.155653 sdss_clu-2.1.0/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-06-21 19:00:04.155941 sdss_clu-2.1.0/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-06-21 19:00:04.156310 sdss_clu-2.1.0/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-06-21 19:00:04.157049 sdss_clu-2.1.0/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-06-21 19:00:04.157341 sdss_clu-2.1.0/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-06-21 19:00:04.157780 sdss_clu-2.1.0/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-06-21 19:00:04.158177 sdss_clu-2.1.0/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11758 2023-06-21 19:00:04.158499 sdss_clu-2.1.0/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-06-21 19:00:04.158939 sdss_clu-2.1.0/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20428 2023-06-21 19:00:04.159248 sdss_clu-2.1.0/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-06-21 19:00:04.159550 sdss_clu-2.1.0/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-06-21 19:00:04.159899 sdss_clu-2.1.0/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-06-21 19:00:04.160148 sdss_clu-2.1.0/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-06-21 19:00:04.160404 sdss_clu-2.1.0/python/clu/testing.py
+-rw-r--r--   0        0        0    16901 2023-06-21 19:00:04.160692 sdss_clu-2.1.0/python/clu/tools.py
+-rw-r--r--   0        0        0     3648 2023-06-21 19:00:04.160967 sdss_clu-2.1.0/python/clu/websocket.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.0/PKG-INFO
```

### Comparing `sdss_clu-2.0.2b1/LICENSE.md` & `sdss_clu-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/README.rst` & `sdss_clu-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/pyproject.toml` & `sdss_clu-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.0.2b1"
+version = "2.1.0"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
@@ -31,14 +31,16 @@
 click = "^8.0"
 aio_pika = "^9.0.0"
 jsonschema = "^4.0.1"
 sdsstools = "^1.0.0"
 prompt_toolkit = "^3.0.6"
 aiormq = "^6.6.4"
 unclick = "^0.1.0b4"
+websockets = {version = "^11.0.3", optional = true}
+click-default-group = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 toml = ">=0.10.0"
 isort = ">=5.2.2"
@@ -56,14 +58,17 @@
 Sphinx = ">=5.0.0"
 myst-parser = ">=0.14.0"
 sphinx-copybutton = ">=0.3.3"
 nox = ">=2021.6.12"
 sphinx-autobuild = ">=2021.3.14"
 furo = ">=2021.6.18"
 
+[tool.poetry.extras]
+websocket = ["websockets"]
+
 [tool.black]
 line-length = 88
 target-version = ['py311']
 fast = true
 extend-exclude = 'docs/sphinx/examples/.+\.py'
 
 [tool.isort]
```

### Comparing `sdss_clu-2.0.2b1/python/clu/__init__.py` & `sdss_clu-2.1.0/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/__main__.py` & `sdss_clu-2.1.0/python/clu/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,22 @@
 #
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2019-05-20
 # @Filename: __main__.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 import asyncio
-import datetime
-import json
-import os
-import uuid
 
 import aio_pika
 import click
-import prompt_toolkit
-import pygments
-import pygments.lexers
-from prompt_toolkit import print_formatted_text as print
-from prompt_toolkit.formatted_text import PygmentsTokens
-from prompt_toolkit.history import FileHistory
-from prompt_toolkit.patch_stdout import patch_stdout
-from prompt_toolkit.styles import style_from_pygments_cls
-from pygments.styles import STYLE_MAP, get_style_by_name
+from click_default_group import DefaultGroup
 
 import clu
 
 
-style_name = "solarized-dark" if "solarized-dark" in STYLE_MAP else "default"
-style = style_from_pygments_cls(get_style_by_name(style_name))  # type: ignore
-
-
 color_codes = {
     ">": "lightblue",
     "i": "lightblue",
     "d": "gray",
     "w": "yellow",
     "e": "LightCoral",
     "f": "red",
@@ -46,32 +30,48 @@
     """A shell client."""
 
     actors: tuple[str, ...] = ()
     indent = False
     show_time = True
     ignore_broadcasts = False
     internal = False
+    all_ = False
 
     async def handle_reply(self, message: aio_pika.IncomingMessage):
         """Prints the formatted reply."""
 
+        import datetime
+        import json
+
+        import prompt_toolkit
+        import pygments.lexers
+        from prompt_toolkit import print_formatted_text as print
+        from prompt_toolkit.formatted_text import PygmentsTokens
+        from prompt_toolkit.styles import style_from_pygments_cls
+        from pygments.styles import STYLE_MAP, get_style_by_name
+
         reply = await super().handle_reply(message)
 
         if reply is None or (self.internal is False and reply.internal is True):
             return
 
         headers = reply.info.get("headers", {})
         commander_id = headers.get("commander_id", None)
         if commander_id:
             commander_id = str(commander_id).split(".")[0]
 
         routing_key = message.routing_key
         is_broadcast = routing_key == "reply.broadcast" or reply.command_id is None
 
-        if commander_id and commander_id != self.name and not is_broadcast:
+        if (
+            commander_id
+            and commander_id != self.name
+            and not is_broadcast
+            and not self.all_
+        ):
             return
 
         if self.ignore_broadcasts and is_broadcast:
             return
 
         message_code = reply.message_code
         sender = headers.get("sender", "")
@@ -111,33 +111,44 @@
                     f'<style fg="magenta">{sender}</style>'
                 ),
             )
 
         if message_code:
             print_chunks.append(message_code_formatted)
 
+        style_name = "solarized-dark" if "solarized-dark" in STYLE_MAP else "default"
+        style = style_from_pygments_cls(get_style_by_name(style_name))  # type: ignore
+
         if body:
             print_chunks.append(PygmentsTokens(body_tokens))
             print(*print_chunks, style=style, end="")
         else:
             print(*print_chunks)  # Newline
 
 
 async def shell_client_prompt(
     actors: tuple[str, ...] = (),
     url: str | None = None,
     user: str = "guest",
     password: str = "guest",
     host: str = "127.0.0.1",
     port: int = 5672,
+    all_: bool = False,
     indent=True,
     show_time=True,
     ignore_broadcasts=False,
     internal=False,
 ):
+    import os
+    import uuid
+
+    import prompt_toolkit
+    from prompt_toolkit.history import FileHistory
+    from prompt_toolkit.patch_stdout import patch_stdout
+
     # Give each client a unique name to ensure the queues are unique.
     uid = str(uuid.uuid4()).split("-")[0]
 
     client = await ShellClient(
         f"shell_client_{uid}",
         url=url,
         user=user,
@@ -148,14 +159,15 @@
     ).start()
 
     client.actors = actors
     client.indent = indent
     client.show_time = show_time
     client.ignore_broadcasts = ignore_broadcasts
     client.internal = internal
+    client.all_ = all_
 
     history = FileHistory(os.path.expanduser("~/.clu_history"))
 
     session = prompt_toolkit.PromptSession("", history=history)
 
     while True:
         with patch_stdout():
@@ -176,18 +188,29 @@
                     if len(chunks) < 2:
                         print(f"Invalid command {text!r}")
                         continue
 
                     actor = chunks[0]
                     command_string = " ".join(chunks[1:])
 
-                    await client.send_command(actor, command_string)
+                    await client.send_command(
+                        actor,
+                        command_string,
+                        await_command=False,
+                    )
+
+
+@click.group(cls=DefaultGroup, default="cli", default_if_no_args=True, name="clu")
+def clu_cli():
+    """CLU command line interface."""
+
+    pass
 
 
-@click.command(name="clu")
+@clu_cli.command(name="cli")
 @click.argument(
     "ACTORS",
     type=str,
     required=False,
     nargs=-1,
 )
 @click.option(
@@ -224,14 +247,21 @@
     "-p",
     type=int,
     show_default=True,
     default=5672,
     help="The port on which the server is running",
 )
 @click.option(
+    "--all",
+    "-a",
+    "all_",
+    is_flag=True,
+    help="Print all messages, not only those replying to commands sent from this CLI.",
+)
+@click.option(
     "--no-indent",
     "-n",
     is_flag=True,
     default=False,
     help="Do not indent the output JSONs.",
 )
 @click.option(
@@ -249,21 +279,22 @@
     help="Do not show the message time.",
 )
 @click.option(
     "--internal",
     is_flag=True,
     help="Show internal messages.",
 )
-def clu_cli(
+def cli(
     actors: tuple[str, ...] = (),
     url: str | None = None,
     user: str = "guest",
     password: str = "guest",
     host: str = "localhost",
     port: int = 5672,
+    all_: bool = False,
     no_indent=False,
     no_time=False,
     ignore_broadcasts=False,
     internal=False,
 ):
     """Runs the AMQP command line interpreter."""
 
@@ -271,22 +302,67 @@
         shell_client_prompt(
             actors=actors,
             url=url,
             user=user,
             password=password,
             host=host,
             port=port,
+            all_=all_,
             indent=not no_indent,
             show_time=not no_time,
             ignore_broadcasts=ignore_broadcasts,
             internal=internal,
         )
     )
     asyncio.get_event_loop().run_until_complete(shell_task)
 
 
+@clu_cli.command()
+@click.option(
+    "--port",
+    "-p",
+    default=9876,
+    show_default=True,
+    type=int,
+    help="The port on which to serve the websocket",
+)
+@click.option(
+    "--rabbitmq-host",
+    "-H",
+    type=str,
+    show_default=True,
+    default="localhost",
+    help="The host running the AMQP server.",
+)
+@click.option(
+    "--rabbitmq-port",
+    "-P",
+    type=int,
+    show_default=True,
+    default=5672,
+    help="The port on which the AMQP server is running.",
+)
+def websocket(port=9876, rabbitmq_host="localhost", rabbitmq_port=5672):
+    """Launches a websocket server connected to a RabbitMQ exchange."""
+
+    try:
+        from clu.websocket import WebsocketServer
+    except ImportError:
+        click.echo("websockets package is needed. Try pip install sdss-clu[websocket].")
+        return
+
+    async def _async_helper():
+        ws = WebsocketServer(wport=port, host=rabbitmq_host, port=rabbitmq_port)
+        await ws.start()
+
+        # Run forever.
+        await asyncio.Future()
+
+    asyncio.run(_async_helper())
+
+
 def main():
     clu_cli(obj={})
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sdss_clu-2.0.2b1/python/clu/actor.py` & `sdss_clu-2.1.0/python/clu/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/base.py` & `sdss_clu-2.1.0/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/client.py` & `sdss_clu-2.1.0/python/clu/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,29 +162,32 @@
         A list of actor models whose schemas will be monitored.
     """
 
     __EXCHANGE_NAME__ = "sdss_exchange"
 
     def __init__(
         self,
-        name: str,
+        name: str | None = None,
         url: Optional[str] = None,
         user: str = "guest",
         password: str = "guest",
         host: str = "localhost",
         port: int = 5672,
         virtualhost: str = "/",
         ssl: bool = False,
         version: Optional[str] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         log_dir: Optional[PathLike] = None,
         log: Optional[SDSSLogger] = None,
         models: List[str] = [],
         **kwargs,
     ):
+        if name is None:
+            name = "amqp-client-" + str(uuid.uuid4()).split("-")[-1]
+
         super().__init__(
             name,
             version=version,
             loop=loop,
             log_dir=log_dir,
             log=log,
             **kwargs,
```

### Comparing `sdss_clu-2.0.2b1/python/clu/command.py` & `sdss_clu-2.1.0/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/device.py` & `sdss_clu-2.1.0/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/exceptions.py` & `sdss_clu-2.1.0/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/actor.py` & `sdss_clu-2.1.0/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/tron.py` & `sdss_clu-2.1.0/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/html.py` & `sdss_clu-2.1.0/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py` & `sdss_clu-2.1.0/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py` & `sdss_clu-2.1.0/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py` & `sdss_clu-2.1.0/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.1.0/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.1.0/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.1.0/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.1.0/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.1.0/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py` & `sdss_clu-2.1.0/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/legacy/types/types.py` & `sdss_clu-2.1.0/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/model.py` & `sdss_clu-2.1.0/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/parsers/click.py` & `sdss_clu-2.1.0/python/clu/parsers/click.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/parsers/json.py` & `sdss_clu-2.1.0/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/protocol.py` & `sdss_clu-2.1.0/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/store.py` & `sdss_clu-2.1.0/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/testing.py` & `sdss_clu-2.1.0/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/python/clu/tools.py` & `sdss_clu-2.1.0/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2b1/PKG-INFO` & `sdss_clu-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.0.2b1
+Version: 2.1.0
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -16,21 +16,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: websocket
 Requires-Dist: aio_pika (>=9.0.0,<10.0.0)
 Requires-Dist: aiormq (>=6.6.4,<7.0.0)
 Requires-Dist: click (>=8.0,<9.0)
+Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: jsonschema (>=4.0.1,<5.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.6,<4.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: unclick (>=0.1.0b4,<0.2.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0) ; extra == "websocket"
 Project-URL: Documentation, https://clu.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/clu
 Description-Content-Type: text/x-rst
 
 `CLU <https://tron.fandom.com/wiki/Clu>`__
 ==========================================
```

