# Comparing `tmp/configzen-0.3.7.tar.gz` & `tmp/configzen-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.7.tar", max compression
+gzip compressed data, was "configzen-0.3.8.tar", max compression
```

## Comparing `configzen-0.3.7.tar` & `configzen-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.7/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.7/configzen/__main__.py
--rw-r--r--   0        0        0    67816 2023-06-15 18:54:00.040515 configzen-0.3.7/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.7/configzen/decorators.py
--rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.7/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.7/configzen/field.py
--rw-r--r--   0        0        0    26185 2023-06-15 21:21:22.530453 configzen-0.3.7/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.7/configzen/py.typed
--rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.7/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.7/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.7/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-15 21:21:53.913600 configzen-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.7/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.8/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.8/configzen/__main__.py
+-rw-r--r--   0        0        0    69360 2023-06-21 19:39:30.254748 configzen-0.3.8/configzen/config.py
+-rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.8/configzen/decorators.py
+-rw-r--r--   0        0        0     3635 2023-06-21 19:36:00.617371 configzen-0.3.8/configzen/errors.py
+-rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.8/configzen/field.py
+-rw-r--r--   0        0        0    26257 2023-06-21 19:40:28.209184 configzen-0.3.8/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.8/configzen/py.typed
+-rw-r--r--   0        0        0     4686 2023-06-21 19:36:00.610371 configzen-0.3.8/configzen/route.py
+-rw-r--r--   0        0        0     1124 2023-06-21 19:40:00.222571 configzen-0.3.8/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1255 2023-06-21 19:42:27.934760 configzen-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.8/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.8/PKG-INFO
```

### Comparing `configzen-0.3.7/configzen/__init__.py` & `configzen-0.3.8/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/configzen/__main__.py` & `configzen-0.3.8/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/configzen/config.py` & `configzen-0.3.8/configzen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,18 @@
     no_type_check,
     overload,
 )
 
 import anyconfig
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
-from pydantic.fields import (
-    ModelField,  # type: ignore[attr-defined]
+from pydantic.fields import (  # type: ignore[attr-defined]
+    ModelField,
     make_generic_validator,
+    Undefined
 )
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
 from configzen.errors import (
     ConfigAccessError,
@@ -136,15 +137,15 @@
 ) - {""}
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
-] = contextvars.ContextVar("current_context", default=None)
+    ] = contextvars.ContextVar("current_context", default=None)
 
 _exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
     "_exporting", default=False
 )
 
 
 def _get_defaults_from_model_class(
@@ -1160,27 +1161,42 @@
         The route to the item.
     """
 
     owner: ConfigModelT
     mapping: dict[str, Any] | None
     route: SupportsRoute
 
-    def get(self) -> Any:
+    def get(self, route: SupportsRoute | None = None, default: Any = Undefined) -> Any:
         """
         Get the value of the item.
 
+        Parameters
+        ----------
+        route
+            The route to the item. If not given, the sole route of this item is used.
+            If given, the route is appended to the sole route of this item.
+        default
+            The default value to return if the item is not found.
+
         Returns
         -------
         The value of the item.
         """
+        base_route = ConfigRoute(self.route)
+        if route is None:
+            route = base_route
+        else:
+            route = base_route.enter(ConfigRoute(route, allow_empty=True))
         try:
-            scope = at(self.mapping or self.owner, self.route)
-        except KeyError as err:
-            route_here = err.args[1]
-            raise ConfigAccessError(self.owner, route_here) from None
+            scope = at(self.mapping or self.owner, route)
+        except ResourceLookupError as err:
+            if default is Undefined:
+                route_here = err.route
+                raise ConfigAccessError(self.owner, route_here) from None
+            scope = default
         return scope
 
     def update(self, value: Any) -> Any:
         """
         Update the value of the item with regard to this item mapping.
 
         Parameters
@@ -1566,15 +1582,15 @@
     def trace_route(self) -> collections.abc.Iterator[str]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
     def at(self) -> ConfigAt[ConfigModelT]:
         if self.owner is None:
-            msg = "Cannot get section pointed to by an unbound context"
+            msg = "Cannot get at() of a model without parent model"
             raise ValueError(msg)
         return ConfigAt(self.owner, None, self.route)
 
     @property
     def owner(self) -> ConfigModelT | None:
         return self._parent.owner
 
@@ -1682,18 +1698,17 @@
     root=True,
 ):
     """The base class for configuration models."""
 
     def __init__(self, **kwargs: Any) -> None:
         # Set private attributes via the constructor
         # to allow preprocessor-related instances to exist.
-        missing = object()
         for private_attr in self.__private_attributes__:
-            value = kwargs.pop(private_attr, missing)
-            if value is not missing:
+            value = kwargs.pop(private_attr, Undefined)
+            if value is not Undefined:
                 setattr(self, private_attr, value)
                 if private_attr == CONTEXT:
                     current_context.set(value)
         super().__init__(**kwargs)
 
     def _init_private_attributes(self) -> None:
         super()._init_private_attributes()
