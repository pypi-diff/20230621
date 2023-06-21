# Comparing `tmp/typeapi-2.0.0.tar.gz` & `tmp/typeapi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeapi-2.0.0.tar", max compression
+gzip compressed data, was "typeapi-2.0.1.tar", max compression
```

## Comparing `typeapi-2.0.0.tar` & `typeapi-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      991 2023-06-11 20:15:18.012081 typeapi-2.0.0/LICENSE
--rw-r--r--   0        0        0     2215 2023-06-11 22:16:59.354580 typeapi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4481 2023-06-11 20:15:18.014315 typeapi-2.0.0/readme.md
--rw-r--r--   0        0        0      595 2023-06-11 22:16:59.354754 typeapi-2.0.0/src/typeapi/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-11 20:15:18.015669 typeapi-2.0.0/src/typeapi/backport/inspect.py
--rw-r--r--   0        0        0     5505 2023-06-11 20:15:18.016315 typeapi-2.0.0/src/typeapi/future/astrewrite.py
--rw-r--r--   0        0        0     2342 2023-06-11 20:15:18.016523 typeapi-2.0.0/src/typeapi/future/fake.py
--rw-r--r--   0        0        0     1570 2023-06-11 20:15:18.016706 typeapi-2.0.0/src/typeapi/future/fake_test.py
--rw-r--r--   0        0        0        0 2023-06-11 20:15:18.016850 typeapi-2.0.0/src/typeapi/py.typed
--rw-r--r--   0        0        0    17259 2023-06-11 22:14:04.755853 typeapi-2.0.0/src/typeapi/typehint.py
--rw-r--r--   0        0        0    15922 2023-06-11 22:13:57.158852 typeapi-2.0.0/src/typeapi/typehint_test.py
--rw-r--r--   0        0        0    13472 2023-06-11 20:18:39.495442 typeapi-2.0.0/src/typeapi/utils.py
--rw-r--r--   0        0        0    16290 2023-06-11 20:19:19.937028 typeapi-2.0.0/src/typeapi/utils_test.py
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 typeapi-2.0.0/setup.py
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 typeapi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      991 2023-06-11 20:15:18.012081 typeapi-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2215 2023-06-21 14:33:37.275061 typeapi-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4481 2023-06-11 20:15:18.014315 typeapi-2.0.1/readme.md
+-rw-r--r--   0        0        0      595 2023-06-21 14:33:37.275542 typeapi-2.0.1/src/typeapi/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-11 20:15:18.015669 typeapi-2.0.1/src/typeapi/backport/inspect.py
+-rw-r--r--   0        0        0     5505 2023-06-11 20:15:18.016315 typeapi-2.0.1/src/typeapi/future/astrewrite.py
+-rw-r--r--   0        0        0     2342 2023-06-11 20:15:18.016523 typeapi-2.0.1/src/typeapi/future/fake.py
+-rw-r--r--   0        0        0     1570 2023-06-11 20:15:18.016706 typeapi-2.0.1/src/typeapi/future/fake_test.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:15:18.016850 typeapi-2.0.1/src/typeapi/py.typed
+-rw-r--r--   0        0        0    17348 2023-06-21 14:32:14.219685 typeapi-2.0.1/src/typeapi/typehint.py
+-rw-r--r--   0        0        0    17066 2023-06-21 14:32:02.005693 typeapi-2.0.1/src/typeapi/typehint_test.py
+-rw-r--r--   0        0        0    13472 2023-06-11 20:18:39.495442 typeapi-2.0.1/src/typeapi/utils.py
+-rw-r--r--   0        0        0    16290 2023-06-11 20:19:19.937028 typeapi-2.0.1/src/typeapi/utils_test.py
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 typeapi-2.0.1/setup.py
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 typeapi-2.0.1/PKG-INFO
```

### Comparing `typeapi-2.0.0/LICENSE` & `typeapi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/pyproject.toml` & `typeapi-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # NOTE(NiklasRosenstein): We pin this version so we can keep using the old way that Slap supports installing
 #                         the "docs" extra without Poetry complaining about invalid format of the requirements.
 requires = ["poetry-core==1.1.0a6"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "typeapi"
-version = "2.0.0"
+version = "2.0.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "typeapi", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `typeapi-2.0.0/readme.md` & `typeapi-2.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/__init__.py` & `typeapi-2.0.1/src/typeapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 from .typehint import (
     AnnotatedTypeHint,
     ClassTypeHint,
     ForwardRefTypeHint,
     LiteralTypeHint,
     TupleTypeHint,
```

### Comparing `typeapi-2.0.0/src/typeapi/backport/inspect.py` & `typeapi-2.0.1/src/typeapi/backport/inspect.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/future/astrewrite.py` & `typeapi-2.0.1/src/typeapi/future/astrewrite.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/future/fake.py` & `typeapi-2.0.1/src/typeapi/future/fake.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/future/fake_test.py` & `typeapi-2.0.1/src/typeapi/future/fake_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/typehint.py` & `typeapi-2.0.1/src/typeapi/typehint.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,18 @@
                     f"Expected to find a ClassTypeHint in the base classes of {self!r}, found {current!r} instead."
                 )
 
             response = yield current
             if response == "skip":
                 continue
 
