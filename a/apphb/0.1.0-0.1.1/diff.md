# Comparing `tmp/apphb-0.1.0.tar.gz` & `tmp/apphb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cimes/apphb-python/dist/tmps5kf66_n/apphb-0.1.0.tar", last modified: Wed Dec 15 16:13:38 2021, max compression
+gzip compressed data, was "apphb-0.1.1.tar", last modified: Wed Jun 21 14:09:24 2023, max compression
```

## Comparing `apphb-0.1.0.tar` & `apphb-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cimes      (502) staff       (20)        0 2021-12-15 16:13:38.870677 apphb-0.1.0/
--rw-r--r--   0 cimes      (502) staff       (20)     1512 2021-11-15 18:26:45.000000 apphb-0.1.0/LICENSE
--rw-r--r--   0 cimes      (502) staff       (20)     1922 2021-12-15 16:13:38.871063 apphb-0.1.0/PKG-INFO
--rw-r--r--   0 cimes      (502) staff       (20)     1537 2021-11-16 15:21:57.000000 apphb-0.1.0/README.md
-drwxr-xr-x   0 cimes      (502) staff       (20)        0 2021-12-15 16:13:38.861484 apphb-0.1.0/apphb/
--rw-r--r--   0 cimes      (502) staff       (20)    16448 2021-12-02 18:13:24.000000 apphb-0.1.0/apphb/__init__.py
--rw-r--r--   0 cimes      (502) staff       (20)     6916 2021-12-02 20:11:15.000000 apphb-0.1.0/apphb/logging.py
-drwxr-xr-x   0 cimes      (502) staff       (20)        0 2021-12-15 16:13:38.866135 apphb-0.1.0/apphb.egg-info/
--rw-r--r--   0 cimes      (502) staff       (20)     1922 2021-12-15 16:13:38.000000 apphb-0.1.0/apphb.egg-info/PKG-INFO
--rw-r--r--   0 cimes      (502) staff       (20)      254 2021-12-15 16:13:38.000000 apphb-0.1.0/apphb.egg-info/SOURCES.txt
--rw-r--r--   0 cimes      (502) staff       (20)        1 2021-12-15 16:13:38.000000 apphb-0.1.0/apphb.egg-info/dependency_links.txt
--rw-r--r--   0 cimes      (502) staff       (20)       11 2021-12-15 16:13:38.000000 apphb-0.1.0/apphb.egg-info/top_level.txt
--rw-r--r--   0 cimes      (502) staff       (20)      107 2021-11-15 18:26:45.000000 apphb-0.1.0/pyproject.toml
--rw-r--r--   0 cimes      (502) staff       (20)      475 2021-12-15 16:13:38.872785 apphb-0.1.0/setup.cfg
-drwxr-xr-x   0 cimes      (502) staff       (20)        0 2021-12-15 16:13:38.869636 apphb-0.1.0/test/
--rw-r--r--   0 cimes      (502) staff       (20)        0 2021-11-15 18:26:45.000000 apphb-0.1.0/test/__init__.py
--rw-r--r--   0 cimes      (502) staff       (20)    14096 2021-11-15 18:26:46.000000 apphb-0.1.0/test/test_heartbeat.py
--rw-r--r--   0 cimes      (502) staff       (20)     8294 2021-12-02 20:15:51.000000 apphb-0.1.0/test/test_logging.py
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-21 14:09:24.685027 apphb-0.1.1/
+-rw-r--r--   0 cimes      (501) staff       (20)     1517 2023-06-20 16:50:47.000000 apphb-0.1.1/LICENSE
+-rw-r--r--   0 cimes      (501) staff       (20)     1946 2023-06-21 14:09:24.685103 apphb-0.1.1/PKG-INFO
+-rw-r--r--   0 cimes      (501) staff       (20)     1598 2023-06-20 16:53:10.000000 apphb-0.1.1/README.md
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-21 14:09:24.682931 apphb-0.1.1/apphb/
+-rw-r--r--   0 cimes      (501) staff       (20)    16628 2022-06-30 20:39:37.000000 apphb-0.1.1/apphb/__init__.py
+-rw-r--r--   0 cimes      (501) staff       (20)     7081 2022-06-30 20:37:03.000000 apphb-0.1.1/apphb/logging.py
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-21 14:09:24.683805 apphb-0.1.1/apphb.egg-info/
+-rw-r--r--   0 cimes      (501) staff       (20)     1946 2023-06-21 14:09:24.000000 apphb-0.1.1/apphb.egg-info/PKG-INFO
+-rw-r--r--   0 cimes      (501) staff       (20)      254 2023-06-21 14:09:24.000000 apphb-0.1.1/apphb.egg-info/SOURCES.txt
+-rw-r--r--   0 cimes      (501) staff       (20)        1 2023-06-21 14:09:24.000000 apphb-0.1.1/apphb.egg-info/dependency_links.txt
+-rw-r--r--   0 cimes      (501) staff       (20)       11 2023-06-21 14:09:24.000000 apphb-0.1.1/apphb.egg-info/top_level.txt
+-rw-r--r--   0 cimes      (501) staff       (20)      107 2022-02-07 16:11:53.000000 apphb-0.1.1/pyproject.toml
+-rw-r--r--   0 cimes      (501) staff       (20)      475 2023-06-21 14:09:24.685438 apphb-0.1.1/setup.cfg
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-21 14:09:24.684664 apphb-0.1.1/test/
+-rw-r--r--   0 cimes      (501) staff       (20)        0 2022-02-07 16:11:53.000000 apphb-0.1.1/test/__init__.py
+-rw-r--r--   0 cimes      (501) staff       (20)    14096 2022-02-07 16:11:53.000000 apphb-0.1.1/test/test_heartbeat.py
+-rw-r--r--   0 cimes      (501) staff       (20)     8294 2022-02-07 16:11:53.000000 apphb-0.1.1/test/test_logging.py
```

### Comparing `apphb-0.1.0/LICENSE` & `apphb-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021, Connor Imes
+Copyright (c) 2021-2023, Connor Imes
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright
```

### Comparing `apphb-0.1.0/PKG-INFO` & `apphb-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: apphb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Application heartbeats
 Home-page: https://github.com/libheartbeats/apphb-python
 Author: Connor Imes