@@ -1855,31 +1870,68 @@
         It is a copy of the configuration state
         at the last time of loading, reloading or saving.
         """
         return get_context(self).initial_state
 
     def at(
         self: ConfigModelT,
-        route: SupportsRoute,
-    ) -> ConfigAt[ConfigModelT]:
+        route: SupportsRoute | None = None,
+    ) -> ConfigModelT | ConfigAt[ConfigModelT]:
         """
         Lazily point to a specific item in the configuration.
 
         Parameters
         ----------
         route
             The access route to the item in this configuration.
+            If None, the whole configuration is returned.
 
         Returns
         -------
         The configuration accessor.
         """
+        if route is None:
+            return self
         return ConfigAt(self, None, route)
 
-    def update(self, **kwargs: Any) -> None:
+    @overload
+    def get(
+        self: ConfigModelT,
+        route: None = None,
+        default: Any = ...
+    ) -> ConfigModelT:
+        ...
+
+    @overload
+    def get(
+        self: ConfigModelT,
+        route: SupportsRoute = ...,
+        default: Any = ...
+    ) -> Any:
+        ...
+
+    def get(
+        self,
+        route: SupportsRoute | None = None,
+        default: Any = Undefined
+    ) -> Any:
+        """
+        Get a value from the configuration.
+
+        Parameters
+        ----------
+        route
+            Route to access the item. If None, the whole configuration is returned.
+        default
+        """
+        if route is None:
+            return self
+        return self.at(route).get(default=default)
+
+    def update(self, kwargs: dict[str, Any]) -> None:
         """
         Update the configuration with new values, in-place.
 
         Parameters
         ----------
         kwargs
             The new values to update the configuration with.
@@ -1985,15 +2037,15 @@
         if context.owner is self:
             changed = context.agent.read(config_class=type(self), **kwargs)
         else:
             changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
         current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
-        self.update(**state)
+        self.update(state)
         return self
 
     def save(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file.
@@ -2109,15 +2161,15 @@
         else:
             changed = await reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
         current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
-        self.update(**state)
+        self.update(state)
         return self
 
     async def save_async(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file asynchronously.
```

### Comparing `configzen-0.3.7/configzen/decorators.py` & `configzen-0.3.8/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/configzen/errors.py` & `configzen-0.3.8/configzen/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,12 +100,13 @@
 class ResourceLookupError(ConfigError, LookupError):
     """An error occurred while looking up a resource."""
 
     def __init__(
         self, resource: ConfigAgent[ConfigModelT] | None, route: list[str]
     ) -> None:
         resource_name = resource.resource if resource else "the provided resource"
+        self.route = route
         super().__init__(f"{route} not found in {resource_name}")
 
 
 class ConfigPreprocessingError(ConfigProcessorError, ValueError):
     """An error occurred while preprocessing a configuration value."""
```

### Comparing `configzen-0.3.7/configzen/field.py` & `configzen-0.3.8/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/configzen/processor.py` & `configzen-0.3.8/configzen/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import copy
 import dataclasses
 import enum
 import pathlib
 from collections.abc import Callable
+from pydantic.fields import Undefined
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import ConfigPreprocessingError
 from configzen.typedefs import ConfigModelT, SupportsRoute
 
@@ -92,15 +93,15 @@
 
 
 def parse_directive_call(
     prefix: str,
     directive_name: str,
 ) -> str:
     if directive_name.startswith(prefix):
-        directive_name = directive_name[len(prefix) :].casefold()
+        directive_name = directive_name[len(prefix):].casefold()
 
         if not directive_name.isidentifier():
             msg = f"Invalid directive name: {directive_name}"
             raise ConfigPreprocessingError(msg)
 
     return directive_name
 
@@ -649,15 +650,15 @@
                     context=context,
                     preprocess=preprocess,
                     key_order=list(ctx.container),
                 ),
             }
 
     @classmethod
