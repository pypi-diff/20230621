# Comparing `tmp/ultima-1.1.1.zip` & `tmp/ultima-1.1.5.zip`

## zipinfo {}

```diff
@@ -1,36 +1,38 @@
-Zip file size: 58495 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-17 21:44 ultima-1.1.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-17 21:44 ultima-1.1.1/ultima/
--rw-r--r--  2.0 unx     1493 b- defN 23-Jan-17 21:44 ultima-1.1.1/setup.py
--rw-r--r--  2.0 unx     2885 b- defN 23-Jan-17 21:44 ultima-1.1.1/PKG-INFO
--rw-r--r--  2.0 unx     1493 b- defN 23-Jan-17 21:44 ultima-1.1.1/quicklib_setup_from_yml.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jan-17 21:44 ultima-1.1.1/setup.cfg
--rw-r--r--  2.0 unx      247 b- defN 23-Jan-17 21:44 ultima-1.1.1/MANIFEST.in
--rw-r--r--  2.0 unx     1581 b- defN 23-Jan-17 21:44 ultima-1.1.1/README.md
--rw-rw-rw-  2.0 unx    27123 b- defN 23-Jan-17 21:44 ultima-1.1.1/quicklib_incorporated.v2.4.zip
--rw-r--r--  2.0 unx        2 b- defN 23-Jan-17 21:44 ultima-1.1.1/dynamic_extras_require.txt
--rw-r--r--  2.0 unx     1071 b- defN 23-Jan-17 21:44 ultima-1.1.1/LICENSE.md
--rw-r--r--  2.0 unx        8 b- defN 23-Jan-17 21:44 ultima-1.1.1/dynamic_install_requires.txt
--rw-r--r--  2.0 unx     2885 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/top_level.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/requires.txt
--rw-r--r--  2.0 unx      591 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-17 21:44 ultima-1.1.1/ultima/tests/
--rw-r--r--  2.0 unx     8552 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/_mapping.py
--rw-r--r--  2.0 unx      272 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/typing.py
--rw-r--r--  2.0 unx     9100 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/bfr.py
--rw-r--r--  2.0 unx     5134 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/_workerapi.py
--rw-r--r--  2.0 unx     2022 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/_registry.py
--rw-r--r--  2.0 unx    13497 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/workforce.py
--rw-r--r--  2.0 unx     1861 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/args.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/inline.py
--rw-r--r--  2.0 unx     1490 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/utils.py
--rw-r--r--  2.0 unx     9203 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/backend.py
--rw-r--r--  2.0 unx      303 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/__version__.py
--rw-r--r--  2.0 unx     1774 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/tests/conftest.py
--rw-r--r--  2.0 unx    22755 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/tests/test_ultima.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-17 21:44 ultima-1.1.1/ultima/tests/__init__.py
-34 files, 116534 bytes uncompressed, 53753 bytes compressed:  53.9%
+Zip file size: 52184 bytes, number of entries: 36
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:16 ultima-1.1.5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:16 ultima-1.1.5/ultima/
+-rw-r--r--  2.0 unx     1493 b- defN 23-Jun-20 14:16 ultima-1.1.5/quicklib_setup_from_yml.py
+-rw-r--r--  2.0 unx     1883 b- defN 23-Jun-20 14:15 ultima-1.1.5/README.md
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jun-20 14:15 ultima-1.1.5/LICENSE.md
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-20 14:16 ultima-1.1.5/MANIFEST.in
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-20 14:16 ultima-1.1.5/dynamic_install_requires.txt
+-rw-r--r--  2.0 unx     1493 b- defN 23-Jun-20 14:16 ultima-1.1.5/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-20 14:16 ultima-1.1.5/setup.cfg
+-rw-r--r--  2.0 unx     3291 b- defN 23-Jun-20 14:16 ultima-1.1.5/PKG-INFO
+-rw-r--r--  2.0 unx        2 b- defN 23-Jun-20 14:16 ultima-1.1.5/dynamic_extras_require.txt
+-rw-rw-rw-  2.0 unx    17043 b- defN 23-Jun-20 14:16 ultima-1.1.5/quicklib_incorporated.v2.5.zip
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/requires.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      643 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     3291 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 14:16 ultima-1.1.5/ultima/tests/
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/__init__.py
+-rw-r--r--  2.0 unx      279 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/typing.py
+-rw-r--r--  2.0 unx     9152 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/bfr.py
+-rw-r--r--  2.0 unx     1861 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/args.py
+-rw-r--r--  2.0 unx     8424 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/_mapping.py
+-rw-r--r--  2.0 unx    19360 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/workforce.py
+-rw-r--r--  2.0 unx     5134 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/_workerapi.py
+-rw-r--r--  2.0 unx     5310 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/_recursive.py
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/inline.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-20 14:16 ultima-1.1.5/ultima/__version__.py
+-rw-r--r--  2.0 unx     1490 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/utils.py
+-rw-r--r--  2.0 unx     2051 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/_registry.py
+-rw-r--r--  2.0 unx     9358 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/backend.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/tests/__init__.py
+-rw-r--r--  2.0 unx     1774 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/tests/conftest.py
+-rw-r--r--  2.0 unx    22893 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/tests/test_ultima.py
+-rw-r--r--  2.0 unx     3323 b- defN 23-Jun-20 14:15 ultima-1.1.5/ultima/tests/test_recursive.py
+36 files, 122369 bytes uncompressed, 47138 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,103 +1,109 @@
-Filename: ultima-1.1.1/
+Filename: ultima-1.1.5/
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/
+Filename: ultima-1.1.5/ultima.egg-info/
 Comment: 
 
-Filename: ultima-1.1.1/ultima/
+Filename: ultima-1.1.5/ultima/
 Comment: 
 
-Filename: ultima-1.1.1/setup.py
+Filename: ultima-1.1.5/quicklib_setup_from_yml.py
 Comment: 
 
-Filename: ultima-1.1.1/PKG-INFO
+Filename: ultima-1.1.5/README.md
 Comment: 
 
-Filename: ultima-1.1.1/quicklib_setup_from_yml.py
+Filename: ultima-1.1.5/LICENSE.md
 Comment: 
 
-Filename: ultima-1.1.1/setup.cfg
+Filename: ultima-1.1.5/MANIFEST.in
 Comment: 
 
-Filename: ultima-1.1.1/MANIFEST.in
+Filename: ultima-1.1.5/dynamic_install_requires.txt
 Comment: 
 
-Filename: ultima-1.1.1/README.md
+Filename: ultima-1.1.5/setup.py
 Comment: 
 
-Filename: ultima-1.1.1/quicklib_incorporated.v2.4.zip
+Filename: ultima-1.1.5/setup.cfg
 Comment: 
 
-Filename: ultima-1.1.1/dynamic_extras_require.txt
+Filename: ultima-1.1.5/PKG-INFO
 Comment: 
 
-Filename: ultima-1.1.1/LICENSE.md
+Filename: ultima-1.1.5/dynamic_extras_require.txt
 Comment: 
 
-Filename: ultima-1.1.1/dynamic_install_requires.txt
+Filename: ultima-1.1.5/quicklib_incorporated.v2.5.zip
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/PKG-INFO
+Filename: ultima-1.1.5/ultima.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/dependency_links.txt
+Filename: ultima-1.1.5/ultima.egg-info/requires.txt
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/top_level.txt
+Filename: ultima-1.1.5/ultima.egg-info/top_level.txt
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/requires.txt
+Filename: ultima-1.1.5/ultima.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ultima-1.1.1/ultima.egg-info/SOURCES.txt
+Filename: ultima-1.1.5/ultima.egg-info/PKG-INFO
 Comment: 
 
-Filename: ultima-1.1.1/ultima/tests/
+Filename: ultima-1.1.5/ultima/tests/
 Comment: 
 
-Filename: ultima-1.1.1/ultima/_mapping.py
+Filename: ultima-1.1.5/ultima/__init__.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/typing.py
+Filename: ultima-1.1.5/ultima/typing.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/bfr.py
+Filename: ultima-1.1.5/ultima/bfr.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/_workerapi.py
+Filename: ultima-1.1.5/ultima/args.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/_registry.py
+Filename: ultima-1.1.5/ultima/_mapping.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/workforce.py
+Filename: ultima-1.1.5/ultima/workforce.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/args.py
+Filename: ultima-1.1.5/ultima/_workerapi.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/inline.py
+Filename: ultima-1.1.5/ultima/_recursive.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/utils.py
+Filename: ultima-1.1.5/ultima/inline.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/backend.py
+Filename: ultima-1.1.5/ultima/__version__.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/__init__.py
+Filename: ultima-1.1.5/ultima/utils.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/__version__.py
+Filename: ultima-1.1.5/ultima/_registry.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/tests/conftest.py
+Filename: ultima-1.1.5/ultima/backend.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/tests/test_ultima.py
+Filename: ultima-1.1.5/ultima/tests/__init__.py
 Comment: 
 
-Filename: ultima-1.1.1/ultima/tests/__init__.py
+Filename: ultima-1.1.5/ultima/tests/conftest.py
+Comment: 
+
+Filename: ultima-1.1.5/ultima/tests/test_ultima.py
+Comment: 
+
+Filename: ultima-1.1.5/ultima/tests/test_recursive.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ultima-1.1.1/setup.py` & `ultima-1.1.5/quicklib_setup_from_yml.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/PKG-INFO` & `ultima-1.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima
-Version: 1.1.1
+Version: 1.1.5
 Summary: Intuitive parallel map calls for Python
 Home-page: https://github.com/Cybereason/ultima
 Author: Yonatan Perry, Assaf Ben-David, Uri Sternfeld
 License: MIT License
 Description: # Ultima - intuitive parallel `map()` for Python
         [![Ultima CI](https://github.com/Cybereason/ultima/actions/workflows/ci.yml/badge.svg)](https://github.com/Cybereason/ultima/actions/workflows/ci.yml)
         
@@ -61,14 +61,27 @@
         
         urls = open("urls.txt")
         webpages = ultimap(io_intensive, urls, backend='threading', n_workers=64)
         hashes = ultimap(cpu_intensive, webpages, backend='multiprocessing')
         print(len(set(hashes)))
         ```
         
