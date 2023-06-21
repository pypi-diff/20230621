# Comparing `tmp/nepseutils-0.3.5.tar.gz` & `tmp/nepseutils-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepseutils-0.3.5.tar", max compression
+gzip compressed data, was "nepseutils-0.3.6.tar", max compression
```

## Comparing `nepseutils-0.3.5.tar` & `nepseutils-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-03-26 03:54:38.614127 nepseutils-0.3.5/LICENSE
--rw-r--r--   0        0        0     7523 2023-03-26 03:54:38.614127 nepseutils-0.3.5/README.md
--rw-r--r--   0        0        0       66 2023-03-26 03:54:38.614127 nepseutils-0.3.5/nepseutils/__init__.py
--rw-r--r--   0        0        0    12431 2023-03-26 03:54:38.614127 nepseutils-0.3.5/nepseutils/__main__.py
--rw-r--r--   0        0        0    24154 2023-03-26 03:54:38.614127 nepseutils-0.3.5/nepseutils/meroshare.py
--rw-r--r--   0        0        0      661 2023-03-26 03:54:38.614127 nepseutils-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     8281 1970-01-01 00:00:00.000000 nepseutils-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-21 02:03:07.078591 nepseutils-0.3.6/LICENSE
+-rw-r--r--   0        0        0     7523 2023-06-21 02:03:07.078591 nepseutils-0.3.6/README.md
+-rw-r--r--   0        0        0       66 2023-06-21 02:03:07.078591 nepseutils-0.3.6/nepseutils/__init__.py
+-rw-r--r--   0        0        0    12431 2023-06-21 02:03:07.078591 nepseutils-0.3.6/nepseutils/__main__.py
+-rw-r--r--   0        0        0    24137 2023-06-21 02:03:07.078591 nepseutils-0.3.6/nepseutils/meroshare.py
+-rw-r--r--   0        0        0      665 2023-06-21 02:03:07.078591 nepseutils-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     8284 1970-01-01 00:00:00.000000 nepseutils-0.3.6/PKG-INFO
```

### Comparing `nepseutils-0.3.5/LICENSE` & `nepseutils-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nepseutils-0.3.5/README.md` & `nepseutils-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nepseutils-0.3.5/nepseutils/__main__.py` & `nepseutils-0.3.6/nepseutils/__main__.py`

 * *Files identical despite different names*

### Comparing `nepseutils-0.3.5/nepseutils/meroshare.py` & `nepseutils-0.3.6/nepseutils/meroshare.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         capitals = {}
         with requests.Session() as sess:
             sess.headers = BASE_HEADERS
             headers = {
                 "Authorization": "null",
             }
             sess.headers.update(headers)
-            cap_req = sess.get("https://backend.cdsc.com.np/api/meroShare/capital/")
+            cap_req = sess.get(f"{MS_API_BASE}/meroShare/capital/")
             cap_list = cap_req.json()
 
             any(
                 map(
                     lambda x: capitals.update({x.get("code"): x.get("id")}),
                     cap_list,
                 )
```

### Comparing `nepseutils-0.3.5/pyproject.toml` & `nepseutils-0.3.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "nepseutils"
-version = "0.3.5"
+version = "0.3.6"
 description = "Collection of scripts to interact with NEPSE related websites!"
 authors = ["Daze <dazehere@yandex.com>"]
 repository = "https://github.com/arpandaze/nepseutils"
 readme = "README.md"
 keywords = ["nepse","meroshare","tms"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.25.1"
-tenacity = "^7.0.0"
-cryptography = "^3.4.7"
-tabulate = "^0.8.9"
+requests = "^2.31.0"
+tenacity = "^8.2.2"
+cryptography = "^41.0.1"
+tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-pylint = "^2.7.4"
-black = "^20.8b1"
-jedi = "^0.18.0"
-isort = "^5.8.0"
-rope = "^0.18.0"
-flake8 = "^3.9.0"
+pytest = "^7.3.2"
+pylint = "^2.17.4"
+black = "^23.3.0"
+jedi = "^0.18.2"
+isort = "^5.12.0"
+rope = "^1.8.0"
+flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nepseutils-0.3.5/PKG-INFO` & `nepseutils-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nepseutils
-Version: 0.3.5
+Version: 0.3.6
 Summary: Collection of scripts to interact with NEPSE related websites!
 Home-page: https://github.com/arpandaze/nepseutils
 Keywords: nepse,meroshare,tms
 Author: Daze
 Author-email: dazehere@yandex.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=3.4.7,<4.0.0)
-Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: tenacity (>=7.0.0,<8.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Repository, https://github.com/arpandaze/nepseutils
 Description-Content-Type: text/markdown
 
 # NEPSE Utils
 Collection of scripts to interact with NEPSE related sites.
 
 ## Installation instruction
```

