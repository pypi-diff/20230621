# Comparing `tmp/cameralyze-1.4.7.tar.gz` & `tmp/cameralyze-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameralyze-1.4.7.tar", last modified: Thu May 25 09:45:44 2023, max compression
+gzip compressed data, was "cameralyze-1.4.8.tar", last modified: Wed Jun 21 08:15:30 2023, max compression
```

## Comparing `cameralyze-1.4.7.tar` & `cameralyze-1.4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.015082 cameralyze-1.4.7/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-05-25 09:45:44.014899 cameralyze-1.4.7/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.7/README.md
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.013963 cameralyze-1.4.7/cameralyze/
--rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.7/cameralyze/__init__.py
--rw-r--r--   0 ufukdag    (501) staff       (20)     4057 2023-05-25 09:44:22.000000 cameralyze-1.4.7/cameralyze/model.py
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.014707 cameralyze-1.4.7/cameralyze.egg-info/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-05-25 09:45:44.000000 cameralyze-1.4.7/cameralyze.egg-info/SOURCES.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/dependency_links.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/requires.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/top_level.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-05-25 09:45:44.015150 cameralyze-1.4.7/setup.cfg
--rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-05-25 09:45:26.000000 cameralyze-1.4.7/setup.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-06-21 08:15:30.949512 cameralyze-1.4.8/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-06-21 08:15:30.949289 cameralyze-1.4.8/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.8/README.md
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-06-21 08:15:30.948084 cameralyze-1.4.8/cameralyze/
+-rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.8/cameralyze/__init__.py
+-rw-r--r--   0 ufukdag    (501) staff       (20)     3369 2023-06-21 08:14:25.000000 cameralyze-1.4.8/cameralyze/model.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-06-21 08:15:30.948997 cameralyze-1.4.8/cameralyze.egg-info/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-06-21 08:15:30.000000 cameralyze-1.4.8/cameralyze.egg-info/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-06-21 08:15:30.000000 cameralyze-1.4.8/cameralyze.egg-info/SOURCES.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-06-21 08:15:30.000000 cameralyze-1.4.8/cameralyze.egg-info/dependency_links.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-06-21 08:15:30.000000 cameralyze-1.4.8/cameralyze.egg-info/requires.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-06-21 08:15:30.000000 cameralyze-1.4.8/cameralyze.egg-info/top_level.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-06-21 08:15:30.949581 cameralyze-1.4.8/setup.cfg
+-rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-06-21 08:15:26.000000 cameralyze-1.4.8/setup.py
```

### Comparing `cameralyze-1.4.7/cameralyze/model.py` & `cameralyze-1.4.8/cameralyze/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import requests
-import filetype
+import json
 
 from typing import Union, Any
-from uuid import uuid4
-
 
 class Connect:
     def __init__(self, api_key: str = None):
         self.model = None
         self.endpoint = None
         self.background_job = None
         self.flow = None
         self.beautify = False
         self.get_response = True
-        self.base_domain = "https://run.plugger.ai"
+        self.base_domain = "https://inference.plugger.ai"
         self.test_temporary_image_domain = "https://tmp.cameralyze.co"
-        self.upload_url = "https://platform.api.cameralyze.com/temporary-file/generate"
+        self.upload_url = "https://platform.api.plugger.ai/tmp/upload"
         self.platform_url = "https://platform.cameralyze.co"
         self.api_key = api_key
         self.configuration = None
         
     def beautify_response(self):
         self.beautify = True
         
@@ -43,43 +41,37 @@
     def set_model(self, model: str):
         """
         Args:
             model (str): Model UUID or model alias name
         """
         self.model = model
         
-        return self
-                
-    def __get_presigned_upload_url(self, file_type: str, file_name: str) -> str:
-        return requests.post(self.upload_url, json={"fileType": file_type, "fileName": file_name}).json()["data"]        
+        return self   
 
     def read_file(self, path: str) -> str:
-        file_type = filetype.guess(path).mime
-        file_name = str(uuid4())
-        file = "{file_name}.{file_extension}".format(file_name=file_name, file_extension=path.split(".")[-1])
-
-        self.__upload_file(path=path, file_type=file_type, file_name=file)
+        file = path.split("/")[-1]
+        
+        with open(path, 'rb') as local_file:
+            local_file_body = local_file.read()
+            
+        response = requests.put(
+            "{url}/{file}".format(url=self.upload_url, file=file), 
+            data=local_file_body,
+            headers={'Content-Type': 'application/octet-stream'}
+        )
+        
+        print(response.status_code)
 
         return "{test_temporary_image_domain}/{file}".format(
             test_temporary_image_domain=self.test_temporary_image_domain, 
             file=file
         )
 
-    def __upload_file(self, path: str, file_type: str, file_name: str):
-        with open(path, 'rb') as local_file:
-            local_file_body = local_file.read()
-
-        requests.put(
-            self.__get_presigned_upload_url(file_type=file_type, file_name=file_name), 
-            data=local_file_body, 
-            headers={'Content-Type': file_type, 'x-amz-acl': 'public-read'}
-        )
-
     def __get_json(self, image: Union[str, tuple] = None, text:str = None, **kwargs: Any) -> dict:
-        json={"apiKey": self.api_key, "rawResponse": not self.beautify, "getResponse": self.get_response, "input": kwargs}
+        json={"rawResponse": not self.beautify, "getResponse": self.get_response, "input": kwargs}
 
         if image != None:
             if isinstance(image, tuple):
                 json["fileId"] = image[0]
                 json["fileType"] = image[1]
             elif image.startswith("http"):
                 json["url"] = image
@@ -92,31 +84,20 @@
         if self.model:
             json["itemUuid"] = self.model
         
         if self.configuration != None:
             json["configuration"] = self.configuration
 
         return json
-    
-    def __get_path(self) -> str:
-        if self.flow:
-            return "flow"
-        
-        return "model"
-    
-    def __get_unique_id(self) -> str:
-        if self.flow:
-            return self.flow
-        
-        return self.model
 
     def predict(self, image: Union[str, tuple] = None, text: str = None, **kwargs: Any) -> dict:
         api_call = requests.post(
             self.base_domain,
-            json=self.__get_json(image=image, text=text, **kwargs)
+            headers={"x-api-key": self.api_key, "Content-Type": "application/json"},
+            data=json.dumps(self.__get_json(image=image, text=text, **kwargs))
         )
 
         return api_call.json() 
 
     def show_configuration(self):
         print(
             "You can see configuration in here:\n{platform_url}/model-detail/{model}".format(
```

### Comparing `cameralyze-1.4.7/setup.py` & `cameralyze-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.7' 
+VERSION = '1.4.8' 
 DESCRIPTION = 'Cameralyze No-Code AI Platform'
 LONG_DESCRIPTION = 'Offical Cameralyze No-Code AI Platform package'
 
 setup(
         name="cameralyze", 
         version=VERSION,
         author="Cameralyze Inc",
```