+        You can also map a function recursively:
+        
+        ```python
+        from ultima import ultimap
+        
+        def visit(graph, node, add_input):
+            for child_node in graph.get_children(node):
+                add_input(graph, child_node)
+            return f"visited {node}"
+        
+        print(list(ultimap(visit, [(graph, graph.root)], recursive=True)))
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

## Comparing `ultima-1.1.1/quicklib_setup_from_yml.py` & `ultima-1.1.5/setup.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/README.md` & `ultima-1.1.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -53,7 +53,20 @@
     return hashlib.sha1(page.encode()).hexdigest()
 
 urls = open("urls.txt")
 webpages = ultimap(io_intensive, urls, backend='threading', n_workers=64)
 hashes = ultimap(cpu_intensive, webpages, backend='multiprocessing')
 print(len(set(hashes)))
 ```
+
+You can also map a function recursively:
+
+```python
+from ultima import ultimap
+
+def visit(graph, node, add_input):
+    for child_node in graph.get_children(node):
+        add_input(graph, child_node)
+    return f"visited {node}"
+
+print(list(ultimap(visit, [(graph, graph.root)], recursive=True)))
+```
```

## Comparing `ultima-1.1.1/LICENSE.md` & `ultima-1.1.5/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima.egg-info/PKG-INFO` & `ultima-1.1.5/ultima.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima
-Version: 1.1.1
+Version: 1.1.5
 Summary: Intuitive parallel map calls for Python
 Home-page: https://github.com/Cybereason/ultima
 Author: Yonatan Perry, Assaf Ben-David, Uri Sternfeld
 License: MIT License
 Description: # Ultima - intuitive parallel `map()` for Python
         [![Ultima CI](https://github.com/Cybereason/ultima/actions/workflows/ci.yml/badge.svg)](https://github.com/Cybereason/ultima/actions/workflows/ci.yml)
         
@@ -61,14 +61,27 @@
         
         urls = open("urls.txt")
         webpages = ultimap(io_intensive, urls, backend='threading', n_workers=64)
         hashes = ultimap(cpu_intensive, webpages, backend='multiprocessing')
         print(len(set(hashes)))
         ```
         
+        You can also map a function recursively:
+        
+        ```python
+        from ultima import ultimap
+        
+        def visit(graph, node, add_input):
+            for child_node in graph.get_children(node):
+                add_input(graph, child_node)
+            return f"visited {node}"
+        
+        print(list(ultimap(visit, [(graph, graph.root)], recursive=True)))
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

## Comparing `ultima-1.1.1/ultima.egg-info/SOURCES.txt` & `ultima-1.1.5/ultima.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE.md
 MANIFEST.in
 README.md
 dynamic_extras_require.txt
 dynamic_install_requires.txt
-quicklib_incorporated.v2.4.zip
+quicklib_incorporated.v2.5.zip
 quicklib_setup_from_yml.py
 ultima/__init__.py
 ultima/__version__.py
 ultima/_mapping.py
+ultima/_recursive.py
 ultima/_registry.py
 ultima/_workerapi.py
 ultima/args.py
 ultima/backend.py
 ultima/bfr.py
 ultima/inline.py
 ultima/typing.py
@@ -20,8 +21,9 @@
 ultima.egg-info/PKG-INFO
 ultima.egg-info/SOURCES.txt
 ultima.egg-info/dependency_links.txt
 ultima.egg-info/requires.txt
 ultima.egg-info/top_level.txt
 ultima/tests/__init__.py
 ultima/tests/conftest.py
+ultima/tests/test_recursive.py
 ultima/tests/test_ultima.py
```

## Comparing `ultima-1.1.1/ultima/_mapping.py` & `ultima-1.1.5/ultima/_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from math import ceil
 from functools import partial
 from collections.abc import Sized
 from concurrent.futures import BrokenExecutor
-from typing import Optional, Callable, Iterable, List, Collection, \
-    Union, Tuple, Any, Generic, TypeVar, TYPE_CHECKING, get_args
+from typing import Optional, Callable, Iterable, Iterator, List, \
+    Collection, Generic, TypeVar, TYPE_CHECKING, get_args, cast
 
 from .bfr import BufferedFutureResolver, KeyedFuture
 from .args import Args
 from .utils import class_logger, batches
 from .typing import ReturnKey, Error
 from ._registry import RegistryKey
 from ._workerapi import WorkerAPI, ErrorResult
@@ -61,16 +61,16 @@
         Return with each result a key identifying it as a tuple (key, result). May be useful if `ordered` is False.
         - 'none':  Do not return a key. Each result is yielded as is.
         - 'idx':   The key is the zero-based running index of the input.
         - 'input': The key is the input itself in its entirety.
     """
     logger = class_logger()
 
-    def __init__(self, workforce: "Workforce", func: Callable[..., T], inputs: Iterable, ordered: bool = False,
-                 buffering: Optional[int] = None, batch_size: int = 1, errors: Error = 'raise',
+    def __init__(self, workforce: "Workforce", func: Callable, inputs: Iterable,
+                 ordered: bool = False, buffering: Optional[int] = None, batch_size: int = 1, errors: Error = 'raise',
                  timeout: Optional[float] = None, return_key: ReturnKey = 'none'):
         assert errors in get_args(Error)
         assert return_key in get_args(ReturnKey)
         self.batch_size = batch_size
         self.errors = errors
         self.return_key = return_key
         func_key = workforce.func_registry.register(func)
@@ -91,22 +91,22 @@
         )
         results = self.bfr
         results = self._unbatch_results(results)
         results = self._handle_errors(results)
         results = self._handle_workforce_failures(results, workforce)
         if self.return_key == 'none':
             results = (i[1] for i in results)
-        self._results = results
+        self._results = cast(Iterator[T], results)
 
     def __len__(self) -> int:
         if self._n_inputs is None:
             raise TypeError("input iterable has no length")
         return self._n_inputs
 
-    def __iter__(self) -> Union[Iterable[Union[T, Exception]], Iterable[Tuple[Any, Union[T, Exception]]]]:
+    def __iter__(self) -> Iterator[T]:
         return self._results
 
     def _batch_inputs(self, inputs: Iterable[Args]) -> Iterable[List[Args]]:
         return map(list, batches(inputs, self.batch_size))
 
     def _generate_keyed_futures(self, workforce: "Workforce", func_key: RegistryKey,
                                 input_batches: Iterable[List[Args]]) -> Iterable[KeyedFuture[list]]:
@@ -174,15 +174,15 @@
     This Mapping is used when it is the only Mapping of a Workforce, which cannot be used as
     a context manager to allow proper shutdown, e.g. by the ultimap sugaring function.
     """
     def __init__(self, workforce: "Workforce", *args, **kwargs):
         super().__init__(workforce, *args, **kwargs)
         self.workforce = workforce
 
-    def __iter__(self) -> Union[Iterable[Union[T, Exception]], Iterable[Tuple[Any, Union[T, Exception]]]]:
+    def __iter__(self) -> Iterator[T]:
         try:
             yield from super().__iter__()
         finally:
             self.terminate()
 
     def terminate(self) -> None:
         self.workforce.shutdown()
```

## Comparing `ultima-1.1.1/ultima/bfr.py` & `ultima-1.1.5/ultima/bfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import threading
 import concurrent.futures
-from typing import Iterable, Optional, Generic, TypeVar, Tuple, Any
+from typing import Iterable, Iterator, Dict, Optional, Generic, TypeVar, Tuple, Any
 
 from .utils import class_logger
 
 
 T = TypeVar("T")
 
 
@@ -59,23 +59,23 @@
         self.active = True
         self._start_time = None
         self._feeder_error = None
 
         self.lock = threading.Lock()
         self.evt_new_future = threading.Event()
         self.evt_new_capacity = threading.Event()
-        self.futures = {}
+        self.futures: Dict[concurrent.futures.Future, T] = {}
 
         self.feeder_thread = threading.Thread(
             target=self._feeder_thread_impl,
             daemon=True,
             name=None if self.name is None else f"{self.name}-FeederThread"
         )
 
-    def __iter__(self) -> Iterable[Tuple[T, Any]]:
+    def __iter__(self) -> Iterator[Tuple[T, Any]]:
         self._start_time = time.monotonic()
         self.feeder_thread.start()
         yield from self._futures_iter()
 
     # dev note: this code runs in a single-use thread
     # WARNING: this is a daemon thread, do not assume resource cleanup or try-finally mechanisms work
     def _feeder_thread_impl(self):
```

## Comparing `ultima-1.1.1/ultima/_workerapi.py` & `ultima-1.1.5/ultima/_workerapi.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima/_registry.py` & `ultima-1.1.5/ultima/_registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import hashlib
-from typing import Union, Callable, TypeVar, Iterator, Generic, Mapping
+from typing import Union, Callable, TypeVar, Iterator, Generic, Mapping, Dict
 
 from .backend import Backend
 
 
 T = TypeVar("T")
 KT = TypeVar("KT")
 VT_co = TypeVar('VT_co', covariant=True)
@@ -13,28 +13,28 @@
 class DeserializerMapping(Mapping[KT, VT_co]):
     """
     A wrapper for a mapping, which also deserializes the values upon access.
 
     In addition, values are cached when accessed.
     """
     def __init__(self, items: Mapping[KT, T], deserializer: Callable[[T], VT_co]):
-        self.items = items
-        self.deserializer = deserializer
-        self._cache = {}
+        self._items = items
+        self._deserializer = deserializer
+        self._cache: Dict[KT, VT_co] = {}
 
     def __getitem__(self, key: KT) -> VT_co:
         if key not in self._cache:
-            self._cache[key] = self.deserializer(self.items[key])
+            self._cache[key] = self._deserializer(self._items[key])
         return self._cache[key]
 
     def __len__(self) -> int:
-        return len(self.items)
+        return len(self._items)
 
     def __iter__(self) -> Iterator[KT]:
-        return iter(self.items)
+        return iter(self._items)
 
 
 class SerializedItemsRegistry(Generic[T]):
     """
     A registry of serialized items, accessible from both the Workforce side and the workers.
 
     The registry is implemented using a Mapping appropriate for the backend used, and the serialization is also
```

## Comparing `ultima-1.1.1/ultima/args.py` & `ultima-1.1.5/ultima/args.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima/inline.py` & `ultima-1.1.5/ultima/inline.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima/utils.py` & `ultima-1.1.5/ultima/utils.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima/backend.py` & `ultima-1.1.5/ultima/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import signal
 import threading
 import multiprocessing
 import multiprocessing.managers
 import concurrent.futures
 from functools import partial
 from abc import ABC, abstractmethod
-from typing import Union, Type, TypeVar, Literal
+from typing import Union, Type, TypeVar, Literal, Optional, overload
 
 import dill
 
 from .inline import InlineExecutor
 
 
 #
@@ -40,15 +40,15 @@
     @property
     def executor_shutdown_nowait_allowed(self) -> bool:
         """Indicates whether we should call executor.shutdown with wait=False."""
         return True
 
     @classmethod
     @abstractmethod
-    def parse_n_workers(cls, n_workers: Union[int, float, None]) -> int:
+    def parse_n_workers(cls, n_workers) -> int:
         """
         Parse the `n_workers` parameters in the context of the relevant backend
         and return the actual number of workers to use.
 
         Parameters
         ----------
         n_workers : int, float or None
@@ -108,18 +108,24 @@
 
     def shutdown(self):
         """Shut down any resources this backend uses."""
         pass
 
 
 BackendType = TypeVar('BackendType', bound=Backend)
-BackendArgument = Union[str, BackendType, Type[BackendType]]
+BackendArgument = Union[str, Backend, Type[Backend]]
 
 
-def get_backend(name_or_backend: BackendArgument) -> BackendType:
+@overload
+def get_backend(name_or_backend: Union[BackendType, Type[BackendType]]) -> BackendType: ...
+@overload
+def get_backend(name_or_backend: str) -> Backend: ...
+
+
+def get_backend(name_or_backend: BackendArgument):
     """
     Get a Backend object by name or, if already providing a backend class or object,
     returns an instance of the backend.
 
     Parameters
     ----------
     name_or_backend : str, Backend or Backend class
@@ -195,15 +201,15 @@
     Attributes
     ----------
     manager
     CONTEXT : str or None
         Name of the multiprocessing context used by this backend.
     """
     NAME = "multiprocessing"
-    CONTEXT = None
+    CONTEXT: Optional[str] = None
 
     def __init__(self):
         self._manager = None
         self._lock = threading.Lock()
 
     @property
     def _ctx(self):
```

## Comparing `ultima-1.1.1/ultima/tests/conftest.py` & `ultima-1.1.5/ultima/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `ultima-1.1.1/ultima/tests/test_ultima.py` & `ultima-1.1.5/ultima/tests/test_ultima.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import math
 import time
 import random
 import signal
 import weakref
 import itertools
 import threading
-from numbers import Number
+from typing import Optional
 from functools import partial
 from contextlib import contextmanager
 from concurrent.futures import BrokenExecutor
 
 import psutil
 import pytest
 
 from ultima import Workforce, Args, ultimap, MultiprocessingBackend, ThreadingBackend, InlineBackend
 from ultima.utils import class_logger
+from ultima.typing import Error
 
 
 #
 # marks
 #
 
 skip = pytest.mark.skip
@@ -325,14 +326,15 @@
         else:
             pytest.fail()
 
     @mark_flaky
     @stages(4)
     @on_three_backends
     @pytest.mark.timeout(30)
+    @pytest.mark.skipif(sys.platform == 'win32', reason='occasionally fails on Windows')
     def test_incomplete_usage(self, backend, n_workers, stage):
         def once():
             with Workforce(backend, n_workers, shutdown_mode='wait') as workforce:
                 if stage >= 1:
                     mapping = workforce.map(
                         Func.pow2, range(10), ordered=False, buffering=3, batch_size=1, errors='return',
                         timeout=None, return_key='idx',
@@ -423,15 +425,15 @@
 
 class TestInline:
     @pytest.mark.parametrize("ordered", [True, False])
     @pytest.mark.parametrize("buffering", [None, 4])
     @pytest.mark.parametrize("batch_size", [1, 2])
     @pytest.mark.parametrize("errors", ['ignore', 'log', 'raise', 'return'])
     @pytest.mark.parametrize("timeout", [None, 10])
-    def test_inline_multi(self, ordered, buffering, batch_size, errors, timeout: Number):
+    def test_inline_multi(self, ordered, buffering, batch_size, errors: Error, timeout: Optional[float]):
         with Workforce('inline', n_workers=0) as workforce:
             result = sum(workforce.map(
                 Func.pow2, range(10), ordered=ordered, buffering=buffering, batch_size=batch_size, errors=errors,
                 timeout=timeout
             ))
         assert result == sum(i**2 for i in range(10))
```

