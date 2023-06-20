# Comparing `tmp/immoney-0.2.0.tar.gz` & `tmp/immoney-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immoney-0.2.0.tar", last modified: Tue Jun 20 18:43:19 2023, max compression
+gzip compressed data, was "immoney-0.3.0.tar", last modified: Tue Jun 20 22:05:04 2023, max compression
```

## Comparing `immoney-0.2.0.tar` & `immoney-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:43:19.224604 immoney-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-20 18:43:02.000000 immoney-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 18:43:02.000000 immoney-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-20 18:43:19.224604 immoney-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-20 18:43:02.000000 immoney-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 18:43:02.000000 immoney-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 18:43:19.228604 immoney-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:43:02.000000 immoney-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:43:19.220605 immoney-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:43:19.224604 immoney-0.2.0/src/immoney/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/_frozen.py
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)    35908 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-20 18:43:02.000000 immoney-0.2.0/src/immoney/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:43:19.224604 immoney-0.2.0/src/immoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-20 18:43:19.000000 immoney-0.2.0/src/immoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-20 18:43:19.000000 immoney-0.2.0/src/immoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:43:19.000000 immoney-0.2.0/src/immoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 18:43:19.000000 immoney-0.2.0/src/immoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 18:43:19.000000 immoney-0.2.0/src/immoney.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:05:04.455592 immoney-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-20 22:04:51.000000 immoney-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 22:04:51.000000 immoney-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-20 22:05:04.455592 immoney-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-20 22:04:51.000000 immoney-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 22:04:51.000000 immoney-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-20 22:05:04.455592 immoney-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:04:51.000000 immoney-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:05:04.451592 immoney-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:05:04.455592 immoney-0.3.0/src/immoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35908 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 22:04:51.000000 immoney-0.3.0/src/immoney/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:05:04.455592 immoney-0.3.0/src/immoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-20 22:05:04.000000 immoney-0.3.0/src/immoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 22:05:04.000000 immoney-0.3.0/src/immoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:05:04.000000 immoney-0.3.0/src/immoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 22:05:04.000000 immoney-0.3.0/src/immoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 22:05:04.000000 immoney-0.3.0/src/immoney.egg-info/top_level.txt
```

### Comparing `immoney-0.2.0/LICENSE` & `immoney-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `immoney-0.2.0/PKG-INFO` & `immoney-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immoney
-Version: 0.2.0
+Version: 0.3.0
 Summary: Immutable money types for Python
 Home-page: https://github.com/antonagestam/immoney/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -112,14 +112,26 @@
 the price of an item in a store, can be discovered with a static type checker.
 
 #### Type-safe comparison
 
 Instances of `Money` do not support direct comparison with numeric scalar values. For
 convenience an exception is made for integer zero, which is always unambiguous.
 
+```pycon
+>>> from immoney.currencies import SEK
+>>> SEK(1) == 1
+False
+>>> SEK(1) >= 1
+Traceback (most recent call last):
+  ...
+TypeError: '>=' not supported between instances of 'Money' and 'int'
+>>> SEK(0) == 0
+True
+```
+
 #### Immediate and full instantiation
 
 "2 dollars" is represented exactly the same as "2.00 dollars", in every aspect. This
 means that normalization of values happen at instantiation time.
 
 Instantiating normalizes precision to the number of subunits of the instantiated
 currency.
```

### Comparing `immoney-0.2.0/README.md` & `immoney-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,26 @@
 the price of an item in a store, can be discovered with a static type checker.
 
 #### Type-safe comparison
 
 Instances of `Money` do not support direct comparison with numeric scalar values. For
 convenience an exception is made for integer zero, which is always unambiguous.
 
+```pycon
+>>> from immoney.currencies import SEK
+>>> SEK(1) == 1
+False
+>>> SEK(1) >= 1
+Traceback (most recent call last):
+  ...
+TypeError: '>=' not supported between instances of 'Money' and 'int'
+>>> SEK(0) == 0
+True
+```
+
 #### Immediate and full instantiation
 
 "2 dollars" is represented exactly the same as "2.00 dollars", in every aspect. This
 means that normalization of values happen at instantiation time.
 
 Instantiating normalizes precision to the number of subunits of the instantiated
 currency.
```

### Comparing `immoney-0.2.0/setup.cfg` & `immoney-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -23,18 +23,16 @@
 [options]
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.10
 install_requires = 
-	phantom-types>=2.1.0
 	typing-extensions>=4.6.3
 	abcattrs>=0.3.2
-	immutables>=0.19.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 immoney = py.typed
```

### Comparing `immoney-0.2.0/src/immoney/_base.py` & `immoney-0.3.0/src/immoney/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,38 @@
 from fractions import Fraction
 from functools import cached_property
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import ClassVar
 from typing import Final
 from typing import Generic
