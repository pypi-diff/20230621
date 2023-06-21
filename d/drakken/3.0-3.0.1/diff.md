# Comparing `tmp/drakken-3.0.tar.gz` & `tmp/drakken-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakken-3.0.tar", last modified: Sun Mar 12 13:24:39 2023, max compression
+gzip compressed data, was "drakken-3.0.1.tar", last modified: Wed Jun 21 10:59:26 2023, max compression
```

## Comparing `drakken-3.0.tar` & `drakken-3.0.1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.453409 drakken-3.0/
--rw-r--r--   0 craighoward   (501) staff       (20)     1263 2023-03-12 13:21:19.000000 drakken-3.0/HISTORY
--rw-r--r--   0 craighoward   (501) staff       (20)     1073 2023-01-22 20:14:50.000000 drakken-3.0/LICENSE
--rw-r--r--   0 craighoward   (501) staff       (20)       39 2023-03-06 13:18:07.000000 drakken-3.0/MANIFEST.in
--rw-r--r--   0 craighoward   (501) staff       (20)     1661 2023-03-12 13:24:39.453724 drakken-3.0/PKG-INFO
--rw-r--r--   0 craighoward   (501) staff       (20)     1221 2023-02-03 16:03:37.000000 drakken-3.0/README
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.429080 drakken-3.0/demo/
--rw-r--r--   0 craighoward   (501) staff       (20)     6148 2023-01-26 11:37:59.000000 drakken-3.0/demo/.DS_Store
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.435559 drakken-3.0/demo/__pycache__/
--rw-r--r--   0 craighoward   (501) staff       (20)      716 2023-01-26 11:37:59.000000 drakken-3.0/demo/__pycache__/account.cpython-310.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)     1097 2023-02-27 13:01:04.000000 drakken-3.0/demo/__pycache__/account.cpython-311.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)      719 2023-01-26 11:37:59.000000 drakken-3.0/demo/__pycache__/accounts.cpython-310.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)      741 2023-01-26 11:37:59.000000 drakken-3.0/demo/__pycache__/accounts.cpython-39.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)     2421 2023-01-26 11:37:59.000000 drakken-3.0/demo/__pycache__/app.cpython-39.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)      483 2023-01-26 11:37:59.000000 drakken-3.0/demo/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 craighoward   (501) staff       (20)      399 2023-02-27 13:00:10.000000 drakken-3.0/demo/account.py
--rw-r--r--   0 craighoward   (501) staff       (20)     1798 2023-03-05 14:36:28.000000 drakken-3.0/demo/demo.py
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.420582 drakken-3.0/demo/static/
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.436322 drakken-3.0/demo/static/css/
--rw-r--r--   0 craighoward   (501) staff       (20)      119 2023-03-01 15:30:27.000000 drakken-3.0/demo/static/css/demo.css
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.438797 drakken-3.0/demo/templates/
--rw-r--r--   0 craighoward   (501) staff       (20)      317 2023-02-03 00:03:52.000000 drakken-3.0/demo/templates/base.html
--rw-r--r--   0 craighoward   (501) staff       (20)      245 2023-03-01 15:30:27.000000 drakken-3.0/demo/templates/main.html
--rw-r--r--   0 craighoward   (501) staff       (20)       30 2023-01-26 11:37:59.000000 drakken-3.0/demo/templates/robots.txt
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.445146 drakken-3.0/drakken/
--rw-r--r--   0 craighoward   (501) staff       (20)       21 2023-03-12 13:21:26.000000 drakken-3.0/drakken/__init__.py
--rw-r--r--   0 craighoward   (501) staff       (20)     1407 2023-03-06 17:20:38.000000 drakken-3.0/drakken/config.py
--rw-r--r--   0 craighoward   (501) staff       (20)     9106 2023-03-06 17:20:17.000000 drakken-3.0/drakken/core.py
--rw-r--r--   0 craighoward   (501) staff       (20)     1692 2023-02-14 19:51:52.000000 drakken-3.0/drakken/exceptions.py
--rw-r--r--   0 craighoward   (501) staff       (20)     2178 2023-03-06 17:19:52.000000 drakken-3.0/drakken/mail.py
--rw-r--r--   0 craighoward   (501) staff       (20)     2692 2023-03-10 20:46:25.000000 drakken-3.0/drakken/middleware.py
--rw-r--r--   0 craighoward   (501) staff       (20)    12257 2023-03-10 13:55:11.000000 drakken-3.0/drakken/model.py
--rw-r--r--   0 craighoward   (501) staff       (20)     3109 2023-03-12 13:21:48.000000 drakken-3.0/drakken/rate_limit.py
--rw-r--r--   0 craighoward   (501) staff       (20)     2409 2023-03-06 17:38:20.000000 drakken-3.0/drakken/security.py
--rw-r--r--   0 craighoward   (501) staff       (20)     2726 2023-03-06 17:39:20.000000 drakken-3.0/drakken/template.py
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.446813 drakken-3.0/drakken.egg-info/
--rw-r--r--   0 craighoward   (501) staff       (20)     1661 2023-03-12 13:24:39.000000 drakken-3.0/drakken.egg-info/PKG-INFO
--rw-r--r--   0 craighoward   (501) staff       (20)     1002 2023-03-12 13:24:39.000000 drakken-3.0/drakken.egg-info/SOURCES.txt
--rw-r--r--   0 craighoward   (501) staff       (20)        1 2023-03-12 13:24:39.000000 drakken-3.0/drakken.egg-info/dependency_links.txt
--rw-r--r--   0 craighoward   (501) staff       (20)       65 2023-03-12 13:24:39.000000 drakken-3.0/drakken.egg-info/requires.txt
--rw-r--r--   0 craighoward   (501) staff       (20)       13 2023-03-12 13:24:39.000000 drakken-3.0/drakken.egg-info/top_level.txt
--rw-r--r--   0 craighoward   (501) staff       (20)       81 2023-02-03 13:32:00.000000 drakken-3.0/pyproject.toml
--rw-r--r--   0 craighoward   (501) staff       (20)      641 2023-03-12 13:24:39.454813 drakken-3.0/setup.cfg
-drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-03-12 13:24:39.452319 drakken-3.0/test/
--rw-r--r--   0 craighoward   (501) staff       (20)        0 2023-01-26 11:37:59.000000 drakken-3.0/test/__init__.py
--rw-r--r--   0 craighoward   (501) staff       (20)      994 2023-03-06 17:42:45.000000 drakken-3.0/test/test_config.py
--rw-r--r--   0 craighoward   (501) staff       (20)     6759 2023-03-05 14:40:28.000000 drakken-3.0/test/test_core.py
--rw-r--r--   0 craighoward   (501) staff       (20)     5299 2023-03-01 15:30:27.000000 drakken-3.0/test/test_mail.py
--rw-r--r--   0 craighoward   (501) staff       (20)     3306 2023-02-26 07:46:46.000000 drakken-3.0/test/test_middleware.py
--rw-r--r--   0 craighoward   (501) staff       (20)     5388 2023-03-02 01:58:08.000000 drakken-3.0/test/test_named_route.py
--rw-r--r--   0 craighoward   (501) staff       (20)     5598 2023-03-06 17:48:23.000000 drakken-3.0/test/test_rate_limit.py
--rw-r--r--   0 craighoward   (501) staff       (20)     1070 2023-03-06 17:48:30.000000 drakken-3.0/test/test_security.py
--rw-r--r--   0 craighoward   (501) staff       (20)    15149 2023-02-25 21:33:46.000000 drakken-3.0/test/test_session.py
--rw-r--r--   0 craighoward   (501) staff       (20)     3425 2023-02-26 12:25:06.000000 drakken-3.0/test/test_template.py
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.929427 drakken-3.0.1/
+-rw-r--r--   0 craighoward   (501) staff       (20)     1359 2023-06-20 12:06:21.000000 drakken-3.0.1/HISTORY
+-rw-r--r--   0 craighoward   (501) staff       (20)     1073 2023-06-14 19:24:48.000000 drakken-3.0.1/LICENSE
+-rw-r--r--   0 craighoward   (501) staff       (20)       39 2023-03-06 13:18:07.000000 drakken-3.0.1/MANIFEST.in
+-rw-r--r--   0 craighoward   (501) staff       (20)     1663 2023-06-21 10:59:26.929617 drakken-3.0.1/PKG-INFO
+-rw-r--r--   0 craighoward   (501) staff       (20)     1221 2023-02-03 16:03:37.000000 drakken-3.0.1/README
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.896328 drakken-3.0.1/demo/
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.903071 drakken-3.0.1/demo/__pycache__/
+-rw-r--r--   0 craighoward   (501) staff       (20)      716 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/__pycache__/account.cpython-310.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)     1097 2023-02-27 13:01:04.000000 drakken-3.0.1/demo/__pycache__/account.cpython-311.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)      719 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/__pycache__/accounts.cpython-310.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)      741 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/__pycache__/accounts.cpython-39.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)     2421 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/__pycache__/app.cpython-39.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)      483 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 craighoward   (501) staff       (20)      399 2023-02-27 13:00:10.000000 drakken-3.0.1/demo/account.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     1798 2023-03-05 14:36:28.000000 drakken-3.0.1/demo/demo.py
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.887813 drakken-3.0.1/demo/static/
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.904000 drakken-3.0.1/demo/static/css/
+-rw-r--r--   0 craighoward   (501) staff       (20)      119 2023-03-01 15:30:27.000000 drakken-3.0.1/demo/static/css/demo.css
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.906724 drakken-3.0.1/demo/templates/
+-rw-r--r--   0 craighoward   (501) staff       (20)      317 2023-02-03 00:03:52.000000 drakken-3.0.1/demo/templates/base.html
+-rw-r--r--   0 craighoward   (501) staff       (20)      245 2023-03-01 15:30:27.000000 drakken-3.0.1/demo/templates/main.html
+-rw-r--r--   0 craighoward   (501) staff       (20)       30 2023-01-26 11:37:59.000000 drakken-3.0.1/demo/templates/robots.txt
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.915510 drakken-3.0.1/drakken/
+-rw-r--r--   0 craighoward   (501) staff       (20)       23 2023-06-20 12:06:21.000000 drakken-3.0.1/drakken/__init__.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     1407 2023-03-06 17:20:38.000000 drakken-3.0.1/drakken/config.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     9341 2023-06-20 12:06:21.000000 drakken-3.0.1/drakken/core.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     1692 2023-02-14 19:51:52.000000 drakken-3.0.1/drakken/exceptions.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     2178 2023-03-06 17:19:52.000000 drakken-3.0.1/drakken/mail.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     2692 2023-03-28 18:09:32.000000 drakken-3.0.1/drakken/middleware.py
+-rw-r--r--   0 craighoward   (501) staff       (20)    12283 2023-03-28 18:09:50.000000 drakken-3.0.1/drakken/model.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     3109 2023-03-28 18:09:50.000000 drakken-3.0.1/drakken/rate_limit.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     2409 2023-03-06 17:38:20.000000 drakken-3.0.1/drakken/security.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     2726 2023-03-06 17:39:20.000000 drakken-3.0.1/drakken/template.py
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.919369 drakken-3.0.1/drakken.egg-info/
+-rw-r--r--   0 craighoward   (501) staff       (20)     1663 2023-06-21 10:59:26.000000 drakken-3.0.1/drakken.egg-info/PKG-INFO
+-rw-r--r--   0 craighoward   (501) staff       (20)      987 2023-06-21 10:59:26.000000 drakken-3.0.1/drakken.egg-info/SOURCES.txt
+-rw-r--r--   0 craighoward   (501) staff       (20)        1 2023-06-21 10:59:26.000000 drakken-3.0.1/drakken.egg-info/dependency_links.txt
+-rw-r--r--   0 craighoward   (501) staff       (20)       65 2023-06-21 10:59:26.000000 drakken-3.0.1/drakken.egg-info/requires.txt
+-rw-r--r--   0 craighoward   (501) staff       (20)       13 2023-06-21 10:59:26.000000 drakken-3.0.1/drakken.egg-info/top_level.txt
+-rw-r--r--   0 craighoward   (501) staff       (20)       81 2023-02-03 13:32:00.000000 drakken-3.0.1/pyproject.toml
+-rw-r--r--   0 craighoward   (501) staff       (20)      641 2023-06-21 10:59:26.930656 drakken-3.0.1/setup.cfg
+drwxr-xr-x   0 craighoward   (501) staff       (20)        0 2023-06-21 10:59:26.928725 drakken-3.0.1/test/
+-rw-r--r--   0 craighoward   (501) staff       (20)        0 2023-01-26 11:37:59.000000 drakken-3.0.1/test/__init__.py
+-rw-r--r--   0 craighoward   (501) staff       (20)      994 2023-03-06 17:42:45.000000 drakken-3.0.1/test/test_config.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     8966 2023-06-20 12:06:21.000000 drakken-3.0.1/test/test_core.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     5299 2023-03-01 15:30:27.000000 drakken-3.0.1/test/test_mail.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     3306 2023-02-26 07:46:46.000000 drakken-3.0.1/test/test_middleware.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     5388 2023-03-02 01:58:08.000000 drakken-3.0.1/test/test_named_route.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     5598 2023-03-06 17:48:23.000000 drakken-3.0.1/test/test_rate_limit.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     1070 2023-03-06 17:48:30.000000 drakken-3.0.1/test/test_security.py
+-rw-r--r--   0 craighoward   (501) staff       (20)    15149 2023-02-25 21:33:46.000000 drakken-3.0.1/test/test_session.py
+-rw-r--r--   0 craighoward   (501) staff       (20)     3425 2023-02-26 12:25:06.000000 drakken-3.0.1/test/test_template.py
```

### Comparing `drakken-3.0/HISTORY` & `drakken-3.0.1/HISTORY`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Drakken release history
 
-## 2023-03-12
+## 3.0.1 - 2023-06-20
+- FIX: ${STATIC} variable can be a relative or absolute file path.
+
+## 3.0 - 2023-03-12
 - ADD: 301 redirect if URL is missing a trailing slash or added one.
 - ADD: email handler.
 - ADD: send email to admins on 500 error.
 - ADD: rate limiter to prevent email floods.
 - ADD: named URLs.
 - ADD: support JSON and YAML config files.
 - CHANGE: drakken.config.read_file() -> drakken.config.load().
```

