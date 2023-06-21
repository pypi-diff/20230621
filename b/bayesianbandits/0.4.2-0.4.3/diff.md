# Comparing `tmp/bayesianbandits-0.4.2.tar.gz` & `tmp/bayesianbandits-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.4.2.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.3.tar", max compression
```

## Comparing `bayesianbandits-0.4.2.tar` & `bayesianbandits-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/README.md
--rw-r--r--   0        0        0     2740 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    20408 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    29847 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5036 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2634 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-14 01:38:50.709377 bayesianbandits-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/README.md
+-rw-r--r--   0        0        0     2919 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    22393 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29847 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5036 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2634 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-21 20:28:19.170026 bayesianbandits-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.3/PKG-INFO
```

### Comparing `bayesianbandits-0.4.2/LICENSE` & `bayesianbandits-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/README.md` & `bayesianbandits-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/bayesianbandits/__init__.py` & `bayesianbandits-0.4.3/bayesianbandits/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,23 +75,33 @@
     :toctree: _autosummary
 
     DirichletClassifier
     GammaRegressor
     NormalRegressor
     NormalInverseGammaRegressor
 
+Exceptions
+==========
+
+These are custom exceptions raised by the bandit classes.
+
+.. autosummary::
+    :toctree: _autosummary
+
+    DelayedRewardException
+
 """
 
 
-from ._basebandit import Bandit, contextual, restless
 from ._arm import Arm
-from ._policy_decorators import (
-    epsilon_greedy,
-    thompson_sampling,
-    upper_confidence_bound,
-)
+from ._basebandit import Bandit, DelayedRewardException, contextual, restless
 from ._estimators import (
     DirichletClassifier,
     GammaRegressor,
-    NormalRegressor,
     NormalInverseGammaRegressor,
+    NormalRegressor,
+)
+from ._policy_decorators import (
+    epsilon_greedy,
+    thompson_sampling,
+    upper_confidence_bound,
 )
```

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_arm.py` & `bayesianbandits-0.4.3/bayesianbandits/_arm.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.3/bayesianbandits/_basebandit.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
+from warnings import warn
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 from sklearn.base import clone
 from typing_extensions import Literal, dataclass_transform
 
 from ._np_utils import groupby_array
 from ._typing import ArmProtocol, BanditProtocol, Learner
 
-
 _B = TypeVar("_B", bound="Bandit")
 
 
 @dataclass_transform(field_specifiers=(Field[Any], field))
 @dataclass
 class Bandit:
     """
@@ -240,14 +240,21 @@
         if self.__class__._delayed_reward is True:
             unique_id = kwargs.get("unique_id")
             if unique_id is None:
                 raise ValueError(
                     "The `unique_id` keyword argument is required when the "
                     "`delayed_reward = True`."
                 )
+            assert self.cache is not None  # this is here for the type checker
+
+            if unique_id in self.cache:
+                raise DelayedRewardException(
+                    f"The unique_id {unique_id} has already been used. "
+                    "Please use a unique identifier."
+                )
 
         ret_val = arm.pull()
 
         if self.__class__._delayed_reward is True:
             # this is here for the type checker
             assert self.cache is not None
 
@@ -310,31 +317,66 @@
                 )
             # check if `unique_id` is a non-string iterable
             elif isinstance(unique_id, Collection) and not isinstance(unique_id, str):
                 return self._update_batch(
                     X_fit, y_fit, cast(Collection[Any], unique_id)
                 )
 
-            arm_to_update = self.arms[self.cache.pop(unique_id)]  # type: ignore
+            try:
+                arm_to_update = self.arms[self.cache.pop(unique_id)]  # type: ignore
+            except KeyError:
+                raise DelayedRewardException(
+                    f"The unique_id {unique_id} is not in the cache. "
+                    "Please use a valid unique identifier."
+                )
 
         else:
             arm_to_update = cast(ArmProtocol, self.last_arm_pulled)
 
         arm_to_update.update(X_fit, y_fit)
 
     def _update_batch(
         self, X: NDArray[np.float_], y: NDArray[np.float_], unique_ids: Collection[Any]
     ):
         # fetch the arms names from the cache
         assert self.cache is not None  # for the type checker
+
+        # get indexes of unique_ids that are in the cache
+        present_ids = np.array(
+            [idx for idx, v in enumerate(unique_ids) if v in self.cache], dtype=int
+        )
+
+        # get the arm names from the cache, get None for missing ids
         arm_names = np.array(
-            [self.cache.pop(unique_id) for unique_id in unique_ids], dtype=str
+            [self.cache.pop(unique_id, None) for unique_id in unique_ids],
+            dtype=str,
         )
 
-        for X_part, y_part, arms in groupby_array(X, y, arm_names, by=arm_names):
+        # raise if all ids are missing
+        if len(present_ids) == 0:
+            raise DelayedRewardException(
+                f"None of the unique_ids {unique_ids} are in the cache. "
+                "Please use valid unique identifiers."
+            )
+
+        # warn if some ids are missing
+        if (missing_ids := len(arm_names) - len(present_ids)) > 0:
+            warn(
+                f"{missing_ids} unique_ids not in the cache. Skipping those updates.",
+                DelayedRewardWarning,
+                stacklevel=2,
+            )
+
+        # update the arms, dropping the missing ids
+        for X_part, y_part, arms in groupby_array(
+            X[present_ids],
+            y[present_ids],
+            arm_names[present_ids],
+            by=arm_names[present_ids],
+        ):
             arm_name = arms[0]
             self.arms[arm_name].update(X_part, y_part)
 
     @overload
     def sample(self, X: ArrayLike, /, *, size: int = 1) -> ArrayLike:
         ...
 
@@ -647,7 +689,25 @@
 
     return cast(Type[_B], cls)
 
 
 def check_is_bandit(cls: type):
     if not issubclass(cls, Bandit):
         raise ValueError("This decorator can only be used on a Bandit subclass.")
+
+
+class DelayedRewardException(Exception):
+    """Exception raised when the user does not handle delayed reward bandits
+    correctly.
+
+    For example, if the user tries to reuse a `unique_id`."""
+
+    pass
+
+
+class DelayedRewardWarning(UserWarning):
+    """Warning raised when the user does not handle delayed reward bandits
+    correctly.
+
+    For example, if the user tries to reuse a `unique_id`."""
+
+    pass
```

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.3/bayesianbandits/_estimators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.3/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.3/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/bayesianbandits/_typing.py` & `bayesianbandits-0.4.3/bayesianbandits/_typing.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.2/pyproject.toml` & `bayesianbandits-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.4.2/PKG-INFO` & `bayesianbandits-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