+from typing import NewType
+from typing import TypeAlias
 from typing import TypeVar
-from typing import cast
 from typing import final
 from typing import overload
 
 from abcattrs import Abstract
 from abcattrs import abstractattrs
+from typing_extensions import Self
 
 from ._cache import InstanceCache
 from ._frozen import Frozen
 from .errors import DivisionByZero
 from .errors import InvalidSubunit
 from .errors import MoneyParseError
-from .types import ParsableMoneyValue
-from .types import PositiveDecimal
 
 if TYPE_CHECKING:
     from pydantic_core.core_schema import CoreSchema
 
     from .registry import CurrencyRegistry
 
-CurrencySelf = TypeVar("CurrencySelf", bound="Currency")
+ParsableMoneyValue: TypeAlias = int | str | Decimal
+PositiveDecimal = NewType("PositiveDecimal", Decimal)
+
 valid_subunit: Final = frozenset({10**i for i in range(20)})
 
 
 @abstractattrs
 class Currency(Frozen, abc.ABC):
     code: ClassVar[Abstract[str]]
     subunit: ClassVar[Abstract[int]]
@@ -60,65 +62,73 @@
 
     def __str__(self) -> str:
         return self.code
 
     def __repr__(self) -> str:
         return f"Currency(code={self.code}, subunit={self.subunit})"
 
-    def __call__(self: CurrencySelf, value: Decimal | int | str) -> Money[CurrencySelf]:
+    def __call__(self, value: Decimal | int | str) -> Money[Self]:
         return Money(value, self)
 
     def __hash__(self) -> int:
         return hash((self.code, self.subunit))
 
     @cached_property
     def decimal_exponent(self) -> Decimal:
         # Is there a smarter way to do this?
         return Decimal("0." + int(math.log10(self.subunit)) * "0")
 
     @cached_property
-    def zero(self: CurrencySelf) -> Money[CurrencySelf]:
+    def zero(self) -> Money[Self]:
         return Money(0, self)
 
     def normalize_value(self, value: Decimal | int | str) -> PositiveDecimal:
-        try:
-            positive = PositiveDecimal.parse(value)
-        except TypeError as e:
-            raise MoneyParseError(
-                "Failed to interpret value as non-negative decimal"
-            ) from e
+        if not isinstance(value, Decimal):
+            try:
+                value = Decimal(value)
+            except decimal.InvalidOperation:
+                raise MoneyParseError("Failed parsing Decimal")
+
+        if value.is_nan():
+            raise MoneyParseError("Cannot parse from NaN")
 
-        quantized = cast(PositiveDecimal, positive.quantize(self.decimal_exponent))
+        if not value.is_finite():
+            raise MoneyParseError("Cannot parse from non-finite")
 
-        if positive != quantized:
+        if value < 0:
+            raise MoneyParseError("Cannot parse from negative value")
+
+        quantized = value.quantize(self.decimal_exponent)
+
+        if value != quantized:
             raise MoneyParseError(
                 f"Cannot interpret value as Money of currency {self.code} without loss "
                 f"of precision. Explicitly round the value or consider using "
                 f"SubunitFraction."
             )
 
-        return quantized
+        return PositiveDecimal(quantized)
 
-    def from_subunit(self: CurrencySelf, value: int) -> Money[CurrencySelf]:
+    def from_subunit(self, value: int) -> Money[Self]:
         return Money.from_subunit(value, self)
 
     @cached_property
-    def one_subunit(self: CurrencySelf) -> Money[CurrencySelf]:
+    def one_subunit(self) -> Money[Self]:
         return self.from_subunit(1)
 
     def fraction(
-        self: CurrencySelf,
+        self,
         subunit_value: Fraction | Decimal | int,
-    ) -> SubunitFraction[CurrencySelf]:
+    ) -> SubunitFraction[Self]:
         return SubunitFraction(subunit_value, self)
 
     def overdraft(
-        self: CurrencySelf,
+        self: Self,
         value: Decimal | int | str,
-    ) -> Overdraft[CurrencySelf]:
+    ) -> Overdraft[Self]:
         return Overdraft(Money(value, self))
 
     @classmethod
     def get_default_registry(cls) -> CurrencyRegistry[Currency]:
         from .currencies import registry
 
         return registry
@@ -132,15 +142,14 @@
         from ._pydantic import build_currency_schema
 
         return build_currency_schema(cls)
 
 
 C_co = TypeVar("C_co", bound=Currency, covariant=True)
 C_inv = TypeVar("C_inv", bound=Currency, covariant=False, contravariant=False)
