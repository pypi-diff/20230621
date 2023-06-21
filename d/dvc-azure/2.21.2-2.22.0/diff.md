# Comparing `tmp/dvc-azure-2.21.2.tar.gz` & `tmp/dvc-azure-2.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-azure-2.21.2.tar", last modified: Wed May 31 11:02:45 2023, max compression
+gzip compressed data, was "dvc-azure-2.22.0.tar", last modified: Wed Jun 21 05:56:06 2023, max compression
```

## Comparing `dvc-azure-2.21.2.tar` & `dvc-azure-2.22.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure/
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure/_dvc_azure_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/path.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/dvc_azure/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:02:45.935277 dvc-azure-2.21.2/dvc_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 11:02:45.000000 dvc-azure-2.21.2/dvc_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-31 11:02:45.939277 dvc-azure-2.21.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 11:02:25.000000 dvc-azure-2.21.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.717455 dvc-azure-2.22.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/dvc_azure/
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure/_dvc_azure_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/dvc_azure/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/dvc_azure/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 05:56:06.721455 dvc-azure-2.22.0/dvc_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-21 05:56:06.000000 dvc-azure-2.22.0/dvc_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-06-21 05:56:06.725456 dvc-azure-2.22.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 05:55:44.000000 dvc-azure-2.22.0/setup.py
```

### Comparing `dvc-azure-2.21.2/.github/workflows/benchmarks.yaml` & `dvc-azure-2.22.0/.github/workflows/benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/.github/workflows/release.yaml` & `dvc-azure-2.22.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/.github/workflows/tests.yaml` & `dvc-azure-2.22.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/.github/workflows/update-template.yaml` & `dvc-azure-2.22.0/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/.gitignore` & `dvc-azure-2.22.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/.pre-commit-config.yaml` & `dvc-azure-2.22.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/LICENSE` & `dvc-azure-2.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/PKG-INFO` & `dvc-azure-2.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-azure
-Version: 2.21.2
+Version: 2.22.0
 Summary: azure plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-azure
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-azure
 Keywords: dvc,azure
```

### Comparing `dvc-azure-2.21.2/dvc_azure/__init__.py` & `dvc-azure-2.22.0/dvc_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/dvc_azure/path.py` & `dvc-azure-2.22.0/dvc_azure/path.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/dvc_azure/tests/cloud.py` & `dvc-azure-2.22.0/dvc_azure/tests/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/dvc_azure/tests/fixtures.py` & `dvc-azure-2.22.0/dvc_azure/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/dvc_azure/tests/test_dvc.py` & `dvc-azure-2.22.0/dvc_azure/tests/test_dvc.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 @pytest.mark.xfail(
     reason="waiting for https://github.com/fsspec/adlfs/pull/333"
 )
 class TestImport(_TestImport):
     @pytest.fixture
     def stage_md5(self):
-        return "2aa17f8daa26996b3f7a4cf8888ac9ac"
+        return "ffe462bbb08432b7a1c3985fcf82ad3a"
 
     @pytest.fixture
     def is_object_storage(self):
         return True
 
     @pytest.fixture
     def dir_md5(self):
```

### Comparing `dvc-azure-2.21.2/dvc_azure.egg-info/PKG-INFO` & `dvc-azure-2.22.0/dvc_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-azure
-Version: 2.21.2
+Version: 2.22.0
 Summary: azure plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-azure
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-azure
 Keywords: dvc,azure
```

### Comparing `dvc-azure-2.21.2/dvc_azure.egg-info/SOURCES.txt` & `dvc-azure-2.22.0/dvc_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/dvc_azure.egg-info/requires.txt` & `dvc-azure-2.22.0/dvc_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/pyproject.toml` & `dvc-azure-2.22.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-azure-2.21.2/setup.cfg` & `dvc-azure-2.22.0/setup.cfg`

 * *Files identical despite different names*

