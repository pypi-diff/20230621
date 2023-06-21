# Comparing `tmp/fs.webdavfs-0.4.3.tar.gz` & `tmp/fs.webdavfs-0.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs.webdavfs-0.4.3.tar", last modified: Wed Jun 21 12:12:06 2023, max compression
+gzip compressed data, was "fs.webdavfs-0.4.3.1.tar", last modified: Wed Jun 21 12:56:09 2023, max compression
```

## Comparing `fs.webdavfs-0.4.3.tar` & `fs.webdavfs-0.4.3.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/
--rw-------   0 ajung     (1000) ajung     (1000)       23 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/MANIFEST.in
--rw-------   0 ajung     (1000) ajung     (1000)     5599 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     1628 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/README.rst
-drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/
--rw-------   0 ajung     (1000) ajung     (1000)     5599 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)      454 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/SOURCES.txt
--rw-------   0 ajung     (1000) ajung     (1000)        1 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/dependency_links.txt
--rw-------   0 ajung     (1000) ajung     (1000)       90 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/entry_points.txt
--rw-------   0 ajung     (1000) ajung     (1000)       48 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/requires.txt
--rw-------   0 ajung     (1000) ajung     (1000)        9 2023-06-21 12:12:06.000000 fs.webdavfs-0.4.3/fs.webdavfs.egg-info/top_level.txt
--rw-------   0 ajung     (1000) ajung     (1000)       91 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/setup.cfg
--rw-------   0 ajung     (1000) ajung     (1000)     1485 2023-06-21 12:10:25.000000 fs.webdavfs-0.4.3/setup.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/webdavfs/
--rw-------   0 ajung     (1000) ajung     (1000)       14 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/webdavfs/__init__.py
--rw-------   0 ajung     (1000) ajung     (1000)     1103 2023-06-21 12:09:41.000000 fs.webdavfs-0.4.3/webdavfs/opener.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:12:06.266267 fs.webdavfs-0.4.3/webdavfs/tests/
--rw-------   0 ajung     (1000) ajung     (1000)       14 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/webdavfs/tests/__init__.py
--rw-------   0 ajung     (1000) ajung     (1000)      991 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/webdavfs/tests/base.py
--rw-------   0 ajung     (1000) ajung     (1000)     1674 2021-01-27 07:37:18.000000 fs.webdavfs-0.4.3/webdavfs/tests/test_docker.py
--rw-------   0 ajung     (1000) ajung     (1000)      421 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/webdavfs/tests/test_opener.py
--rw-------   0 ajung     (1000) ajung     (1000)      712 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3/webdavfs/tests/test_server.py
--rw-------   0 ajung     (1000) ajung     (1000)    13816 2023-06-21 12:09:41.000000 fs.webdavfs-0.4.3/webdavfs/webdavfs.py
+drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:56:09.158695 fs.webdavfs-0.4.3.1/
+-rw-------   0 ajung     (1000) ajung     (1000)     1771 2023-06-21 12:11:16.000000 fs.webdavfs-0.4.3.1/HISTORY.rst
+-rw-------   0 ajung     (1000) ajung     (1000)       36 2023-06-21 12:55:14.000000 fs.webdavfs-0.4.3.1/MANIFEST.in
+-rw-------   0 ajung     (1000) ajung     (1000)     5601 2023-06-21 12:56:09.158695 fs.webdavfs-0.4.3.1/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     1628 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/README.rst
+drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:56:09.154695 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/
+-rw-------   0 ajung     (1000) ajung     (1000)     5601 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)      466 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/SOURCES.txt
+-rw-------   0 ajung     (1000) ajung     (1000)        1 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/dependency_links.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       90 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/entry_points.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       48 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/requires.txt
+-rw-------   0 ajung     (1000) ajung     (1000)        9 2023-06-21 12:56:09.000000 fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/top_level.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       91 2023-06-21 12:56:09.158695 fs.webdavfs-0.4.3.1/setup.cfg
+-rw-------   0 ajung     (1000) ajung     (1000)     1487 2023-06-21 12:55:52.000000 fs.webdavfs-0.4.3.1/setup.py
+drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:56:09.154695 fs.webdavfs-0.4.3.1/webdavfs/
+-rw-------   0 ajung     (1000) ajung     (1000)       14 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/webdavfs/__init__.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1103 2023-06-21 12:09:41.000000 fs.webdavfs-0.4.3.1/webdavfs/opener.py
+drwx------   0 ajung     (1000) ajung     (1000)        0 2023-06-21 12:56:09.158695 fs.webdavfs-0.4.3.1/webdavfs/tests/
+-rw-------   0 ajung     (1000) ajung     (1000)       14 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/webdavfs/tests/__init__.py
+-rw-------   0 ajung     (1000) ajung     (1000)      991 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/webdavfs/tests/base.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1674 2021-01-27 07:37:18.000000 fs.webdavfs-0.4.3.1/webdavfs/tests/test_docker.py
+-rw-------   0 ajung     (1000) ajung     (1000)      421 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/webdavfs/tests/test_opener.py
+-rw-------   0 ajung     (1000) ajung     (1000)      712 2021-01-27 07:33:23.000000 fs.webdavfs-0.4.3.1/webdavfs/tests/test_server.py
+-rw-------   0 ajung     (1000) ajung     (1000)    13816 2023-06-21 12:09:41.000000 fs.webdavfs-0.4.3.1/webdavfs/webdavfs.py
```

### Comparing `fs.webdavfs-0.4.3/PKG-INFO` & `fs.webdavfs-0.4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fs.webdavfs
-Version: 0.4.3
+Version: 0.4.3.1
 Summary: WebDAV support for pyfilesystem2
 Home-page: http://pypi.python.org/pypi/fs.webdavfs/
 Author: Andreas Jung and others
 Author-email: info@zopyx.com
 License: MIT
 Description: fs.webdavfs
         ===========
