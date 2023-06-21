# Comparing `tmp/complycube-1.1.4.tar.gz` & `tmp/complycube-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complycube-1.1.4.tar", last modified: Thu Nov 11 02:01:44 2021, max compression
+gzip compressed data, was "complycube-1.1.5.tar", last modified: Wed Jun 21 01:17:05 2023, max compression
```

## Comparing `complycube-1.1.4.tar` & `complycube-1.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.936675 complycube-1.1.4/
--rw-r--r--   0 harry      (501) staff       (20)     1066 2021-11-11 01:06:11.000000 complycube-1.1.4/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)     3355 2021-11-11 02:01:44.936812 complycube-1.1.4/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)     2348 2021-10-31 15:14:54.000000 complycube-1.1.4/README.md
--rw-r--r--   0 harry      (501) staff       (20)      103 2021-11-11 01:06:11.000000 complycube-1.1.4/pyproject.toml
--rw-r--r--   0 harry      (501) staff       (20)     1072 2021-11-11 02:01:44.937450 complycube-1.1.4/setup.cfg
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.918056 complycube-1.1.4/src/
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.922675 complycube-1.1.4/src/complycube/
--rw-r--r--   0 harry      (501) staff       (20)      117 2021-11-11 01:10:54.000000 complycube-1.1.4/src/complycube/__init__.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.927513 complycube-1.1.4/src/complycube/api_resource_actions/
--rw-r--r--   0 harry      (501) staff       (20)      229 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/__init__.py
--rw-r--r--   0 harry      (501) staff       (20)      269 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/createresource.py
--rw-r--r--   0 harry      (501) staff       (20)      256 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/deleteresource.py
--rw-r--r--   0 harry      (501) staff       (20)      269 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/getresource.py
--rw-r--r--   0 harry      (501) staff       (20)      879 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/listresource.py
--rw-r--r--   0 harry      (501) staff       (20)      274 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resource_actions/updateresource.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.931964 complycube-1.1.4/src/complycube/api_resources/
--rw-r--r--   0 harry      (501) staff       (20)        0 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/__init__.py
--rw-r--r--   0 harry      (501) staff       (20)      649 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/accountinfo.py
--rw-r--r--   0 harry      (501) staff       (20)     1916 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/address.py
--rw-r--r--   0 harry      (501) staff       (20)      780 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/auditlog.py
--rw-r--r--   0 harry      (501) staff       (20)     1888 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/check.py
--rw-r--r--   0 harry      (501) staff       (20)     1878 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/client.py
--rw-r--r--   0 harry      (501) staff       (20)      176 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/complycuberesource.py
--rw-r--r--   0 harry      (501) staff       (20)     3311 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/document.py
--rw-r--r--   0 harry      (501) staff       (20)      385 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/flow.py
--rw-r--r--   0 harry      (501) staff       (20)     2454 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/livephoto.py
--rw-r--r--   0 harry      (501) staff       (20)      751 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/livevideo.py
--rw-r--r--   0 harry      (501) staff       (20)     1197 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/report.py
--rw-r--r--   0 harry      (501) staff       (20)      749 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/riskprofile.py
--rw-r--r--   0 harry      (501) staff       (20)      328 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/api_resources/static.py
--rw-r--r--   0 harry      (501) staff       (20)      819 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/teammember.py
--rw-r--r--   0 harry      (501) staff       (20)     1242 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/token.py
--rw-r--r--   0 harry      (501) staff       (20)     1296 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/api_resources/webhook.py
--rw-r--r--   0 harry      (501) staff       (20)     8407 2021-11-11 02:01:39.000000 complycube-1.1.4/src/complycube/complycube.py
--rw-r--r--   0 harry      (501) staff       (20)      155 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/error.py
--rw-r--r--   0 harry      (501) staff       (20)     1220 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/eventverifier.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.936457 complycube-1.1.4/src/complycube/model/
--rw-r--r--   0 harry      (501) staff       (20)      101 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/__init__.py
--rw-r--r--   0 harry      (501) staff       (20)      591 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/model/accountinfo.py
--rw-r--r--   0 harry      (501) staff       (20)     1923 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/address.py
--rw-r--r--   0 harry      (501) staff       (20)     1349 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/auditlog.py
--rw-r--r--   0 harry      (501) staff       (20)     2324 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/check.py
--rw-r--r--   0 harry      (501) staff       (20)     4556 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/model/client.py
--rw-r--r--   0 harry      (501) staff       (20)      334 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/complycubecollection.py
--rw-r--r--   0 harry      (501) staff       (20)     1388 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/complycubeobject.py
--rw-r--r--   0 harry      (501) staff       (20)     2897 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/document.py
--rw-r--r--   0 harry      (501) staff       (20)      412 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/model/flow.py
--rw-r--r--   0 harry      (501) staff       (20)     1752 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/livephoto.py
--rw-r--r--   0 harry      (501) staff       (20)     1229 2021-11-11 01:06:11.000000 complycube-1.1.4/src/complycube/model/livevideo.py
--rw-r--r--   0 harry      (501) staff       (20)      411 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/report.py
--rw-r--r--   0 harry      (501) staff       (20)     1696 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/riskprofile.py
--rw-r--r--   0 harry      (501) staff       (20)      606 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/teammember.py
--rw-r--r--   0 harry      (501) staff       (20)      380 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/token.py
--rw-r--r--   0 harry      (501) staff       (20)     2262 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/model/webhook.py
--rw-r--r--   0 harry      (501) staff       (20)      375 2021-11-11 00:43:57.000000 complycube-1.1.4/src/complycube/util.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2021-11-11 02:01:44.924997 complycube-1.1.4/src/complycube.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)     3355 2021-11-11 02:01:44.000000 complycube-1.1.4/src/complycube.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)     1953 2021-11-11 02:01:44.000000 complycube-1.1.4/src/complycube.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2021-11-11 02:01:44.000000 complycube-1.1.4/src/complycube.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)       32 2021-11-11 02:01:44.000000 complycube-1.1.4/src/complycube.egg-info/requires.txt
--rw-r--r--   0 harry      (501) staff       (20)       11 2021-11-11 02:01:44.000000 complycube-1.1.4/src/complycube.egg-info/top_level.txt
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.262117 complycube-1.1.5/
+-rw-r--r--   0 harry      (501) staff       (20)     1066 2022-12-15 16:00:29.000000 complycube-1.1.5/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)     3317 2023-06-21 01:17:05.262257 complycube-1.1.5/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     2348 2021-10-31 15:14:54.000000 complycube-1.1.5/README.md
+-rw-r--r--   0 harry      (501) staff       (20)      103 2022-12-15 16:00:29.000000 complycube-1.1.5/pyproject.toml
+-rw-r--r--   0 harry      (501) staff       (20)     1087 2023-06-21 01:17:05.262962 complycube-1.1.5/setup.cfg
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.206737 complycube-1.1.5/src/
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.214456 complycube-1.1.5/src/complycube/
+-rw-r--r--   0 harry      (501) staff       (20)      117 2023-06-20 13:00:03.000000 complycube-1.1.5/src/complycube/__init__.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.221523 complycube-1.1.5/src/complycube/api_resource_actions/
+-rw-r--r--   0 harry      (501) staff       (20)      229 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)      269 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/createresource.py
+-rw-r--r--   0 harry      (501) staff       (20)      256 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/deleteresource.py
+-rw-r--r--   0 harry      (501) staff       (20)      269 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/getresource.py
+-rw-r--r--   0 harry      (501) staff       (20)      879 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/listresource.py
+-rw-r--r--   0 harry      (501) staff       (20)      274 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resource_actions/updateresource.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.249864 complycube-1.1.5/src/complycube/api_resources/
+-rw-r--r--   0 harry      (501) staff       (20)        0 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)      649 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/accountinfo.py
+-rw-r--r--   0 harry      (501) staff       (20)     1916 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/address.py
+-rw-r--r--   0 harry      (501) staff       (20)      780 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/auditlog.py
+-rw-r--r--   0 harry      (501) staff       (20)     1888 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/check.py
+-rw-r--r--   0 harry      (501) staff       (20)     1878 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/client.py
+-rw-r--r--   0 harry      (501) staff       (20)      176 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/complycuberesource.py
+-rw-r--r--   0 harry      (501) staff       (20)     3311 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/document.py
+-rw-r--r--   0 harry      (501) staff       (20)      385 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/flow.py
+-rw-r--r--   0 harry      (501) staff       (20)     2454 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/livephoto.py
+-rw-r--r--   0 harry      (501) staff       (20)      751 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/livevideo.py
+-rw-r--r--   0 harry      (501) staff       (20)     1197 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/report.py
+-rw-r--r--   0 harry      (501) staff       (20)      749 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/riskprofile.py
+-rw-r--r--   0 harry      (501) staff       (20)      328 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/static.py
+-rw-r--r--   0 harry      (501) staff       (20)      819 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/teammember.py
+-rw-r--r--   0 harry      (501) staff       (20)     1397 2023-06-21 01:12:34.000000 complycube-1.1.5/src/complycube/api_resources/token.py
+-rw-r--r--   0 harry      (501) staff       (20)     1296 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/api_resources/webhook.py
+-rw-r--r--   0 harry      (501) staff       (20)     8370 2023-06-20 22:59:26.000000 complycube-1.1.5/src/complycube/complycube.py
+-rw-r--r--   0 harry      (501) staff       (20)      155 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/error.py
+-rw-r--r--   0 harry      (501) staff       (20)     1220 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/eventverifier.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.261616 complycube-1.1.5/src/complycube/model/
+-rw-r--r--   0 harry      (501) staff       (20)      101 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)      591 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/accountinfo.py
+-rw-r--r--   0 harry      (501) staff       (20)     1923 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/address.py
+-rw-r--r--   0 harry      (501) staff       (20)     1349 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/auditlog.py
+-rw-r--r--   0 harry      (501) staff       (20)     2324 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/check.py
+-rw-r--r--   0 harry      (501) staff       (20)     4556 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/client.py
+-rw-r--r--   0 harry      (501) staff       (20)      334 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/complycubecollection.py
+-rw-r--r--   0 harry      (501) staff       (20)     1388 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/complycubeobject.py
+-rw-r--r--   0 harry      (501) staff       (20)     2897 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/document.py
+-rw-r--r--   0 harry      (501) staff       (20)      412 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/flow.py
+-rw-r--r--   0 harry      (501) staff       (20)     1752 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/livephoto.py
+-rw-r--r--   0 harry      (501) staff       (20)     1229 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/livevideo.py
+-rw-r--r--   0 harry      (501) staff       (20)      411 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/report.py
+-rw-r--r--   0 harry      (501) staff       (20)     1696 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/riskprofile.py
+-rw-r--r--   0 harry      (501) staff       (20)      606 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/teammember.py
+-rw-r--r--   0 harry      (501) staff       (20)      380 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/token.py
+-rw-r--r--   0 harry      (501) staff       (20)     2262 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/model/webhook.py
+-rw-r--r--   0 harry      (501) staff       (20)      375 2022-12-15 16:00:29.000000 complycube-1.1.5/src/complycube/util.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-06-21 01:17:05.217065 complycube-1.1.5/src/complycube.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)     3317 2023-06-21 01:17:05.000000 complycube-1.1.5/src/complycube.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     1953 2023-06-21 01:17:05.000000 complycube-1.1.5/src/complycube.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-06-21 01:17:05.000000 complycube-1.1.5/src/complycube.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)       46 2023-06-21 01:17:05.000000 complycube-1.1.5/src/complycube.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       11 2023-06-21 01:17:05.000000 complycube-1.1.5/src/complycube.egg-info/top_level.txt
```

### Comparing `complycube-1.1.4/LICENSE` & `complycube-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/PKG-INFO` & `complycube-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: complycube
-Version: 1.1.4
+Version: 1.1.5
 Summary: Official Python client for the ComplyCube API
