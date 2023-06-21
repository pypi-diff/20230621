# Comparing `tmp/pyextrasafe-0.0.0a1.tar.gz` & `tmp/pyextrasafe-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyextrasafe-0.0.0a1.tar", last modified: Tue May 23 19:39:09 2023, max compression
+gzip compressed data, was "pyextrasafe-0.1.0a1.tar", last modified: Wed Jun 21 12:54:29 2023, max compression
```

## Comparing `pyextrasafe-0.0.0a1.tar` & `pyextrasafe-0.1.0a1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      306 2023-05-22 20:44:19.000000 pyextrasafe-0.0.0a1/CHANGELOG.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1082 2023-05-23 19:29:49.000000 pyextrasafe-0.0.0a1/Cargo.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    10494 2023-05-22 09:25:15.000000 pyextrasafe-0.0.0a1/LICENSE.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      145 2023-05-22 20:44:44.000000 pyextrasafe-0.0.0a1/MANIFEST.in
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1398 2023-05-23 16:08:52.000000 pyextrasafe-0.0.0a1/Makefile
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3286 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1982 2023-05-23 19:27:31.000000 pyextrasafe-0.0.0a1/README.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      668 2023-05-22 08:46:08.000000 pyextrasafe-0.0.0a1/build.rs
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/docs/
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/docs/_static/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      280 2023-05-23 19:11:41.000000 pyextrasafe-0.0.0a1/docs/_static/custom.css
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1010 2023-05-23 19:09:14.000000 pyextrasafe-0.0.0a1/docs/conf.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)       42 2023-05-23 19:07:25.000000 pyextrasafe-0.0.0a1/docs/index.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      204 2023-05-22 22:45:05.000000 pyextrasafe-0.0.0a1/pyproject.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      228 2023-05-22 23:44:25.000000 pyextrasafe-0.0.0a1/requirements-dev.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      164 2023-05-23 19:29:53.000000 pyextrasafe-0.0.0a1/requirements-readthedocs.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2023-05-22 10:16:45.000000 pyextrasafe-0.0.0a1/rustfmt.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1368 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/setup.cfg
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      479 2023-05-22 20:46:15.000000 pyextrasafe-0.0.0a1/setup.py
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/src/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2775 2023-05-23 16:04:22.000000 pyextrasafe-0.0.0a1/src/lib.rs
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/src/pyextrasafe/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     4020 2023-05-23 19:27:10.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/__init__.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      296 2023-05-22 19:07:07.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/__init__.pyi
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5850 2023-05-23 18:29:04.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/_pyextrasafe.pyi
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2023-05-22 09:17:19.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/py.typed
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3286 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      578 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/SOURCES.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/dependency_links.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-22 23:43:44.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/not-zip-safe
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)       12 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/top_level.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    17180 2023-05-23 18:29:01.000000 pyextrasafe-0.0.0a1/src/rule_sets.rs
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     4247 2023-05-23 17:02:52.000000 pyextrasafe-0.0.0a1/src/safety_ctx.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      306 2023-05-22 20:44:19.000000 pyextrasafe-0.1.0a1/CHANGELOG.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1196 2023-06-21 12:36:27.000000 pyextrasafe-0.1.0a1/Cargo.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    10494 2023-05-22 09:25:15.000000 pyextrasafe-0.1.0a1/LICENSE.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      145 2023-05-22 20:44:44.000000 pyextrasafe-0.1.0a1/MANIFEST.in
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1829 2023-05-26 21:14:17.000000 pyextrasafe-0.1.0a1/Makefile
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3336 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1982 2023-05-26 22:03:15.000000 pyextrasafe-0.1.0a1/README.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      668 2023-05-22 08:46:08.000000 pyextrasafe-0.1.0a1/build.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/docs/
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/docs/_templates/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      505 2023-05-28 01:17:26.000000 pyextrasafe-0.1.0a1/docs/_templates/base.html
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3766 2023-06-18 19:27:08.000000 pyextrasafe-0.1.0a1/docs/conf.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    15536 2023-06-21 12:34:01.000000 pyextrasafe-0.1.0a1/docs/index.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      204 2023-05-22 22:45:05.000000 pyextrasafe-0.1.0a1/pyproject.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      206 2023-05-27 12:55:29.000000 pyextrasafe-0.1.0a1/requirements-dev.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      142 2023-06-21 12:35:11.000000 pyextrasafe-0.1.0a1/requirements-readthedocs.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2023-05-22 10:16:45.000000 pyextrasafe-0.1.0a1/rustfmt.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1407 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/setup.cfg
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      850 2023-05-26 22:48:11.000000 pyextrasafe-0.1.0a1/setup.py
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/src/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     4042 2023-05-27 02:57:49.000000 pyextrasafe-0.1.0a1/src/additional.rs
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     8413 2023-06-21 12:24:12.000000 pyextrasafe-0.1.0a1/src/custom.rs
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3241 2023-06-21 12:24:37.000000 pyextrasafe-0.1.0a1/src/lib.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/src/pyextrasafe/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1418 2023-06-21 12:29:52.000000 pyextrasafe-0.1.0a1/src/pyextrasafe/__init__.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      296 2023-05-22 19:07:07.000000 pyextrasafe-0.1.0a1/src/pyextrasafe/__init__.pyi
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     7459 2023-06-21 12:39:37.000000 pyextrasafe-0.1.0a1/src/pyextrasafe/_pyextrasafe.pyi
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2023-05-22 09:17:19.000000 pyextrasafe-0.1.0a1/src/pyextrasafe/py.typed
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-21 12:54:29.388785 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3336 2023-06-21 12:54:29.000000 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      612 2023-06-21 12:54:29.000000 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/SOURCES.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-06-21 12:54:29.000000 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/dependency_links.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-27 12:56:26.000000 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/not-zip-safe
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)       12 2023-06-21 12:54:29.000000 pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/top_level.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    11026 2023-06-21 12:25:51.000000 pyextrasafe-0.1.0a1/src/rule_sets.rs
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2886 2023-05-27 02:21:18.000000 pyextrasafe-0.1.0a1/src/safety_ctx.rs
```

### Comparing `pyextrasafe-0.0.0a1/Cargo.toml` & `pyextrasafe-0.1.0a1/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 # KEEP SYNCHRONOUS TO REQUIREMENTS-READTHEDOCS.TXT (pyextrasafe)
 # KEEP SYNCHRONOUS TO LINKS IN README.MD (raw.githubusercontent.com)
 # Rust uses semver (https://semver.org/).
 # Python uses PEP 440 (https://www.python.org/dev/peps/pep-0440/).
 # Normal releases are exactly the same.
 # Pre-releases are X.Y.Z-aN in semver, and X.Y.ZaN in PEP 440.
 # Post-releases are X.Y.Z+N in semver, and X.Y.Z.postN in PEP 440.
