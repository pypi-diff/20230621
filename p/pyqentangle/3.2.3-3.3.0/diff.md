# Comparing `tmp/pyqentangle-3.2.3.tar.gz` & `tmp/pyqentangle-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyqentangle-3.2.3.tar", last modified: Fri Sep 30 01:33:56 2022, max compression
+gzip compressed data, was "dist/pyqentangle-3.3.0.tar", last modified: Wed Jun 21 16:24:32 2023, max compression
```

## Comparing `pyqentangle-3.2.3.tar` & `pyqentangle-3.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.955548 pyqentangle-3.2.3/
--rw-r--r--   0 stephenhky   (501) staff       (20)      178 2022-09-23 14:54:14.000000 pyqentangle-3.2.3/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)     6624 2022-09-30 01:33:56.954078 pyqentangle-3.2.3/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     4645 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/README.md
--rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-09-22 14:45:30.000000 pyqentangle-3.2.3/pyproject.toml
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.929908 pyqentangle-3.2.3/pyqentangle/
--rw-r--r--   0 stephenhky   (501) staff       (20)      366 2022-06-13 19:06:49.000000 pyqentangle-3.2.3/pyqentangle/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     6504 2021-09-04 16:42:55.000000 pyqentangle-3.2.3/pyqentangle/continuous.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.938531 pyqentangle-3.2.3/pyqentangle/cythonmodule/
--rw-r--r--   0 stephenhky   (501) staff       (20)       61 2021-12-15 05:08:01.000000 pyqentangle-3.2.3/pyqentangle/cythonmodule/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      233 2021-09-04 16:42:55.000000 pyqentangle-3.2.3/pyqentangle/cythonmodule/interpolate.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   222815 2022-09-23 15:08:55.000000 pyqentangle-3.2.3/pyqentangle/cythonmodule/interpolate_nocheck.c
--rw-r--r--   0 stephenhky   (501) staff       (20)      651 2021-09-04 16:42:55.000000 pyqentangle-3.2.3/pyqentangle/cythonmodule/interpolate_nocheck.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)     4484 2022-06-13 19:10:02.000000 pyqentangle-3.2.3/pyqentangle/metrics.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.942503 pyqentangle-3.2.3/pyqentangle/quantumstates/
--rw-r--r--   0 stephenhky   (501) staff       (20)       49 2020-10-13 13:49:27.000000 pyqentangle-3.2.3/pyqentangle/quantumstates/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      138 2020-10-13 13:49:27.000000 pyqentangle-3.2.3/pyqentangle/quantumstates/bipartite.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2975 2021-09-04 16:42:55.000000 pyqentangle-3.2.3/pyqentangle/quantumstates/harmonics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3481 2021-09-04 16:42:55.000000 pyqentangle-3.2.3/pyqentangle/schmidt.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3618 2020-10-13 13:49:27.000000 pyqentangle-3.2.3/pyqentangle/tncompute.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      661 2020-10-13 13:49:27.000000 pyqentangle-3.2.3/pyqentangle/utils.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.932776 pyqentangle-3.2.3/pyqentangle.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)     6624 2022-09-30 01:33:56.000000 pyqentangle-3.2.3/pyqentangle.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)      972 2022-09-30 01:33:56.000000 pyqentangle-3.2.3/pyqentangle.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-09-30 01:33:56.000000 pyqentangle-3.2.3/pyqentangle.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-16 17:47:10.000000 pyqentangle-3.2.3/pyqentangle.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)       63 2022-09-30 01:33:56.000000 pyqentangle-3.2.3/pyqentangle.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       12 2022-09-30 01:33:56.000000 pyqentangle-3.2.3/pyqentangle.egg-info/top_level.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       63 2022-09-23 14:59:21.000000 pyqentangle-3.2.3/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       38 2022-09-30 01:33:56.955709 pyqentangle-3.2.3/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     2145 2022-09-30 01:30:44.000000 pyqentangle-3.2.3/setup.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 01:33:56.953086 pyqentangle-3.2.3/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)      318 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/testConcurrence.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1855 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/testContinuousEntanglement.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      803 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/testDiscreteEntanglement.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3795 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/testRedDenMat.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      747 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/test_continuous_complex.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      768 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/test_fullredden.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1318 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/test_harmonics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      809 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/test_interpolation.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1183 2022-06-13 19:06:49.000000 pyqentangle-3.2.3/test/test_metrics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2896 2022-05-28 21:29:26.000000 pyqentangle-3.2.3/test/test_partialtranspose.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.734476 pyqentangle-3.3.0/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      178 2022-09-23 14:54:14.000000 pyqentangle-3.3.0/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6727 2023-06-21 16:24:32.733531 pyqentangle-3.3.0/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4739 2023-06-21 16:22:58.000000 pyqentangle-3.3.0/README.md
+-rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-09-22 14:45:30.000000 pyqentangle-3.3.0/pyproject.toml
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.634116 pyqentangle-3.3.0/pyqentangle/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      366 2022-06-13 19:06:49.000000 pyqentangle-3.3.0/pyqentangle/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6506 2023-06-21 16:22:58.000000 pyqentangle-3.3.0/pyqentangle/continuous.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.694801 pyqentangle-3.3.0/pyqentangle/cythonmodule/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       27 2023-06-21 16:22:58.000000 pyqentangle-3.3.0/pyqentangle/cythonmodule/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      233 2021-09-04 16:42:55.000000 pyqentangle-3.3.0/pyqentangle/cythonmodule/interpolate.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   222815 2022-09-23 15:08:55.000000 pyqentangle-3.3.0/pyqentangle/cythonmodule/interpolate_nocheck.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)      651 2021-09-04 16:42:55.000000 pyqentangle-3.3.0/pyqentangle/cythonmodule/interpolate_nocheck.pyx
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4484 2022-06-13 19:10:02.000000 pyqentangle-3.3.0/pyqentangle/metrics.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.699633 pyqentangle-3.3.0/pyqentangle/quantumstates/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       49 2020-10-13 13:49:27.000000 pyqentangle-3.3.0/pyqentangle/quantumstates/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      138 2020-10-13 13:49:27.000000 pyqentangle-3.3.0/pyqentangle/quantumstates/bipartite.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2975 2021-09-04 16:42:55.000000 pyqentangle-3.3.0/pyqentangle/quantumstates/harmonics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3481 2021-09-04 16:42:55.000000 pyqentangle-3.3.0/pyqentangle/schmidt.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3618 2020-10-13 13:49:27.000000 pyqentangle-3.3.0/pyqentangle/tncompute.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      661 2020-10-13 13:49:27.000000 pyqentangle-3.3.0/pyqentangle/utils.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.650374 pyqentangle-3.3.0/pyqentangle.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6727 2023-06-21 16:24:31.000000 pyqentangle-3.3.0/pyqentangle.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)      972 2023-06-21 16:24:31.000000 pyqentangle-3.3.0/pyqentangle.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2023-06-21 16:24:31.000000 pyqentangle-3.3.0/pyqentangle.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-16 17:47:10.000000 pyqentangle-3.3.0/pyqentangle.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)       63 2023-06-21 16:24:31.000000 pyqentangle-3.3.0/pyqentangle.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       12 2023-06-21 16:24:31.000000 pyqentangle-3.3.0/pyqentangle.egg-info/top_level.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       63 2023-06-21 16:22:58.000000 pyqentangle-3.3.0/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       38 2023-06-21 16:24:32.734764 pyqentangle-3.3.0/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2359 2023-06-21 16:22:58.000000 pyqentangle-3.3.0/setup.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-21 16:24:32.730366 pyqentangle-3.3.0/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      318 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/testConcurrence.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1855 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/testContinuousEntanglement.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      803 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/testDiscreteEntanglement.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3795 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/testRedDenMat.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      747 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/test_continuous_complex.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      768 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/test_fullredden.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1318 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/test_harmonics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      809 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/test_interpolation.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1183 2022-06-13 19:06:49.000000 pyqentangle-3.3.0/test/test_metrics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2896 2022-05-28 21:29:26.000000 pyqentangle-3.3.0/test/test_partialtranspose.py
```

### Comparing `pyqentangle-3.2.3/PKG-INFO` & `pyqentangle-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqentangle
-Version: 3.2.3
+Version: 3.3.0
 Summary: Quantum Entanglement in Python
 Home-page: https://github.com/stephenhky/pyqentangle
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: # Quantum Entanglement in Python
         