-Home-page: UNKNOWN
 Author: Complycube
 Author-email: tech@complycube.com
 License: MIT
 Keywords: complycube,aml,kyc,client,api,wrapper,PEP,identity verification,identity checks,document verification
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
@@ -121,8 +119,7 @@
 proxies = {
   'https': 'http://10.10.1.10:1080',
 }
 ccapi.clients.create(**input_client_dict proxies=proxies)
 ```
 
 For additional information, news and our latest blogs visit us at https://www.complycube.com/
-
```

### Comparing `complycube-1.1.4/README.md` & `complycube-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/setup.cfg` & `complycube-1.1.5/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = complycube
-version = 1.1.4
+version = 1.1.5
 author = Complycube
 author_email = tech@complycube.com
 description = Official Python client for the ComplyCube API
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = complycube, aml, kyc, client, api, wrapper, PEP, identity verification, identity checks, document verification
 license = MIT
@@ -26,14 +26,15 @@
 	= src
 packages = find:
 python_requires = 
 	>=3.6
 install_requires = 
 	requests>=2.20.0
 	pyhumps>=1.2.0
+	urllib3>=1.26
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `complycube-1.1.4/src/complycube/api_resource_actions/listresource.py` & `complycube-1.1.5/src/complycube/api_resource_actions/listresource.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/accountinfo.py` & `complycube-1.1.5/src/complycube/api_resources/accountinfo.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/address.py` & `complycube-1.1.5/src/complycube/api_resources/address.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/auditlog.py` & `complycube-1.1.5/src/complycube/api_resources/auditlog.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/check.py` & `complycube-1.1.5/src/complycube/api_resources/check.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/client.py` & `complycube-1.1.5/src/complycube/api_resources/client.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/document.py` & `complycube-1.1.5/src/complycube/api_resources/document.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/livephoto.py` & `complycube-1.1.5/src/complycube/api_resources/livephoto.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/livevideo.py` & `complycube-1.1.5/src/complycube/api_resources/livevideo.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/report.py` & `complycube-1.1.5/src/complycube/api_resources/report.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/riskprofile.py` & `complycube-1.1.5/src/complycube/api_resources/riskprofile.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/teammember.py` & `complycube-1.1.5/src/complycube/api_resources/teammember.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/api_resources/token.py` & `complycube-1.1.5/src/complycube/api_resources/token.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from complycube.api_resource_actions import ListResourceMixin
 from complycube.api_resources.complycuberesource import ComplyCubeResource
 
 class Token(ComplyCubeResource, CreateResourceMixin):
 
     @property
     def endpoint(self):
-        return 'webhooks' 
+        return 'tokens' 
 
-    def create(self,clientId,referrer,**kwargs):
+    def create(self,clientId,**kwargs):
         """[Generates an SDK token.]
 
-        Args:
-            clientId ([str]): [The ID of the client.]
-            referrer ([string]): [The referrer attributes specifies the URI of the web page where the Web SDK will be used. 
-                The referrer sent by the browser must match the referrer URI pattern in the JWT for the SDK to successfully authenticate. ]
+        Arguments:
+            clientId {str} -- [The ID of the client.]
+            referrer {str} -- [The referrer attributes specifies the URI of the web page where the Web SDK will be used. The referrer sent by the browser must match the referrer URI pattern in the JWT for the SDK to successfully authenticate. ]
+            appId {str} -- [The appId attributes specifies the bundle identifier of the app using the SDK. The bundle ID must match the bundle in the JWT for the SDK to successfully authenticate. ]
 
         Returns:
             [Token]: [Returns a token object with the generated token set.]
         """
-        return super(Token, self).create(clientId=clientId,referrer=referrer,**kwargs)
+        return super(Token, self).create(clientId=clientId, **kwargs)
 
     def resource_object(self,**response):
         return token.Token(**response)
```

