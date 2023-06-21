# Comparing `tmp/onedep_deposition-0.1.dev5.tar.gz` & `tmp/onedep_deposition-0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev5.tar", last modified: Tue Jun 20 13:28:07 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev6.tar", last modified: Wed Jun 21 13:40:39 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev5.tar` & `onedep_deposition-0.1.dev6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-20 13:28:07.659219 onedep_deposition-0.1.dev5/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev5/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-20 13:28:07.658846 onedep_deposition-0.1.dev5/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev5/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-20 13:28:07.654933 onedep_deposition-0.1.dev5/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-20 13:27:41.000000 onedep_deposition-0.1.dev5/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-20 13:28:07.658105 onedep_deposition-0.1.dev5/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev5/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    12637 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev5/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev5/onedep_deposition/decorators.py
--rw-r--r--   0 peisach    (502) staff       (20)    15104 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev5/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev5/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev5/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    12847 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev5/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev5/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-20 13:28:07.657434 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-20 13:28:07.000000 onedep_deposition-0.1.dev5/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev5/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-20 13:28:07.659317 onedep_deposition-0.1.dev5/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.906260 onedep_deposition-0.1.dev6/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev6/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-21 13:40:39.905965 onedep_deposition-0.1.dev6/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev6/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.902060 onedep_deposition-0.1.dev6/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-21 13:40:22.000000 onedep_deposition-0.1.dev6/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.905135 onedep_deposition-0.1.dev6/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev6/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12637 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/decorators.py
+-rw-r--r--   0 peisach    (502) staff       (20)    15148 2023-06-21 13:40:11.000000 onedep_deposition-0.1.dev6/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev6/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12847 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev6/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.904502 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev6/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-21 13:40:39.906349 onedep_deposition-0.1.dev6/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev5/LICENSE` & `onedep_deposition-0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/PKG-INFO` & `onedep_deposition-0.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_deposition
-Version: 0.1.dev5
+Version: 0.1.dev6
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev5/README.md` & `onedep_deposition-0.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev6/onedep_deposition/cli/cli.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/decorators.py` & `onedep_deposition-0.1.dev6/onedep_deposition/decorators.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev6/onedep_deposition/deposit_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     def _connect(self, hostname: str = None) -> None:
         if hostname:
             self._hostname = hostname
         self._rest_adapter = RestAdapter(self._hostname, self._api_key, self._version, self._ssl_verify, self._logger)
 
     @handle_invalid_deposit_site
-    def create_deposition(self, email: str, users: List[str], country: Country,
-                          experiments: List[Experiment], password: str = "") -> Deposit:
+    def create_deposition(self, email: str, users: List[str], country: Country, # pylint: disable=unused-argument
+                          experiments: List[Experiment], password: str = "", **kwargs) -> Deposit:
         """
         General method to create a deposition passing an Experiment object
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param experiments: List of Experiment objects
         :param password: Password
```

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev6/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/models.py` & `onedep_deposition-0.1.dev6/onedep_deposition/models.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev6/onedep_deposition/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev6/onedep_deposition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-deposition
-Version: 0.1.dev5
+Version: 0.1.dev6
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev5/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev6/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev5/pyproject.toml` & `onedep_deposition-0.1.dev6/pyproject.toml`

 * *Files identical despite different names*