-MoneySelf = TypeVar("MoneySelf", bound="Money[Any]")
 
 
 @final
 class Money(Frozen, Generic[C_co], metaclass=InstanceCache):
     __slots__ = ("value", "currency")
 
     def __init__(self, value: ParsableMoneyValue, currency: C_co, /) -> None:
@@ -150,15 +159,15 @@
 
     @classmethod
     def _normalize(
         cls,
         value: ParsableMoneyValue,
         currency: C_inv,
         /,
-    ) -> tuple[Decimal, C_inv]:
+    ) -> tuple[PositiveDecimal, C_inv]:
         if not isinstance(currency, Currency):
             raise TypeError(
                 f"Argument 'currency' of {cls.__qualname__!r} must be a Currency, "
                 f"got object of type {type(currency)!r}"
             )
         return currency.normalize_value(value), currency
 
@@ -220,15 +229,15 @@
             return (
                 Money(value, self.currency)
                 if value >= 0
                 else Overdraft(Money(-value, self.currency))
             )
         return NotImplemented
 
-    def __pos__(self: MoneySelf) -> MoneySelf:
+    def __pos__(self) -> Self:
         return self
 
     def __neg__(self: Money[C_co]) -> Overdraft[C_co]:
         return Overdraft(self)
 
     # TODO: Support precision-lossy multiplication with floats?
     @overload
@@ -312,15 +321,15 @@
     def __floordiv__(self, other: object) -> SubunitFraction[C_co]:
         if not isinstance(other, (int, Fraction)):
             return NotImplemented
         if other == 0:
             raise DivisionByZero
         return SubunitFraction.from_money(self, other)
 
-    def __abs__(self: MoneySelf) -> MoneySelf:
+    def __abs__(self) -> Self:
         return self
 
     def as_subunit(self) -> int:
         return int(self.currency.subunit * self.value)
 
     @classmethod
     # This needs HKT to allow typing to work properly for subclasses of Money.
```

### Comparing `immoney-0.2.0/src/immoney/_cache.py` & `immoney-0.3.0/src/immoney/_cache.py`

 * *Files identical despite different names*

### Comparing `immoney-0.2.0/src/immoney/_frozen.py` & `immoney-0.3.0/src/immoney/_frozen.py`

 * *Files identical despite different names*

### Comparing `immoney-0.2.0/src/immoney/_pydantic.py` & `immoney-0.3.0/src/immoney/_pydantic.py`

 * *Files identical despite different names*

### Comparing `immoney-0.2.0/src/immoney/currencies.py` & `immoney-0.3.0/src/immoney/currencies.py`

 * *Files identical despite different names*

### Comparing `immoney-0.2.0/src/immoney/registry.py` & `immoney-0.3.0/src/immoney/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections.abc import Mapping
+from types import MappingProxyType
 from typing import Generic
 from typing import TypeAlias
 from typing import TypeVar
 
-from immutables import Map
-
 from ._base import Currency
 
 C = TypeVar("C", bound=Currency)
 CurrencyRegistry: TypeAlias = Mapping[str, C]
 
 
 class CurrencyCollector(Generic[C]):
@@ -17,8 +16,8 @@
     def __init__(self) -> None:
         self.__collection = list[tuple[str, C]]()
 
     def add(self, currency: C) -> None:
         self.__collection.append((currency.code, currency))
 
     def finalize(self) -> CurrencyRegistry[C]:
-        return Map(self.__collection)
+        return MappingProxyType(dict(self.__collection))
```

### Comparing `immoney-0.2.0/src/immoney.egg-info/PKG-INFO` & `immoney-0.3.0/src/immoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immoney
-Version: 0.2.0
+Version: 0.3.0
 Summary: Immutable money types for Python
 Home-page: https://github.com/antonagestam/immoney/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -112,14 +112,26 @@
 the price of an item in a store, can be discovered with a static type checker.
 
 #### Type-safe comparison
 
 Instances of `Money` do not support direct comparison with numeric scalar values. For
 convenience an exception is made for integer zero, which is always unambiguous.
 
+```pycon
+>>> from immoney.currencies import SEK
+>>> SEK(1) == 1
+False
+>>> SEK(1) >= 1
+Traceback (most recent call last):
+  ...
+TypeError: '>=' not supported between instances of 'Money' and 'int'
+>>> SEK(0) == 0
+True
+```
+
 #### Immediate and full instantiation
 
 "2 dollars" is represented exactly the same as "2.00 dollars", in every aspect. This
 means that normalization of values happen at instantiation time.
 
 Instantiating normalizes precision to the number of subunits of the instantiated
 currency.
```

