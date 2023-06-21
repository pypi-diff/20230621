# Comparing `tmp/intercom_python_2-0.1.0.tar.gz` & `tmp/intercom_python_2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intercom_python_2-0.1.0.tar", max compression
+gzip compressed data, was "intercom_python_2-0.1.1.tar", max compression
```

## Comparing `intercom_python_2-0.1.0.tar` & `intercom_python_2-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-06-13 14:07:54.443433 intercom_python_2-0.1.0/LICENSE
--rw-r--r--   0        0        0     2553 2023-06-13 14:07:54.443539 intercom_python_2-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 14:07:54.443623 intercom_python_2-0.1.0/intercom/__init__.py
--rw-r--r--   0        0        0     5001 2023-06-13 14:07:54.443867 intercom_python_2-0.1.0/intercom/client.py
--rw-r--r--   0        0        0      191 2023-06-13 14:07:54.443992 intercom_python_2-0.1.0/intercom/exceptions.py
--rw-r--r--   0        0        0      398 2023-06-13 14:10:14.316300 intercom_python_2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 intercom_python_2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-13 14:07:54.443433 intercom_python_2-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2555 2023-06-21 18:51:51.841362 intercom_python_2-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 14:07:54.443623 intercom_python_2-0.1.1/intercom/__init__.py
+-rw-r--r--   0        0        0     5096 2023-06-21 18:51:51.841567 intercom_python_2-0.1.1/intercom/client.py
+-rw-r--r--   0        0        0      191 2023-06-13 14:07:54.443992 intercom_python_2-0.1.1/intercom/exceptions.py
+-rw-r--r--   0        0        0      398 2023-06-21 18:51:51.841741 intercom_python_2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 intercom_python_2-0.1.1/PKG-INFO
```

### Comparing `intercom_python_2-0.1.0/LICENSE` & `intercom_python_2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intercom_python_2-0.1.0/README.md` & `intercom_python_2-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # intercom-python
-![](https://img.shields.io/badge/version-0.1.0-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.1-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *intercom-python* is an API wrapper for intercom, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
-pip install intercom-python
+pip install intercom-python-2
 ```
 ## Usage
 ```python
 # if you have an access token:
 from intercom.client import Client
 client = Client(access_token=access_token)
 ```
```

### Comparing `intercom_python_2-0.1.0/intercom/client.py` & `intercom_python_2-0.1.1/intercom/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 
     def __init__(self, client_id=None, client_secret=None, access_token=None):
         self.CLIENT_ID = client_id
         self.CLIENT_SECRET = client_secret
         if access_token is not None:
             self.headers.update(Authorization=f"Bearer {access_token}")
 
-    def authorization_url(self, state=None):
+    def authorization_url(self, redirect_uri=None, state=None):
         params = {"response_type": "code", "client_id": self.CLIENT_ID}
         if state:
             params["state"] = state
+        if redirect_uri:
+            params["redirect_uri"] = redirect_uri
+
         return self.AUTH_URL + urlencode(params)
 
     def get_access_token(self, code):
         body = {"client_id": self.CLIENT_ID, "client_secret": self.CLIENT_SECRET, "code": code}
         return self.post("auth/eagle/token", data=json.dumps(body))
 
     def set_token(self, access_token):
```

### Comparing `intercom_python_2-0.1.0/PKG-INFO` & `intercom_python_2-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercom-python-2
-Version: 0.1.0
+Version: 0.1.1
 Summary: API wrapper for intercom written in Python
 License: MIT
 Author: Juan Carlos Rios
 Author-email: juankrios15@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # intercom-python
-![](https://img.shields.io/badge/version-0.1.0-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
+![](https://img.shields.io/badge/version-0.1.1-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *intercom-python* is an API wrapper for intercom, written in Python.  
 This library uses Oauth2 for authentication.
 ## Installing
 ```
-pip install intercom-python
+pip install intercom-python-2
 ```
 ## Usage
 ```python
 # if you have an access token:
 from intercom.client import Client
 client = Client(access_token=access_token)
 ```
```

