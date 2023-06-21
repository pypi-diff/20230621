# Comparing `tmp/niondata-0.15.4.tar.gz` & `tmp/niondata-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niondata-0.15.4.tar", last modified: Mon Jun 19 22:10:23 2023, max compression
+gzip compressed data, was "niondata-0.15.5.tar", last modified: Wed Jun 21 17:06:17 2023, max compression
```

## Comparing `niondata-0.15.4.tar` & `niondata-0.15.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:23.614162 niondata-0.15.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5057 2023-06-19 22:10:08.000000 niondata-0.15.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-19 22:10:08.000000 niondata-0.15.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-19 22:10:23.614162 niondata-0.15.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-19 22:10:08.000000 niondata-0.15.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:23.610162 niondata-0.15.4/nion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:23.614162 niondata-0.15.4/nion/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/Calibration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   116238 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    51832 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/DataAndMetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21750 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/Image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25288 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/MultiDimensionalProcessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/RGB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4909 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/TemplateMatching.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:23.614162 niondata-0.15.4/nion/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/Calibration_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    63748 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/Core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/ExtendedData_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/Image_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20250 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/MultiDimensionalProcessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23565 2023-06-19 22:10:08.000000 niondata-0.15.4/nion/data/xdata_1_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:10:23.614162 niondata-0.15.4/niondata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-19 22:10:23.000000 niondata-0.15.4/niondata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-19 22:10:23.000000 niondata-0.15.4/niondata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:10:23.000000 niondata-0.15.4/niondata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 22:10:23.000000 niondata-0.15.4/niondata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 22:10:23.000000 niondata-0.15.4/niondata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 22:10:08.000000 niondata-0.15.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 22:10:23.614162 niondata-0.15.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-06-19 22:10:08.000000 niondata-0.15.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:17.103253 niondata-0.15.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5158 2023-06-21 17:06:04.000000 niondata-0.15.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 17:06:04.000000 niondata-0.15.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-21 17:06:17.103253 niondata-0.15.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-21 17:06:04.000000 niondata-0.15.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:17.099253 niondata-0.15.5/nion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:17.103253 niondata-0.15.5/nion/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/Calibration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   116238 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50458 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/DataAndMetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21750 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/Image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25288 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/MultiDimensionalProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/RGB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4909 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/TemplateMatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:17.103253 niondata-0.15.5/nion/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/Calibration_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63748 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/Core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/ExtendedData_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/Image_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20250 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/MultiDimensionalProcessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23565 2023-06-21 17:06:04.000000 niondata-0.15.5/nion/data/xdata_1_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:06:17.103253 niondata-0.15.5/niondata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-21 17:06:17.000000 niondata-0.15.5/niondata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-21 17:06:17.000000 niondata-0.15.5/niondata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:06:17.000000 niondata-0.15.5/niondata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 17:06:17.000000 niondata-0.15.5/niondata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 17:06:17.000000 niondata-0.15.5/niondata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 17:06:04.000000 niondata-0.15.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 17:06:17.107253 niondata-0.15.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-06-21 17:06:04.000000 niondata-0.15.5/setup.py
```

### Comparing `niondata-0.15.4/CHANGES.rst` & `niondata-0.15.5/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog (niondata)
 ====================
 
+0.15.5 (2023-06-21)
+-------------------
+- Revert breaking change: DataMetadata read-only accessors.
+
 0.15.4 (2023-06-19)
 -------------------
 - Introduce rebin_factor xdata function.
 - Carry through intensity calibration during FFT/IFFT.
 - Add copy magic method to data metadata.
 - Make read-only accessors to all DataMetadata properties instead of having them be read/write.
 - Require Python 3.9 or higher.
```

### Comparing `niondata-0.15.4/LICENSE.txt` & `niondata-0.15.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/PKG-INFO` & `niondata-0.15.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niondata
-Version: 0.15.4
+Version: 0.15.5
 Summary: A data processing library for Nion Swift.
 Home-page: https://github.com/nion-software/niondata
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,14 +46,18 @@
 ----------------
 
 - `Changelog <https://github.com/nion-software/niondata/blob/master/CHANGES.rst>`_
 
 Changelog (niondata)
 ====================
 
