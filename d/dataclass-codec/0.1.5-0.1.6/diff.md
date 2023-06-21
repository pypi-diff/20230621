# Comparing `tmp/dataclass_codec-0.1.5.tar.gz` & `tmp/dataclass_codec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.5.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.6.tar", max compression
```

## Comparing `dataclass_codec-0.1.5.tar` & `dataclass_codec-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.5/README.md
--rw-r--r--   0        0        0      600 2023-06-21 00:14:42.815650 dataclass_codec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.5/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0     9996 2023-06-18 02:54:59.562182 dataclass_codec-0.1.5/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.5/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.5/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    14799 2023-06-18 02:43:02.922253 dataclass_codec-0.1.5/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.5/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      101 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/README.md
+-rw-r--r--   0        0        0      600 2023-06-21 01:56:10.975311 dataclass_codec-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.6/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    10238 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.6/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    16060 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.6/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.1.6/PKG-INFO
```

### Comparing `dataclass_codec-0.1.5/pyproject.toml` & `dataclass_codec-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.5/src/dataclass_codec/decode.py` & `dataclass_codec-0.1.6/src/dataclass_codec/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
+from uuid import UUID
 
 from dataclass_codec.types_predicates import (
     is_dataclass_predicate,
     is_enum_predicate,
 )
 
 
@@ -230,14 +231,19 @@
 
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
     assert isinstance(
         obj, (str, int, float)
     ), "{} is {} not str, int or float".format(current_path(), type(obj))
     return Decimal(obj)
 
+def uuid_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
+    assert isinstance(
+        obj, str
+    ), "{} is {} not str".format(current_path(), type(obj))
+    return UUID(obj)
 
 def is_generic_list_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is list
 
 
 def generic_list_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
     assert is_generic_list_predicate(_type), "{} is not a list".format(
@@ -351,14 +357,15 @@
     list: list_hook,
     dict: dict_hook,
     bytes: base64_to_bytes,
     datetime: iso_datetime_to_datetime,
     date: iso_date_to_date,
     time: iso_time_to_time,
     Decimal: decimal_from_str,
+    UUID: uuid_from_str,
 }
 
 DEFAULT_DECODERS_BY_PREDICATE: List[Tuple[TYPEMATCHPREDICATE, TYPEDECODER]] = [
     (is_dataclass_predicate, dataclass_from_primitive_dict),
     (is_generic_list_predicate, generic_list_decoder),
     (is_generic_dict_predicate, generic_dict_decoder),
     (is_union_predicate, generic_union_decoder),
```

### Comparing `dataclass_codec-0.1.5/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.6/src/dataclass_codec/encode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Callable, Dict, Type, Tuple, List
 
+from uuid import UUID
+
 from dataclass_codec.types_predicates import (
     is_dataclass_predicate,
     is_enum_predicate,
 )
 
 
 TYPEMATCHPREDICATE = Callable[[Type[Any]], bool]
@@ -79,27 +81,33 @@
 
 
 def decimal_to_str(obj: Any, _encode_it: ENCODEIT) -> Any:
     assert isinstance(obj, Decimal)
     return str(obj)
 
 
+def uuid_to_str(obj: Any, _encode_it: ENCODEIT) -> Any:
+    assert isinstance(obj, UUID), f"Expected UUID, got {type(obj)}"
+    return str(obj)
+
+
 def encode(obj: Any) -> Any:
     return raw_encode(
         obj,
         {
             **{t: primitive_hook(t) for t in [bool, int, float, str]},
             type(None): lambda obj, _: None,
             list: list_hook,
             tuple: list_hook,
             dict: dict_hook,
             bytes: bytes_to_base64,
             datetime: datetime_to_iso,
             date: datetime_to_iso,
             time: datetime_to_iso,
             Decimal: decimal_to_str,
+            UUID: uuid_to_str,
         },
         [
             (is_dataclass_predicate, dataclass_to_primitive_dict),
             (is_enum_predicate, enum_to_primitive),
         ],
     )
```

### Comparing `dataclass_codec-0.1.5/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.1.6/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 8% similar despite different names*

```diff
@@ -534,7 +534,54 @@
     "access_list": null,
     "use_default_location": true,
     "ipv6": true
 }"""
         )
 
         decode(json_data, ProxyHostAddResponse)
+
+    def test_encode_uuid(self) -> None:
+        import uuid
+
+        assert (
+            encode(uuid.UUID("12345678-1234-5678-1234-567812345678"))
+            == "12345678-1234-5678-1234-567812345678"
+        )
+
+    def test_decode_uuid(self) -> None:
+        import uuid
+
+        @dataclass
+        class Dummy:
+            uuid_: uuid.UUID
+
+        assert decode(
+            {"uuid_": "12345678-1234-5678-1234-567812345678"}, Dummy
+        ) == Dummy(uuid.UUID("12345678-1234-5678-1234-567812345678"))
+
+    def test_decode_uuid_with_invalid_value(self) -> None:
+        import uuid
+
+        @dataclass
+        class Dummy:
+            uuid_: uuid.UUID
+
+        with pytest.raises(ValueError):
+            decode({"uuid_": "hello"}, Dummy)
+
+    def test_decode_uuid_without_dash(self) -> None:
+        import uuid
+
+        @dataclass
+        class Dummy:
+            uuid_: uuid.UUID
+
+        assert decode(
+            {"uuid_": "12345678123456781234567812345678"}, Dummy
+        ) == Dummy(uuid.UUID("12345678-1234-5678-1234-567812345678"))
+
+    def test_decode_raw_uuid(self) -> None:
+        import uuid
+
+        assert decode(
+            "12345678-1234-5678-1234-567812345678", uuid.UUID
+        ) == uuid.UUID("12345678-1234-5678-1234-567812345678")
```

### Comparing `dataclass_codec-0.1.5/PKG-INFO` & `dataclass_codec-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Dataclass Codec
 
-Serialize and deserialize dataclasses to primitive types and back.
+Serialize and deserialize dataclasses and typings to primitive types and back.
+
+
+
```

