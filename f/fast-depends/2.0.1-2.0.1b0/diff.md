# Comparing `tmp/fast_depends-2.0.1.tar.gz` & `tmp/fast_depends-2.0.1b0.tar.gz`

## Comparing `fast_depends-2.0.1.tar` & `fast_depends-2.0.1b0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/__init__.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/_compat.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/use.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/core/build.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.1/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.1/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.1/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.1/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.1/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.1/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.1/README.md
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 fast_depends-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 fast_depends-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/_compat.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/types.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/use.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/build.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/README.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/PKG-INFO
```

### Comparing `fast_depends-2.0.1/CONTRIBUTING.md` & `fast_depends-2.0.1b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/.github/workflows/documentation.yml` & `fast_depends-2.0.1b0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.1b0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.1b0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/.github/workflows/tests.yml` & `fast_depends-2.0.1b0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/fast_depends/utils.py` & `fast_depends-2.0.1b0/fast_depends/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 import functools
 import inspect
 from contextlib import AsyncExitStack, ExitStack, asynccontextmanager, contextmanager
 from typing import (
     Any,
     AsyncGenerator,
-    Awaitable,
     Callable,
     ContextManager,
     Dict,
     ForwardRef,
     Iterable,
     List,
     Tuple,
-    Union,
-    cast,
 )
 
 import anyio
 from typing_extensions import ParamSpec, TypeVar
 
 from fast_depends._compat import evaluate_forwardref
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-async def run_async(
-    func: Union[
-        Callable[P, T],
-        Callable[P, Awaitable[T]],
-    ],
-    *args: P.args,
-    **kwargs: P.kwargs,
-) -> T:
+async def run_async(func: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> T:
     if is_coroutine_callable(func):
-        return await cast(Callable[P, Awaitable[T]], func)(*args, **kwargs)
+        return await func(*args, **kwargs)
     else:
-        return await run_in_threadpool(cast(Callable[P, T], func), *args, **kwargs)
+        return await run_in_threadpool(func, *args, **kwargs)
 
 
 async def run_in_threadpool(
     func: Callable[P, T], *args: P.args, **kwargs: P.kwargs
 ) -> T:
     if kwargs:  # pragma: no cover
         func = functools.partial(func, **kwargs)
@@ -61,15 +51,15 @@
     *, call: Callable[..., Any], stack: ExitStack, **sub_values: Any
 ) -> Any:
     cm = contextmanager(call)(**sub_values)
     return stack.enter_context(cm)
 
 
 def args_to_kwargs(
-    arguments: Iterable[str], *args: Any, **kwargs: Any
+    arguments: Iterable[str], *args: P.args, **kwargs: P.kwargs
 ) -> Dict[str, Any]:
     if not args:
         return kwargs
 
     unused = filter(lambda x: x not in kwargs, arguments)
 
     return dict((*zip(unused, args), *kwargs.items()))
```

### Comparing `fast_depends-2.0.1/fast_depends/core/build.py` & `fast_depends-2.0.1b0/fast_depends/core/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,43 @@
 import inspect
-from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Optional
 
-from typing_extensions import (
-    Annotated,
-    ParamSpec,
-    TypeVar,
-    assert_never,
-    get_args,
-    get_origin,
-)
+from typing_extensions import Annotated, assert_never, get_args, get_origin
 
 from fast_depends._compat import create_model
 from fast_depends.core.model import CallModel
 from fast_depends.dependencies import Depends
 from fast_depends.library import CustomField
 from fast_depends.utils import get_typed_signature, is_coroutine_callable
 
 CUSTOM_ANNOTATIONS = (Depends, CustomField)
 
 
-P = ParamSpec("P")
-T = TypeVar("T")
-
-
 def build_call_model(
-    call: Union[
-        Callable[P, T],
-        Callable[P, Awaitable[T]],
-    ],
+    call: Callable[..., Any],
     *,
     cast: bool = True,
     use_cache: bool = True,
     is_sync: Optional[bool] = None,
-) -> CallModel[P, T]:
+) -> CallModel:
     name = getattr(call, "__name__", type(call).__name__)
 
     is_call_async = is_coroutine_callable(call)
     if is_sync is None:
         is_sync = not is_call_async
     else:
         assert not (
             is_sync and is_call_async
         ), f"You cannot use async dependency `{name}` at sync main"
 
     typed_params, return_annotation = get_typed_signature(call)
 
