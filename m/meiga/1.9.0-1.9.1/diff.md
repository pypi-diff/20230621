# Comparing `tmp/meiga-1.9.0.tar.gz` & `tmp/meiga-1.9.1.tar.gz`

## Comparing `meiga-1.9.0.tar` & `meiga-1.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/VERSION
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/alias.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/deprecation.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/error.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/handlers.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/misc.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/no_given_value.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/on_failure_exception.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/public_api.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/py.typed
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/result.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/__init__.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/assert_failure.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/assert_success.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/__init__.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/early_return.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/to_result.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/unexpected_decoration_order_error.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 meiga-1.9.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meiga-1.9.0/LICENSE
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 meiga-1.9.0/README.md
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 meiga-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 meiga-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/VERSION
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/alias.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/deprecation.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/error.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/handlers.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/misc.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/no_given_value.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/on_failure_exception.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/public_api.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/py.typed
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/result.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/assertions/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/assertions/assert_failure.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/assertions/assert_success.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/decorators/__init__.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/decorators/early_return.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/decorators/to_result.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 meiga-1.9.1/meiga/decorators/unexpected_decoration_order_error.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 meiga-1.9.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meiga-1.9.1/LICENSE
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 meiga-1.9.1/README.md
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 meiga-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 meiga-1.9.1/PKG-INFO
```

### Comparing `meiga-1.9.0/meiga/alias.py` & `meiga-1.9.1/meiga/alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     __match_args__ = ("_value_failure",)
 
     def __init__(self, error: TF = cast(TF, Error())) -> None:
         super().__init__(failure=error)
 
 
 BoolResult = Result[bool, Error]
-AnyResult = Result[Any, Error]
+AnyResult = Result[Any, Any]
 isSuccess: AnyResult = Success()
 isFailure: AnyResult = Failure()
 NotImplementedMethodError: AnyResult = isFailure
```

### Comparing `meiga-1.9.0/meiga/deprecation.py` & `meiga-1.9.1/meiga/deprecation.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/error.py` & `meiga-1.9.1/meiga/error.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/handlers.py` & `meiga-1.9.1/meiga/handlers.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/public_api.py` & `meiga-1.9.1/meiga/public_api.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/result.py` & `meiga-1.9.1/meiga/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,31 +64,29 @@
         if self._is_success:
             return hash((self._is_success, self._value_success))
         else:
             return hash((self._is_success, self._value_failure))
 
     def _assert_values(self) -> None:
         self._is_success = False
-        if isinstance(self._value_success, type(NoGivenValue)) and isinstance(
-            self._value_failure, type(NoGivenValue)
-        ):
+        if self._value_success is NoGivenValue and self._value_failure is NoGivenValue:
             raise TypeError(
                 "Result is a monad, it must be a success or a failure. "
                 "Please model your result selecting only one type [success or failure]."
             )
-        elif not isinstance(self._value_success, type(NoGivenValue)) and not isinstance(
-            self._value_failure, type(NoGivenValue)
+        elif (
+            self._value_success is not NoGivenValue
+            and self._value_failure is not NoGivenValue
         ):
             raise TypeError(
                 "Result is a monad, it cannot be success and failure at the same time. "
                 "Please model your result selecting only one type [success or failure]."
             )
-        elif not isinstance(self._value_success, type(NoGivenValue)):
-            self._is_success = True
-        return None
+        else:
+            self._is_success = self._value_success is not NoGivenValue
 
     def get_value(self) -> TS | TF:
         if self._is_success:
             return cast(TS, self._value_success)
         else:
             return cast(TF, self._value_failure)
```

### Comparing `meiga-1.9.0/meiga/assertions/assert_failure.py` & `meiga-1.9.1/meiga/assertions/assert_failure.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/assertions/assert_success.py` & `meiga-1.9.1/meiga/assertions/assert_success.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/decorators/early_return.py` & `meiga-1.9.1/meiga/decorators/early_return.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/meiga/decorators/to_result.py` & `meiga-1.9.1/meiga/decorators/to_result.py`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/.gitignore` & `meiga-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/LICENSE` & `meiga-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/README.md` & `meiga-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/pyproject.toml` & `meiga-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meiga-1.9.0/PKG-INFO` & `meiga-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meiga
-Version: 1.9.0
+Version: 1.9.1
 Summary: A simple, typed and monad-based Result type for Python
 Project-URL: Documentation, https://alice-biometrics.github.io/meiga/
 Project-URL: Homepage, https://github.com/alice-biometrics/meiga
 Author-email: Alice Biometrics <support@alicebiometrics.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Monad,Result,Typed,Typing,result-type
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meiga Version: 1.9.0 Summary: A simple, typed and
+Metadata-Version: 2.1 Name: meiga Version: 1.9.1 Summary: A simple, typed and
 monad-based Result type for Python Project-URL: Documentation, https://alice-
 biometrics.github.io/meiga/ Project-URL: Homepage, https://github.com/alice-
 biometrics/meiga Author-email: Alice Biometrics
 alicebiometrics.com> License-Expression: MIT License-File: LICENSE Keywords:
 Monad,Result,Typed,Typing,result-type Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
```

