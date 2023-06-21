# Comparing `tmp/elias-0.2.2.tar.gz` & `tmp/elias-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-hueguy6a/elias-0.2.2.tar", last modified: Wed Jun 21 14:23:45 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-bvkk1f3m/elias-0.2.3.tar", last modified: Wed Jun 21 15:10:03 2023, max compression
```

## Comparing `elias-0.2.2.tar` & `elias-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.829326 elias-0.2.2/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 14:23:45.829326 elias-0.2.2/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.2/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.2/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-21 14:23:45.829326 elias-0.2.2/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.2/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.118004 elias-0.2.2/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.307908 elias-0.2.2/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.2/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.724000 elias-0.2.2/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.027385 elias-0.2.2/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.2/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.2/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.2/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.2/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.387624 elias-0.2.2/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.2/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.2/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.2/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.2/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:45.785415 elias-0.2.2/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.2/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.2/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.2/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.2/src/elias/util/random.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.2/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.2/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.2/src/elias/util/typing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.2/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 14:23:44.482925 elias-0.2.2/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-06-21 14:23:44.000000 elias-0.2.2/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-21 14:23:43.000000 elias-0.2.2/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.916242 elias-0.2.3/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 15:10:03.919085 elias-0.2.3/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.3/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.3/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-21 15:10:03.932315 elias-0.2.3/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.3/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.285404 elias-0.2.3/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.472916 elias-0.2.3/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    23125 2023-06-21 14:55:32.000000 elias-0.2.3/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.894836 elias-0.2.3/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.160211 elias-0.2.3/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.3/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.3/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.3/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.3/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.474347 elias-0.2.3/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.3/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.3/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.3/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.3/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:03.863406 elias-0.2.3/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.3/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.3/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.3/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.3/src/elias/util/random.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.3/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.3/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.3/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.3/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-21 15:10:02.662744 elias-0.2.3/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-06-21 15:10:02.000000 elias-0.2.3/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-21 15:10:01.000000 elias-0.2.3/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.2.2/PKG-INFO` & `elias-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.2
+Version: 0.2.3
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.2/README.md` & `elias-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/setup.cfg` & `elias-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.2.2
+version = 0.2.3
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls =
```

### Comparing `elias-0.2.2/src/elias/config.py` & `elias-0.2.3/src/elias/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, asdict, fields, field
 from enum import Enum, EnumMeta, auto
 from pydoc import locate
-from typing import List, Tuple, Any, Type, get_type_hints, Generic, TypeVar, Dict, Iterator
+from typing import List, Tuple, Any, Type, get_type_hints, Generic, TypeVar, Dict, Iterator, Callable, Optional
 
 import dacite
 import numpy as np
 from dacite import from_dict
 from dacite.dataclasses import get_fields
 from silberstral import gather_types, is_type_var_instantiated, reveal_type_var
 
@@ -246,26 +246,37 @@
                     casts.append(field_type)
         casts.append(tuple)  # Tuples are stored as [] lists in JSON. Cast them back to tuple here
 
         return casts
 
     # TODO: rename. It doesn't make sense that this method is called from_json
     @classmethod
-    def from_json(cls, json_config: dict) -> Config:
+    def from_json(cls,
+                  json_config: dict,
+                  type_hooks: Optional[Dict[Type, Callable[[Any], Any]]] = None) -> Config:
         """
         Constructs this Config dataclass from the given Python dictionary which typically will be a parsed JSON.
         As enums are not serialized in JSONs, special attention is put to such attributes.
         Any enum value that were stored as strings in the JSON file will be explicitly converted to their respective
         enum type.
 
         Parameters
         ----------
         json_config: dict
             the dictionary representing the JSON configuration. if the dictionary contains keys that don't match the
             dataclass an exception will be thrown. If you want to ignore excess items, see :meth:`from_dict`
+        type_hooks: Dict[Type, Callable[[Any], Any]]]
+            type hooks can be used to guide the deserialization process.
+            For example, a complicated data structure may be serialized as a series of lists, but in the loaded config
+            one may want to hold the data structure and not the serialized version of it.
+            In this case, a type hook defines the mapping from serialized -> data structure
+            Per-default, a type hook that maps series of lists back to numpy arrays is already added:
+            {
+                np.ndarray: lambda array_values: np.asarray(array_values)
+            }
 
         Returns
         -------
             This dataclass with all the values from :attr:`json_config` filled in. Enum attributes are explicitly
             converted.
 
         """
@@ -300,29 +311,34 @@
                 sub_class = class_mapping[abstract_dataclass_values['type']]
 
             # Delete the type attribute from the JSON input as it is implicitly defined
             del abstract_dataclass_values['type']
 
             return sub_class.from_json(abstract_dataclass_values)
 
-        type_hooks = {
+        all_type_hooks = {
             # Use Lambda closure (i=i) to ensure data_sub_class_type is copied for each lambda
             abstract_dataclass:
                 lambda abstract_dataclass_values, data_sub_class_type=data_sub_class_type:
                 instantiate_adc_with_sub_class(abstract_dataclass_values, data_sub_class_type)
             for abstract_dataclass, data_sub_class_type
             in zip(abstract_dataclasses, data_sub_class_types)}
+
         # Numpy arrays are serialized as lists. Cast them back to np array here
-        type_hooks[np.ndarray] = lambda array_values: np.asarray(array_values)
+        all_type_hooks[np.ndarray] = lambda array_values: np.asarray(array_values)
+
+        if type_hooks is not None:
+            # Add use-defined type hooks
+            all_type_hooks.update(type_hooks)
 
         # Register type hooks to replace every single AbstractDataClass with the respective subclass hinted by the
         # 'type' attribute
         dacite_config = dacite.Config(
             cast=cls._define_casts(),
-            type_hooks=type_hooks)
+            type_hooks=all_type_hooks)
 
         # backward_cls = type(cls.__name__, cls.__bases__, dict(cls.__dict__))
         #
         # def backward_compatibility_new(cls_new, *args, **kwargs):
         #     obj = super(Config, cls).__new__(cls)
         #     obj._enable_backward_compatibility = True
         #     # For some reason, __init__ isn't called anymore if __new__ is overridden. So manually call it here
```

### Comparing `elias-0.2.2/src/elias/data/combined.py` & `elias-0.2.3/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/data/loader.py` & `elias-0.2.3/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/data/sampling.py` & `elias-0.2.3/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/data/stop_criterion.py` & `elias-0.2.3/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/folder/analysis.py` & `elias-0.2.3/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/folder/data.py` & `elias-0.2.3/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/folder/folder.py` & `elias-0.2.3/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/folder/model.py` & `elias-0.2.3/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/folder/run.py` & `elias-0.2.3/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/analysis.py` & `elias-0.2.3/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/artifact.py` & `elias-0.2.3/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/buffered.py` & `elias-0.2.3/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/data.py` & `elias-0.2.3/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/model.py` & `elias-0.2.3/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/manager/run.py` & `elias-0.2.3/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/util/fs.py` & `elias-0.2.3/src/elias/util/fs.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/util/io.py` & `elias-0.2.3/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/util/range.py` & `elias-0.2.3/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/util/timing.py` & `elias-0.2.3/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias/util/version.py` & `elias-0.2.3/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.2/src/elias.egg-info/PKG-INFO` & `elias-0.2.3/src/elias.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.2
+Version: 0.2.3
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.2/src/elias.egg-info/SOURCES.txt` & `elias-0.2.3/src/elias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