-    class_fields: Dict[str, Tuple[Any, Any]] = {}
-    dependencies: Dict[str, CallModel[..., Any]] = {}
-    custom_fields: Dict[str, CustomField] = {}
+    class_fields = {}
+    dependencies = {}
+    custom_fields = {}
     for param in typed_params:
         dep: Optional[Depends] = None
         custom: Optional[CustomField] = None
 
         if param.annotation is inspect._empty:
             annotation = Any
 
@@ -78,44 +64,29 @@
                 annotation = type_annotation
             else:
                 annotation = param.annotation
         else:
             annotation = param.annotation
 
         default = param.default
-        if isinstance(default, Depends):
-            assert (
-                not dep
-            ), "You can not use `Depends` with `Annotated` and default both"
-            dep = default
-
-        elif isinstance(default, CustomField):
-            assert (
-                not custom
-            ), "You can not use `CustomField` with `Annotated` and default both"
-            custom = default
+        if dep or isinstance(default, Depends):
+            dep = dep or default
 
-        elif default is inspect._empty:
-            class_fields[param.name] = (annotation, ...)
-
-        else:
-            class_fields[param.name] = (annotation, default)
-
-        if dep:
             dependencies[param.name] = build_call_model(
                 dep.call,
                 cast=dep.cast,
                 use_cache=dep.use_cache,
                 is_sync=is_sync,
             )
 
             if dep.cast is True:
                 class_fields[param.name] = (annotation, ...)
 
-        if custom:
+        elif custom or isinstance(default, CustomField):
+            custom = custom or default
             assert not (
                 is_sync and is_coroutine_callable(custom.use)
             ), f"You cannot use async custom field `{type(custom).__name__}` at sync `{name}`"
 
             custom.set_param_name(param.name)
             custom_fields[param.name] = custom
 
@@ -123,23 +94,29 @@
                 annotation = Any
 
             if custom.required:
                 class_fields[param.name] = (annotation, ...)
             else:
                 class_fields[param.name] = (Optional[annotation], None)
 
-    func_model = create_model(name, **class_fields)  # type: ignore
+        elif default is inspect._empty:
+            class_fields[param.name] = (annotation, ...)
+
+        else:
+            class_fields[param.name] = (annotation, default)
 
     if cast and return_annotation is not inspect._empty:
         response_model = create_model(
             "ResponseModel", response=(return_annotation, ...)
         )
     else:
         response_model = None
 
+    func_model = create_model(name, **class_fields)
+
     return CallModel(
         call=call,
         model=func_model,
         response_model=response_model,
         cast=cast,
         use_cache=use_cache,
         is_async=is_call_async,
```

### Comparing `fast_depends-2.0.1/fast_depends/core/model.py` & `fast_depends-2.0.1b0/fast_depends/core/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from contextlib import AsyncExitStack, ExitStack
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generator,
-    Generic,
     List,
     Optional,
     Set,
     Type,
     Union,
 )
 
-from typing_extensions import ParamSpec, TypeVar, assert_never
+from typing_extensions import ParamSpec, TypeVar
 
 from fast_depends._compat import PYDANTIC_V2, BaseModel
 from fast_depends.library import CustomField
 from fast_depends.utils import (
     args_to_kwargs,
     is_async_gen_callable,
     is_coroutine_callable,
@@ -27,35 +26,35 @@
     solve_generator_sync,
 )
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-class CallModel(Generic[P, T]):
+class CallModel:
     call: Union[
         Callable[P, T],
         Callable[P, Awaitable[T]],
     ]
     is_async: bool
     is_generator: bool
     model: Type[BaseModel]
     response_model: Optional[Type[BaseModel]]
     arguments: List[str]
     alias_arguments: List[str]
 
-    dependencies: Dict[str, "CallModel[..., Any]"]
+    dependencies: Dict[str, "CallModel"]
     custom_fields: Dict[str, CustomField]
 
     # Dependencies and custom fields
     use_cache: bool
     cast: bool
 
     @property
