# Comparing `tmp/odb-plotter-0.5.4.tar.gz` & `tmp/odb-plotter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.5.4.tar", last modified: Sat Jun 10 00:10:04 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.0.tar", last modified: Wed Jun 21 18:29:22 2023, max compression
```

## Comparing `odb-plotter-0.5.4.tar` & `odb-plotter-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.5.4/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3587 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1662 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1194 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3587 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      144 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-10 00:10:04.000000 odb-plotter-0.5.4/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.4/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24794 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.5.4/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.4/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     3964 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    17751 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-10 00:10:04.280442 odb-plotter-0.5.4/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-06-09 23:40:46.000000 odb-plotter-0.5.4/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     7226 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2382 2023-06-10 00:09:22.000000 odb-plotter-0.5.4/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    28791 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     1925 2023-06-09 23:40:49.000000 odb-plotter-0.5.4/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.0/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3667 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1742 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1221 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.103066 odb-plotter-0.6.0/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.103066 odb-plotter-0.6.0/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3667 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      133 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.0/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.0/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.0/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    36497 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.0/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/writer.py
```

### Comparing `odb-plotter-0.5.4/LICENSE` & `odb-plotter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.4/PKG-INFO` & `odb-plotter-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.4
+Version: 0.6.0
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -63,14 +63,13 @@
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
+* 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
 * Upcoming:
-    * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
-    * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
-    * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
-    * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
-    * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
-    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
+    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
+    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
+    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
+    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.5.4/README.md` & `odb-plotter-0.6.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,13 @@
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
+* 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
 * Upcoming:
-    * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
-    * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
-    * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
-    * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
-    * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
-    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
+    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
+    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
+    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
+    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.5.4/pyproject.toml` & `odb-plotter-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [project]
 name = "odb-plotter"
 description = "Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer"
 readme = "README.md"
 license = {file = "LICENSE"}
-keywords = ["abaqus", "abq", "fea", "odb", "waam", "wa-ded", "visualization"]
-authors = [{name = "Clark Hensley", email = "clarkhensley@duck.com"}]
-maintainers = [{name = "Clark Hensley", email = "clarkhensley@duck.com"}]
+keywords = ["abaqus", "abq", "fea", "odb", "waam", "wa-ded", "visualization",]
+authors = [{name = "Clark Hensley", email = "clarkhensley@duck.com"},]
+maintainers = [{name = "Clark Hensley", email = "clarkhensley@duck.com"},]
 dependencies = [
 "platformdirs",
 "h5py",
 "numpy",
 "tomli>=1.1.0; python_version < '3.11'",
 "tomli_w",
 "pandas",
-"matplotlib",
-"pyreadline3; platform_system == 'Windows'",
 "pyvista",
+"pyreadline3; platform_system == 'Windows'",
 ]
-dynamic = ["version"]
+dynamic = ["version",]
 
 [project.urls]
 "Homepage" = "https://www.cmml.me.msstate.edu"
 "Bug Reports" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues"
 "Source" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter"
 
 [tool.setuptools]
-package-data = {odbp = ["data/views.toml", "data/config.toml", "py2_scripts/odb_to_npz.py", "py2_scripts/extract.py"]}
+package-data = {odbp = ["data/views.toml", "data/config.toml", "py2_scripts/converter.py", "py2_scripts/extractor.py", "py2_scripts/state_collector.py",]}
 
 [tool.setuptools.dynamic]
 version = {attr = "odbp.__version__"}
 
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools", "wheel",]
 build-backend = "setuptools.build_meta"
```

### Comparing `odb-plotter-0.5.4/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.0/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.5.4
+Version: 0.6.0
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -63,14 +63,13 @@
 ## Changelog
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
+* 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
 * Upcoming:
-    * 0.6.0: Improved extractor across all file types. Improved Odb object iteration.
-    * 0.7.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline
-    * 0.8.0: Parametrize input values such as nodes, nodesets, frames, steps, parts, and colors (both in the API and CLI).
-    * 0.9.0: Create two-dimensional plotting capabilities and sane defaults.
-    * 0.10.0: Improve PyVista: views, gifs, non-interactive image saving, leaving viewer, etc. Ensure functionality of Abaqus 2019
-    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding (or following) a publication.
+    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
+    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
+    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
+    * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.5.4/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.0/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 src/odb_plotter.egg-info/SOURCES.txt
 src/odb_plotter.egg-info/dependency_links.txt
 src/odb_plotter.egg-info/requires.txt
 src/odb_plotter.egg-info/top_level.txt
 src/odbp/__init__.py
 src/odbp/__main__.py
 src/odbp/cli.py
-src/odbp/npz_to_hdf.py
 src/odbp/odb.py
 src/odbp/odb_visualizer.py
-src/odbp/read_hdf5.py
+src/odbp/reader.py
 src/odbp/state.py
 src/odbp/util.py
+src/odbp/writer.py
 src/odbp/data/config.toml
 src/odbp/data/views.toml
-src/odbp/py2_scripts/extract.py
-src/odbp/py2_scripts/odb_to_npz.py
+src/odbp/py2_scripts/converter.py
+src/odbp/py2_scripts/extractor.py
+src/odbp/py2_scripts/state_collector.py
```

### Comparing `odb-plotter-0.5.4/src/odbp/cli.py` & `odb-plotter-0.6.0/src/odbp/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 import numpy as np
 import pandas as pd
-from typing import Any, Union, TextIO, List, Tuple, Dict
+from typing import Any, Union, TextIO, List, Tuple, Dict, Optional
 from .odb_visualizer import OdbVisualizer
 from .util import confirm
 from .state import CLIOptions, UserOptions, process_input, print_state, load_views_dict
 from odbp import __version__
 
 
 def cli() -> None:
@@ -132,15 +132,15 @@
 
     if user_input in odb_options:
         # process odb
         odb_path_valid: bool = False
         while not odb_path_valid:
             user_input = input("Please enter the path of the odb file: ")
             if(confirm(f"You entered {user_input}", "Is this correct", "yes")):
-                output: Union[bool, None] = state.select_odb(user_options, user_input)
+                output: Optional[bool] = state.select_odb(user_options, user_input)
                 if isinstance(output, bool):
                     print(f"Error: the file {user_input} could not be found")
 
                 else:
                     odb_path_valid = True
 
         gen_time_sample: bool = False
@@ -179,17 +179,17 @@
         user_input: str = input("Please enter the desired name of the generated .hdf5 file: ")
         if confirm(f"You entered {user_input}", "Is this correct", "yes"):
             state.odb_to_hdf(user_input)
             break
 
 
 def pre_process_data(state: OdbVisualizer, user_options: UserOptions):
-    meltpoint: Union[float, None] = None
-    low_temp: Union[float, None] = None
-    time_sample: Union[int, None] = None
+    meltpoint: Optional[float] = None
+    low_temp: Optional[float] = None
+    time_sample: Optional[int] = None
 
     if user_options.config_file_path is not None:
         config_file: TextIO
         with open(user_options.config_file_path, "rb") as config_file:
             config: Dict[str, Any] = tomllib.load(config_file)
 
         if "hdf_file_path" in config:
```

### Comparing `odb-plotter-0.5.4/src/odbp/data/config.toml` & `odb-plotter-0.6.0/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.4/src/odbp/npz_to_hdf.py` & `odb-plotter-0.6.0/src/odbp/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,15 @@
     node_coords_file: NPZFileType
     with np.load(node_coords_path) as node_coords_file:
         coordinate_data: NDArrayType = node_coords_file[
                 node_coords_file.files[0]
                 ]
 
     temps_dir: pathlib.Path = npz_dir / pathlib.Path("temps")
-    temp_dict: Dict[str, Dict[str, NDArrayType]] = dict()
-    root: pathlib.Path
-    files: List[pathlib.Path]
+    temp_dict: Dict[pathlib.Path, Dict[str, NDArrayType]] = dict()
     for root, _, files in os.walk(temps_dir):
         root = pathlib.Path(root)
         step_name: str = root.stem
         temp_dict[step_name] = dict()
         files.sort()
         file: pathlib.Path
         for file in files:
@@ -90,20 +88,21 @@
     hdf5_file: H5PYFileType
     with h5py.File(hdf_path, "w") as hdf5_file:
         # Temps/Coords
         step: str
         node_data: NDArrayType
         for step in temp_dict:
             i: int
-            items: Tuple[str, Dict[str, NDArrayType]]
+            items: Tuple[str, NDArrayType]
             for i, items in enumerate(temp_dict[step].items()):
                 file: str
                 node_data: NDArrayType
                 file, node_data = items
                 frame: str = pathlib.Path(file).stem
+                print(frame)
                 target_len: int = len(node_data)
                 hdf5_file.create_dataset(
                         f"nodes/{step}/{frame}",
                         data = np.hstack((
                             node_data,
                             np.vstack(
                                 np.full(
```

### Comparing `odb-plotter-0.5.4/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.0/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.5.4/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.6.0/src/odbp/py2_scripts/converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 """
-ODBPlotter odb_to_npz.py
+ODBPlotter convert.py
 
 ODBPlotter
 https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
 MIT License (c) 2023
 
 This is a Python 2 file which implements an Abaqus Python interface to
 convert data from within a .odb file into a hierarchical directory of .npz
@@ -18,14 +18,15 @@
 
 
 import os
 import pickle
 import numpy as np
 import argparse
 import multiprocessing
+import collections
 from odbAccess import openOdb
 
 
 def main():
     """
     Helper function to parse command-line arguments from subprocess.run
     and format these values to correctly convert the .odb to the .npz files.
@@ -38,44 +39,76 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(input_args, nargs="*")
     odb_path, pickle_path, result_path = vars(parser.parse_args())[input_args]
 
     # Try our best to manage Python 2 file handling
     pickle_file = open(pickle_path, "rb")
     try:
-        data_to_extract = pickle.load(pickle_file)
+        input_dict = pickle.load(pickle_file)
 
     finally:
         pickle_file.close()
 
     # Now we can remove the file
     os.remove(pickle_path)
 
-    nodesets = data_to_extract["nodesets"]
-    frames = data_to_extract["frames"]
-    num_cpus = data_to_extract["cpus"]
+    user_nodes = input_dict.get("nodes")
+    if isinstance(user_nodes, collections.Mapping):
+        temp_nodes = dict()
+        for key, val in user_nodes.items():
+            temp_nodes[str(key)] = val
+        user_nodes = temp_nodes
+
+    unicode_nodesets = input_dict.get("nodesets")
+    if unicode_nodesets is not None:
+        user_nodesets = list()
+        for nodeset in unicode_nodesets:
+            user_nodesets.append(str(nodeset))
+    else:
+        user_nodesets = None
+
+    user_frames = input_dict.get("frames")
+
+    unicode_parts = input_dict.get("parts")
+    if unicode_parts is not None:
+        user_parts = list()
+        for part in unicode_parts:
+            user_parts.append(str(part))
+    else:
+        user_parts = None
+
+    unicode_steps = input_dict.get("steps")
+    if unicode_steps is not None:
+        user_steps = list()
+        for step in unicode_steps:
+            user_steps.append(str(step))
+    else:
+        user_steps = None
+
+    coord_key = str(input_dict.get("coord_key", "COORD"))
+    temp_key = str(input_dict.get("temp_key", "NT11"))
+    num_cpus = int(input_dict.get("cpus"))
 
-    result_name = convert_odb_to_npz(odb_path, nodesets, frames, num_cpus)
-    result_file = open(result_path, "wb")
+    result_name = convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_frames, user_parts, user_steps, coord_key, temp_key, num_cpus)
     try:
+        result_file = open(result_path, "wb")
         pickle.dump(result_name, result_file)
     finally:
         result_file.close()
 
 
-
-def convert_odb_to_npz(odb_path, nodesets, frames, num_cpus):
+def convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_frames, user_parts, user_steps, coord_key, temp_key, num_cpus):
     """
     Based on the 4 lists given, convert the .odb data to .npz files
     odb_path: str path to the .odb file
-    nodes: list[int] which nodes to convert (default to all)
-    parts: list[str] which parts to convert (default to no specific part)
-    nodesets: list[str] which nodesets to convert (default to the first
-    nodeset)
+    user_parts: list[str] which parts to convert (default to all)
+    user_nodesets: list[str] which nodesets to convert (default to all)
+    user_nodes: list[int] which nodes to turn into a new nodeset (default to None)
     frames: list[int] which frames to convert (default to all)
+    user_steps: list[str] which steps to convert (default to alll)
 
     return the name of the directory of .npz files created
     """
 
     # Create the results directory
     parent_dir = os.path.join(os.getcwd(), "tmp_npz")
     if not os.path.exists(parent_dir):
@@ -85,76 +118,106 @@
     if not os.path.exists(temps_dir):
         os.mkdir(temps_dir)
 
     time_dir = os.path.join(parent_dir, "step_frame_times")
     if not os.path.exists(time_dir):
         os.mkdir(time_dir)
 
-    odb = openOdb(odb_path, readOnly=True)
+    try:
+        odb = openOdb(odb_path, readOnly=True)
 
-    steps = odb.steps
+        steps = odb.steps
 
-    base_times = [
-        (step_key, step_val.totalTime) for step_key, step_val in steps.items()
-        ]
-    
-    assembly = odb.rootAssembly
-    nodeset_keys = assembly.nodeSets.keys()
-    if nodesets is None:
-        nodesets = nodeset_keys
-    else:
-        for nodeset in nodesets:
-            if nodeset not in nodeset_keys:
-                raise ValueError(
-                    '"{0}" is not a valid nodeset key.' \
-                        'Possible values in this .odb are "{1}"'
-                .format(nodeset, nodeset_keys)
-                )
+        base_times = [
+            (step_key, step_val.totalTime) for step_key, step_val in steps.items()
+            ]
 
-    odb.close()
+        assembly = odb.rootAssembly
+
+        target_frames = set()
+        if user_steps is not None:
+            for step in user_steps:
+                step_data = steps[step]
+                for frame in step_data.frames:
+                    target_frames.add(frame.frameId)
+
+        if user_frames is not None:
+            for frame in user_frames:
+                target_frames.add(frame.frameId)
+
+        target_frames = sorted(list(target_frames))
+
+        if len(target_frames) == 0:
+            for step_data in steps.values():
+                for frame in step_data.frames:
+                    target_frames.append(frame.frameId) 
+
+        target_nodesets = set()
+        if user_nodes is not None:
+            if isinstance(user_nodes, collections.Mapping):
+                for key, val in user_nodes.items():
+                    assembly.NodeSetFromNodeLabels(name=key, nodeLabels=(val,))
+                    target_nodesets.add(key)
+            elif isinstance(user_nodes, collections.Iterable):
+                if isinstance(user_nodes[0], int):
+                    user_nodes = [user_nodes]
+                for i, val in enumerate(user_nodes):
+                    assembly.NodeSetFromNodeLabels(name=i, nodeLabels=(val,))
+                    target_nodesets.add(i)
+
+        if user_parts is not None:
+            for part in assembly.instances.keys():
+                for nodeset in assembly.instances[part].nodeSets:
+                    target_nodesets.append(nodeset)
+
+        if user_nodesets is not None:
+            for nodeset in user_nodesets:
+                target_nodesets.add(nodeset)
+
+        target_nodesets = sorted(list(target_nodesets))
 
-    for nodeset in nodesets:
+        if len(target_nodesets) == 0:
+            target_nodesets = list(assembly.nodeSets.keys())
+
+    finally:
+        odb.close()
+
+    for nodeset in target_nodesets:
         for step_key, base_time in base_times:
             coord_file = os.path.join(parent_dir, "node_coords.npz")
-            read_nodeset_coords(odb_path, nodeset, coord_file, step_key)
-            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset, num_cpus)
+            read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key)
+            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus)
 
     return parent_dir
 
 
