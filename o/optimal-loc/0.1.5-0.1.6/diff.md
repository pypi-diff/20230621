# Comparing `tmp/optimal_loc-0.1.5.tar.gz` & `tmp/optimal_loc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.5.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.6.tar", max compression
```

## Comparing `optimal_loc-0.1.5.tar` & `optimal_loc-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.5/LICENSE
--rw-r--r--   0        0        0     5240 2023-06-14 22:54:07.375334 optimal_loc-0.1.5/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.5/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-06-14 22:54:07.370490 optimal_loc-0.1.5/optimal_loc/__init__.py
--rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.5/optimal_loc/app.py
--rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.5/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.5/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.5/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-06-14 22:54:07.372554 optimal_loc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 optimal_loc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5212 2023-06-21 13:00:03.522976 optimal_loc-0.1.6/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.6/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-06-21 13:10:57.614671 optimal_loc-0.1.6/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    19221 2023-06-21 13:10:12.600058 optimal_loc-0.1.6/optimal_loc/app.py
+-rw-r--r--   0        0        0      684 2023-06-18 22:59:24.338162 optimal_loc-0.1.6/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.6/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.6/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-06-21 13:11:08.442029 optimal_loc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 optimal_loc-0.1.6/PKG-INFO
```

### Comparing `optimal_loc-0.1.5/LICENSE` & `optimal_loc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.5/README.md` & `optimal_loc-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 5. Read the distances:
    - If you have a large distance dataset, you can store it in a MongoDB database and read it using the `read_distances_from_mongodb` method.
    - Alternatively, you can directly read the distance data from a dataframe using the `read_distances` method.
 
     Example (reading from MongoDB):
     ```bash
-    sol.read_distances_from_mongodb(mongo_client=my_mongo_client("username", "password"),
+    sol.read_distances_from_mongodb(mongo_client=MongoClient,
                                     mongo_database_name="db_name",
                                     mongo_collection_name="collection_name")
     ```
 
     Example (reading from a dataframe):
     ```bash
     sol.read_distances(read_from_dataframe=True, distance_dataframe=distance_data)
```

### Comparing `optimal_loc-0.1.5/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.6/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.5/optimal_loc/app.py` & `optimal_loc-0.1.6/optimal_loc/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                          popup={"Total Event": i["total_event"]}
                          ).add_to(map_nyc)
 
         plugins.Fullscreen(position='topleft').add_to(map_nyc)
 
         return map_nyc
 
-    def event_frequency(self, raw_input_data: DataFrame, hex_size: str = 'auto') -> None:
+    def event_frequency(self, raw_input_data: DataFrame, hex_size: str = 'auto', resolution: int = None) -> None:
         """
         Calculate the frequency of events in each hexagonal region.
 
         Parameters:
         raw_data (DataFrame): pandas DataFrame containing event data, with columns "latitude" and "longitude".
         hex_size (string): You can specify hexagon sizes by small, medium or big, otherwise it will be assigned as auto
 
@@ -82,15 +82,18 @@
         raw_event_data = pd.DataFrame({'latitude': [42.123, 42.456, 42.789], 'longitude': [-71.123, -71.456, -71.789]})
         object_name = OptimalLoc()
         object_name.event_frequency(raw_event_data)
         event_freq_data = object_name.event_frequency_data
         print(event_freq_data)
         """
         raw_data = raw_input_data.copy()
-        self.resolution = set_resolution(raw_data, hex_size)
+        if resolution:
+            self.resolution = resolution
+        else:
+            self.resolution = set_resolution(raw_data, hex_size)
 
         raw_data[HEX_ID] = raw_data.apply(lambda x: geo_to_h3(x[LATITUDE], x[LONGITUDE], self.resolution), 1)
 
         raw_data = raw_data[HEX_ID].value_counts().reset_index().rename(columns={INDEX: HEXAGON_ID,
                                                                                  HEX_ID: TOTAL_EVENT})
         raw_data[HEX_LOCATION] = raw_data.apply(lambda x: h3_to_geo(h=x[HEXAGON_ID]), 1)
         raw_data[HEX_LAT] = raw_data.apply(lambda x: x[HEX_LOCATION][0], 1)
