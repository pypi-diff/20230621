# Comparing `tmp/binapy-0.6.0.tar.gz` & `tmp/binapy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binapy-0.6.0.tar", max compression
+gzip compressed data, was "binapy-0.6.1.tar", max compression
```

## Comparing `binapy-0.6.0.tar` & `binapy-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1073 2022-07-28 07:54:17.356617 binapy-0.6.0/LICENSE
--rw-r--r--   0        0        0     1783 2022-07-28 07:54:17.356617 binapy-0.6.0/README.md
--rw-r--r--   0        0        0      471 2022-07-28 07:54:17.356617 binapy-0.6.0/binapy/__init__.py
--rw-r--r--   0        0        0    23440 2022-07-28 07:54:17.356617 binapy-0.6.0/binapy/binapy.py
--rw-r--r--   0        0        0       78 2022-07-28 07:54:17.356617 binapy-0.6.0/binapy/compression/__init__.py
--rw-r--r--   0        0        0     1606 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/compression/zlib.py
--rw-r--r--   0        0        0      203 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/encoding/__init__.py
--rw-r--r--   0        0        0     3392 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/encoding/base64.py
--rw-r--r--   0        0        0      958 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/encoding/hex.py
--rw-r--r--   0        0        0     1348 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/encoding/url.py
--rw-r--r--   0        0        0      104 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/hashing/__init__.py
--rw-r--r--   0        0        0     3008 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/hashing/sha.py
--rw-r--r--   0        0        0     1943 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/hashing/shake.py
--rw-r--r--   0        0        0      107 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/parsing/__init__.py
--rw-r--r--   0        0        0     1734 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/parsing/json.py
--rw-r--r--   0        0        0        0 2022-07-28 07:54:17.360617 binapy-0.6.0/binapy/py.typed
--rw-r--r--   0        0        0     1971 2022-07-28 07:54:17.360617 binapy-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       36 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     6698 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_binapy.py
--rw-r--r--   0        0        0     2195 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_compression.py
--rw-r--r--   0        0        0     1361 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_encoding.py
--rw-r--r--   0        0        0     4447 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_hash.py
--rw-r--r--   0        0        0     1582 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_json.py
--rw-r--r--   0        0        0      785 2022-07-28 07:54:17.360617 binapy-0.6.0/tests/test_ldap_hash.py
--rw-r--r--   0        0        0     2579 2022-07-28 07:55:09.210358 binapy-0.6.0/setup.py
--rw-r--r--   0        0        0     2551 2022-07-28 07:55:09.210700 binapy-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 12:59:11.684518 binapy-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1637 2023-06-21 12:59:11.684518 binapy-0.6.1/README.md
+-rw-r--r--   0        0        0      471 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/__init__.py
+-rw-r--r--   0        0        0    23456 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/binapy.py
+-rw-r--r--   0        0        0       78 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/compression/__init__.py
+-rw-r--r--   0        0        0     1606 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/compression/zlib.py
+-rw-r--r--   0        0        0      203 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/__init__.py
+-rw-r--r--   0        0        0     3392 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/base64.py
+-rw-r--r--   0        0        0      958 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/hex.py
+-rw-r--r--   0        0        0     1348 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/url.py
+-rw-r--r--   0        0        0      104 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/__init__.py
+-rw-r--r--   0        0        0     3008 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/sha.py
+-rw-r--r--   0        0        0     1943 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/shake.py
+-rw-r--r--   0        0        0      107 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/parsing/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/parsing/json.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/py.typed
+-rw-r--r--   0        0        0     2017 2023-06-21 12:59:11.688519 binapy-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     6698 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_binapy.py
+-rw-r--r--   0        0        0     2195 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_compression.py
+-rw-r--r--   0        0        0     1361 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_encoding.py
+-rw-r--r--   0        0        0     4447 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_hash.py
+-rw-r--r--   0        0        0     1582 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_json.py
+-rw-r--r--   0        0        0      785 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_ldap_hash.py
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 binapy-0.6.1/PKG-INFO
```

### Comparing `binapy-0.6.0/LICENSE` & `binapy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/README.md` & `binapy-0.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # BinaPy
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Downloads](https://pepy.tech/badge/binapy/month)](https://pepy.tech/project/binapy)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/binapy.svg)](https://pypi.org/project/binapy)
-[![PyPi license](https://badgen.net/pypi/license/binapy/)](https://pypi.com/project/binapy/)
+[![PyPi version](https://badgen.net/pypi/v/binapy)](https://badgen.net/pypi/v/binapy)
 [![PyPI status](https://img.shields.io/pypi/status/binapy.svg)](https://pypi.python.org/pypi/binapy/)
-[![GitHub commits](https://badgen.net/github/commits/guillp/binapy)](https://github.com/guillp/binapy/commit/)
-[![GitHub latest commit](https://badgen.net/github/last-commit/guillp/binapy)](https://github.com/guillp/binapy/commit/)
+[![PyPi license](https://badgen.net/pypi/license/binapy/)](https://pypi.com/project/binapy/)
 
 **BinaPy** is a module that makes Binary Data manipulation simpler and easier than what is offered in the Python standard library.
 
 With BinaPy, encoding or decoding data in a number of formats (base64, base64url, hex, url-encoding, etc.), compressing or decompressing (gzip), hashing (SHA1, SHA256, MD5, etc., with or without salt), is all a single method call away! And you can extend it with new formats and features.
 
 ```python
 from binapy import BinaPy
```

### Comparing `binapy-0.6.0/binapy/binapy.py` & `binapy-0.6.1/binapy/binapy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
+    SupportsBytes,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from typing_extensions import Literal, SupportsIndex
@@ -30,15 +31,15 @@
     Actual transformations into formats such as Base64, JSON, etc. are implemented using
     Extensions. Those extensions are registered using the decorators `binapy_encoder`,
     `binapy_decoder`, `binapy_checker`, `binapy_serializer`, and `binapy_parser`.
     """
 
     def __new__(
         cls,
-        value: Union[bytes, str, int] = b"",
+        value: Union[bytes, str, int, SupportsBytes] = b"",
         encoding: str = "utf-8",
         errors: str = "strict",
     ) -> "BinaPy":
         """Override base method to accept a string with a default encoding of "utf-8".
 
         See Also:
             [`bytes` constructor](https://docs.python.org/3/library/stdtypes.html#bytes) and
@@ -319,17 +320,15 @@
         spos = sorted(pos)
         return [
             self.__class__(self[start:end])
             for start, end in zip([0] + spos, spos + [len(self)])
         ]
 
     extensions: Dict[str, Dict[str, Callable[..., Any]]] = {}
-    """
-    Extension registry.
-    """
+    """Extension registry."""
 
     @classmethod
     def _get_extension_methods(cls, name: str) -> Dict[str, Callable[..., Any]]:
         extension = cls.extensions.get(name)
         if extension is None:
             raise NotImplementedError(f"Extension {name} not found")
         return extension
@@ -451,17 +450,17 @@
                 raise exc
             except Exception as exc:
                 if raise_on_error:
                     raise exc from exc
                 return False
         except NotImplementedError:
             try:
-                decoder = self._get_decoder(name)
                 # if checker is not implemented and decode is True, try to decode instead
-                if decode and decoder:
+                if decode:
+                    decoder = self._get_decoder(name)
                     try:
                         decoder(self)
                         return True
                     except Exception as exc:
                         if raise_on_error:
                             raise exc from exc
                         return False
```

### Comparing `binapy-0.6.0/binapy/compression/zlib.py` & `binapy-0.6.1/binapy/compression/zlib.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/encoding/base64.py` & `binapy-0.6.1/binapy/encoding/base64.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/encoding/hex.py` & `binapy-0.6.1/binapy/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/encoding/url.py` & `binapy-0.6.1/binapy/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/hashing/sha.py` & `binapy-0.6.1/binapy/hashing/sha.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/hashing/shake.py` & `binapy-0.6.1/binapy/hashing/shake.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/binapy/parsing/json.py` & `binapy-0.6.1/binapy/parsing/json.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/pyproject.toml` & `binapy-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "binapy"
-version = "0.6.0"
+version = "0.6.1"
 homepage = "https://github.com/guillp/binapy"
 description = "Binary Data manipulation, for humans."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -13,14 +13,15 @@
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "binapy" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `binapy-0.6.0/tests/test_binapy.py` & `binapy-0.6.1/tests/test_binapy.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/tests/test_compression.py` & `binapy-0.6.1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/tests/test_encoding.py` & `binapy-0.6.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/tests/test_hash.py` & `binapy-0.6.1/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/tests/test_json.py` & `binapy-0.6.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/tests/test_ldap_hash.py` & `binapy-0.6.1/tests/test_ldap_hash.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.0/PKG-INFO` & `binapy-0.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: binapy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Binary Data manipulation, for humans.
 Home-page: https://github.com/guillp/binapy
 License: MIT
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # BinaPy
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Downloads](https://pepy.tech/badge/binapy/month)](https://pepy.tech/project/binapy)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/binapy.svg)](https://pypi.org/project/binapy)
-[![PyPi license](https://badgen.net/pypi/license/binapy/)](https://pypi.com/project/binapy/)
+[![PyPi version](https://badgen.net/pypi/v/binapy)](https://badgen.net/pypi/v/binapy)
 [![PyPI status](https://img.shields.io/pypi/status/binapy.svg)](https://pypi.python.org/pypi/binapy/)
-[![GitHub commits](https://badgen.net/github/commits/guillp/binapy)](https://github.com/guillp/binapy/commit/)
-[![GitHub latest commit](https://badgen.net/github/last-commit/guillp/binapy)](https://github.com/guillp/binapy/commit/)
+[![PyPi license](https://badgen.net/pypi/license/binapy/)](https://pypi.com/project/binapy/)
 
 **BinaPy** is a module that makes Binary Data manipulation simpler and easier than what is offered in the Python standard library.
 
 With BinaPy, encoding or decoding data in a number of formats (base64, base64url, hex, url-encoding, etc.), compressing or decompressing (gzip), hashing (SHA1, SHA256, MD5, etc., with or without salt), is all a single method call away! And you can extend it with new formats and features.
 
 ```python
 from binapy import BinaPy
```