+0.15.5 (2023-06-21)
+-------------------
+- Revert breaking change: DataMetadata read-only accessors.
+
 0.15.4 (2023-06-19)
 -------------------
 - Introduce rebin_factor xdata function.
 - Carry through intensity calibration during FFT/IFFT.
 - Add copy magic method to data metadata.
 - Make read-only accessors to all DataMetadata properties instead of having them be read/write.
 - Require Python 3.9 or higher.
```

### Comparing `niondata-0.15.4/README.rst` & `niondata-0.15.5/README.rst`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/Calibration.py` & `niondata-0.15.5/nion/data/Calibration.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/Core.py` & `niondata-0.15.5/nion/data/Core.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/DataAndMetadata.py` & `niondata-0.15.5/nion/data/DataAndMetadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
+from __future__ import annotations
+
 # standard libraries
 import copy
 import datetime
 import gettext
 import logging
 import numbers
+import pickle
+import re
 import threading
 import typing
 import warnings
 
 import numpy
 import numpy.typing
 
@@ -124,16 +128,15 @@
                  metadata: typing.Optional[MetadataType] = None,
                  timestamp: typing.Optional[datetime.datetime] = None,
                  data_descriptor: typing.Optional[DataDescriptor] = None,
                  timezone: typing.Optional[str] = None,
                  timezone_offset: typing.Optional[str] = None):
         if data_shape_and_dtype is not None and data_shape_and_dtype[0] is not None and not all([type(data_shape_item) == int for data_shape_item in data_shape_and_dtype[0]]):
             warnings.warn('using a non-integer shape in DataAndMetadata', DeprecationWarning, stacklevel=2)
-
-        self.__data_shape_and_dtype = (tuple(data_shape_and_dtype[0]), typing.cast(numpy.typing.DTypeLike, numpy.dtype(data_shape_and_dtype[1]))) if data_shape_and_dtype is not None else None
+        self.data_shape_and_dtype = (tuple(data_shape_and_dtype[0]), numpy.dtype(data_shape_and_dtype[1])) if data_shape_and_dtype is not None else None
 
         dimensional_shape: typing.List[int] = list()
         if data_shape_and_dtype is not None:
             ds = Image.dimensional_shape_from_shape_and_dtype(data_shape_and_dtype[0], data_shape_and_dtype[1])
             assert ds is not None
             dimensional_shape = list(ds)
         dimension_count = len(dimensional_shape) if dimensional_shape else 0
@@ -144,26 +147,26 @@
             datum_dimension_count = dimension_count - collection_dimension_count
             data_descriptor = DataDescriptor(is_sequence, collection_dimension_count, datum_dimension_count)
 
         assert data_descriptor.expected_dimension_count == dimension_count
         assert timezone is None or timezone
         assert timezone_offset is None or timezone_offset
 
-        self.__data_descriptor = data_descriptor
+        self.data_descriptor = data_descriptor
 
-        self.__intensity_calibration: Calibration.Calibration = copy.deepcopy(intensity_calibration) if intensity_calibration else Calibration.Calibration()
+        self.intensity_calibration: Calibration.Calibration = copy.deepcopy(intensity_calibration) if intensity_calibration else Calibration.Calibration()
         if dimensional_calibrations is None:
             dimensional_calibrations = list()
             for _ in dimensional_shape:
                 dimensional_calibrations.append(Calibration.Calibration())
-        self.__dimensional_calibrations = copy.deepcopy(dimensional_calibrations)
-        self.__timestamp = timestamp if timestamp else DateTime.utcnow()
-        self.__timezone = timezone
-        self.__timezone_offset = timezone_offset
-        self.__metadata = copy.deepcopy(dict(metadata)) if metadata is not None else dict()
+        self.dimensional_calibrations = copy.deepcopy(dimensional_calibrations)
+        self.timestamp = timestamp if timestamp else DateTime.utcnow()
+        self.timezone = timezone
+        self.timezone_offset = timezone_offset
+        self.metadata = copy.deepcopy(dict(metadata)) if metadata is not None else dict()
 
         assert isinstance(self.metadata, dict)
         assert len(dimensional_calibrations) == len(dimensional_shape)
 
     def __eq__(self, other: typing.Any) -> bool:
         if not isinstance(other, self.__class__):
             return False
@@ -184,56 +187,24 @@
         return True
 
     def __deepcopy__(self, memo: typing.Dict[typing.Any, typing.Any]) -> DataMetadata:
         return DataMetadata(self.data_shape_and_dtype, self.intensity_calibration, self.dimensional_calibrations,
                             self.metadata, self.timestamp, self.data_descriptor, self.timezone, self.timezone_offset)
 
     @property
-    def data_shape_and_dtype(self) -> typing.Optional[typing.Tuple[ShapeType, numpy.typing.DTypeLike]]:
-        return self.__data_shape_and_dtype
-
-    @property
     def data_shape(self) -> ShapeType:
         data_shape_and_dtype = self.data_shape_and_dtype
         return tuple(data_shape_and_dtype[0]) if data_shape_and_dtype is not None else tuple()
 
     @property
     def data_dtype(self) -> typing.Optional[numpy.typing.DTypeLike]:
         data_shape_and_dtype = self.data_shape_and_dtype
         return data_shape_and_dtype[1] if data_shape_and_dtype is not None else None
 
     @property
-    def data_descriptor(self) -> DataDescriptor:
-        return self.__data_descriptor
-
-    @property
-    def intensity_calibration(self) -> Calibration.Calibration:
-        return copy.deepcopy(self.__intensity_calibration)
-
-    @property
-    def dimensional_calibrations(self) -> CalibrationListType:
-        return self.__dimensional_calibrations
-
-    @property
-    def timestamp(self) -> datetime.datetime:
-        return self.__timestamp
-
-    @property
-    def timezone(self) -> typing.Optional[str]:
-        return self.__timezone
-
-    @property
-    def timezone_offset(self) -> typing.Optional[str]:
-        return self.__timezone_offset
-
-    @property
-    def metadata(self) -> MetadataType:
-        return copy.deepcopy(self.__metadata)
-
-    @property
     def dimensional_shape(self) -> ShapeType:
         data_shape_and_dtype = self.data_shape_and_dtype
         if data_shape_and_dtype is not None:
             data_shape, data_dtype = data_shape_and_dtype
             shape = Image.dimensional_shape_from_shape_and_dtype(data_shape, data_dtype)
             return tuple(shape) if shape is not None else tuple()
         return tuple()
@@ -344,38 +315,29 @@
 
     def get_intensity_calibration(self) -> Calibration.Calibration:
         return self.intensity_calibration
 
     def get_dimensional_calibration(self, index: int) -> Calibration.Calibration:
         return self.dimensional_calibrations[index]
 
-    def _set_data_shape_and_dtype(self, data_shape_and_dtype: typing.Optional[typing.Tuple[ShapeType, numpy.typing.DTypeLike]]) -> None:
-        self.__data_shape_and_dtype = data_shape_and_dtype
-
     def _set_intensity_calibration(self, intensity_calibration: Calibration.Calibration) -> None:
-        self.__intensity_calibration = copy.deepcopy(intensity_calibration)
+        self.intensity_calibration = copy.deepcopy(intensity_calibration)
 
     def _set_dimensional_calibrations(self, dimensional_calibrations: CalibrationListType) -> None:
         assert len(dimensional_calibrations) == len(self.dimensional_shape)
-        self.__dimensional_calibrations = copy.deepcopy(dimensional_calibrations)
+        self.dimensional_calibrations = copy.deepcopy(dimensional_calibrations)
 
     def _set_data_descriptor(self, data_descriptor: DataDescriptor) -> None:
-        self.__data_descriptor = copy.deepcopy(data_descriptor)
+        self.data_descriptor = copy.deepcopy(data_descriptor)
 
     def _set_metadata(self, metadata: MetadataType) -> None:
-        self.__metadata = copy.deepcopy(dict(metadata))
+        self.metadata = copy.deepcopy(dict(metadata))
 
     def _set_timestamp(self, timestamp: datetime.datetime) -> None:
-        self.__timestamp = timestamp
-
-    def _set_timezone(self, timezone: typing.Optional[str]) -> None:
-        self.__timezone = timezone
-
-    def _set_timezone_offset(self, timezone_offset: typing.Optional[str]) -> None:
-        self.__timezone_offset = timezone_offset
+        self.timestamp = timestamp
 
     @property
     def is_data_1d(self) -> bool:
         data_shape_and_dtype = self.data_shape_and_dtype
         return Image.is_shape_and_dtype_1d(*data_shape_and_dtype) if data_shape_and_dtype else False
 
     @property
@@ -712,31 +674,31 @@
 
     @property
     def timestamp(self) -> datetime.datetime:
         return self.__data_metadata.timestamp
 
     @timestamp.setter
     def timestamp(self, value: datetime.datetime) -> None:
-        self.__data_metadata._set_timestamp(value)
+        self.__data_metadata.timestamp = value
 
     @property
     def timezone(self) -> typing.Optional[str]:
         return self.__data_metadata.timezone
 
     @timezone.setter
     def timezone(self, value: str) -> None:
-        self.__data_metadata._set_timezone(value)
+        self.__data_metadata.timezone = value
 
     @property
     def timezone_offset(self) -> typing.Optional[str]:
         return self.__data_metadata.timezone_offset
 
     @timezone_offset.setter
     def timezone_offset(self, value: str) -> None:
-        self.__data_metadata._set_timezone_offset(value)
+        self.__data_metadata.timezone_offset = value
 
     @property
     def is_data_1d(self) -> bool:
         return self.__data_metadata.is_data_1d
 
     @property
     def is_data_2d(self) -> bool:
```

