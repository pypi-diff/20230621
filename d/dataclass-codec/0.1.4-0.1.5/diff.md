# Comparing `tmp/dataclass_codec-0.1.4.tar.gz` & `tmp/dataclass_codec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.4.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.5.tar", max compression
```

## Comparing `dataclass_codec-0.1.4.tar` & `dataclass_codec-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.4/README.md
--rw-r--r--   0        0        0      600 2023-06-18 02:49:57.842218 dataclass_codec-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.4/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0     8899 2023-06-18 02:49:41.022220 dataclass_codec-0.1.4/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.4/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.4/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    14799 2023-06-18 02:43:02.922253 dataclass_codec-0.1.4/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.4/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.5/README.md
+-rw-r--r--   0        0        0      600 2023-06-21 00:14:42.815650 dataclass_codec-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.5/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0     9996 2023-06-18 02:54:59.562182 dataclass_codec-0.1.5/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.5/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.5/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    14799 2023-06-18 02:43:02.922253 dataclass_codec-0.1.5/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.5/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.5/PKG-INFO
```

### Comparing `dataclass_codec-0.1.4/pyproject.toml` & `dataclass_codec-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.4/src/dataclass_codec/decode.py` & `dataclass_codec-0.1.5/src/dataclass_codec/decode.py`

 * *Files 24% similar despite different names*

```diff
@@ -156,51 +156,66 @@
 
 
 def list_hook(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
     return [decode_it(i, _type) for i in obj]
 
 
 def dict_hook(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
-    assert isinstance(obj, dict)
+    assert isinstance(obj, dict), "{} is {} not dict".format(
+        current_path(), type(obj)
+    )
 
     def make_value(k: str) -> Any:
         with current_path_scope(current_path() + "." + k):
             return decode_it(obj[k], _type)
 
     return {k: make_value(v) for k, v in obj.items()}
 
 
 def base64_to_bytes(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
-    assert isinstance(obj, str)
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
     return base64.b64decode(obj)
 
 
 def iso_datetime_to_datetime(
     obj: Any, _type: ANYTYPE, _decode_it: DECODEIT
 ) -> Any:
-    assert isinstance(obj, str)
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
     return datetime.fromisoformat(obj)
 
 
 def iso_date_to_date(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
-    assert isinstance(obj, str)
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
     return datetime.fromisoformat(obj).date()
 
 
 def iso_time_to_time(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
-    assert isinstance(obj, str)
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
     return time.fromisoformat(obj)
 
 
 def dataclass_from_primitive_dict(
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
     cxt = decode_context()
-    assert is_dataclass_predicate(_type)
-    assert isinstance(obj, dict)
+    assert is_dataclass_predicate(_type), "{} is not a dataclass".format(
+        _type.__name__
+    )
+
+    assert isinstance(obj, dict), "{} is {} not dict".format(
+        current_path(), type(obj)
+    )
 
     def make_value(k: str) -> Any:
         with current_path_scope(current_path() + "." + k):
             if k not in obj:
                 if cxt.dataclass_unset_as_none:
                     return None
                 else:
@@ -210,40 +225,51 @@
 
     return _type(
         **{k: make_value(k) for k in _type.__dataclass_fields__.keys()}
     )
 
 
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
-    assert isinstance(obj, (str, int, float))
+    assert isinstance(
+        obj, (str, int, float)
+    ), "{} is {} not str, int or float".format(current_path(), type(obj))
     return Decimal(obj)
 
 
 def is_generic_list_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is list
 
 
 def generic_list_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
-    assert is_generic_list_predicate(_type)
-    assert isinstance(obj, list)
+    assert is_generic_list_predicate(_type), "{} is not a list".format(
+        _type.__name__
+    )
+
+    assert isinstance(obj, list), "{} is {} not list".format(
+        current_path(), type(obj)
+    )
 
     def make_value(i: int) -> Any:
         with current_path_scope(current_path() + f"[{i}]"):
             return decode_it(obj[i], _type.__args__[0])
 
     return [make_value(i) for i in range(len(obj))]
 
 
 def is_generic_dict_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is dict
 
 
 def generic_dict_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
-    assert is_generic_dict_predicate(_type)
-    assert isinstance(obj, dict)
+    assert is_generic_dict_predicate(_type), "{} is not a dict".format(
+        _type.__name__
+    )
+    assert isinstance(obj, dict), "{} is {} not dict".format(
+        current_path(), type(obj)
+    )
 
     def make_value(k: str) -> Any:
         with current_path_scope(current_path() + "." + k):
             return decode_it(obj[k], _type.__args__[1])
 
     return {k: make_value(k) for k in obj.keys()}
 
@@ -251,55 +277,63 @@
 def is_union_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is Union
 
 
 def generic_union_decoder(
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
-    assert is_union_predicate(_type)
+    assert is_union_predicate(_type), "{} is not a union".format(
+        _type.__name__
+    )
 
     obj_type = type(obj)
     allowed_types = _type.__args__
 
     if obj_type in allowed_types:
         return decode_it(obj, obj_type)
 
     raise TypeError(f"Cannot decode {obj_type} as {allowed_types}")
 
 
 def enum_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
-    assert issubclass(_type, Enum)
-    assert isinstance(obj, str)
+    assert issubclass(_type, Enum), "{} is not an enum".format(_type.__name__)
+    assert isinstance(obj, str), "{} is {} not str".format(
+        current_path(), type(obj)
+    )
 
     return _type[obj]
 
 
 def inherits_some_class_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__bases__") and len(_type.__bases__) > 0
 
 
 def generic_inheritance_decoder(
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
-    assert inherits_some_class_predicate(_type)
+    assert inherits_some_class_predicate(_type), "{} is not a class".format(
+        _type.__name__
+    )
 
     parent_types = _type.__bases__
     first_parent_type = parent_types[0]
 
     return _type(decode_it(obj, first_parent_type))
 
 
 def is_new_type_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__supertype__")
 
 
 def generic_new_type_decoder(
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
-    assert is_new_type_predicate(_type)
+    assert is_new_type_predicate(_type), "{} is not a new type".format(
+        _type.__name__
+    )
 
     type(obj)
     supertype = _type.__supertype__
 
     return _type(decode_it(obj, supertype))
```

### Comparing `dataclass_codec-0.1.4/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.5/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.4/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.1.5/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.4/PKG-INFO` & `dataclass_codec-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