-def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset, num_cpus):
+def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus):
     odb = openOdb(odb_path, readOnly=True)
     steps = odb.steps
 
     curr_step_dir = os.path.join(temps_dir, step_key)
     if not os.path.exists(curr_step_dir):
         os.mkdir(curr_step_dir)
 
-    if frames is not None:
-        max_frame = max(frames)
-
-    else:
-        max_frame = len(steps[step_key].frames)
+    max_frame = max(target_frames)
 
     max_pad = len(str(max_frame))
 
     manager = multiprocessing.Manager()
     frame_times = manager.list()
-    #frame_times = list()
     if len(steps[step_key].frames) > 0:
         idx_list = [i for i in range(len(steps[step_key].frames))]
         idx_list_len = len(idx_list)
-        idx_list_max = idx_list[-1]
         # TODO: what if the length isn't divisible by the number of processors (is it now?)
         final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
         odb.close()
 
         temp_procs = list()
         for idx_list in final_idx_list:
-            p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, frames, step_key, curr_step_dir, frame_times, base_time, nodeset))
+            p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key))
             p.start()
             temp_procs.append(p)
 
         for p in temp_procs:
             p.join()
 
         np.savez_compressed(
@@ -168,58 +231,58 @@
                 np.array(
                     frame_times
                     )
                 )
             )
 
 
