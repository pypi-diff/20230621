# Comparing `tmp/property-graph-2.0.2.tar.gz` & `tmp/property-graph-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-graph-2.0.2.tar", last modified: Wed Jun 21 19:47:36 2023, max compression
+gzip compressed data, was "property-graph-2.0.3.tar", last modified: Wed Jun 21 20:25:57 2023, max compression
```

## Comparing `property-graph-2.0.2.tar` & `property-graph-2.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.057281 property-graph-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 19:47:27.000000 property-graph-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 19:47:36.057281 property-graph-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-21 19:47:27.000000 property-graph-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 19:47:27.000000 property-graph-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:47:36.057281 property-graph-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.049281 property-graph-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.053281 property-graph-2.0.2/src/property_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 19:47:36.000000 property-graph-2.0.2/src/property_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 19:47:36.000000 property-graph-2.0.2/src/property_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:47:36.000000 property-graph-2.0.2/src/property_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 19:47:36.000000 property-graph-2.0.2/src/property_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.053281 property-graph-2.0.2/src/pypg/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/property_transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.057281 property-graph-2.0.2/src/pypg/traits/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/traits/validated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 19:47:27.000000 property-graph-2.0.2/src/pypg/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:47:36.057281 property-graph-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 19:47:27.000000 property-graph-2.0.2/tests/test_type_schema_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 20:25:45.000000 property-graph-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 20:25:57.056223 property-graph-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-21 20:25:45.000000 property-graph-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 20:25:45.000000 property-graph-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:25:57.056223 property-graph-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/property_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/pypg/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/property_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/src/pypg/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/validated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_type_schema_encoding.py
```

### Comparing `property-graph-2.0.2/LICENSE` & `property-graph-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/PKG-INFO` & `property-graph-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 2.0.2
+Version: 2.0.3
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-2.0.2/README.md` & `property-graph-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/pyproject.toml` & `property-graph-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/property_graph.egg-info/PKG-INFO` & `property-graph-2.0.3/src/property_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 2.0.2
+Version: 2.0.3
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-2.0.2/src/property_graph.egg-info/SOURCES.txt` & `property-graph-2.0.3/src/property_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/locator.py` & `property-graph-2.0.3/src/pypg/locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/property.py` & `property-graph-2.0.3/src/pypg/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,18 +325,14 @@
     @cached_property
     def value_type(self):
         return self.__orig_class__.__args__[0]
 
     def __bind__(self, name, cls: PropertyType):
         self.name = name
         self.__declaring_type = cls
-        self._default, self._getter, self._setter = (
-            MethodReference(obj) if is_method(cls, obj) else obj
-            for obj in (self._default, self._getter, self._setter)
-        )
 
     def __bind_subclass__(self, cls):
         proxy = _Proxy(self, cls)
         for t in proxy.traits:
             t.__bind__(self)
         self._subclass_proxies[cls] = proxy
```

### Comparing `property-graph-2.0.2/src/pypg/property_transcoder.py` & `property-graph-2.0.3/src/pypg/property_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/allowed_range.py` & `property-graph-2.0.3/src/pypg/traits/allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/config.py` & `property-graph-2.0.3/src/pypg/traits/config.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/obligate.py` & `property-graph-2.0.3/src/pypg/traits/obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/observable.py` & `property-graph-2.0.3/src/pypg/traits/observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/overridable.py` & `property-graph-2.0.3/src/pypg/traits/overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/read_only.py` & `property-graph-2.0.3/src/pypg/traits/read_only.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/traits/validated.py` & `property-graph-2.0.3/src/pypg/traits/validated.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/transcode.py` & `property-graph-2.0.3/src/pypg/transcode.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/type_registry.py` & `property-graph-2.0.3/src/pypg/type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/src/pypg/type_utils.py` & `property-graph-2.0.3/src/pypg/type_utils.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_allowed_range.py` & `property-graph-2.0.3/tests/test_allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_config.py` & `property-graph-2.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_locator.py` & `property-graph-2.0.3/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_obligate.py` & `property-graph-2.0.3/tests/test_obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_observable.py` & `property-graph-2.0.3/tests/test_observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_overridable.py` & `property-graph-2.0.3/tests/test_overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_property.py` & `property-graph-2.0.3/tests/test_property.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     a = Property[float](default=MethodReference(default_poly, offset=1))
     a2 = Property[float](default=MethodReference(default_poly, offset=2))
 
     @classmethod
     def default_gain(cls):
         return 1
 
-    b = Property[float](default=default_gain)
+    b = Property[float](default=MethodReference(default_gain))
 
     @classmethod
     def _optional_c_traits(cls):
         pass
 
     c = Property[int](default=1, traits=_optional_c_traits)
 
@@ -32,15 +32,15 @@
         return self.a + self.b + self.c
 
     @classmethod
     def _d_traits(cls):
         return Unit("mm"), Observable[PostSet]()
 
     d = Property[float](
-        default=1, getter=default_sum, traits=_d_traits
+        default=1, getter=MethodReference(default_sum), traits=_d_traits
     )
 
 
 class PropertyTest(TestCase):
     def test_method_reference(self):
         mr = MethodReference(Example.default_poly)
         ex = Example()
```

### Comparing `property-graph-2.0.2/tests/test_readonly.py` & `property-graph-2.0.3/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_traits.py` & `property-graph-2.0.3/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_transcoder.py` & `property-graph-2.0.3/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_type_registry.py` & `property-graph-2.0.3/tests/test_type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.2/tests/test_type_schema_encoding.py` & `property-graph-2.0.3/tests/test_type_schema_encoding.py`

 * *Files identical despite different names*