-            current_bases = cast(List[ClassTypeHint], [TypeHint(x, current.type).evaluate() for x in current.bases])
+            current_bases = cast(
+                List[ClassTypeHint],
+                [TypeHint(x, current.type).evaluate().parameterize(current.get_parameter_map()) for x in current.bases],
+            )
 
             if order == "bfs":
                 bases.extend(current_bases)
             elif order == "dfs":
                 bases.extendleft(reversed(current_bases))
             else:
                 raise ValueError(f"Invalid order {order!r}")
```

### Comparing `typeapi-2.0.0/src/typeapi/typehint_test.py` & `typeapi-2.0.1/src/typeapi/typehint_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,24 +498,27 @@
     assert hint.hint == Tuple[int, ...]
     assert hint.origin == tuple
     assert hint.args == (int,)
     assert hint.parameters == ()
     assert hint.repeated
 
 
-def test__ClassTypeHint__iter_all_bases() -> None:
+def test__ClassTypeHint__recurse_bases_generic() -> None:
     class A:
         pass
 
     class B(A, int):
         pass
 
     class C(B, Generic[T]):
         pass
 
+    class D(C[T]):
+        pass
+
     hint = TypeHint(C)
     assert isinstance(hint, ClassTypeHint)
     assert hint.type is C
     assert hint.bases == (B, Generic[T])
     assert list(hint.recurse_bases("bfs")) == [
         TypeHint(C),
         TypeHint(B),
@@ -532,7 +535,48 @@
         TypeHint(A),
         TypeHint(object),
         TypeHint(int),
         TypeHint(object),
         TypeHint(Generic[T]),
         TypeHint(object),
     ]