-def read_single_frame_temp(odb_path, idx_list, max_pad, frames, step_key, curr_step_dir, frame_times, base_time, nodeset):
+def read_single_frame_temp(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key):
 
     odb = openOdb(odb_path, readOnly=True)
     steps = odb.steps
     assembly = odb.rootAssembly
 
     for idx in idx_list:
-        if frames is not None and idx not in frames:
+        if idx not in target_frames:
             continue
         
         frame = steps[step_key].frames[idx]
 
-        field = frame.fieldOutputs["NT11"].getSubset(region=assembly.nodeSets[nodeset])
+        field = frame.fieldOutputs[temp_key].getSubset(region=assembly.nodeSets[nodeset])
         frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
         node_temps = list()
         for item in field.values:
             temp = item.data
             node_temps.append(temp)
 
         num = str(idx + 1).zfill(max_pad)
         np.savez_compressed(
                 os.path.join(
                     curr_step_dir,
-                    "frame_{".format(num)
+                    "frame_{}".format(num)
                     ),
                 np.array(node_temps)
                 )
 
     odb.close()
 
 
-def read_nodeset_coords(odb_path, nodeset, coord_file, step_key):
+def read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key):
 
     # Only extract coordinates from the first given nodeset/step
     if not os.path.exists(coord_file):
 
         odb = openOdb(odb_path, readOnly=True)
         assembly = odb.rootAssembly
         steps = odb.steps
 
         frame = steps[step_key].frames[0]
 
         try:
-            coords = frame.fieldOutputs["COORD"].getSubset(region=assembly.nodeSets[nodeset])
+            coords = frame.fieldOutputs[coord_key].getSubset(region=assembly.nodeSets[nodeset])
 
             results_list = list()
             for item in coords.values:
                 node = item.nodeLabel
                 coord = item.data
                 xyz = [node]
                 for axis in coord:
```

### Comparing `odb-plotter-0.5.4/src/odbp/read_hdf5.py` & `odb-plotter-0.6.0/src/odbp/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 
 Originally written by CMML Member CJ Nguyen
 """
 
 import h5py
 import multiprocessing
 import pathlib
-import numpy as np
 import pandas as pd
 from typing import Tuple, List
-from .util import NDArrayType, DataFrameType, H5PYGroupType, H5PYFileType, MultiprocessingPoolType
+from .util import DataFrameType, H5PYFileType, MultiprocessingPoolType
 
 
 def get_odb_data(
-    hdf_path: pathlib.Path
+    hdf_path: pathlib.Path,
     cpus: int
     ) -> DataFrameType:
     """
     get_node_coords(hdf_path: pathlib.Path) -> DataFrameType
     return a data frame with nodes by integer index and floating point
     3-dimensional coordinates.
     """
@@ -32,15 +31,15 @@
     try:
         hdf_file: H5PYFileType
         with h5py.File(hdf_path) as hdf_file:
             step: str
             for step in hdf_file["nodes"].keys():
                 frame_name: str
                 # TODO dataclass
-                args_list: List[Tuple(H5PYFileType, str, str)] = [
+                args_list: List[Tuple[H5PYFileType, str, str]] = [
                         (hdf_path, step, frame_name)
                         for frame_name
                         in hdf_file["nodes"][step].keys() 
                         ]
 
                 results: List[DataFrameType]
                 pool: MultiprocessingPoolType
```

### Comparing `odb-plotter-0.5.4/src/odbp/state.py` & `odb-plotter-0.6.0/src/odbp/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import tomli as tomllib
 import sys
 import os
 import platformdirs
 import subprocess
 import pickle
 import pandas as pd
-from typing import Union, Any, TextIO, Tuple, List, Dict
+from typing import Union, Any, TextIO, Tuple, List, Dict, Optional
 from .odb_visualizer import OdbVisualizer
 from .util import confirm
 from odbp import __version__
 
 
 class UserOptions():
     """
