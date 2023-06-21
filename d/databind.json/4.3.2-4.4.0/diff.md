# Comparing `tmp/databind.json-4.3.2.tar.gz` & `tmp/databind.json-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.json-4.3.2.tar", max compression
+gzip compressed data, was "databind.json-4.4.0.tar", max compression
```

## Comparing `databind.json-4.3.2.tar` & `databind.json-4.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3339 2023-06-07 22:10:11.709365 databind.json-4.3.2/README.md
--rw-r--r--   0        0        0     1563 2023-06-09 13:43:37.674709 databind.json-4.3.2/pyproject.toml
--rw-r--r--   0        0        0     2411 2023-06-09 13:43:37.674709 databind.json-4.3.2/src/databind/json/__init__.py
--rw-r--r--   0        0        0    34876 2023-06-09 13:40:15.388664 databind.json-4.3.2/src/databind/json/converters.py
--rw-r--r--   0        0        0     2706 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/py.typed
--rw-r--r--   0        0        0     1773 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/settings.py
--rw-r--r--   0        0        0    20842 2023-06-09 13:40:08.508594 databind.json-4.3.2/src/databind/json/tests/converters_test.py
--rw-r--r--   0        0        0     4246 2023-06-09 13:43:50.705751 databind.json-4.3.2/setup.py
--rw-r--r--   0        0        0     4368 2023-06-09 13:43:50.706195 databind.json-4.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3339 2023-06-10 09:03:45.388291 databind.json-4.4.0/README.md
+-rw-r--r--   0        0        0     1563 2023-06-21 15:24:21.844109 databind.json-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2411 2023-06-21 15:24:21.844214 databind.json-4.4.0/src/databind/json/__init__.py
+-rw-r--r--   0        0        0    35510 2023-06-21 15:21:57.020811 databind.json-4.4.0/src/databind/json/converters.py
+-rw-r--r--   0        0        0     2952 2023-06-21 15:21:57.021649 databind.json-4.4.0/src/databind/json/module.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:03:45.390665 databind.json-4.4.0/src/databind/json/py.typed
+-rw-r--r--   0        0        0     1933 2023-06-21 15:21:57.022393 databind.json-4.4.0/src/databind/json/settings.py
+-rw-r--r--   0        0        0    27496 2023-06-21 15:23:40.326723 databind.json-4.4.0/src/databind/json/tests/converters_test.py
+-rw-r--r--   0        0        0     4246 2023-06-21 15:24:37.886853 databind.json-4.4.0/setup.py
+-rw-r--r--   0        0        0     4368 2023-06-21 15:24:37.887170 databind.json-4.4.0/PKG-INFO
```

### Comparing `databind.json-4.3.2/README.md` & `databind.json-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `databind.json-4.3.2/pyproject.toml` & `databind.json-4.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "databind.json"
-version = "4.3.2"
+version = "4.4.0"
 description = "De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/json", from = "src"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
 Documentation = "https://niklasrosenstein.github.io/python-databind/"
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
-"databind.core" = "^4.3.2"
+"databind.core" = "^4.4.0"
 nr-date = "^2.0.0"
-typeapi = "^1.4.2"
+typeapi = "^2.0.1"
 typing-extensions = ">=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
```

### Comparing `databind.json-4.3.2/src/databind/json/__init__.py` & `databind.json-4.4.0/src/databind/json/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing as t
 
 from databind.core import ObjectMapper, Setting, Settings
 
 from databind.json.module import JsonModule
 from databind.json.settings import JsonConverter
 