### Comparing `drakken-3.0/LICENSE` & `drakken-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drakken-3.0/PKG-INFO` & `drakken-3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakken
-Version: 3.0
+Version: 3.0.1
 Summary: Python web framework
 Home-page: https://seagrape.us/drakken.html
 Author: Craig Howard
 Author-email: craig@seagrape.us
 License: MIT
 Keywords: Minimalist Python web framework
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drakken-3.0/README` & `drakken-3.0.1/README`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/__pycache__/account.cpython-310.pyc` & `drakken-3.0.1/demo/__pycache__/account.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/__pycache__/account.cpython-311.pyc` & `drakken-3.0.1/demo/__pycache__/account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/__pycache__/accounts.cpython-310.pyc` & `drakken-3.0.1/demo/__pycache__/accounts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/__pycache__/accounts.cpython-39.pyc` & `drakken-3.0.1/demo/__pycache__/accounts.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/__pycache__/app.cpython-39.pyc` & `drakken-3.0.1/demo/__pycache__/app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drakken-3.0/demo/demo.py` & `drakken-3.0.1/demo/demo.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/config.py` & `drakken-3.0.1/drakken/config.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/core.py` & `drakken-3.0.1/drakken/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 logger = logging.getLogger(__name__)
 
 
 class Drakken:
     """The Drakken Application class."""
 
     def __init__(self):
+        """Initialize Drakken application."""
         self.routes = {}
         self.named_routes = {}
         # Middleware wraps around self (the application).
         self.middleware = Middleware(self)
 
     def __call__(self, environ, start_response):
         """WSGI API.
@@ -106,26 +107,31 @@
         Args:
             middleware: subclass of drakken.middleware.Middleware.
         """
         self.middleware.add(middleware)
 
     def _serve_static_file(self, request, response):
         """Serve static file."""
-        fpath = os.path.join(os.getcwd(), request.path[1:])
-        if os.path.exists(fpath):
+        # Absolute path: use as is.
+        if os.path.exists(request.path):
+            fpath = request.path
+        # Relative path: convert to absolute path.
+        else:
+            fpath = os.path.abspath(request.path[1:])
+        try:
             ftype = mimetypes.guess_type(fpath)[0]
             response.content_type = ftype
             if ftype in TEXT_FILE_TYPES:
                 with io.open(fpath, 'r', encoding='ISO-8859-1') as f:
                     response.text = f.read()
             else:
                 with io.open(fpath, 'rb') as f:
                     response.body = f.read()
             return response
-        else:
+        except (FileNotFoundError, IsADirectoryError):
             raise NotFound
 
     def _not_found(self, response):
         """Return 404 response."""
         response.status_code = 404
         template_path = os.path.join(
             config.get('TEMPLATE_DIR'),
```

