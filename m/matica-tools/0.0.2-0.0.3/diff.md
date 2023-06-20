# Comparing `tmp/matica_tools-0.0.2.tar.gz` & `tmp/matica_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matica_tools-0.0.2.tar", last modified: Tue Jun 20 22:27:47 2023, max compression
+gzip compressed data, was "matica_tools-0.0.3.tar", last modified: Tue Jun 20 22:54:16 2023, max compression
```

## Comparing `matica_tools-0.0.2.tar` & `matica_tools-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.215194 matica_tools-0.0.2/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.2/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:27:47.215025 matica_tools-0.0.2/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.2/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.213369 matica_tools-0.0.2/matica_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1950 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     4771 2023-06-20 22:27:08.000000 matica_tools-0.0.2/matica_tools/api.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.2/matica_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:27:47.214682 matica_tools-0.0.2/matica_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.2/matica_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-20 22:27:47.000000 matica_tools-0.0.2/matica_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-20 22:27:28.000000 matica_tools-0.0.2/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-20 22:27:47.215253 matica_tools-0.0.2/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.2/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.353786 matica_tools-0.0.3/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.3/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:54:16.353621 matica_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.3/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.352225 matica_tools-0.0.3/matica_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1950 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     4903 2023-06-20 22:53:34.000000 matica_tools-0.0.3/matica_tools/api.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.3/matica_tools/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 22:54:16.353393 matica_tools-0.0.3/matica_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.3/matica_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-20 22:54:16.000000 matica_tools-0.0.3/matica_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-20 22:53:51.000000 matica_tools-0.0.3/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-20 22:54:16.353841 matica_tools-0.0.3/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.3/setup.py
```

### Comparing `matica_tools-0.0.2/LICENSE` & `matica_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.2/PKG-INFO` & `matica_tools-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.2/matica_tools/_modidx.py` & `matica_tools-0.0.3/matica_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.2/matica_tools/api.py` & `matica_tools-0.0.3/matica_tools/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import scp as scp2
 import base64
 import requests
 import time
 
 # %% ../nbs/api.ipynb 4
 class MaticaAPIClient(object):
+    time_span = 2
+
     @staticmethod
     def main(hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, uploaded_file_path, transfer_type, transfer_accession, storage_username, storage_password, file_dir_path='/home/files'):
         client = MaticaAPIClient(hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, storage_username, storage_password, file_dir_path=file_dir_path)
         client.upload(uploaded_file_path)
         directory = client.transfer(transfer_type, transfer_accession)
 
         transfer_UUID = client.approve_transfer(transfer_type, directory)
@@ -101,39 +103,43 @@
             }
 
             response3 = requests.post(f'{self.endpoint}/transfer/approve/', headers=self.headers, data=data)
 
             if "uuid" in response3.json():
                 break
 
-            time.sleep(5)
+            time.sleep(self.time_span)
 
         return response3.json()["uuid"]
     
     def check_transfer_status(self, transfer_UUID):
         while 1:
 
             response5 = requests.get(f'{self.endpoint}/transfer/status/{transfer_UUID}', headers=self.headers)
 
-            if response5.json()["status"] != "PROCESSING":
+            r = response5.json()
+
+            if "status" in r and r["status"] != "PROCESSING":
                 break
 
-            time.sleep(5)
+            time.sleep(self.time_span)
 
         return response5.json()["sip_uuid"]
     
     def ingest(self, sip_UUID):
         while 1:
 
             response4 = requests.get(f'{self.endpoint}/ingest/status/{sip_UUID}', headers=self.headers)
 
-            if response4.json()["status"] != "PROCESSING":
+            r = response4.json()
+
+            if "status" in r and r["status"] != "PROCESSING":
                 break
 
-            time.sleep(5)
+            time.sleep(self.time_span)
 
         return response4.json()["uuid"]
     
     def get_aip_url(self, ingest_UUID):
         endpoint2 = f"http://{self.hostname}:8001/api"
         url2 = f"{endpoint2}/v2/file/{ingest_UUID}/download/"
```

### Comparing `matica_tools-0.0.2/matica_tools.egg-info/PKG-INFO` & `matica_tools-0.0.3/matica_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.2/settings.ini` & `matica_tools-0.0.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = matica_tools
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = matica_tools
```

### Comparing `matica_tools-0.0.2/setup.py` & `matica_tools-0.0.3/setup.py`

 * *Files identical despite different names*

