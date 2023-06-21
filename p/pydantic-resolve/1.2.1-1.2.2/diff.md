# Comparing `tmp/pydantic_resolve-1.2.1.tar.gz` & `tmp/pydantic_resolve-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.2.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.2.2.tar", max compression
```

## Comparing `pydantic_resolve-1.2.1.tar` & `pydantic_resolve-1.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.1/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2217 2023-06-18 14:39:54.866965 pydantic_resolve-1.2.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     5170 2023-06-19 10:02:56.509176 pydantic_resolve-1.2.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     3898 2023-06-18 01:11:55.489541 pydantic_resolve-1.2.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-19 10:06:48.583578 pydantic_resolve-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.2.1/README.md
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.2/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.2/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.2/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.2.2/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.2/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     4927 2023-06-21 15:02:54.668646 pydantic_resolve-1.2.2/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     3916 2023-06-20 06:16:54.008785 pydantic_resolve-1.2.2/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-21 15:05:32.966535 pydantic_resolve-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.2.2/README.md
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.2/PKG-INFO
```

### Comparing `pydantic_resolve-1.2.1/LICENSE` & `pydantic_resolve-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.1/pydantic_resolve/__init__.py` & `pydantic_resolve-1.2.2/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.1/pydantic_resolve/core.py` & `pydantic_resolve-1.2.2/pydantic_resolve/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,22 @@
 def iter_over_object_post_methods(target):
     """get method starts with post_"""
     for k in dir(target):
         if k.startswith(POST_PREFIX) and ismethod(target.__getattribute__(k)):
             yield k
 
 async def resolve_obj(target, field):
+    """
+    TODO: deprecated, will remove in v2.0
+    """
     item = target.__getattribute__(field)
     try:
         val = item()
     except AttributeError as e:
         if str(e) == "'Depends' object has no attribute 'load'":  
-            # TODO: str(e) may changes in future, not stable
             raise DataloaderDependCantBeResolved("DataLoader used in schema, use Resolver().resolve() instead")
         raise e
 
     while iscoroutine(val) or asyncio.isfuture(val):
         val = await val
 
     val = await resolve(val)  
@@ -49,15 +51,18 @@
     replace_attr_name = field.replace(PREFIX, '')
     if hasattr(target, replace_attr_name):
         target.__setattr__(replace_attr_name, val)
     else:
         raise ResolverTargetAttrNotFound(f"attribute {replace_attr_name} not found")
 
 async def resolve(target: T) -> T:
-    """ entry: resolve dataclass object or pydantic object / or list in place """
+    """ 
+    entry: resolve dataclass object or pydantic object / or list in place 
+    TODO: deprecated, will remove in v2.0
+    """
 
     if isinstance(target, (list, tuple)):  # core/test_1, 3
         await asyncio.gather(*[resolve(t) for t in target])
 
     if is_acceptable_type(target):
         await asyncio.gather(*[resolve_obj(target, field) 
                                for field in iter_over_object_resolvers(target)])
```

### Comparing `pydantic_resolve-1.2.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.2.2/pydantic_resolve/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     Entrypoint of a resolve action
     """
     def __init__(self, loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, ensure_type=False):
         self.ctx = contextvars.ContextVar('pydantic_resolve_internal_context', default={})
         self.loader_filters_ctx = contextvars.ContextVar('pydantic_resolve_internal_filter', default=loader_filters or {})
         self.ensure_type = ensure_type
     
+
     def exec_method(self, method):
         signature = inspect.signature(method)
         params = {}
 
         # manage the creation of loader instances
         for k, v in signature.parameters.items():
             if isinstance(v.default, Depends):
                 # Base: DataLoader or batch_load_fn
-                # transform: data transform function
                 Base = v.default.dependency
 
                 # module.kls to avoid same kls name from different module
                 cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
 
                 cache_provider = self.ctx.get()
                 hit = cache_provider.get(cache_key, None)
@@ -61,18 +61,16 @@
                         loader = Base()
 
                         # and pick config from 'loader_filters' param, only for DataClass
                         filter_config_provider = self.loader_filters_ctx.get()
                         filter_config = filter_config_provider.get(Base, {})
 
                         # class ExampleLoader(DataLoader):
-                        #     filtar_x: bool  <--------------- set this
-                        #
-                        #     async def batch_load_fn(self, keys):
-                        #         ....
+                        #     filtar_x: bool  <--------------- set this field
+
                         for field in get_class_field_annotations(Base):
                             try:
                                 value = filter_config[field]
                                 setattr(loader, field, value)
                             except KeyError:
                                 raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
@@ -81,46 +79,45 @@
                         loader = DataLoader(batch_load_fn=Base) # type:ignore
 
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
+
     async def resolve_obj(self, target, field):
         item = target.__getattribute__(field)
         target_attr_name = str(field).replace(PREFIX, '')
-        val = self.exec_method(item)
 
         if not hasattr(target, target_attr_name):
             raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
 
         if self.ensure_type:
             if not item.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
+        val = self.exec_method(item)
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
-        # start to resolve
         val = await self.resolve(val)  
-        # all children is resolved
         target.__setattr__(target_attr_name, val)
 
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
 
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
             await asyncio.gather(*[self.resolve_obj(target, field) 
                                    for field in core.iter_over_object_resolvers(target)])
 
-            # execute post methods, accept no params
+            # execute post methods, take no params
             for post_key in core.iter_over_object_post_methods(target):
                 post_attr_name = post_key.replace(POST_PREFIX, '')
                 if not hasattr(target, post_attr_name):
                     raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
 
                 post_method = target.__getattribute__(post_key)
                 post_method()
```

### Comparing `pydantic_resolve-1.2.1/pydantic_resolve/util.py` & `pydantic_resolve-1.2.2/pydantic_resolve/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import asyncio
 from collections import defaultdict
 from dataclasses import is_dataclass
 import functools
 from pydantic import BaseModel
 from inspect import iscoroutine
-from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator
 import types
 
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
 T = TypeVar("T")
 V = TypeVar("V")
 
-def build_object(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> List[Optional[T]]:
+def build_object(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> Iterator[Optional[T]]:
     """
     helper function to build return object data required by aiodataloader
     """
     dct: Mapping[V, T] = {}
     for item in items:
         _key = get_pk(item)
         dct[_key] = item
-    results = [dct.get(k, None) for k in keys]
+    results = (dct.get(k, None) for k in keys)
     return results
 
 
-def build_list(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> List[List[T]]:
+def build_list(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> Iterator[List[T]]:
     """
     helper function to build return list data required by aiodataloader
     """
     dct: DefaultDict[V, List[T]] = defaultdict(list) 
     for item in items:
         _key = get_pk(item)
         dct[_key].append(item)
-    results = [dct.get(k, []) for k in keys]
+    results = (dct.get(k, []) for k in keys)
     return results
 
 
 def replace_method(cls: Type, cls_name: str, func_name: str, func: Callable):
     KLS = type(cls_name, (cls,), {func_name: func})
     return KLS
```

### Comparing `pydantic_resolve-1.2.1/pyproject.toml` & `pydantic_resolve-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.2.1"
+version = "1.2.2"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.2.1/README.md` & `pydantic_resolve-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.1/PKG-INFO` & `pydantic_resolve-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.2.1
+Version: 1.2.2
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

