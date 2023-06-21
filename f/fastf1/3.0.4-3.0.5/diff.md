# Comparing `tmp/fastf1-3.0.4.tar.gz` & `tmp/fastf1-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-3.0.4.tar", last modified: Sat Jun  3 16:58:13 2023, max compression
+gzip compressed data, was "fastf1-3.0.5.tar", last modified: Wed Jun 21 09:59:43 2023, max compression
```

## Comparing `fastf1-3.0.4.tar` & `fastf1-3.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-03 16:57:57.000000 fastf1-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 16:57:57.000000 fastf1-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 16:58:13.087779 fastf1-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-03 16:57:57.000000 fastf1-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   136246 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/ergast/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/ergast/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/req.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1/signalr_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/events/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/events/_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/hubs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/hubs/_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.087779 fastf1-3.0.4/fastf1/signalr_aio/transports/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 16:57:57.000000 fastf1-3.0.4/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:58:13.083778 fastf1-3.0.4/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-03 16:58:13.000000 fastf1-3.0.4/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 16:58:12.000000 fastf1-3.0.4/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 16:57:57.000000 fastf1-3.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 16:58:13.087779 fastf1-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-03 16:57:57.000000 fastf1-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.619133 fastf1-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 09:59:29.000000 fastf1-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 09:59:29.000000 fastf1-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-21 09:59:43.619133 fastf1-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-21 09:59:29.000000 fastf1-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70557 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136455 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/signalr_aio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1/signalr_aio/hubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.619133 fastf1-3.0.5/fastf1/signalr_aio/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 09:59:29.000000 fastf1-3.0.5/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:59:43.615133 fastf1-3.0.5/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 09:59:43.000000 fastf1-3.0.5/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 09:59:29.000000 fastf1-3.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 09:59:43.619133 fastf1-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 09:59:29.000000 fastf1-3.0.5/setup.py
```

### Comparing `fastf1-3.0.4/LICENSE` & `fastf1-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/PKG-INFO` & `fastf1-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.4
+Version: 3.0.5
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.4 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.5 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
```

### Comparing `fastf1-3.0.4/README.md` & `fastf1-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/__init__.py` & `fastf1-3.0.5/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/_api.py` & `fastf1-3.0.5/fastf1/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,14 +348,17 @@
     lapcnt = 0  # we're keeping two separate lap counts because sometimes the api has a non existent lap too much...
     api_lapcnt = 0  # ...at the beginning; we can correct that though;
     # api_lapcnt does not count backwards even if the source data does
     in_past = False  # flag for when the data went back in time
 
     personal_best_lap_times = list()
 
+    session_split_times = [datetime.timedelta(0)]
+    # start times of (sub)sessions (Q1, Q2, Q3)
+
     pitstops = -1  # start with -1 because first is out lap, needs to be zero after that
 
     # iterate through the data; new lap triggers next row in data
     for time, resp in driver_raw:
         # the first three ifs are just edge case handling for the rare sessions were the data goes back in time
         if in_past and 'NumberOfLaps' in resp and resp['NumberOfLaps'] == api_lapcnt:
             in_past = False  # we're back in the present
@@ -419,16 +422,34 @@
                 # or beginning of next lap less than 5 seconds away
                 drv_data['PitOutTime'][lapcnt + 1] = to_timedelta(time)  # add to next lap
                 pitstops += 1
             else:
                 drv_data['PitOutTime'][lapcnt] = to_timedelta(time)  # add to current lap
                 pitstops += 1
 
+        # Get save information about personal best lap times at the timestamp
+        # at which this information was received.
+        # Whenever a lap is deleted (if that happens quickly after it was set),
+        # the previous 'BestLapTime' value is sent again. There is some extra
+        # logic at then end that correctly marks personal best laps based on
+        # the data that is saved here.
         if val := recursive_dict_get(resp, 'BestLapTime', 'Value'):
-            personal_best_lap_times.append(to_timedelta(val))
+            personal_best_lap_times.append(
+                (to_timedelta(time), to_timedelta(val))
+            )
+
+        # Create approximate (sub)session (i.e. quali) split times by
+        # (mis)using the session number counter from 'BestLapTimes'.
+        # (Note: those lap times cannot be used for correct personal best
+        #  detection, because the previous value is not resent here when a lap
+        #  is deleted.)
+        if val := recursive_dict_get(resp, 'BestLapTimes'):
+            session_n = int(list(val.keys())[0])
+            if (session_n + 1) > len(session_split_times):
+                session_split_times.append(to_timedelta(time))
 
         # new lap; create next row
         if 'NumberOfLaps' in resp and resp['NumberOfLaps'] > api_lapcnt:
             api_lapcnt += 1
             # make sure the car actually drove out of the pits already; it can't be a new lap if it didn't
             if pitstops >= 0:
                 drv_data['Time'][lapcnt] = to_timedelta(time)
