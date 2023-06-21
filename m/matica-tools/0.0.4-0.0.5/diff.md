# Comparing `tmp/matica_tools-0.0.4.tar.gz` & `tmp/matica_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matica_tools-0.0.4.tar", last modified: Wed Jun 21 00:21:56 2023, max compression
+gzip compressed data, was "matica_tools-0.0.5.tar", last modified: Wed Jun 21 01:03:26 2023, max compression
```

## Comparing `matica_tools-0.0.4.tar` & `matica_tools-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.114614 matica_tools-0.0.4/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.4/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.4/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 00:21:56.114436 matica_tools-0.0.4/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.4/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.112614 matica_tools-0.0.4/matica_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     2313 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     9300 2023-06-21 00:15:07.000000 matica_tools-0.0.4/matica_tools/api.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.4/matica_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 00:21:56.114148 matica_tools-0.0.4/matica_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.4/matica_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-21 00:21:56.000000 matica_tools-0.0.4/matica_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-21 00:21:35.000000 matica_tools-0.0.4/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 00:21:56.114671 matica_tools-0.0.4/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.4/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 01:03:26.792217 matica_tools-0.0.5/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 matica_tools-0.0.5/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 matica_tools-0.0.5/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 01:03:26.792055 matica_tools-0.0.5/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      309 2023-06-20 22:27:11.000000 matica_tools-0.0.5/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 01:03:26.790505 matica_tools-0.0.5/matica_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 01:02:19.000000 matica_tools-0.0.5/matica_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     2313 2023-06-21 01:02:19.000000 matica_tools-0.0.5/matica_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     9244 2023-06-21 01:02:19.000000 matica_tools-0.0.5/matica_tools/api.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-06-19 22:22:57.000000 matica_tools-0.0.5/matica_tools/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 01:03:26.791815 matica_tools-0.0.5/matica_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1076 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      394 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       67 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-19 22:58:12.000000 matica_tools-0.0.5/matica_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       13 2023-06-21 01:03:26.000000 matica_tools-0.0.5/matica_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-21 01:02:16.000000 matica_tools-0.0.5/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 01:03:26.792269 matica_tools-0.0.5/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 matica_tools-0.0.5/setup.py
```

### Comparing `matica_tools-0.0.4/LICENSE` & `matica_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.4/PKG-INFO` & `matica_tools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.4/matica_tools/_modidx.py` & `matica_tools-0.0.5/matica_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `matica_tools-0.0.4/matica_tools/api.py` & `matica_tools-0.0.5/matica_tools/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
             response5 = requests.get(f'{self.endpoint}/transfer/status/{transfer_UUID}', headers=self.headers)
 
             r = response5.json()
 
             if "status" in r and r["status"] != "PROCESSING":
                 # break
-                self.stage = 3
+                # self.stage = 3
 
                 self.sip_UUID = response5.json()["sip_uuid"]
 
                 # time.sleep(self.time_span)
 
                 # return response5.json()["sip_uuid"]
 
@@ -109,44 +109,43 @@
                 "status": "transfer processing"
             }
         # elif self.stage == 3:
         elif "sip_UUID" in params:
 
             sip_UUID = params["sip_UUID"] # self.sip_UUID
 
-            if "download" in params:
-                return {
-                    "status": "completed",
-                    "data": self.get_aip_url(sip_UUID)
-                }
+            
 
             response4 = requests.get(f'{self.endpoint}/ingest/status/{sip_UUID}', headers=self.headers)
 
             r = response4.json()
 
             if "status" in r and r["status"] != "PROCESSING":
                 # break
-                self.stage = 4
+                # self.stage = 4
                 return {
                     "data": {
                         "ingest_UUID": response4.json()["uuid"],
-                        "download": 1
+                        # "download": 1
                     },
                     "status": "ingest done",
                 }
 
             return {
                 "status": "ingest processing"
             }
         
         # 
-        else:
+        elif "ingest_UUID" in params:
+
+            ingest_UUID = params["ingest_UUID"] # self.ingest_UUID
+            
             return {
                 "status": "completed",
-                "data": self.get_aip_url(self.sip_UUID)
+                "data": self.get_aip_url(ingest_UUID)
             }
 
 
     def __init__ (self, hostname, username, api_key, location_uuid, ssh_username, ssh_password, task_id, uploaded_file_path, transfer_type, transfer_accession, storage_username, storage_password, file_dir_path='/home/files'):
         self.hostname = hostname
         self.username = username
         self.api_key = api_key
```

### Comparing `matica_tools-0.0.4/matica_tools.egg-info/PKG-INFO` & `matica_tools-0.0.5/matica_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matica-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/matica_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `matica_tools-0.0.4/settings.ini` & `matica_tools-0.0.5/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = matica_tools
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = matica_tools
```

### Comparing `matica_tools-0.0.4/setup.py` & `matica_tools-0.0.5/setup.py`

 * *Files identical despite different names*