```

### Comparing `fs.webdavfs-0.4.3/README.rst` & `fs.webdavfs-0.4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `fs.webdavfs-0.4.3/fs.webdavfs.egg-info/PKG-INFO` & `fs.webdavfs-0.4.3.1/fs.webdavfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fs.webdavfs
-Version: 0.4.3
+Version: 0.4.3.1
 Summary: WebDAV support for pyfilesystem2
 Home-page: http://pypi.python.org/pypi/fs.webdavfs/
 Author: Andreas Jung and others
 Author-email: info@zopyx.com
 License: MIT
 Description: fs.webdavfs
         ===========
```

### Comparing `fs.webdavfs-0.4.3/setup.py` & `fs.webdavfs-0.4.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,9 +46,9 @@
     name='fs.webdavfs',
     packages=find_packages(exclude=("tests",)),
     platforms=['any'],
     setup_requires=['nose'],
     tests_require=['docker'],
     test_suite='webdavfs.tests',
     url="http://pypi.python.org/pypi/fs.webdavfs/",
-    version="0.4.3"
+    version="0.4.3.1"
 )
```

### Comparing `fs.webdavfs-0.4.3/webdavfs/opener.py` & `fs.webdavfs-0.4.3.1/webdavfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs.webdavfs-0.4.3/webdavfs/tests/base.py` & `fs.webdavfs-0.4.3.1/webdavfs/tests/base.py`

 * *Files identical despite different names*

### Comparing `fs.webdavfs-0.4.3/webdavfs/tests/test_docker.py` & `fs.webdavfs-0.4.3.1/webdavfs/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `fs.webdavfs-0.4.3/webdavfs/tests/test_server.py` & `fs.webdavfs-0.4.3.1/webdavfs/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `fs.webdavfs-0.4.3/webdavfs/webdavfs.py` & `fs.webdavfs-0.4.3.1/webdavfs/webdavfs.py`

 * *Files identical despite different names*

