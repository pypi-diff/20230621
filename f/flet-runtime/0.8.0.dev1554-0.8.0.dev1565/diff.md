# Comparing `tmp/flet_runtime-0.8.0.dev1554.tar.gz` & `tmp/flet_runtime-0.8.0.dev1565.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.8.0.dev1554.tar", max compression
+gzip compressed data, was "flet_runtime-0.8.0.dev1565.tar", max compression
```

## Comparing `flet_runtime-0.8.0.dev1554.tar` & `flet_runtime-0.8.0.dev1565.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      204 2023-06-19 04:40:36.662001 flet_runtime-0.8.0.dev1554/README.md
--rw-r--r--   0        0        0      747 2023-06-19 04:41:06.657593 flet_runtime-0.8.0.dev1554/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-19 04:40:36.662001 flet_runtime-0.8.0.dev1554/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    23064 2023-06-19 04:40:36.662001 flet_runtime-0.8.0.dev1554/src/flet_runtime/app.py
--rw-r--r--   0        0        0     6309 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/async_local_socket_connection.py
--rw-r--r--   0        0        0      252 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0     9107 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1515 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0    10255 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/pubsub.py
--rw-r--r--   0        0        0     6934 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/sync_local_socket_connection.py
--rw-r--r--   0        0        0     3593 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/utils.py
--rw-r--r--   0        0        0      103 2023-06-19 04:40:36.666001 flet_runtime-0.8.0.dev1554/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1554/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/README.md
+-rw-r--r--   0        0        0      747 2023-06-21 16:21:49.315894 flet_runtime-0.8.0.dev1565/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    23672 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/app.py
+-rw-r--r--   0        0        0     6309 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/async_local_socket_connection.py
+-rw-r--r--   0        0        0      252 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0     9107 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1515 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0    10255 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/pubsub.py
+-rw-r--r--   0        0        0     6934 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     3593 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/utils.py
+-rw-r--r--   0        0        0      103 2023-06-21 16:21:15.972190 flet_runtime-0.8.0.dev1565/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1565/PKG-INFO
```

### Comparing `flet_runtime-0.8.0.dev1554/pyproject.toml` & `flet_runtime-0.8.0.dev1565/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-runtime"
-version = "0.8.0.dev1554"
+version = "0.8.0.dev1565"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1554"
+flet-core = "0.8.0.dev1565"
 python = "^3.7"
 oauthlib = "^3.2.2"
 httpx = "^0.24.1"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/app.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     WEB_BROWSER,
     AppView,
     WebRenderer,
 )
 from flet_core.event import Event
 from flet_core.page import Page
 from flet_core.utils import is_coroutine, random_string
-from flet_runtime import version
 from flet_runtime.async_local_socket_connection import AsyncLocalSocketConnection
 from flet_runtime.sync_local_socket_connection import SyncLocalSocketConnection
 from flet_runtime.utils import (
     get_arch,
     get_current_script_dir,
     get_free_tcp_port,
     get_package_bin_dir,
@@ -53,24 +52,29 @@
     class AsyncWebSocketConnection(Connection):
         pass
 
     class SyncWebSocketConnection(Connection):
         pass
 
 
+try:
+    from flet import version
+except ImportError:
+    from flet_runtime import version
+
 logger = logging.getLogger(flet_runtime.__name__)
 
 
 def app(
     target,
     name="",
     host=None,
     port=0,
     view: Optional[AppView] = AppView.FLET_APP,
-    assets_dir=None,
+    assets_dir="assets",
     upload_dir=None,
     web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
     use_color_emoji=False,
     route_url_strategy="path",
     auth_token=None,
 ):
     if is_coroutine(target):
@@ -107,15 +111,15 @@
 
 def __app_sync(
     target,
     name="",
     host=None,
     port=0,
     view: Optional[AppView] = AppView.FLET_APP,
-    assets_dir=None,
+    assets_dir="assets",
     upload_dir=None,
     web_renderer: WebRenderer = WebRenderer.CANVAS_KIT,
     use_color_emoji=False,
     route_url_strategy="path",
     auth_token=None,
 ):
     if isinstance(view, str):
@@ -168,15 +172,17 @@
             or view == AppView.FLET_APP_WEB
         )
         and not is_linux_server()
         and not is_mobile()
         and url_prefix is None
     ):
         fvp, pid_file = open_flet_view(
-            conn.page_url, assets_dir, view == AppView.FLET_APP_HIDDEN
+            conn.page_url,
+            assets_dir if view != AppView.FLET_APP_WEB else None,
+            view == AppView.FLET_APP_HIDDEN,
         )
         try:
             fvp.wait()
         except Exception as e:
             pass
     else:
         if view == AppView.WEB_BROWSER and url_prefix is None:
@@ -255,15 +261,17 @@
             or view == AppView.FLET_APP_WEB
         )
         and not is_linux_server()
         and not is_mobile()
         and url_prefix is None
     ):
         fvp, pid_file = await open_flet_view_async(
-            conn.page_url, assets_dir, view == AppView.FLET_APP_HIDDEN
+            conn.page_url,
+            assets_dir if view != AppView.FLET_APP_WEB else None,
+            view == AppView.FLET_APP_HIDDEN,
         )
         try:
             await fvp.wait()
         except Exception as e:
             pass
     else:
         if view == AppView.WEB_BROWSER and url_prefix is None:
@@ -347,26 +355,28 @@
         except Exception as e:
             print(
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
             page.error(f"There was an error while processing your request: {e}")
 
+    env_page_name = os.getenv("FLET_PAGE_NAME")
+
     if is_socket_server:
         conn = SyncLocalSocketConnection(
             port,
             uds_path,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     else:
         assert server
         conn = SyncWebSocketConnection(
             server_address=server,
-            page_name=page_name,
+            page_name=env_page_name if not page_name and env_page_name else page_name,
             token=auth_token,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     conn.connect()
     return conn
 
@@ -429,26 +439,28 @@
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
             await page.error_async(
                 f"There was an error while processing your request: {e}"
             )
 
+    env_page_name = os.getenv("FLET_PAGE_NAME")
+
     if is_socket_server:
         conn = AsyncLocalSocketConnection(
             port,
             uds_path,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     else:
         assert server
         conn = AsyncWebSocketConnection(
             server_address=server,
-            page_name=page_name,
+            page_name=env_page_name if not page_name and env_page_name else page_name,
             auth_token=auth_token,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     await conn.connect()
     return conn
 
@@ -525,15 +537,21 @@
 
     if assets_dir:
         args.extend(["--assets-dir", assets_dir])
 
     creationflags = 0
     start_new_session = False
 
-    args.append("--attached")
+    if os.getenv("FLET_DETACH_FLETD") is None:
+        args.append("--attached")
+    else:
+        if is_windows():
+            creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
+        else:
+            start_new_session = True
 
     log_level = logging.getLogger(flet_runtime.__name__).getEffectiveLevel()
     if log_level == logging.CRITICAL:
         log_level = logging.FATAL
 
     if log_level != logging.NOTSET:
         log_level_name = logging.getLevelName(log_level).lower()
```

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/async_local_socket_connection.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/authorization.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/oauth_provider.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/oauth_token.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/pubsub.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/sync_local_socket_connection.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/src/flet_runtime/utils.py` & `flet_runtime-0.8.0.dev1565/src/flet_runtime/utils.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1554/PKG-INFO` & `flet_runtime-0.8.0.dev1565/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-runtime
-Version: 0.8.0.dev1554
+Version: 0.8.0.dev1565
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1554)
+Requires-Dist: flet-core (==0.8.0.dev1565)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```

