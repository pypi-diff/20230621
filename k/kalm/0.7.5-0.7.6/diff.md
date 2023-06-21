# Comparing `tmp/kalm-0.7.5.tar.gz` & `tmp/kalm-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.7.5.tar", max compression
+gzip compressed data, was "kalm-0.7.6.tar", max compression
```

## Comparing `kalm-0.7.5.tar` & `kalm-0.7.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.5/LICENSE.txt
--rw-r--r--   0        0        0     2181 2023-06-21 07:19:37.760128 kalm-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    10467 2023-06-21 07:19:26.396067 kalm-0.7.5/src/kalm/__init__.py
--rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.5/src/kalm/common.py
--rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.5/src/kalm/dns/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.5/src/kalm/dns/dns.py
--rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.5/src/kalm/gitea/__init__.py
--rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.5/src/kalm/gitea/gitea.py
--rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.5/src/kalm/inabox/__init__.py
--rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.5/src/kalm/inabox/inabox.py
--rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.5/src/kalm/jenkins/__init__.py
--rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.5/src/kalm/jenkins/jenkins.py
--rw-r--r--   0        0        0    35971 2023-06-21 07:16:21.779089 kalm-0.7.5/src/kalm/kalm.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.5/src/kalm/package_data.dat
--rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.5/src/kalm/pypi/__init__.py
--rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.5/src/kalm/pypi/pypi.py
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.5/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.6/LICENSE.txt
+-rw-r--r--   0        0        0     2181 2023-06-21 07:27:06.346600 kalm-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0    10467 2023-06-21 07:19:26.396067 kalm-0.7.6/src/kalm/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.6/src/kalm/common.py
+-rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/dns/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/dns/dns.py
+-rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/gitea/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.6/src/kalm/gitea/gitea.py
+-rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.6/src/kalm/inabox/__init__.py
+-rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.6/src/kalm/inabox/inabox.py
+-rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.6/src/kalm/jenkins/__init__.py
+-rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.6/src/kalm/jenkins/jenkins.py
+-rw-r--r--   0        0        0    36170 2023-06-21 07:26:55.642540 kalm-0.7.6/src/kalm/kalm.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.6/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.6/src/kalm/pypi/__init__.py
+-rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.6/src/kalm/pypi/pypi.py
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.6/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.6/PKG-INFO
```

### Comparing `kalm-0.7.5/LICENSE.txt` & `kalm-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/pyproject.toml` & `kalm-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.7.5"
+version = "0.7.6"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -28,15 +28,15 @@
 python-jenkins = "^1.7.0"
 urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.7.04" 
+version = "0.7.05" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.7.5/src/kalm/__init__.py` & `kalm-0.7.6/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/dns/__init__.py` & `kalm-0.7.6/src/kalm/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/dns/dns.py` & `kalm-0.7.6/src/kalm/dns/dns.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/gitea/__init__.py` & `kalm-0.7.6/src/kalm/gitea/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/inabox/__init__.py` & `kalm-0.7.6/src/kalm/inabox/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/inabox/inabox.py` & `kalm-0.7.6/src/kalm/inabox/inabox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/jenkins/__init__.py` & `kalm-0.7.6/src/kalm/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/jenkins/jenkins.py` & `kalm-0.7.6/src/kalm/jenkins/jenkins.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/kalm.py` & `kalm-0.7.6/src/kalm/kalm.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,14 +303,19 @@
   return fileval
 
 
 ############################################################################################################################
 # update ansible vault
 ############################################################################################################################
 def awx_update_vault(ansiblevault, organization, mytoken, r):
+  print("------------------------------------------------------------------")
+  print(ansiblevault)
+  print(organization)
+  print("------------------------------------------------------------------")
+
   for vault in ansiblevault[organization]['vault']:
     credential = { 
       "name": vault['name'], 
       "description": vault['description'], 
       "type": "Vault", 
       "vault_id": vault['vault_id'], 
       "vault_password": vault['vault_password'], 
@@ -717,15 +722,15 @@
   # Load and set ansible secrets in ansible vault
   ########################################################################################################################
   prettyllog("init", "runtime", "config", "init", "001", "loadning secrets")
   ansiblevaultfile = "/etc/kalm/secret.json"
   f = open(ansiblevaultfile)
   ansiblevault = json.loads(f.read())
   print(ansiblevault)
-  
+
   f.close
 
 
   ########################################################################################################################
   # Load  and set ansible automation org
   ########################################################################################################################
   cfgfile = "/etc/kalm/kalm.json"
```

### Comparing `kalm-0.7.5/src/kalm/pypi/__init__.py` & `kalm-0.7.6/src/kalm/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/src/kalm/pypi/pypi.py` & `kalm-0.7.6/src/kalm/pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.5/PKG-INFO` & `kalm-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.7.5
+Version: 0.7.6
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