@@ -19,14 +19,15 @@
         ## Version
         
         The releases of `pyqentangle` 2.x.x is incompatible with previous releases.
         
         The releases of `pyqentangle` 3.x.x is incompatible with previous releases.
         
         Since release 3.1.0, the support for Python 2.7 and 3.5 has been decomissioned.
+        Since release 3.3.0, support for Python 3.6 is diminished, but that for Python 3.11 is added.
         
         ## Installation
         
         This package can be installed using `pip`.
         
         ```
         >>> pip install -U pyqentangle
@@ -126,18 +127,18 @@
         
 Keywords: quantum physics Schmidt decompostion entanglement
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Description-Content-Type: text/markdown
```

### Comparing `pyqentangle-3.2.3/README.md` & `pyqentangle-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## Version
 
 The releases of `pyqentangle` 2.x.x is incompatible with previous releases.
 
 The releases of `pyqentangle` 3.x.x is incompatible with previous releases.
 
 Since release 3.1.0, the support for Python 2.7 and 3.5 has been decomissioned.
+Since release 3.3.0, support for Python 3.6 is diminished, but that for Python 3.11 is added.
 
 ## Installation
 
 This package can be installed using `pip`.
 
 ```
 >>> pip install -U pyqentangle
```

### Comparing `pyqentangle-3.2.3/pyqentangle/continuous.py` & `pyqentangle-3.3.0/pyqentangle/continuous.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     :return: a lambda function that takes a `numpy.ndarray` as the input parameter and calculate the values
     :type xarray: numpy.ndarray
     :type yarray: numpy.ndarray
     :rtype: function
     :raises: OutOfRangeException
     """
     return lambda xs: np.array(list(map(lambda x: numerical_continuous_interpolation(xarray, yarray, x), xs)),
-                               dtype=np.complex)
+                               dtype=np.complex_)
 
 
 def discretize_continuous_bipartitesys(fcn, x1_lo, x1_hi, x2_lo, x2_hi, nb_x1=100, nb_x2=100):
     """Find the discretized representation of the continuous bipartite system
 
     Given a function `fcn` (a function with two input variables),
     find the discretized representation of the bipartite system, with