-    def call_name(self) -> str:
+    def call_name(self):
         return getattr(self.call, "__name__", type(self.call).__name__)
 
     @property
     def real_params(self) -> Set[str]:
         return set(self.arguments) - set(self.dependencies.keys())
 
     @property
@@ -67,33 +66,33 @@
 
     def __init__(
         self,
         call: Union[
             Callable[P, T],
             Callable[P, Awaitable[T]],
         ],
-        model: Type[BaseModel],
+        model: BaseModel,
         response_model: Optional[Type[BaseModel]] = None,
         use_cache: bool = True,
         cast: bool = True,
         is_async: bool = False,
-        dependencies: Optional[Dict[str, "CallModel[..., Any]"]] = None,
+        dependencies: Optional[Dict[str, "CallModel"]] = None,
         custom_fields: Optional[Dict[str, CustomField]] = None,
     ):
         self.call = call
         self.model = model
         self.response_model = response_model
 
         self.arguments = []
         self.alias_arguments = []
 
         if PYDANTIC_V2:
             fields = self.model.model_fields
         else:  # pragma: no cover
-            fields = self.model.__fields__  # type: ignore[assignment]
+            fields = self.model.__fields__
 
         for name, f in fields.items():
             self.arguments.append(name)
             self.alias_arguments.append(f.alias or name)
 
         self.dependencies = dependencies or {}
         self.custom_fields = custom_fields or {}
@@ -101,107 +100,57 @@
         self.use_cache = use_cache
         self.cast = cast
         self.is_async = is_async or is_coroutine_callable(call)
         self.is_generator = is_gen_callable(self.call) or is_async_gen_callable(
             self.call
         )
 
-    def _solve(
+    def _cast_args(
         self,
         *args: P.args,
-        cache_dependencies: Dict[
-            Union[
-                Callable[P, T],
-                Callable[P, Awaitable[T]],
-            ],
-            T,
-        ],
-        dependency_overrides: Optional[
-            Dict[
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-            ]
-        ] = None,
         **kwargs: P.kwargs,
-    ) -> Generator[Dict[str, Any], Any, T]:
-        if dependency_overrides:
-            self.call = dependency_overrides.get(self.call, self.call)
-            assert self.is_async or not is_coroutine_callable(
-                self.call
-            ), f"You cannot use async dependency `{self.call_name}` at sync main"
-
-        if self.use_cache and self.call in cache_dependencies:
-            return cache_dependencies[self.call]
-
+    ) -> Generator[Dict[str, Any], Any, T,]:
         kw = args_to_kwargs(self.alias_arguments, *args, **kwargs)
 
-        solved_kw: Dict[str, Any]
-        solved_kw = yield kw
+        kw_with_solved_dep = yield kw
 
-        casted_model = self.model(**solved_kw)
+        casted_model = self.model(**kw_with_solved_dep)
 
         casted_kw = {
-            arg: getattr(casted_model, arg, solved_kw.get(arg))
+            arg: getattr(casted_model, arg, kw_with_solved_dep.get(arg))
             for arg in (*self.arguments, *self.dependencies.keys())
         }
 
-        response: T
         response = yield casted_kw
 
         if self.cast is True and self.response_model is not None:
             casted_resp = self.response_model(response=response)
-            response = casted_resp.response  # type: ignore
-
-        if self.use_cache:  # pragma: no branch
-            cache_dependencies[self.call] = response
+            response = casted_resp.response
 
         return response
 
     def solve(
         self,
         *args: P.args,
         stack: ExitStack,
-        cache_dependencies: Dict[
-            Union[
-                Callable[P, T],
-                Callable[P, Awaitable[T]],
-            ],
-            T,
-        ],
-        dependency_overrides: Optional[
-            Dict[
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-            ]
-        ] = None,
+        cache_dependencies: Dict[str, Any],
+        dependency_overrides: Optional[Dict[Callable[..., Any], Any]] = None,
         **kwargs: P.kwargs,
     ) -> T:
