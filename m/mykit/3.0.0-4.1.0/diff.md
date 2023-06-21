# Comparing `tmp/mykit-3.0.0.tar.gz` & `tmp/mykit-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-tgo56sui/mykit-3.0.0.tar", last modified: Sat Jun 17 17:20:30 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-p06t2_t1/mykit-4.1.0.tar", last modified: Wed Jun 21 14:18:19 2023, max compression
```

## Comparing `mykit-3.0.0.tar` & `mykit-4.1.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-17 17:20:10.000000 mykit-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-17 17:20:30.000000 mykit-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-17 17:20:10.000000 mykit-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27032 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-17 17:20:10.000000 mykit-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 17:20:30.000000 mykit-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 17:20:10.000000 mykit-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 14:18:03.000000 mykit-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-21 14:18:19.000000 mykit-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-21 14:18:03.000000 mykit-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 14:18:03.000000 mykit-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 14:18:19.000000 mykit-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 14:18:03.000000 mykit-4.1.0/setup.py
```

### Comparing `mykit-3.0.0/LICENSE` & `mykit-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/PKG-INFO` & `mykit-4.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 3.0.0
+Version: 4.1.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -21,22 +21,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<!-- make the status easily visible -->
+[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+
+
 # myKit
 
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
-![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -61,14 +65,23 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 4.1.0 (June 21, 2023):
+    - NEW: in `/kit/utils.py`: `slowprint` and `print_screen`
+- 4.0.0 (June 18, 2023):
+    - Breaking changes:
+        - `LIB_DIR_PTH` in `mykit` replaced by `DIST_DIR_PTH`
+        - Changed `/app/` mechanism:
+            - removed `/app/_runtime.py`
+    - `.app.App.listen`: Added aliases for event listener types
+    - New: `/app/architecture`
 - 3.0.0 (June 17, 2023):
     - Breaking changes:
         - Changed `title` arg to `name` in `.app.App`
         - Now `/kit/keycrate` must be a .txt file, and the file must exist
         - Added `export` method to `.kit.keycrate.KeyCrate`
     - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
@@ -116,13 +129,13 @@
     - transform `/kit/text/` -> `/kit/text.py`
     - transform `/kit/time/` -> `/kit/time.py`
     - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
-- To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
+- If you find any bugs, feel free to contribute by opening an issue or pull request. Thanks!
 
 
 ## License
 
 This project is licensed under the MIT license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mykit-3.0.0/README.md` & `mykit-4.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+<!-- make the status easily visible -->
+[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+
+
 # myKit
 
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
-![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -34,14 +38,23 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 4.1.0 (June 21, 2023):
+    - NEW: in `/kit/utils.py`: `slowprint` and `print_screen`
+- 4.0.0 (June 18, 2023):
+    - Breaking changes:
+        - `LIB_DIR_PTH` in `mykit` replaced by `DIST_DIR_PTH`
+        - Changed `/app/` mechanism:
+            - removed `/app/_runtime.py`
+    - `.app.App.listen`: Added aliases for event listener types
+    - New: `/app/architecture`
 - 3.0.0 (June 17, 2023):
     - Breaking changes:
         - Changed `title` arg to `name` in `.app.App`
         - Now `/kit/keycrate` must be a .txt file, and the file must exist
         - Added `export` method to `.kit.keycrate.KeyCrate`
     - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
@@ -89,13 +102,13 @@
     - transform `/kit/text/` -> `/kit/text.py`
     - transform `/kit/time/` -> `/kit/time.py`
     - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
-- To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
+- If you find any bugs, feel free to contribute by opening an issue or pull request. Thanks!
 
 
 ## License
 
 This project is licensed under the MIT license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mykit-3.0.0/mykit/__main__.py` & `mykit-4.1.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/app/__init__.py` & `mykit-4.1.0/mykit/app/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,176 @@
 import tkinter as _tk
 from typing import (
     Callable as _Callable,
-    List as _List
+    List as _List,
+    Optional as _Optional
 )
 
-from mykit.app._runtime import Runtime as _Rt
+from mykit.app.architecture import Architecture as _Architecture
+
 from mykit.app.button import Button as _Button
 from mykit.app.label import Label as _Label
 from mykit.app.slider import _Slider
 
+from mykit.app.arrow import Arrow as _Arrow
+from mykit.app.complex.plot import Plot as _Plot
+from mykit.app.complex.biplot import Biplot as _Biplot
+
 
-class App(_Rt):
+class App:
     """
-    Single-page app.
+    A single-page app framework.
+    (currently in beta)
 
     ---
 
     ## Limitations
     - currently available only in fullscreen mode
     """
 
     def __init__(
         self,
         name: str = 'app',
-        bg: str = '#111111'
+        bg: str = '#111111',
+        architecture: _Optional[_Architecture] = None
     ) -> None:
 
         self.root = _tk.Tk()
         self.root.attributes('-fullscreen', True)
         self.root.title(name)
 
-        page = _tk.Canvas(
+        ## app's page
+        self.page = _tk.Canvas(
             master=self.root,
             width=self.root.winfo_screenwidth(),
             height=self.root.winfo_screenheight(),
             background=bg,
             borderwidth=0, highlightthickness=0
         )
-        page.place(x=0, y=0)
-        App._set_page(page)
+        self.page.place(x=0, y=0)
+
+
+        ## <register the page>
+        
+        ## widgets
+        _Button._set_page(self.page)
+        _Slider._set_page(self.page)
+
+        ## others
+        _Arrow._set_page(self.page)
+        _Plot._set_page(self.page)
+        _Biplot._set_page(self.page)
+
+        ## </register the page>
 
 
         ## <constants>
+
         self.MON_WIDTH = self.root.winfo_screenwidth()
         self.MON_HEIGHT = self.root.winfo_screenheight()
+        
         ## </constants>
 
 
         ## <runtime>
+
         self._left_mouse_press = []
         self._left_mouse_hold = []
         self._left_mouse_release = []
 
         self._background_processes = {}
 
         self._setup = []
         self._teardown = []
+
         ## </runtime>
 
     def listen(self, to: str, do: _Callable[[_tk.Event], None]):
         """
         Add event listener.
 
         ---
 
         ## Params
-        - `to`: `Literal["left-mouse-press", "left-mouse-hold", "left-mouse-release"]`
+        - `to`: event type:
+            - `"left-mouse-press"` or `"lmp"`
+            - `"left-mouse-hold"` or `"lmh"`
+            - `"left-mouse-release"` or `"lmr"`
 
         ## Docs
         - `do` function takes 1 positional parameter, which is a tkinter event object
         """
         
-        if to == 'left-mouse-press':
+        if to in {'left-mouse-press', 'lmp'}:
             self._left_mouse_press.append(do)
-        elif to == 'left-mouse-hold':
+        elif to in {'left-mouse-hold', 'lmh'}:
             self._left_mouse_hold.append(do)
-        elif to == 'left-mouse-release':
+        elif to in {'left-mouse-release', 'lmr'}:
             self._left_mouse_release.append(do)
         else:
             ValueError(f'Invalid event: {repr(to)}.')
     
     def add_background_processes(self, every: int, do: _Callable[[], None]) -> None:
         """
         Execute `do` every `every` milliseconds.
-        The first execution occurs immediately after the app runs.
+        
+        ---
+
+        ## Docs
+        - the first execution occurs immediately after the app runs
         """
-        if every in self._background_processes:
-            self._background_processes[every].append(do)
-        else:
-            self._background_processes[every] = [do]
+        if every not in self._background_processes:
+            self._background_processes[every] = []
+        self._background_processes[every].append(do)
 
     def setup(self, funcs: _List[_Callable[[], None]]):
         self._setup = funcs
 
     def teardown(self, funcs: _List[_Callable[[], None]]):
         self._teardown = funcs
 
     def run(self):
-        
+
+        ## <internal>
+
+        self.listen(to='left-mouse-press', do=_Button._press_listener)
+        self.listen(to='left-mouse-press', do=_Slider._press_listener)
+
+        self.listen(to='left-mouse-hold', do=_Slider._hold_listener)
+
+        self.listen(to='left-mouse-release', do=_Button._release_listener)
+        self.listen(to='left-mouse-release', do=_Slider._release_listener)
+
+        self.add_background_processes(every=50, do=_Button._hover_listener)
+        self.add_background_processes(every=50, do=_Slider._hover_listener)
+
+        ## </internal>
+
+
         ## <listeners>
 
-        def left_mouse_press(e):
-            
-            ## internal
-            _Button.press_listener()
-            _Slider.press_listener()
-            
-            ## external
-            for fn in self._left_mouse_press:
-                fn(e)
-
-        self.root.bind('<ButtonPress-1>', left_mouse_press)
-
-        def left_mouse_hold(e):
-            
-            ## internal
-            _Slider.hold_listener()
-
-            ## external
-            for fn in self._left_mouse_hold:
-                fn(e)
-
-        self.root.bind('<B1-Motion>', left_mouse_hold)
-
-        def left_mouse_release(e):
-
-            ## internal
-            _Button.release_listener()
-            _Slider.release_listener()
-
-            ## external
-            for fn in self._left_mouse_release:
-                fn(e)
-        self.root.bind('<ButtonRelease-1>', left_mouse_release)
+        self.root.bind('<ButtonPress-1>',   lambda e: [f(e) for f in self._left_mouse_press])
+        self.root.bind('<B1-Motion>',       lambda e: [f(e) for f in self._left_mouse_hold])
+        self.root.bind('<ButtonRelease-1>', lambda e: [f(e) for f in self._left_mouse_release])
 
         self.root.bind('<Escape>', lambda e: self.root.destroy())
 
         ## </listeners>
 
 
-        ## <background processes>
-
-        ## internal
-        def repeat50():
-            _Button.hover_listener()
-            _Slider.hover_listener()
-            self.root.after(50, repeat50)
-        # self.root.after(50, repeat50)  # start after 50ms
-        repeat50()  # start immediately
-
-        ## users
-        def setup_background_processes():
+        def run_background_processes():
             def wrapper(dur, funcs):
                 def inner():
                     for fn in funcs: fn()
                     self.root.after(dur, inner)
                 return inner
             for dur, funcs in self._background_processes.items():
                 fn = wrapper(dur, funcs)
                 fn()  # start immediately
-        setup_background_processes()
-        
-        ## </background processes>
+        run_background_processes()
 
 
         ## setup
         for fn in self._setup: fn()
 
         ## run
         self.root.mainloop()
```

### Comparing `mykit-3.0.0/mykit/app/arrow.py` & `mykit-4.1.0/mykit/app/arrow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import math as _math
 import random as _random
+import tkinter as _tk
 from typing import (
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
-from mykit.app._runtime import Runtime as _Rt
 from mykit.kit.math import (
     get_angle as _get_angle,
     rotate as _rotate
 )
 
 
-class Arrow(_Rt):
+class Arrow:
+
+    ## <runtime>
+
+    _page: _tk.Canvas = None
+    @staticmethod
+    def _set_page(page):
+        Arrow._page = page
 
     arrows: _Dict[str, 'Arrow'] = {}
     arrow_tags: _Dict[str, _List['Arrow']] = {}
 
+    ## </runtime>
+
     def __init__(
         self,
         from_x: int, from_y: int,
         to_x: int, to_y: int,
         /,
         color: str = '#ddd',
         width_rod: int = 1,
@@ -32,64 +41,77 @@
         tip_angle: float = 35,
         visible: bool = True,
         
         id: _Optional[str] = None,
         tags: _Optional[_Union[str, _List[str]]] = None,
     ) -> None:
 
-        if Arrow.page is None:
-            raise AssertionError('App has not been initialized.')
+        ## <dependencies check>
+
+        ## reminder: Arrow isn't actually a widget. it can be used as a utility
+        ##           outside App's purposes. so just use Arrow._set_page to achieve it.
+        if Arrow._page is None:
+            raise AssertionError('Can\'t use widgets before App initialized.')
+        
+        ## </dependencies check>
         
         self.from_x = from_x
         self.from_y = from_y
         self.to_x = to_x
         self.to_y = to_y
 
         self.color = color
         self.width_rod = width_rod
         self.width_tip = width_tip
         self.tip_len = tip_len
         self.tip_angle = tip_angle
 
         self.visible = visible
 
+        ## <id>
+
         ## to make sure that we can modify a specific arrow without affecting the others
         if id is None:
             self.id = _random.randint(-10000, 10000)
             while self.id in Arrow.arrows:
                 self.id = _random.randint(-10000, 10000)
         else:
             self.id = id
             if self.id in Arrow.arrows:
                 raise ValueError(f'The Arrow\'s id {repr(id)} is duplicated.')
+        
         Arrow.arrows[self.id] = self
 
+        ## </id>
+
         ## <tags>
+
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
         
         if tags is not None:
             for tag in self.tags:
                 if tag in Arrow.arrow_tags:
                     Arrow.arrow_tags[tag].append(self)
                 else:
                     Arrow.arrow_tags[tag] = [self]
+        
         ## </tags>
 
         ## init
         self._redraw()
 
     def _redraw(self):
 
-        Arrow.page.delete(f'Arrow_{self.id}')
+        Arrow._page.delete(f'Arrow_{self.id}')
 
         if self.visible:
-            Arrow.page.create_line(
+            Arrow._page.create_line(
                 self.from_x, self.from_y,
                 self.to_x, self.to_y,
                 fill=self.color, width=self.width_rod, tags=f'Arrow_{self.id}'
             )
 
             ## <creating the tip>
             ## for `angle`: remember to flip the y-sign because tkinter's y-positive direction towards the bottom
@@ -104,15 +126,15 @@
             tip_right = _rotate(tipx, -tipy, 0, 0, angle)
 
             ## Revert to the tkinter coordinate scheme, where y-positive is oriented downwards.
             tip_left = (self.to_x+tip_left[0], self.to_y-tip_left[1])
             tip_right = (self.to_x+tip_right[0], self.to_y-tip_right[1])
 
             tip_points = [tip_left, (self.to_x, self.to_y), tip_right]
-            Arrow.page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
+            Arrow._page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
             ## </creating the tip>
 
 
     def set_visibility(self, visible: bool, /):
         if visible != self.visible:
             self.visible = visible
             self._redraw()
```

### Comparing `mykit-3.0.0/mykit/app/button.py` & `mykit-4.1.0/mykit/app/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import random as _random
+import tkinter as _tk
 from typing import (
     Callable as _Callable,
     Dict as _Dict,
     List as _List,
     Literal as _Literal,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
-from mykit.app._runtime import Runtime as _Rt
 
+class Button:
 
-class Button(_Rt):
+    ## <runtime>
+
+    _page: _tk.Canvas = None
+    @staticmethod
+    def _set_page(page):
+        Button._page = page
 
     buttons: _Dict[str, 'Button'] = {}
     button_tags: _Dict[str, _List['Button']] = {}
 
+    ## </runtime>
+
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
         fn: _Optional[_Callable[[], None]] = None,
         label: str = '',
         label_font: _Union[str, _Tuple[str, int]] = 'Verdana 8',
@@ -46,16 +54,20 @@
         ## Params
         - `x` and `y` is the position of the `anchor` (not the center of the button)
         - `color_btn_normal`: button's color
         - `color_bd_normal`: button's border color
         - `color_lbl_normal`: button's label color
         """
 
-        if Button.page is None:
-            raise AssertionError('App has not been initialized.')
+        ## <dependencies check>
+
+        if Button._page is None:
+            raise AssertionError('Can\'t use widgets before App initialized.')
+        
+        ## </dependencies check>
 
         self.x = x
         self.y = y
         self.fn = fn
         self.label = label
         self.label_font = label_font
         self.anchor = anchor
@@ -69,37 +81,44 @@
         self.color_btn_press = color_btn_press
         self.color_btn_locked = color_btn_locked
         self.color_bd_normal = color_bd_normal
         self.color_bd_locked = color_bd_locked
         self.color_lbl_normal = color_lbl_normal
         self.color_lbl_locked = color_lbl_locked
 
+        ## <id>
+
         ## self.id ensures that we can modify a specific instance without affecting the others
         if id is None:
             self.id = str(_random.randint(0, 100_000))
             while self.id in Button.buttons:
                 self.id = str(_random.randint(0, 100_000))
         else:
             self.id = id
             if self.id in Button.buttons:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
+        
         Button.buttons[self.id] = self
 
+        ## </id>
+
         ## <tags>
+
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
         
         if tags is not None:
             for tag in self.tags:
                 if tag in Button.button_tags:
                     Button.button_tags[tag].append(self)
                 else:
                     Button.button_tags[tag] = [self]
+
         ## </tags>
 
 
         ## runtime
 
         self.default_label = label
         self.pressed = False
@@ -126,97 +145,97 @@
             color_bd = self.color_bd_normal
             color_lbl = self.color_lbl_normal
         else:
             color_btn = self.color_btn_normal
             color_bd = self.color_bd_normal
             color_lbl = self.color_lbl_normal
 
-        Button.page.delete(f'Button_{self.id}')
+        Button._page.delete(f'Button_{self.id}')
 
         if self.visible:
 
             ## This overhead will be executed each time this function is called.
             ## It may be inefficient, but it makes the code cleaner.
             X, Y = self.get_anchor_loc('center')  # the center of the button
 
-            Button.page.create_rectangle(
+            Button._page.create_rectangle(
                 X - self.width/2, Y - self.height/2,
                 X + self.width/2, Y + self.height/2,
                 fill=color_btn, width=1, outline=color_bd,
                 tags=f'Button_{self.id}'
             )
-            Button.page.create_text(
+            Button._page.create_text(
                 X, Y,
                 text=self.label, font=self.label_font,
                 fill=color_lbl,
                 tags=f'Button_{self.id}'
             )
 
 
     def _hover(self):
 
         w2 = self.width/2
         h2 = self.height/2
         
-        x = Button.page.winfo_pointerx()
-        y = Button.page.winfo_pointery()
+        x = Button._page.winfo_pointerx()
+        y = Button._page.winfo_pointery()
 
         X, Y = self.get_anchor_loc('center')
 
         ## `True` if the mouse cursor is inside the button
         inside = (X-w2 <= x <= X+w2) and (Y-h2 <= y <= Y+h2)
 
         if inside and (not self.locked) and self.visible and (not self.hovered):
             self.hovered = True
             self._redraw()  # just redraw once here
 
         elif self.hovered and (not inside):
             self.hovered = False
             self._redraw()  # just redraw once here
 
-        ## reminder: don't put it right here because it will redraw regardless of the hovered state
+        ## reminder: don't put self._redraw below here because it will redraw regardless of the "hovered" state
         # self._redraw()
 
     @staticmethod
-    def hover_listener():
+    def _hover_listener():  # reminder: hover listeners don't need `e: _tk.Event` arg
         for button in Button.buttons.values():
             button._hover()
 
 
-    def press(self):
+    def _press(self):
         
-        x = Button.page.winfo_pointerx()
-        y = Button.page.winfo_pointery()
+        x = Button._page.winfo_pointerx()
+        y = Button._page.winfo_pointery()
 
         X, Y = self.get_anchor_loc('center')
         w2 = self.width/2
         h2 = self.height/2
         inside = (X-w2 <= x <= X+w2) and (Y-h2 <= y <= Y+h2)
 
         if inside and (not self.locked) and self.visible:
             self.pressed = True
             self._redraw()
 
     @staticmethod
-    def press_listener():
+    def _press_listener(e: _tk.Event):
         for button in Button.buttons.values():
-            button.press()
+            button._press()
 
 
-    def release(self):
+    def _release(self):
         if self.pressed:
             self.pressed = False
             self._redraw()            
             if self.fn is not None:
                 self.fn()
 
     @staticmethod
-    def release_listener():
+    def _release_listener(e: _tk.Event):
         for button in list(Button.buttons.values()):
-            button.release()
+            button._release()
 
 
     def set_lock(self, locked: bool, /):
         if self.locked is not locked:
             self.locked = locked
             self._redraw()
     
@@ -410,15 +429,15 @@
         
         if self.tags is not None:
             for tag in self.tags:
                 Button.button_tags[tag].remove(self)
                 if Button.button_tags[tag] == []:
                     Button.button_tags.pop(tag)
 
-        Button.page.delete(f'Button_{self.id}')
+        Button._page.delete(f'Button_{self.id}')
     
     @staticmethod
     def destroy_by_id(id: str, /) -> None:
         Button.buttons[id].destroy()
 
     @staticmethod
     def destroy_by_tag(tag: str, /) -> None:
```

### Comparing `mykit-3.0.0/mykit/app/complex/biplot.py` & `mykit-4.1.0/mykit/app/complex/biplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import random as _random
+import tkinter as _tk
 from typing import (
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
-from mykit.app._runtime import Runtime as _Rt
 
+class Biplot:
 
-class Biplot(_Rt):
+    ## <runtime>
+
+    _page: _tk.Canvas = None
+    @staticmethod
+    def _set_page(page):
+        Biplot._page = page
 
     biplots: _Dict[str, 'Biplot'] = {}
     biplot_tags: _Dict[str, _List['Biplot']] = {}
 
+    ## </runtime>
+
     def __init__(
         self,
         points1: _List[_Tuple[float, float]] = [],
         points2: _List[_Tuple[float, float]] = [],
 
         xmin: _Optional[float] = None,
         xmax: _Optional[float] = None,
@@ -100,16 +108,22 @@
         ---
         
         ## Params
         - `xrange`: if `None` -> using the x-range from `points`
         - `yrange`: if `None` -> using the y-range from `points`
         """
 
-        if Biplot.page is None:
-            raise AssertionError('App has not been initialized.')
+        ## <dependencies check>
+
+        ## reminder: Biplot isn't actually a widget. it can be used as a utility
+        ##           outside App's purposes. so just use Biplot._set_page to achieve it.
+        if Biplot._page is None:
+            raise AssertionError('Can\'t use widgets before App initialized.')
+        
+        ## </dependencies check>
 
         self.points1 = points1
         self.points2 = points2
 
         self.xmin = xmin
         self.xmax = xmax
         self.ymin = ymin
@@ -175,37 +189,44 @@
         self.legends_font = legends_font
         self.legends_color = legends_color
         self.legends_shift_x = legends_shift_x
         self.legends_shift_y = legends_shift_y
 
         self.visible = visible
 
+        ## <id>
+
         ## `self.id`: to make sure that we can modify a specific instance without affecting the others
         if id is None:
             self.id = _random.randint(-10000, 10000)
             while self.id in Biplot.biplots:
                 self.id = _random.randint(-10000, 10000)
         else:
             self.id = id
             if self.id in Biplot.biplots:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
+        
         Biplot.biplots[self.id] = self
 
+        ## </id>
+
         ## <tags>
+
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
 
         if tags is not None:
             for tag in self.tags:
                 if tag in Biplot.biplot_tags:
                     Biplot.biplot_tags[tag].append(self)
                 else:
                     Biplot.biplot_tags[tag] = [self]
+        
         ## </tags>
 
 
         ## <preprocessing>
         self.plot_width = width*(1-pad_x)
         self.plot_height = height*(1-pad_y)
         ## </preprocessing>
@@ -243,189 +264,189 @@
             YMAX = self.ymax
 
         LEN_X = XMAX - XMIN
         LEN_Y = YMAX - YMIN
 
 
         ## title
-        Biplot.page.create_text(
+        Biplot._page.create_text(
             self.tl_x+self.width/2, self.tl_y,
             text=self.title, font=self.title_font, fill=self.title_color,
             tags=f'Biplot_{self.id}'
         )
 
 
         ## grids
         if self.show_grid:
 
             ## vertical grids
             for x in range(self.ntick_x):
                 X = self.tl_x + ((x+1)/self.ntick_x)*self.plot_width
-                Biplot.page.create_line(
+                Biplot._page.create_line(
                     X, self.tl_y+(self.height-self.plot_height),
                     X, self.tl_y+self.height,
                     fill=self.grid_color, width=1, tags=f'Biplot_{self.id}'
                 )
 
             ## horizontal grids
             for y in range(self.ntick_y):
                 Y = self.tl_y+self.height - ((y+1)/self.ntick_y)*self.plot_height
-                Biplot.page.create_line(
+                Biplot._page.create_line(
                     self.tl_x                , Y,
                     self.tl_x+self.plot_width, Y,
                     fill=self.grid_color, width=1, tags=f'Biplot_{self.id}'
                 )
 
 
         ## x-axis
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             self.tl_x           , self.tl_y+self.height,
             self.tl_x+self.width, self.tl_y+self.height,
             fill=self.axes_color, width=1, tags=f'Biplot_{self.id}'
         )
         ## x-axis arrow
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             self.tl_x+self.width-self.arrow_size, self.tl_y+self.height-self.arrow_size,
             self.tl_x+self.width                , self.tl_y+self.height,
             self.tl_x+self.width-self.arrow_size, self.tl_y+self.height+self.arrow_size,
             fill=self.axes_color, width=self.arrow_width, tags=f'Biplot_{self.id}'
         )
         ## x-axis label
-        Biplot.page.create_text(
+        Biplot._page.create_text(
             self.tl_x+self.width+self.x_axis_label_shift, self.tl_y+self.height,
             text=self.x_axis_label, anchor='w', fill=self.axes_label_color, font=self.x_axis_label_font, tags=f'Biplot_{self.id}'
         )
 
         ## y-axis
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             self.tl_x, self.tl_y,
             self.tl_x, self.tl_y+self.height,
             fill=self.axes_color, width=1, tags=f'Biplot_{self.id}'
         )
         ## y-axis arrow
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             self.tl_x-self.arrow_size, self.tl_y+self.arrow_size,
             self.tl_x, self.tl_y,
             self.tl_x+self.arrow_size, self.tl_y+self.arrow_size,
             fill=self.axes_color, width=self.arrow_width, tags=f'Biplot_{self.id}'
         )
         ## y-axis label
-        Biplot.page.create_text(
+        Biplot._page.create_text(
             self.tl_x, self.tl_y-self.y_axis_label_shift,
             text=self.y_axis_label, anchor='s', fill=self.axes_label_color, font=self.y_axis_label_font, tags=f'Biplot_{self.id}'
         )
 
 
         ## ticks
         if self.show_tick:
 
             ## x-axis ticks
             for x in range(self.ntick_x+1):
                 X = self.tl_x + (x/self.ntick_x)*self.plot_width
 
                 ## tick
-                Biplot.page.create_line(
+                Biplot._page.create_line(
                     X, self.tl_y+self.height-self.tick_len/2,
                     X, self.tl_y+self.height+self.tick_len/2,
                     fill=self.tick_color, width=1, tags=f'Biplot_{self.id}'
                 )
 
                 ## tick-label
                 _num = XMIN + (x/self.ntick_x)*(LEN_X)
                 if self.tick_x_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_x_prec)
                 text = self.tick_x_prefix + str(_num) + self.tick_x_suffix
-                Biplot.page.create_text(
+                Biplot._page.create_text(
                     X, self.tl_y+self.height+self.tick_len+self.tick_x_shift,
                     text=text, anchor='n', font=self.tick_x_font, fill=self.axes_label_color,
                     tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_ticks')
                 )
 
             ## y-axis ticks
             for y in range(self.ntick_y+1):
                 Y = self.tl_y+self.height - (y/self.ntick_y)*self.plot_height
 
                 ## tick
-                Biplot.page.create_line(
+                Biplot._page.create_line(
                     self.tl_x-self.tick_len/2, Y,
                     self.tl_x+self.tick_len/2, Y,
                     fill=self.tick_color, width=1, tags=f'Biplot_{self.id}'
                 )
 
                 ## tick-label
                 _num = YMIN + (y/self.ntick_y)*(LEN_Y)
                 if self.tick_y_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_y_prec)
                 text = self.tick_y_prefix + str(_num) + self.tick_y_suffix
-                Biplot.page.create_text(
+                Biplot._page.create_text(
                     self.tl_x-self.tick_len-self.tick_y_shift, Y,
                     text=text, anchor='e', font=self.tick_y_font, fill=self.axes_label_color,
                     tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_ticks')
                 )
 
 
         ## plot 1
         coords1 = []
         for x, y in self.points1:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords1.append((X, Y))
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             coords1,
             fill=self.plot_color1, width=self.plot_thick,
             tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_plot')
         )
 
         ## plot 2
         coords2 = []
         for x, y in self.points2:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords2.append((X, Y))
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             coords2,
             fill=self.plot_color2, width=self.plot_thick,
             tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_plot')
         )
 
         if self.show_points:
             for x, y in (coords1 + coords2):
-                Biplot.page.create_oval(
+                Biplot._page.create_oval(
                     x-self.points_rad/2, y-self.points_rad/2,
                     x+self.points_rad/2, y+self.points_rad/2,
                     fill=self.points_color, outline=self.points_border, width=1, tags=f'Biplot_{self.id}'
                 )
         
 
         ## legends
         if self.legend1 is not None:
-            Biplot.page.create_rectangle(
+            Biplot._page.create_rectangle(
                 self.tl_x+self.legends_shift_x, self.tl_y+self.legends_shift_y,
                 self.tl_x+self.legends_shift_x+self.legends_bar_width, self.tl_y+self.legends_shift_y+self.legends_bar_height,
                 fill=self.plot_color1, width=0, tags=f'Biplot_{self.id}'
             )
-            Biplot.page.create_text(
+            Biplot._page.create_text(
                 self.tl_x+self.legends_shift_x+self.legends_bar_width+self.legends_pad_x,
                 self.tl_y+self.legends_shift_y+self.legends_bar_height/2,
                 text=self.legend1, font=self.legends_font, justify='left', anchor='w', fill=self.legends_color,
                 tags=f'Biplot_{self.id}'
             )
         if self.legend2 is not None:
-            Biplot.page.create_rectangle(
+            Biplot._page.create_rectangle(
                 self.tl_x+self.legends_shift_x,
                 self.tl_y+self.legends_shift_y+self.legends_pad_y,
                 self.tl_x+self.legends_shift_x+self.legends_bar_width,
                 self.tl_y+self.legends_shift_y+self.legends_pad_y+self.legends_bar_height,
                 fill=self.plot_color2, width=0, tags=f'Biplot_{self.id}'
             )
-            Biplot.page.create_text(
+            Biplot._page.create_text(
                 self.tl_x+self.legends_shift_x+self.legends_bar_width+self.legends_pad_x,
                 self.tl_y+self.legends_shift_y+self.legends_pad_y+self.legends_bar_height/2,
                 text=self.legend2, font=self.legends_font, justify='left', anchor='w', fill=self.legends_color,
                 tags=f'Biplot_{self.id}'
             )
 
     def redraw_plot(self, points1: _List[_Tuple[float, float]], points2: _List[_Tuple[float, float]], /) -> None:
@@ -469,30 +490,30 @@
         ## LEN_X and LEN_Y can't be zero
         LEN_X = max(10**(-self.tick_x_prec), XMAX - XMIN)
         LEN_Y = max(10**(-self.tick_y_prec), YMAX - YMIN)
 
 
         ## redraw the ticks
 
-        Biplot.page.delete(f'Biplot_{self.id}_ticks')
+        Biplot._page.delete(f'Biplot_{self.id}_ticks')
 
         if self.show_tick:
 
             ## x-axis ticks
             for x in range(self.ntick_x+1):
                 X = self.tl_x + (x/self.ntick_x)*self.plot_width
 
                 ## tick-label
                 _num = XMIN + (x/self.ntick_x)*(LEN_X)
                 if self.tick_x_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_x_prec)
                 text = self.tick_x_prefix + str(_num) + self.tick_x_suffix
-                Biplot.page.create_text(
+                Biplot._page.create_text(
                     X, self.tl_y+self.height+self.tick_len+self.tick_x_shift,
                     text=text, anchor='n', font=self.tick_x_font, fill=self.axes_label_color,
                     tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_ticks')
                 )
 
             ## y-axis ticks
             for y in range(self.ntick_y+1):
@@ -501,44 +522,44 @@
                 ## tick-label
                 _num = YMIN + (y/self.ntick_y)*(LEN_Y)
                 if self.tick_y_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_y_prec)
                 text = self.tick_y_prefix + str(_num) + self.tick_y_suffix
-                Biplot.page.create_text(
+                Biplot._page.create_text(
                     self.tl_x-self.tick_len-self.tick_y_shift, Y,
                     text=text, anchor='e', font=self.tick_y_font, fill=self.axes_label_color,
                     tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_ticks')
                 )
 
 
         ## redraw the plot
 
-        Biplot.page.delete(f'Biplot_{self.id}_plot')
+        Biplot._page.delete(f'Biplot_{self.id}_plot')
 
         ## plot 1
         coords1 = []
         for x, y in self.points1:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords1.append((X, Y))
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             coords1,
             fill=self.plot_color1, width=self.plot_thick,
             tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_plot')
         )
 
         ## plot 2
         coords2 = []
         for x, y in self.points2:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords2.append((X, Y))
-        Biplot.page.create_line(
+        Biplot._page.create_line(
             coords2,
             fill=self.plot_color2, width=self.plot_thick,
             tags=(f'Biplot_{self.id}', f'Biplot_{self.id}_plot')
         )
 
     def shift_plot(self, new_points1: _List[_Tuple[float, float]], new_points2: _List[_Tuple[float, float]], /) -> None:
         """
```

### Comparing `mykit-3.0.0/mykit/app/complex/plot.py` & `mykit-4.1.0/mykit/app/complex/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import random as _random
+import tkinter as _tk
 from typing import (
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
-from mykit.app._runtime import Runtime as _Rt
 
+class Plot:
 
-class Plot(_Rt):
+    ## <runtime>
+
+    _page: _tk.Canvas = None
+    @staticmethod
+    def _set_page(page):
+        Plot._page = page
 
     plots: _Dict[str, 'Plot'] = {}
     plot_tags: _Dict[str, _List['Plot']] = {}
 
+    ## </runtime>
+
     def __init__(
         self,
         points: _List[_Tuple[float, float]] = [],
 
         xmin: _Optional[float] = None,
         xmax: _Optional[float] = None,
         ymin: _Optional[float] = None,
@@ -86,16 +94,22 @@
         ---
 
         ## Params
         - `xrange`: if `None` -> using the x-range from `points`
         - `yrange`: if `None` -> using the y-range from `points`
         """
 
-        if Plot.page is None:
-            raise AssertionError('App has not been initialized.')
+        ## <dependencies check>
+
+        ## reminder: Plot isn't actually a widget. it can be used as a utility
+        ##           outside App's purposes. so just use Plot._set_page to achieve it.
+        if Plot._page is None:
+            raise AssertionError('Can\'t use widgets before App initialized.')
+        
+        ## </dependencies check>
 
         self.points = points
 
         self.xmin = xmin
         self.xmax = xmax
         self.ymin = ymin
         self.ymax = ymax
@@ -148,37 +162,44 @@
         self.show_points = show_points
         self.points_rad = points_rad
         self.points_color = points_color
         self.points_border = points_border
 
         self.visibile = visible
 
+        ## <id>
+
         ## `self.id`: to make sure that we can modify a specific instance without affecting the others
         if id is None:
             self.id = _random.randint(-10000, 10000)
             while self.id in Plot.plots:
                 self.id = _random.randint(-10000, 10000)
         else:
             self.id = id
             if self.id in Plot.plots:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
+        
         Plot.plots[self.id] = self
 
+        ## </id>
+
         ## <tags>
+        
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
 
         if tags is not None:
             for tag in self.tags:
                 if tag in Plot.plot_tags:
                     Plot.plot_tags[tag].append(self)
                 else:
                     Plot.plot_tags[tag] = [self]
+        
         ## </tags>
 
 
         ## <preprocessing>
         self.plot_width = width*(1-pad_x)
         self.plot_height = height*(1-pad_y)
         ## </preprocessing>
@@ -215,149 +236,149 @@
             YMAX = self.ymax
 
         LEN_X = XMAX - XMIN
         LEN_Y = YMAX - YMIN
 
 
         ## title
-        Plot.page.create_text(
+        Plot._page.create_text(
             self.tl_x+self.width/2, self.tl_y,
             text=self.title, font=self.title_font, fill=self.title_color,
             tags=f'Plot_{self.id}'
         )
 
 
         ## grids
         if self.show_grid:
 
             ## vertical grids
             for x in range(self.ntick_x):
                 X = self.tl_x + ((x+1)/self.ntick_x)*self.plot_width
-                Plot.page.create_line(
+                Plot._page.create_line(
                     X, self.tl_y+(self.height-self.plot_height),
                     X, self.tl_y+self.height,
                     fill=self.grid_color, width=1, tags=f'Plot_{self.id}'
                 )
 
             ## horizontal grids
             for y in range(self.ntick_y):
                 Y = self.tl_y+self.height - ((y+1)/self.ntick_y)*self.plot_height
-                Plot.page.create_line(
+                Plot._page.create_line(
                     self.tl_x                , Y,
                     self.tl_x+self.plot_width, Y,
                     fill=self.grid_color, width=1, tags=f'Plot_{self.id}'
                 )
 
 
         ## x-axis
-        Plot.page.create_line(
+        Plot._page.create_line(
             self.tl_x           , self.tl_y+self.height,
             self.tl_x+self.width, self.tl_y+self.height,
             fill=self.axes_color, width=1, tags=f'Plot_{self.id}'
         )
         ## x-axis arrow
-        Plot.page.create_line(
+        Plot._page.create_line(
             self.tl_x+self.width-self.arrow_size, self.tl_y+self.height-self.arrow_size,
             self.tl_x+self.width                , self.tl_y+self.height,
             self.tl_x+self.width-self.arrow_size, self.tl_y+self.height+self.arrow_size,
             fill=self.axes_color, width=self.arrow_width, tags=f'Plot_{self.id}'
         )
         ## x-axis label
-        Plot.page.create_text(
+        Plot._page.create_text(
             self.tl_x+self.width+self.x_axis_label_shift, self.tl_y+self.height,
             text=self.x_axis_label, anchor='w', fill=self.axes_label_color, font=self.x_axis_label_font, tags=f'Plot_{self.id}'
         )
 
         ## y-axis
-        Plot.page.create_line(
+        Plot._page.create_line(
             self.tl_x, self.tl_y,
             self.tl_x, self.tl_y+self.height,
             fill=self.axes_color, width=1, tags=f'Plot_{self.id}'
         )
         ## y-axis arrow
-        Plot.page.create_line(
+        Plot._page.create_line(
             self.tl_x-self.arrow_size, self.tl_y+self.arrow_size,
             self.tl_x, self.tl_y,
             self.tl_x+self.arrow_size, self.tl_y+self.arrow_size,
             fill=self.axes_color, width=self.arrow_width, tags=f'Plot_{self.id}'
         )
         ## y-axis label
-        Plot.page.create_text(
+        Plot._page.create_text(
             self.tl_x, self.tl_y-self.y_axis_label_shift,
             text=self.y_axis_label, anchor='s', fill=self.axes_label_color, font=self.y_axis_label_font, tags=f'Plot_{self.id}'
         )
 
 
         ## ticks
         if self.show_tick:
 
             ## x-axis ticks
             for x in range(self.ntick_x+1):
                 X = self.tl_x + (x/self.ntick_x)*self.plot_width
 
                 ## tick
-                Plot.page.create_line(
+                Plot._page.create_line(
                     X, self.tl_y+self.height-self.tick_len/2,
                     X, self.tl_y+self.height+self.tick_len/2,
                     fill=self.tick_color, width=1, tags=f'Plot_{self.id}'
                 )
 
                 ## tick-label
                 _num = XMIN + (x/self.ntick_x)*(LEN_X)
                 if self.tick_x_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_x_prec)
                 text = self.tick_x_prefix + str(_num) + self.tick_x_suffix
-                Plot.page.create_text(
+                Plot._page.create_text(
                     X, self.tl_y+self.height+self.tick_len+self.tick_x_shift,
                     text=text, anchor='n', font=self.tick_x_font, fill=self.axes_label_color,
                     tags=(f'Plot_{self.id}', f'Plot_{self.id}_ticks')
                 )
 
             ## y-axis ticks
             for y in range(self.ntick_y+1):
                 Y = self.tl_y+self.height - (y/self.ntick_y)*self.plot_height
 
                 ## tick
-                Plot.page.create_line(
+                Plot._page.create_line(
                     self.tl_x-self.tick_len/2, Y,
                     self.tl_x+self.tick_len/2, Y,
                     fill=self.tick_color, width=1, tags=f'Plot_{self.id}'
                 )
 
                 ## tick-label
                 _num = YMIN + (y/self.ntick_y)*(LEN_Y)
                 if self.tick_y_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_y_prec)
                 text = self.tick_y_prefix + str(_num) + self.tick_y_suffix
-                Plot.page.create_text(
+                Plot._page.create_text(
                     self.tl_x-self.tick_len-self.tick_y_shift, Y,
                     text=text, anchor='e', font=self.tick_y_font, fill=self.axes_label_color,
                     tags=(f'Plot_{self.id}', f'Plot_{self.id}_ticks')
                 )
 
 
         ## plot
         coords = []
         for x, y in self.points:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords.append((X, Y))
-        Plot.page.create_line(
+        Plot._page.create_line(
             coords,
             fill=self.plot_color, width=self.plot_thick,
             tags=(f'Plot_{self.id}', f'Plot_{self.id}_plot')
         )
 
         if self.show_points:
             for x, y in coords:
-                Plot.page.create_oval(
+                Plot._page.create_oval(
                     x-self.points_rad/2, y-self.points_rad/2,
                     x+self.points_rad/2, y+self.points_rad/2,
                     fill=self.points_color, outline=self.points_border, width=1, tags=f'Plot_{self.id}'
                 )
     
     def redraw_plot(self, points: _List[_Tuple[float, float]], /) -> None:
         """
@@ -398,30 +419,30 @@
         ## LEN_X and LEN_Y can't be zero
         LEN_X = max(10**(-self.tick_x_prec), XMAX - XMIN)
         LEN_Y = max(10**(-self.tick_y_prec), YMAX - YMIN)
 
 
         ## redraw the ticks
 
-        Plot.page.delete(f'Plot_{self.id}_ticks')
+        Plot._page.delete(f'Plot_{self.id}_ticks')
 
         if self.show_tick:
 
             ## x-axis ticks
             for x in range(self.ntick_x+1):
                 X = self.tl_x + (x/self.ntick_x)*self.plot_width
 
                 ## tick-label
                 _num = XMIN + (x/self.ntick_x)*(LEN_X)
                 if self.tick_x_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_x_prec)
                 text = self.tick_x_prefix + str(_num) + self.tick_x_suffix
-                Plot.page.create_text(
+                Plot._page.create_text(
                     X, self.tl_y+self.height+self.tick_len+self.tick_x_shift,
                     text=text, anchor='n', font=self.tick_x_font, fill=self.axes_label_color,
                     tags=(f'Plot_{self.id}', f'Plot_{self.id}_ticks')
                 )
 
             ## y-axis ticks
             for y in range(self.ntick_y+1):
@@ -430,31 +451,31 @@
                 ## tick-label
                 _num = YMIN + (y/self.ntick_y)*(LEN_Y)
                 if self.tick_y_prec == 0:
                     _num = int(_num)
                 else:
                     _num = round(_num, self.tick_y_prec)
                 text = self.tick_y_prefix + str(_num) + self.tick_y_suffix
-                Plot.page.create_text(
+                Plot._page.create_text(
                     self.tl_x-self.tick_len-self.tick_y_shift, Y,
                     text=text, anchor='e', font=self.tick_y_font, fill=self.axes_label_color,
                     tags=(f'Plot_{self.id}', f'Plot_{self.id}_ticks')
                 )
 
 
         ## redraw the plot
 
-        Plot.page.delete(f'Plot_{self.id}_plot')
+        Plot._page.delete(f'Plot_{self.id}_plot')
 
         coords = []
         for x, y in self.points:
             X = self.tl_x + (x - XMIN)*(self.plot_width/LEN_X)
             Y = self.tl_y + self.height - (y - YMIN)*(self.plot_height/LEN_Y)
             coords.append((X, Y))
-        Plot.page.create_line(
+        Plot._page.create_line(
             coords,
             fill=self.plot_color, width=self.plot_thick,
             tags=(f'Plot_{self.id}', f'Plot_{self.id}_plot')
         )
 
     def shift_plot(self, new_points: _List[_Tuple[float, float]], /) -> None:
         """
```

### Comparing `mykit-3.0.0/mykit/app/label.py` & `mykit-4.1.0/mykit/app/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     Literal as _Literal,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
 
+## reminder: Label is different because it uses tkinter.Label
+##           instead of tkinter.Canvas. Not sure if it'll be okay,
+##           but for now, let's go with it.  @June 18, 2023 - Nicholas
 class Label:
 
     labels: _Dict[str, 'Label'] = {}
     label_tags: _Dict[str, _List['Label']] = {}
 
     def __init__(
         self,
@@ -58,37 +61,46 @@
             wraplength=wraplength,
             padx=padx, pady=pady
         )
 
         if visible:
             self.label.place(x=x, y=y, anchor=anchor)
 
+
+        ## <id>
+
         ## self.id ensures that we can modify a specific instance without affecting the others
         if id is None:
             self.id = str(_random.randint(0, 100_000))
             while self.id in Label.labels:
                 self.id = str(_random.randint(0, 100_000))
         else:
             self.id = id
             if self.id in Label.labels:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
+        
         Label.labels[self.id] = self
 
+        ## </id>
+
+
         ## <tags>
+        
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
         
         if tags is not None:
             for tag in self.tags:
                 if tag in Label.label_tags:
                     Label.label_tags[tag].append(self)
                 else:
                     Label.label_tags[tag] = [self]
+        
         ## <tags>
 
 
     def set_text(self, text: _Optional[str], /):
         """if None -> set default text."""
 
         if text is None:
```

### Comparing `mykit-3.0.0/mykit/app/slider.py` & `mykit-4.1.0/mykit/app/slider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import random as _random
+import tkinter as _tk
 from typing import (
     Callable as _Callable,
     Dict as _Dict,
     List as _List,
     Literal as _Literal,
     Optional as _Optional,
     Tuple as _Tuple,
     Union as _Union
 )
 
-from mykit.app._runtime import Runtime as _Rt
 from mykit.kit.utils import minmax_normalization as _norm
 
 
-class _Slider(_Rt):
+class _Slider:
+
+    ## <runtime>
+
+    _page: _tk.Canvas = None
+    @staticmethod
+    def _set_page(page):
+        _Slider._page = page
 
     sliders: _Dict[str, '_Slider'] = {}
     slider_tags: _Dict[str, _List['_Slider']] = {}  # note that the horizontal and vertical sliders store the tags together
 
+    ## </runtime>
+
     def __init__(
         self,
         min: float = 0,
         max: float = 1,
         step: _Optional[float] = None,
         init: _Optional[float] = None,
         fn: _Optional[_Callable[[], None]] = None,
@@ -73,16 +82,20 @@
         - `x` and `y` is the position of the `anchor` (not the center of the button)
         - `tolerance`: to determine how closely the cursor needs to be to the slider's step values for it to move to a new value
 
         ## Docs
         - box color, width, and height should be provided if the box shown
         """
 
-        if _Slider.page is None:
-            raise AssertionError('App has not been initialized.')
+        ## <dependencies check>
+
+        if _Slider._page is None:
+            raise AssertionError('Can\'t use widgets before App initialized.')
+        
+        ## </dependencies check>
 
         self.min = min
         self.max = max
         self.step = step if step is not None else (max-min)/10
         self.init = init if init is not None else (max-min)/2
         self.fn = fn
 
@@ -121,71 +134,79 @@
         self.color_btn_hover = color_btn_hover
         self.color_btn_bd_normal = color_btn_bd_normal
         self.color_btn_bd_locked = color_btn_bd_locked
 
         self.locked = locked
         self.visible = visible
 
+        ## <id>
+
         ## self.id ensures that we can modify a specific instance without affecting the others
         if id is None:
             self.id = str(_random.randint(0, 100_000))
             while self.id in _Slider.sliders:
                 self.id = str(_random.randint(0, 100_000))
         else:
             self.id = id
             if self.id in _Slider.sliders:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
+        
         _Slider.sliders[self.id] = self
 
+        ## </id>
+
+
         ## <tags>
+
         if type(tags) is str:
             self.tags = [tags]
         elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
             self.tags = tags
         
         if tags is not None:
             for tag in self.tags:
                 if tag in _Slider.slider_tags:
                     _Slider.slider_tags[tag].append(self)
                 else:
                     _Slider.slider_tags[tag] = [self]
+
         ## </tags>
 
 
         ## runtime
 
         self.value = self.init
         self.prec = len(str(abs(self.step)).split('.')[1]) if '.' in str(self.step) else 0
         self.pressed = False
         self.hovered = False
 
 
     @staticmethod
-    def hover_listener():
+    def _hover_listener():  # reminder: hover listeners don't need `e: _tk.Event` arg
         for slider in _Slider.sliders.values():
             slider._hover()
 
     @staticmethod
-    def press_listener():
+    def _press_listener(e: _tk.Event):
         for slider in _Slider.sliders.values():
             slider._press()
 
     @staticmethod
-    def hold_listener():
+    def _hold_listener(e: _tk.Event):
         for slider in list(_Slider.sliders.values()):
             slider._hold()
     
 
     def _release(self):
         if self.pressed:
             self.pressed = False
             self._redraw()
 
     @staticmethod
-    def release_listener():
+    def _release_listener(e: _tk.Event):
         for slider in list(_Slider.sliders.values()):
             slider._release()
 
 
     def set_lock(self, locked: bool, /) -> None:
         if self.locked is not locked:
             self.locked = locked
@@ -390,15 +411,15 @@
 
         if self.tags is not None:
             for tag in self.tags:
                 _Slider.slider_tags[tag].remove(self)
                 if _Slider.slider_tags[tag] == []:
                     _Slider.slider_tags.pop(tag)
 
-        _Slider.page.delete(f'Slider_{self.id}')
+        _Slider._page.delete(f'Slider_{self.id}')
 
     @staticmethod
     def destroy_by_id(id: str, /) -> None:
         _Slider.sliders[id].destroy()
 
     @staticmethod
     def destroy_by_tag(tag: str, /) -> None:
@@ -501,64 +522,64 @@
             color_btn = self.color_btn_hover
             color_btn_bd = self.color_btn_bd_normal
         else:
             color_rod = self.color_rod_normal
             color_btn = self.color_btn_normal
             color_btn_bd = self.color_btn_bd_normal
 
-        self.page.delete(f'Slider_{self.id}')
+        _Slider._page.delete(f'Slider_{self.id}')
 
         if self.visible:
 
             X, Y = self.get_anchor_loc('center')
             w2 = self.width/2
             h2 = self.height/2
 
-            self.page.create_rectangle(
+            _Slider._page.create_rectangle(
                 X-w2, Y-h2,
                 X+w2, Y+h2,
                 fill=color_rod, width=0, tags=f'Slider_{self.id}'
             )
-            self.page.create_oval(
+            _Slider._page.create_oval(
                 X-w2+_norm(self.value, self.min, self.max)*self.width-self.btn_r, Y-self.btn_r,
                 X-w2+_norm(self.value, self.min, self.max)*self.width+self.btn_r, Y+self.btn_r,
                 fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
             )
 
             if self.show_label_box:
-                self.page.create_rectangle(
+                _Slider._page.create_rectangle(
                     X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
                     X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
                     fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
                 )
             if self.label is not None:
-                self.page.create_text(
+                _Slider._page.create_text(
                     X, Y-h2+self.label_y_shift,
                     text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
                 )
 
             if self.show_value_box:
-                self.page.create_rectangle(
+                _Slider._page.create_rectangle(
                     X+w2+self.value_box_x_shift-self.value_box_width/2, Y-self.value_box_height/2,
                     X+w2+self.value_box_x_shift+self.value_box_width/2, Y+self.value_box_height/2,
                     fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
                 )
             if self.show_value:
-                self.page.create_text(
+                _Slider._page.create_text(
                     X+w2+self.value_box_x_shift, Y,
                     text=self.value_prefix + str(self.value) + self.value_suffix,
                     font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
                 )
 
     def _hover(self):
 
         X, Y = self.get_anchor_loc('center')
 
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
+        x = _Slider._page.winfo_pointerx()
+        y = _Slider._page.winfo_pointery()
 
         ## button coordinate
         bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
         by = Y
         br = self.btn_r  # button radius
 
         ## `True` if the mouse cursor is inside the slider button
@@ -572,16 +593,16 @@
             self.hovered = False
             self._redraw()
 
     def _press(self):
 
         X, Y = self.get_anchor_loc('center')
 
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
+        x = _Slider._page.winfo_pointerx()
+        y = _Slider._page.winfo_pointery()
 
         bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
         by = Y
         br = self.btn_r
 
         inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
 
@@ -591,15 +612,15 @@
 
     def _hold(self):
 
         if self.pressed:
 
             X, _ = self.get_anchor_loc('center')
 
-            mousex = self.page.winfo_pointerx()
+            mousex = _Slider._page.winfo_pointerx()
             value = self.min + ((mousex - (X - self.width/2))/self.width)*(self.max - self.min)
 
             if self.prec == 0:
                 value = int(value)
             else:
                 value = round(value, self.prec)
 
@@ -709,64 +730,64 @@
             color_btn = self.color_btn_hover
             color_btn_bd = self.color_btn_bd_normal
         else:
             color_rod = self.color_rod_normal
             color_btn = self.color_btn_normal
             color_btn_bd = self.color_btn_bd_normal
 
-        self.page.delete(f'Slider_{self.id}')
+        _Slider._page.delete(f'Slider_{self.id}')
 
         if self.visible:
 
             X, Y = self.get_anchor_loc('center')
             w2 = self.width/2
             h2 = self.height/2
 
-            self.page.create_rectangle(
+            _Slider._page.create_rectangle(
                 X-w2, Y-h2,
                 X+w2, Y+h2,
                 fill=color_rod, width=0, tags=f'Slider_{self.id}'
             )
-            self.page.create_oval(
+            _Slider._page.create_oval(
                 X-self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height-self.btn_r,
                 X+self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height+self.btn_r,
                 fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
             )
 
             if self.show_label_box:
-                self.page.create_rectangle(
+                _Slider._page.create_rectangle(
                     X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
                     X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
                     fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
                 )
             if self.label is not None:
-                self.page.create_text(
+                _Slider._page.create_text(
                     X, Y-h2+self.label_y_shift,
                     text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
                 )
 
             if self.show_value_box:
-                self.page.create_rectangle(
+                _Slider._page.create_rectangle(
                     X-self.value_box_width/2, Y+h2+self.value_box_y_shift-self.value_box_height/2,
                     X+self.value_box_width/2, Y+h2+self.value_box_y_shift+self.value_box_height/2,
                     fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
                 )
             if self.show_value:
-                self.page.create_text(
+                _Slider._page.create_text(
                     X, Y+h2+self.value_box_y_shift,
                     text=self.value_prefix + str(self.value) + self.value_suffix,
                     font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
                 )
 
     def _hover(self):
 
         X, Y = self.get_anchor_loc('center')
 
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
+        x = _Slider._page.winfo_pointerx()
+        y = _Slider._page.winfo_pointery()
 
         bx = X
         by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
         br = self.btn_r
 
         inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
 
@@ -778,16 +799,16 @@
             self.hovered = False
             self._redraw()
 
     def _press(self):
 
         X, Y = self.get_anchor_loc('center')
 
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
+        x = _Slider._page.winfo_pointerx()
+        y = _Slider._page.winfo_pointery()
 
         bx = X
         by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
         br = self.btn_r
 
         inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
 
@@ -797,15 +818,15 @@
 
     def _hold(self):
 
         if self.pressed:
 
             _, Y = self.get_anchor_loc('center')
 
-            mousey = self.page.winfo_pointery()
+            mousey = _Slider._page.winfo_pointery()
             value = self.max - ((mousey - (Y - self.height/2))/self.height)*(self.max - self.min)
     
             if self.prec == 0:
                 value = int(value)
             else:
                 value = round(value, self.prec)
```

### Comparing `mykit-3.0.0/mykit/kit/color.py` & `mykit-4.1.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-4.1.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/ffmpeg.py` & `mykit-4.1.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/keycrate/__init__.py` & `mykit-4.1.0/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/math.py` & `mykit-4.1.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/neuralnet/dense.py` & `mykit-4.1.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/neuralnet/genetic.py` & `mykit-4.1.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/noise.py` & `mykit-4.1.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/path.py` & `mykit-4.1.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit/kit/time.py` & `mykit-4.1.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-3.0.0/mykit.egg-info/PKG-INFO` & `mykit-4.1.0/mykit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 3.0.0
+Version: 4.1.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -21,22 +21,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<!-- make the status easily visible -->
+[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+
+
 # myKit
 
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
-![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -61,14 +65,23 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 4.1.0 (June 21, 2023):
+    - NEW: in `/kit/utils.py`: `slowprint` and `print_screen`
+- 4.0.0 (June 18, 2023):
+    - Breaking changes:
+        - `LIB_DIR_PTH` in `mykit` replaced by `DIST_DIR_PTH`
+        - Changed `/app/` mechanism:
+            - removed `/app/_runtime.py`
+    - `.app.App.listen`: Added aliases for event listener types
+    - New: `/app/architecture`
 - 3.0.0 (June 17, 2023):
     - Breaking changes:
         - Changed `title` arg to `name` in `.app.App`
         - Now `/kit/keycrate` must be a .txt file, and the file must exist
         - Added `export` method to `.kit.keycrate.KeyCrate`
     - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
@@ -116,13 +129,13 @@
     - transform `/kit/text/` -> `/kit/text.py`
     - transform `/kit/time/` -> `/kit/time.py`
     - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
-- To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
+- If you find any bugs, feel free to contribute by opening an issue or pull request. Thanks!
 
 
 ## License
 
 This project is licensed under the MIT license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mykit-3.0.0/mykit.egg-info/SOURCES.txt` & `mykit-4.1.0/mykit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 mykit.egg-info/PKG-INFO
 mykit.egg-info/SOURCES.txt
 mykit.egg-info/dependency_links.txt
 mykit.egg-info/entry_points.txt
 mykit.egg-info/requires.txt
 mykit.egg-info/top_level.txt
 mykit/app/__init__.py
-mykit/app/_runtime.py
 mykit/app/arrow.py
 mykit/app/button.py
 mykit/app/label.py
 mykit/app/slider.py
+mykit/app/architecture/__init__.py
+mykit/app/architecture/eventdriven.py
 mykit/app/complex/biplot.py
 mykit/app/complex/plot.py
 mykit/kit/color.py
 mykit/kit/ffmpeg.py
 mykit/kit/math.py
 mykit/kit/noise.py
 mykit/kit/path.py
```

### Comparing `mykit-3.0.0/pyproject.toml` & `mykit-4.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "3.0.0"
+version = "4.1.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
@@ -33,14 +33,15 @@
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "assets*",
     "tests*",
     "demo*",
+    "docs*",
 ]
 
 
 [project.urls]
 documentation = "https://nvfp.github.io/mykit/docs"
 "report bugs" = "https://github.com/nvfp/mykit/issues"
 repo = "https://github.com/nvfp/mykit"
```

