# Comparing `tmp/flatjsondict-1.0.0.tar.gz` & `tmp/flatjsondict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.0.0.tar", max compression
+gzip compressed data, was "flatjsondict-1.0.1.tar", max compression
```

## Comparing `flatjsondict-1.0.0.tar` & `flatjsondict-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2023-06-21 12:34:19.251495 flatjsondict-1.0.0/LICENSE
--rw-r--r--   0        0        0     3085 2023-06-21 12:34:19.251495 flatjsondict-1.0.0/README.md
--rw-r--r--   0        0        0       58 2023-06-21 12:34:19.252494 flatjsondict-1.0.0/flatjsondict/__init__.py
--rw-r--r--   0        0        0    17092 2023-06-21 12:34:19.252494 flatjsondict-1.0.0/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      393 2023-06-21 12:34:19.252494 flatjsondict-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 flatjsondict-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/README.md
+-rw-r--r--   0        0        0       58 2023-06-21 13:43:44.886386 flatjsondict-1.0.1/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    17093 2023-06-21 13:43:44.887386 flatjsondict-1.0.1/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2023-06-21 13:43:44.887386 flatjsondict-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.1/PKG-INFO
```

### Comparing `flatjsondict-1.0.0/LICENSE` & `flatjsondict-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.0/README.md` & `flatjsondict-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# flatjsondict: efficient JSON-like data transormation tool
+# flatjsondict: efficient JSON-like data transformation tool
 
 ## What is it?
 **flatjsondict** is nested JSON-like object transformation tool that provides 
 `FlatJson` object for flat Pandas `Series` index-like label and filesystem 
 path-like label access and manipulation for nested JSON-like data. Primarily 
-used to efficently transorm Pandas `Series` with MultiIndex index to nested 
+used to efficently transform Pandas `Series` with MultiIndex index to nested 
 JSON-like (dict, list) object and nested JSON-like data to flat Pandas 
 `Series` with MultiIndex index.
 
 Labels need to be tuples or path-like strings. The default separator for 
 path-like text labels is ``/``, but can be configured by constructor or 
 updated by calling :meth:`FlatJson.set_keypath_separator`.
```

### Comparing `flatjsondict-1.0.0/flatjsondict/flatjsondict.py` & `flatjsondict-1.0.1/flatjsondict/flatjsondict.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # FlatJson class
 
 class FlatJson(MutableMapping):
     """
 	`FlatJson` object is a flat representation of nested JSON-like data with 
 	Pandas `Series` index-like label and filesystem path-like label access and 
 	manipulation for nested JSON-like data. Primarily used to efficently 
-	transorm Pandas `Series` with MultiIndex index to nested JSON-like (dict, 
+	transform Pandas `Series` with MultiIndex index to nested JSON-like (dict, 
 	list) object and nested JSON-like data to flat Pandas `Series` with 
 	MultiIndex index.
 
 	Labels need to be tuples or path-like strings. The default separator for 
 	path-like text labels is ``/``, but can be configured by constructor or 
 	updated by calling :meth:`FlatJson.set_keypath_separator`.
```

### Comparing `flatjsondict-1.0.0/PKG-INFO` & `flatjsondict-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.0.0
-Summary: JSON-like data manipulation and transofrmation to and from nested parent-child and flat label-value data items.
+Version: 1.0.1
+Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
+Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Documentation, https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md
+Project-URL: Repository, https://gitlab.com/martins-bruvelis/flatjsondict
 Description-Content-Type: text/markdown
 
-# flatjsondict: efficient JSON-like data transormation tool
+# flatjsondict: efficient JSON-like data transformation tool
 
 ## What is it?
 **flatjsondict** is nested JSON-like object transformation tool that provides 
 `FlatJson` object for flat Pandas `Series` index-like label and filesystem 
 path-like label access and manipulation for nested JSON-like data. Primarily 
-used to efficently transorm Pandas `Series` with MultiIndex index to nested 
+used to efficently transform Pandas `Series` with MultiIndex index to nested 
 JSON-like (dict, list) object and nested JSON-like data to flat Pandas 
 `Series` with MultiIndex index.
 
 Labels need to be tuples or path-like strings. The default separator for 
 path-like text labels is ``/``, but can be configured by constructor or 
 updated by calling :meth:`FlatJson.set_keypath_separator`.
```

