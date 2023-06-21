# Comparing `tmp/flask_sqlalchemy-3.0.4.tar.gz` & `tmp/flask_sqlalchemy-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_sqlalchemy-3.0.4.tar", last modified: Mon Jun 19 17:31:22 2023, max compression
+gzip compressed data, was "flask_sqlalchemy-3.0.5.tar", last modified: Wed Jun 21 16:37:47 2023, max compression
```

## Comparing `flask_sqlalchemy-3.0.4.tar` & `flask_sqlalchemy-3.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    14114 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/CHANGES.rst
--rw-r--r--   0        0        0     1475 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/LICENSE.rst
--rw-r--r--   0        0        0     2210 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/README.rst
--rw-r--r--   0        0        0      634 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/Makefile
--rw-r--r--   0        0        0    16397 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-logo.png
--rw-r--r--   0        0        0    11109 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-title.png
--rw-r--r--   0        0        0     2276 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/api.rst
--rw-r--r--   0        0        0     3463 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/binds.rst
--rw-r--r--   0        0        0       45 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/changes.rst
--rw-r--r--   0        0        0     1902 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/conf.py
--rw-r--r--   0        0        0     7369 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/config.rst
--rw-r--r--   0        0        0     2744 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/contexts.rst
--rw-r--r--   0        0        0     7548 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/customizing.rst
--rw-r--r--   0        0        0     1171 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/index.rst
--rw-r--r--   0        0        0     2314 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/legacy-query.rst
--rw-r--r--   0        0        0       71 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/license.rst
--rw-r--r--   0        0        0      765 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/make.bat
--rw-r--r--   0        0        0     3487 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/models.rst
--rw-r--r--   0        0        0     2655 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/pagination.rst
--rw-r--r--   0        0        0     3116 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/queries.rst
--rw-r--r--   0        0        0     7503 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/quickstart.rst
--rw-r--r--   0        0        0     1150 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/record-queries.rst
--rw-r--r--   0        0        0      962 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/track-modifications.rst
--rw-r--r--   0        0        0     1917 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/dev.in
--rw-r--r--   0        0        0     1310 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/dev.txt
--rw-r--r--   0        0        0       69 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/docs.in
--rw-r--r--   0        0        0     1281 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/docs.txt
--rw-r--r--   0        0        0       23 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/mypy.in
--rw-r--r--   0        0        0      532 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/mypy.txt
--rw-r--r--   0        0        0       45 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests-min.in
--rw-r--r--   0        0        0      524 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests-min.txt
--rw-r--r--   0        0        0       15 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests.in
--rw-r--r--   0        0        0      342 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests.txt
--rw-r--r--   0        0        0     1250 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      484 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/cli.py
--rw-r--r--   0        0        0    38305 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/extension.py
--rw-r--r--   0        0        0     7112 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/model.py
--rw-r--r--   0        0        0    10963 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/pagination.py
--rw-r--r--   0        0        0        0 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/py.typed
--rw-r--r--   0        0        0     3748 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/query.py
--rw-r--r--   0        0        0     4306 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/record_queries.py
--rw-r--r--   0        0        0     3189 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/session.py
--rw-r--r--   0        0        0      859 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/table.py
--rw-r--r--   0        0        0     2755 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/track_modifications.py
--rw-r--r--   0        0        0     1047 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/conftest.py
--rw-r--r--   0        0        0      365 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_cli.py
--rw-r--r--   0        0        0     3919 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_engine.py
--rw-r--r--   0        0        0     3727 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_legacy_query.py
--rw-r--r--   0        0        0     4032 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_metadata.py
--rw-r--r--   0        0        0     1612 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model.py
--rw-r--r--   0        0        0     2579 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model_bind.py
--rw-r--r--   0        0        0     7793 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model_name.py
--rw-r--r--   0        0        0     5356 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_pagination.py
--rw-r--r--   0        0        0      931 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_record_queries.py
--rw-r--r--   0        0        0     2523 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_session.py
--rw-r--r--   0        0        0     1203 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_table_bind.py
--rw-r--r--   0        0        0     1966 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_track_modifications.py
--rw-r--r--   0        0        0     2356 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_view_query.py
--rw-r--r--   0        0        0      918 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tox.ini
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 flask_sqlalchemy-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    14318 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/CHANGES.rst
+-rw-r--r--   0        0        0     1475 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/LICENSE.rst
+-rw-r--r--   0        0        0     2210 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/README.rst
+-rw-r--r--   0        0        0      634 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/Makefile
+-rw-r--r--   0        0        0    16397 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/_static/flask-sqlalchemy-logo.png
+-rw-r--r--   0        0        0    11109 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/_static/flask-sqlalchemy-title.png
+-rw-r--r--   0        0        0     2276 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/api.rst
+-rw-r--r--   0        0        0     3463 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/binds.rst
+-rw-r--r--   0        0        0       45 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/changes.rst
+-rw-r--r--   0        0        0     1902 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/conf.py
+-rw-r--r--   0        0        0     7369 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/config.rst
+-rw-r--r--   0        0        0     2744 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/contexts.rst
+-rw-r--r--   0        0        0     7548 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/customizing.rst
+-rw-r--r--   0        0        0     1171 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/index.rst
+-rw-r--r--   0        0        0     2314 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/legacy-query.rst
+-rw-r--r--   0        0        0       71 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/license.rst
+-rw-r--r--   0        0        0      765 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/make.bat
+-rw-r--r--   0        0        0     3487 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/models.rst
+-rw-r--r--   0        0        0     2655 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/pagination.rst
+-rw-r--r--   0        0        0     3116 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/queries.rst
+-rw-r--r--   0        0        0     7503 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/quickstart.rst
+-rw-r--r--   0        0        0     1150 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/record-queries.rst
+-rw-r--r--   0        0        0      962 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/docs/track-modifications.rst
+-rw-r--r--   0        0        0     1917 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/dev.in
+-rw-r--r--   0        0        0     1310 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/dev.txt
+-rw-r--r--   0        0        0       69 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/docs.in
+-rw-r--r--   0        0        0     1281 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/docs.txt
+-rw-r--r--   0        0        0       23 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/mypy.in
+-rw-r--r--   0        0        0      532 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/mypy.txt
+-rw-r--r--   0        0        0       45 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/tests-min.in
+-rw-r--r--   0        0        0      524 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/tests-min.txt
+-rw-r--r--   0        0        0       15 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/tests.in
+-rw-r--r--   0        0        0      342 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/requirements/tests.txt
+-rw-r--r--   0        0        0     1250 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      484 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/cli.py
+-rw-r--r--   0        0        0    38293 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/extension.py
+-rw-r--r--   0        0        0     7112 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/model.py
+-rw-r--r--   0        0        0    11119 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/py.typed
+-rw-r--r--   0        0        0     3748 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/query.py
+-rw-r--r--   0        0        0     4306 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/record_queries.py
+-rw-r--r--   0        0        0     3189 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/session.py
+-rw-r--r--   0        0        0      859 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/table.py
+-rw-r--r--   0        0        0     2755 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/track_modifications.py
+-rw-r--r--   0        0        0     1047 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      365 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_cli.py
+-rw-r--r--   0        0        0     3919 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_engine.py
+-rw-r--r--   0        0        0     3727 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_legacy_query.py
+-rw-r--r--   0        0        0     4032 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_metadata.py
+-rw-r--r--   0        0        0     1612 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_model.py
+-rw-r--r--   0        0        0     2579 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_model_bind.py
+-rw-r--r--   0        0        0     7793 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_model_name.py
+-rw-r--r--   0        0        0     5627 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_pagination.py
+-rw-r--r--   0        0        0      931 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_record_queries.py
+-rw-r--r--   0        0        0     2523 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_session.py
+-rw-r--r--   0        0        0     1203 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_table_bind.py
+-rw-r--r--   0        0        0     1966 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_track_modifications.py
+-rw-r--r--   0        0        0     2406 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tests/test_view_query.py
+-rw-r--r--   0        0        0      918 2023-06-21 16:37:47.000000 flask_sqlalchemy-3.0.5/tox.ini
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 flask_sqlalchemy-3.0.5/PKG-INFO
```

### Comparing `flask_sqlalchemy-3.0.4/CHANGES.rst` & `flask_sqlalchemy-3.0.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 3.0.5
+-------------
+
+Released 2023-06-21
+
+-   ``Pagination.next()`` enforces ``max_per_page``. :issue:`1201`
+-   Improve type hint for ``get_or_404`` return value to be non-optional. :pr:`1226`
+
+
 Version 3.0.4
 -------------
 
 Released 2023-06-19
 
 -   Fix type hint for ``get_or_404`` return value. :pr:`1208`
 -   Fix type hints for pyright (used by VS Code Pylance extension). :issue:`1205`