-version = "0.0.0-a1"
+version = "0.1.0-a1"
 
 [lib]
 name = "_pyextrasafe"
 crate-type = ["cdylib"]
 
 [dependencies]
-bitflags = "2.3.1"
-extrasafe = "0.1.2"
-pyo3 = { version = "0.18.3", default-features = false, features = ["extension-module", "macros", "multiple-pymethods"] }
+bitflags = "2.3.2"
+extrasafe = "0.1.4"
+libseccomp = "0.3.0"
+pyo3 = { version = "0.19.0", default-features = false, features = ["extension-module", "macros", "multiple-pymethods"] }
+rustix = { version = "0.37.20", features = ["fs", "process", "thread"] }
+syscalls = "0.6.13"
 
 [build-dependencies]
-pyo3-build-config = "0.18.3"
+pyo3-build-config = "0.19.0"
 
 [profile.release]
-opt-level = "s"
+opt-level = "z"
 lto = "fat"
 codegen-units = 1
```

### Comparing `pyextrasafe-0.0.0a1/LICENSE.md` & `pyextrasafe-0.1.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyextrasafe-0.0.0a1/PKG-INFO` & `pyextrasafe-0.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrasafe
-Version: 0.0.0a1
+Version: 0.1.0a1
 Summary: Make your code extrasafe by preventing it from calling unneeded syscalls
 Home-page: https://github.com/Kijewski/pyextrasafe
 Author: René Kijewski
 Author-email: pypi.org@k6i.de
 License: MIT License
 Project-URL: Changelog, https://github.com/Kijewski/pyextrasafe/blob/main/CHANGELOG.md
 Project-URL: Code, https://github.com/Kijewski/pyextrasafe