@@ -85,15 +85,15 @@
     :type nb_x1: int
     :type nb_x2: int
     :rtype: numpy.ndarray
 
     """
     x1 = np.linspace(x1_lo, x1_hi, nb_x1)
     x2 = np.linspace(x2_lo, x2_hi, nb_x2)
-    tensor = np.zeros((len(x1), len(x2)), dtype=np.complex)
+    tensor = np.zeros((len(x1), len(x2)), dtype=np.complex_)
     for i, j in product(*map(range, tensor.shape)):
         tensor[i, j] = fcn(x1[i], x2[j])
     return tensor
 
 
 def continuous_schmidt_decomposition(fcn, x1_lo, x1_hi, x2_lo, x2_hi, nb_x1=100, nb_x2=100, keep=None,
                                      approach='tensornetwork'):
```

### Comparing `pyqentangle-3.2.3/pyqentangle/cythonmodule/interpolate_nocheck.c` & `pyqentangle-3.3.0/pyqentangle/cythonmodule/interpolate_nocheck.c`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/cythonmodule/interpolate_nocheck.pyx` & `pyqentangle-3.3.0/pyqentangle/cythonmodule/interpolate_nocheck.pyx`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/metrics.py` & `pyqentangle-3.3.0/pyqentangle/metrics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/quantumstates/harmonics.py` & `pyqentangle-3.3.0/pyqentangle/quantumstates/harmonics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/schmidt.py` & `pyqentangle-3.3.0/pyqentangle/schmidt.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/tncompute.py` & `pyqentangle-3.3.0/pyqentangle/tncompute.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle/utils.py` & `pyqentangle-3.3.0/pyqentangle/utils.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/pyqentangle.egg-info/PKG-INFO` & `pyqentangle-3.3.0/pyqentangle.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqentangle
-Version: 3.2.3
+Version: 3.3.0
 Summary: Quantum Entanglement in Python
 Home-page: https://github.com/stephenhky/pyqentangle
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: # Quantum Entanglement in Python
         
@@ -19,14 +19,15 @@
         ## Version
         
         The releases of `pyqentangle` 2.x.x is incompatible with previous releases.
         
         The releases of `pyqentangle` 3.x.x is incompatible with previous releases.
         
         Since release 3.1.0, the support for Python 2.7 and 3.5 has been decomissioned.
+        Since release 3.3.0, support for Python 3.6 is diminished, but that for Python 3.11 is added.
         
         ## Installation
         
         This package can be installed using `pip`.
         
         ```
         >>> pip install -U pyqentangle
@@ -126,18 +127,18 @@
         
 Keywords: quantum physics Schmidt decompostion entanglement
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Description-Content-Type: text/markdown
```

### Comparing `pyqentangle-3.2.3/pyqentangle.egg-info/SOURCES.txt` & `pyqentangle-3.3.0/pyqentangle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/setup.py` & `pyqentangle-3.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 from setuptools import setup
 import numpy as np
-from Cython.Build import cythonize
 
-
-ext_modules = cythonize(['pyqentangle/cythonmodule/interpolate_nocheck.pyx'])
+try:
+    from Cython.Build import cythonize
+    ext_modules = cythonize(['pyqentangle/cythonmodule/interpolate_nocheck.pyx'])
+except ImportError:
+    from setuptools import Extension
+    ext_modules = [
+        Extension('pyqentangle.cythonmodule.interpolate_nocheck', ['pyqentangle/cythonmodule/interpolate_nocheck.c'])
+    ]
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
@@ -19,28 +24,28 @@
 
 
 def install_requirements():
     return [package_string.strip() for package_string in open('requirements.txt', 'r')]
 
 
 setup(name='pyqentangle',
-      version="3.2.3",
+      version="3.3.0",
       description="Quantum Entanglement in Python",
       long_description=package_description(),
       long_description_content_type='text/markdown',
       classifiers=[
           "Topic :: Scientific/Engineering :: Physics",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Chemistry",
           "License :: OSI Approved :: MIT License",
-          "Programming Language :: Python :: 3.6",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "Programming Language :: Cython",
           "Programming Language :: C",
           "Intended Audience :: Science/Research",
           "Intended Audience :: Developers",
           "Intended Audience :: Education"
       ],
       keywords="quantum physics Schmidt decompostion entanglement",
```

### Comparing `pyqentangle-3.2.3/test/testContinuousEntanglement.py` & `pyqentangle-3.3.0/test/testContinuousEntanglement.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/testDiscreteEntanglement.py` & `pyqentangle-3.3.0/test/testDiscreteEntanglement.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/testRedDenMat.py` & `pyqentangle-3.3.0/test/testRedDenMat.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_continuous_complex.py` & `pyqentangle-3.3.0/test/test_continuous_complex.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_fullredden.py` & `pyqentangle-3.3.0/test/test_fullredden.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_harmonics.py` & `pyqentangle-3.3.0/test/test_harmonics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_interpolation.py` & `pyqentangle-3.3.0/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_metrics.py` & `pyqentangle-3.3.0/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.2.3/test/test_partialtranspose.py` & `pyqentangle-3.3.0/test/test_partialtranspose.py`

 * *Files identical despite different names*