```

### Comparing `flask_sqlalchemy-3.0.4/LICENSE.rst` & `flask_sqlalchemy-3.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/README.rst` & `flask_sqlalchemy-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/Makefile` & `flask_sqlalchemy-3.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-logo.png` & `flask_sqlalchemy-3.0.5/docs/_static/flask-sqlalchemy-logo.png`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-title.png` & `flask_sqlalchemy-3.0.5/docs/_static/flask-sqlalchemy-title.png`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/api.rst` & `flask_sqlalchemy-3.0.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/binds.rst` & `flask_sqlalchemy-3.0.5/docs/binds.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/conf.py` & `flask_sqlalchemy-3.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/config.rst` & `flask_sqlalchemy-3.0.5/docs/config.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/contexts.rst` & `flask_sqlalchemy-3.0.5/docs/contexts.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/customizing.rst` & `flask_sqlalchemy-3.0.5/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/index.rst` & `flask_sqlalchemy-3.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/legacy-query.rst` & `flask_sqlalchemy-3.0.5/docs/legacy-query.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/make.bat` & `flask_sqlalchemy-3.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/models.rst` & `flask_sqlalchemy-3.0.5/docs/models.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/pagination.rst` & `flask_sqlalchemy-3.0.5/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/queries.rst` & `flask_sqlalchemy-3.0.5/docs/queries.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/quickstart.rst` & `flask_sqlalchemy-3.0.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/record-queries.rst` & `flask_sqlalchemy-3.0.5/docs/record-queries.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/docs/track-modifications.rst` & `flask_sqlalchemy-3.0.5/docs/track-modifications.rst`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/pyproject.toml` & `flask_sqlalchemy-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/requirements/dev.txt` & `flask_sqlalchemy-3.0.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/requirements/docs.txt` & `flask_sqlalchemy-3.0.5/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/requirements/mypy.txt` & `flask_sqlalchemy-3.0.5/requirements/mypy.txt`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/requirements/tests-min.txt` & `flask_sqlalchemy-3.0.5/requirements/tests-min.txt`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/__init__.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 from .extension import SQLAlchemy
 
-__version__ = "3.0.4"
+__version__ = "3.0.5"
 
 __all__ = [
     "SQLAlchemy",
 ]
 
 _deprecated_map = {
     "Model": ".model.Model",
```

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/extension.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
             table: engine
             for bind_key, engine in self.engines.items()
             for table in self.metadatas[bind_key].tables.values()
         }
 
     def get_or_404(
         self, entity: type[_O], ident: t.Any, *, description: str | None = None
-    ) -> t.Optional[_O]:
+    ) -> _O:
         """Like :meth:`session.get() <sqlalchemy.orm.Session.get>` but aborts with a
         ``404 Not Found`` error instead of returning ``None``.
 
         :param entity: The model class to query.
         :param ident: The primary key to query.
         :param description: A custom message to show on the error page.
```

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/model.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/pagination.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
         self.page: int = page
         """The current page."""
 
         self.per_page: int = per_page
         """The maximum number of items on a page."""
 
+        self.max_per_page: int | None = max_per_page
+        """The maximum allowed value for ``per_page``."""
+
         items = self._query_items()
 
         if not items and page != 1 and error_out:
             abort(404)
 
         self.items: list[t.Any] = items
         """The items on the current page. Iterating over the pagination object is
