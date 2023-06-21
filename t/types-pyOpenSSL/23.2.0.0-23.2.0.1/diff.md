# Comparing `tmp/types-pyOpenSSL-23.2.0.0.tar.gz` & `tmp/types-pyOpenSSL-23.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyOpenSSL-23.2.0.0.tar", last modified: Thu Jun  1 01:54:18 2023, max compression
+gzip compressed data, was "types-pyOpenSSL-23.2.0.1.tar", last modified: Wed Jun 21 21:14:18 2023, max compression
```

## Comparing `types-pyOpenSSL-23.2.0.0.tar` & `types-pyOpenSSL-23.2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:54:18.303213 types-pyOpenSSL-23.2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-01 01:54:17.000000 types-pyOpenSSL-23.2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 01:54:17.000000 types-pyOpenSSL-23.2.0.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:54:18.299213 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 01:54:17.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-01 01:54:02.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/SSL.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 01:54:02.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-01 01:54:02.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 01:54:02.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 01:54:02.000000 types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-01 01:54:18.303213 types-pyOpenSSL-23.2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 01:54:18.303213 types-pyOpenSSL-23.2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-01 01:54:17.000000 types-pyOpenSSL-23.2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:54:18.299213 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-01 01:54:18.000000 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 01:54:18.000000 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:54:18.000000 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 01:54:18.000000 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 01:54:18.000000 types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/SSL.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 21:14:01.000000 types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-21 21:14:14.000000 types-pyOpenSSL-23.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:14:18.464179 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 21:14:18.000000 types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/top_level.txt
```

### Comparing `types-pyOpenSSL-23.2.0.0/CHANGELOG.md` & `types-pyOpenSSL-23.2.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 23.2.0.1 (2023-06-21)
+
+Add missing constants to `OpenSSL/crypto.pyi` (#10345)
+
+Adds typing for missing constants `TYPE_DH` and `TYPE_EC`
+
+See https://github.com/pyca/pyopenssl/blob/main/src/OpenSSL/crypto.py#L94-L95
+
 ## 23.2.0.0 (2023-06-01)
 
 [stubsabot] Bump pyOpenSSL to 23.2.* (#10235)
 
 Release: https://pypi.org/pypi/pyOpenSSL/23.2.0
 Homepage: https://pyopenssl.org/
 Diff: https://github.com/pyca/pyopenssl/compare/23.1.1...23.2.0
```

### Comparing `types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/SSL.pyi` & `types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/SSL.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-23.2.0.0/OpenSSL-stubs/crypto.pyi` & `types-pyOpenSSL-23.2.0.1/OpenSSL-stubs/crypto.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 FILETYPE_PEM: int
 FILETYPE_ASN1: int
 FILETYPE_TEXT: int
 
 TYPE_RSA: int
 TYPE_DSA: int
+TYPE_DH: int
+TYPE_EC: int
 
 class _EllipticCurve:
     def __init__(self, lib: Incomplete | None, nid: int, name: str) -> None: ...
 
 class Error(Exception): ...
 
 class PKey:
```

### Comparing `types-pyOpenSSL-23.2.0.0/PKG-INFO` & `types-pyOpenSSL-23.2.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.2.0.0
+Version: 23.2.0.1
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d7a2b8b7fdd35f478da6c51efbaaaef09238a667`.
+This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-pyOpenSSL-23.2.0.0/setup.py` & `types-pyOpenSSL-23.2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d7a2b8b7fdd35f478da6c51efbaaaef09238a667`.
+This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="23.2.0.0",
+      version="23.2.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['cryptography>=35.0.0'],
       packages=['OpenSSL-stubs'],
-      package_data={'OpenSSL-stubs': ['SSL.pyi', '__init__.pyi', 'crypto.pyi', 'rand.pyi', 'version.pyi', 'METADATA.toml']},
+      package_data={'OpenSSL-stubs': ['SSL.pyi', '__init__.pyi', 'crypto.pyi', 'rand.pyi', 'version.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pyOpenSSL-23.2.0.0/types_pyOpenSSL.egg-info/PKG-INFO` & `types-pyOpenSSL-23.2.0.1/types_pyOpenSSL.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 23.2.0.0
+Version: 23.2.0.1
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d7a2b8b7fdd35f478da6c51efbaaaef09238a667`.
+This package was generated from typeshed commit `4c1e94d8e0f212f3b611d06698427d77e696e636` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

