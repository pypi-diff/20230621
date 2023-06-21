# Comparing `tmp/homeassistant-historical-sensor-1.0.0a2.tar.gz` & `tmp/homeassistant-historical-sensor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-1.0.0a2.tar", last modified: Mon Jun 19 12:52:56 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-1.0.1.tar", last modified: Wed Jun 21 15:14:42 2023, max compression
```

## Comparing `homeassistant-historical-sensor-1.0.0a2.tar` & `homeassistant-historical-sensor-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:52:56.645316 homeassistant-historical-sensor-1.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 12:52:56.645316 homeassistant-historical-sensor-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:52:56.645316 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:52:56.645316 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 12:52:56.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-19 12:52:56.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:52:56.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 12:52:56.000000 homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 12:52:43.000000 homeassistant-historical-sensor-1.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-19 12:52:56.645316 homeassistant-historical-sensor-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 15:14:42.000000 homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 15:14:32.000000 homeassistant-historical-sensor-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 15:14:42.059312 homeassistant-historical-sensor-1.0.1/setup.cfg
```

### Comparing `homeassistant-historical-sensor-1.0.0a2/PKG-INFO` & `homeassistant-historical-sensor-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.0a2
+Version: 1.0.1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a2
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-1.0.0a2/README.md` & `homeassistant-historical-sensor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/consts.py` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/consts.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,18 +306,18 @@
         #
         # Calculate stats
         #
         statistics_data = await self.async_calculate_statistic_data(
             hist_states, latest=latest
         )
 
-        for stat in statistics_data:
-            tmp = dict(stat)
-            start_dt = dtutil.as_local(tmp.pop("start"))
-            _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
+        # for stat in statistics_data:
+        #     tmp = dict(stat)
+        #     start_dt = dtutil.as_local(tmp.pop("start"))
+        #     _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
 
         if valid_statistic_id(self.statatistic_id):
             async_add_external_statistics(self.hass, statistics_meta, statistics_data)
         else:
             async_import_statistics(self.hass, statistics_meta, statistics_data)
 
         return hist_states
```

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.0a2
+Version: 1.0.1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a2
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-1.0.0a2/homeassistant_historical_sensor.egg-info/SOURCES.txt` & `homeassistant-historical-sensor-1.0.1/homeassistant_historical_sensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a2/setup.cfg` & `homeassistant-historical-sensor-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 1.0.0a2
+version = 1.0.1
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