@@ -245,14 +248,15 @@
         :param error_out: Abort with a ``404 Not Found`` error if no items are returned
             and ``page`` is not 1, or if ``page`` or ``per_page`` is less than 1, or if
             either are not ints.
         """
         p = type(self)(
             page=self.page + 1,
             per_page=self.per_page,
+            max_per_page=self.max_per_page,
             error_out=error_out,
             count=False,
             **self._query_args,
         )
         p.total = self.total
         return p
```

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/query.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/record_queries.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/record_queries.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/session.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/session.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/table.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/table.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/track_modifications.py` & `flask_sqlalchemy-3.0.5/src/flask_sqlalchemy/track_modifications.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/conftest.py` & `flask_sqlalchemy-3.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_engine.py` & `flask_sqlalchemy-3.0.5/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_legacy_query.py` & `flask_sqlalchemy-3.0.5/tests/test_legacy_query.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_metadata.py` & `flask_sqlalchemy-3.0.5/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_model.py` & `flask_sqlalchemy-3.0.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_model_bind.py` & `flask_sqlalchemy-3.0.5/tests/test_model_bind.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_model_name.py` & `flask_sqlalchemy-3.0.5/tests/test_model_name.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_pagination.py` & `flask_sqlalchemy-3.0.5/tests/test_pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,42 +141,52 @@
                 count=count,
             )
 
 
 @pytest.fixture
 def paginate(app: Flask, db: SQLAlchemy, Todo: t.Any) -> _PaginateCallable:
     with app.app_context():
-        for i in range(1, 101):
+        for i in range(1, 251):
             db.session.add(Todo(title=f"task {i}"))
 
         db.session.commit()
 
     return _PaginateCallable(app, db, Todo)
 
 
 def test_paginate(paginate: _PaginateCallable) -> None:
     p = paginate()
     assert p.page == 1
     assert p.per_page == 20
     assert len(p.items) == 20
-    assert p.total == 100
-    assert p.pages == 5
+    assert p.total == 250
+    assert p.pages == 13
 
 
 def test_paginate_qs(paginate: _PaginateCallable) -> None:
     p = paginate(page=2, per_page=10)
     assert p.page == 2
     assert p.per_page == 10
 
 
 def test_paginate_max(paginate: _PaginateCallable) -> None:
     p = paginate(per_page=100, max_per_page=50)
     assert p.per_page == 50
 
 
+@pytest.mark.usefixtures("app_ctx")
+def test_next_page_size(paginate: _PaginateCallable) -> None:
+    p = paginate(per_page=110, max_per_page=250)
+    assert p.page == 1
+    assert p.per_page == 110
+    p = p.next()
+    assert p.page == 2
+    assert p.per_page == 110
+
+
 def test_no_count(paginate: _PaginateCallable) -> None:
     p = paginate(count=False)
     assert p.total is None
 
 
 @pytest.mark.parametrize(
     ("page", "per_page"), [("abc", None), (None, "abc"), (0, None), (None, -1)]
```

### Comparing `flask_sqlalchemy-3.0.4/tests/test_record_queries.py` & `flask_sqlalchemy-3.0.5/tests/test_record_queries.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_session.py` & `flask_sqlalchemy-3.0.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_table_bind.py` & `flask_sqlalchemy-3.0.5/tests/test_table_bind.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_track_modifications.py` & `flask_sqlalchemy-3.0.5/tests/test_track_modifications.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/tests/test_view_query.py` & `flask_sqlalchemy-3.0.5/tests/test_view_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,17 +66,18 @@
 def test_view_get_or_404_typed(db: SQLAlchemy, app: Flask) -> None:
     class Quiz(db.Model):
         id = sa.Column(sa.Integer, primary_key=True)
         topic = sa.Column(sa.String)
 
     db.create_all()
 
-    item: Quiz = Quiz()
+    item: Quiz = Quiz(topic="Python")
     db.session.add(item)
     db.session.commit()
     result = db.get_or_404(Quiz, 1)
+    assert result.topic == "Python"
     assert result is item
     if hasattr(t, "assert_type"):
         t.assert_type(result, Quiz)
     with pytest.raises(NotFound):
         assert db.get_or_404(Quiz, 2)
     db.drop_all()
```

### Comparing `flask_sqlalchemy-3.0.4/tox.ini` & `flask_sqlalchemy-3.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy-3.0.4/PKG-INFO` & `flask_sqlalchemy-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQLAlchemy
-Version: 3.0.4
+Version: 3.0.5
 Summary: Add SQLAlchemy support to your Flask application.
 Maintainer-email: Pallets <contact@palletsprojects.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

