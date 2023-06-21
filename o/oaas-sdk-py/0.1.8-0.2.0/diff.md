# Comparing `tmp/oaas_sdk_py-0.1.8.tar.gz` & `tmp/oaas_sdk_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.8.tar", last modified: Mon May  1 10:14:35 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.2.0.tar", last modified: Wed Jun 21 07:04:13 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.8.tar` & `oaas_sdk_py-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.618412 oaas_sdk_py-0.1.8/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      258 2023-05-01 10:14:35.617875 oaas_sdk_py-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.8/README.md
--rw-rw-rw-   0        0        0      495 2023-05-01 10:12:29.000000 oaas_sdk_py-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 10:14:35.618412 oaas_sdk_py-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.603930 oaas_sdk_py-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.609766 oaas_sdk_py-0.1.8/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8945 2023-05-01 10:10:36.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-04-24 11:01:38.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.614613 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 07:04:13.286620 oaas_sdk_py-0.2.0/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-06-21 07:04:13.285616 oaas_sdk_py-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.2.0/README.md
+-rw-rw-rw-   0        0        0      495 2023-06-21 07:03:46.000000 oaas_sdk_py-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:04:13.286620 oaas_sdk_py-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 07:04:13.268837 oaas_sdk_py-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 07:04:13.279032 oaas_sdk_py-0.2.0/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8945 2023-05-01 10:10:36.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1798 2023-06-21 07:02:46.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:04:13.284069 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-21 07:04:13.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-06-21 07:04:13.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:04:13.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-21 07:04:13.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 07:04:13.000000 oaas_sdk_py-0.2.0/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.8/LICENSE` & `oaas_sdk_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.8/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.2.0/src/oaas_sdk_py/__init__.py`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.8/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.2.0/src/oaas_sdk_py/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,25 @@
         return self.json_dict['funcName']
 
 
 class OaasObject:
 
     def __init__(self, json_dict):
         self.json_dict = json_dict
-        self.origin = OaasObjectOrigin(self.json_dict["origin"])
         self.data = self.json_dict.get("data", {})
         self.updated_keys: [str] = []
 
     @property
     def id(self):
         return self.json_dict["id"]
 
+    @property
+    def cls(self):
+        return self.json_dict["cls"]
+
 
 class OaasTask:
     input: [OaasObject]
     output_obj: OaasObject = None
 
     def __init__(self, json_dict):
         self.json_dict = json_dict
```

