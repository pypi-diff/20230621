# Comparing `tmp/muffin-sentry-1.4.2.tar.gz` & `tmp/muffin_sentry-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-sentry-1.4.2.tar", last modified: Sat Mar  4 10:05:06 2023, max compression
+gzip compressed data, was "muffin_sentry-1.4.3.tar", max compression
```

## Comparing `muffin-sentry-1.4.2.tar` & `muffin_sentry-1.4.3.tar`

### file list

```diff
@@ -1,16 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:05:06.904863 muffin-sentry-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-04 10:05:06.904863 muffin-sentry-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:05:06.904863 muffin-sentry-1.4.2/muffin_sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/muffin_sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/muffin_sentry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:05:06.904863 muffin-sentry-1.4.2/muffin_sentry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-04 10:05:06.000000 muffin-sentry-1.4.2/muffin_sentry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-04 10:05:06.000000 muffin-sentry-1.4.2/muffin_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 10:05:06.000000 muffin-sentry-1.4.2/muffin_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-04 10:05:06.000000 muffin-sentry-1.4.2/muffin_sentry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-04 10:05:06.000000 muffin-sentry-1.4.2/muffin_sentry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-04 10:04:58.000000 muffin-sentry-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 10:05:06.904863 muffin-sentry-1.4.2/setup.cfg
+-rw-r--r--   0        0        0     3841 2023-06-21 12:19:04.859211 muffin_sentry-1.4.3/README.rst
+-rw-r--r--   0        0        0     3970 2023-06-21 12:19:04.859211 muffin_sentry-1.4.3/muffin_sentry/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:19:04.859211 muffin_sentry-1.4.3/muffin_sentry/py.typed
+-rw-r--r--   0        0        0     1922 2023-06-21 12:19:04.859211 muffin_sentry-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 muffin_sentry-1.4.3/PKG-INFO
```

### Comparing `muffin-sentry-1.4.2/PKG-INFO` & `muffin_sentry-1.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: muffin-sentry
-Version: 1.4.2
+Version: 1.4.3
 Summary: Sentry Integration for Muffin framework
-Author-email: Kirill Klenov <horneds@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/klen/muffin-sentry
-Project-URL: repository, https://github.com/klen/muffin-sentry
-Project-URL: changelog, https://raw.githubusercontent.com/klen/muffin-sentry/master/CHANGELOG.md
+Home-page: https://github.com/klen/muffin-sentry
+License: MIT
 Keywords: sentry,asyncio,trio,asgi,muffin
+Author: Kirill Klenov
+Author-email: horneds@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Framework :: AsyncIO
-Classifier: Framework :: Trio
-Requires-Python: >=3.8
+Requires-Dist: muffin (>=0,<1)
+Requires-Dist: sentry-sdk
+Project-URL: Repository, https://github.com/klen/muffin-sentry
 Description-Content-Type: text/x-rst
-Provides-Extra: tests
-Provides-Extra: dev
-Provides-Extra: yaml
-Provides-Extra: example
-Provides-Extra: peewee
-Provides-Extra: sqlalchemy
-License-File: LICENSE
 
 Muffin-Sentry
 #############
 
 .. _description:
 
 **Muffin-Sentry** -- Sentry_ Integration for Muffin_ framework
@@ -183,7 +178,8 @@
 
 
 .. _klen: https://github.com/klen
 .. _Muffin: https://github.com/klen/muffin
 .. _Sentry: https://sentry.io/
 
 .. _MIT license: http://opensource.org/licenses/MIT