### Comparing `drakken-3.0/drakken/exceptions.py` & `drakken-3.0.1/drakken/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/mail.py` & `drakken-3.0.1/drakken/mail.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/middleware.py` & `drakken-3.0.1/drakken/middleware.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/model.py` & `drakken-3.0.1/drakken/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     return user
 
 
 def authenticate(**kwargs):
     """Authenticate user.
 
     Args:
+        username: string.
         email: string.
         password: string.
 
     Raises:
         AuthenticateFail: username/email and password don't match the
         database.
     """
```

### Comparing `drakken-3.0/drakken/rate_limit.py` & `drakken-3.0.1/drakken/rate_limit.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/security.py` & `drakken-3.0.1/drakken/security.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken/template.py` & `drakken-3.0.1/drakken/template.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/drakken.egg-info/PKG-INFO` & `drakken-3.0.1/drakken.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakken
-Version: 3.0
+Version: 3.0.1
 Summary: Python web framework
 Home-page: https://seagrape.us/drakken.html
 Author: Craig Howard
 Author-email: craig@seagrape.us
 License: MIT
 Keywords: Minimalist Python web framework
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drakken-3.0/drakken.egg-info/SOURCES.txt` & `drakken-3.0.1/drakken.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 HISTORY
 LICENSE
 MANIFEST.in
 README
 pyproject.toml
 setup.cfg