@@ -31,15 +31,15 @@
         run_immediate: False
         """
         self.hdf_source_directory: str = "" 
         self.odb_source_directory: str = "" 
         self.results_directory: str = ""
         self.image_title: str = ""
         self.image_label: str = ""
-        self.config_file_path: Union[str, None] = None
+        self.config_file_path: Optional[str] = None
         self.run_immediate: bool = False
 
 
 class CLIOptions():
     """
     Struct to store cli options without repeating
     """
@@ -342,63 +342,15 @@
             else:
                 print("You may perform this conversion later with the \"convert\" command")
 
     return (state, user_options)
 
 
 def extract_from_file(args: argparse.Namespace) -> pd.DataFrame:
-    if not args.odb:
-        print("Error: You must supply the path to a .odb file from which to extract")
-        sys.exit(1)
-
-    state: OdbVisualizer
-    state, _ = generate_cli_settings(args)
-
-    odb_extract_script_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "py2_scripts", "extract.py")
-    temp_save_path = os.path.join(os.getcwd(), "temp.pickle")
-
-    # Because of the python3-2 cross-talk, we use strings of "None", unfortunately
-    parts: Union[List[str], None] = None
-    nodesets: Union[List[str], None] = None
-    nodes: Union[Dict[str, List[int]], None] = None
-    if hasattr(state, "parts"):
-        parts = state.parts
-
-    if hasattr(state, "nodesets"):
-        nodesets = state.nodesets
-
-    if hasattr(state, "nodes"):
-        nodes = state.nodes
-
-    # subprocess won't handle the Nones or dicts or lists well, so instead we pickle in the output path, and read in the python2 version
-    # They're all built-ins, so pickle should work
-    temp_file: TextIO
-    input_dict: Dict[str, Any] = {
-        "parts": parts,
-        "nodesets": nodesets,
-        "nodes": nodes,
-    }
-    # TODO Time Sample
-    with open(temp_save_path, "wb") as temp_file:
-        pickle.dump(input_dict, temp_file, protocol=2)
-    odb_extract_args: List[str] = [state.abaqus_program, "python", odb_extract_script_path, state.odb_file_path, temp_save_path]
-    subprocess.run(odb_extract_args, shell=True)
-
-    #odb_to_npz_args: List[str] = [self.abaqus_program, "python", odb_to_npz_script_path, os.path.join(os.getcwd(), self.odb_file_path), str(self.time_sample)]
-    #subprocess.run(odb_to_npz_args, shell=True)
-
-    return_data: pd.DataFrame
-    with open(temp_save_path, "rb") as temp_file:
-        # From the Pickle Spec, decoding numpy arrays from python 2 must use encoding="latin-1"
-        return_data = pd.DataFrame(pickle.load(temp_file, encoding="latin-1"))
-
-    if os.path.exists(temp_save_path):
-        os.remove(temp_save_path)
-
-    return return_data
+    pass
 
 
 def read_setting_dict(state: OdbVisualizer, user_options: UserOptions, settings_dict: "Dict[str, Any]") -> "Tuple[OdbVisualizer, UserOptions]":
     hdf_source_dir: str
     if "hdf_source_directory" in settings_dict:
         hdf_source_dir = os.path.abspath(settings_dict["hdf_source_directory"])
 
@@ -473,15 +425,15 @@
         else:
             user_options = output
 
         # If none of these values are set, read as many as are available out of the .toml config file
         # Otherwise, the file must have already been read
 
         # Search for the stored toml values for this hdf
-        config: Union[Dict[str, Any], None] = None
+        config: Optional[Dict[str, Any]] = None
         if user_options.config_file_path is None:
             print(f".toml config file for {state.hdf_file_path} could not be found")
         else:
             config_file: TextIO
             with open(user_options.config_file_path, "rb") as config_file:
                 config = tomllib.load(config_file)
```

### Comparing `odb-plotter-0.5.4/src/odbp/util.py` & `odb-plotter-0.6.0/src/odbp/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,44 +9,54 @@
 import pathlib
 import numpy as np
 import pandas as pd
 
 
 # Python 3.10+ version
 ####### Type Aliases for this Project
-#from typing import TypeAlias
+#from typing import TypeAlias, Optional
 #
 ## Lists that can be None, used for defaults of lists of frames or nodesets
-#NullableIntList: TypeAlias = list[int] | None
-#NullableStrList: TypeAlias = list[str] | None
-#
+#NullableIntList: TypeAlias = Optional[list[int]]
+#NullableStrList: TypeAlias = Optional[list[str]]
+#NodeType: TypeAlais = dict[str, list[int]] | list[list[int]] | list[int]
+#NullableNodeType: TypeAlias = Optional[NodeType]
 ## Types of large data-science types
 #NDArrayType: TypeAlias = np.ndarray
 #NPZFileType: TypeAlias = np.lib.npyio.NpzFile
-#DataFrameType: TypeAlias = pd.core.frame.DataFrame
+#DataFrameType: TypeAlias = pd.DataFrame
 #H5PYGroupType: TypeAlias = h5py._hl.group.Group
 #H5PYFileType: TypeAlias = h5py.File
 #MultiprocessingPoolType: TypeAlias = multiprocessing.Pool
 #
 ######
 
 # Python 3.6+ version
-from typing import Union, Tuple, List
-NullableIntList = Union[List[int], None]
-NullableStrList = Union[List[str], None]
+from typing import Union, Tuple, List, Optional, Dict
+NullableIntList = Optional[List[int]]
+NullableStrList = Optional[List[str]]
+NodeType = Union[
+    Dict[str, List[int]], List[List[int]], List[int]
+]
+NullableNodeType = Optional[NodeType]
 
 NDArrayType = np.ndarray
 NPZFileType = np.lib.npyio.NpzFile
-DataFrameType = pd.core.frame.DataFrame
-H5PYGroupType = h5py._hl.group.Group
+DataFrameType = pd.DataFrame
+H5PYGroupType = h5py.Group
 H5PYFileType = h5py.File
 MultiprocessingPoolType = multiprocessing.Pool
 
+# Magic # Constants
+ODB_MAGIC_NUM: bytes = b"HKSRD0"
+HDF_MAGIC_NUM: bytes = b"\x89HDF\r\n"
+
+
 
-def confirm(message: str, confirmation: str, default: "Union[str, None]" = None) -> bool:
+def confirm(message: str, confirmation: str, default: "Optional[str]" = None) -> bool:
     yes_vals: Union[Tuple[str, str], Tuple[str, str, str]] = ("yes", "y")
     no_vals: Union[Tuple[str, str], Tuple[str, str, str]] = ("no", "n")
     if isinstance(default, str):
         if default.lower() in yes_vals:
             yes_vals = ("yes", "y", "")
             confirmation += " (Y/n)? "
         elif default.lower() in no_vals:
```

