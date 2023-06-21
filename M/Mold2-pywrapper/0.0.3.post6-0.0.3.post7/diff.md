# Comparing `tmp/Mold2_pywrapper-0.0.3.post6.tar.gz` & `tmp/Mold2_pywrapper-0.0.3.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mold2_pywrapper-0.0.3.post6.tar", last modified: Wed Jun 21 13:29:08 2023, max compression
+gzip compressed data, was "Mold2_pywrapper-0.0.3.post7.tar", last modified: Wed Jun 21 14:27:12 2023, max compression
```

## Comparing `Mold2_pywrapper-0.0.3.post6.tar` & `Mold2_pywrapper-0.0.3.post7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.593406 Mold2_pywrapper-0.0.3.post6/
--rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post6/LICENSE
--rw-rw-rw-   0        0        0     4964 2023-06-21 13:29:08.594396 Mold2_pywrapper-0.0.3.post6/PKG-INFO
--rw-rw-rw-   0        0        0     4047 2023-02-07 12:55:23.000000 Mold2_pywrapper-0.0.3.post6/README.md
--rw-rw-rw-   0        0        0     1301 2023-06-21 13:29:08.599293 Mold2_pywrapper-0.0.3.post6/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.566879 Mold2_pywrapper-0.0.3.post6/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.578910 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/
--rw-rw-rw-   0        0        0      127 2023-06-21 13:28:40.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    47122 2023-06-21 13:24:39.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/descriptors.json
--rw-rw-rw-   0        0        0    13993 2023-06-21 13:25:58.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/mold2_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.593406 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     4964 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 14:27:12.377226 Mold2_pywrapper-0.0.3.post7/
+-rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post7/LICENSE
+-rw-rw-rw-   0        0        0     5173 2023-06-21 14:27:12.378237 Mold2_pywrapper-0.0.3.post7/PKG-INFO
+-rw-rw-rw-   0        0        0     4256 2023-06-21 14:24:38.000000 Mold2_pywrapper-0.0.3.post7/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-21 14:27:12.379233 Mold2_pywrapper-0.0.3.post7/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:27:12.354713 Mold2_pywrapper-0.0.3.post7/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:27:12.359712 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/
+-rw-rw-rw-   0        0        0      127 2023-06-21 14:26:19.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    47122 2023-06-21 13:24:39.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/descriptors.json
+-rw-rw-rw-   0        0        0    14150 2023-06-21 14:19:53.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/mold2_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:27:12.377226 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     5173 2023-06-21 14:27:12.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-21 14:27:12.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:27:12.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-21 14:27:12.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-21 14:27:12.000000 Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/top_level.txt
```

### Comparing `Mold2_pywrapper-0.0.3.post6/LICENSE` & `Mold2_pywrapper-0.0.3.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post6/PKG-INFO` & `Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mold2_pywrapper
-Version: 0.0.3.post6
+Name: Mold2-pywrapper
+Version: 0.0.3.post7
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -18,14 +18,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: testing
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  
+
 # Mold² Python wrapper
 
 Python wrapper to ease the calculation of Mold2 molecular descriptors.
 
 ## Copyright notice
 
 Mold2 is a product designed and produced by the National Center for Toxicological
```

### Comparing `Mold2_pywrapper-0.0.3.post6/README.md` & `Mold2_pywrapper-0.0.3.post7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  
+
 # Mold² Python wrapper
 
 Python wrapper to ease the calculation of Mold2 molecular descriptors.
 
 ## Copyright notice
 
 Mold2 is a product designed and produced by the National Center for Toxicological
```

### Comparing `Mold2_pywrapper-0.0.3.post6/setup.cfg` & `Mold2_pywrapper-0.0.3.post7/setup.cfg`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/descriptors.json` & `Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/descriptors.json`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/mold2_wrapper.py` & `Mold2_pywrapper-0.0.3.post7/src/Mold2_pywrapper/mold2_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                                             'Mold2-Executable-File.zip'))
 
     def __init__(self, verbose: bool = True):
         """Instantiate a wrapper to calculate Mold2 molecular descriptors.
 
         :param verbose: Should details about the download of executables be printed out
         """
+        if platform not in ['win32', 'linux']:
+            raise RuntimeError(f'Mold2 descriptors can only be calculated on Windows and Linux platforms.')
         # Ensure executables are available
         self._download_executables(verbose)
 
     def __del__(self):
         """Remove downloaded executables."""
         if os.path.isdir(self._dir):
             shutil.rmtree(self._dir)
```

### Comparing `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/PKG-INFO` & `Mold2_pywrapper-0.0.3.post7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mold2-pywrapper
-Version: 0.0.3.post6
+Name: Mold2_pywrapper
+Version: 0.0.3.post7
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -18,14 +18,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: testing
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  
+
 # Mold² Python wrapper
 
 Python wrapper to ease the calculation of Mold2 molecular descriptors.
 
 ## Copyright notice
 
 Mold2 is a product designed and produced by the National Center for Toxicological
```