### Comparing `niondata-0.15.4/nion/data/Image.py` & `niondata-0.15.5/nion/data/Image.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/MultiDimensionalProcessing.py` & `niondata-0.15.5/nion/data/MultiDimensionalProcessing.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/RGB.py` & `niondata-0.15.5/nion/data/RGB.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/TemplateMatching.py` & `niondata-0.15.5/nion/data/TemplateMatching.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/test/Calibration_test.py` & `niondata-0.15.5/nion/data/test/Calibration_test.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/test/Core_test.py` & `niondata-0.15.5/nion/data/test/Core_test.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/test/ExtendedData_test.py` & `niondata-0.15.5/nion/data/test/ExtendedData_test.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/test/Image_test.py` & `niondata-0.15.5/nion/data/test/Image_test.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/test/MultiDimensionalProcessing_test.py` & `niondata-0.15.5/nion/data/test/MultiDimensionalProcessing_test.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/nion/data/xdata_1_0.py` & `niondata-0.15.5/nion/data/xdata_1_0.py`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/niondata.egg-info/PKG-INFO` & `niondata-0.15.5/niondata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niondata
-Version: 0.15.4
+Version: 0.15.5
 Summary: A data processing library for Nion Swift.
 Home-page: https://github.com/nion-software/niondata
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,14 +46,18 @@
 ----------------
 
 - `Changelog <https://github.com/nion-software/niondata/blob/master/CHANGES.rst>`_
 
 Changelog (niondata)
 ====================
 
+0.15.5 (2023-06-21)
+-------------------
+- Revert breaking change: DataMetadata read-only accessors.
+
 0.15.4 (2023-06-19)
 -------------------
 - Introduce rebin_factor xdata function.
 - Carry through intensity calibration during FFT/IFFT.
 - Add copy magic method to data metadata.
 - Make read-only accessors to all DataMetadata properties instead of having them be read/write.
 - Require Python 3.9 or higher.
```

### Comparing `niondata-0.15.4/niondata.egg-info/SOURCES.txt` & `niondata-0.15.5/niondata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niondata-0.15.4/setup.cfg` & `niondata-0.15.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = niondata
-version = 0.15.4
+version = 0.15.5
 author = Nion Software
 author_email = swift@nion.com
 description = A data processing library for Nion Swift.
 long_description = file: README.rst, CHANGES.rst, LICENSE.rst
 url = https://github.com/nion-software/niondata
 license = Apache-2.0
 classifiers =
```

