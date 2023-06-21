# Comparing `tmp/optimal_loc-0.1.6.tar.gz` & `tmp/optimal_loc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.6.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.7.tar", max compression
```

## Comparing `optimal_loc-0.1.6.tar` & `optimal_loc-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.6/LICENSE
--rw-r--r--   0        0        0     5212 2023-06-21 13:00:03.522976 optimal_loc-0.1.6/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.6/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-06-21 13:10:57.614671 optimal_loc-0.1.6/optimal_loc/__init__.py
--rw-r--r--   0        0        0    19221 2023-06-21 13:10:12.600058 optimal_loc-0.1.6/optimal_loc/app.py
--rw-r--r--   0        0        0      684 2023-06-18 22:59:24.338162 optimal_loc-0.1.6/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.6/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.6/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-06-21 13:11:08.442029 optimal_loc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 optimal_loc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5212 2023-06-21 13:00:03.522976 optimal_loc-0.1.7/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.7/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-06-21 13:15:41.817551 optimal_loc-0.1.7/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    19257 2023-06-21 13:15:20.412572 optimal_loc-0.1.7/optimal_loc/app.py
+-rw-r--r--   0        0        0      684 2023-06-18 22:59:24.338162 optimal_loc-0.1.7/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.7/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.7/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-06-21 13:15:46.777213 optimal_loc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 optimal_loc-0.1.7/PKG-INFO
```

### Comparing `optimal_loc-0.1.6/LICENSE` & `optimal_loc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.6/README.md` & `optimal_loc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.6/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.7/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.6/optimal_loc/app.py` & `optimal_loc-0.1.7/optimal_loc/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         raw_data[HEX_LOCATION] = raw_data.apply(lambda x: h3_to_geo(h=x[HEXAGON_ID]), 1)
         raw_data[HEX_LAT] = raw_data.apply(lambda x: x[HEX_LOCATION][0], 1)
         raw_data[HEX_LON] = raw_data.apply(lambda x: x[HEX_LOCATION][1], 1)
         raw_data = raw_data.drop(columns=HEX_LOCATION)
 
         self.event_frequency_data = raw_data
 
-    def create_hexagon_distance_data(self, raw_data: DataFrame, hex_size: str = 'auto') -> None:
+    def create_hexagon_distance_data(self, raw_data: DataFrame, hex_size: str = 'auto', resolution: int = None) -> None:
         """
         Create a DataFrame containing the distances between pairs of hexagonal regions.
 
         Parameters:
         raw_data (DataFrame): pandas DataFrame containing event data, with columns "latitude" and "longitude".
         hex_size (string): You can specify hexagon sizes by small, medium or big, otherwise it will be assigned as auto
 
@@ -126,15 +126,15 @@
 
         Example:
         raw_event_data = pd.DataFrame({'latitude': [42.123, 42.456, 42.789], 'longitude': [-71.123, -71.456, -71.789]})
         object = OptimalLoc()
         object.create_hexagon_distance_data(raw_event_data)
         hex_distance_data = object.hex_distance_data
         """
-        self.event_frequency(raw_data, hex_size)
+        self.event_frequency(raw_data, hex_size, resolution)
         event_data = self.event_frequency_data.copy()
 
         hexagon_ids = event_data[[HEXAGON_ID, HEX_LAT, HEX_LON]].rename(columns={HEXAGON_ID: HEXAGON})
         out_list = array(meshgrid(hexagon_ids.hexagon, hexagon_ids.hexagon)).T.reshape(-1, 2)
 
         hex_distance_data = DataFrame(data=out_list, columns=[FROMHEX, TOHEX])
```

### Comparing `optimal_loc-0.1.6/optimal_loc/app_constants.py` & `optimal_loc-0.1.7/optimal_loc/app_constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.6/optimal_loc/st_app.py` & `optimal_loc-0.1.7/optimal_loc/st_app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.6/pyproject.toml` & `optimal_loc-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.6"
+version = "0.1.7"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.6/PKG-INFO` & `optimal_loc-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

