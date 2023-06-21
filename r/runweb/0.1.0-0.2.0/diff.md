# Comparing `tmp/runweb-0.1.0.tar.gz` & `tmp/runweb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runweb-0.1.0.tar", last modified: Sat Jun 17 17:13:31 2023, max compression
+gzip compressed data, was "runweb-0.2.0.tar", last modified: Wed Jun 21 15:50:23 2023, max compression
```

## Comparing `runweb-0.1.0.tar` & `runweb-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11341 2023-06-17 17:13:12.036382 runweb-0.1.0/LICENSE
--rw-r--r--   0        0        0      729 2023-06-17 17:13:12.036382 runweb-0.1.0/README.md
--rw-r--r--   0        0        0     1218 2023-06-17 17:13:31.184450 runweb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/__init__.py
--rw-r--r--   0        0        0       29 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/__main__.py
--rw-r--r--   0        0        0       22 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/__version__.py
--rw-r--r--   0        0        0     3544 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/main.py
--rw-r--r--   0        0        0     2298 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/multiprocess.py
--rw-r--r--   0        0        0     1897 2023-06-17 17:13:12.036382 runweb-0.1.0/runweb/parse.py
--rw-r--r--   0        0        0        0 2023-06-17 17:13:12.040382 runweb-0.1.0/runweb/runner/__init__.py
--rw-r--r--   0        0        0      851 2023-06-17 17:13:12.040382 runweb-0.1.0/runweb/runner/uvicorn.py
--rw-r--r--   0        0        0      840 2023-06-17 17:13:12.040382 runweb-0.1.0/runweb/runner/waitress.py
--rw-r--r--   0        0        0        0 2023-06-17 17:13:12.040382 runweb-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-06-17 17:13:12.040382 runweb-0.1.0/tests/test_uvicorn.py
--rw-r--r--   0        0        0      934 2023-06-17 17:13:12.040382 runweb-0.1.0/tests/test_waitress.py
--rw-r--r--   0        0        0      866 2023-06-17 17:13:12.040382 runweb-0.1.0/tests/utils.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-06-21 15:50:04.971581 runweb-0.2.0/LICENSE
+-rw-r--r--   0        0        0      729 2023-06-21 15:50:04.971581 runweb-0.2.0/README.md
+-rw-r--r--   0        0        0     1218 2023-06-21 15:50:23.816752 runweb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__init__.py
+-rw-r--r--   0        0        0       29 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__version__.py
+-rw-r--r--   0        0        0     3544 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/main.py
+-rw-r--r--   0        0        0     2171 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/multiprocess.py
+-rw-r--r--   0        0        0     2110 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/parse.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/__init__.py
+-rw-r--r--   0        0        0      798 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/uvicorn.py
+-rw-r--r--   0        0        0      787 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/waitress.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/test_uvicorn.py
+-rw-r--r--   0        0        0      934 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/test_waitress.py
+-rw-r--r--   0        0        0      866 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.2.0/PKG-INFO
```

### Comparing `runweb-0.1.0/LICENSE` & `runweb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/README.md` & `runweb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/pyproject.toml` & `runweb-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "click>=8.1.3",
 ]
 description = "Run web server with one command."
 dynamic = []
 name = "runweb"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 tui = [
     "trogon>=0.4.0",
```

### Comparing `runweb-0.1.0/runweb/main.py` & `runweb-0.2.0/runweb/main.py`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/runweb/multiprocess.py` & `runweb-0.2.0/runweb/multiprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,61 @@
-import multiprocessing
 import os
 import signal
 import threading
 from multiprocessing.context import SpawnProcess
 from typing import Callable
 
 import click
 
-multiprocessing.allow_connection_pickling()
-
 
 def multiprocess(workers_num: int, create_process: Callable[[], SpawnProcess]) -> None:
     should_exit = threading.Event()
 
     click.echo(
         "Started parent process [{}]".format(
             click.style(str(os.getpid()), fg="cyan", bold=True)
         )
     )
 
     for sig in (
         signal.SIGINT,  # Sent by Ctrl+C.
-        signal.SIGTERM,  # Sent by `kill <pid>`.
+        signal.SIGTERM  # Sent by `kill <pid>`. Not sent on Windows.
+        if os.name != "nt"
+        else signal.SIGBREAK,  # Sent by `Ctrl+Break` on Windows.
     ):
         signal.signal(sig, lambda sig, frame: should_exit.set())
 
     processes: list[SpawnProcess] = []
-    for _ in range(workers_num):
+
+    def create_child() -> SpawnProcess:
         process = create_process()
         processes.append(process)
         process.start()
         click.echo(
             "Started child process [{}]".format(
                 click.style(str(process.pid), fg="cyan", bold=True)
             )
         )
+        return process
+
+    for _ in range(workers_num):
+        create_child()
 
     while not should_exit.wait(0.5):
         for idx, process in enumerate(tuple(processes)):
             if process.is_alive():
                 continue
 
             click.echo(
                 "Child process [{}] died unexpectedly".format(
                     click.style(str(process.pid), fg="cyan", bold=True)
                 )
             )
             del processes[idx]
-            process = create_process()
-            processes.append(process)
-            process.start()
-            click.echo(
-                "Started child process [{}]".format(
-                    click.style(str(process.pid), fg="cyan", bold=True)
-                )
-            )
-
-    click.echo(
-        "Stopping parent process [{}]".format(
-            click.style(str(os.getpid()), fg="cyan", bold=True)
-        )
-    )
+            create_child()
 
     for process in processes:
         if process.pid is None:
             continue
 
         if os.name == "nt":
             # Windows doesn't support SIGTERM.
@@ -75,7 +66,13 @@
     for process in processes:
         click.echo(
             "Waiting for child process [{}] to terminate".format(
                 click.style(str(process.pid), fg="cyan", bold=True)
             )
         )
         process.join()
+
+    click.echo(
+        "Stopped parent process [{}]".format(
+            click.style(str(os.getpid()), fg="cyan", bold=True)
+        )
+    )
```

### Comparing `runweb-0.1.0/runweb/parse.py` & `runweb-0.2.0/runweb/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     if not 0 < port < 65536:
         raise click.BadParameter("Bind port must be between 0 and 65536")
 
     address = ipaddress.ip_address(host)
     sock = socket.socket(
         socket.AF_INET if address.version == 4 else socket.AF_INET6, socket.SOCK_STREAM
     )
+    if os.name != "nt":
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+    else:  # In windows, SO_REUSEPORT is not available
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.bind((str(address), port))
     return sock
 
 
 def parse_application(value) -> Any:
     module_str, _, attrs_str = value.partition(":")
     if not module_str or not attrs_str:
```

### Comparing `runweb-0.1.0/runweb/runner/uvicorn.py` & `runweb-0.2.0/runweb/runner/uvicorn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import multiprocessing
-import socket
 
 from typing import Any, Union
 
 from uvicorn import Server, Config
 
 from ..parse import parse_application, parse_bind
 from ..multiprocess import multiprocess
 
 spawn = multiprocessing.get_context("spawn")
 
 
-def singleprocess(application: Any, bind: socket.socket) -> None:
+def singleprocess(application: Any, bind_address: str) -> None:
     config = Config(application)
     server = Server(config)
-    server.run([bind])
+    server.run([parse_bind(bind_address)])
 
 
 def asgi(bind_address: str, application: str, workers_num: Union[int, None]) -> None:
     callback = parse_application(application)
-    bind_socket = parse_bind(bind_address)
+    parse_bind(bind_address).close()
 
     if workers_num is None:
-        singleprocess(callback, bind_socket)
+        singleprocess(callback, bind_address)
     else:
-
-        def create_process():
-            process = spawn.Process(target=singleprocess, args=(callback, bind_socket))
-            return process
-
-        multiprocess(workers_num, create_process)
+        multiprocess(
+            workers_num,
+            lambda: spawn.Process(target=singleprocess, args=(callback, bind_address)),
+        )
```

### Comparing `runweb-0.1.0/runweb/runner/waitress.py` & `runweb-0.2.0/runweb/runner/waitress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import multiprocessing
-import socket
 
 from typing import Any, Union
 
 from waitress import create_server
 
 from ..parse import parse_application, parse_bind
 from ..multiprocess import multiprocess
 
 spawn = multiprocessing.get_context("spawn")
 
 
-def singleprocess(application: Any, bind: socket.socket) -> None:
-    server = create_server(application, sockets=[bind])
+def singleprocess(application: Any, bind_address: str) -> None:
+    server = create_server(application, sockets=[parse_bind(bind_address)])
     server.run()
 
 
 def wsgi(bind_address: str, application: str, workers_num: Union[int, None]) -> None:
     callback = parse_application(application)
-    bind_socket = parse_bind(bind_address)
+    parse_bind(bind_address).close()
 
     if workers_num is None:
-        singleprocess(callback, bind_socket)
+        singleprocess(callback, bind_address)
     else:
-
-        def create_process():
-            process = spawn.Process(target=singleprocess, args=(callback, bind_socket))
-            return process
-
-        multiprocess(workers_num, create_process)
+        multiprocess(
+            workers_num,
+            lambda: spawn.Process(target=singleprocess, args=(callback, bind_address)),
+        )
```

### Comparing `runweb-0.1.0/tests/test_uvicorn.py` & `runweb-0.2.0/tests/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/tests/test_waitress.py` & `runweb-0.2.0/tests/test_waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/tests/utils.py` & `runweb-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `runweb-0.1.0/PKG-INFO` & `runweb-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runweb
-Version: 0.1.0
+Version: 0.2.0
 Summary: Run web server with one command.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
 Requires-Dist: trogon>=0.4.0; extra == "tui"
 Requires-Dist: waitress; extra == "waitress"
```

