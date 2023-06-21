# Comparing `tmp/flatjsondict-1.0.2.tar.gz` & `tmp/flatjsondict-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.0.2.tar", max compression
+gzip compressed data, was "flatjsondict-1.0.3.tar", max compression
```

## Comparing `flatjsondict-1.0.2.tar` & `flatjsondict-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/LICENSE
--rw-r--r--   0        0        0     3087 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/README.md
--rw-r--r--   0        0        0       58 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/flatjsondict/__init__.py
--rw-r--r--   0        0        0    17234 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-21 17:53:04.277562 flatjsondict-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-21 17:53:04.277562 flatjsondict-1.0.3/README.md
+-rw-r--r--   0        0        0       58 2023-06-21 17:53:04.277562 flatjsondict-1.0.3/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    17230 2023-06-21 17:53:04.277562 flatjsondict-1.0.3/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2023-06-21 17:53:04.277562 flatjsondict-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.3/PKG-INFO
```

### Comparing `flatjsondict-1.0.2/LICENSE` & `flatjsondict-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.2/README.md` & `flatjsondict-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.2/flatjsondict/flatjsondict.py` & `flatjsondict-1.0.3/flatjsondict/flatjsondict.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
             if isinstance(self._values[key], FlatJson):
                 self._values[key].set_keyfill_value(keyfill_value)
 
     def clear(self) -> None:
         """Remove all items from the flat dictionary."""
         self._values.clear()
 
-    def copy(self) -> FlatJson:
+    def copy(self) -> Self:
         """Return a shallow copy of the flat dictionary."""
         return self.__class__(
             self._as_json(),
             self._keypath_separator,
             self._keyfill_value
         )
```

### Comparing `flatjsondict-1.0.2/pyproject.toml` & `flatjsondict-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.0.2"
+version = "1.0.3"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.0.2/PKG-INFO` & `flatjsondict-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.0.2
+Version: 1.0.3
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