@@ -585,22 +606,33 @@
             drv_data['Sector2SessionTime'][i+1] = new_s2_time
         if (new_s3_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1]
                 + drv_data['Sector2Time'][i+1]
                 + drv_data['Sector3Time'][i+1]) \
                 < drv_data['Sector3SessionTime'][i+1]:
             drv_data['Sector3SessionTime'][i+1] = new_s3_time
 
-    # iterate over list of personal lap times set 'IsPersonalBest'
-    # when a lap is deleted, the API resends the previous personal best.
+    # Iterate over list of personal lap times set 'IsPersonalBest'.
+    # When a lap is deleted, the API resends the previous personal best.
     # Therefore, by iterating in reverse, if any lap is encountered that is
     # quicker than already processed personal best lap times, it must have
     # been deleted.
+    # This is just best effort but not exhaustive as it can only handle lap
+    # times that were deleted quickly (before the next personal best was set).
     _corrected_personal_best_lap_times = list()
     # list is only used for backreference within the loop
-    for pb_lap_time in reversed(personal_best_lap_times):
+    cur_sn = len(session_split_times) - 1
+    # current (sub)session number, personal best lap times need to be
+    # considered for each (sub)session individually
+    for time, pb_lap_time in reversed(personal_best_lap_times):
+        if time < session_split_times[cur_sn]:
+            # transitioned into the previous (sub)session (reverse iteration!)
+            # reset the reference list, so time are considered individually
+            cur_sn -= 1
+            _corrected_personal_best_lap_times = list()
+
         if _corrected_personal_best_lap_times:
             if pb_lap_time in _corrected_personal_best_lap_times:
                 continue
             elif pb_lap_time < min(_corrected_personal_best_lap_times):
                 continue
 
         _corrected_personal_best_lap_times.append(pb_lap_time)
```

### Comparing `fastf1-3.0.4/fastf1/api.py` & `fastf1-3.0.5/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/core.py` & `fastf1-3.0.5/fastf1/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2014,15 +2014,20 @@
             if session_name in _QUALI_LIKE_SESSIONS:
                 rename_return.update({
                     'Q1': 'Q1',
                     'Q2': 'Q2',
                     'Q3': 'Q3',
                 })
 
-        d = data.loc[:, list(rename_return.keys())] \
+        # ergast does not provide all data for old sessions
+        # (example: 'driverCode'), select only existing columns
+        existing_keys = set(rename_return.keys())\
+            .intersection(data.columns)
+
+        d = data.loc[:, list(existing_keys)] \
             .rename(columns=rename_return) \
             .astype({'DriverNumber': 'str'})
 
         if load_drivers:
             d['FullName'] = d['FirstName'] + " " + d['LastName']
 
         return d
```

### Comparing `fastf1-3.0.4/fastf1/ergast/interface.py` & `fastf1-3.0.5/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/ergast/legacy.py` & `fastf1-3.0.5/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/ergast/sphinx.py` & `fastf1-3.0.5/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/ergast/structure.py` & `fastf1-3.0.5/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/events.py` & `fastf1-3.0.5/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/legacy.py` & `fastf1-3.0.5/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/livetiming/__init__.py` & `fastf1-3.0.5/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/livetiming/__main__.py` & `fastf1-3.0.5/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/livetiming/client.py` & `fastf1-3.0.5/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/livetiming/data.py` & `fastf1-3.0.5/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/logger.py` & `fastf1-3.0.5/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/plotting.py` & `fastf1-3.0.5/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/req.py` & `fastf1-3.0.5/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/signalr_aio/_connection.py` & `fastf1-3.0.5/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.0.5/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.0.5/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.0.5/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1/utils.py` & `fastf1-3.0.5/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/fastf1.egg-info/PKG-INFO` & `fastf1-3.0.5/fastf1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.4
+Version: 3.0.5
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.4 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.5 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
```

### Comparing `fastf1-3.0.4/fastf1.egg-info/SOURCES.txt` & `fastf1-3.0.5/fastf1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.4/setup.cfg` & `fastf1-3.0.5/setup.cfg`

 * *Files identical despite different names*

