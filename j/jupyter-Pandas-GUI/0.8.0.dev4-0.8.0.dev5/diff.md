# Comparing `tmp/jupyter_Pandas_GUI-0.8.0.dev4.tar.gz` & `tmp/jupyter_Pandas_GUI-0.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev4.tar", last modified: Wed May 31 22:03:24 2023, max compression
+gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev5.tar", last modified: Wed Jun 21 20:39:29 2023, max compression
```

## Comparing `jupyter_Pandas_GUI-0.8.0.dev4.tar` & `jupyter_Pandas_GUI-0.8.0.dev5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev4/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9816 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9070 2023-05-31 21:59:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/README.md
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.258275 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9816 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-31 22:03:24.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49800 2023-05-24 21:34:46.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/fit_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/new_pandas_column_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/plot_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14252 2023-05-23 17:50:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-31 21:48:40.000000 jupyter_Pandas_GUI-0.8.0.dev4/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-21 20:39:29.186780 jupyter_Pandas_GUI-0.8.0.dev5/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev5/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10026 2023-06-21 20:39:29.186780 jupyter_Pandas_GUI-0.8.0.dev5/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9280 2023-06-19 15:56:14.000000 jupyter_Pandas_GUI-0.8.0.dev5/README.md
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-21 20:39:29.186780 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10026 2023-06-21 20:39:29.000000 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-06-21 20:39:29.000000 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-21 20:39:29.000000 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      151 2023-06-21 20:39:29.000000 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-06-21 20:39:29.000000 jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-21 20:39:29.186780 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49800 2023-05-24 21:34:46.000000 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/fit_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/new_pandas_column_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/plot_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14252 2023-05-23 17:50:14.000000 jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-21 20:39:29.186780 jupyter_Pandas_GUI-0.8.0.dev5/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1319 2023-06-19 15:55:09.000000 jupyter_Pandas_GUI-0.8.0.dev5/setup.py
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/LICENSE` & `jupyter_Pandas_GUI-0.8.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_Pandas_GUI
-Version: 0.8.0.dev4
+Version: 0.8.0.dev5
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -151,24 +151,25 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
-* 0.8.0dev (2023-5-)
+* 0.8.0dev (2023-6-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
   * Colab behavior has been inconsistent. To avoid problems for the time being 
     the user is required to copy the code from the textbox it is created in 
     and paste it into an empty code cell to run it.
   * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
     codes, so when copied and pasted output formatting is maintained.
   * Changes to avoid warnings caused by JSON having no representation for 
     floating point infinity and not-a-number.
+  * Requirements updates to reflect changes in the Jupyter ecosystem.
   * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
@@ -203,14 +204,16 @@
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
 ### Known issues
 * In Google Colabratory images in point styles buttons do not show up. This 
   is a related to a known [issue with
   Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
   depend on updates to Colab.
+* In Google Colabratory typset rendering of Latex in widgets is hit or miss.
+  It works most of the time in regular outputs and for plots. 
 
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/README.md` & `jupyter_Pandas_GUI-0.8.0.dev5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -132,24 +132,25 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
-* 0.8.0dev (2023-5-)
+* 0.8.0dev (2023-6-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
   * Colab behavior has been inconsistent. To avoid problems for the time being 
     the user is required to copy the code from the textbox it is created in 
     and paste it into an empty code cell to run it.
   * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
     codes, so when copied and pasted output formatting is maintained.
   * Changes to avoid warnings caused by JSON having no representation for 
     floating point infinity and not-a-number.
+  * Requirements updates to reflect changes in the Jupyter ecosystem.
   * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
@@ -184,14 +185,16 @@
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
 ### Known issues
 * In Google Colabratory images in point styles buttons do not show up. This 
   is a related to a known [issue with
   Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
   depend on updates to Colab.
+* In Google Colabratory typset rendering of Latex in widgets is hit or miss.
+  It works most of the time in regular outputs and for plots. 
 
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev5/jupyter_Pandas_GUI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-Pandas-GUI
-Version: 0.8.0.dev4
+Version: 0.8.0.dev5
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -151,24 +151,25 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
-* 0.8.0dev (2023-5-)
+* 0.8.0dev (2023-6-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
   * Colab behavior has been inconsistent. To avoid problems for the time being 
     the user is required to copy the code from the textbox it is created in 
     and paste it into an empty code cell to run it.
   * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
     codes, so when copied and pasted output formatting is maintained.
   * Changes to avoid warnings caused by JSON having no representation for 
     floating point infinity and not-a-number.
+  * Requirements updates to reflect changes in the Jupyter ecosystem.
   * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
@@ -203,14 +204,16 @@
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
 ### Known issues
 * In Google Colabratory images in point styles buttons do not show up. This 
   is a related to a known [issue with
   Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
   depend on updates to Colab.
+* In Google Colabratory typset rendering of Latex in widgets is hit or miss.
+  It works most of the time in regular outputs and for plots. 
 
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/__init__.py` & `jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/fit_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/fit_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/new_pandas_column_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/new_pandas_column_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/plot_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/plot_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/utils.py` & `jupyter_Pandas_GUI-0.8.0.dev5/pandas_GUI/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev4/setup.py` & `jupyter_Pandas_GUI-0.8.0.dev5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="jupyter_Pandas_GUI",
-    version="0.8.0dev4",
+    version="0.8.0.dev5",
     description="Pandas expression composers using Jupyter widgets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="fitting, data-analysis, plotting, learning to code",
     license="GPL-3.0+",
     packages=setuptools.find_packages(),
     package_data={},
     include_package_data=True,
     install_requires=[
         # 'python>=3.6',
         'jupyter>=1.0.0',
-        'jupyterlab>=3.6, <4.0',
+        'jupyterlab>=3.6,<4.0',
         'pandas>=1.5.2',
         'numpy>=1.23.0',
         'plotly>=5.5.0',
-        'ipywidgets>=7.6.2, <8.0',
+        'ipywidgets>=7.6.2',
         'JPSLUtils>=0.7.0',
         'lmfit>=1.1.0',
         'round-using-error>=1.2.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

