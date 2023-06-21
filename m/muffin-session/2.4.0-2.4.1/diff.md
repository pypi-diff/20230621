# Comparing `tmp/muffin_session-2.4.0.tar.gz` & `tmp/muffin_session-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_session-2.4.0.tar", max compression
+gzip compressed data, was "muffin_session-2.4.1.tar", max compression
```

## Comparing `muffin_session-2.4.0.tar` & `muffin_session-2.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6162 2023-04-04 06:02:50.676706 muffin_session-2.4.0/README.rst
--rw-r--r--   0        0        0     7668 2023-04-04 06:02:50.676706 muffin_session-2.4.0/muffin_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 06:02:50.676706 muffin_session-2.4.0/muffin_session/py.typed
--rw-r--r--   0        0        0     2089 2023-04-04 06:02:50.676706 muffin_session-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     7621 1970-01-01 00:00:00.000000 muffin_session-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6162 2023-06-21 06:41:31.113701 muffin_session-2.4.1/README.rst
+-rw-r--r--   0        0        0     7668 2023-06-21 06:41:31.113701 muffin_session-2.4.1/muffin_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:41:31.113701 muffin_session-2.4.1/muffin_session/py.typed
+-rw-r--r--   0        0        0     2143 2023-06-21 06:41:31.113701 muffin_session-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7351 1970-01-01 00:00:00.000000 muffin_session-2.4.1/PKG-INFO
```

### Comparing `muffin_session-2.4.0/README.rst` & `muffin_session-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_session-2.4.0/muffin_session/__init__.py` & `muffin_session-2.4.1/muffin_session/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_session-2.4.0/pyproject.toml` & `muffin_session-2.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-session"
-version = "2.4.0"
+version = "2.4.1"
 description = "Signed Cookie-Based HTTP sessions for the Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-session"
 repository = "https://github.com/klen/muffin-session"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["asyncio", "trio", "asgi", "muffin", "web", "cookie", "sessions", "session"]
@@ -22,32 +22,32 @@
   "Framework :: AsyncIO",
   "Framework :: Trio",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 muffin = "^0"
-asgi-sessions = {version = "^1", extras = ["jwt"]}
+asgi-sessions = { version = "^1", extras = ["jwt"] }
 
 # Optional dependencies
-pyjwt = {version = "^2", optional = true}
-cryptography = {version = "^40", optional = true}
+pyjwt = { version = "*", optional = true }
+cryptography = { version = "*", optional = true }
 
 [tool.poetry.extras]
 jwt = ["pyjwt"]
 fernet = ["cryptography"]
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
-cryptography = "^40"
+cryptography = "*"
 ipdb = "*"
 pre-commit = "*"
-pyjwt = "^2"
+pyjwt = "*"
 pytest = "*"
-pytest-aio = {version = "*", extras = ["curio", "trio"]}
+pytest-aio = { version = "*", extras = ["curio", "trio"] }
 pytest-mypy = "*"
 ruff = "*"
 
 [tool.pytest.ini_options]
 addopts = "-lxsv tests.py"
 log_cli = true
 
@@ -73,12 +73,31 @@
 	pytest tests.py
 """
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 select = ["ALL"]
-ignore = ["ARG", "D", "UP", "ANN", "DJ", "EM", "COM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003"]
+ignore = [
+  "ARG",
+  "D",
+  "UP",
+  "ANN",
+  "DJ",
+  "EM",
+  "COM",
+  "RSE",
+  "SLF",
+  "RET",
+  "S101",
+  "PLR2004",
+  "PLR0912",
+  "N804",
+  "A003",
+  "TRY003",
+  "TD",
+  "FIX",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `muffin_session-2.4.0/PKG-INFO` & `muffin_session-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-session
-Version: 2.4.0
+Version: 2.4.1
 Summary: Signed Cookie-Based HTTP sessions for the Muffin framework
 Home-page: https://github.com/klen/muffin-session
 License: MIT
 Keywords: asyncio,trio,asgi,muffin,web,cookie,sessions,session
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,26 +15,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Provides-Extra: fernet
 Provides-Extra: jwt
 Requires-Dist: asgi-sessions[jwt] (>=1,<2)
-Requires-Dist: cryptography (>=40,<41) ; extra == "fernet"
+Requires-Dist: cryptography ; extra == "fernet"
 Requires-Dist: muffin (>=0,<1)
-Requires-Dist: pyjwt (>=2,<3) ; extra == "jwt"
+Requires-Dist: pyjwt ; extra == "jwt"
 Project-URL: Repository, https://github.com/klen/muffin-session
 Description-Content-Type: text/x-rst
 
 Muffin-Session
 ##############
 
 .. _description:
```

