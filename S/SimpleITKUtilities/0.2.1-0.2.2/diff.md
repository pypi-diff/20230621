# Comparing `tmp/SimpleITKUtilities-0.2.1.tar.gz` & `tmp/SimpleITKUtilities-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleITKUtilities-0.2.1.tar", last modified: Mon Jun 12 20:24:52 2023, max compression
+gzip compressed data, was "SimpleITKUtilities-0.2.2.tar", last modified: Wed Jun 21 18:43:47 2023, max compression
```

## Comparing `SimpleITKUtilities-0.2.1.tar` & `SimpleITKUtilities-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.952475 SimpleITKUtilities-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/SimpleITK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/SimpleITK/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/make_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/overlay_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/pyside.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/slice_by_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:24:52.952475 SimpleITKUtilities-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_pyside.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.000734 SimpleITKUtilities-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.004734 SimpleITKUtilities-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.000734 SimpleITKUtilities-0.2.2/SimpleITK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.004734 SimpleITKUtilities-0.2.2/SimpleITK/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 18:43:46.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/make_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/overlay_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/slice_by_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/SimpleITK/utilities/vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 18:43:46.000000 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-21 18:43:47.000000 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:43:46.000000 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 18:43:46.000000 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 18:43:46.000000 SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:47.008734 SimpleITKUtilities-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/test/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/test/test_pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-21 18:43:31.000000 SimpleITKUtilities-0.2.2/test/test_utilities.py
```

### Comparing `SimpleITKUtilities-0.2.1/.github/workflows/docs.yml` & `SimpleITKUtilities-0.2.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/.github/workflows/main.yml` & `SimpleITKUtilities-0.2.2/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[vtk,dask,pyside] -r test/requirements.txt
+        sudo apt-get update
         sudo apt install libegl1
 
     - name: Test with pytest
       env:
         QT_QPA_PLATFORM: offscreen
       run: |
         python -m pytest
@@ -77,8 +78,8 @@
         python -m twine check dist/*
         ls -la dist
     - name: Upload package
       if: github.event_name == 'push'
       uses: actions/upload-artifact@v3
       with:
         name: python-packages
-        path: dist
+        path: dist
```

### Comparing `SimpleITKUtilities-0.2.1/.github/workflows/publish.yml` & `SimpleITKUtilities-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/.pre-commit-config.yaml` & `SimpleITKUtilities-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/LICENSE` & `SimpleITKUtilities-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/PKG-INFO` & `SimpleITKUtilities-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SimpleITKUtilities-0.2.1/README.md` & `SimpleITKUtilities-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/Logger.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/Logger.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/__init__.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/dask.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/dask.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/fft.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/fft.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/make_isotropic.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/make_isotropic.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/overlay_bounding_boxes.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/overlay_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/pyside.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/pyside.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/resize.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/resize.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/slice_by_slice.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/SimpleITK/utilities/vtk.py` & `SimpleITKUtilities-0.2.2/SimpleITK/utilities/vtk.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         logger.warning(
             "VTK version <9 does not support direction matrix which is ignored"
         )
     else:
         vtk_image.SetDirectionMatrix(direction)
 
     # Set pixel data
-    depth_array = vtknp.numpy_to_vtk(sitk.GetArrayViewFromImage(image).ravel())
+    depth_array = vtknp.numpy_to_vtk(sitk.GetArrayFromImage(image).ravel())
     depth_array.SetNumberOfComponents(ncomp)
     vtk_image.GetPointData().SetScalars(depth_array)
 
     vtk_image.Modified()
     return vtk_image
```

### Comparing `SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/PKG-INFO` & `SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/SOURCES.txt` & `SimpleITKUtilities-0.2.2/SimpleITKUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/docs/Makefile` & `SimpleITKUtilities-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/docs/make.bat` & `SimpleITKUtilities-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/docs/source/conf.py` & `SimpleITKUtilities-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/pyproject.toml` & `SimpleITKUtilities-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/test/conftest.py` & `SimpleITKUtilities-0.2.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/test/test_dask.py` & `SimpleITKUtilities-0.2.2/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/test/test_pyside.py` & `SimpleITKUtilities-0.2.2/test/test_pyside.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2.1/test/test_utilities.py` & `SimpleITKUtilities-0.2.2/test/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import gc
 
 import SimpleITK as sitk
 import SimpleITK.utilities as sitkutils
 from numpy.testing import assert_allclose
 
 
 def test_Logger():
@@ -33,16 +34,23 @@
 
     for z in range(img.GetSize()[2]):
         assert img[0, 0, z] == z
 
 
 def test_sitktovtk():
     img = sitk.Image([10, 10, 5], sitk.sitkFloat32)
+    img = img + 42.0
     vtk_img = sitkutils.sitk2vtk(img)
 
+    # free the SimpleITK image's memory
+    img = None
+    gc.collect()
+
+    assert vtk_img.GetScalarComponentAsFloat(0, 0, 0, 0) == 42.0
+
 
 def test_fft_initialization():
     fixed_img = sitk.Image([1024, 512], sitk.sitkInt8)
 
     fixed_img[510:520, 255:265] = 10
 
     moving_img = sitk.Image([1024, 512], sitk.sitkInt8)
```

