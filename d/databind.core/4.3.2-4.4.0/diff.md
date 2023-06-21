# Comparing `tmp/databind.core-4.3.2.tar.gz` & `tmp/databind.core-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.3.2.tar", max compression
+gzip compressed data, was "databind.core-4.4.0.tar", max compression
```

## Comparing `databind.core-4.3.2.tar` & `databind.core-4.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      337 2023-06-07 22:10:11.705365 databind.core-4.3.2/README.md
--rw-r--r--   0        0        0     1687 2023-06-09 13:43:37.674709 databind.core-4.3.2/pyproject.toml
--rw-r--r--   0        0        0     1601 2023-06-09 13:43:37.674709 databind.core-4.3.2/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/context.py
--rw-r--r--   0        0        0     6059 2023-06-09 13:06:50.872189 databind.core-4.3.2/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/py.typed
--rw-r--r--   0        0        0    15494 2023-06-07 22:10:11.705365 databind.core-4.3.2/src/databind/core/schema.py
--rw-r--r--   0        0        0    27732 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/settings.py
--rw-r--r--   0        0        0     1044 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/context_test.py
--rw-r--r--   0        0        0     1275 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_docspec_example_test.py
--rw-r--r--   0        0        0    11386 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_test.py
--rw-r--r--   0        0        0      733 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py
--rw-r--r--   0        0        0     8709 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-06-07 22:10:11.709365 databind.core-4.3.2/src/databind/core/utils.py
--rw-r--r--   0        0        0     1261 2023-06-09 13:43:49.375274 databind.core-4.3.2/setup.py
--rw-r--r--   0        0        0     1435 2023-06-09 13:43:49.375778 databind.core-4.3.2/PKG-INFO
+-rw-r--r--   0        0        0      337 2023-06-10 09:03:45.347280 databind.core-4.4.0/README.md
+-rw-r--r--   0        0        0     1687 2023-06-21 15:24:21.843680 databind.core-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1601 2023-06-21 15:24:21.843994 databind.core-4.4.0/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-06-10 09:03:45.349068 databind.core-4.4.0/src/databind/core/context.py
+-rw-r--r--   0        0        0     6703 2023-06-21 15:21:57.017985 databind.core-4.4.0/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-06-10 09:03:45.350170 databind.core-4.4.0/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-06-10 09:03:45.359491 databind.core-4.4.0/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-06-10 09:03:45.359945 databind.core-4.4.0/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:03:45.360157 databind.core-4.4.0/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15523 2023-06-10 11:23:02.604368 databind.core-4.4.0/src/databind/core/schema.py
+-rw-r--r--   0        0        0    27732 2023-06-10 09:03:45.361540 databind.core-4.4.0/src/databind/core/settings.py
+-rw-r--r--   0        0        0     1044 2023-06-10 09:03:45.362093 databind.core-4.4.0/src/databind/core/tests/context_test.py
+-rw-r--r--   0        0        0     1275 2023-06-10 09:03:45.362345 databind.core-4.4.0/src/databind/core/tests/schema_docspec_example_test.py
+-rw-r--r--   0        0        0    11386 2023-06-10 09:03:45.362600 databind.core-4.4.0/src/databind/core/tests/schema_test.py
+-rw-r--r--   0        0        0      733 2023-06-10 09:03:45.362814 databind.core-4.4.0/src/databind/core/tests/schema_with_nested_dataclasses_test.py
+-rw-r--r--   0        0        0     8709 2023-06-10 09:03:45.363059 databind.core-4.4.0/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-06-21 14:35:58.691696 databind.core-4.4.0/src/databind/core/utils.py
+-rw-r--r--   0        0        0     1261 2023-06-21 15:24:36.461306 databind.core-4.4.0/setup.py
+-rw-r--r--   0        0        0     1435 2023-06-21 15:24:36.461478 databind.core-4.4.0/PKG-INFO
```

### Comparing `databind.core-4.3.2/pyproject.toml` & `databind.core-4.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.3.2"
+version = "4.4.0"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
@@ -14,15 +14,15 @@
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
 Deprecated = "^1.2.12"
 nr-date = "^2.0.0"
 nr-stream = "^1.0.0"
-typeapi = "^1.4.2"
+typeapi = "^2.0.1"
 typing-extensions = ">=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
