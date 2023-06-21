# Comparing `tmp/unifi_tracker-0.0.7.tar.gz` & `tmp/unifi_tracker-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_tracker-0.0.7.tar", last modified: Mon Jun 19 23:20:29 2023, max compression
+gzip compressed data, was "unifi_tracker-0.0.8.tar", last modified: Tue Jun 20 23:58:50 2023, max compression
```

## Comparing `unifi_tracker-0.0.7.tar` & `unifi_tracker-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2023-06-19 21:44:59.000000 unifi_tracker-0.0.7/LICENSE
--rw-r--r--   0 joelp     (1000) joelp     (1000)     6140 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)     5571 2023-06-19 21:37:12.000000 unifi_tracker-0.0.7/README.md
--rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2022-01-19 19:50:03.000000 unifi_tracker-0.0.7/pyproject.toml
--rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/setup.cfg
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/unifi_tracker/
--rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2023-06-19 21:45:24.000000 unifi_tracker-0.0.7/src/unifi_tracker/__init__.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)     6971 2023-06-19 23:08:20.000000 unifi_tracker-0.0.7/src/unifi_tracker/unifi_tracker.py
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     6140 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)      321 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/tests/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     2263 2022-02-09 21:14:36.000000 unifi_tracker-0.0.7/tests/test_diff.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)     2100 2023-06-19 21:19:32.000000 unifi_tracker-0.0.7/tests/test_property_setters.py
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-20 23:58:50.260365 unifi_tracker-0.0.8/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2023-06-19 21:44:59.000000 unifi_tracker-0.0.8/LICENSE
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6292 2023-06-20 23:58:50.260365 unifi_tracker-0.0.8/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     5723 2023-06-20 23:48:25.000000 unifi_tracker-0.0.8/README.md
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2022-01-19 19:50:03.000000 unifi_tracker-0.0.8/pyproject.toml
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2023-06-20 23:58:50.260365 unifi_tracker-0.0.8/setup.cfg
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-20 23:58:50.256365 unifi_tracker-0.0.8/src/
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-20 23:58:50.256365 unifi_tracker-0.0.8/src/unifi_tracker/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2023-06-20 23:49:18.000000 unifi_tracker-0.0.8/src/unifi_tracker/__init__.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6971 2023-06-19 23:08:20.000000 unifi_tracker-0.0.8/src/unifi_tracker/unifi_tracker.py
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-20 23:58:50.260365 unifi_tracker-0.0.8/src/unifi_tracker.egg-info/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6292 2023-06-20 23:58:50.000000 unifi_tracker-0.0.8/src/unifi_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      321 2023-06-20 23:58:50.000000 unifi_tracker-0.0.8/src/unifi_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2023-06-20 23:58:50.000000 unifi_tracker-0.0.8/src/unifi_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2023-06-20 23:58:50.000000 unifi_tracker-0.0.8/src/unifi_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-20 23:58:50.260365 unifi_tracker-0.0.8/tests/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2263 2022-02-09 21:14:36.000000 unifi_tracker-0.0.8/tests/test_diff.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2100 2023-06-19 21:19:32.000000 unifi_tracker-0.0.8/tests/test_property_setters.py
```

### Comparing `unifi_tracker-0.0.7/LICENSE` & `unifi_tracker-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unifi_tracker-0.0.7/PKG-INFO` & `unifi_tracker-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi_tracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,18 +77,19 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.8
+- Bug fix: Recreate paho.mqtt.client.Client to avoid ```ERROR:labtracker:SSL/TLS has already been configured.``` on MQTT disconnect/reconnect.
 ### v0.0.7
 - Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
 - Tested under Python11 and Debian12.
--
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

### Comparing `unifi_tracker-0.0.7/README.md` & `unifi_tracker-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,19 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.8
+- Bug fix: Recreate paho.mqtt.client.Client to avoid ```ERROR:labtracker:SSL/TLS has already been configured.``` on MQTT disconnect/reconnect.
 ### v0.0.7
 - Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
 - Tested under Python11 and Debian12.
--
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

### Comparing `unifi_tracker-0.0.7/setup.cfg` & `unifi_tracker-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unifi_tracker
-version = 0.0.7
+version = 0.0.8
 author = Joel P.
 author_email = joelp@live.com
 description = Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/idatum/unifi_tracker
 project_urls =
```

### Comparing `unifi_tracker-0.0.7/src/unifi_tracker/unifi_tracker.py` & `unifi_tracker-0.0.8/src/unifi_tracker/unifi_tracker.py`

 * *Files identical despite different names*

### Comparing `unifi_tracker-0.0.7/src/unifi_tracker.egg-info/PKG-INFO` & `unifi_tracker-0.0.8/src/unifi_tracker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi-tracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,18 +77,19 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.8
+- Bug fix: Recreate paho.mqtt.client.Client to avoid ```ERROR:labtracker:SSL/TLS has already been configured.``` on MQTT disconnect/reconnect.
 ### v0.0.7
 - Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
 - Tested under Python11 and Debian12.
--
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

### Comparing `unifi_tracker-0.0.7/tests/test_diff.py` & `unifi_tracker-0.0.8/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `unifi_tracker-0.0.7/tests/test_property_setters.py` & `unifi_tracker-0.0.8/tests/test_property_setters.py`

 * *Files identical despite different names*

