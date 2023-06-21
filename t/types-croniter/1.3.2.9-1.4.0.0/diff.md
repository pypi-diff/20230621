# Comparing `tmp/types-croniter-1.3.2.9.tar.gz` & `tmp/types-croniter-1.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-croniter-1.3.2.9.tar", last modified: Thu Apr 13 01:12:14 2023, max compression
+gzip compressed data, was "types-croniter-1.4.0.0.tar", last modified: Wed Jun 21 15:14:47 2023, max compression
```

## Comparing `types-croniter-1.3.2.9.tar` & `types-croniter-1.4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.837728 types-croniter-1.3.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/croniter-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/croniter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 01:11:59.000000 types-croniter-1.3.2.9/croniter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-13 01:11:59.000000 types-croniter-1.3.2.9/croniter-stubs/croniter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 01:12:14.837728 types-croniter-1.3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 01:12:13.000000 types-croniter-1.3.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:12:14.833727 types-croniter-1.3.2.9/types_croniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 01:12:14.000000 types-croniter-1.3.2.9/types_croniter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/croniter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/croniter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 15:14:34.000000 types-croniter-1.4.0.0/croniter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-21 15:14:34.000000 types-croniter-1.4.0.0/croniter-stubs/croniter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/types_croniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/top_level.txt
```

### Comparing `types-croniter-1.3.2.9/CHANGELOG.md` & `types-croniter-1.4.0.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 1.4.0.0 (2023-06-21)
+
+Bump croniter to 1.4 (#10341)
+
+Also require `bytes` for all `hash_id`s for consistency, even
+if some methods might work with other types as well. But
+using other types might hint at some inconsistent type
+usage and be a source of possible bugs.
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 1.3.2.9 (2023-04-13)
 
 Delete allowlist for croniter (#10041)
 
 Fixes #10040
 
 ## 1.3.2.8 (2023-04-09)
```

### Comparing `types-croniter-1.3.2.9/PKG-INFO` & `types-croniter-1.4.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.9
+Version: 1.4.0.0
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
+This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-croniter-1.3.2.9/croniter-stubs/croniter.pyi` & `types-croniter-1.4.0.0/croniter-stubs/croniter.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,93 @@
 import datetime
-from _typeshed import ReadableBuffer, Unused
+from _typeshed import Unused
 from collections import OrderedDict
 from collections.abc import Iterator
 from re import Match, Pattern
 from typing import Any, overload
-from typing_extensions import Final, Literal, Self, TypeAlias
+from typing_extensions import Final, Literal, Never, Self, TypeAlias
 
 _RetType: TypeAlias = type[float | datetime.datetime]
+_Expressions: TypeAlias = list[str]  # fixed-length list of 5 or 6 strings
 
-step_search_re: Pattern[str]
-only_int_re: Pattern[str]
-star_or_int_re: Pattern[str]
-special_dow_re: Pattern[str]
-hash_expression_re: Pattern[str]
-VALID_LEN_EXPRESSION: Final[list[int]]
-ALPHAS: Final[dict[str, int]]
-DOW_ALPHAS: Final[dict[str, int]]
-MONTHS: Final[str]
 M_ALPHAS: Final[dict[str, int]]
+DOW_ALPHAS: Final[dict[str, int]]
+ALPHAS: Final[dict[str, int]]
+step_search_re: Final[Pattern[str]]
+only_int_re: Final[Pattern[str]]
+
 WEEKDAYS: Final[str]
+MONTHS: Final[str]
+star_or_int_re: Final[Pattern[str]]
+special_dow_re: Final[Pattern[str]]
+re_star: Final[Pattern[str]]
+hash_expression_re: Final[Pattern[str]]
+VALID_LEN_EXPRESSION: Final[list[int]]
+EXPRESSIONS: dict[tuple[str, bytes], _Expressions]
 
 def timedelta_to_seconds(td: datetime.timedelta) -> float: ...
 
 class CroniterError(ValueError): ...
 class CroniterBadTypeRangeError(TypeError): ...
 class CroniterBadCronError(CroniterError): ...
 class CroniterUnsupportedSyntaxError(CroniterBadCronError): ...
 class CroniterBadDateError(CroniterError): ...
 class CroniterNotAlphaError(CroniterError): ...
 
 def datetime_to_timestamp(d: datetime.datetime) -> float: ...
 
 class croniter(Iterator[Any]):
-    MONTHS_IN_YEAR: Literal[12]
-    RANGES: tuple[tuple[int, int], ...]
-    DAYS: tuple[
-        Literal[31],
-        Literal[28],
-        Literal[31],
-        Literal[30],
-        Literal[31],
-        Literal[30],
-        Literal[31],
-        Literal[31],
-        Literal[30],
-        Literal[31],
-        Literal[30],
-        Literal[31],
+    MONTHS_IN_YEAR: Final[Literal[12]]
+    RANGES: Final[tuple[tuple[int, int], tuple[int, int], tuple[int, int], tuple[int, int], tuple[int, int], tuple[int, int]]]
+    DAYS: Final[
+        tuple[
+            Literal[31],
+            Literal[28],
+            Literal[31],
+            Literal[30],
+            Literal[31],
+            Literal[30],
+            Literal[31],
+            Literal[31],
+            Literal[30],
+            Literal[31],
+            Literal[30],
+            Literal[31],
+        ]
     ]
-    ALPHACONV: tuple[dict[str, Any], ...]
-    LOWMAP: tuple[dict[int, Any], ...]
-    LEN_MEANS_ALL: tuple[int, ...]
-    bad_length: str
+    ALPHACONV: Final[
+        tuple[dict[Never, Never], dict[Never, Never], dict[str, str], dict[str, int], dict[str, int], dict[Never, Never]]
+    ]
+    LOWMAP: Final[
+        tuple[dict[Never, Never], dict[Never, Never], dict[int, int], dict[int, int], dict[int, int], dict[Never, Never]]
+    ]
+    LEN_MEANS_ALL: Final[tuple[int, int, int, int, int, int]]
+    bad_length: Final[str]
+
     tzinfo: datetime.tzinfo | None
-    cur: float
-    expanded: list[list[str]]
+
+    # Initialized to None, but immediately set to a float.
     start_time: float
     dst_start_time: float
-    nth_weekday_of_month: dict[str, Any]
+    cur: float
+
+    expanded: list[list[str]]
+    nth_weekday_of_month: dict[str, set[int]]
+    expressions: _Expressions
+
     def __init__(
         self,
         expr_format: str,
         start_time: float | datetime.datetime | None = None,
         ret_type: _RetType | None = ...,
         day_or: bool = True,
         max_years_between_matches: int | None = None,
         is_prev: bool = False,
         hash_id: str | bytes | None = None,
+        implement_cron_bug: bool = False,
     ) -> None: ...
     # Most return value depend on ret_type, which can be passed in both as a method argument and as
     # a constructor argument.
     def get_next(self, ret_type: _RetType | None = None, start_time: float | datetime.datetime | None = None) -> Any: ...
     def get_prev(self, ret_type: _RetType | None = None) -> Any: ...
     def get_current(self, ret_type: _RetType | None = None) -> Any: ...
     def set_current(self, start_time: float | datetime.datetime | None, force: bool = True) -> float: ...
@@ -80,17 +97,17 @@
     ) -> Any: ...
     __next__ = next
     def all_next(self, ret_type: _RetType | None = None) -> Iterator[Any]: ...
     def all_prev(self, ret_type: _RetType | None = None) -> Iterator[Any]: ...
     def iter(self, ret_type: _RetType | None = ...) -> Iterator[Any]: ...
     def is_leap(self, year: int) -> bool: ...
     @classmethod
-    def expand(cls, expr_format: str, hash_id: str | bytes | None = None) -> tuple[list[list[str]], dict[str, Any]]: ...
+    def expand(cls, expr_format: str, hash_id: bytes | None = None) -> tuple[list[list[str]], dict[str, set[int]]]: ...
     @classmethod
-    def is_valid(cls, expression: str, hash_id: str | bytes | None = None) -> bool: ...
+    def is_valid(cls, expression: str, hash_id: bytes | None = None) -> bool: ...
     @classmethod
     def match(cls, cron_expression: str, testdate: float | datetime.datetime | None, day_or: bool = True) -> bool: ...
 
 def croniter_range(
     start: float | datetime.datetime,
     stop: float | datetime.datetime,
     expr_format: str,
@@ -110,31 +127,25 @@
         hash_type: Literal["r"],
         hash_id: None = None,
         range_end: int | None = None,
         range_begin: int | None = None,
     ) -> int: ...
     @overload
     def do(
-        self, idx: int, hash_type: str, hash_id: ReadableBuffer, range_end: int | None = None, range_begin: int | None = None
+        self, idx: int, hash_type: str, hash_id: bytes, range_end: int | None = None, range_begin: int | None = None
     ) -> int: ...
     @overload
     def do(
-        self,
-        idx: int,
-        hash_type: str = "h",
-        *,
-        hash_id: ReadableBuffer,
-        range_end: int | None = None,
-        range_begin: int | None = None,
+        self, idx: int, hash_type: str = "h", *, hash_id: bytes, range_end: int | None = None, range_begin: int | None = None
     ) -> int: ...
-    def match(self, efl: Unused, idx: Unused, expr: str, hash_id: Unused = None, **kw: Unused) -> Match[str] | None: ...
+    def match(self, efl: Unused, idx: Unused, expr: str, hash_id: bytes | None = None, **kw: Unused) -> Match[str] | None: ...
     def expand(
         self,
         efl: object,
         idx: int,
         expr: str,
-        hash_id: ReadableBuffer | None = None,
+        hash_id: bytes | None = None,
         match: Match[str] | None | Literal[""] = "",
         **kw: object,
     ) -> str: ...
 
 EXPANDERS: OrderedDict[str, HashExpander]
```

### Comparing `types-croniter-1.3.2.9/setup.py` & `types-croniter-1.4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
+This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.2.9",
+      version="1.4.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md",
```

### Comparing `types-croniter-1.3.2.9/types_croniter.egg-info/PKG-INFO` & `types-croniter-1.4.0.0/types_croniter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.3.2.9
+Version: 1.4.0.0
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `308a36bf5c711cebc406ba89fe7ba173bc57a6ef`.
+This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

