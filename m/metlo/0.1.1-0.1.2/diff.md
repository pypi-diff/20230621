# Comparing `tmp/metlo-0.1.1.tar.gz` & `tmp/metlo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-_70q7hhx/metlo-0.1.1.tar", last modified: Wed Jun 21 17:26:55 2023, max compression
+gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-62r3kicq/metlo-0.1.2.tar", last modified: Wed Jun 21 18:29:27 2023, max compression
```

## Comparing `metlo-0.1.1.tar` & `metlo-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 17:26:55.000000 metlo-0.1.1/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.1/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.1/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/django.py
--rw-r--r--   0 akshay     (501) staff       (20)    21350 2023-06-21 17:25:51.000000 metlo-0.1.1/metlo/fastapi.py
--rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/flask.py
--rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.1/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 17:26:55.000000 metlo-0.1.1/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.1/pyproject.toml
--rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 17:26:55.000000 metlo-0.1.1/setup.cfg
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 18:29:27.000000 metlo-0.1.2/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.2/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.2/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/django.py
+-rw-r--r--   0 akshay     (501) staff       (20)    21704 2023-06-21 18:28:46.000000 metlo-0.1.2/metlo/fastapi.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/flask.py
+-rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.2/pyproject.toml
+-rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 18:29:27.000000 metlo-0.1.2/setup.cfg
```

### Comparing `metlo-0.1.1/PKG-INFO` & `metlo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.1/README.md` & `metlo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `metlo-0.1.1/metlo/django.py` & `metlo-0.1.2/metlo/django.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.1/metlo/fastapi.py` & `metlo-0.1.2/metlo/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,50 +279,57 @@
                 if "api_host" in settings:
                     if (settings["api_host"] is not None) and isinstance(
                         settings["api_host"], str
                     ):
                         self.api_host = settings["api_host"]
                     else:
                         self.api_host = None
-                        self.logger.error(
+                        self.logger.warn(
                             "Metlo api_host arg is incorrectly specified. Defaulting to value from connection"
                         )
                 else:
                     self.api_host = None
 
                 # Get User
-                if (
-                    "get_user" in settings
-                    and callable(settings["get_user"])
-                    and not iscoroutinefunction(settings["get_user"])
-                ):
-                    self.get_user = settings["get_user"]
+                if "get_user" in settings:
+                    if callable(settings["get_user"]) and not iscoroutinefunction(
+                        settings["get_user"]
+                    ):
+                        self.get_user = settings["get_user"]
+                    else:
+                        self.logger.warn(
+                            "Metlo get_user arg is incorrectly specified or unspecified. Require a synchronous function returning a string"
+                        )
+                        self.get_user = None
                 else:
-                    self.logger.warn(
-                        "Metlo get_user arg is incorrectly specified or unspecified. Require a synchronous function returning a string"
-                    )
                     self.get_user = None
 
                 # Reject Response
-                if (
-                    "reject_response" in settings
-                    and callable(settings["reject_response"])
-                    and not iscoroutinefunction(settings["reject_response"])
-                ):
-                    self.reject_response = settings["reject_response"]
+                if "reject_response" in settings:
+                    if callable(
+                        settings["reject_response"]
+                    ) and not iscoroutinefunction(settings["reject_response"]):
+                        self.reject_response = settings["reject_response"]
+                    else:
+                        self.logger.warn(
+                            "Metlo reject_response arg is incorrectly specified or unspecified. Require a synchronous function returning a Response subclass"
+                        )
+                        self.reject_response = None
                 else:
-                    self.logger.warn(
-                        "Metlo reject_response arg is incorrectly specified or unspecified. Require a synchronous function returning a Response subclass"
-                    )
                     self.reject_response = None
 
-                if "max_body" in settings and isinstance(settings["max_body"], int):
-                    self.max_body = settings["max_body"]
+                if "max_body" in settings:
+                    if isinstance(settings["max_body"], int):
+                        self.max_body = settings["max_body"]
+                    else:
+                        self.logger.warn(
+                            "Could not read passed body size. Metlo will be using the default body capture size"
+                        )
+                        self.max_body = DEFAULT_BODY_SIZE
                 else:
-                    self.logger.debug("Metlo using default body capture size")
                     self.max_body = DEFAULT_BODY_SIZE
 
                 can_start = False
                 try:
                     if shouldStart:
                         metlo_python_agent_bindings_common.setup(
                             self.host, self.key, **params
@@ -423,15 +430,15 @@
                         scope,
                     )
             except Exception as e:
                 self.logger.error(
                     "Encountered an error while processing http request. Processing as normal"
                 )
                 self.logger.error(e)
-            return req        
+            return req
         else:
             return req
 
     async def sendfn(self, scope: Scope, send: Send, message: Message) -> None:
         if "http" in message["type"]:
             try:
                 # We received http response start. Can record status and headers from this
```

### Comparing `metlo-0.1.1/metlo/flask.py` & `metlo-0.1.2/metlo/flask.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.1/metlo.egg-info/PKG-INFO` & `metlo-0.1.2/metlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.1/setup.cfg` & `metlo-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metlo
-version = 0.1.1
+version = 0.1.2
 description = The Python Agent for Metlo
 long_description = file: README.md
 long_description_content_type = text/markdown
 repository = https://github.com/metlo-labs/metlo
 url = https://www.metlo.com
 license = MIT
 project_urls =
```