@@ -15,28 +15,29 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
-[![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
+[![Python >= 3.7](https://img.shields.io/badge/python-%E2%89%A5%203.7-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
```

### Comparing `pyextrasafe-0.0.0a1/README.md` & `pyextrasafe-0.1.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
-[![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
+[![Python >= 3.7](https://img.shields.io/badge/python-%E2%89%A5%203.7-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
```

### Comparing `pyextrasafe-0.0.0a1/build.rs` & `pyextrasafe-0.1.0a1/build.rs`

 * *Files identical despite different names*

### Comparing `pyextrasafe-0.0.0a1/setup.cfg` & `pyextrasafe-0.1.0a1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.0a1
+version = 0.1.0a1
 name = pyextrasafe
 description = Make your code extrasafe by preventing it from calling unneeded syscalls
 author = René Kijewski
 author_email = pypi.org@k6i.de
 license = MIT License
 license_files = LICENSE.md
 long_description = file: README.md
@@ -20,25 +20,26 @@
 	License :: OSI Approved :: Apache Software License
 	Development Status :: 3 - Alpha
 	Programming Language :: Rust
 	Operating System :: POSIX :: Linux
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 packages = pyextrasafe
 package_dir = 
 	= src
 zip_safe = False
 include_package_data = True
 setup_requires = setuptools-rust == 1.*
-python_requires = >= 3.8, < 4
+python_requires = >= 3.7, < 4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyextrasafe-0.0.0a1/src/lib.rs` & `pyextrasafe-0.1.0a1/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -32,37 +32,46 @@
 #![warn(unused_extern_crates)]
 #![warn(unused_lifetimes)]
 #![warn(unused_results)]
 
 //! PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 //! allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
+mod additional;
+// mod custom;
 mod rule_sets;
 mod safety_ctx;
 
 use pyo3::exceptions::PyException;
 use pyo3::types::PyModule;
-use pyo3::{pymodule, PyResult, PyTypeInfo, Python};
+use pyo3::{pymodule, wrap_pyfunction, PyResult, PyTypeInfo, Python};
 
 pyo3::create_exception!(
     pyextrasafe,
     ExtraSafeError,
     PyException,
     "An exception thrown by PyExtraSafe."
 );
 
 #[pymodule]
 fn _pyextrasafe(py: Python<'_>, m: &PyModule) -> PyResult<()> {
+    // m.add_class::<self::custom::PyCompare>()?;
+    // m.add_class::<self::custom::PyCompareOp>()?;
+    // m.add_class::<self::custom::PyCustom>()?;
+    // m.add_class::<self::custom::PyRule>()?;
     m.add_class::<self::rule_sets::PyBasicCapabilities>()?;
     m.add_class::<self::rule_sets::PyForkAndExec>()?;
     m.add_class::<self::rule_sets::PyNetworking>()?;
     m.add_class::<self::rule_sets::PyRuleSet>()?;
     m.add_class::<self::rule_sets::PySystemIO>()?;
     m.add_class::<self::rule_sets::PyThreads>()?;
     m.add_class::<self::rule_sets::PyTime>()?;
     m.add_class::<self::safety_ctx::PySafetyContext>()?;
+    m.add_function(wrap_pyfunction!(self::additional::lock_pid_file, m)?)?;
+    m.add_function(wrap_pyfunction!(self::additional::restrict_privileges, m)?)?;
     m.add("__author__", env!("CARGO_PKG_AUTHORS"))?;
     m.add("__license__", env!("CARGO_PKG_LICENSE"))?;
     m.add("__version__", env!("pyextrasafe-version"))?;
     m.add("ExtraSafeError", ExtraSafeError::type_object(py))?;
+    // m.add("sysno", self::custom::make_syscall_dict(py)?)?;
     Ok(())
 }
```

### Comparing `pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/PKG-INFO` & `pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrasafe
-Version: 0.0.0a1
+Version: 0.1.0a1
 Summary: Make your code extrasafe by preventing it from calling unneeded syscalls
 Home-page: https://github.com/Kijewski/pyextrasafe
 Author: René Kijewski
 Author-email: pypi.org@k6i.de
 License: MIT License
 Project-URL: Changelog, https://github.com/Kijewski/pyextrasafe/blob/main/CHANGELOG.md
 Project-URL: Code, https://github.com/Kijewski/pyextrasafe
@@ -15,28 +15,29 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
-[![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
+[![Python >= 3.7](https://img.shields.io/badge/python-%E2%89%A5%203.7-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
```

### Comparing `pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/SOURCES.txt` & `pyextrasafe-0.1.0a1/src/pyextrasafe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 requirements-dev.txt
 requirements-readthedocs.txt
 rustfmt.toml
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
-docs/_static/custom.css
+docs/_templates/base.html
+src/additional.rs
+src/custom.rs
 src/lib.rs
 src/rule_sets.rs
 src/safety_ctx.rs
 src/pyextrasafe/__init__.py
 src/pyextrasafe/__init__.pyi
 src/pyextrasafe/_pyextrasafe.pyi
 src/pyextrasafe/py.typed
```