-__version__ = "4.3.2"
+__version__ = "4.4.0"
 __all__ = [
     "dump",
     "dumps",
     "get_object_mapper",
     "JsonConverter",
     "JsonModule",
     "JsonType",
```

### Comparing `databind.json-4.3.2/src/databind/json/converters.py` & `databind.json-4.4.0/src/databind/json/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,21 +123,26 @@
             def _length_check() -> None:
                 if len(ctx.value) != len(datatype):
                     raise ConversionError(
                         self, ctx, f"expected a tuple of length {len(datatype)}, found {len(ctx.value)}"
                     )
 
         else:
-            # There could be no arguments to the collection type, in which case we
-            # consider Any as the item type.
-            item_types_iterator = iter(lambda: datatype[0] if datatype.args else TypeHint(t.Any), None)
-            if isinstance(datatype, TupleTypeHint):
-                python_type = tuple
-            else:
-                python_type = datatype.type
+            candidates = set()
+            for current in datatype.recurse_bases():
+                if issubclass(current.type, t.Collection) and len(current.args) == 1:
+                    candidates.add(current.args[0])
+            if len(candidates) == 0:
+                raise ConversionError(self, ctx, f"could not find item type in {datatype}")
+            elif len(candidates) > 1:
+                raise ConversionError(self, ctx, f"found multiple item types in {datatype}: {candidates}")
+
+            item_type = TypeHint(next(iter(candidates)))
+            item_types_iterator = iter(lambda: item_type, None)
+            python_type = datatype.type
 
             def _length_check() -> None:
                 pass
 
         values: t.Iterable[t.Any] = (
             ctx.spawn(val, item_type, idx).convert()
             for idx, (val, item_type) in enumerate(zip(ctx.value, item_types_iterator))
@@ -313,21 +318,28 @@
 
 class MappingConverter(Converter):
     def __init__(self, json_mapping_type: t.Type[t.Mapping[str, t.Any]] = dict) -> None:
         self.json_mapping_type = json_mapping_type
 
     def convert(self, ctx: Context) -> t.Any:
         datatype = _unwrap_annotated(ctx.datatype)
+
+        # Find the key and value types of the mapping.
         if not isinstance(datatype, ClassTypeHint) or not issubclass(datatype.type, t.Mapping):
             raise NotImplementedError
+        candidates = set()
+        for current in datatype.recurse_bases():
+            if issubclass(current.type, t.Mapping) and len(current.args) == 2:
+                candidates.add(current.args)
+        if len(candidates) == 0:
+            raise ConversionError(self, ctx, f"could not find key/value type in {datatype}")
+        elif len(candidates) > 1:
+            raise ConversionError(self, ctx, f"found multiple key/value types in {datatype}: {candidates}")
 
-        if not datatype.args:
-            key_type, value_type = t.Any, t.Any
-        else:
-            key_type, value_type = datatype.args
+        key_type, value_type = next(iter(candidates))
 
         if not isinstance(ctx.value, t.Mapping):
             raise ConversionError.expected(self, ctx, t.Mapping)
 
         result = {}
         for key, value in ctx.value.items():
             value = ctx.spawn(value, value_type, key).convert()
@@ -413,16 +425,15 @@
             if ctx.direction == Direction.DESERIALIZE
             else Strict(True)
         )
         adapters = self._strict_adapters if strict.enabled else self._nonstrict_adapters
         adapter = adapters.get((source_type, target_type))
 
         if adapter is None:
-            msg = f"unable to {ctx.direction.name.lower()} {source_type.__name__} -> {target_type.__name__}"
-            raise ConversionError(self, ctx, msg)
+            raise ConversionError.expected(self, ctx, target_type, source_type)
 
         try:
             return adapter(ctx.value)
         except ValueError as exc:
             raise ConversionError(self, ctx, str(exc)) from exc
```

### Comparing `databind.json-4.3.2/src/databind/json/module.py` & `databind.json-4.4.0/src/databind/json/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,12 +51,23 @@
         #       substition principle (otherwise you would end up deserializing a `Path` field as a `PurePath` but
         #       then actually serialize it as a `Path` which causes an error, "expected Path, got PurePath").
         self.register(StringifyConverter(pathlib.PurePath, name="JsonModule:pathlib.PurePath"), first=True)
         self.register(StringifyConverter(pathlib.Path, name="JsonModule:pathlib.Path"), first=True)
         self.register(StringifyConverter(duration, duration.parse, name="JsonModule:nr.date.duration"), first=True)
         self.register(LiteralConverter())
 
+        self.register(JsonConverterSupport(), first=True)
+
+
+class JsonConverterSupport(Module):
+    """
+    Handles the JsonConverter setting.
+    """
+
+    def __init__(self) -> None:
+        super().__init__(__name__ + ".JsonConverterSupport")
+
     def get_converters(self, ctx: Context) -> Iterator[Converter]:
         converter_setting = ctx.get_setting(JsonConverter)
         if converter_setting is not None:
             yield converter_setting.supplier()
         yield from super().get_converters(ctx)
```

### Comparing `databind.json-4.3.2/src/databind/json/settings.py` & `databind.json-4.4.0/src/databind/json/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,9 +52,16 @@
         super().__init__()
         if isinstance(supplier, Converter):
             self.supplier = lambda: supplier
         else:
             self.supplier = supplier
 
     @staticmethod
-    def using_classmethods(*, serialize: "str | None" = None, deserialize: "str | None" = None) -> "JsonConverter":
-        return JsonConverter(DelegateToClassmethodConverter(serialize=serialize, deserialize=deserialize))
+    def using_classmethods(
+        serialized_type: t.Union[t.Type[t.Any], t.Tuple[t.Type[t.Any], ...], None] = None,
+        *,
+        serialize: "str | None" = None,
+        deserialize: "str | None" = None
+    ) -> "JsonConverter":
+        return JsonConverter(
+            DelegateToClassmethodConverter(serialized_type, serialize=serialize, deserialize=deserialize)
+        )
```

### Comparing `databind.json-4.3.2/setup.py` & `databind.json-4.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['json', 'json.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['databind.core>=4.3.2,<5.0.0',
+['databind.core>=4.4.0,<5.0.0',
  'nr-date>=2.0.0,<3.0.0',
- 'typeapi>=1.4.2,<2.0.0',
+ 'typeapi>=2.0.1,<3.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.json',
-    'version': '4.3.2',
+    'version': '4.4.0',
     'description': 'De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.json\n\nThe `databind.json` package implements the de-/serialization to or from JSON payloads using\nthe `databind.core` framework.\n\nCheck out the [Documentation][0] for examples.\n\n[0]: https://niklasrosenstein.github.io/python-databind/\n\n## Built-in converters\n\nThe following tables shows which types can be deserialized from / serialize to Python types with the native\nconverters provided by the `databind.json` module:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `AnyConverter` | `typing.Any` | Accept any value (useful for arbitrary JSON). |\n| `CollectionConverter` | `typing.Collection[T]`, excl. `str`, `bytes`, `bytearray`, `memoryview` and `typing.Mapping[K, V]` | Converts between native Python collections and JSON arrays. |\n| `DatetimeConverter` | `datetime.date`, `datetime.datetime`, `datetime.time` | Converts between strings and date/time formats, using ISO 8601 time format by default (can be changed with the `databind.core.settings.DateFormat` setting). |\n| `DecimalConverter` | `decimal.Decimal` | Converts between strings (and ints/floats if strict mode is off, strict mode is on by default) and decimals. The precision can be controlled with the `databind.core.settings.Precision` setting. |\n| `EnumConverter` | `enum.Enum`, `enum.IntEnum` | Convert between strings and Python enumerations. The serialized form of `IntEnum` is the integer value, whereas the serialized form of `Enum` is a string (name of the enumeration value). |\n| `MappingConverter` | `typing.Mapping[K, V]` | Converts between Python dicts and JSON objects. (While in theory `K` can be any type, for JSON `K` always needs to be `str`). |\n| `OptionalConverter` | `typing.Optional[T]` | Handles optional fields in a schema. |\n| `PlainDatatypeConverter` | `bytes`, `str`, `int`, `float`, `bool` | Converts between plain datatypes. In non-strict mode (off by default), numeric types will also accept strings as input for the deserialization. |\n| `SchemaConverter` | `dataclasses.dataclass`, `typing.TypedDict` | Converts between Python dataclasses or typed dictionary and JSON objects. |\n| `UnionConverter` | `typing.Union[...]` | Handles union types. Unions in JSON can be expressed in a multitide of ways, e.g. using a discriminator key and flat, keyed or nested structure or "best match". Check out the examples section of the documentation for more information. |\n| `LiteralConverter` | `typing.Literal[...]` | Accepts or rejects a value based on whether it matches one of the values in the literal type hint. |\n\n\nThe following converters are provided for convenience:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `StringifyConverter` | n/a | A helper that allows to easily create de/serializers from a "to string" and "from string" function. |\n\nThe following additional types are natively supported by `databind.json` using `StringifyConverter`:\n\n| Types | Description |\n| ----- | ----------- |\n| `uuid.UUID` | Convert between strings and UUIDs. |\n| `pathlib.Path` | Convert between strings and paths. |\n| `pathlib.PurePath` | Convert between strings and paths. |\n| `nr.date.duration` | Deserialize from ISO 8601 duration strings or the object form, serialize to ISO 8601 strings. |\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.json-4.3.2/PKG-INFO` & `databind.json-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: databind.json
-Version: 4.3.2
+Version: 4.4.0
 Summary: De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.3.2,<5.0.0)
+Requires-Dist: databind.core (>=4.4.0,<5.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
-Requires-Dist: typeapi (>=1.4.2,<2.0.0)
+Requires-Dist: typeapi (>=2.0.1,<3.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
 
 # databind.json
```

