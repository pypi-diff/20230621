# Comparing `tmp/Mold2_pywrapper-0.0.3.post5.tar.gz` & `tmp/Mold2_pywrapper-0.0.3.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mold2_pywrapper-0.0.3.post5.tar", last modified: Fri Jun 16 17:05:33 2023, max compression
+gzip compressed data, was "Mold2_pywrapper-0.0.3.post6.tar", last modified: Wed Jun 21 13:29:08 2023, max compression
```

## Comparing `Mold2_pywrapper-0.0.3.post5.tar` & `Mold2_pywrapper-0.0.3.post6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.948719 Mold2_pywrapper-0.0.3.post5/
--rw-rw-rw-   0        0        0     1100 2023-01-14 16:21:14.000000 Mold2_pywrapper-0.0.3.post5/LICENSE
--rw-rw-rw-   0        0        0     4964 2023-06-16 17:05:32.949697 Mold2_pywrapper-0.0.3.post5/PKG-INFO
--rw-rw-rw-   0        0        0     4047 2023-02-06 18:52:51.000000 Mold2_pywrapper-0.0.3.post5/README.md
--rw-rw-rw-   0        0        0     1301 2023-06-16 17:05:32.959473 Mold2_pywrapper-0.0.3.post5/setup.cfg
--rw-rw-rw-   0        0        0      123 2020-09-22 21:34:54.000000 Mold2_pywrapper-0.0.3.post5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.894950 Mold2_pywrapper-0.0.3.post5/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.911569 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/
--rw-rw-rw-   0        0        0      127 2023-06-16 17:04:00.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    47122 2023-06-16 16:57:59.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/descriptors.json
--rw-rw-rw-   0        0        0    14004 2023-06-16 17:01:25.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/mold2_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:05:32.945786 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     4964 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-16 17:05:32.000000 Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.593406 Mold2_pywrapper-0.0.3.post6/
+-rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post6/LICENSE
+-rw-rw-rw-   0        0        0     4964 2023-06-21 13:29:08.594396 Mold2_pywrapper-0.0.3.post6/PKG-INFO
+-rw-rw-rw-   0        0        0     4047 2023-02-07 12:55:23.000000 Mold2_pywrapper-0.0.3.post6/README.md
+-rw-rw-rw-   0        0        0     1301 2023-06-21 13:29:08.599293 Mold2_pywrapper-0.0.3.post6/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Mold2_pywrapper-0.0.3.post6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.566879 Mold2_pywrapper-0.0.3.post6/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.578910 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/
+-rw-rw-rw-   0        0        0      127 2023-06-21 13:28:40.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    47122 2023-06-21 13:24:39.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/descriptors.json
+-rw-rw-rw-   0        0        0    13993 2023-06-21 13:25:58.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/mold2_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:29:08.593406 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     4964 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-21 13:29:08.000000 Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/top_level.txt
```

### Comparing `Mold2_pywrapper-0.0.3.post5/LICENSE` & `Mold2_pywrapper-0.0.3.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post5/PKG-INFO` & `Mold2_pywrapper-0.0.3.post6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2_pywrapper
-Version: 0.0.3.post5
+Version: 0.0.3.post6
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Mold2_pywrapper-0.0.3.post5/README.md` & `Mold2_pywrapper-0.0.3.post6/README.md`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post5/setup.cfg` & `Mold2_pywrapper-0.0.3.post6/setup.cfg`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/descriptors.json` & `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/descriptors.json`

 * *Files identical despite different names*

### Comparing `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper/mold2_wrapper.py` & `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper/mold2_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 from rdkit import Chem
 from rdkit.Chem import AllChem
 
 
 class Mold2:
     """Mold2 wrapper to obtain molecular descriptors."""
 
+    # Default folder for Mold2 executables
+    _zipfile = os.path.abspath(os.path.join(pystow.join('Mold2').as_posix(),
+                                            'Mold2-Executable-File.zip'))
+
     def __init__(self, verbose: bool = True):
         """Instantiate a wrapper to calculate Mold2 molecular descriptors.
 
         :param verbose: Should details about the download of executables be printed out
         """
-        # Default folder for Mold2 executables
-        self._zipfile = os.path.abspath(os.path.join(pystow.join('Mold2').as_posix(),
-                                                     'Mold2-Executable-File.zip'))
         # Ensure executables are available
         self._download_executables(verbose)
 
     def __del__(self):
         """Remove downloaded executables."""
         if os.path.isdir(self._dir):
             shutil.rmtree(self._dir)
@@ -79,24 +80,25 @@
 
     def descriptor_details(self):
         # Lazy loading to avoid too large memory footprint
         if not hasattr(self, '_details'):
             self._parse_details()
         return self._details
 
-    def from_executable(self, zipfile_path: str) -> Mold2:
+    @staticmethod
+    def from_executable(zipfile_path: str) -> Mold2:
         """Instantiate a Mold2 object from the user-downloaded mold2 zip file containing binaries.
 
         The provided ZIP file is extracted, so that default instantiation of Mold2 is henceforth possible.
         The ZIP file must be downloaded from "https://www.fda.gov/science-research/bioinformatics-tools/mold2"
 
         :param zipfile_path: Path to the zip file containing Mold2 binaries
         :return: a Mold2 calculator object
         """
-        shutil.copy(zipfile_path, self._zipfile)
+        shutil.copy(zipfile_path, Mold2._zipfile)
         return Mold2()
 
     def _show_banner(self):
         """Print info message for citing."""
         print("""Mold2 calculates a large and diverse set of molecular descriptors encoding two-
 dimensional chemical structure information. Comparative analysis of Mold2 descriptors
 with those calculated from commercial software on several published datasets
@@ -247,15 +249,15 @@
         if data.iloc[0, 0] != 'D001':
             # Header is not provided if first molecule failed
             data.columns = [f'D{x:03d}' for x in range(1, 778)]
         else:
             data.columns = data.iloc[0, :]
             data.drop(index=0, inplace=True)
         data.reset_index(drop=True, inplace=True)
-        data = data.apply(lambda x: pd.to_numeric(x, errors='coerce'))
+        data = data.apply(pd.to_numeric, errors='coerce', axis=1)
         data = data.convert_dtypes()
         return data
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Caclulate Mold2 descriptors on one process.
 
         :param mols: RDkit molecules for which Mold2 descriptors should be calculated
```

### Comparing `Mold2_pywrapper-0.0.3.post5/src/Mold2_pywrapper.egg-info/PKG-INFO` & `Mold2_pywrapper-0.0.3.post6/src/Mold2_pywrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mold2-pywrapper
-Version: 0.0.3.post5
+Version: 0.0.3.post6
 Summary: Python wrapper for Mold2 descriptors
 Home-page: https://github.com/OlivierBeq/Mold2_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: mold2,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

