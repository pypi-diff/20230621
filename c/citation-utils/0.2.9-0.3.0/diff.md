# Comparing `tmp/citation_utils-0.2.9.tar.gz` & `tmp/citation_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.2.9.tar", max compression
+gzip compressed data, was "citation_utils-0.3.0.tar", max compression
```

## Comparing `citation_utils-0.2.9.tar` & `citation_utils-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       70 2023-05-15 16:32:51.983670 citation_utils-0.2.9/citation_utils/__init__.py
--rw-r--r--   0        0        0     2566 2023-03-06 01:26:55.330877 citation_utils-0.2.9/citation_utils/db.py
--rw-r--r--   0        0        0     1580 2023-02-25 08:59:18.991399 citation_utils-0.2.9/citation_utils/helpers.py
--rw-r--r--   0        0        0    17514 2023-05-15 16:39:38.638376 citation_utils-0.2.9/citation_utils/main.py
--rw-r--r--   0        0        0      541 2022-11-20 00:05:42.227549 citation_utils-0.2.9/citation_utils/sql/legacy/multiple_cat_idx.sql
--rw-r--r--   0        0        0     1443 2023-05-15 16:32:42.500144 citation_utils-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 citation_utils-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:09:44.831887 citation_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0       48 2023-06-21 17:13:19.096449 citation_utils-0.3.0/citation_utils/__init__.py
+-rw-r--r--   0        0        0     1580 2023-06-21 16:59:09.647600 citation_utils-0.3.0/citation_utils/helpers.py
+-rw-r--r--   0        0        0     9366 2023-06-21 17:53:25.038555 citation_utils-0.3.0/citation_utils/main.py
+-rw-r--r--   0        0        0      541 2023-06-21 15:09:44.832651 citation_utils-0.3.0/citation_utils/sql/legacy/multiple_cat_idx.sql
+-rw-r--r--   0        0        0     1437 2023-06-21 17:51:04.566583 citation_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 citation_utils-0.3.0/PKG-INFO
```

### Comparing `citation_utils-0.2.9/citation_utils/helpers.py` & `citation_utils-0.3.0/citation_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.2.9/citation_utils/sql/legacy/multiple_cat_idx.sql` & `citation_utils-0.3.0/citation_utils/sql/legacy/multiple_cat_idx.sql`

 * *Files identical despite different names*

### Comparing `citation_utils-0.2.9/PKG-INFO` & `citation_utils-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.2.9
+Version: 0.3.0
 Summary: Regex-based docket- and report- styled citations based on Philippine Supreme Court decisions.
 Home-page: https://lawsql.com
-License: MIT
 Author: Marcelino G. Veloso III
-Author-email: mars@veloso.one
+Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation-docket (>=0.1.3,<0.2.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: python-slugify (>=8.0,<9.0)
-Requires-Dist: sqlite-utils (>=3.31,<4.0)
+Requires-Dist: citation-docket (>=0.1.5,<0.2.0)
 Project-URL: Documentation, https://justmars.github.io/citation-utils
 Project-URL: Repository, https://github.com/justmars/citation-utils
```

