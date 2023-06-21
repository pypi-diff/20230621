# Comparing `tmp/flatjsondict-1.0.1.tar.gz` & `tmp/flatjsondict-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.0.1.tar", max compression
+gzip compressed data, was "flatjsondict-1.0.2.tar", max compression
```

## Comparing `flatjsondict-1.0.1.tar` & `flatjsondict-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/LICENSE
--rw-r--r--   0        0        0     3087 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/README.md
--rw-r--r--   0        0        0       58 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/flatjsondict/__init__.py
--rw-r--r--   0        0        0    17093 2023-06-21 13:43:44.887386 flatjsondict-1.0.1/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2023-06-21 13:43:44.887386 flatjsondict-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/README.md
+-rw-r--r--   0        0        0       58 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    17234 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2023-06-21 17:27:10.285890 flatjsondict-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.2/PKG-INFO
```

### Comparing `flatjsondict-1.0.1/LICENSE` & `flatjsondict-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.1/README.md` & `flatjsondict-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.1/flatjsondict/flatjsondict.py` & `flatjsondict-1.0.2/flatjsondict/flatjsondict.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 logger = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------
 # FlatJson class
 
 class FlatJson(MutableMapping):
     """
-	`FlatJson` object is a flat representation of nested JSON-like data with 
-	Pandas `Series` index-like label and filesystem path-like label access and 
-	manipulation for nested JSON-like data. Primarily used to efficently 
-	transform Pandas `Series` with MultiIndex index to nested JSON-like (dict, 
-	list) object and nested JSON-like data to flat Pandas `Series` with 
-	MultiIndex index.
-
-	Labels need to be tuples or path-like strings. The default separator for 
-	path-like text labels is ``/``, but can be configured by constructor or 
-	updated by calling :meth:`FlatJson.set_keypath_separator`.
-
-	Note that `FlatJson` provides :meth:`FlatJson.to_series()` to prepare 
-	JSON-like data for efficiently creating Pandas `Series` object with data 
-	MultiIndex index allowing to efficiently transform nested JSON-like object 
-	to Pandas `Series`.
-
-	Note that `FlatJson` provides :meth:`FlatJson.to_json()` to efficiently 
-	create nested JSON-like object from flat tuple-like label dictionary. 
-	Alternatively, `FlatJson` can be used as the target dictionary-like class when 
-	calling `Series.to_dict(FlatJson)`, then `FlatJson.to_json()` can be called 
-	to return nested json-like data for use with JSON:API applications.
+    `FlatJson` object is a flat representation of nested JSON-like data with 
+    Pandas `Series` index-like label and filesystem path-like label access and 
+    manipulation for nested JSON-like data. Primarily used to efficently 
+    transform Pandas `Series` with MultiIndex index to nested JSON-like (dict, 
+    list) object and nested JSON-like data to flat Pandas `Series` with 
+    MultiIndex index.
+
+    Labels need to be tuples or path-like strings. The default separator for 
+    path-like text labels is ``/``, but can be configured by constructor or 
+    updated by calling :meth:`FlatJson.set_keypath_separator`.
+
+    Note that `FlatJson` provides :meth:`FlatJson.to_series()` to prepare 
+    JSON-like data for efficiently creating Pandas `Series` object with data 
+    MultiIndex index allowing to efficiently transform nested JSON-like object 
+    to Pandas `Series`.
+
+    Note that `FlatJson` provides :meth:`FlatJson.to_json()` to efficiently 
+    create nested JSON-like object from flat tuple-like label dictionary. 
+    Alternatively, `FlatJson` can be used as the target dictionary-like class when 
+    calling `Series.to_dict(FlatJson)`, then `FlatJson.to_json()` can be called 
+    to return nested json-like data for use with JSON:API applications.
 
     Parameters
     ----------
     data : json-like nested iterable, dict, or list
         Contains json-like data objects stored in `FlatJson`.
     keypath_separator : str, default ``/``
         Path-like separator for 
@@ -104,26 +104,26 @@
 
     def __init__(
         self,
         data = None,
         keypath_separator: str = '/',
         keyfill_value: object = ''
     ) -> None:
-    	logger.debug('original data type: %s', type(data))
+        logger.debug('original data type: %s', type(data))
         self.original_type = type(data)
         if self.original_type in self._ARRAYS:
             data = {i: value for i, value in enumerate(data)}
         elif self.original_type in (dict,):
             data = self.__parse_dict(data, keyfill_value = keyfill_value)
         else:
             self.original_type = dict
-    		logger.debug(
-    			'Setting self.original_type data type to %s '\
-    			'for source data type %s', self.original_type, type(data)
-			)
+            logger.debug(
+                'Setting self.original_type data type to %s '\
+                'for source data type %s', self.original_type, type(data)
+            )
         super().__init__()
         self._keypath_separator = keypath_separator
         self._keyfill_value = keyfill_value
         self._values = dict()
         self.__update(data)
 
     def __contains__(self, key) -> bool:
@@ -249,20 +249,20 @@
         Parameters
         ----------
         data : dict, list or json-like
             Data used to populate the new `FlatJson`.
 
         """
         if isinstance(data, (Generator, zip)):
-    		logger.debug(
-    			'Converting %s type data source to dictionary and '\
-    			'deriving FlatJson with self.original_type set to %s',
-    			type(data),
-    			self.original_type
-			)
+            logger.debug(
+                'Converting %s type data source to dictionary and '\
+                'deriving FlatJson with self.original_type set to %s',
+                type(data),
+                self.original_type
+            )
             [
                 self.__setitem__(k, v)
                  for k, v in 
                  self.__parse_dict(
                      dict(data),
                      keyfill_value = self._keyfill_value
                  ).items()
```

### Comparing `flatjsondict-1.0.1/pyproject.toml` & `flatjsondict-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.0.1"
+version = "1.0.2"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.0.1/PKG-INFO` & `flatjsondict-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.0.1
+Version: 1.0.2
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