+
+    hint = TypeHint(D[int])
+    assert isinstance(hint, ClassTypeHint)
+    assert hint.type is D
+    assert hint.bases == (C[T],)
+    assert list(hint.recurse_bases("bfs")) == [
+        TypeHint(D[int]),
+        TypeHint(C[int]),
+        TypeHint(B),
+        TypeHint(Generic[T]),
+        TypeHint(A),
+        TypeHint(int),
+        TypeHint(object),
+        TypeHint(object),
+        TypeHint(object),
+    ]
+
+
+def test__ClassTypeHint__recurse_bases_for_list_subclass() -> None:
+    class CustomList(List[T]):
+        pass
+
+    hint = TypeHint(CustomList)
+    assert isinstance(hint, ClassTypeHint)
+    assert hint.type is CustomList
+    assert hint.bases == (List[T],)
+    assert list(hint.recurse_bases("bfs")) == [
+        TypeHint(CustomList),
+        TypeHint(List[T]),
+        TypeHint(object),
+    ]
+
+    hint = TypeHint(CustomList[int])
+    assert isinstance(hint, ClassTypeHint)
+    assert hint.type is CustomList
+    assert hint.bases == (List[T],)
+    assert list(hint.recurse_bases("bfs")) == [
+        TypeHint(CustomList[int]),
+        TypeHint(List[int]),
+        TypeHint(object),
+    ]
```

### Comparing `typeapi-2.0.0/src/typeapi/utils.py` & `typeapi-2.0.1/src/typeapi/utils.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/src/typeapi/utils_test.py` & `typeapi-2.0.1/src/typeapi/utils_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-2.0.0/setup.py` & `typeapi-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=3.0.0']
 
 setup_kwargs = {
     'name': 'typeapi',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': '',
     'long_description': '# typeapi\n\n[![Python](https://github.com/NiklasRosenstein/python-typeapi/actions/workflows/python.yml/badge.svg)](https://github.com/NiklasRosenstein/python-typeapi/actions/workflows/python.yml)\n\n  [PEP484]: https://peps.python.org/pep-0484/\n  [PEP585]: https://peps.python.org/pep-0585/\n  [PEP604]: https://peps.python.org/pep-0604/\n\n__Compatibility__: Python 3.6.3+\n\nThe `typeapi` package provides an object-oriented interface for introspecting [PEP484][] type hints at runtime,\nincluding forward references that make use of the more recent [PEP585][] and [PEP604][] type hint features in\nPython versions that don\'t natively support them.\n\nThe main API of this module is comprised of:\n\n* `typeapi.TypeHint()` &ndash; A class to parse low-level type hints and present them in a consistent, object-oriented API.\n* `typeapi.get_annotations()` &ndash; Retrieve an object\'s `__annotations__` with support for evaluating future type hints ([PEP585][], [PEP604][]).\n\nThe following kinds of type hints are currently supported:\n\n| Concrete type | Description | Added in |\n| ------------- | ----------- | -------- |\n| `ClassTypeHint` | For any normal or generic type as well as `typing.Any`. Provides access to the underlying type, the type arguments and parameters, if any. | 1.0.0 |\n| `UnionTypeHint` | Represents `Union` type hint and gives access to the union members. | 1.0.0 |\n| `LiteralTypeHint` | Represents a `Literal` type hint and gives access to the literal values. | 1.0.0 |\n| `AnnotatedTypeHint` | Represents an `Annotated` type hint and gives access to the annotated type as well as the metadata. | 1.0.0 |\n| `TypeVarTypeHint` | Represents a `TypeVar` type hint and gives an interface to access the variable\'s metadata (such as constarints, variance, ...). | 1.0.0 |\n| `ForwardRefTypeHint` | Represents a forward reference. Can be evaluated in Python 3.6+ even if it contains [PEP585][] and [PEP604][] expressions. <sup>1)</sup> | 1.0.0, future support in 1.3.0 |\n| `TupleTypeHint` | Reperesents a `Tuple` type hint, allowing you to differentiate between repeated and explicitly sized tuples. | 1.2.0 |\n\n<sup>1)</sup> New-style type union evaluation will continue to return a `typing.Union`, even if the same syntax\nevaluated natively by Python 3.10+ results in a `types.UnionType`.\n\n## Examples\n\nInspect a `List[int]` type hint:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import ClassTypeHint, TypeHint\nfrom typing import List\n\nhint = TypeHint(List[int])\nassert isinstance(hint, ClassTypeHint)\nassert hint.type is list\n\nitem_hint = hint[0]\nassert isinstance(item_hint, ClassTypeHint)\nassert item_hint.type is int\n```\n\nRetrieve the metadata from an `Annotated[...]` type hint:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import AnnotatedTypeHint, ClassTypeHint, TypeHint\nfrom typing_extensions import Annotated\n\nhint = TypeHint(Annotated[int, 42])\nassert isinstance(hint, AnnotatedTypeHint)\nassert hint.type is int\nassert hint.metadata == (42,)\n\nsub_hint = hint[0]\nassert isinstance(sub_hint, ClassTypeHint)\nassert sub_hint.type is int\n```\n\nParameterize one type hint with the parameterization of a generic alias:\n\n```py\n# cat <<EOF | python -\nfrom dataclasses import dataclass\nfrom typeapi import ClassTypeHint, TypeHint\nfrom typing import Generic, TypeVar\nfrom typing_extensions import Annotated\n\nT = TypeVar("T")\n\n@dataclass\nclass MyGeneric(Generic[T]):\n  value: T\n\nhint = TypeHint(MyGeneric[int])\nassert isinstance(hint, ClassTypeHint)\nassert hint.get_parameter_map() == {T: int}\n\nmember_hint = TypeHint(T).parameterize(hint.get_parameter_map())\nassert isinstance(member_hint, ClassTypeHint)\nassert member_hint.type is int\n```\n\nEvaluate forward references with `get_annotations()`:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import get_annotations\nfrom typing import Optional\nfrom sys import version_info\n\nclass MyType:\n  a: "str | None"\n\nannotations = get_annotations(MyType)\n\nif version_info[:2] < (3, 10):\n  assert annotations == {"a": Optional[str]}\nelse:\n  assert annotations == {"a": str | None}\n```\n\nEvaluating forward references with the `TypeHint` API:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import ClassTypeHint, ForwardRefTypeHint, TypeHint\n\nMyVector = "list[MyType]"\n\nclass MyType:\n  pass\n\nhint = TypeHint(MyVector).evaluate(globals())\nprint(hint)  # TypeHint(typing.List[__main__.MyType])\nassert isinstance(hint, ClassTypeHint)\nassert hint.type is list\n\nitem_hint = hint[0]\nassert isinstance(item_hint, ClassTypeHint)\nassert item_hint.type is MyType\n```\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `typeapi-2.0.0/PKG-INFO` & `typeapi-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeapi
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