-License: UNKNOWN
 Keywords: heartbeats,profiling
-Platform: UNKNOWN
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Application Heartbeats
@@ -24,14 +22,20 @@
 
 The `apphb` package is published in the Python Package Index and installable with pip:
 
 ```sh
 pip install apphb
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
 
 
@@ -62,9 +66,7 @@
 
 ## Project Source
 
 Find this and related project sources at the [libheartbeats organization on GitHub](https://github.com/libheartbeats).  
 This project originates at: https://github.com/libheartbeats/apphb-python
 
 Bug reports and pull requests for bug fixes and enhancements are welcome.
-
-
```

### Comparing `apphb-0.1.0/README.md` & `apphb-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 The `apphb` package is published in the Python Package Index and installable with pip:
 
 ```sh
 pip install apphb
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
```

### Comparing `apphb-0.1.0/apphb/__init__.py` & `apphb-0.1.1/apphb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """An application-level heartbeats interface."""
 import dataclasses
 from dataclasses import dataclass
-from typing import List, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 #: Type for heartbeat field record `val` field.
 HeartbeatFieldValue = Union[Tuple[int], Tuple[float], Tuple[int, int], Tuple[float, float]]
 #: Type for heartbeat field record `glbl`, `wndw`, and `inst` fields.
 HeartbeatFieldCount = Union[int, float]
 #: Type for heartbeat field record `glbl_rate`, `wndw_rate`, and `inst_rate` fields.
 HeartbeatFieldRate = float
@@ -35,16 +35,16 @@
     wndw_rate: HeartbeatFieldRate = 0
     """The record's window rate."""
     inst_rate: HeartbeatFieldRate = 0
     """The record's instant rate."""
 
     # NOTE: using 'HeartbeatFieldRecord' as type hint b/c Python doesn't currently support forward
     #       references in type hints.
-    def copy(self, norm: HeartbeatFieldCount=None, rate_norm: HeartbeatFieldRate=None) -> \
-        'HeartbeatFieldRecord':
+    def copy(self, norm: Optional[HeartbeatFieldCount]=None,
+             rate_norm: Optional[HeartbeatFieldRate]=None) -> 'HeartbeatFieldRecord':
         """
         Create a copy, optionally by normalizing values, counts, and rates.
 
         Parameters
         ----------
         norm : HeartbeatFieldCount, optional
             The normalization factor for `val` tuple values, `glbl`, `wndw`, and `inst`.
@@ -128,15 +128,16 @@
         The only acceptable values in the tuple are ``1`` and ``2``.
         For example, if the :meth:`heartbeat` `fields` param is going to be:
         ``fields=[(total_value_1,), (start_value_2, end_value_2)]``,
         then the shape would be:
         ``fields_shape=(1, 2)``.
     """
 
