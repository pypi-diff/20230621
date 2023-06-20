# Comparing `tmp/matica_tools-0.0.1.tar.gz` & `tmp/matica_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matica_tools-0.0.1.tar", last modified: Mon Jun 19 23:38:22 2023, max compression
+gzip compressed data, was "matica_tools-0.0.2.tar", last modified: Tue Jun 20 22:27:47 2023, max compression
```

## Comparing `matica_tools-0.0.1.tar` & `matica_tools-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-19 23:38:22.864568 matica_tools-0.0.1/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.1/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.1/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-19 23:38:22.864380 matica_tools-0.0.1/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-19 22:23:00.000000 matica_tools-0.0.1/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-19 23:38:22.861894 matica_tools-0.0.1/matica_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-19 23:36:28.000000 matica_tools-0.0.1/matica_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1950 2023-06-19 23:36:28.000000 matica_tools-0.0.1/matica_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     4793 2023-06-19 23:36:28.000000 matica_tools-0.0.1/matica_tools/api.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.1/matica_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-19 23:38:22.864096 matica_tools-0.0.1/matica_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.1/matica_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-19 23:38:22.000000 matica_tools-0.0.1/matica_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-19 23:36:20.000000 matica_tools-0.0.1/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-19 23:38:22.864632 matica_tools-0.0.1/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.1/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.215194 matica_tools-0.0.2/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.2/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.2/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:27:47.215025 matica_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.2/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.213369 matica_tools-0.0.2/matica_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1950 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     4771 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/api.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.2/matica_tools/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.214682 matica_tools-0.0.2/matica_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.2/matica_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-20 22:27:28.000000 matica_tools-0.0.2/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-20 22:27:47.215253 matica_tools-0.0.2/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.2/setup.py
```

### Comparing `matica_tools-0.0.1/LICENSE` & `matica_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.1/PKG-INFO` & `matica_tools-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.1/matica_tools/_modidx.py` & `matica_tools-0.0.2/matica_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.1/matica_tools/api.py` & `matica_tools-0.0.2/matica_tools/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 # %% ../nbs/api.ipynb 3
 import paramiko
 import scp as scp2
 import base64
 import requests
 import time
-from requests.auth import HTTPBasicAuth
 
 # %% ../nbs/api.ipynb 4
 class MaticaAPIClient(object):
     @staticmethod
     def main(hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, uploaded_file_path, transfer_type, transfer_accession, storage_username, storage_password, file_dir_path='/home/files'):
         client = MaticaAPIClient(hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, storage_username, storage_password, file_dir_path=file_dir_path)
         client.upload(uploaded_file_path)
@@ -22,17 +21,17 @@
         transfer_UUID = client.approve_transfer(transfer_type, directory)
 
         sip_UUID = client.check_transfer_status(transfer_UUID)
 
         # ingest
         ingest_UUID = client.ingest(sip_UUID)
 
-        base64 = client.get_aip_url(ingest_UUID)
+        url = client.get_aip_url(ingest_UUID)
 
-        return base64
+        return url
 
 
     def __init__(self, hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, storage_username, storage_password, file_dir_path='/home/files'):
         self.hostname = hostname
         self.username = username
         self.api_key = api_key
         self.location_uuid = location_uuid
@@ -134,16 +133,17 @@
 
         return response4.json()["uuid"]
     
     def get_aip_url(self, ingest_UUID):
         endpoint2 = f"http://{self.hostname}:8001/api"
         url2 = f"{endpoint2}/v2/file/{ingest_UUID}/download/"
 
-        response6 = requests.get(url2, auth=HTTPBasicAuth(self.storage_username, self.storage_password))
+        # response6 = requests.get(url2, auth=HTTPBasicAuth(self.storage_username, self.storage_password))
 
         '''
         output_path = "/Users/nakamura/git/kim/matica_tools/demo/test.7z"
         with open(output_path ,mode='wb') as f: # wb でバイト型を書き込める
             f.write(response6.content)
         '''
 
-        return response6.content
+        # return response6.content
+        return url2
```

### Comparing `matica_tools-0.0.1/matica_tools.egg-info/PKG-INFO` & `matica_tools-0.0.2/matica_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.1/settings.ini` & `matica_tools-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = matica_tools
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = matica_tools
```

### Comparing `matica_tools-0.0.1/setup.py` & `matica_tools-0.0.2/setup.py`

 * *Files identical despite different names*

