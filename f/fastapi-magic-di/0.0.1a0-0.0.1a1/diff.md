# Comparing `tmp/fastapi_magic_di-0.0.1a0.tar.gz` & `tmp/fastapi_magic_di-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_magic_di-0.0.1a0.tar", max compression
+gzip compressed data, was "fastapi_magic_di-0.0.1a1.tar", max compression
```

## Comparing `fastapi_magic_di-0.0.1a0.tar` & `fastapi_magic_di-0.0.1a1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-06-19 15:24:15.936987 fastapi_magic_di-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     6121 2023-06-20 17:58:52.765447 fastapi_magic_di-0.0.1a0/README.md
--rw-r--r--   0        0        0      135 2023-06-19 17:30:16.294073 fastapi_magic_di-0.0.1a0/fastapi_di/__init__.py
--rw-r--r--   0        0        0      194 2023-06-13 12:43:05.534905 fastapi_magic_di-0.0.1a0/fastapi_di/_client.py
--rw-r--r--   0        0        0     3214 2023-06-20 17:39:51.603148 fastapi_magic_di-0.0.1a0/fastapi_di/_injector.py
--rw-r--r--   0        0        0      403 2023-06-19 17:30:16.287886 fastapi_magic_di-0.0.1a0/fastapi_di/_provide.py
--rw-r--r--   0        0        0      323 2023-06-20 15:38:00.089246 fastapi_magic_di-0.0.1a0/fastapi_di/app.py
--rw-r--r--   0        0        0     1263 2023-06-20 17:39:08.841831 fastapi_magic_di-0.0.1a0/fastapi_di/env_fields.py
--rw-r--r--   0        0        0      642 2023-06-20 17:22:25.327646 fastapi_magic_di-0.0.1a0/fastapi_di/testing.py
--rw-r--r--   0        0        0      539 2023-06-20 17:56:49.616212 fastapi_magic_di-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     6662 1970-01-01 00:00:00.000000 fastapi_magic_di-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 15:24:15.936987 fastapi_magic_di-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     6594 2023-06-20 22:43:28.229677 fastapi_magic_di-0.0.1a1/README.md
+-rw-r--r--   0        0        0      135 2023-06-20 23:10:27.653763 fastapi_magic_di-0.0.1a1/fastapi_di/__init__.py
+-rw-r--r--   0        0        0      194 2023-06-13 12:43:05.534905 fastapi_magic_di-0.0.1a1/fastapi_di/_client.py
+-rw-r--r--   0        0        0     3726 2023-06-20 21:07:58.474624 fastapi_magic_di-0.0.1a1/fastapi_di/_injector.py
+-rw-r--r--   0        0        0      647 2023-06-20 23:11:38.870175 fastapi_magic_di-0.0.1a1/fastapi_di/_provide.py
+-rw-r--r--   0        0        0      323 2023-06-20 15:38:00.089246 fastapi_magic_di-0.0.1a1/fastapi_di/app.py
+-rw-r--r--   0        0        0     1263 2023-06-20 17:39:08.841831 fastapi_magic_di-0.0.1a1/fastapi_di/env_fields.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:11:07.065409 fastapi_magic_di-0.0.1a1/fastapi_di/py.typed
+-rw-r--r--   0        0        0      642 2023-06-20 17:22:25.327646 fastapi_magic_di-0.0.1a1/fastapi_di/testing.py
+-rw-r--r--   0        0        0      574 2023-06-20 23:12:17.565646 fastapi_magic_di-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 fastapi_magic_di-0.0.1a1/PKG-INFO
```

### Comparing `fastapi_magic_di-0.0.1a0/LICENSE` & `fastapi_magic_di-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a0/README.md` & `fastapi_magic_di-0.0.1a1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # FastAPI Magic DI
 Dependency Injector for FastAPI that makes your life easier
 
 
 What are the problems with FastAPI’s dependency injector? 
 1) It forces you to use global variables. 
-2) It is hard to test. For example, what if you need to mock only one embedded dependency?  
+2) You need to write an endless number of fabrics with startup logic
 3) It makes your project highly dependent on FastAPI’s injector by using “Depends” everywhere.
 
 To solve these problems, you can use this dead-simple Dependency Injector that will make development so much easier.
 