```

### Comparing `databind.core-4.3.2/src/databind/core/__init__.py` & `databind.core-4.4.0/src/databind/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.3.2"
+__version__ = "4.4.0"
 
 from .context import Context, Direction, Location, format_context_trace
 from .converter import ConversionError, Converter, DelegateToClassmethodConverter, Module, NoMatchingConverter
 from .mapper import ObjectMapper
 from .schema import (
     Field,
     Schema,
```

### Comparing `databind.core-4.3.2/src/databind/core/context.py` & `databind.core-4.4.0/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/converter.py` & `databind.core-4.4.0/src/databind/core/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,19 @@
         assert isinstance(converter, Converter), converter
         if first:
             self.converters.insert(0, converter)
         else:
             self.converters.append(converter)
 
     def get_converters(self, ctx: "Context") -> t.Iterator[Converter]:
-        yield from self.converters
+        for converter in self.converters:
+            if isinstance(converter, Module):
+                yield from converter.get_converters(ctx)
+            else:
+                yield converter
 
     def convert(self, ctx: "Context") -> t.Any:
         errors: t.List[t.Tuple[Converter, Exception]] = []
         for converter in self.get_converters(ctx):
             try:
                 return converter.convert(ctx)
             except NotImplementedError:
@@ -146,22 +150,33 @@
 class DelegateToClassmethodConverter(Converter):
     """
     This converter delegaes to the methods defined by name to perform serialization and deserialization of a type. This
     converter is usually used in conjunction with settings that override the converteer to be used in a specifc
     scenario (e.g. such as de/serializing JSON with the #databind.json.settings.JsonConverter setting).
     """
 
-    def __init__(self, *, serialize: "str | None" = None, deserialize: "str | None" = None) -> None:
+    def __init__(
+        self,
+        serialized_type: t.Union[t.Type[t.Any], t.Tuple[t.Type[t.Any], ...], None] = None,
+        *,
+        serialize: "str | None" = None,
+        deserialize: "str | None" = None,
+    ) -> None:
+        self._serialized_type = serialized_type
         self._serialize = serialize
         self._deserialize = deserialize
 
     def serialize(self, ctx: "Context") -> t.Any:
         if self._serialize is None or not isinstance(ctx.datatype, ClassTypeHint):
             raise NotImplementedError
+        if not isinstance(ctx.value, ctx.datatype.type):
+            raise ConversionError.expected(self, ctx, ctx.datatype.type)
         method: t.Callable[[t.Any], t.Any] = getattr(ctx.datatype.type, self._serialize)
         return method(ctx.value)
 
     def deserialize(self, ctx: "Context") -> t.Any:
         if self._deserialize is None or not isinstance(ctx.datatype, ClassTypeHint):
             raise NotImplementedError
+        if self._serialized_type is not None and not isinstance(ctx.value, self._serialized_type):
+            raise ConversionError.expected(self, ctx, self._serialized_type)
         method: t.Callable[[t.Any], t.Any] = getattr(ctx.datatype.type, self._deserialize)
         return method(ctx.value)
```

### Comparing `databind.core-4.3.2/src/databind/core/dataclasses.py` & `databind.core-4.4.0/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/dataclasses.pyi` & `databind.core-4.4.0/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/mapper.py` & `databind.core-4.4.0/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/schema.py` & `databind.core-4.4.0/src/databind/core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         else:
             # This could mean that a base class is a dataclass but all of its members
             # are overwritten by other fields.
             pass
 
         # Continue with the base classes.
         for base in hint.bases or hint.type.__bases__:
-            base_hint = TypeHint(base).parameterize(parameter_map)
+            base_hint = TypeHint(base, source=hint.type).evaluate().parameterize(parameter_map)
             assert isinstance(base_hint, ClassTypeHint), f"nani? {base_hint}"
             if dataclasses.is_dataclass(base_hint.type):
                 queue.append(base_hint)
 
     return Schema(fields, t.cast("Constructor", dataclass_type), dataclass_type)
```

### Comparing `databind.core-4.3.2/src/databind/core/settings.py` & `databind.core-4.4.0/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/tests/context_test.py` & `databind.core-4.4.0/src/databind/core/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/tests/schema_docspec_example_test.py` & `databind.core-4.4.0/src/databind/core/tests/schema_docspec_example_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/tests/schema_test.py` & `databind.core-4.4.0/src/databind/core/tests/schema_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/tests/schema_with_nested_dataclasses_test.py` & `databind.core-4.4.0/src/databind/core/tests/schema_with_nested_dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/union.py` & `databind.core-4.4.0/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/src/databind/core/utils.py` & `databind.core-4.4.0/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.3.2/setup.py` & `databind.core-4.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Deprecated>=1.2.12,<2.0.0',
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
- 'typeapi>=1.4.2,<2.0.0',
+ 'typeapi>=2.0.1,<3.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.3.2',
+    'version': '4.4.0',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# `databind.core`\n\nThis library provides the core functionality to implement serialization functions to and from Python objects, with\na great support for many features of the Python type system. A JSON implementation is provided by the `databind.json`\npackage.\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.3.2/PKG-INFO` & `databind.core-4.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.3.2
+Version: 4.4.0
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
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
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: nr-stream (>=1.0.0,<2.0.0)
-Requires-Dist: typeapi (>=1.4.2,<2.0.0)
+Requires-Dist: typeapi (>=2.0.1,<3.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
 
 # `databind.core`
```