-    def _export(
+    def _export(  # noqa: C901
         cls,
         state: dict[str, Any],
         metadata: ExportMetadata[ConfigModelT],
     ) -> None:
         """
         Exports model state preserving substition directive calls in the model state.
 
@@ -680,31 +681,30 @@
             loaded = agent.load_dict(reader.read())
 
             if route:
                 loaded = at(loaded, route, agent=agent)
 
         substituted_values = loaded.copy()
 
-        missing = object()
-
         for key, value in loaded.items():
-            counterpart_value = state.pop(key, missing)
-            if counterpart_value is missing:
+            counterpart_value = state.pop(key, Undefined)
+            if counterpart_value is Undefined:
                 continue
             counterpart_value = pre_serialize(counterpart_value)
 
             if is_dict_like(value):
                 if EXPORT in value:
                     value.pop(CONTEXT, None)
                     cls.export(value, metadata=value.pop(EXPORT))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
-                        (orig := value.get(sub_key, missing)) is missing or orig != comp
+                        (orig := value.get(sub_key, Undefined))
+                        is Undefined or orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
@@ -725,15 +725,15 @@
             overrides=overrides,
             values=substituted_values,
             route=route,
             key_order=key_order,
         )
 
     @classmethod
-    async def _export_async(
+    async def _export_async(  # noqa: C901
         cls,
         state: dict[str, Any],
         metadata: ExportMetadata[ConfigModelT],
     ) -> None:
         """
         Exports model state preserving substition directive calls in the model state.
 
@@ -756,31 +756,30 @@
             loaded = await agent.load_dict_async(await reader.read())
 
             if route:
                 loaded = at(loaded, route, agent=agent)
 
         substituted_values = loaded.copy()
 
-        missing = object()
-
         for key, value in loaded.items():
-            counterpart_value = state.pop(key, missing)
-            if counterpart_value is missing:
+            counterpart_value = state.pop(key, Undefined)
+            if counterpart_value is Undefined:
                 continue
             counterpart_value = pre_serialize(counterpart_value)
 
             if is_dict_like(value):
                 if EXPORT in value:
                     value.pop(CONTEXT, None)
                     await cls.export_async(value, metadata=value.pop(EXPORT))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
-                        (orig := value.get(sub_key, missing)) is missing or orig != comp
+                        (orig := value.get(sub_key, Undefined))
+                        is Undefined or orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
```

### Comparing `configzen-0.3.7/configzen/route.py` & `configzen-0.3.8/configzen/route.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,41 +14,44 @@
 
 class ConfigRoute:
     TOK_DOT: ClassVar[str] = "."
     TOK_ESCAPE: ClassVar[str] = "\\"
     TOK_DOTLISTESC_ENTER: ClassVar[str] = "["
     TOK_DOTLISTESC_EXIT: ClassVar[str] = "]"
 
-    def __init__(self, route: SupportsRoute) -> None:
-        self.list_route = self.parse(route)
+    def __init__(self, route: SupportsRoute, *, allow_empty: bool = False) -> None:
+        items = self.parse(route)
+        if not (allow_empty or items):
+            raise ValueError("Empty configuration route")
+        self.items = items
 
     @classmethod
     def parse(cls, route: SupportsRoute) -> list[str]:
         if isinstance(route, ConfigRoute):
-            return route.list_route
+            return route.items
         if isinstance(route, list):
             return route
         if isinstance(route, str):
             with formatted_syntax_error(route):
                 return cls._decompose(route)
-        raise TypeError(f"invalid route type {type(route)!r}")
+        raise TypeError(f"Invalid route type {type(route)!r}")
 
     @classmethod
     def _decompose(cls, route: str) -> list[str]:  # noqa: C901, PLR0912
         tok_dot = cls.TOK_DOT
         tok_escape = cls.TOK_ESCAPE
         tok_dle_enter = cls.TOK_DOTLISTESC_ENTER
         tok_dle_exit = cls.TOK_DOTLISTESC_EXIT
 
         route = route.removesuffix(tok_dot) + tok_dot
 
         part = ""
         dle_ctx = None
-        list_route: list[str] = []
-        enter = list_route.append
+        items: list[str] = []
+        enter = items.append
         error = functools.partial(InternalSyntaxError, prefix="Route(", suffix=")")
         escape = False
 
         for index, char in enumerate(route):
             if escape:
                 part += char
                 escape = False
@@ -87,15 +90,15 @@
                 part += char
             if is_last and dle_ctx is not None:
                 msg = (
                     "Unclosed dotlist escape sequence "
                     f"(expected {tok_dle_exit!r} token)"
                 )
                 raise error(msg, index=dle_ctx)
-        return list_route
+        return items
 
     @classmethod
     def decompose(cls, route: str) -> list[str]:
         with formatted_syntax_error(route):
             return cls._decompose(route)
 
     def compose(self) -> str:
@@ -104,30 +107,30 @@
         return self.TOK_DOT.join(
             fragment.join(escape).replace(
                 self.TOK_DOTLISTESC_EXIT + self.TOK_DOT,
                 self.TOK_DOTLISTESC_EXIT + self.TOK_ESCAPE + self.TOK_DOT,
             )
             if self.TOK_DOT in fragment
             else fragment.join(raw)
-            for fragment in self.list_route
+            for fragment in self.items
         )
 
     def enter(self, subroute: SupportsRoute) -> ConfigRoute:
-        return type(self)(self.list_route + self.parse(subroute))
+        return type(self)(self.items + self.parse(subroute))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, ConfigRoute):
-            return self.list_route == other.list_route
+            return self.items == other.items
         if isinstance(other, str):
-            return self.list_route == self.decompose(other)
+            return self.items == self.decompose(other)
         if isinstance(other, list):
-            return self.list_route == other
+            return self.items == other
         return NotImplemented
 
     def __str__(self) -> str:
         return self.compose()
 
     def __iter__(self) -> collections.abc.Iterator[str]:
-        yield from self.list_route
+        yield from self.items
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}({self.list_route})"
+        return f"{type(self).__name__}({self.items})"
```

### Comparing `configzen-0.3.7/configzen/typedefs.py` & `configzen-0.3.8/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/LICENSE` & `configzen-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/pyproject.toml` & `configzen-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.3.7"
+version = "0.3.8"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.3.7/README.md` & `configzen-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.3.7/PKG-INFO` & `configzen-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.3.7
+Version: 0.3.8
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

