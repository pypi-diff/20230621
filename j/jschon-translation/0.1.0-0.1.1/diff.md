# Comparing `tmp/jschon-translation-0.1.0.tar.gz` & `tmp/jschon-translation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschon-translation-0.1.0.tar", last modified: Tue Apr  4 10:32:45 2023, max compression
+gzip compressed data, was "jschon-translation-0.1.1.tar", last modified: Wed Jun 21 12:24:20 2023, max compression
```

## Comparing `jschon-translation-0.1.0.tar` & `jschon-translation-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.139364 jschon-translation-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-04 10:32:45.139364 jschon-translation-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.131364 jschon-translation-0.1.0/jschon_translation/
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.135364 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.127364 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.135364 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/
--rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input.json
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output.json
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.139364 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/combine-arrays.json
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/combine-objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/conditionals.json
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/multi-level-arrays.json
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/objectify-array-items.json
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/reparent-leaves.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/jschon_translation/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.131364 jschon-translation-0.1.0/jschon_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-04 10:32:45.000000 jschon-translation-0.1.0/jschon_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-04 10:32:45.000000 jschon-translation-0.1.0/jschon_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:32:45.000000 jschon-translation-0.1.0/jschon_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-04 10:32:45.000000 jschon-translation-0.1.0/jschon_translation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 10:32:45.000000 jschon-translation-0.1.0/jschon_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-04 10:32:45.143364 jschon-translation-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:32:45.139364 jschon-translation-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-04 10:32:25.000000 jschon-translation-0.1.0/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.518208 jschon-translation-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-21 12:24:20.518208 jschon-translation-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.514208 jschon-translation-0.1.1/jschon_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.514208 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.510208 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.514208 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.518208 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/combine-arrays.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/combine-objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/conditionals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/multi-level-arrays.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/objectify-array-items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/reparent-leaves.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/jschon_translation/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.514208 jschon-translation-0.1.1/jschon_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-21 12:24:20.000000 jschon-translation-0.1.1/jschon_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 12:24:20.000000 jschon-translation-0.1.1/jschon_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:24:20.000000 jschon-translation-0.1.1/jschon_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 12:24:20.000000 jschon-translation-0.1.1/jschon_translation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 12:24:20.000000 jschon-translation-0.1.1/jschon_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 12:24:20.518208 jschon-translation-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:24:20.518208 jschon-translation-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-21 12:23:59.000000 jschon-translation-0.1.1/tests/test_suite.py
```

### Comparing `jschon-translation-0.1.0/LICENSE` & `jschon-translation-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/PKG-INFO` & `jschon-translation-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jschon-translation
-Version: 0.1.0
+Version: 0.1.1
 Summary: JSON Schema-based JSON document translation
 Home-page: https://github.com/marksparkza/jschon-translation
 Author: Mark Jacobson
 Author-email: mark@saeon.ac.za
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jschon-translation-0.1.0/README.rst` & `jschon-translation-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/__init__.py` & `jschon-translation-0.1.1/jschon_translation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
-from jschon.exceptions import RelativeJSONPointerError
+from jschon.exc import RelativeJSONPointerReferenceError
 from jschon.json import JSON, JSONCompatible
 from jschon.jsonpatch import JSONPatch, JSONPatchOperation, PatchOp
 from jschon.jsonpointer import JSONPointer, RelativeJSONPointer
 from jschon.jsonschema import JSONSchema, Result
 from jschon.output import output_formatter
 
 __all__ = [
@@ -39,30 +39,30 @@
         self.t9n_leaf: bool = True
         super().__init__(*args, **kwargs)
 
     def evaluate(self, instance: JSON, result: TranslationResult = None) -> Result:
         if self.t9n_source is not None:
             try:
                 source = self.t9n_source.evaluate(instance)
-            except RelativeJSONPointerError:
+            except RelativeJSONPointerReferenceError:
                 return result
         else:
             source = instance
 
         super().evaluate(source, result)
 
         if result.valid and self.t9n_leaf:
             if self.t9n_const is not NoValue:
                 value = self.t9n_const
             elif self.t9n_concat is not None:
                 value = []
                 for item in self.t9n_concat:
                     try:
                         value += [self._make_value(item.evaluate(source))]
-                    except RelativeJSONPointerError:
+                    except RelativeJSONPointerReferenceError:
                         pass
                 if value:
                     value = self.t9n_sep.join(str(v) for v in value)
                 else:
                     value = NoValue
             else:
                 value = self._make_value(source)
```

### Comparing `jschon-translation-0.1.0/jschon_translation/catalog.py` & `jschon-translation-0.1.1/jschon_translation/catalog.py`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input-schema.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/input.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output-schema.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/examples/iso19115-to-datacite/output.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/schema.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/schema.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/combine-arrays.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/combine-arrays.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/combine-objects.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/combine-objects.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/conditionals.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/conditionals.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/multi-level-arrays.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/multi-level-arrays.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/objectify-array-items.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/objectify-array-items.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/tests/reparent-leaves.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/tests/reparent-leaves.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/json-translation-vocabulary/vocabulary.json` & `jschon-translation-0.1.1/jschon_translation/json-translation-vocabulary/vocabulary.json`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/jschon_translation/vocab.py` & `jschon-translation-0.1.1/jschon_translation/vocab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Mapping, Optional, Sequence
 
-from jschon.exceptions import JSONSchemaError
+from jschon.exc import JSONSchemaError
 from jschon.json import JSON, JSONCompatible
 from jschon.jsonpointer import JSONPointer, RelativeJSONPointer
 from jschon.jsonschema import JSONSchema, Result
 from jschon.vocabulary import Keyword, Subschema, SubschemaMixin
 from jschon_translation import JSONTranslationSchema, TranslationResult
 
 __all__ = [
```

### Comparing `jschon-translation-0.1.0/jschon_translation.egg-info/PKG-INFO` & `jschon-translation-0.1.1/jschon_translation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jschon-translation
-Version: 0.1.0
+Version: 0.1.1
 Summary: JSON Schema-based JSON document translation
 Home-page: https://github.com/marksparkza/jschon-translation
 Author: Mark Jacobson
 Author-email: mark@saeon.ac.za
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jschon-translation-0.1.0/jschon_translation.egg-info/SOURCES.txt` & `jschon-translation-0.1.1/jschon_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/setup.cfg` & `jschon-translation-0.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jschon-translation
-version = 0.1.0
+version = 0.1.1
 description = JSON Schema-based JSON document translation
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/marksparkza/jschon-translation
 author = Mark Jacobson
 author_email = mark@saeon.ac.za
 license = MIT
@@ -20,15 +20,15 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = ~=3.8
 install_requires = 
-	jschon
+	jschon>=0.11
 
 [options.extras_require]
 dev = 
 	pytest
 	coverage
 test = 
 	tox
```

### Comparing `jschon-translation-0.1.0/tests/test_examples.py` & `jschon-translation-0.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jschon-translation-0.1.0/tests/test_suite.py` & `jschon-translation-0.1.1/tests/test_suite.py`

 * *Files identical despite different names*

