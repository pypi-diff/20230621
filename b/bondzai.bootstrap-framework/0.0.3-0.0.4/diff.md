# Comparing `tmp/bondzai.bootstrap-framework-0.0.3.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.3.tar", last modified: Wed Jun 21 10:24:45 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.4.tar", last modified: Wed Jun 21 15:39:53 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.3.tar` & `bondzai.bootstrap-framework-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:52:03.430072 bondzai.bootstrap-framework-0.0.3/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-21 10:50:13.000000 bondzai.bootstrap-framework-0.0.3/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 10:52:03.430072 bondzai.bootstrap-framework-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      141 2023-06-21 10:50:13.000000 bondzai.bootstrap-framework-0.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:52:02.956200 bondzai.bootstrap-framework-0.0.3/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:52:03.228074 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/
--rwxrwxrwx   0 root         (0) root         (0)      212 2023-06-21 10:51:53.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2696 2023-06-21 10:50:13.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/bootstrap.py
--rwxrwxrwx   0 root         (0) root         (0)     9176 2023-06-21 10:50:13.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_agent.py
--rwxrwxrwx   0 root         (0) root         (0)    14052 2023-06-21 10:50:13.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_com.py
--rwxrwxrwx   0 root         (0) root         (0)     5973 2023-06-21 10:50:14.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_config.py
--rwxrwxrwx   0 root         (0) root         (0)     2228 2023-06-21 10:50:14.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/file_handler.py
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-06-21 10:50:14.000000 bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/logger.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:52:03.406861 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:52:02.000000 bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-21 10:50:14.000000 bondzai.bootstrap-framework-0.0.3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-21 10:52:03.434587 bondzai.bootstrap-framework-0.0.3/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.627519 bondzai.bootstrap-framework-0.0.4/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-06-21 15:39:53.627664 bondzai.bootstrap-framework-0.0.4/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      141 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.621286 bondzai.bootstrap-framework-0.0.4/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.624837 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/
+-rw-r--r--   0 theo       (501) staff       (20)      212 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2696 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/bootstrap.py
+-rw-r--r--   0 theo       (501) staff       (20)     9159 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_agent.py
+-rw-r--r--   0 theo       (501) staff       (20)    14052 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_com.py
+-rw-r--r--   0 theo       (501) staff       (20)     5973 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_config.py
+-rw-r--r--   0 theo       (501) staff       (20)     2917 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/file_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/logger.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 15:39:53.627220 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       52 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 15:39:53.000000 bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-06-21 15:39:31.000000 bondzai.bootstrap-framework-0.0.4/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      755 2023-06-21 15:39:53.628514 bondzai.bootstrap-framework-0.0.4/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.3/NOTICE` & `bondzai.bootstrap-framework-0.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.3/PKG-INFO` & `bondzai.bootstrap-framework-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,19 +128,19 @@
             self.config.register_external_ops(op,custom_ops[op])
 
     def load_initial_data(self):
         """
         Load all data from a given dataset
         Args:
         """
+        dataset_definition = None
 
         my_tar = self.config.preload_targz()
-        dataset_definition = self.config.load_initial_dataset_definition_targz(my_tar)
-
-        # dataset_definition = self.config.load_initial_dataset_definition()
+        if my_tar.tar:
+            dataset_definition = self.config.load_initial_dataset_definition_targz(my_tar)
 
         ack = 0
         if dataset_definition:
             outputs_definition = dataset_definition["outputs"]
             dataset = dataset_definition["dataset"]
 
             for my_data in dataset:
```

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/dvs_config.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.4/bondzai/bootstrap_framework/file_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,32 @@
 
 
 class Tar:
     """
     Class to handle tar.gz files
     """
     def __init__(self, path: Path):
-        self.tar = tarfile.open(path, "r:gz")
-        self.name_list = self.tar.getnames()
+
+        self.tar = None
+        if path.is_file():
+            self.tar = tarfile.open(path, "r:gz")
+            self.name_list = self.tar.getnames()
 
     def get_file(self, file_name: str) -> BufferedReader:
         """
         From file name, get file data
         Args:
             file_name: name of the file
         Returns:
             file: file as reader, should be opened with any dedicated reader
 
         """
+        if self.tar is None:
+            raise Exception(f"impossible to load {file_name}, tar file not found")
+
         file = None
         if file_name in self.name_list:
             member = self.tar.getmember(file_name)
             file = self.tar.extractfile(member)
         return file
 
     def extract_file(self, file_name: str, folder: Path) -> Path:
@@ -38,14 +44,17 @@
         Args:
             file_name: name of the file
             folder: folder where to extract the file
         Returns:
             file_path: file path of the extract file
 
         """
+        if self.tar is None:
+            raise Exception(f"impossible to extract {file_name}, tar file not found")
+
         if not folder.exists():
             folder.mkdir(parents=True)
         file_path = None
         if file_name in self.name_list:
             member = self.tar.getmember(file_name)
             self.tar.extract(member, folder)
             file_path = folder / file_name
@@ -53,26 +62,36 @@
 
     def extract(self, folder: Path):
         """
         Extract all files at once in given folder
         Args:
             folder: folder where to extract the files
         """
+        if self.tar is None:
+            raise Exception(f"impossible to extract folder {folder}, tar file not found")
+
         if not folder.exists():
             folder.mkdir(parents=True)
         self.tar.extractall(folder)
 
     def __del__(self):
-        self.tar.close()
+        if self.tar:
+            self.tar.close()
 
     def read_yml(self,filepath):
+        if self.tar is None:
+            raise Exception(f"impossible to read yml {filepath}, tar file not found")
+ 
         f = self.get_file(filepath)
         data = yaml.safe_load(f)
 
         return data
     
     def read_binary(self,filepath): # "./output/id10883_train9.bin"
+        if self.tar is None:
+            raise Exception(f"impossible to read binary {filepath}, tar file not found")
+
         f = self.get_file(filepath)
         if f is None:
             raise Exception(f" file {filepath} not found")
         d = f.read()
         return handle_binary_file_data(d)
```

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.3/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.4/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.3/setup.cfg` & `bondzai.bootstrap-framework-0.0.4/setup.cfg`

 * *Files identical despite different names*