### Comparing `complycube-1.1.4/src/complycube/api_resources/webhook.py` & `complycube-1.1.5/src/complycube/api_resources/webhook.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/complycube.py` & `complycube-1.1.5/src/complycube/complycube.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,22 +203,20 @@
         self.client_session.headers['Authorization'] = kwargs.pop('api_key',self.api_key)
         self.client_session.headers['User-Agent'] = '%s-python/%s' % (__package__,complycube.__version__)
         
         if method in ['post','put','patch']:
             request_args['headers'] = {'Content-Type': 'application/json'}
             request_args['data'] = json.dumps(kwargs)        
 
+        request_function = getattr(self.client_session, method)
         try:
-            request_function = getattr(self.client_session, method)
             response = request_function(url, params=params, **request_args)
-            content = response.content.decode('utf-8')
-
         except requests.RequestException as e:
-            print(content)
-            content = dict(error=str(e))
+            raise ComplyCubeAPIError(e)
+        content = response.content.decode('utf-8')
 
         if response.status_code != 204:
             content = json.loads(content)
         
         if response.status_code >= 400:
             raise ComplyCubeAPIError(content['message'])
         return content , response.status_code
```

### Comparing `complycube-1.1.4/src/complycube/eventverifier.py` & `complycube-1.1.5/src/complycube/eventverifier.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/accountinfo.py` & `complycube-1.1.5/src/complycube/model/accountinfo.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/address.py` & `complycube-1.1.5/src/complycube/model/address.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/auditlog.py` & `complycube-1.1.5/src/complycube/model/auditlog.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/check.py` & `complycube-1.1.5/src/complycube/model/check.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/client.py` & `complycube-1.1.5/src/complycube/model/client.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/complycubeobject.py` & `complycube-1.1.5/src/complycube/model/complycubeobject.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/document.py` & `complycube-1.1.5/src/complycube/model/document.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/livephoto.py` & `complycube-1.1.5/src/complycube/model/livephoto.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/livevideo.py` & `complycube-1.1.5/src/complycube/model/livevideo.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/riskprofile.py` & `complycube-1.1.5/src/complycube/model/riskprofile.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/teammember.py` & `complycube-1.1.5/src/complycube/model/teammember.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube/model/webhook.py` & `complycube-1.1.5/src/complycube/model/webhook.py`

 * *Files identical despite different names*

### Comparing `complycube-1.1.4/src/complycube.egg-info/PKG-INFO` & `complycube-1.1.5/src/complycube.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: complycube
-Version: 1.1.4
+Version: 1.1.5
 Summary: Official Python client for the ComplyCube API
-Home-page: UNKNOWN
 Author: Complycube
 Author-email: tech@complycube.com
 License: MIT
 Keywords: complycube,aml,kyc,client,api,wrapper,PEP,identity verification,identity checks,document verification
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
@@ -121,8 +119,7 @@
 proxies = {
   'https': 'http://10.10.1.10:1080',
 }
 ccapi.clients.create(**input_client_dict proxies=proxies)
 ```
 
 For additional information, news and our latest blogs visit us at https://www.complycube.com/
-
```

### Comparing `complycube-1.1.4/src/complycube.egg-info/SOURCES.txt` & `complycube-1.1.5/src/complycube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

