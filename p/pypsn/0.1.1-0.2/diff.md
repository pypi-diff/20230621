# Comparing `tmp/pypsn-0.1.1.tar.gz` & `tmp/pypsn-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypsn-0.1.1.tar", last modified: Tue Apr 18 12:02:00 2023, max compression
+gzip compressed data, was "pypsn-0.2.tar", last modified: Wed Jun 21 18:21:27 2023, max compression
```

## Comparing `pypsn-0.1.1.tar` & `pypsn-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/
--rw-r--r--   0 vanous    (1000) vanous    (1000)     1063 2023-04-05 17:36:44.000000 pypsn-0.1.1/LICENSE
--rw-r--r--   0 vanous    (1000) vanous    (1000)     2255 2023-04-18 12:02:00.553688 pypsn-0.1.1/PKG-INFO
--rw-r--r--   0 vanous    (1000) vanous    (1000)     1847 2023-04-18 11:54:55.000000 pypsn-0.1.1/README.md
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/pypsn/
--rwxr-xr-x   0 vanous    (1000) vanous    (1000)     9627 2023-04-18 11:58:57.000000 pypsn-0.1.1/pypsn/__init__.py
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/pypsn.egg-info/
--rw-r--r--   0 vanous    (1000) vanous    (1000)     2255 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/PKG-INFO
--rw-r--r--   0 vanous    (1000) vanous    (1000)      160 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/SOURCES.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)        1 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/dependency_links.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)        6 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/top_level.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)       38 2023-04-18 12:02:00.553688 pypsn-0.1.1/setup.cfg
--rw-r--r--   0 vanous    (1000) vanous    (1000)      611 2023-04-18 11:52:07.000000 pypsn-0.1.1/setup.py
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-06-21 18:21:27.256646 pypsn-0.2/
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     1063 2023-04-05 17:36:44.000000 pypsn-0.2/LICENSE
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     2241 2023-06-21 18:21:27.256646 pypsn-0.2/PKG-INFO
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     1835 2023-06-21 18:03:36.000000 pypsn-0.2/README.md
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-06-21 18:21:27.252646 pypsn-0.2/pypsn/
+-rwxr-xr-x   0 vanous    (1000) vanous    (1000)     9637 2023-06-21 18:03:13.000000 pypsn-0.2/pypsn/__init__.py
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-06-21 18:21:27.256646 pypsn-0.2/pypsn.egg-info/
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     2241 2023-06-21 18:21:27.000000 pypsn-0.2/pypsn.egg-info/PKG-INFO
+-rw-r--r--   0 vanous    (1000) vanous    (1000)      160 2023-06-21 18:21:27.000000 pypsn-0.2/pypsn.egg-info/SOURCES.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)        1 2023-06-21 18:21:27.000000 pypsn-0.2/pypsn.egg-info/dependency_links.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)        6 2023-06-21 18:21:27.000000 pypsn-0.2/pypsn.egg-info/top_level.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)       38 2023-06-21 18:21:27.256646 pypsn-0.2/setup.cfg
+-rw-r--r--   0 vanous    (1000) vanous    (1000)      609 2023-06-21 18:09:36.000000 pypsn-0.2/setup.py
```

### Comparing `pypsn-0.1.1/LICENSE` & `pypsn-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypsn-0.1.1/PKG-INFO` & `pypsn-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsn
-Version: 0.1.1
+Version: 0.2
 Summary: PosiStageNet parser
 Home-page: https://github.com/open-stage/python-psn
 Author: vanous
 Author-email: noreply@nodomain.com
 License: MIT
 Project-URL: Source, https://github.com/open-stage/python-psn
 Project-URL: Changelog, https://github.com/open-stage/python-psn/blob/master/CHANGELOG.md
@@ -43,15 +43,15 @@
 
     if isinstance(data, pypsn_module.psn_info_packet): # packet type: psn.psn_info_packet
         print(data.name) # print server name
         for tracker in data.trackers: # loop through all trackers
             print(tracker.tracker_name) # print the received tracker name
 
 # provide a callback function and an IP address
-receiver = pypsn.receiver(callback_function, "10.0.0.1")
+receiver = pypsn.receiver(callback_function)
 receiver.start()  # start the receiving thread
 
 receiver.stop() # stop receiving
 
 ```
 See examples folder for some more examples.
```

### Comparing `pypsn-0.1.1/README.md` & `pypsn-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     if isinstance(data, pypsn_module.psn_info_packet): # packet type: psn.psn_info_packet
         print(data.name) # print server name
         for tracker in data.trackers: # loop through all trackers
             print(tracker.tracker_name) # print the received tracker name
 
 # provide a callback function and an IP address
-receiver = pypsn.receiver(callback_function, "10.0.0.1")
+receiver = pypsn.receiver(callback_function)
 receiver.start()  # start the receiving thread
 
 receiver.stop() # stop receiving
 
 ```
 See examples folder for some more examples.
```

### Comparing `pypsn-0.1.1/pypsn/__init__.py` & `pypsn-0.2/pypsn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         return str(os.name)
 
     else:
         return "Operating system not supported"
 
 
 class receiver(Thread):
-    def __init__(self, callback, ip_addr, mcast_port=56565, timeout=None):
+    def __init__(self, callback, ip_addr="0.0.0.0", mcast_port=56565, timeout=None):
         Thread.__init__(self)
         self.callback = callback
         self.running = True
         self.socket = get_socket(ip_addr, mcast_port)
         if timeout is not None and self.socket is not None:
             self.socket.settimeout(timeout)
```

### Comparing `pypsn-0.1.1/pypsn.egg-info/PKG-INFO` & `pypsn-0.2/pypsn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsn
-Version: 0.1.1
+Version: 0.2
 Summary: PosiStageNet parser
 Home-page: https://github.com/open-stage/python-psn
 Author: vanous
 Author-email: noreply@nodomain.com
 License: MIT
 Project-URL: Source, https://github.com/open-stage/python-psn
 Project-URL: Changelog, https://github.com/open-stage/python-psn/blob/master/CHANGELOG.md
@@ -43,15 +43,15 @@
 
     if isinstance(data, pypsn_module.psn_info_packet): # packet type: psn.psn_info_packet
         print(data.name) # print server name
         for tracker in data.trackers: # loop through all trackers
             print(tracker.tracker_name) # print the received tracker name
 
 # provide a callback function and an IP address
-receiver = pypsn.receiver(callback_function, "10.0.0.1")
+receiver = pypsn.receiver(callback_function)
 receiver.start()  # start the receiving thread
 
 receiver.stop() # stop receiving
 
 ```
 See examples folder for some more examples.
```

### Comparing `pypsn-0.1.1/setup.py` & `pypsn-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pypsn",
-    version="0.1.1",
+    version="0.2",
     long_description=long_description,
     description="PosiStageNet parser",
     license="MIT",
     url="https://github.com/open-stage/python-psn",
     long_description_content_type="text/markdown",
     author="vanous",
     author_email="noreply@nodomain.com",
```