-    def __init__(self, window_size: int, time_shape: int=1, fields_shape: Tuple[int, ...]=None):
+    def __init__(self, window_size: int, time_shape: int=1,
+                 fields_shape: Optional[Tuple[int, ...]]=None):
         """
         Initialize a heartbeat instance.
         """
         if window_size <= 0:
             raise ValueError('window_size must be > 0')
         if time_shape not in [1, 2]:
             raise ValueError('time_shape must be 1 or 2')
@@ -172,15 +173,15 @@
             curr_rec.inst_rate = curr_rec.inst / curr.time.inst
         # rates for the time field are a special case (heart rate), so recompute them:
         curr.time.glbl_rate = (curr.ident + 1) / curr.time.glbl
         curr.time.wndw_rate = min(curr.ident + 1, len(self._window_buffer)) / curr.time.wndw
         curr.time.inst_rate = 1 / curr.time.inst
 
     def heartbeat(self, tag: HeartbeatIdentifier, time: HeartbeatFieldValue,
-                  fields: Tuple[HeartbeatFieldValue, ...]=None):
+                  fields: Optional[Tuple[HeartbeatFieldValue, ...]]=None):
         """
         Issue a heartbeat.
 
         Parameters
         ----------
         tag : HeartbeatIdentifier
             A user-specified identifier - most likely a unique `int` value.
@@ -211,30 +212,30 @@
 
         # record the heartbeat and update state
         self._record_heartbeat(tag, time, fields)
         self._counter += 1
         self._buffer_idx = (self._buffer_idx + 1) % len(self._window_buffer)
 
     @property
-    def count(self):
+    def count(self) -> int:
         """int: The heartbeat count."""
         return self._counter
 
     @property
-    def window_size(self):
+    def window_size(self) -> int:
         """int: The window size."""
         return len(self._window_buffer)
 
     @property
-    def time_shape(self):
+    def time_shape(self) -> int:
         """int: The time shape."""
         return self._time_shape
 
     @property
-    def fields_shape(self):
+    def fields_shape(self) -> Tuple[int, ...]:
         """Tuple[int, ...]: The fields shape."""
         return self._fields_shape
 
     def _to_buffer_index(self, off):
         """
         Get the buffer index relative to current buffer pointer and offset.
         We support -window_size <= off <= 0 to be consistent with Python indexing, although
@@ -268,15 +269,15 @@
         """
         return self._window_buffer[self._to_buffer_index(off)]
 
     def _to_field_record(self, off, fld):
         hbr = self._window_buffer[self._to_buffer_index(off)]
         return hbr.time if fld is None else hbr.field_records[fld]
 
-    def get_value(self, off: int=0, fld: int=None) -> HeartbeatFieldValue:
+    def get_value(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldValue:
         """
         Get a heartbeat field value.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -289,15 +290,15 @@
         -------
         HeartbeatFieldValue
             The requested value.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.val
 
