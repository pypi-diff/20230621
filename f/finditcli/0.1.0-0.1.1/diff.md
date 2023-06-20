# Comparing `tmp/finditcli-0.1.0.tar.gz` & `tmp/finditcli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finditcli-0.1.0.tar", max compression
+gzip compressed data, was "finditcli-0.1.1.tar", max compression
```

## Comparing `finditcli-0.1.0.tar` & `finditcli-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       12 2023-06-20 09:46:17.433802 finditcli-0.1.0/README.md
--rw-r--r--   0        0        0      257 2023-06-20 20:58:19.603692 finditcli-0.1.0/file_finder/cli.py
--rw-r--r--   0        0        0      319 2023-06-20 20:47:27.383710 finditcli-0.1.0/file_finder/constants.py
--rw-r--r--   0        0        0      363 2023-06-20 19:22:11.453803 finditcli-0.1.0/file_finder/exceptions.py
--rw-r--r--   0        0        0     5973 2023-06-20 20:48:25.593711 finditcli-0.1.0/file_finder/finder.py
--rw-r--r--   0        0        0      150 2023-06-20 20:49:32.043677 finditcli-0.1.0/file_finder/teste.py
--rw-r--r--   0        0        0     3477 2023-06-20 20:47:32.663711 finditcli-0.1.0/file_finder/utils.py
--rw-r--r--   0        0        0      457 2023-06-20 22:17:16.733704 finditcli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 finditcli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2836 2023-06-20 22:57:59.883709 finditcli-0.1.1/README.md
+-rw-r--r--   0        0        0      257 2023-06-20 20:58:19.603692 finditcli-0.1.1/file_finder/cli.py
+-rw-r--r--   0        0        0      319 2023-06-20 20:47:27.383710 finditcli-0.1.1/file_finder/constants.py
+-rw-r--r--   0        0        0      363 2023-06-20 19:22:11.453803 finditcli-0.1.1/file_finder/exceptions.py
+-rw-r--r--   0        0        0     5973 2023-06-20 20:48:25.593711 finditcli-0.1.1/file_finder/finder.py
+-rw-r--r--   0        0        0      150 2023-06-20 20:49:32.043677 finditcli-0.1.1/file_finder/teste.py
+-rw-r--r--   0        0        0     3638 2023-06-20 22:55:42.513693 finditcli-0.1.1/file_finder/utils.py
+-rw-r--r--   0        0        0      457 2023-06-20 22:57:07.273707 finditcli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 finditcli-0.1.1/PKG-INFO
```

### Comparing `finditcli-0.1.0/file_finder/finder.py` & `finditcli-0.1.1/file_finder/finder.py`

 * *Files identical despite different names*

### Comparing `finditcli-0.1.0/file_finder/utils.py` & `finditcli-0.1.1/file_finder/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+import platform
 from file_finder.exceptions import InvalidInputError
 
 
 def get_folders(path):
     """Obtém os subdiretórios no diretório pesquisado.
 
     Args:
@@ -95,13 +96,19 @@
     """
     files_details = []
 
     for file in files:
         stat = file.stat()
         details = [
             file.name,
-            timestamp_to_string(stat.st_ctime),
+            timestamp_to_string(get_created_timestamp(stat)),
             timestamp_to_string(stat.st_mtime),
             file.absolute(),
         ]
         files_details.append(details)
     return files_details
+
+
+def get_created_timestamp(stat):
+    if platform.system() == "Darwin":
+        return stat.st_birthtime
+    return stat.st_ctime
```

