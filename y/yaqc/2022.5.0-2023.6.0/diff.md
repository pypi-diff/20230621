# Comparing `tmp/yaqc-2022.5.0.tar.gz` & `tmp/yaqc-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqc-2022.5.0.tar", last modified: Thu May 19 21:46:29 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `yaqc-2022.5.0.tar` & `yaqc-2023.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3526 2022-05-19 21:46:11.918100 yaqc-2022.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     7652 2022-05-19 21:46:11.918100 yaqc-2022.5.0/LICENSE
--rw-r--r--   0        0        0      626 2022-05-19 21:46:11.918100 yaqc-2022.5.0/README.md
--rw-r--r--   0        0        0     1157 2022-05-19 21:46:11.918100 yaqc-2022.5.0/pyproject.toml
--rw-r--r--   0        0        0      372 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/HandshakeRequest.avsc
--rw-r--r--   0        0        0      484 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/HandshakeResponse.avsc
--rw-r--r--   0        0        0        9 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/VERSION
--rw-r--r--   0        0        0      104 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/__init__.py
--rw-r--r--   0        0        0      564 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/__version__.py
--rw-r--r--   0        0        0      791 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_avro_numpy.py
--rw-r--r--   0        0        0     3618 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_client.py
--rw-r--r--   0        0        0      513 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_dotdict.py
--rw-r--r--   0        0        0     1001 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_properties.py
--rw-r--r--   0        0        0      262 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_schema.py
--rw-r--r--   0        0        0     5231 2022-05-19 21:46:11.918100 yaqc-2022.5.0/yaqc/_socket.py
--rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 yaqc-2022.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yaqc-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/HandshakeRequest.avsc
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/HandshakeResponse.avsc
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/__version__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_avro_numpy.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_client.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_dotdict.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_properties.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_schema.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 yaqc-2023.6.0/yaqc/_socket.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 yaqc-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 yaqc-2023.6.0/LICENSE
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 yaqc-2023.6.0/README.md
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 yaqc-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 yaqc-2023.6.0/PKG-INFO
```

### Comparing `yaqc-2022.5.0/CHANGELOG.md` & `yaqc-2023.6.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0]
+
+### Fixed
+- fastavro >=1.7 prevents infrequent CPU locking from bad string parsing
+
+### Added
+- `timeout` argument to Client, defaulting to 10 seconds
+
+### Changed
+- moved to hatchling build system
+
 ## [2022.5.0]
 
 ### Changed
 - New repo home at https://github.com/yaq-project/yaq-python
 
 ## [2022.4.0]
 
@@ -108,15 +119,16 @@
 - prevent failure on long messages
 
 ## [0.1.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqc-2022.5.0...main
+[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqc-2023.6.0...main
+[2023.6.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2022.5.0...yaqc-2023.6.0
 [2022.5.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2022.4.0...yaqc-2022.5.0
 [2022.4.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2021.12.0...yaqc-2022.4.0
 [2021.12.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2021.10.0...yaqc-2021.12.0
 [2021.10.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2021.4.0...yaqc-2021.10.0
 [2021.4.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2020.10.0...yaqc-2021.4.0
 [2020.10.0]: https://github.com/yaq-project/yaq-python/compare/yaqc-2020.07.3...yaqc-2020.10.0
 [2020.07.3]: https://github.com/yaq-project/yaq-python/compare/yaqc-2020.07.2...yaqc-2020.07.3
```

### Comparing `yaqc-2022.5.0/LICENSE` & `yaqc-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqc-2022.5.0/README.md` & `yaqc-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yaqc-2022.5.0/yaqc/_avro_numpy.py` & `yaqc-2023.6.0/yaqc/_avro_numpy.py`

 * *Files identical despite different names*

### Comparing `yaqc-2022.5.0/yaqc/_client.py` & `yaqc-2023.6.0/yaqc/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
             self.handshake()
             return fun(self, *args, **kwargs)
 
     return inner
 
 
 class Client:
-    def __init__(self, port, host="127.0.0.1"):
+    def __init__(self, port, host="127.0.0.1", timeout=10):
         self._host = host
         self._port = port
-        self._socket = Socket(self._host, self._port)
+        self._socket = Socket(self._host, self._port, timeout)
         self._id_counter = 0
         self._connection_callbacks = []
         self._mutex = Lock()
         self._cached_id = dict()
         self.handshake()
         self.id()  # populates cached_id
```

### Comparing `yaqc-2022.5.0/yaqc/_dotdict.py` & `yaqc-2023.6.0/yaqc/_dotdict.py`

 * *Files identical despite different names*

### Comparing `yaqc-2022.5.0/yaqc/_properties.py` & `yaqc-2023.6.0/yaqc/_properties.py`

 * *Files identical despite different names*

### Comparing `yaqc-2022.5.0/yaqc/_socket.py` & `yaqc-2023.6.0/yaqc/_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from ._schema import handshake_request, handshake_response
 
 
 BUFFSIZE = 4096
 
 
 class Socket:
-    def __init__(self, host, port):
+    def __init__(self, host, port, timeout=None):
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self._socket.settimeout(None)
+        self._socket.settimeout(timeout)
         self._socket.connect((host, port))
         self._named_types = {}
 
     def _read(self, response_schema):
         response_schema = fastavro.parse_schema(
             response_schema, expand=True, named_schemas=self._named_types
         )
```

### Comparing `yaqc-2022.5.0/PKG-INFO` & `yaqc-2023.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: yaqc
-Version: 2022.5.0
+Version: 2023.6.0
 Summary: Generic yaq client.
-Home-page: https://yaq.fyi
+Project-URL: Home Page, https://yaq.fyi
+Project-URL: Source, https://github.com/yaq-project/yaq-python
+Project-URL: Issues, https://github.com/yaq-project/yaq-python/issues
+Project-URL: Documentation, https://yaq.fyi/blog/yaqc/
 Author: yaq developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+License-Expression: LGPL-3.0-only
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: fastavro>=1.4
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Project-URL: Documentation, https://python.yaq.fyi/yaqc/
-Project-URL: Issues, https://github.com/yaq-project/yaq-python/issues
-Project-URL: Source, https://github.com/yaq-project/yaq-python
+Requires-Python: >=3.6
+Requires-Dist: fastavro>=1.7
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # yaqc-python
 
 [![PyPI](https://img.shields.io/pypi/v/yaqc)](https://pypi.org/project/yaqc)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/yaqc)](https://anaconda.org/conda-forge/yaqc)
 [![yaq](https://img.shields.io/badge/framework-yaq-orange)](https://yaq.fyi/)
 [![black](https://img.shields.io/badge/code--style-black-black)](https://black.readthedocs.io/)
 [![ver](https://img.shields.io/badge/calver-YYYY.M.MICRO-blue)](https://calver.org/)
 [![log](https://img.shields.io/badge/change-log-informational)](https://github.com/yaq-project/yaq-python/blob/main/yaqc/CHANGELOG.md)
 
 Generic yaq client, written in Python.
-
```