+__Q: But why not to use [python-dependency-injector](https://github.com/ets-labs/python-dependency-injector) or other libs?__
+
+A: The goal of this Dependency Injector is to __reduce the amount of code as much as possible__ and get rid of enterprise code with millions of configs, containers, and fabrics. That’s why python-dependency-injector and similar libraries are overkill. The philosophy of this injector is that clients know how to configure themselves and perform all startup routines.
+
 * [Install](#install)
 * [Getting Started](#getting-started)
 * [Clients Configuration](#clients-configuration)
   * [Zero config clients](#zero-config-clients)
   * [Clients with Config](#clients-with-config)
 * [Using interfaces instead of implementations](#using-interfaces-instead-of-implementations)
 * [Testing](#testing)
@@ -49,15 +53,15 @@
         self.db = db
         
     def is_connected(self):
         return self.db.connected
     
 
 @app.get(path="/hello-world")
-def hello_world(service: Provide(Service)) -> dict:
+def hello_world(service: Provide[Service]) -> dict:
     return {
         "is_connected": service.is_connected()
     }
 
 ```
 
 That's all!
@@ -162,15 +166,15 @@
 app = inject_app(FastAPI())
 
 injector.bind({MyInterface: MyInterfaceImplementation})
 
 
 
 @app.get(path="/hello-world")
-def hello_world(service: Provide(MyInterface)) -> dict:
+def hello_world(service: Provide[MyInterface]) -> dict:
     return {
         "result": service.do_something(),
     }
 ```
 
 Using `injector.bind`, you can bind implementations that will be injected everywhere the bound interface is used.
```

### Comparing `fastapi_magic_di-0.0.1a0/fastapi_di/_injector.py` & `fastapi_magic_di-0.0.1a1/fastapi_di/_injector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 import logging
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from functools import partial
-from typing import (
-    Any,
-    Type,
-    TypeVar,
-    get_type_hints,
-    Callable,
-    Union,
-)
+from types import UnionType
+from typing import Any, Type, TypeVar, get_type_hints, Callable, Union, get_args
 
 from fastapi_di._client import ClientProtocol
 
 
 def is_client(cls: Type[ClientProtocol]) -> bool:
     try:
         return issubclass(cls, ClientProtocol)
     except TypeError:
         return False
 
 
 T = TypeVar("T")
 
 
+def _get_cls_from_optional(cls: Type[T]) -> Type[T]:
+    if not isinstance(cls, UnionType):
+        return cls
+
+    args = get_args(cls)
+    if len(args) != 2:
+        raise ValueError(
+            "Dependency injector doesn't support such complex hints. "
+            "Supported only 'Union[cls, None]', 'cls | None', 'Optional[cls]'"
+        )
+
+    for typo in args:
+        if not issubclass(typo, type(None)):
+            return typo
+
+
 def _is_class(obj: Any) -> bool:
     return isinstance(obj, type)
 
 
 @dataclass
 class DependencyInjector:
     logger: logging.Logger = field(
         default_factory=lambda: logging.getLogger("injector")
     )
     bindings: dict = field(default_factory=dict)
     _deps: dict[Type[T], T] = field(init=False, default_factory=dict)  # type: ignore
     _postponed: list[Type[T]] = field(init=False, default_factory=list)
 
     def inject(self, obj: Union[Type[T], Callable]) -> Union[T, Callable]:
+        obj = _get_cls_from_optional(obj)
         obj = self.bindings.get(obj, obj)
 
         if instance := self._deps.get(obj):
             return instance  # type: ignore
 
         if _is_class(obj):
             hints = get_type_hints(obj.__init__)
         else:
             hints = get_type_hints(obj)
 
         clients = {}
 
         for name, hint in hints.items():
-            bound_obj_for_hint = self.bindings.get(hint, hint)
-            if not is_client(bound_obj_for_hint):
+            hint = _get_cls_from_optional(hint)
+            hint = self.bindings.get(hint, hint)
+
+            if not is_client(hint):
                 continue
 
             instance = self.inject(hint)
             clients[name] = instance
 
         if _is_class(obj):
             self._deps[obj] = obj(**clients)  # type: ignore
```

### Comparing `fastapi_magic_di-0.0.1a0/fastapi_di/env_fields.py` & `fastapi_magic_di-0.0.1a1/fastapi_di/env_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a0/fastapi_di/testing.py` & `fastapi_magic_di-0.0.1a1/fastapi_di/testing.py`

 * *Files identical despite different names*

### Comparing `fastapi_magic_di-0.0.1a0/PKG-INFO` & `fastapi_magic_di-0.0.1a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-magic-di
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Dependency Injector for FastAPI that makes your life easier
 License: MIT
 Author: Nikita Zavadin
 Author-email: zavadin142@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,23 @@
 
 # FastAPI Magic DI
 Dependency Injector for FastAPI that makes your life easier
 
 
 What are the problems with FastAPI’s dependency injector? 
 1) It forces you to use global variables. 
-2) It is hard to test. For example, what if you need to mock only one embedded dependency?  
+2) You need to write an endless number of fabrics with startup logic
 3) It makes your project highly dependent on FastAPI’s injector by using “Depends” everywhere.
 
 To solve these problems, you can use this dead-simple Dependency Injector that will make development so much easier.
 
+__Q: But why not to use [python-dependency-injector](https://github.com/ets-labs/python-dependency-injector) or other libs?__
+
+A: The goal of this Dependency Injector is to __reduce the amount of code as much as possible__ and get rid of enterprise code with millions of configs, containers, and fabrics. That’s why python-dependency-injector and similar libraries are overkill. The philosophy of this injector is that clients know how to configure themselves and perform all startup routines.
+
 * [Install](#install)
 * [Getting Started](#getting-started)
 * [Clients Configuration](#clients-configuration)
   * [Zero config clients](#zero-config-clients)
   * [Clients with Config](#clients-with-config)
 * [Using interfaces instead of implementations](#using-interfaces-instead-of-implementations)
 * [Testing](#testing)
@@ -65,15 +69,15 @@
         self.db = db
         
     def is_connected(self):
         return self.db.connected
     
 
 @app.get(path="/hello-world")
-def hello_world(service: Provide(Service)) -> dict:
+def hello_world(service: Provide[Service]) -> dict:
     return {
         "is_connected": service.is_connected()
     }
 
 ```
 
 That's all!
@@ -178,15 +182,15 @@
 app = inject_app(FastAPI())
 
 injector.bind({MyInterface: MyInterfaceImplementation})
 
 
 
 @app.get(path="/hello-world")
-def hello_world(service: Provide(MyInterface)) -> dict:
+def hello_world(service: Provide[MyInterface]) -> dict:
     return {
         "result": service.do_something(),
     }
 ```
 
 Using `injector.bind`, you can bind implementations that will be injected everywhere the bound interface is used.
```