+
```

### Comparing `muffin-sentry-1.4.2/README.rst` & `muffin_sentry-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-sentry-1.4.2/muffin_sentry/__init__.py` & `muffin_sentry-1.4.3/muffin_sentry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Sentry integration to Muffin framework."""
 from __future__ import annotations
 
 from contextvars import ContextVar
 from functools import partial
-from typing import TYPE_CHECKING, Callable, Dict, List, Optional, TypeVar
+from typing import TYPE_CHECKING, Callable, ClassVar, Dict, List, Optional, TypeVar
 
 from muffin import Application, Request, ResponseError, ResponseRedirect
 from muffin.plugins import BasePlugin
 from sentry_sdk import Hub
 from sentry_sdk import Scope as SentryScope
 from sentry_sdk import init as sentry_init
 from sentry_sdk.tracing import Transaction
@@ -21,38 +21,38 @@
 
 class Plugin(BasePlugin):
 
     """Setup Sentry and send exceptions and messages."""
 
     name = "sentry"
     client = None
-    defaults = {
+    defaults: ClassVar[Dict] = {
         "dsn": "",  # Sentry DSN
         "sdk_options": {},  # See https://docs.sentry.io/platforms/python/configuration/options/
         "ignore_errors": (ResponseError, ResponseRedirect),
     }
     current_scope: ContextVar[Optional[SentryScope]] = ContextVar(
-        "sentry_scope", default=None,
+        "sentry_scope",
+        default=None,
     )
     processors: List[TProcess]
 
     def __init__(self, *args, **kwargs):
         """Initialize the plugin."""
         super(Plugin, self).__init__(*args, **kwargs)
         self.processors = []
 
     def setup(self, app: Application, **options):
         """Initialize Sentry Client."""
         super().setup(app, **options)
 
-        if not self.cfg.dsn:
-            return
-
         # Setup Sentry
-        sentry_init(dsn=self.cfg.dsn, **self.cfg.sdk_options)
+        dsn = self.cfg.dsn
+        if dsn:
+            sentry_init(dsn=dsn, **self.cfg.sdk_options)
 
     async def middleware(  # type: ignore[override]
         self,
         handler: TASGIApp,
         request: Request,
         receive: TASGIReceive,
         send: TASGISend,
@@ -63,15 +63,16 @@
             scope.clear_breadcrumbs()
             scope._name = "muffin"
             self.current_scope.set(scope)
             scope.add_event_processor(partial(self.process_data, request=request))
 
             with hub.start_transaction(
                 Transaction.continue_from_headers(
-                    request.headers, op=f"{request.scope['type']}.muffin",
+                    request.headers,
+                    op=f"{request.scope['type']}.muffin",
                 ),
                 custom_sampling_context={"asgi_scope": scope},
             ):
                 try:
                     return await handler(request, receive, send)
 
                 except Exception as exc:
@@ -101,14 +102,16 @@
         for processor in self.processors:
             event = processor(event, hint, request)
 
         return event
 
     def capture_exception(self, *args, **kwargs):
         """Capture exception."""
-        with Hub(Hub.current, self.current_scope.get()) as hub:
-            return hub.capture_exception(*args, **kwargs)
+        if self.cfg.dsn:
+            with Hub(Hub.current, self.current_scope.get()) as hub:
+                return hub.capture_exception(*args, **kwargs)
 
     def capture_message(self, *args, **kwargs):
         """Capture message."""
-        with Hub(Hub.current, self.current_scope.get()) as hub:
-            return hub.capture_message(*args, **kwargs)
+        if self.cfg.dsn:
+            with Hub(Hub.current, self.current_scope.get()) as hub:
+                return hub.capture_message(*args, **kwargs)
```

### Comparing `muffin-sentry-1.4.2/pyproject.toml` & `muffin_sentry-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-[project]
+[tool.poetry]
 name = "muffin-sentry"
-version = "1.4.2"
+version = "1.4.3"
 description = "Sentry Integration for Muffin framework"
 readme = "README.rst"
-requires-python = ">=3.8"
-license = {"text" = "MIT License"}
-authors = [{ name = "Kirill Klenov", email = "horneds@gmail.com" }]
+license = "MIT"
+authors = ["Kirill Klenov <horneds@gmail.com>"]
+homepage = "https://github.com/klen/muffin-sentry"
+repository = "https://github.com/klen/muffin-sentry"
 keywords = ["sentry", "asyncio", "trio", "asgi", "muffin"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
@@ -17,52 +18,31 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Framework :: AsyncIO",
   "Framework :: Trio",
 ]
-dependencies = [
-  "muffin >= 0.92",
-  "sentry-sdk >= 1.4.3",
-]
 
-[project.urls]
-homepage = "https://github.com/klen/muffin-sentry"
-repository = "https://github.com/klen/muffin-sentry"
-changelog = "https://raw.githubusercontent.com/klen/muffin-sentry/master/CHANGELOG.md"
-
-[project.optional-dependencies]
-tests = [
-  "pytest",
-  "pytest-aio[curio,trio]",
-  "pytest-mypy",
-  "ruff",
-]
-dev = ["pre-commit", "refurb", "bump2version"]
-yaml = ["pyyaml"]
-example = ["uvicorn", "muffin-peewee-aio", "marshmallow-peewee"]
-peewee = [
-    "muffin-peewee-aio >= 0.2.2",
-    "marshmallow-peewee >= 3.2.0",
-]
-sqlalchemy = [
-    "muffin-databases >= 0.3.2",
-    "marshmallow-sqlalchemy",
-    "sqlalchemy",
-]
-
-[tool.setuptools]
-packages = ['muffin_sentry']
-
-[tool.setuptools.package-data]
-muffin_sentry = ["py.typed"]
+[tool.poetry.dependencies]
+python = "^3.8"
+muffin = "^0"
+sentry-sdk = "*"
+
+[tool.poetry.group.dev.dependencies]
+black = "*"
+ipdb = "*"
+pre-commit = "*"
+pytest = "*"
+pytest-aio = { version = "*", extras = ["curio", "trio"] }
+pytest-mypy = "*"
+ruff = "*"
 
 [tool.pytest.ini_options]
-addopts = "-xsv"
+addopts = "-lxsv"
 log_cli = true
 
 [tool.mypy]
 packages = ["muffin_sentry"]
 install_types = true
 non_interactive = true
 ignore_missing_imports = true
@@ -85,8 +65,32 @@
 
 [tool.ruff]
 fix = true
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
 select = ["ALL"]
-ignore = ["D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003"]
+ignore = [
+  "D",
+  "UP",
+  "ANN",
+  "DJ",
+  "EM",
+  "RSE",
+  "SLF",
+  "RET",
+  "S101",
+  "PLR2004",
+  "PLR0912",
+  "N804",
+  "A003",
+  "TRY003",
+]
+
+[tool.black]
+line-length = 100
+target-version = ["py311"]
+preview = true
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