-demo/.DS_Store
 demo/account.py
 demo/demo.py
 demo/__pycache__/account.cpython-310.pyc
 demo/__pycache__/account.cpython-311.pyc
 demo/__pycache__/accounts.cpython-310.pyc
 demo/__pycache__/accounts.cpython-39.pyc
 demo/__pycache__/app.cpython-39.pyc
```

### Comparing `drakken-3.0/setup.cfg` & `drakken-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_config.py` & `drakken-3.0.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_core.py` & `drakken-3.0.1/test/test_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import logging
 import os
 import tempfile
 import unittest
 
 import requests
 from wsgiadapter import WSGIAdapter  # from requests-wsgi-adapter
@@ -145,14 +146,79 @@
         url = 'http://testserver/%ff'
         self.assertEqual(self.client.get(url).status_code, 400)
 
     def tearDown(self):
         logging.disable(logging.NOTSET)
 
 
+class TestStaticFiles(unittest.TestCase):
+    def setUp(self):
+        self.app = Drakken()
+        self.client = requests.Session()
+        self.client.mount(
+            prefix='http://testserver',
+            adapter=WSGIAdapter(
+                self.app))
+        logging.disable(logging.WARNING)
+        self.dir = tempfile.TemporaryDirectory()
+        self.local_dir = tempfile.TemporaryDirectory(dir=os.getcwd())
+
+    def test_absolute_path(self):
+        fpath = os.path.join(self.dir.name, 'hello.txt')
+        with io.open(fpath, 'wb') as f:
+            f.write(b'Hello world')
+        cfg = {'STATIC_DIR': self.dir.name}
+        loads(cfg)
+
+        furl = f'http://testserver{fpath}'
+        response = self.client.get(furl)
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.text, 'Hello world')
+
+    def test_relative_path(self):
+        fpath = os.path.join(self.local_dir.name, 'hello.txt')
+        with io.open(fpath, 'wb') as f:
+            f.write(b'Hello world')
+        spath = os.path.split(self.local_dir.name)[1]
+        cfg = {'STATIC_DIR': spath}
+        loads(cfg)
+
+        furl = os.path.join('http://testserver', spath, 'hello.txt')
+        response = self.client.get(furl)
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.text, 'Hello world')
+
+    def test_no_file(self):
+        fpath = os.path.join(self.dir.name, 'hello.txt')
+        cfg = {'STATIC_DIR': self.dir.name}
+        loads(cfg)
+
+        furl = f'http://testserver{fpath}'
+        response = self.client.get(furl)
+        self.assertEqual(response.status_code, 404)
+
+    def test_directory(self):
+        # Client asks for a directory. Written for production bugfix.
+        fpath = os.path.join(self.dir.name, 'my-dir')
+        os.makedirs(fpath)
+        cfg = {'STATIC_DIR': self.dir.name}
+        loads(cfg)
+
+        furl = f'http://testserver{fpath}'
+        response = self.client.get(furl)
+        self.assertEqual(response.status_code, 404)
+
+    def tearDown(self):
+        self.dir.cleanup()
+        self.local_dir.cleanup()
+        logging.disable(logging.NOTSET)
+        cfg = {'STATIC_DIR': 'static'}
+        loads(cfg)
+
+
 class TestTrailingSlashRedirect(unittest.TestCase):
     def setUp(self):
         self.app = Drakken()
         self.client = requests.Session()
         self.client.mount(
             prefix='http://testserver',
             adapter=WSGIAdapter(
```

### Comparing `drakken-3.0/test/test_mail.py` & `drakken-3.0.1/test/test_mail.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_middleware.py` & `drakken-3.0.1/test/test_middleware.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_named_route.py` & `drakken-3.0.1/test/test_named_route.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_rate_limit.py` & `drakken-3.0.1/test/test_rate_limit.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_security.py` & `drakken-3.0.1/test/test_security.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_session.py` & `drakken-3.0.1/test/test_session.py`

 * *Files identical despite different names*

### Comparing `drakken-3.0/test/test_template.py` & `drakken-3.0.1/test/test_template.py`

 * *Files identical despite different names*

