# Comparing `tmp/typing_extensions-4.6.3.tar.gz` & `tmp/typing_extensions-4.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typing_extensions-4.7.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.6.3.tar` & `typing_extensions-4.7.0rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11557 2023-06-01 23:39:03.206669 typing_extensions-4.6.3/CHANGELOG.md
--rw-r--r--   0        0        0    13936 2023-06-01 23:37:58.110406 typing_extensions-4.6.3/LICENSE
--rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.3/README.md
--rw-r--r--   0        0        0     1916 2023-06-01 23:39:19.239989 typing_extensions-4.6.3/pyproject.toml
--rw-r--r--   0        0        0      426 2023-05-27 00:24:46.431541 typing_extensions-4.6.3/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   174623 2023-06-01 23:37:58.216239 typing_extensions-4.6.3/src/test_typing_extensions.py
--rw-r--r--   0        0        0   104335 2023-06-01 23:37:58.217871 typing_extensions-4.6.3/src/typing_extensions.py
--rw-r--r--   0        0        0      135 2023-06-01 23:37:57.995967 typing_extensions-4.6.3/tox.ini
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.3/PKG-INFO
+-rw-r--r--   0        0        0    14528 2023-06-21 14:51:28.991627 typing_extensions-4.7.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    13936 2023-06-01 23:37:58.110406 typing_extensions-4.7.0rc1/LICENSE
+-rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.7.0rc1/README.md
+-rw-r--r--   0        0        0     1965 2023-06-21 14:51:28.993380 typing_extensions-4.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      563 2023-06-15 04:06:19.836805 typing_extensions-4.7.0rc1/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   202262 2023-06-21 14:51:28.994930 typing_extensions-4.7.0rc1/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   110420 2023-06-21 14:51:28.996059 typing_extensions-4.7.0rc1/src/typing_extensions.py
+-rw-r--r--   0        0        0      142 2023-06-01 23:56:14.224477 typing_extensions-4.7.0rc1/tox.ini
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 typing_extensions-4.7.0rc1/PKG-INFO
```

### Comparing `typing_extensions-4.6.3/CHANGELOG.md` & `typing_extensions-4.7.0rc1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,56 @@
+# Release 4.7.0rc1 (June 21, 2023)
+
+- Add `typing_extensions.get_protocol_members` and
+  `typing_extensions.is_protocol` (backport of CPython PR #104878).
+  Patch by Jelle Zijlstra.
+- `typing_extensions` now re-exports all names in the standard library's
+  `typing` module, except the deprecated `ByteString`. Patch by Jelle
+  Zijlstra.
+- Due to changes in the implementation of `typing_extensions.Protocol`,
+  `typing.runtime_checkable` can now be used on `typing_extensions.Protocol`
+  (previously, users had to use `typing_extensions.runtime_checkable` if they
+  were using `typing_extensions.Protocol`).
+- Align the implementation of `TypedDict` with the implementation in the
+  standard library on Python 3.9 and higher.
+  `typing_extensions.TypedDict` is now a function instead of a class. The
+  private functions `_check_fails`, `_dict_new`, and `_typeddict_new`
+  have been removed. `is_typeddict` now returns `False` when called with
+  `TypedDict` itself as the argument. Patch by Jelle Zijlstra.
+- Declare support for Python 3.12. Patch by Jelle Zijlstra.
+- Fix tests on Python 3.13, which removes support for creating
+  `TypedDict` classes through the keyword-argument syntax. Patch by
+  Jelle Zijlstra.
+- Fix a regression introduced in v4.6.3 that meant that
+  ``issubclass(object, typing_extensions.Protocol)`` would erroneously raise
+  ``TypeError``. Patch by Alex Waygood (backporting the CPython PR
+  https://github.com/python/cpython/pull/105239).
+- Allow `Protocol` classes to inherit from `typing_extensions.Buffer` or
+  `collections.abc.Buffer`. Patch by Alex Waygood (backporting
+  https://github.com/python/cpython/pull/104827, by Jelle Zijlstra).
+- Allow classes to inherit from both `typing.Protocol` and `typing_extensions.Protocol`
+  simultaneously. Since v4.6.0, this caused `TypeError` to be raised due to a
+  metaclass conflict. Patch by Alex Waygood.
+- Backport several deprecations from CPython relating to unusual ways to
+  create `TypedDict`s and `NamedTuple`s. CPython PRs #105609 and #105780
+  by Alex Waygood; `typing_extensions` backport by Jelle Zijlstra.
+  - Creating a `NamedTuple` using the functional syntax with keyword arguments
+    (`NT = NamedTuple("NT", a=int)`) is now deprecated.
+  - Creating a `NamedTuple` with zero fields using the syntax `NT = NamedTuple("NT")`
+    or `NT = NamedTuple("NT", None)` is now deprecated.
+  - Creating a `TypedDict` with zero fields using the syntax `TD = TypedDict("TD")`
+    or `TD = TypedDict("TD", None)` is now deprecated.
+- Fix bug on Python 3.7 where a protocol `X` that had a member `a` would not be
+  considered an implicit subclass of an unrelated protocol `Y` that only has a
+  member `a`. Where the members of `X` are a superset of the members of `Y`,
+  `X` should always be considered a subclass of `Y` iff `Y` is a
+  runtime-checkable protocol that only has callable members. Patch by Alex
+  Waygood (backporting CPython PR
+  https://github.com/python/cpython/pull/105835).
+
 # Release 4.6.3 (June 1, 2023)
 
 - Fix a regression introduced in v4.6.0 in the implementation of
   runtime-checkable protocols. The regression meant
   that doing `class Foo(X, typing_extensions.Protocol)`, where `X` was a class that
   had `abc.ABCMeta` as its metaclass, would then cause subsequent
   `isinstance(1, X)` calls to erroneously raise `TypeError`. Patch by
```

### Comparing `typing_extensions-4.6.3/LICENSE` & `typing_extensions-4.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.3/README.md` & `typing_extensions-4.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.3/pyproject.toml` & `typing_extensions-4.7.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.6.3"
+version = "4.7.0rc1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
@@ -35,14 +35,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
 ]
 
 [project.urls]
 Home = "https://github.com/python/typing_extensions"
 Repository = "https://github.com/python/typing_extensions"
 Changes = "https://github.com/python/typing_extensions/blob/main/CHANGELOG.md"
```

### Comparing `typing_extensions-4.6.3/src/test_typing_extensions.py` & `typing_extensions-4.7.0rc1/src/test_typing_extensions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import abc
+import gc
 import io
 import contextlib
 import collections
 from collections import defaultdict
 import collections.abc
 import copy
 from functools import lru_cache
@@ -32,29 +33,33 @@
 from typing_extensions import TypeAlias, ParamSpec, Concatenate, ParamSpecArgs, ParamSpecKwargs, TypeGuard
 from typing_extensions import Awaitable, AsyncIterator, AsyncContextManager, Required, NotRequired
 from typing_extensions import Protocol, runtime, runtime_checkable, Annotated, final, is_typeddict
 from typing_extensions import TypeVarTuple, Unpack, dataclass_transform, reveal_type, Never, assert_never, LiteralString
 from typing_extensions import assert_type, get_type_hints, get_origin, get_args, get_original_bases
 from typing_extensions import clear_overloads, get_overloads, overload
 from typing_extensions import NamedTuple
-from typing_extensions import override, deprecated, Buffer, TypeAliasType, TypeVar
-from _typed_dict_test_helper import Foo, FooGeneric
+from typing_extensions import override, deprecated, Buffer, TypeAliasType, TypeVar, get_protocol_members, is_protocol
+from _typed_dict_test_helper import Foo, FooGeneric, VeryAnnotated
 
 # Flags used to mark tests that only apply after a specific
 # version of the typing module.
 TYPING_3_8_0 = sys.version_info[:3] >= (3, 8, 0)
 TYPING_3_9_0 = sys.version_info[:3] >= (3, 9, 0)
 TYPING_3_10_0 = sys.version_info[:3] >= (3, 10, 0)
 
 # 3.11 makes runtime type checks (_type_check) more lenient.
 TYPING_3_11_0 = sys.version_info[:3] >= (3, 11, 0)
 
 # 3.12 changes the representation of Unpack[] (PEP 692)
 TYPING_3_12_0 = sys.version_info[:3] >= (3, 12, 0)
 
+only_with_typing_Protocol = skipUnless(
+    hasattr(typing, "Protocol"), "Only relevant when typing.Protocol exists"
+)
+
 # https://github.com/python/cpython/pull/27017 was backported into some 3.9 and 3.10
 # versions, but not all
 HAS_FORWARD_MODULE = "module" in inspect.signature(typing._type_check).parameters
 
 ANN_MODULE_SOURCE = '''\
 from typing import Optional
 from functools import wraps
@@ -1143,18 +1148,34 @@
     title: str
     year: NotRequired[int]
 
 class NontotalMovie(TypedDict, total=False):
     title: Required[str]
     year: int
 
+class ParentNontotalMovie(TypedDict, total=False):
+    title: Required[str]
+
+class ChildTotalMovie(ParentNontotalMovie):
+    year: NotRequired[int]
+
+class ParentDeeplyAnnotatedMovie(TypedDict):
+    title: Annotated[Annotated[Required[str], "foobar"], "another level"]
+
+class ChildDeeplyAnnotatedMovie(ParentDeeplyAnnotatedMovie):
+    year: NotRequired[Annotated[int, 2000]]
+
 class AnnotatedMovie(TypedDict):
     title: Annotated[Required[str], "foobar"]
     year: NotRequired[Annotated[int, 2000]]
 
+class WeirdlyQuotedMovie(TypedDict):
+    title: Annotated['Annotated[Required[str], "foobar"]', "another level"]
+    year: NotRequired['Annotated[int, 2000]']
+
 
 gth = get_type_hints
 
 
 class GetTypeHintTests(BaseTestCase):
     @classmethod
     def setUpClass(cls):
@@ -1316,32 +1337,26 @@
         self.assertNotIsInstance(1, collections.abc.Sized)
         with self.assertRaises(TypeError):
             isinstance(collections.deque(), typing_extensions.Deque[int])
         with self.assertRaises(TypeError):
             issubclass(collections.Counter, typing_extensions.Counter[str])
 
     def test_awaitable(self):
-        ns = {}
-        exec(
-            "async def foo() -> typing_extensions.Awaitable[int]:\n"
-            "    return await AwaitableWrapper(42)\n",
-            globals(), ns)
-        foo = ns['foo']
+        async def foo() -> typing_extensions.Awaitable[int]:
+            return await AwaitableWrapper(42)
+
         g = foo()
         self.assertIsInstance(g, typing_extensions.Awaitable)
         self.assertNotIsInstance(foo, typing_extensions.Awaitable)
         g.send(None)  # Run foo() till completion, to avoid warning.
 
     def test_coroutine(self):
-        ns = {}
-        exec(
-            "async def foo():\n"
-            "    return\n",
-            globals(), ns)
-        foo = ns['foo']
+        async def foo():
+            return
+
         g = foo()
         self.assertIsInstance(g, typing_extensions.Coroutine)
         with self.assertRaises(TypeError):
             isinstance(g, typing_extensions.Coroutine[int])
         self.assertNotIsInstance(foo, typing_extensions.Coroutine)
         try:
             g.send(None)
@@ -1453,18 +1468,18 @@
 
         d = MyCounter()
         self.assertIsInstance(d, MyCounter)
         self.assertIsInstance(d, collections.Counter)
         self.assertIsInstance(d, typing_extensions.Counter)
 
     def test_async_generator(self):
-        ns = {}
-        exec("async def f():\n"
-             "    yield 42\n", globals(), ns)
-        g = ns['f']()
+        async def f():
+            yield 42
+
+        g = f()
         self.assertIsSubclass(type(g), typing_extensions.AsyncGenerator)
 
     def test_no_async_generator_instantiation(self):
         with self.assertRaises(TypeError):
             typing_extensions.AsyncGenerator()
         with self.assertRaises(TypeError):
             typing_extensions.AsyncGenerator[T, T]()
@@ -1474,17 +1489,16 @@
     def test_subclassing_async_generator(self):
         class G(typing_extensions.AsyncGenerator[int, int]):
             def asend(self, value):
                 pass
             def athrow(self, typ, val=None, tb=None):
                 pass
 
-        ns = {}
-        exec('async def g(): yield 0', globals(), ns)
-        g = ns['g']
+        async def g(): yield 0
+
         self.assertIsSubclass(G, typing_extensions.AsyncGenerator)
         self.assertIsSubclass(G, typing_extensions.AsyncIterable)
         self.assertIsSubclass(G, collections.abc.AsyncGenerator)
         self.assertIsSubclass(G, collections.abc.AsyncIterable)
         self.assertNotIsSubclass(type(g), G)
 
         instance = G()
@@ -1753,30 +1767,91 @@
             class P(BP, C, Protocol):
                 pass
         class D(BP, C): pass
         class E(C, BP): pass
         self.assertNotIsInstance(D(), E)
         self.assertNotIsInstance(E(), D)
 
-    @skipUnless(
-        hasattr(typing, "Protocol"),
-        "Test is only relevant if typing.Protocol exists"
-    )
+    @only_with_typing_Protocol
     def test_runtimecheckable_on_typing_dot_Protocol(self):
         @runtime_checkable
         class Foo(typing.Protocol):
             x: int
 
         class Bar:
             def __init__(self):
                 self.x = 42
 
         self.assertIsInstance(Bar(), Foo)
         self.assertNotIsInstance(object(), Foo)
 
+    @only_with_typing_Protocol
+    def test_typing_dot_runtimecheckable_on_Protocol(self):
+        @typing.runtime_checkable
+        class Foo(Protocol):
+            x: int
+
+        class Bar:
+            def __init__(self):
+                self.x = 42
+
+        self.assertIsInstance(Bar(), Foo)
+        self.assertNotIsInstance(object(), Foo)
+
+    @only_with_typing_Protocol
+    def test_typing_Protocol_and_extensions_Protocol_can_mix(self):
+        class TypingProto(typing.Protocol):
+            x: int
+
+        class ExtensionsProto(Protocol):
+            y: int
+
+        class SubProto(TypingProto, ExtensionsProto, typing.Protocol):
+            z: int
+
+        class SubProto2(TypingProto, ExtensionsProto, Protocol):
+            z: int
+
+        class SubProto3(ExtensionsProto, TypingProto, typing.Protocol):
+            z: int
+
+        class SubProto4(ExtensionsProto, TypingProto, Protocol):
+            z: int
+
+        for proto in (
+            ExtensionsProto, SubProto, SubProto2, SubProto3, SubProto4
+        ):
+            with self.subTest(proto=proto.__name__):
+                self.assertTrue(is_protocol(proto))
+                if Protocol is not typing.Protocol:
+                    self.assertIsInstance(proto, typing_extensions._ProtocolMeta)
+                self.assertIsInstance(proto.__protocol_attrs__, set)
+                with self.assertRaisesRegex(
+                    TypeError, "Protocols cannot be instantiated"
+                ):
+                    proto()
+                # check these don't raise
+                runtime_checkable(proto)
+                typing.runtime_checkable(proto)
+
+        class Concrete(SubProto): pass
+        class Concrete2(SubProto2): pass
+        class Concrete3(SubProto3): pass
+        class Concrete4(SubProto4): pass
+
+        for cls in Concrete, Concrete2, Concrete3, Concrete4:
+            with self.subTest(cls=cls.__name__):
+                self.assertFalse(is_protocol(cls))
+                # Check that this doesn't raise:
+                self.assertIsInstance(cls(), cls)
+                with self.assertRaises(TypeError):
+                    runtime_checkable(cls)
+                with self.assertRaises(TypeError):
+                    typing.runtime_checkable(cls)
+
     def test_no_instantiation(self):
         class P(Protocol): pass
         with self.assertRaises(TypeError):
             P()
         class C(P): pass
         self.assertIsInstance(C(), C)
         T = TypeVar('T')
@@ -1934,14 +2009,162 @@
         with self.assertRaisesRegex(TypeError, only_classes_allowed):
             issubclass(1, PG)
         with self.assertRaisesRegex(TypeError, only_classes_allowed):
             issubclass(1, BadP)
         with self.assertRaisesRegex(TypeError, only_classes_allowed):
             issubclass(1, BadPG)
 
+    def test_implicit_issubclass_between_two_protocols(self):
+        @runtime_checkable
+        class CallableMembersProto(Protocol):
+            def meth(self): ...
+
+        # All the below protocols should be considered "subclasses"
+        # of CallableMembersProto at runtime,
+        # even though none of them explicitly subclass CallableMembersProto
+
+        class IdenticalProto(Protocol):
+            def meth(self): ...
+
+        class SupersetProto(Protocol):
+            def meth(self): ...
+            def meth2(self): ...
+
+        class NonCallableMembersProto(Protocol):
+            meth: Callable[[], None]
+
+        class NonCallableMembersSupersetProto(Protocol):
+            meth: Callable[[], None]
+            meth2: Callable[[str, int], bool]
+
+        class MixedMembersProto1(Protocol):
+            meth: Callable[[], None]
+            def meth2(self): ...
+
+        class MixedMembersProto2(Protocol):
+            def meth(self): ...
+            meth2: Callable[[str, int], bool]
+
+        for proto in (
+            IdenticalProto, SupersetProto, NonCallableMembersProto,
+            NonCallableMembersSupersetProto, MixedMembersProto1, MixedMembersProto2
+        ):
+            with self.subTest(proto=proto.__name__):
+                self.assertIsSubclass(proto, CallableMembersProto)
+
+        # These two shouldn't be considered subclasses of CallableMembersProto, however,
+        # since they don't have the `meth` protocol member
+
+        class EmptyProtocol(Protocol): ...
+        class UnrelatedProtocol(Protocol):
+            def wut(self): ...
+
+        self.assertNotIsSubclass(EmptyProtocol, CallableMembersProto)
+        self.assertNotIsSubclass(UnrelatedProtocol, CallableMembersProto)
+
+        # These aren't protocols at all (despite having annotations),
+        # so they should only be considered subclasses of CallableMembersProto
+        # if they *actually have an attribute* matching the `meth` member
+        # (just having an annotation is insufficient)
+
+        class AnnotatedButNotAProtocol:
+            meth: Callable[[], None]
+
+        class NotAProtocolButAnImplicitSubclass:
+            def meth(self): pass
+
+        class NotAProtocolButAnImplicitSubclass2:
+            meth: Callable[[], None]
+            def meth(self): pass
+
+        class NotAProtocolButAnImplicitSubclass3:
+            meth: Callable[[], None]
+            meth2: Callable[[int, str], bool]
+            def meth(self): pass
+            def meth(self, x, y): return True
+
+        self.assertNotIsSubclass(AnnotatedButNotAProtocol, CallableMembersProto)
+        self.assertIsSubclass(NotAProtocolButAnImplicitSubclass, CallableMembersProto)
+        self.assertIsSubclass(NotAProtocolButAnImplicitSubclass2, CallableMembersProto)
+        self.assertIsSubclass(NotAProtocolButAnImplicitSubclass3, CallableMembersProto)
+
+    @skip_if_py312b1
+    def test_issubclass_and_isinstance_on_Protocol_itself(self):
+        class C:
+            def x(self): pass
+
+        self.assertNotIsSubclass(object, Protocol)
+        self.assertNotIsInstance(object(), Protocol)
+
+        self.assertNotIsSubclass(str, Protocol)
+        self.assertNotIsInstance('foo', Protocol)
+
+        self.assertNotIsSubclass(C, Protocol)
+        self.assertNotIsInstance(C(), Protocol)
+
+        only_classes_allowed = r"issubclass\(\) arg 1 must be a class"
+
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(1, Protocol)
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass('foo', Protocol)
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(C(), Protocol)
+
+        T = TypeVar('T')
+
+        @runtime_checkable
+        class EmptyProtocol(Protocol): pass
+
+        @runtime_checkable
+        class SupportsStartsWith(Protocol):
+            def startswith(self, x: str) -> bool: ...
+
+        @runtime_checkable
+        class SupportsX(Protocol[T]):
+            def x(self): ...
+
+        for proto in EmptyProtocol, SupportsStartsWith, SupportsX:
+            with self.subTest(proto=proto.__name__):
+                self.assertIsSubclass(proto, Protocol)
+
+        # gh-105237 / PR #105239:
+        # check that the presence of Protocol subclasses
+        # where `issubclass(X, <subclass>)` evaluates to True
+        # doesn't influence the result of `issubclass(X, Protocol)`
+
+        self.assertIsSubclass(object, EmptyProtocol)
+        self.assertIsInstance(object(), EmptyProtocol)
+        self.assertNotIsSubclass(object, Protocol)
+        self.assertNotIsInstance(object(), Protocol)
+
+        self.assertIsSubclass(str, SupportsStartsWith)
+        self.assertIsInstance('foo', SupportsStartsWith)
+        self.assertNotIsSubclass(str, Protocol)
+        self.assertNotIsInstance('foo', Protocol)
+
+        self.assertIsSubclass(C, SupportsX)
+        self.assertIsInstance(C(), SupportsX)
+        self.assertNotIsSubclass(C, Protocol)
+        self.assertNotIsInstance(C(), Protocol)
+
+    @skip_if_py312b1
+    def test_isinstance_checks_not_at_whim_of_gc(self):
+        self.addCleanup(gc.enable)
+        gc.disable()
+
+        with self.assertRaisesRegex(
+            TypeError,
+            "Protocols can only inherit from other protocols"
+        ):
+            class Foo(collections.abc.Mapping, Protocol):
+                pass
+
+        self.assertNotIsInstance([], collections.abc.Mapping)
+
     def test_protocols_issubclass_non_callable(self):
         class C:
             x = 1
 
         @runtime_checkable
         class PNonCall(Protocol):
             x = 1
@@ -2740,22 +2963,62 @@
                 return []
             def close(self):
                 return 0
 
         self.assertIsSubclass(B, Custom)
         self.assertNotIsSubclass(A, Custom)
 
+    @skipUnless(
+        hasattr(collections.abc, "Buffer"),
+        "needs collections.abc.Buffer to exist"
+    )
+    @skip_if_py312b1
+    def test_collections_abc_buffer_protocol_allowed(self):
+        @runtime_checkable
+        class ReleasableBuffer(collections.abc.Buffer, Protocol):
+            def __release_buffer__(self, mv: memoryview) -> None: ...
+
+        class C: pass
+        class D:
+            def __buffer__(self, flags: int) -> memoryview:
+                return memoryview(b'')
+            def __release_buffer__(self, mv: memoryview) -> None:
+                pass
+
+        self.assertIsSubclass(D, ReleasableBuffer)
+        self.assertIsInstance(D(), ReleasableBuffer)
+        self.assertNotIsSubclass(C, ReleasableBuffer)
+        self.assertNotIsInstance(C(), ReleasableBuffer)
+
     def test_builtin_protocol_allowlist(self):
         with self.assertRaises(TypeError):
             class CustomProtocol(TestCase, Protocol):
                 pass
 
         class CustomContextManager(typing.ContextManager, Protocol):
             pass
 
+    @skip_if_py312b1
+    def test_typing_extensions_protocol_allowlist(self):
+        @runtime_checkable
+        class ReleasableBuffer(Buffer, Protocol):
+            def __release_buffer__(self, mv: memoryview) -> None: ...
+
+        class C: pass
+        class D:
+            def __buffer__(self, flags: int) -> memoryview:
+                return memoryview(b'')
+            def __release_buffer__(self, mv: memoryview) -> None:
+                pass
+
+        self.assertIsSubclass(D, ReleasableBuffer)
+        self.assertIsInstance(D(), ReleasableBuffer)
+        self.assertNotIsSubclass(C, ReleasableBuffer)
+        self.assertNotIsInstance(C(), ReleasableBuffer)
+
     def test_non_runtime_protocol_isinstance_check(self):
         class P(Protocol):
             x: int
 
         with self.assertRaisesRegex(TypeError, "@runtime_checkable"):
             isinstance(1, P)
 
@@ -2820,14 +3083,119 @@
         self.assertEqual(X.__parameters__, (T, T2))
         self.assertEqual(X.__args__, (int, T, T2))
 
         Y = X[bytes, memoryview]
         self.assertEqual(Y.__parameters__, ())
         self.assertEqual(Y.__args__, (int, bytes, memoryview))
 
+    def test_get_protocol_members(self):
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(object)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(object())
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Protocol)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Generic)
+
+        class P(Protocol):
+            a: int
+            def b(self) -> str: ...
+            @property
+            def c(self) -> int: ...
+
+        self.assertEqual(get_protocol_members(P), {'a', 'b', 'c'})
+        self.assertIsInstance(get_protocol_members(P), frozenset)
+        self.assertIsNot(get_protocol_members(P), P.__protocol_attrs__)
+
+        class Concrete:
+            a: int
+            def b(self) -> str: return "capybara"
+            @property
+            def c(self) -> int: return 5
+
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Concrete)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Concrete())
+
+        class ConcreteInherit(P):
+            a: int = 42
+            def b(self) -> str: return "capybara"
+            @property
+            def c(self) -> int: return 5
+
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(ConcreteInherit)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(ConcreteInherit())
+
+    @only_with_typing_Protocol
+    def test_get_protocol_members_typing(self):
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(typing.Protocol)
+
+        class P(typing.Protocol):
+            a: int
+            def b(self) -> str: ...
+            @property
+            def c(self) -> int: ...
+
+        self.assertEqual(get_protocol_members(P), {'a', 'b', 'c'})
+        self.assertIsInstance(get_protocol_members(P), frozenset)
+        if hasattr(P, "__protocol_attrs__"):
+            self.assertIsNot(get_protocol_members(P), P.__protocol_attrs__)
+
+        class Concrete:
+            a: int
+            def b(self) -> str: return "capybara"
+            @property
+            def c(self) -> int: return 5
+
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Concrete)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(Concrete())
+
+        class ConcreteInherit(P):
+            a: int = 42
+            def b(self) -> str: return "capybara"
+            @property
+            def c(self) -> int: return 5
+
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(ConcreteInherit)
+        with self.assertRaisesRegex(TypeError, "not a Protocol"):
+            get_protocol_members(ConcreteInherit())
+
+    def test_is_protocol(self):
+        self.assertTrue(is_protocol(Proto))
+        self.assertTrue(is_protocol(Point))
+        self.assertFalse(is_protocol(Concrete))
+        self.assertFalse(is_protocol(Concrete()))
+        self.assertFalse(is_protocol(Generic))
+        self.assertFalse(is_protocol(object))
+
+        # Protocol is not itself a protocol
+        self.assertFalse(is_protocol(Protocol))
+
+    @only_with_typing_Protocol
+    def test_is_protocol_with_typing(self):
+        self.assertFalse(is_protocol(typing.Protocol))
+
+        class TypingProto(typing.Protocol):
+            a: int
+
+        self.assertTrue(is_protocol(TypingProto))
+
+        class Concrete(TypingProto):
+            a: int
+
+        self.assertFalse(is_protocol(Concrete))
+
     @skip_if_py312b1
     def test_interaction_with_isinstance_checks_on_superclasses_with_ABCMeta(self):
         # Ensure the cache is empty, or this test won't work correctly
         collections.abc.Sized._abc_registry_clear()
 
         class Foo(collections.abc.Sized, Protocol): pass
 
@@ -2844,14 +3212,79 @@
         class Foo(typing.Sized, Protocol): pass
 
         # CPython gh-105144: this previously raised TypeError
         # if a Protocol subclass of Sized had been created
         # before any isinstance() checks against Sized
         self.assertNotIsInstance(1, typing.Sized)
 
+    def test_empty_protocol_decorated_with_final(self):
+        @final
+        @runtime_checkable
+        class EmptyProtocol(Protocol): ...
+
+        self.assertIsSubclass(object, EmptyProtocol)
+        self.assertIsInstance(object(), EmptyProtocol)
+
+    def test_protocol_decorated_with_final_callable_members(self):
+        @final
+        @runtime_checkable
+        class ProtocolWithMethod(Protocol):
+            def startswith(self, string: str) -> bool: ...
+
+        self.assertIsSubclass(str, ProtocolWithMethod)
+        self.assertNotIsSubclass(int, ProtocolWithMethod)
+        self.assertIsInstance('foo', ProtocolWithMethod)
+        self.assertNotIsInstance(42, ProtocolWithMethod)
+
+    def test_protocol_decorated_with_final_noncallable_members(self):
+        @final
+        @runtime_checkable
+        class ProtocolWithNonCallableMember(Protocol):
+            x: int
+
+        class Foo:
+            x = 42
+
+        only_callable_members_please = (
+            r"Protocols with non-method members don't support issubclass()"
+        )
+
+        with self.assertRaisesRegex(TypeError, only_callable_members_please):
+            issubclass(Foo, ProtocolWithNonCallableMember)
+
+        with self.assertRaisesRegex(TypeError, only_callable_members_please):
+            issubclass(int, ProtocolWithNonCallableMember)
+
+        self.assertIsInstance(Foo(), ProtocolWithNonCallableMember)
+        self.assertNotIsInstance(42, ProtocolWithNonCallableMember)
+
+    def test_protocol_decorated_with_final_mixed_members(self):
+        @final
+        @runtime_checkable
+        class ProtocolWithMixedMembers(Protocol):
+            x: int
+            def method(self) -> None: ...
+
+        class Foo:
+            x = 42
+            def method(self) -> None: ...
+
+        only_callable_members_please = (
+            r"Protocols with non-method members don't support issubclass()"
+        )
+
+        with self.assertRaisesRegex(TypeError, only_callable_members_please):
+            issubclass(Foo, ProtocolWithMixedMembers)
+
+        with self.assertRaisesRegex(TypeError, only_callable_members_please):
+            issubclass(int, ProtocolWithMixedMembers)
+
+        self.assertIsInstance(Foo(), ProtocolWithMixedMembers)
+        self.assertNotIsInstance(42, ProtocolWithMixedMembers)
+
 
 class Point2DGeneric(Generic[T], TypedDict):
     a: T
     b: T
 
 
 class Bar(Foo):
@@ -2859,30 +3292,35 @@
 
 
 class BarGeneric(FooGeneric[T], total=False):
     b: int
 
 
 class TypedDictTests(BaseTestCase):
-
-    def test_basics_iterable_syntax(self):
+    def test_basics_functional_syntax(self):
         Emp = TypedDict('Emp', {'name': str, 'id': int})
         self.assertIsSubclass(Emp, dict)
         self.assertIsSubclass(Emp, typing.MutableMapping)
         self.assertNotIsSubclass(Emp, collections.abc.Sequence)
         jim = Emp(name='Jim', id=1)
         self.assertIs(type(jim), dict)
         self.assertEqual(jim['name'], 'Jim')
         self.assertEqual(jim['id'], 1)
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__module__, __name__)
         self.assertEqual(Emp.__bases__, (dict,))
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
         self.assertEqual(Emp.__total__, True)
 
+    @skipIf(sys.version_info < (3, 13), "Change in behavior in 3.13")
+    def test_keywords_syntax_raises_on_3_13(self):
+        with self.assertRaises(TypeError):
+            Emp = TypedDict('Emp', name=str, id=int)
+
+    @skipIf(sys.version_info >= (3, 13), "3.13 removes support for kwargs")
     def test_basics_keywords_syntax(self):
         with self.assertWarns(DeprecationWarning):
             Emp = TypedDict('Emp', name=str, id=int)
         self.assertIsSubclass(Emp, dict)
         self.assertIsSubclass(Emp, typing.MutableMapping)
         self.assertNotIsSubclass(Emp, collections.abc.Sequence)
         jim = Emp(name='Jim', id=1)
@@ -2891,14 +3329,15 @@
         self.assertEqual(jim['id'], 1)
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__module__, __name__)
         self.assertEqual(Emp.__bases__, (dict,))
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
         self.assertEqual(Emp.__total__, True)
 
+    @skipIf(sys.version_info >= (3, 13), "3.13 removes support for kwargs")
     def test_typeddict_special_keyword_names(self):
         with self.assertWarns(DeprecationWarning):
             TD = TypedDict("TD", cls=type, self=object, typename=str, _typename=int,
                            fields=list, _fields=dict)
         self.assertEqual(TD.__name__, 'TD')
         self.assertEqual(TD.__annotations__, {'cls': type, 'self': object, 'typename': str,
                                               '_typename': int, 'fields': list, '_fields': dict})
@@ -2907,36 +3346,30 @@
         self.assertEqual(a['cls'], str)
         self.assertEqual(a['self'], 42)
         self.assertEqual(a['typename'], 'foo')
         self.assertEqual(a['_typename'], 53)
         self.assertEqual(a['fields'], [('bar', tuple)])
         self.assertEqual(a['_fields'], {'baz', set})
 
-    @skipIf(hasattr(typing, 'TypedDict'), "Should be tested by upstream")
     def test_typeddict_create_errors(self):
         with self.assertRaises(TypeError):
             TypedDict.__new__()
         with self.assertRaises(TypeError):
             TypedDict()
         with self.assertRaises(TypeError):
             TypedDict('Emp', [('name', str)], None)
 
         with self.assertWarns(DeprecationWarning):
-            Emp = TypedDict(_typename='Emp', name=str, id=int)
-        self.assertEqual(Emp.__name__, 'Emp')
-        self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
-
-        with self.assertWarns(DeprecationWarning):
-            Emp = TypedDict('Emp', _fields={'name': str, 'id': int})
+            Emp = TypedDict('Emp', name=str, id=int)
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
 
     def test_typeddict_errors(self):
         Emp = TypedDict('Emp', {'name': str, 'id': int})
-        if sys.version_info >= (3, 12):
+        if sys.version_info >= (3, 13):
             self.assertEqual(TypedDict.__module__, 'typing')
         else:
             self.assertEqual(TypedDict.__module__, 'typing_extensions')
         jim = Emp(name='Jim', id=1)
         with self.assertRaises(TypeError):
             isinstance({}, Emp)
         with self.assertRaises(TypeError):
@@ -2951,49 +3384,50 @@
                 TypedDict('Hi', [('x', int), ('y', 1)])
         with self.assertRaises(TypeError):
             TypedDict('Hi', [('x', int)], y=int)
 
     def test_py36_class_syntax_usage(self):
         self.assertEqual(LabelPoint2D.__name__, 'LabelPoint2D')
         self.assertEqual(LabelPoint2D.__module__, __name__)
-        self.assertEqual(get_type_hints(LabelPoint2D), {'x': int, 'y': int, 'label': str})
+        self.assertEqual(LabelPoint2D.__annotations__, {'x': int, 'y': int, 'label': str})
         self.assertEqual(LabelPoint2D.__bases__, (dict,))
         self.assertEqual(LabelPoint2D.__total__, True)
         self.assertNotIsSubclass(LabelPoint2D, typing.Sequence)
         not_origin = Point2D(x=0, y=1)
         self.assertEqual(not_origin['x'], 0)
         self.assertEqual(not_origin['y'], 1)
         other = LabelPoint2D(x=0, y=1, label='hi')
         self.assertEqual(other['label'], 'hi')
 
     def test_pickle(self):
         global EmpD  # pickle wants to reference the class by name
-        EmpD = TypedDict('EmpD', {"name": str, "id": int})
+        EmpD = TypedDict('EmpD', {'name': str, 'id': int})
         jane = EmpD({'name': 'jane', 'id': 37})
-        point = Point2DGeneric(a=5.0, b=3.0)
         for proto in range(pickle.HIGHEST_PROTOCOL + 1):
-            # Test non-generic TypedDict
             z = pickle.dumps(jane, proto)
             jane2 = pickle.loads(z)
             self.assertEqual(jane2, jane)
             self.assertEqual(jane2, {'name': 'jane', 'id': 37})
             ZZ = pickle.dumps(EmpD, proto)
             EmpDnew = pickle.loads(ZZ)
             self.assertEqual(EmpDnew({'name': 'jane', 'id': 37}), jane)
-            # and generic TypedDict
-            y = pickle.dumps(point, proto)
-            point2 = pickle.loads(y)
-            self.assertEqual(point, point2)
+
+    def test_pickle_generic(self):
+        point = Point2DGeneric(a=5.0, b=3.0)
+        for proto in range(pickle.HIGHEST_PROTOCOL + 1):
+            z = pickle.dumps(point, proto)
+            point2 = pickle.loads(z)
+            self.assertEqual(point2, point)
             self.assertEqual(point2, {'a': 5.0, 'b': 3.0})
-            YY = pickle.dumps(Point2DGeneric, proto)
-            Point2DGenericNew = pickle.loads(YY)
+            ZZ = pickle.dumps(Point2DGeneric, proto)
+            Point2DGenericNew = pickle.loads(ZZ)
             self.assertEqual(Point2DGenericNew({'a': 5.0, 'b': 3.0}), point)
 
     def test_optional(self):
-        EmpD = TypedDict('EmpD', {"name": str, "id": int})
+        EmpD = TypedDict('EmpD', {'name': str, 'id': int})
 
         self.assertEqual(typing.Optional[EmpD], typing.Union[None, EmpD])
         self.assertNotEqual(typing.List[EmpD], typing.Tuple[EmpD])
 
     def test_total(self):
         D = TypedDict('D', {'x': int}, total=False)
         self.assertEqual(D(), {})
@@ -3005,53 +3439,207 @@
         self.assertEqual(Options(), {})
         self.assertEqual(Options(log_level=2), {'log_level': 2})
         self.assertEqual(Options.__total__, False)
         self.assertEqual(Options.__required_keys__, frozenset())
         self.assertEqual(Options.__optional_keys__, {'log_level', 'log_path'})
 
     def test_optional_keys(self):
+        class Point2Dor3D(Point2D, total=False):
+            z: int
+
         assert Point2Dor3D.__required_keys__ == frozenset(['x', 'y'])
         assert Point2Dor3D.__optional_keys__ == frozenset(['z'])
 
-    def test_required_notrequired_keys(self):
-        assert NontotalMovie.__required_keys__ == frozenset({'title'})
-        assert NontotalMovie.__optional_keys__ == frozenset({'year'})
+    def test_keys_inheritance(self):
+        class BaseAnimal(TypedDict):
+            name: str
 
-        assert TotalMovie.__required_keys__ == frozenset({'title'})
-        assert TotalMovie.__optional_keys__ == frozenset({'year'})
+        class Animal(BaseAnimal, total=False):
+            voice: str
+            tail: bool
 
+        class Cat(Animal):
+            fur_color: str
 
-    def test_keys_inheritance(self):
         assert BaseAnimal.__required_keys__ == frozenset(['name'])
         assert BaseAnimal.__optional_keys__ == frozenset([])
-        assert get_type_hints(BaseAnimal) == {'name': str}
+        assert BaseAnimal.__annotations__ == {'name': str}
 
         assert Animal.__required_keys__ == frozenset(['name'])
         assert Animal.__optional_keys__ == frozenset(['tail', 'voice'])
-        assert get_type_hints(Animal) == {
+        assert Animal.__annotations__ == {
             'name': str,
             'tail': bool,
             'voice': str,
         }
 
         assert Cat.__required_keys__ == frozenset(['name', 'fur_color'])
         assert Cat.__optional_keys__ == frozenset(['tail', 'voice'])
-        assert get_type_hints(Cat) == {
+        assert Cat.__annotations__ == {
             'fur_color': str,
             'name': str,
             'tail': bool,
             'voice': str,
         }
 
+    def test_required_notrequired_keys(self):
+        self.assertEqual(NontotalMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(NontotalMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+        self.assertEqual(TotalMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(TotalMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+        self.assertEqual(VeryAnnotated.__required_keys__,
+                         frozenset())
+        self.assertEqual(VeryAnnotated.__optional_keys__,
+                         frozenset({"a"}))
+
+        self.assertEqual(AnnotatedMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(AnnotatedMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+        self.assertEqual(WeirdlyQuotedMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(WeirdlyQuotedMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+        self.assertEqual(ChildTotalMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(ChildTotalMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+        self.assertEqual(ChildDeeplyAnnotatedMovie.__required_keys__,
+                         frozenset({"title"}))
+        self.assertEqual(ChildDeeplyAnnotatedMovie.__optional_keys__,
+                         frozenset({"year"}))
+
+    def test_multiple_inheritance(self):
+        class One(TypedDict):
+            one: int
+        class Two(TypedDict):
+            two: str
+        class Untotal(TypedDict, total=False):
+            untotal: str
+        Inline = TypedDict('Inline', {'inline': bool})
+        class Regular:
+            pass
+
+        class Child(One, Two):
+            child: bool
+        self.assertEqual(
+            Child.__required_keys__,
+            frozenset(['one', 'two', 'child']),
+        )
+        self.assertEqual(
+            Child.__optional_keys__,
+            frozenset([]),
+        )
+        self.assertEqual(
+            Child.__annotations__,
+            {'one': int, 'two': str, 'child': bool},
+        )
+
+        class ChildWithOptional(One, Untotal):
+            child: bool
+        self.assertEqual(
+            ChildWithOptional.__required_keys__,
+            frozenset(['one', 'child']),
+        )
+        self.assertEqual(
+            ChildWithOptional.__optional_keys__,
+            frozenset(['untotal']),
+        )
+        self.assertEqual(
+            ChildWithOptional.__annotations__,
+            {'one': int, 'untotal': str, 'child': bool},
+        )
+
+        class ChildWithTotalFalse(One, Untotal, total=False):
+            child: bool
+        self.assertEqual(
+            ChildWithTotalFalse.__required_keys__,
+            frozenset(['one']),
+        )
+        self.assertEqual(
+            ChildWithTotalFalse.__optional_keys__,
+            frozenset(['untotal', 'child']),
+        )
+        self.assertEqual(
+            ChildWithTotalFalse.__annotations__,
+            {'one': int, 'untotal': str, 'child': bool},
+        )
+
+        class ChildWithInlineAndOptional(Untotal, Inline):
+            child: bool
+        self.assertEqual(
+            ChildWithInlineAndOptional.__required_keys__,
+            frozenset(['inline', 'child']),
+        )
+        self.assertEqual(
+            ChildWithInlineAndOptional.__optional_keys__,
+            frozenset(['untotal']),
+        )
+        self.assertEqual(
+            ChildWithInlineAndOptional.__annotations__,
+            {'inline': bool, 'untotal': str, 'child': bool},
+        )
+
+        wrong_bases = [
+            (One, Regular),
+            (Regular, One),
+            (One, Two, Regular),
+            (Inline, Regular),
+            (Untotal, Regular),
+        ]
+        for bases in wrong_bases:
+            with self.subTest(bases=bases):
+                with self.assertRaisesRegex(
+                    TypeError,
+                    'cannot inherit from both a TypedDict type and a non-TypedDict',
+                ):
+                    class Wrong(*bases):
+                        pass
+
     def test_is_typeddict(self):
-        assert is_typeddict(Point2D) is True
-        assert is_typeddict(Point2Dor3D) is True
-        assert is_typeddict(Union[str, int]) is False
+        self.assertIs(is_typeddict(Point2D), True)
+        self.assertIs(is_typeddict(Point2Dor3D), True)
+        self.assertIs(is_typeddict(Union[str, int]), False)
         # classes, not instances
-        assert is_typeddict(Point2D()) is False
+        self.assertIs(is_typeddict(Point2D()), False)
+        call_based = TypedDict('call_based', {'a': int})
+        self.assertIs(is_typeddict(call_based), True)
+        self.assertIs(is_typeddict(call_based()), False)
+
+        T = TypeVar("T")
+        class BarGeneric(TypedDict, Generic[T]):
+            a: T
+        self.assertIs(is_typeddict(BarGeneric), True)
+        self.assertIs(is_typeddict(BarGeneric[int]), False)
+        self.assertIs(is_typeddict(BarGeneric()), False)
+
+        if hasattr(typing, "TypeAliasType"):
+            ns = {"TypedDict": TypedDict}
+            exec("""if True:
+                class NewGeneric[T](TypedDict):
+                    a: T
+            """, ns)
+            NewGeneric = ns["NewGeneric"]
+            self.assertIs(is_typeddict(NewGeneric), True)
+            self.assertIs(is_typeddict(NewGeneric[int]), False)
+            self.assertIs(is_typeddict(NewGeneric()), False)
+
+        # The TypedDict constructor is not itself a TypedDict
+        self.assertIs(is_typeddict(TypedDict), False)
+        if hasattr(typing, "TypedDict"):
+            self.assertIs(is_typeddict(typing.TypedDict), False)
 
     @skipUnless(TYPING_3_8_0, "Python 3.8+ required")
     def test_is_typeddict_against_typeddict_from_typing(self):
         Point = typing.TypedDict('Point', {'x': int, 'y': int})
 
         class PointDict2D(typing.TypedDict):
             x: int
@@ -3082,14 +3670,32 @@
             c: str
 
         self.assertEqual(
             get_type_hints(FooBarGeneric),
             {'a': typing.Optional[T], 'b': int, 'c': str}
         )
 
+    @skipUnless(TYPING_3_12_0, "PEP 695 required")
+    def test_pep695_generic_typeddict(self):
+        ns = {"TypedDict": TypedDict}
+        exec("""if True:
+            class A[T](TypedDict):
+                a: T
+            """, ns)
+        A = ns["A"]
+        T, = A.__type_params__
+        self.assertIsInstance(T, TypeVar)
+        self.assertEqual(T.__name__, 'T')
+        self.assertEqual(A.__bases__, (Generic, dict))
+        self.assertEqual(A.__orig_bases__, (TypedDict, Generic[T]))
+        self.assertEqual(A.__mro__, (A, Generic, dict, object))
+        self.assertEqual(A.__parameters__, (T,))
+        self.assertEqual(A[str].__parameters__, ())
+        self.assertEqual(A[str].__args__, (str,))
+
     def test_generic_inheritance(self):
         class A(TypedDict, Generic[T]):
             a: T
 
         self.assertEqual(A.__bases__, (Generic, dict))
         self.assertEqual(A.__orig_bases__, (TypedDict, Generic[T]))
         self.assertEqual(A.__mro__, (A, Generic, dict, object))
@@ -3147,19 +3753,19 @@
         self.assertEqual(Point3D.__bases__, (Generic, dict))
         self.assertEqual(Point3D.__orig_bases__, (Point2DGeneric[T], Generic[T, KT]))
         self.assertEqual(Point3D.__mro__, (Point3D, Generic, dict, object))
         self.assertEqual(Point3D.__parameters__, (T, KT))
         self.assertEqual(Point3D.__total__, True)
         self.assertEqual(Point3D.__optional_keys__, frozenset())
         self.assertEqual(Point3D.__required_keys__, frozenset(['a', 'b', 'c']))
-        assert Point3D.__annotations__ == {
+        self.assertEqual(Point3D.__annotations__, {
             'a': T,
             'b': T,
             'c': KT,
-        }
+        })
         self.assertEqual(Point3D[int, str].__origin__, Point3D)
 
         with self.assertRaises(TypeError):
             Point3D[int]
 
         with self.assertRaises(TypeError):
             class Point3D(Point2DGeneric[T], Generic[KT]):
@@ -3186,14 +3792,111 @@
             'a': T,
             'b': KT,
             'c': int,
         }
         with self.assertRaises(TypeError):
             WithImplicitAny[str]
 
+    @skipUnless(TYPING_3_9_0, "Was changed in 3.9")
+    def test_non_generic_subscript(self):
+        # For backward compatibility, subscription works
+        # on arbitrary TypedDict types.
+        # (But we don't attempt to backport this misfeature onto 3.7 and 3.8.)
+        class TD(TypedDict):
+            a: T
+        A = TD[int]
+        self.assertEqual(A.__origin__, TD)
+        self.assertEqual(A.__parameters__, ())
+        self.assertEqual(A.__args__, (int,))
+        a = A(a=1)
+        self.assertIs(type(a), dict)
+        self.assertEqual(a, {'a': 1})
+
+    def test_orig_bases(self):
+        T = TypeVar('T')
+
+        class Parent(TypedDict):
+            pass
+
+        class Child(Parent):
+            pass
+
+        class OtherChild(Parent):
+            pass
+
+        class MixedChild(Child, OtherChild, Parent):
+            pass
+
+        class GenericParent(TypedDict, Generic[T]):
+            pass
+
+        class GenericChild(GenericParent[int]):
+            pass
+
+        class OtherGenericChild(GenericParent[str]):
+            pass
+
+        class MixedGenericChild(GenericChild, OtherGenericChild, GenericParent[float]):
+            pass
+
+        class MultipleGenericBases(GenericParent[int], GenericParent[float]):
+            pass
+
+        CallTypedDict = TypedDict('CallTypedDict', {})
+
+        self.assertEqual(Parent.__orig_bases__, (TypedDict,))
+        self.assertEqual(Child.__orig_bases__, (Parent,))
+        self.assertEqual(OtherChild.__orig_bases__, (Parent,))
+        self.assertEqual(MixedChild.__orig_bases__, (Child, OtherChild, Parent,))
+        self.assertEqual(GenericParent.__orig_bases__, (TypedDict, Generic[T]))
+        self.assertEqual(GenericChild.__orig_bases__, (GenericParent[int],))
+        self.assertEqual(OtherGenericChild.__orig_bases__, (GenericParent[str],))
+        self.assertEqual(MixedGenericChild.__orig_bases__, (GenericChild, OtherGenericChild, GenericParent[float]))
+        self.assertEqual(MultipleGenericBases.__orig_bases__, (GenericParent[int], GenericParent[float]))
+        self.assertEqual(CallTypedDict.__orig_bases__, (TypedDict,))
+
+    def test_zero_fields_typeddicts(self):
+        T1 = TypedDict("T1", {})
+        class T2(TypedDict): pass
+        try:
+            ns = {"TypedDict": TypedDict}
+            exec("class T3[tvar](TypedDict): pass", ns)
+            T3 = ns["T3"]
+        except SyntaxError:
+            class T3(TypedDict): pass
+        S = TypeVar("S")
+        class T4(TypedDict, Generic[S]): pass
+
+        expected_warning = re.escape(
+            "Failing to pass a value for the 'fields' parameter is deprecated "
+            "and will be disallowed in Python 3.15. "
+            "To create a TypedDict class with 0 fields "
+            "using the functional syntax, "
+            "pass an empty dictionary, e.g. `T5 = TypedDict('T5', {})`."
+        )
+        with self.assertWarnsRegex(DeprecationWarning, fr"^{expected_warning}$"):
+            T5 = TypedDict('T5')
+
+        expected_warning = re.escape(
+            "Passing `None` as the 'fields' parameter is deprecated "
+            "and will be disallowed in Python 3.15. "
+            "To create a TypedDict class with 0 fields "
+            "using the functional syntax, "
+            "pass an empty dictionary, e.g. `T6 = TypedDict('T6', {})`."
+        )
+        with self.assertWarnsRegex(DeprecationWarning, fr"^{expected_warning}$"):
+            T6 = TypedDict('T6', None)
+
+        for klass in T1, T2, T3, T4, T5, T6:
+            with self.subTest(klass=klass.__name__):
+                self.assertEqual(klass.__annotations__, {})
+                self.assertEqual(klass.__required_keys__, set())
+                self.assertEqual(klass.__optional_keys__, set())
+                self.assertIsInstance(klass(), dict)
+
 
 class AnnotatedTests(BaseTestCase):
 
     def test_repr(self):
         if hasattr(typing, 'Annotated'):
             mod_name = 'typing'
         else:
@@ -4243,14 +4946,28 @@
             }
         )
         self.assertIsInstance(CustomerModel, Decorated)
 
 
 class AllTests(BaseTestCase):
 
+    def test_drop_in_for_typing(self):
+        # Check that the typing_extensions.__all__ is a superset of
+        # typing.__all__.
+        t_all = set(typing.__all__)
+        te_all = set(typing_extensions.__all__)
+        exceptions = {"ByteString"}
+        self.assertGreaterEqual(te_all, t_all - exceptions)
+        # Deprecated, to be removed in 3.14
+        self.assertFalse(hasattr(typing_extensions, "ByteString"))
+        # These were never included in `typing.__all__`,
+        # and have been removed in Python 3.13
+        self.assertNotIn('re', te_all)
+        self.assertNotIn('io', te_all)
+
     def test_typing_extensions_includes_standard(self):
         a = typing_extensions.__all__
         self.assertIn('ClassVar', a)
         self.assertIn('Type', a)
         self.assertIn('ChainMap', a)
         self.assertIn('ContextManager', a)
         self.assertIn('Counter', a)
@@ -4319,18 +5036,20 @@
             exclude |= {'get_args', 'get_origin'}
         if sys.version_info < (3, 10, 1):
             exclude |= {"Literal"}
         if sys.version_info < (3, 11):
             exclude |= {'final', 'Any', 'NewType'}
         if sys.version_info < (3, 12):
             exclude |= {
-                'Protocol', 'runtime_checkable', 'SupportsAbs', 'SupportsBytes',
+                'Protocol', 'SupportsAbs', 'SupportsBytes',
                 'SupportsComplex', 'SupportsFloat', 'SupportsIndex', 'SupportsInt',
-                'SupportsRound', 'TypedDict', 'is_typeddict', 'NamedTuple', 'Unpack',
+                'SupportsRound', 'Unpack',
             }
+        if sys.version_info < (3, 13):
+            exclude |= {'NamedTuple', 'TypedDict', 'is_typeddict'}
         for item in typing_extensions.__all__:
             if item not in exclude and hasattr(typing, item):
                 self.assertIs(
                     getattr(typing_extensions, item),
                     getattr(typing, item))
 
     def test_typing_extensions_compiles_with_opt(self):
@@ -4542,44 +5261,90 @@
             Group[int]
 
         for attr in ('__args__', '__origin__', '__parameters__'):
             with self.subTest(attr=attr):
                 self.assertFalse(hasattr(Group, attr))
 
     def test_namedtuple_keyword_usage(self):
-        LocalEmployee = NamedTuple("LocalEmployee", name=str, age=int)
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            "Creating NamedTuple classes using keyword arguments is deprecated"
+        ):
+            LocalEmployee = NamedTuple("LocalEmployee", name=str, age=int)
+
         nick = LocalEmployee('Nick', 25)
         self.assertIsInstance(nick, tuple)
         self.assertEqual(nick.name, 'Nick')
         self.assertEqual(LocalEmployee.__name__, 'LocalEmployee')
         self.assertEqual(LocalEmployee._fields, ('name', 'age'))
         self.assertEqual(LocalEmployee.__annotations__, dict(name=str, age=int))
+
         with self.assertRaisesRegex(
             TypeError,
-            'Either list of fields or keywords can be provided to NamedTuple, not both'
+            "Either list of fields or keywords can be provided to NamedTuple, not both"
         ):
             NamedTuple('Name', [('x', int)], y=str)
 
+        with self.assertRaisesRegex(
+            TypeError,
+            "Either list of fields or keywords can be provided to NamedTuple, not both"
+        ):
+            NamedTuple('Name', [], y=str)
+
+        with self.assertRaisesRegex(
+            TypeError,
+            (
+                r"Cannot pass `None` as the 'fields' parameter "
+                r"and also specify fields using keyword arguments"
+            )
+        ):
+            NamedTuple('Name', None, x=int)
+
     def test_namedtuple_special_keyword_names(self):
-        NT = NamedTuple("NT", cls=type, self=object, typename=str, fields=list)
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            "Creating NamedTuple classes using keyword arguments is deprecated"
+        ):
+            NT = NamedTuple("NT", cls=type, self=object, typename=str, fields=list)
+
         self.assertEqual(NT.__name__, 'NT')
         self.assertEqual(NT._fields, ('cls', 'self', 'typename', 'fields'))
         a = NT(cls=str, self=42, typename='foo', fields=[('bar', tuple)])
         self.assertEqual(a.cls, str)
         self.assertEqual(a.self, 42)
         self.assertEqual(a.typename, 'foo')
         self.assertEqual(a.fields, [('bar', tuple)])
 
     def test_empty_namedtuple(self):
-        NT = NamedTuple('NT')
+        expected_warning = re.escape(
+            "Failing to pass a value for the 'fields' parameter is deprecated "
+            "and will be disallowed in Python 3.15. "
+            "To create a NamedTuple class with 0 fields "
+            "using the functional syntax, "
+            "pass an empty list, e.g. `NT1 = NamedTuple('NT1', [])`."
+        )
+        with self.assertWarnsRegex(DeprecationWarning, fr"^{expected_warning}$"):
+            NT1 = NamedTuple('NT1')
+
+        expected_warning = re.escape(
+            "Passing `None` as the 'fields' parameter is deprecated "
+            "and will be disallowed in Python 3.15. "
+            "To create a NamedTuple class with 0 fields "
+            "using the functional syntax, "
+            "pass an empty list, e.g. `NT2 = NamedTuple('NT2', [])`."
+        )
+        with self.assertWarnsRegex(DeprecationWarning, fr"^{expected_warning}$"):
+            NT2 = NamedTuple('NT2', None)
+
+        NT3 = NamedTuple('NT2', [])
 
         class CNT(NamedTuple):
             pass  # empty body
 
-        for struct in [NT, CNT]:
+        for struct in NT1, NT2, NT3, CNT:
             with self.subTest(struct=struct):
                 self.assertEqual(struct._fields, ())
                 self.assertEqual(struct.__annotations__, {})
                 self.assertIsInstance(struct(), struct)
                 # Attribute was added in a micro version of 3.7
                 # and is tested more fully elsewhere
                 if hasattr(struct, "_field_defaults"):
@@ -4614,15 +5379,14 @@
                 self.assertIsInstance(jane2, cls)
 
                 jane2 = copy.deepcopy(jane)
                 self.assertEqual(jane2, jane)
                 self.assertIsInstance(jane2, cls)
 
     def test_docstring(self):
-        self.assertEqual(NamedTuple.__doc__, typing.NamedTuple.__doc__)
         self.assertIsInstance(NamedTuple.__doc__, str)
 
     @skipUnless(TYPING_3_8_0, "NamedTuple had a bad signature on <=3.7")
     def test_signature_is_same_as_typing_NamedTuple(self):
         self.assertEqual(inspect.signature(NamedTuple), inspect.signature(typing.NamedTuple))
 
     @skipIf(TYPING_3_8_0, "tests are only relevant to <=3.7")
```

### Comparing `typing_extensions-4.6.3/src/typing_extensions.py` & `typing_extensions-4.7.0rc1/src/typing_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,18 @@
     'dataclass_transform',
     'deprecated',
     'get_overloads',
     'final',
     'get_args',
     'get_origin',
     'get_original_bases',
+    'get_protocol_members',
     'get_type_hints',
     'IntVar',
+    'is_protocol',
     'is_typeddict',
     'Literal',
     'NewType',
     'overload',
     'override',
     'Protocol',
     'reveal_type',
@@ -81,14 +83,53 @@
     'TypeAliasType',
     'TypeGuard',
     'TYPE_CHECKING',
     'Never',
     'NoReturn',
     'Required',
     'NotRequired',
+
+    # Pure aliases, have always been in typing
+    'AbstractSet',
+    'AnyStr',
+    'BinaryIO',
+    'Callable',
+    'Collection',
+    'Container',
+    'Dict',
+    'ForwardRef',
+    'FrozenSet',
+    'Generator',
+    'Generic',
+    'Hashable',
+    'IO',
+    'ItemsView',
+    'Iterable',
+    'Iterator',
+    'KeysView',
+    'List',
+    'Mapping',
+    'MappingView',
+    'Match',
+    'MutableMapping',
+    'MutableSequence',
+    'MutableSet',
+    'Optional',
+    'Pattern',
+    'Reversible',
+    'Sequence',
+    'Set',
+    'Sized',
+    'TextIO',
+    'Tuple',
+    'Union',
+    'ValuesView',
+    'cast',
+    'no_type_check',
+    'no_type_check_decorator',
 ]
 
 # for backward compatibility
 PEP_560 = True
 GenericMeta = type
 
 # The functions below are modified copies of typing internal helpers.
@@ -197,25 +238,27 @@
             if cls is Any:
                 raise TypeError("Any cannot be instantiated")
             return super().__new__(cls, *args, **kwargs)
 
 
 ClassVar = typing.ClassVar
 
+
+class _ExtensionsSpecialForm(typing._SpecialForm, _root=True):
+    def __repr__(self):
+        return 'typing_extensions.' + self._name
+
+
 # On older versions of typing there is an internal class named "Final".
 # 3.8+
 if hasattr(typing, 'Final') and sys.version_info[:2] >= (3, 7):
     Final = typing.Final
 # 3.7
 else:
-    class _FinalForm(typing._SpecialForm, _root=True):
-
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
+    class _FinalForm(_ExtensionsSpecialForm, _root=True):
         def __getitem__(self, parameters):
             item = typing._type_check(parameters,
                                       f'{self._name} accepts only a single type.')
             return typing._GenericAlias(self, (item,))
 
     Final = _FinalForm('Final',
                        doc="""A special typing construct to indicate that a name
@@ -299,22 +342,19 @@
             these_args_deduped = set(_value_and_type_iter(self.__args__))
             other_args_deduped = set(_value_and_type_iter(other.__args__))
             return these_args_deduped == other_args_deduped
 
         def __hash__(self):
             return hash(frozenset(_value_and_type_iter(self.__args__)))
 
-    class _LiteralForm(typing._SpecialForm, _root=True):
+    class _LiteralForm(_ExtensionsSpecialForm, _root=True):
         def __init__(self, doc: str):
             self._name = 'Literal'
             self._doc = self.__doc__ = doc
 
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
         def __getitem__(self, parameters):
             if not isinstance(parameters, tuple):
                 parameters = (parameters,)
 
             parameters = _flatten_literal_params(parameters)
 
             val_type_pairs = list(_value_and_type_iter(parameters))
@@ -449,17 +489,18 @@
 Text = typing.Text
 TYPE_CHECKING = typing.TYPE_CHECKING
 
 
 _PROTO_ALLOWLIST = {
     'collections.abc': [
         'Callable', 'Awaitable', 'Iterable', 'Iterator', 'AsyncIterable',
-        'Hashable', 'Sized', 'Container', 'Collection', 'Reversible',
+        'Hashable', 'Sized', 'Container', 'Collection', 'Reversible', 'Buffer',
     ],
     'contextlib': ['AbstractContextManager', 'AbstractAsyncContextManager'],
+    'typing_extensions': ['Buffer'],
 }
 
 
 _EXCLUDED_ATTRS = {
     "__abstractmethods__", "__annotations__", "__weakref__", "_is_protocol",
     "_is_runtime_protocol", "__dict__", "__slots__", "__parameters__",
     "__orig_bases__", "__module__", "_MutableMapping__marker", "__doc__",
@@ -541,41 +582,72 @@
         return None
 
 
 # The performance of runtime-checkable protocols is significantly improved on Python 3.12,
 # so we backport the 3.12 version of Protocol to Python <=3.11
 if sys.version_info >= (3, 12):
     Protocol = typing.Protocol
-    runtime_checkable = typing.runtime_checkable
 else:
     def _allow_reckless_class_checks(depth=3):
         """Allow instance and class checks for special stdlib modules.
         The abc and functools modules indiscriminately call isinstance() and
         issubclass() on the whole MRO of a user class, which may contain protocols.
         """
         return _caller(depth) in {'abc', 'functools', None}
 
     def _no_init(self, *args, **kwargs):
         if type(self)._is_protocol:
             raise TypeError('Protocols cannot be instantiated')
 
-    class _ProtocolMeta(abc.ABCMeta):
+    if sys.version_info >= (3, 8):
+        # Inheriting from typing._ProtocolMeta isn't actually desirable,
+        # but is necessary to allow typing.Protocol and typing_extensions.Protocol
+        # to mix without getting TypeErrors about "metaclass conflict"
+        _typing_Protocol = typing.Protocol
+        _ProtocolMetaBase = type(_typing_Protocol)
+    else:
+        _typing_Protocol = _marker
+        _ProtocolMetaBase = abc.ABCMeta
+
+    class _ProtocolMeta(_ProtocolMetaBase):
         # This metaclass is somewhat unfortunate,
         # but is necessary for several reasons...
+        #
+        # NOTE: DO NOT call super() in any methods in this class
+        # That would call the methods on typing._ProtocolMeta on Python 3.8-3.11
+        # and those are slow
+        def __new__(mcls, name, bases, namespace, **kwargs):
+            if name == "Protocol" and len(bases) < 2:
+                pass
+            elif {Protocol, _typing_Protocol} & set(bases):
+                for base in bases:
+                    if not (
+                        base in {object, typing.Generic, Protocol, _typing_Protocol}
+                        or base.__name__ in _PROTO_ALLOWLIST.get(base.__module__, [])
+                        or is_protocol(base)
+                    ):
+                        raise TypeError(
+                            f"Protocols can only inherit from other protocols, "
+                            f"got {base!r}"
+                        )
+            return abc.ABCMeta.__new__(mcls, name, bases, namespace, **kwargs)
+
         def __init__(cls, *args, **kwargs):
-            super().__init__(*args, **kwargs)
+            abc.ABCMeta.__init__(cls, *args, **kwargs)
             if getattr(cls, "_is_protocol", False):
                 cls.__protocol_attrs__ = _get_protocol_attrs(cls)
                 # PEP 544 prohibits using issubclass()
                 # with protocols that have non-method members.
                 cls.__callable_proto_members_only__ = all(
                     callable(getattr(cls, attr, None)) for attr in cls.__protocol_attrs__
                 )
 
         def __subclasscheck__(cls, other):
+            if cls is Protocol:
+                return type.__subclasscheck__(cls, other)
             if not isinstance(other, type):
                 # Same error message as for issubclass(1, int).
                 raise TypeError('issubclass() arg 1 must be a class')
             if (
                 getattr(cls, '_is_protocol', False)
                 and not _allow_reckless_class_checks()
             ):
@@ -584,31 +656,33 @@
                         "Protocols with non-method members don't support issubclass()"
                     )
                 if not getattr(cls, '_is_runtime_protocol', False):
                     raise TypeError(
                         "Instance and class checks can only be used with "
                         "@runtime_checkable protocols"
                     )
-            return super().__subclasscheck__(other)
+            return abc.ABCMeta.__subclasscheck__(cls, other)
 
         def __instancecheck__(cls, instance):
             # We need this method for situations where attributes are
             # assigned in __init__.
+            if cls is Protocol:
+                return type.__instancecheck__(cls, instance)
             if not getattr(cls, "_is_protocol", False):
                 # i.e., it's a concrete subclass of a protocol
-                return super().__instancecheck__(instance)
+                return abc.ABCMeta.__instancecheck__(cls, instance)
 
             if (
                 not getattr(cls, '_is_runtime_protocol', False) and
                 not _allow_reckless_class_checks()
             ):
                 raise TypeError("Instance and class checks can only be used with"
                                 " @runtime_checkable protocols")
 
-            if super().__instancecheck__(instance):
+            if abc.ABCMeta.__instancecheck__(cls, instance):
                 return True
 
             for attr in cls.__protocol_attrs__:
                 try:
                     val = inspect.getattr_static(instance, attr)
                 except AttributeError:
                     break
@@ -619,15 +693,15 @@
 
             return False
 
         def __eq__(cls, other):
             # Hack so that typing.Generic.__class_getitem__
             # treats typing_extensions.Protocol
             # as equivalent to typing.Protocol on Python 3.8+
-            if super().__eq__(other) is True:
+            if abc.ABCMeta.__eq__(cls, other) is True:
                 return True
             return (
                 cls is Protocol and other is getattr(typing, "Protocol", object())
             )
 
         # This has to be defined, or the abc-module cache
         # complains about classes with this metaclass being unhashable,
@@ -649,31 +723,21 @@
                     break
 
                 # ...or in annotations, if it is a sub-protocol.
                 annotations = getattr(base, '__annotations__', {})
                 if (
                     isinstance(annotations, collections.abc.Mapping)
                     and attr in annotations
-                    and issubclass(other, (typing.Generic, _ProtocolMeta))
-                    and getattr(other, "_is_protocol", False)
+                    and is_protocol(other)
                 ):
                     break
             else:
                 return NotImplemented
         return True
 
-    def _check_proto_bases(cls):
-        for base in cls.__bases__:
-            if not (base in (object, typing.Generic) or
-                    base.__module__ in _PROTO_ALLOWLIST and
-                    base.__name__ in _PROTO_ALLOWLIST[base.__module__] or
-                    isinstance(base, _ProtocolMeta) and base._is_protocol):
-                raise TypeError('Protocols can only inherit from other'
-                                f' protocols, got {repr(base)}')
-
     if sys.version_info >= (3, 8):
         class Protocol(typing.Generic, metaclass=_ProtocolMeta):
             __doc__ = typing.Protocol.__doc__
             __slots__ = ()
             _is_protocol = True
             _is_runtime_protocol = False
 
@@ -688,16 +752,15 @@
                 if '__subclasshook__' not in cls.__dict__:
                     cls.__subclasshook__ = _proto_hook
 
                 # We have nothing more to do for non-protocols...
                 if not cls._is_protocol:
                     return
 
-                # ... otherwise check consistency of bases, and prohibit instantiation.
-                _check_proto_bases(cls)
+                # ... otherwise prohibit instantiation.
                 if cls.__init__ is Protocol.__init__:
                     cls.__init__ = _no_init
 
     else:
         class Protocol(metaclass=_ProtocolMeta):
             # There is quite a lot of overlapping code with typing.Generic.
             # Unfortunately it is hard to avoid this on Python <3.8,
@@ -784,19 +847,22 @@
                 if '__subclasshook__' not in cls.__dict__:
                     cls.__subclasshook__ = _proto_hook
 
                 # We have nothing more to do for non-protocols.
                 if not cls._is_protocol:
                     return
 
-                # Check consistency of bases.
-                _check_proto_bases(cls)
+                # Prohibit instantiation
                 if cls.__init__ is Protocol.__init__:
                     cls.__init__ = _no_init
 
+
+if sys.version_info >= (3, 8):
+    runtime_checkable = typing.runtime_checkable
+else:
     def runtime_checkable(cls):
         """Mark a protocol class as a runtime protocol, so that it
         can be used with isinstance() and issubclass(). Raise TypeError
         if applied to a non-protocol class.
 
         This allows a simple-minded structural check very similar to the
         one-offs in collections.abc such as Hashable.
@@ -888,135 +954,79 @@
         __slots__ = ()
 
         @abc.abstractmethod
         def __round__(self, ndigits: int = 0) -> T_co:
             pass
 
 
-if sys.version_info >= (3, 12):
+if sys.version_info >= (3, 13):
     # The standard library TypedDict in Python 3.8 does not store runtime information
     # about which (if any) keys are optional.  See https://bugs.python.org/issue38834
     # The standard library TypedDict in Python 3.9.0/1 does not honour the "total"
     # keyword with old-style TypedDict().  See https://bugs.python.org/issue42059
     # The standard library TypedDict below Python 3.11 does not store runtime
     # information about optional and required keys when using Required or NotRequired.
     # Generic TypedDicts are also impossible using typing.TypedDict on Python <3.11.
     # Aaaand on 3.12 we add __orig_bases__ to TypedDict
     # to enable better runtime introspection.
+    # On 3.13 we deprecate some odd ways of creating TypedDicts.
     TypedDict = typing.TypedDict
     _TypedDictMeta = typing._TypedDictMeta
     is_typeddict = typing.is_typeddict
 else:
-    def _check_fails(cls, other):
-        try:
-            if _caller() not in {'abc', 'functools', 'typing'}:
-                # Typed dicts are only for static structural subtyping.
-                raise TypeError('TypedDict does not support instance and class checks')
-        except (AttributeError, ValueError):
-            pass
-        return False
-
-    def _dict_new(*args, **kwargs):
-        if not args:
-            raise TypeError('TypedDict.__new__(): not enough arguments')
-        _, args = args[0], args[1:]  # allow the "cls" keyword be passed
-        return dict(*args, **kwargs)
-
-    _dict_new.__text_signature__ = '($cls, _typename, _fields=None, /, **kwargs)'
-
-    def _typeddict_new(*args, total=True, **kwargs):
-        if not args:
-            raise TypeError('TypedDict.__new__(): not enough arguments')
-        _, args = args[0], args[1:]  # allow the "cls" keyword be passed
-        if args:
-            typename, args = args[0], args[1:]  # allow the "_typename" keyword be passed
-        elif '_typename' in kwargs:
-            typename = kwargs.pop('_typename')
-            warnings.warn("Passing '_typename' as keyword argument is deprecated",
-                          DeprecationWarning, stacklevel=2)
-        else:
-            raise TypeError("TypedDict.__new__() missing 1 required positional "
-                            "argument: '_typename'")
-        if args:
-            try:
-                fields, = args  # allow the "_fields" keyword be passed
-            except ValueError:
-                raise TypeError('TypedDict.__new__() takes from 2 to 3 '
-                                f'positional arguments but {len(args) + 2} '
-                                'were given')
-        elif '_fields' in kwargs and len(kwargs) == 1:
-            fields = kwargs.pop('_fields')
-            warnings.warn("Passing '_fields' as keyword argument is deprecated",
-                          DeprecationWarning, stacklevel=2)
-        else:
-            fields = None
-
-        if fields is None:
-            fields = kwargs
-        elif kwargs:
-            raise TypeError("TypedDict takes either a dict or keyword arguments,"
-                            " but not both")
-
-        if kwargs:
-            warnings.warn(
-                "The kwargs-based syntax for TypedDict definitions is deprecated, "
-                "may be removed in a future version, and may not be "
-                "understood by third-party type checkers.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
+    # 3.10.0 and later
+    _TAKES_MODULE = "module" in inspect.signature(typing._type_check).parameters
 
-        ns = {'__annotations__': dict(fields)}
-        module = _caller()
-        if module is not None:
-            # Setting correct module is necessary to make typed dict classes pickleable.
-            ns['__module__'] = module
+    if sys.version_info >= (3, 8):
+        _fake_name = "Protocol"
+    else:
+        _fake_name = "_Protocol"
 
-        return _TypedDictMeta(typename, (), ns, total=total)
+    class _TypedDictMeta(type):
+        def __new__(cls, name, bases, ns, total=True):
+            """Create new typed dict class object.
 
-    _typeddict_new.__text_signature__ = ('($cls, _typename, _fields=None,'
-                                         ' /, *, total=True, **kwargs)')
+            This method is called when TypedDict is subclassed,
+            or when TypedDict is instantiated. This way
+            TypedDict supports all three syntax forms described in its docstring.
+            Subclasses and instances of TypedDict return actual dictionaries.
+            """
+            for base in bases:
+                if type(base) is not _TypedDictMeta and base is not typing.Generic:
+                    raise TypeError('cannot inherit from both a TypedDict type '
+                                    'and a non-TypedDict base class')
 
-    _TAKES_MODULE = "module" in inspect.signature(typing._type_check).parameters
+            if any(issubclass(b, typing.Generic) for b in bases):
+                generic_base = (typing.Generic,)
+            else:
+                generic_base = ()
 
-    class _TypedDictMeta(type):
-        def __init__(cls, name, bases, ns, total=True):
-            super().__init__(name, bases, ns)
+            # typing.py generally doesn't let you inherit from plain Generic, unless
+            # the name of the class happens to be "Protocol" (or "_Protocol" on 3.7).
+            tp_dict = type.__new__(_TypedDictMeta, _fake_name, (*generic_base, dict), ns)
+            tp_dict.__name__ = name
+            if tp_dict.__qualname__ == _fake_name:
+                tp_dict.__qualname__ = name
 
-        def __new__(cls, name, bases, ns, total=True):
-            # Create new typed dict class object.
-            # This method is called directly when TypedDict is subclassed,
-            # or via _typeddict_new when TypedDict is instantiated. This way
-            # TypedDict supports all three syntaxes described in its docstring.
-            # Subclasses and instances of TypedDict return actual dictionaries
-            # via _dict_new.
-            ns['__new__'] = _typeddict_new if name == 'TypedDict' else _dict_new
-            # Don't insert typing.Generic into __bases__ here,
-            # or Generic.__init_subclass__ will raise TypeError
-            # in the super().__new__() call.
-            # Instead, monkey-patch __bases__ onto the class after it's been created.
-            tp_dict = super().__new__(cls, name, (dict,), ns)
-
-            is_generic = any(issubclass(base, typing.Generic) for base in bases)
-
-            if is_generic:
-                tp_dict.__bases__ = (typing.Generic, dict)
-                _maybe_adjust_parameters(tp_dict)
-            else:
-                # generic TypedDicts get __orig_bases__ from Generic
-                tp_dict.__orig_bases__ = bases or (TypedDict,)
+            if not hasattr(tp_dict, '__orig_bases__'):
+                tp_dict.__orig_bases__ = bases
 
             annotations = {}
             own_annotations = ns.get('__annotations__', {})
             msg = "TypedDict('Name', {f0: t0, f1: t1, ...}); each t must be a type"
-            kwds = {"module": tp_dict.__module__} if _TAKES_MODULE else {}
-            own_annotations = {
-                n: typing._type_check(tp, msg, **kwds)
-                for n, tp in own_annotations.items()
-            }
+            if _TAKES_MODULE:
+                own_annotations = {
+                    n: typing._type_check(tp, msg, module=tp_dict.__module__)
+                    for n, tp in own_annotations.items()
+                }
+            else:
+                own_annotations = {
+                    n: typing._type_check(tp, msg)
+                    for n, tp in own_annotations.items()
+                }
             required_keys = set()
             optional_keys = set()
 
             for base in bases:
                 annotations.update(base.__dict__.get('__annotations__', {}))
                 required_keys.update(base.__dict__.get('__required_keys__', ()))
                 optional_keys.update(base.__dict__.get('__optional_keys__', ()))
@@ -1042,47 +1052,107 @@
             tp_dict.__annotations__ = annotations
             tp_dict.__required_keys__ = frozenset(required_keys)
             tp_dict.__optional_keys__ = frozenset(optional_keys)
             if not hasattr(tp_dict, '__total__'):
                 tp_dict.__total__ = total
             return tp_dict
 
-        __instancecheck__ = __subclasscheck__ = _check_fails
+        __call__ = dict  # static method
+
+        def __subclasscheck__(cls, other):
+            # Typed dicts are only for static structural subtyping.
+            raise TypeError('TypedDict does not support instance and class checks')
 
-    TypedDict = _TypedDictMeta('TypedDict', (dict,), {})
-    TypedDict.__module__ = __name__
-    TypedDict.__doc__ = \
-        """A simple typed name space. At runtime it is equivalent to a plain dict.
+        __instancecheck__ = __subclasscheck__
 
-        TypedDict creates a dictionary type that expects all of its
-        instances to have a certain set of keys, with each key
+    def TypedDict(__typename, __fields=_marker, *, total=True, **kwargs):
+        """A simple typed namespace. At runtime it is equivalent to a plain dict.
+
+        TypedDict creates a dictionary type such that a type checker will expect all
+        instances to have a certain set of keys, where each key is
         associated with a value of a consistent type. This expectation
-        is not checked at runtime but is only enforced by type checkers.
+        is not checked at runtime.
+
         Usage::
 
             class Point2D(TypedDict):
                 x: int
                 y: int
                 label: str
 
             a: Point2D = {'x': 1, 'y': 2, 'label': 'good'}  # OK
             b: Point2D = {'z': 3, 'label': 'bad'}           # Fails type check
 
             assert Point2D(x=1, y=2, label='first') == dict(x=1, y=2, label='first')
 
         The type info can be accessed via the Point2D.__annotations__ dict, and
         the Point2D.__required_keys__ and Point2D.__optional_keys__ frozensets.
-        TypedDict supports two additional equivalent forms::
+        TypedDict supports an additional equivalent form::
 
-            Point2D = TypedDict('Point2D', x=int, y=int, label=str)
             Point2D = TypedDict('Point2D', {'x': int, 'y': int, 'label': str})
 
-        The class syntax is only supported in Python 3.6+, while two other
-        syntax forms work for Python 2.7 and 3.2+
+        By default, all keys must be present in a TypedDict. It is possible
+        to override this by specifying totality::
+
+            class Point2D(TypedDict, total=False):
+                x: int
+                y: int
+
+        This means that a Point2D TypedDict can have any of the keys omitted. A type
+        checker is only expected to support a literal False or True as the value of
+        the total argument. True is the default, and makes all items defined in the
+        class body be required.
+
+        The Required and NotRequired special forms can also be used to mark
+        individual keys as being required or not required::
+
+            class Point2D(TypedDict):
+                x: int  # the "x" key must always be present (Required is the default)
+                y: NotRequired[int]  # the "y" key can be omitted
+
+        See PEP 655 for more details on Required and NotRequired.
         """
+        if __fields is _marker or __fields is None:
+            if __fields is _marker:
+                deprecated_thing = "Failing to pass a value for the 'fields' parameter"
+            else:
+                deprecated_thing = "Passing `None` as the 'fields' parameter"
+
+            example = f"`{__typename} = TypedDict({__typename!r}, {{}})`"
+            deprecation_msg = (
+                f"{deprecated_thing} is deprecated and will be disallowed in "
+                "Python 3.15. To create a TypedDict class with 0 fields "
+                "using the functional syntax, pass an empty dictionary, e.g. "
+            ) + example + "."
+            warnings.warn(deprecation_msg, DeprecationWarning, stacklevel=2)
+            __fields = kwargs
+        elif kwargs:
+            raise TypeError("TypedDict takes either a dict or keyword arguments,"
+                            " but not both")
+        if kwargs:
+            warnings.warn(
+                "The kwargs-based syntax for TypedDict definitions is deprecated "
+                "in Python 3.11, will be removed in Python 3.13, and may not be "
+                "understood by third-party type checkers.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
+        ns = {'__annotations__': dict(__fields)}
+        module = _caller()
+        if module is not None:
+            # Setting correct module is necessary to make typed dict classes pickleable.
+            ns['__module__'] = module
+
+        td = _TypedDictMeta(__typename, (), ns, total=total)
+        td.__orig_bases__ = (TypedDict,)
+        return td
+
+    _TypedDict = type.__new__(_TypedDictMeta, 'TypedDict', (), {})
+    TypedDict.__mro_entries__ = lambda bases: (_TypedDict,)
 
     if hasattr(typing, "_TypedDictMeta"):
         _TYPEDDICT_TYPES = (typing._TypedDictMeta, _TypedDictMeta)
     else:
         _TYPEDDICT_TYPES = (_TypedDictMeta,)
 
     def is_typeddict(tp):
@@ -1092,15 +1162,18 @@
             class Film(TypedDict):
                 title: str
                 year: int
 
             is_typeddict(Film)  # => True
             is_typeddict(Union[list, str])  # => False
         """
-        return isinstance(tp, tuple(_TYPEDDICT_TYPES))
+        # On 3.8, this would otherwise return True
+        if hasattr(typing, "TypedDict") and tp is typing.TypedDict:
+            return False
+        return isinstance(tp, _TYPEDDICT_TYPES)
 
 
 if hasattr(typing, "assert_type"):
     assert_type = typing.assert_type
 
 else:
     def assert_type(__val, __typ):
@@ -1362,48 +1435,42 @@
 
 
 # 3.10+
 if hasattr(typing, 'TypeAlias'):
     TypeAlias = typing.TypeAlias
 # 3.9
 elif sys.version_info[:2] >= (3, 9):
-    class _TypeAliasForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
-    @_TypeAliasForm
+    @_ExtensionsSpecialForm
     def TypeAlias(self, parameters):
         """Special marker indicating that an assignment should
         be recognized as a proper type alias definition by type
         checkers.
 
         For example::
 
             Predicate: TypeAlias = Callable[..., bool]
 
         It's invalid when used anywhere except as in the example above.
         """
         raise TypeError(f"{self} is not subscriptable")
 # 3.7-3.8
 else:
-    class _TypeAliasForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
-    TypeAlias = _TypeAliasForm('TypeAlias',
-                               doc="""Special marker indicating that an assignment should
-                               be recognized as a proper type alias definition by type
-                               checkers.
+    TypeAlias = _ExtensionsSpecialForm(
+        'TypeAlias',
+        doc="""Special marker indicating that an assignment should
+        be recognized as a proper type alias definition by type
+        checkers.
 
-                               For example::
+        For example::
 
-                                   Predicate: TypeAlias = Callable[..., bool]
+            Predicate: TypeAlias = Callable[..., bool]
 
-                               It's invalid when used anywhere except as in the example
-                               above.""")
+        It's invalid when used anywhere except as in the example
+        above."""
+    )
 
 
 def _set_default(type_param, default):
     if isinstance(default, (tuple, list)):
         type_param.__default__ = tuple((typing._type_check(d, "Default must be a type")
                                         for d in default))
     elif default != _marker:
@@ -1710,33 +1777,30 @@
 
 # 3.10+
 if hasattr(typing, 'Concatenate'):
     Concatenate = typing.Concatenate
     _ConcatenateGenericAlias = typing._ConcatenateGenericAlias  # noqa: F811
 # 3.9
 elif sys.version_info[:2] >= (3, 9):
-    @_TypeAliasForm
+    @_ExtensionsSpecialForm
     def Concatenate(self, parameters):
         """Used in conjunction with ``ParamSpec`` and ``Callable`` to represent a
         higher order function which adds, removes or transforms parameters of a
         callable.
 
         For example::
 
            Callable[Concatenate[int, P], int]
 
         See PEP 612 for detailed information.
         """
         return _concatenate_getitem(self, parameters)
 # 3.7-8
 else:
-    class _ConcatenateForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
+    class _ConcatenateForm(_ExtensionsSpecialForm, _root=True):
         def __getitem__(self, parameters):
             return _concatenate_getitem(self, parameters)
 
     Concatenate = _ConcatenateForm(
         'Concatenate',
         doc="""Used in conjunction with ``ParamSpec`` and ``Callable`` to represent a
         higher order function which adds, removes or transforms parameters of a
@@ -1750,19 +1814,15 @@
         """)
 
 # 3.10+
 if hasattr(typing, 'TypeGuard'):
     TypeGuard = typing.TypeGuard
 # 3.9
 elif sys.version_info[:2] >= (3, 9):
-    class _TypeGuardForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
-    @_TypeGuardForm
+    @_ExtensionsSpecialForm
     def TypeGuard(self, parameters):
         """Special typing form used to annotate the return type of a user-defined
         type guard function.  ``TypeGuard`` only accepts a single type argument.
         At runtime, functions marked this way should return a boolean.
 
         ``TypeGuard`` aims to benefit *type narrowing* -- a technique used by static
         type checkers to determine a more precise type of an expression within a
@@ -1802,19 +1862,15 @@
         ``TypeGuard`` also works with type variables.  For more information, see
         PEP 647 (User-Defined Type Guards).
         """
         item = typing._type_check(parameters, f'{self} accepts only a single type.')
         return typing._GenericAlias(self, (item,))
 # 3.7-3.8
 else:
-    class _TypeGuardForm(typing._SpecialForm, _root=True):
-
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
+    class _TypeGuardForm(_ExtensionsSpecialForm, _root=True):
         def __getitem__(self, parameters):
             item = typing._type_check(parameters,
                                       f'{self._name} accepts only a single type')
             return typing._GenericAlias(self, (item,))
 
     TypeGuard = _TypeGuardForm(
         'TypeGuard',
@@ -1980,18 +2036,14 @@
         raise TypeError(f"{self} is not subscriptable")
 
 
 if hasattr(typing, 'Required'):
     Required = typing.Required
     NotRequired = typing.NotRequired
 elif sys.version_info[:2] >= (3, 9):
-    class _ExtensionsSpecialForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
     @_ExtensionsSpecialForm
     def Required(self, parameters):
         """A special typing construct to mark a key of a total=False TypedDict
         as required. For example:
 
             class Movie(TypedDict, total=False):
                 title: Required[str]
@@ -2022,18 +2074,15 @@
                 year=1999,
             )
         """
         item = typing._type_check(parameters, f'{self._name} accepts only a single type.')
         return typing._GenericAlias(self, (item,))
 
 else:
-    class _RequiredForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
+    class _RequiredForm(_ExtensionsSpecialForm, _root=True):
         def __getitem__(self, parameters):
             item = typing._type_check(parameters,
                                       f'{self._name} accepts only a single type.')
             return typing._GenericAlias(self, (item,))
 
     Required = _RequiredForm(
         'Required',
@@ -2113,22 +2162,19 @@
 if sys.version_info >= (3, 12):  # PEP 692 changed the repr of Unpack[]
     Unpack = typing.Unpack
 
     def _is_unpack(obj):
         return get_origin(obj) is Unpack
 
 elif sys.version_info[:2] >= (3, 9):
-    class _UnpackSpecialForm(typing._SpecialForm, _root=True):
+    class _UnpackSpecialForm(_ExtensionsSpecialForm, _root=True):
         def __init__(self, getitem):
             super().__init__(getitem)
             self.__doc__ = _UNPACK_DOC
 
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
     class _UnpackAlias(typing._GenericAlias, _root=True):
         __class__ = typing.TypeVar
 
     @_UnpackSpecialForm
     def Unpack(self, parameters):
         item = typing._type_check(parameters, f'{self._name} accepts only a single type.')
         return _UnpackAlias(self, (item,))
@@ -2136,18 +2182,15 @@
     def _is_unpack(obj):
         return isinstance(obj, _UnpackAlias)
 
 else:
     class _UnpackAlias(typing._GenericAlias, _root=True):
         __class__ = typing.TypeVar
 
-    class _UnpackForm(typing._SpecialForm, _root=True):
-        def __repr__(self):
-            return 'typing_extensions.' + self._name
-
+    class _UnpackForm(_ExtensionsSpecialForm, _root=True):
         def __getitem__(self, parameters):
             item = typing._type_check(parameters,
                                       f'{self._name} accepts only a single type.')
             return _UnpackAlias(self, (item,))
 
     Unpack = _UnpackForm('Unpack', doc=_UNPACK_DOC)
 
@@ -2531,15 +2574,16 @@
     typing._check_generic = _check_generic
 
 
 # Backport typing.NamedTuple as it exists in Python 3.12.
 # In 3.11, the ability to define generic `NamedTuple`s was supported.
 # This was explicitly disallowed in 3.9-3.10, and only half-worked in <=3.8.
 # On 3.12, we added __orig_bases__ to call-based NamedTuples
-if sys.version_info >= (3, 12):
+# On 3.13, we deprecated kwargs-based NamedTuples
+if sys.version_info >= (3, 13):
     NamedTuple = typing.NamedTuple
 else:
     def _make_nmtuple(name, types, module, defaults=()):
         fields = [n for n, t in types]
         annotations = {n: typing._type_check(t, f"field {n} annotation must be a type")
                        for n, t in types}
         nm_tpl = collections.namedtuple(name, fields,
@@ -2575,37 +2619,94 @@
             nm_tpl = _make_nmtuple(
                 typename, types.items(),
                 defaults=[ns[n] for n in default_names],
                 module=ns['__module__']
             )
             nm_tpl.__bases__ = bases
             if typing.Generic in bases:
-                class_getitem = typing.Generic.__class_getitem__.__func__
-                nm_tpl.__class_getitem__ = classmethod(class_getitem)
+                if hasattr(typing, '_generic_class_getitem'):  # 3.12+
+                    nm_tpl.__class_getitem__ = classmethod(typing._generic_class_getitem)
+                else:
+                    class_getitem = typing.Generic.__class_getitem__.__func__
+                    nm_tpl.__class_getitem__ = classmethod(class_getitem)
             # update from user namespace without overriding special namedtuple attributes
             for key in ns:
                 if key in _prohibited_namedtuple_fields:
                     raise AttributeError("Cannot overwrite NamedTuple attribute " + key)
                 elif key not in _special_namedtuple_fields and key not in nm_tpl._fields:
                     setattr(nm_tpl, key, ns[key])
             if typing.Generic in bases:
                 nm_tpl.__init_subclass__()
             return nm_tpl
 
-    def NamedTuple(__typename, __fields=None, **kwargs):
-        if __fields is None:
-            __fields = kwargs.items()
+    def NamedTuple(__typename, __fields=_marker, **kwargs):
+        """Typed version of namedtuple.
+
+        Usage::
+
+            class Employee(NamedTuple):
+                name: str
+                id: int
+
+        This is equivalent to::
+
+            Employee = collections.namedtuple('Employee', ['name', 'id'])
+
+        The resulting class has an extra __annotations__ attribute, giving a
+        dict that maps field names to types.  (The field names are also in
+        the _fields attribute, which is part of the namedtuple API.)
+        An alternative equivalent functional syntax is also accepted::
+
+            Employee = NamedTuple('Employee', [('name', str), ('id', int)])
+        """
+        if __fields is _marker:
+            if kwargs:
+                deprecated_thing = "Creating NamedTuple classes using keyword arguments"
+                deprecation_msg = (
+                    "{name} is deprecated and will be disallowed in Python {remove}. "
+                    "Use the class-based or functional syntax instead."
+                )
+            else:
+                deprecated_thing = "Failing to pass a value for the 'fields' parameter"
+                example = f"`{__typename} = NamedTuple({__typename!r}, [])`"
+                deprecation_msg = (
+                    "{name} is deprecated and will be disallowed in Python {remove}. "
+                    "To create a NamedTuple class with 0 fields "
+                    "using the functional syntax, "
+                    "pass an empty list, e.g. "
+                ) + example + "."
+        elif __fields is None:
+            if kwargs:
+                raise TypeError(
+                    "Cannot pass `None` as the 'fields' parameter "
+                    "and also specify fields using keyword arguments"
+                )
+            else:
+                deprecated_thing = "Passing `None` as the 'fields' parameter"
+                example = f"`{__typename} = NamedTuple({__typename!r}, [])`"
+                deprecation_msg = (
+                    "{name} is deprecated and will be disallowed in Python {remove}. "
+                    "To create a NamedTuple class with 0 fields "
+                    "using the functional syntax, "
+                    "pass an empty list, e.g. "
+                ) + example + "."
         elif kwargs:
             raise TypeError("Either list of fields or keywords"
                             " can be provided to NamedTuple, not both")
+        if __fields is _marker or __fields is None:
+            warnings.warn(
+                deprecation_msg.format(name=deprecated_thing, remove="3.15"),
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            __fields = kwargs.items()
         nt = _make_nmtuple(__typename, __fields, module=_caller())
         nt.__orig_bases__ = (NamedTuple,)
         return nt
 
-    NamedTuple.__doc__ = typing.NamedTuple.__doc__
     _NamedTuple = type.__new__(_NamedTupleMeta, 'NamedTuple', (), {})
 
     # On 3.8+, alter the signature so that it matches typing.NamedTuple.
     # The signature of typing.NamedTuple on >=3.8 is invalid syntax in Python 3.7,
     # so just leave the signature as it is on 3.7.
     if sys.version_info >= (3, 8):
         NamedTuple.__text_signature__ = '(typename, fields=None, /, **kwargs)'
@@ -2863,7 +2964,95 @@
                     return NotImplemented
                 return typing.Union[self, right]
 
             def __ror__(self, left):
                 if not _is_unionable(left):
                     return NotImplemented
                 return typing.Union[left, self]
+
+
+if hasattr(typing, "is_protocol"):
+    is_protocol = typing.is_protocol
+    get_protocol_members = typing.get_protocol_members
+else:
+    def is_protocol(__tp: type) -> bool:
+        """Return True if the given type is a Protocol.
+
+        Example::
+
+            >>> from typing_extensions import Protocol, is_protocol
+            >>> class P(Protocol):
+            ...     def a(self) -> str: ...
+            ...     b: int
+            >>> is_protocol(P)
+            True
+            >>> is_protocol(int)
+            False
+        """
+        return (
+            isinstance(__tp, type)
+            and getattr(__tp, '_is_protocol', False)
+            and __tp != Protocol
+        )
+
+    def get_protocol_members(__tp: type) -> typing.FrozenSet[str]:
+        """Return the set of members defined in a Protocol.
+
+        Example::
+
+            >>> from typing_extensions import Protocol, get_protocol_members
+            >>> class P(Protocol):
+            ...     def a(self) -> str: ...
+            ...     b: int
+            >>> get_protocol_members(P)
+            frozenset({'a', 'b'})
+
+        Raise a TypeError for arguments that are not Protocols.
+        """
+        if not is_protocol(__tp):
+            raise TypeError(f'{__tp!r} is not a Protocol')
+        if hasattr(__tp, '__protocol_attrs__'):
+            return frozenset(__tp.__protocol_attrs__)
+        return frozenset(_get_protocol_attrs(__tp))
+
+
+# Aliases for items that have always been in typing.
+# Explicitly assign these (rather than using `from typing import *` at the top),
+# so that we get a CI error if one of these is deleted from typing.py
+# in a future version of Python
+AbstractSet = typing.AbstractSet
+AnyStr = typing.AnyStr
+BinaryIO = typing.BinaryIO
+Callable = typing.Callable
+Collection = typing.Collection
+Container = typing.Container
+Dict = typing.Dict
+ForwardRef = typing.ForwardRef
+FrozenSet = typing.FrozenSet
+Generator = typing.Generator
+Generic = typing.Generic
+Hashable = typing.Hashable
+IO = typing.IO
+ItemsView = typing.ItemsView
+Iterable = typing.Iterable
+Iterator = typing.Iterator
+KeysView = typing.KeysView
+List = typing.List
+Mapping = typing.Mapping
+MappingView = typing.MappingView
+Match = typing.Match
+MutableMapping = typing.MutableMapping
+MutableSequence = typing.MutableSequence
+MutableSet = typing.MutableSet
+Optional = typing.Optional
+Pattern = typing.Pattern
+Reversible = typing.Reversible
+Sequence = typing.Sequence
+Set = typing.Set
+Sized = typing.Sized
+TextIO = typing.TextIO
+Tuple = typing.Tuple
+Union = typing.Union
+ValuesView = typing.ValuesView
+cast = typing.cast
+no_type_check = typing.no_type_check
+no_type_check_decorator = typing.no_type_check_decorator
```

### Comparing `typing_extensions-4.6.3/PKG-INFO` & `typing_extensions-4.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_extensions
-Version: 4.6.3
+Version: 4.7.0rc1
 Summary: Backported and Experimental Type Hints for Python 3.7+
 Keywords: annotations,backport,checker,checking,function,hinting,hints,type,typechecking,typehinting,typehints,typing
 Author-email: "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee" <levkivskyi@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Project-URL: Bug Tracker, https://github.com/python/typing_extensions/issues
 Project-URL: Changes, https://github.com/python/typing_extensions/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://typing-extensions.readthedocs.io/
 Project-URL: Home, https://github.com/python/typing_extensions
 Project-URL: Q & A, https://github.com/python/typing/discussions
 Project-URL: Repository, https://github.com/python/typing_extensions
```

