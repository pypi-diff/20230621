# Comparing `tmp/metlo-0.1.0.tar.gz` & `tmp/metlo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-umkol9th/metlo-0.1.0.tar", last modified: Wed Jun 21 02:58:52 2023, max compression
+gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-_70q7hhx/metlo-0.1.1.tar", last modified: Wed Jun 21 17:26:55 2023, max compression
```

## Comparing `metlo-0.1.0.tar` & `metlo-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 02:58:52.000000 metlo-0.1.0/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.0/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.0/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/django.py
--rw-r--r--   0 akshay     (501) staff       (20)    21150 2023-06-21 02:34:12.000000 metlo-0.1.0/metlo/fastapi.py
--rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/flask.py
--rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.0/pyproject.toml
--rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 02:58:52.000000 metlo-0.1.0/setup.cfg
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 17:26:55.000000 metlo-0.1.1/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.1/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.1/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/django.py
+-rw-r--r--   0 akshay     (501) staff       (20)    21350 2023-06-21 17:25:51.000000 metlo-0.1.1/metlo/fastapi.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/flask.py
+-rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.1/pyproject.toml
+-rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 17:26:55.000000 metlo-0.1.1/setup.cfg
```

### Comparing `metlo-0.1.0/PKG-INFO` & `metlo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.0/README.md` & `metlo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `metlo-0.1.0/metlo/django.py` & `metlo-0.1.1/metlo/django.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.0/metlo/fastapi.py` & `metlo-0.1.1/metlo/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,21 +342,27 @@
 
             async def rec_wrapper():
                 return await self.receivefn(scope, receive, send)
 
             async def send_wrapper(message):
                 await self.sendfn(scope, send, message)
 
-            if "http" in scope["type"]:
-                if self.check_blocking(scope):
-                    set_value_in_state("rejected", True, scope)
-                    await self.process_rejection(scope, receive, send_wrapper)
-                else:
-                    await self.app(scope, rec_wrapper, send_wrapper)
-                return
+            try:
+                if "http" in scope["type"]:
+                    if self.check_blocking(scope):
+                        set_value_in_state("rejected", True, scope)
+                        await self.process_rejection(scope, receive, send_wrapper)
+                    else:
+                        await self.app(scope, rec_wrapper, send_wrapper)
+                    return
+            except Exception as e:
+                self.logger.error(
+                    "Metlo encountered an error while checking for blocking requests"
+                )
+                self.logger.error(e)
 
         await self.app(scope, receive, send)
 
     async def receivefn(self, scope: Scope, receive: Receive, send: Send) -> None:
         # Receive this part of the request body
         req = await receive()
         # Check if we're processing http requests, websockets are currently not supported
@@ -417,17 +423,15 @@
                         scope,
                     )
             except Exception as e:
                 self.logger.error(
                     "Encountered an error while processing http request. Processing as normal"
                 )
                 self.logger.error(e)
-            return req
-        elif "websocket" in req["type"]:
-            return req
+            return req        
         else:
             return req
 
     async def sendfn(self, scope: Scope, send: Send, message: Message) -> None:
         if "http" in message["type"]:
             try:
                 # We received http response start. Can record status and headers from this
```

### Comparing `metlo-0.1.0/metlo/flask.py` & `metlo-0.1.1/metlo/flask.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.0/metlo.egg-info/PKG-INFO` & `metlo-0.1.1/metlo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.0/setup.cfg` & `metlo-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metlo
-version = 0.1.0
+version = 0.1.1
 description = The Python Agent for Metlo
 long_description = file: README.md
 long_description_content_type = text/markdown
 repository = https://github.com/metlo-labs/metlo
 url = https://www.metlo.com
 license = MIT
 project_urls =
```

