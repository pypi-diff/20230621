# Comparing `tmp/proton-api-client-0.0.4.tar.gz` & `tmp/proton-api-client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.4.tar", last modified: Tue Jun 20 20:28:57 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.5.tar", last modified: Tue Jun 20 23:41:09 2023, max compression
```

## Comparing `proton-api-client-0.0.4.tar` & `proton-api-client-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.4/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1173 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      784 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.4/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.4/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.4/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4921 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.4/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2017 2023-06-20 20:20:29.000000 proton-api-client-0.0.4/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.4/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1173 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1669 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.5/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-20 23:38:08.000000 proton-api-client-0.0.5/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.678403 proton-api-client-0.0.5/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.5/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.5/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.5/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     5861 2023-06-20 23:39:35.000000 proton-api-client-0.0.5/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.5/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2017 2023-06-20 20:20:29.000000 proton-api-client-0.0.5/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     1541 2023-06-20 23:40:32.000000 proton-api-client-0.0.5/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 23:41:09.000000 proton-api-client-0.0.5/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 23:41:09.681736 proton-api-client-0.0.5/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-20 23:38:08.000000 proton-api-client-0.0.5/setup.py
```

### Comparing `proton-api-client-0.0.4/LICENSE` & `proton-api-client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.4/PKG-INFO` & `proton-api-client-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -19,18 +19,17 @@
 ```python
 from proton.client import ProtonMail
 
 username, password = ..., ...
 proton = ProtonMail(username, password)
 
 passphrase = 'myPass'
-pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+pk = 'privatekey.test123@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
 proton.gpg_import(pk, passphrase=passphrase)
 
-
 sessions = proton.sessions()
 
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
@@ -48,10 +47,18 @@
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
 
+directory = proton.calendar_directory()
+
+version = proton.version()
+
+plans = proton.plans()
+
+calendar_directory = proton.calendar_directory()
+
 proton.revoke_all_sessions()
 
 ```
```

### Comparing `proton-api-client-0.0.4/README.md` & `proton-api-client-0.0.5/proton_api_client.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+Metadata-Version: 2.1
+Name: proton-api-client
+Version: 0.0.5
+Summary: Proton Mail API
+Home-page: https://github.com/trevorhobenshield/proton-api-client
+Author: Trevor Hobenshield
+Author-email: trevorhobenshield@gmail.com
+Keywords: proton api client async search automation bot scrape mail email
+Requires-Python: >=3.10.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
 ### Proton Mail API
 
 #### Examples
 
 ```python
 from proton.client import ProtonMail
 
 username, password = ..., ...
 proton = ProtonMail(username, password)
 
 passphrase = 'myPass'
-pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+pk = 'privatekey.test123@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
 proton.gpg_import(pk, passphrase=passphrase)
 
-
 sessions = proton.sessions()
 
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
@@ -34,9 +47,18 @@
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
 
+directory = proton.calendar_directory()
+
+version = proton.version()
+
+plans = proton.plans()
+
+calendar_directory = proton.calendar_directory()
+
 proton.revoke_all_sessions()
-```
+
+```
```

### Comparing `proton-api-client-0.0.4/proton/_ctsrp.py` & `proton-api-client-0.0.5/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.4/proton/_pysrp.py` & `proton-api-client-0.0.5/proton/_pysrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.4/proton/constants.py` & `proton-api-client-0.0.5/proton/constants.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.4/proton/helpers.py` & `proton-api-client-0.0.5/proton/helpers.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.4/proton/login.py` & `proton-api-client-0.0.5/proton/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         'ClientEphemeral': b64encode(client_challenge).decode('utf8'),
         'ClientProof': b64encode(client_proof).decode('utf8'),
         'SRPSession': info['SRPSession'],
     }).json()
     user.verify_session(b64decode(auth['ServerProof']))
 
     # todo
-    print('login success') if user.authenticated() else print('login failure')
+    print('login success') if user.authenticated() else print('*** login failure')
 
     if auth['UID']:
         client.headers.update({
             'authorization': f'Bearer {auth["AccessToken"]}',
             'x-pm-uid': auth['UID'],
         })
     client.proton_session = {
```

### Comparing `proton-api-client-0.0.4/setup.py` & `proton-api-client-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,21 @@
     'bcrypt',
     'python-gnupg',
     'pyopenssl',
     'selectolax',
     'orjson',
     'httpx',
     'tqdm',
+    'uvloop',
+    'nest_asyncio',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.4',
+    version='0.0.5',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
@@ -26,18 +28,17 @@
     ```python
     from proton.client import ProtonMail
     
     username, password = ..., ...
     proton = ProtonMail(username, password)
     
     passphrase = 'myPass'
-    pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+    pk = 'privatekey.test123@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
     proton.gpg_import(pk, passphrase=passphrase)
     
-    
     sessions = proton.sessions()
 
     salts = proton.salts()
 
     users = proton.users()
 
     inbox = proton.inbox()
@@ -55,14 +56,22 @@
 
     timezones = proton.timezones()
 
     addresses = proton.addresses()
 
     info = proton.info()
 
+    directory = proton.calendar_directory()
+
+    version = proton.version()
+
+    plans = proton.plans()
+
+    calendar_directory = proton.calendar_directory()
+
     proton.revoke_all_sessions()
     
     ```
     '''),
     long_description_content_type='text/markdown',
     author='Trevor Hobenshield',
     author_email='trevorhobenshield@gmail.com',
```

