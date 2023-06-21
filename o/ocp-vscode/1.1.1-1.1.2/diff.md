# Comparing `tmp/ocp_vscode-1.1.1.tar.gz` & `tmp/ocp_vscode-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.1.1.tar", last modified: Wed Jun 21 07:13:26 2023, max compression
+gzip compressed data, was "ocp_vscode-1.1.2.tar", last modified: Wed Jun 21 19:02:24 2023, max compression
```

## Comparing `ocp_vscode-1.1.1.tar` & `ocp_vscode-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 07:13:26.153623 ocp_vscode-1.1.1/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.1.1/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 07:13:26.153677 ocp_vscode-1.1.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     5484 2023-06-21 06:51:24.000000 ocp_vscode-1.1.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 07:13:26.152886 ocp_vscode-1.1.1/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-17 10:13:52.000000 ocp_vscode-1.1.1/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-17 10:13:52.000000 ocp_vscode-1.1.1/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 07:30:58.000000 ocp_vscode-1.1.1/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-17 10:13:52.000000 ocp_vscode-1.1.1/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-17 10:13:52.000000 ocp_vscode-1.1.1/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-17 10:13:52.000000 ocp_vscode-1.1.1/ocp_vscode/finder.py
--rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 06:30:51.000000 ocp_vscode-1.1.1/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 07:13:26.153526 ocp_vscode-1.1.1/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-21 07:13:26.000000 ocp_vscode-1.1.1/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-21 07:13:26.153944 ocp_vscode-1.1.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-06-21 06:08:10.000000 ocp_vscode-1.1.1/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.718201 ocp_vscode-1.1.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.1.2/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 19:02:24.718261 ocp_vscode-1.1.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     5588 2023-06-21 18:27:01.000000 ocp_vscode-1.1.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.716998 ocp_vscode-1.1.2/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 07:30:58.000000 ocp_vscode-1.1.2/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 06:30:51.000000 ocp_vscode-1.1.2/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.718079 ocp_vscode-1.1.2/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 18:25:16.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-21 19:02:24.718533 ocp_vscode-1.1.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-06-21 18:17:17.000000 ocp_vscode-1.1.2/setup.py
```

### Comparing `ocp_vscode-1.1.1/LICENSE` & `ocp_vscode-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/PKG-INFO` & `ocp_vscode-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 1.1.1
+Version: 1.1.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.1/README.md` & `ocp_vscode-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 ## Installation
 
 ### Prerequisites
 
 -   A fairly recent version of Microsoft VS Code, e.g. 1.76.0 or newer
 -   The [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) installed in VS Code
 -   `python` and `pip` available in the Python enviroment that will be used for CAD development
+-   The command `git` needs to be available
 -   On a Silicon Apple computer `mamba`
 
 **Notes**:
 
 -   For VSCodium, the extension is not available in the VS code market place. You need to download the the vsix file from the [release folder](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases) and install it manually.
 -   Currently, on a Silicon Mac (ARM CPU), _OCP_ and _CadQuery_ can only be installed via `mamba` and Python 3.9 or 3.10. Prepare an environment with `mamba create -n code_cad python=3.9` or `mamba create -n code_cad python=3.10`.
 -   **BREAKING CHANGES**:
     -   IPython and the ipython extensions are not supported any more out of the box. Instead the Microsoft's Jupyter extension with ipykernel is supported. If you have the installation configs in your local VS Code settings.json file, you might want to remove the ipython installation commands.
     -   For the color maps, `CM` is replaced by `ColorMap` (to resolve the conflict with build123d `CM`)
 
 ### Installation
 
-1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.1.1_.
+1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.1.2_.
 
     Afterwards the OCP viewer is available in the VS Code sidebar:
 
     ![](screenshots/ocp_icon.png)
 
 2. Clicking on it shows the OCP CAD Viewer UI:
 
@@ -49,14 +50,15 @@
 
     The Quickstarts will also
 
     -   (optionally) install the the [Jupyter extension for VS Code from Microsoft](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
     -   start the OCP viewer
     -   create a demo file in a temporary folder to quickly see a simple usage example
 
+
 ## Usage
 
 ### Running code using Jupyter
 
 -   Start the _OCP CAD Viewer_ by pressing the green box-arrow button in the "Viewer Manager" section of the _OCP CAD Viewer_ sidebar
 -   Import ocp_vscode and the CAD library by using the paste button behing the library names in the "Viewer Manager" section
 -   Use the usual Run menu to run the code
@@ -77,24 +79,25 @@
 
 ### Library Manager
 
 You can also use "Library Manager" in the _OCP CAD Viewer_ sidebar to manage the Python libraries for _build123d_, _cadquery_, _ipython_ and _ocp_tessellate_ (Presse the green arrow whenhovering over a library to install/upgrade it)
 
 ### Extra topics
 
+-   [Quickstart experience on Windows](docs/quickstart.md)
 -   [Use Jupyter to execute code](docs/run.md)
 -   [Debug code with visual debugging](docs/debug.md)
 -   [Use the `show` command](docs/show.md)
 -   [Use the `show_object` command](docs/show_object.md)
 -   [Download examples for build123d or cadquery](docs/examples.md)
 -   [Use the build123d snippets](docs/snippets.md)
 
 ## Changes
 
-v1.1.1
+v1.1.2
 
 -   Added Visual debugging (including a toggle switch in the status bar)
 -   Added function `show_all` and `show_clear` for the visual debugging
 -   New (opinonated) Quickstart modes to install ever for build123d or CadQury with one click
 -   Websocket communication between Python and the VS Code extension
 -   Remove IPython support and introduce Jupyter / ipykernel support
 -   Rename ColorMap to BaseColorMap and CM to ColorMap
```

### Comparing `ocp_vscode-1.1.1/ocp_vscode/__init__.py` & `ocp_vscode-1.1.2/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/animation.py` & `ocp_vscode-1.1.2/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/colors.py` & `ocp_vscode-1.1.2/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/comms.py` & `ocp_vscode-1.1.2/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/config.py` & `ocp_vscode-1.1.2/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/finder.py` & `ocp_vscode-1.1.2/ocp_vscode/finder.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode/show.py` & `ocp_vscode-1.1.2/ocp_vscode/show.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.1/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.1.2/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 1.1.1
+Version: 1.1.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.1/setup.cfg` & `ocp_vscode-1.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.1
+current_version = 1.1.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.1.1/setup.py` & `ocp_vscode-1.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.1.1",
+    "version": "1.1.2",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "ocp-tessellate>=1.1.0,<1.2.0",
         "requests",
```