```

### Comparing `optimal_loc-0.1.5/optimal_loc/app_constants.py` & `optimal_loc-0.1.6/optimal_loc/app_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 00000000: 434f 4c4f 5552 535f 4c49 5354 203d 205b  COLOURS_LIST = [
 00000010: 0a20 2020 2027 6461 726b 7265 6427 2c0a  .    'darkred',.
 00000020: 2020 2020 276f 7261 6e67 6527 2c0a 2020      'orange',.  
 00000030: 2020 2764 6172 6b67 7265 656e 272c 0a20    'darkgreen',. 
 00000040: 2020 2027 6461 726b 626c 7565 272c 0a20     'darkblue',. 
 00000050: 2020 2027 7075 7270 6c65 272c 0a20 2020     'purple',.   
-00000060: 2027 7069 6e6b 272c 0a20 2020 2027 626c   'pink',.    'bl
-00000070: 6163 6b27 0a5d 0a0a 4449 5354 414e 4345  ack'.]..DISTANCE
-00000080: 203d 2027 6469 7374 616e 6365 270a 4649   = 'distance'.FI
-00000090: 4c45 4e41 4d45 203d 2027 6f70 7469 6d61  LENAME = 'optima
-000000a0: 6c5f 6c6f 6361 7469 6f6e 732e 7069 636b  l_locations.pick
-000000b0: 6c65 270a 4652 4f4d 4845 5820 3d20 2766  le'.FROMHEX = 'f
-000000c0: 726f 6d68 6578 270a 544f 4845 5820 3d20  romhex'.TOHEX = 
-000000d0: 2774 6f68 6578 270a 0a46 524f 4d48 4558  'tohex'..FROMHEX
-000000e0: 5f4c 4154 203d 2027 6672 6f6d 6865 785f  _LAT = 'fromhex_
-000000f0: 6c61 7427 0a46 524f 4d48 4558 5f4c 4f4e  lat'.FROMHEX_LON
-00000100: 203d 2027 6672 6f6d 6865 785f 6c6f 6e27   = 'fromhex_lon'
-00000110: 0a0a 544f 4845 585f 4c41 5420 3d20 2774  ..TOHEX_LAT = 't
-00000120: 6f68 6578 5f6c 6174 270a 544f 4845 585f  ohex_lat'.TOHEX_
-00000130: 4c4f 4e20 3d20 2774 6f68 6578 5f6c 6f6e  LON = 'tohex_lon
-00000140: 270a 0a48 4156 4553 494e 455f 4449 5354  '..HAVESINE_DIST
-00000150: 203d 2027 6861 7665 7273 696e 655f 6469   = 'haversine_di
-00000160: 7374 270a 4845 5841 474f 4e20 3d20 2268  st'.HEXAGON = "h
-00000170: 6578 6167 6f6e 220a 4845 5841 474f 4e5f  exagon".HEXAGON_
-00000180: 4944 203d 2022 6865 7861 676f 6e5f 6964  ID = "hexagon_id
-00000190: 220a 4845 585f 4944 203d 2022 6865 785f  ".HEX_ID = "hex_
-000001a0: 6964 220a 0a48 4558 5f4c 4154 203d 2022  id"..HEX_LAT = "
-000001b0: 6865 785f 6c61 7422 0a48 4558 5f4c 4f4e  hex_lat".HEX_LON
-000001c0: 203d 2022 6865 785f 6c6f 6e22 0a48 4558   = "hex_lon".HEX
-000001d0: 5f4c 4f43 4154 494f 4e20 3d20 2268 6578  _LOCATION = "hex
-000001e0: 5f6c 6f63 6174 696f 6e22 0a0a 494e 4445  _location"..INDE
-000001f0: 5820 3d20 2269 6e64 6578 220a 4c41 5449  X = "index".LATI
-00000200: 5455 4445 203d 2022 6c61 7469 7475 6465  TUDE = "latitude
-00000210: 220a 4c4f 4e47 4954 5544 4520 3d20 226c  ".LONGITUDE = "l
-00000220: 6f6e 6769 7475 6465 220a 0a4f 5054 494d  ongitude"..OPTIM
-00000230: 414c 5f44 4154 415f 434f 4c55 4d4e 203d  AL_DATA_COLUMN =
-00000240: 2022 6f70 7469 6d61 6c5f 6461 7461 220a   "optimal_data".
-00000250: 5355 5050 4c59 5f44 4154 415f 434f 4c55  SUPPLY_DATA_COLU
-00000260: 4d4e 203d 2022 7375 7070 6c79 5f64 6174  MN = "supply_dat
-00000270: 6122 0a53 5550 504c 595f 4845 5841 474f  a".SUPPLY_HEXAGO
-00000280: 4e5f 4944 203d 2022 7375 7070 6c79 5f68  N_ID = "supply_h
-00000290: 6578 6167 6f6e 5f69 6422 0a0a 544f 5441  exagon_id"..TOTA
-000002a0: 4c5f 4556 454e 5420 3d20 2274 6f74 616c  L_EVENT = "total
-000002b0: 5f65 7665 6e74 220a                      _event".
+00000060: 2027 626c 6163 6b27 0a5d 0a0a 4449 5354   'black'.]..DIST
+00000070: 414e 4345 203d 2027 6469 7374 616e 6365  ANCE = 'distance
+00000080: 270a 4649 4c45 4e41 4d45 203d 2027 6f70  '.FILENAME = 'op
+00000090: 7469 6d61 6c5f 6c6f 6361 7469 6f6e 732e  timal_locations.
+000000a0: 7069 636b 6c65 270a 4652 4f4d 4845 5820  pickle'.FROMHEX 
+000000b0: 3d20 2766 726f 6d68 6578 270a 544f 4845  = 'fromhex'.TOHE
+000000c0: 5820 3d20 2774 6f68 6578 270a 0a46 524f  X = 'tohex'..FRO
+000000d0: 4d48 4558 5f4c 4154 203d 2027 6672 6f6d  MHEX_LAT = 'from
+000000e0: 6865 785f 6c61 7427 0a46 524f 4d48 4558  hex_lat'.FROMHEX
+000000f0: 5f4c 4f4e 203d 2027 6672 6f6d 6865 785f  _LON = 'fromhex_
+00000100: 6c6f 6e27 0a0a 544f 4845 585f 4c41 5420  lon'..TOHEX_LAT 
+00000110: 3d20 2774 6f68 6578 5f6c 6174 270a 544f  = 'tohex_lat'.TO
+00000120: 4845 585f 4c4f 4e20 3d20 2774 6f68 6578  HEX_LON = 'tohex
+00000130: 5f6c 6f6e 270a 0a48 4156 4553 494e 455f  _lon'..HAVESINE_
+00000140: 4449 5354 203d 2027 6861 7665 7273 696e  DIST = 'haversin
+00000150: 655f 6469 7374 270a 4845 5841 474f 4e20  e_dist'.HEXAGON 
+00000160: 3d20 2268 6578 6167 6f6e 220a 4845 5841  = "hexagon".HEXA
+00000170: 474f 4e5f 4944 203d 2022 6865 7861 676f  GON_ID = "hexago
+00000180: 6e5f 6964 220a 4845 585f 4944 203d 2022  n_id".HEX_ID = "
+00000190: 6865 785f 6964 220a 0a48 4558 5f4c 4154  hex_id"..HEX_LAT
+000001a0: 203d 2022 6865 785f 6c61 7422 0a48 4558   = "hex_lat".HEX
+000001b0: 5f4c 4f4e 203d 2022 6865 785f 6c6f 6e22  _LON = "hex_lon"
+000001c0: 0a48 4558 5f4c 4f43 4154 494f 4e20 3d20  .HEX_LOCATION = 
+000001d0: 2268 6578 5f6c 6f63 6174 696f 6e22 0a0a  "hex_location"..
+000001e0: 494e 4445 5820 3d20 2269 6e64 6578 220a  INDEX = "index".
+000001f0: 4c41 5449 5455 4445 203d 2022 6c61 7469  LATITUDE = "lati
+00000200: 7475 6465 220a 4c4f 4e47 4954 5544 4520  tude".LONGITUDE 
+00000210: 3d20 226c 6f6e 6769 7475 6465 220a 0a4f  = "longitude"..O
+00000220: 5054 494d 414c 5f44 4154 415f 434f 4c55  PTIMAL_DATA_COLU
+00000230: 4d4e 203d 2022 6f70 7469 6d61 6c5f 6461  MN = "optimal_da
+00000240: 7461 220a 5355 5050 4c59 5f44 4154 415f  ta".SUPPLY_DATA_
+00000250: 434f 4c55 4d4e 203d 2022 7375 7070 6c79  COLUMN = "supply
+00000260: 5f64 6174 6122 0a53 5550 504c 595f 4845  _data".SUPPLY_HE
+00000270: 5841 474f 4e5f 4944 203d 2022 7375 7070  XAGON_ID = "supp
+00000280: 6c79 5f68 6578 6167 6f6e 5f69 6422 0a0a  ly_hexagon_id"..
+00000290: 544f 5441 4c5f 4556 454e 5420 3d20 2274  TOTAL_EVENT = "t
+000002a0: 6f74 616c 5f65 7665 6e74 220a            otal_event".
```

### Comparing `optimal_loc-0.1.5/optimal_loc/st_app.py` & `optimal_loc-0.1.6/optimal_loc/st_app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.5/pyproject.toml` & `optimal_loc-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.5"
+version = "0.1.6"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.5/PKG-INFO` & `optimal_loc-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -81,15 +81,15 @@
 
 5. Read the distances:
    - If you have a large distance dataset, you can store it in a MongoDB database and read it using the `read_distances_from_mongodb` method.
    - Alternatively, you can directly read the distance data from a dataframe using the `read_distances` method.
 
     Example (reading from MongoDB):
     ```bash
-    sol.read_distances_from_mongodb(mongo_client=my_mongo_client("username", "password"),
+    sol.read_distances_from_mongodb(mongo_client=MongoClient,
                                     mongo_database_name="db_name",
                                     mongo_collection_name="collection_name")
     ```
 
     Example (reading from a dataframe):
     ```bash
     sol.read_distances(read_from_dataframe=True, distance_dataframe=distance_data)
```