-    def get_global_count(self, off: int=0, fld: int=None) -> HeartbeatFieldCount:
+    def get_global_count(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldCount:
         """
         Get a heartbeat field global count.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -310,15 +311,15 @@
         -------
         HeartbeatFieldCount
             The requested global count.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.glbl
 
-    def get_window_count(self, off: int=0, fld: int=None) -> HeartbeatFieldCount:
+    def get_window_count(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldCount:
         """
         Get a heartbeat field window count.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -331,15 +332,15 @@
         -------
         HeartbeatFieldCount
             The requested window count.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.wndw
 
-    def get_instant_count(self, off: int=0, fld: int=None) -> HeartbeatFieldCount:
+    def get_instant_count(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldCount:
         """
         Get a heartbeat field instant count.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -352,15 +353,15 @@
         -------
         HeartbeatFieldCount
             The requested instant count.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.inst
 
-    def get_global_rate(self, off: int=0, fld: int=None) -> HeartbeatFieldRate:
+    def get_global_rate(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldRate:
         """
         Get a heartbeat field global rate.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -373,15 +374,15 @@
         -------
         HeartbeatFieldCount
             The requested global rate.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.glbl_rate
 
-    def get_window_rate(self, off: int=0, fld: int=None) -> HeartbeatFieldRate:
+    def get_window_rate(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldRate:
         """
         Get a heartbeat field window rate.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
@@ -394,15 +395,15 @@
         -------
         HeartbeatFieldCount
             The requested window rate.
         """
         hbfr = self._to_field_record(off, fld)
         return hbfr.wndw_rate
 
-    def get_instant_rate(self, off: int=0, fld: int=None) -> HeartbeatFieldRate:
+    def get_instant_rate(self, off: int=0, fld: Optional[int]=None) -> HeartbeatFieldRate:
         """
         Get a heartbeat field instant rate.
 
         Parameters
         ----------
         off : int, optional
             A negative offset relative to the last heartbeat to get older data.
```

### Comparing `apphb-0.1.0/apphb/logging.py` & `apphb-0.1.1/apphb/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Heartbeat logging utilities."""
 import dataclasses
-from typing import List
+from typing import List, Optional
 from apphb import Heartbeat, HeartbeatFieldCount, HeartbeatFieldRate, HeartbeatRecord, \
                   HeartbeatRecordData
 
 def get_log_header(hbt: Heartbeat, time_name: str='Time', heartrate_name: str='Heart Rate',
-                   field_names: List[str]=None, field_rate_names: List[str]=None) -> List[str]:
+                   field_names: Optional[List[str]]=None,
+                   field_rate_names: Optional[List[str]]=None) -> List[str]:
     """
     Get a heartbeat header for logging.
 
     The first entries are always 'Heartbeat' and 'Tag'.
     'Heartbeat' is the internal identifier.
     'Tag' is the user-specified identifier.
     Then for each field, including `time`:
@@ -57,18 +58,19 @@
         else:
             hdrs.extend(['Start ' + str(name), 'End ' + str(name)])
         for suffix in [str(name), str(name_rate)]:
             for prefix in ['Global', 'Window', 'Instant']:
                 hdrs.append(prefix + ' ' + suffix)
     return hdrs
 
-def get_log_record(hbr: HeartbeatRecord, time_norm: HeartbeatFieldCount=None,
-                   heartrate_norm: HeartbeatFieldRate=None,
-                   field_norms: List[HeartbeatFieldCount]=None,
-                   field_rate_norms: List[HeartbeatFieldRate]=None) -> List[HeartbeatRecordData]:
+def get_log_record(hbr: HeartbeatRecord, time_norm: Optional[HeartbeatFieldCount]=None,
+                   heartrate_norm: Optional[HeartbeatFieldRate]=None,
+                   field_norms: Optional[List[HeartbeatFieldCount]]=None,
+                   field_rate_norms: Optional[List[HeartbeatFieldRate]]=None) \
+    -> List[HeartbeatRecordData]:
     """
     Get a heartbeat record for logging.
 
     Parameters
     ----------
     hbr : HeartbeatRecord
         The heartbeat record to be logged.
@@ -105,18 +107,19 @@
     for rec, field_norm, field_rate_norm in zip([hbr.time] + hbr.field_records, norm, rate_norm):
         norm_rec = rec.copy(norm=field_norm, rate_norm=field_rate_norm)
         values.extend(norm_rec.val)
         values.extend(dataclasses.astuple(norm_rec)[1:])
     return values
 
 # pylint: disable=R0913
-def get_log_records(hbt: Heartbeat, count: int=None, time_norm: HeartbeatFieldCount=None,
-                    heartrate_norm: HeartbeatFieldRate=None,
-                    field_norms: List[HeartbeatFieldCount]=None,
-                    field_rate_norms: List[HeartbeatFieldRate]=None) -> \
+def get_log_records(hbt: Heartbeat, count: Optional[int]=None,
+                    time_norm: Optional[HeartbeatFieldCount]=None,
+                    heartrate_norm: Optional[HeartbeatFieldRate]=None,
+                    field_norms: Optional[List[HeartbeatFieldCount]]=None,
+                    field_rate_norms: Optional[List[HeartbeatFieldRate]]=None) -> \
     List[List[HeartbeatRecordData]]:
     """
     Get heartbeat records for logging.
 
     Parameters
     ----------
     hbt : Heartbeat
```

### Comparing `apphb-0.1.0/apphb.egg-info/PKG-INFO` & `apphb-0.1.1/apphb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: apphb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Application heartbeats
 Home-page: https://github.com/libheartbeats/apphb-python
 Author: Connor Imes
-License: UNKNOWN
 Keywords: heartbeats,profiling
-Platform: UNKNOWN
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Application Heartbeats
@@ -24,14 +22,20 @@
 
 The `apphb` package is published in the Python Package Index and installable with pip:
 
 ```sh
 pip install apphb
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
 
 
@@ -62,9 +66,7 @@
 
 ## Project Source
 
 Find this and related project sources at the [libheartbeats organization on GitHub](https://github.com/libheartbeats).  
 This project originates at: https://github.com/libheartbeats/apphb-python
 
 Bug reports and pull requests for bug fixes and enhancements are welcome.
-
-
```

### Comparing `apphb-0.1.0/test/test_heartbeat.py` & `apphb-0.1.1/test/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `apphb-0.1.0/test/test_logging.py` & `apphb-0.1.1/test/test_logging.py`

 * *Files identical despite different names*