-        cast_gen = self._solve(
-            *args,
-            cache_dependencies=cache_dependencies,
-            dependency_overrides=dependency_overrides,
-            **kwargs,
-        )
-        try:
-            kwargs = next(cast_gen)
-        except StopIteration as e:
-            cached_value: T = e.value
-            return cached_value
+        if dependency_overrides:
+            self.call = dependency_overrides.get(self.call, self.call)
+            assert not is_coroutine_callable(
+                self.call
+            ), f"You cannot use async dependency `{self.call_name}` at sync main"
+
+        if self.use_cache and cache_dependencies.get(self.call):
+            return cache_dependencies.get(self.call)
+
+        cast_gen = self._cast_args(*args, **kwargs)
+        kwargs = next(cast_gen)
 
         for dep_arg, dep in self.dependencies.items():
             kwargs[dep_arg] = dep.solve(
                 stack=stack,
                 cache_dependencies=cache_dependencies,
                 dependency_overrides=dependency_overrides,
                 **kwargs,
@@ -220,55 +169,34 @@
             )
         else:
             response = self.call(**final_kw)
 
         try:
             cast_gen.send(response)
         except StopIteration as e:
-            value: T = e.value
-            return value
-
-        assert_never(response)  # pragma: no cover
+            if self.use_cache:  # pragma: no branch
+                cache_dependencies[self.call] = e.value
+            return e.value
 
     async def asolve(
         self,
         *args: P.args,
         stack: AsyncExitStack,
-        cache_dependencies: Dict[
-            Union[
-                Callable[P, T],
-                Callable[P, Awaitable[T]],
-            ],
-            T,
-        ],
-        dependency_overrides: Optional[
-            Dict[
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-                Union[
-                    Callable[P, T],
-                    Callable[P, Awaitable[T]],
-                ],
-            ]
-        ] = None,
+        cache_dependencies: Dict[str, Any],
+        dependency_overrides: Optional[Dict[Callable[..., Any], Any]] = None,
         **kwargs: P.kwargs,
     ) -> T:
-        cast_gen = self._solve(
-            *args,
-            cache_dependencies=cache_dependencies,
-            dependency_overrides=dependency_overrides,
-            **kwargs,
-        )
-        try:
-            kwargs = next(cast_gen)
-        except StopIteration as e:
-            cached_value: T = e.value
-            return cached_value
+        if dependency_overrides:
+            self.call = dependency_overrides.get(self.call, self.call)
+
+        if self.use_cache and cache_dependencies.get(self.call):
+            return cache_dependencies.get(self.call)
+
+        cast_gen = self._cast_args(*args, **kwargs)
+        kwargs = next(cast_gen)
 
         for dep_arg, dep in self.dependencies.items():
             kwargs[dep_arg] = await dep.asolve(
                 stack=stack,
                 cache_dependencies=cache_dependencies,
                 dependency_overrides=dependency_overrides,
                 **kwargs,
@@ -283,15 +211,13 @@
             response = await solve_generator_async(
                 call=self.call,
                 stack=stack,
                 **final_kw,
             )
         else:
             response = await run_async(self.call, **final_kw)
-
         try:
             cast_gen.send(response)
         except StopIteration as e:
-            value: T = e.value
-            return value
-
-        assert_never(response)  # pragma: no cover
+            if self.use_cache:  # pragma: no branch
+                cache_dependencies[self.call] = e.value
+            return e.value
```

### Comparing `fast_depends-2.0.1/fast_depends/dependencies/model.py` & `fast_depends-2.0.1b0/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/fast_depends/library/model.py` & `fast_depends-2.0.1b0/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/LICENSE` & `fast_depends-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/README.md` & `fast_depends-2.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.1/pyproject.toml` & `fast_depends-2.0.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "pydantic>=1.10",
+    "pydantic==2.0b3",
     "anyio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://lancetnik.github.io/FastDepends/"
@@ -138,16 +138,15 @@
     "E501",  # line too long, handled by black
     "C901",  # too complex
 ]
 
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = [
     "fast_depends.Depends",
-    "AsyncHeader", "Header", "MyDep",
-    "pydantic.Field",
+    "AsyncHeader", "Header", "MyDep"
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q"
 testpaths = [
     "tests",
```

### Comparing `fast_depends-2.0.1/PKG-INFO` & `fast_depends-2.0.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.1
+Version: 2.0.1b0
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: anyio
-Requires-Dist: pydantic>=1.10
+Requires-Dist: pydantic==2.0b3
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: fast-depends[doc]; extra == 'dev'
 Requires-Dist: fast-depends[test]; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy>=1.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.260; extra == 'dev'
```

