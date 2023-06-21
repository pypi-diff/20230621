# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.3.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.3.tar", last modified: Tue Jun 20 05:34:53 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.4.tar", last modified: Wed Jun 21 03:16:40 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.152474 hyutils-hyutil-hoyun-lab-0.0.6.3/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-06-20 05:34:53.151973 hyutils-hyutil-hoyun-lab-0.0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 05:34:53.152649 hyutils-hyutil-hoyun-lab-0.0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-06-20 05:32:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.127974 hyutils-hyutil-hoyun-lab-0.0.6.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.144474 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      347 2023-06-20 05:32:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    15304 2023-06-20 04:05:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.150474 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:16:40.908945 hyutils-hyutil-hoyun-lab-0.0.6.4/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-06-21 03:16:40.908445 hyutils-hyutil-hoyun-lab-0.0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:16:40.909584 hyutils-hyutil-hoyun-lab-0.0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-21 03:16:17.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:16:40.888445 hyutils-hyutil-hoyun-lab-0.0.6.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 03:16:40.902946 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      347 2023-06-21 03:16:17.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1290 2023-06-21 02:07:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    15304 2023-06-20 04:05:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:16:40.907446 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-06-21 03:16:40.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-21 03:16:40.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:16:40.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-21 03:16:40.000000 hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.3",
+    version="0.0.6.4",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/dirjob.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,17 +24,23 @@
                 yield file_path, root
 
 def dirs(path):
     for file in os.listdir(path):
         if os.path.isdir(os.path.join(path, file)):
             yield file
 
-def get_entry_count(path):
-	listing = os.listdir(path)
-	return len(listing)
+def get_entry_count(path, ext):
+    total_files = 0
+
+    for root, dirs, files in os.walk(path):
+        for file in files:
+            if file.endswith(ext):
+                total_files += 1
+
+    return total_files
     
 def listfiles(rootdir):
     for file in os.listdir(rootdir):
         d = os.path.join(rootdir, file)
         if os.path.isfile(d):
             yield(d)
         if os.path.isdir(d):
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.6.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

