# Comparing `tmp/decoratory-0.1.4.13.tar.gz` & `tmp/decoratory-0.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.4.13.tar", last modified: Wed Jun 21 06:36:38 2023, max compression
+gzip compressed data, was "decoratory-0.1.5.6.tar", last modified: Wed Jun 21 11:44:41 2023, max compression
```

## Comparing `decoratory-0.1.4.13.tar` & `decoratory-0.1.5.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:36:38.026307 decoratory-0.1.4.13/
--rw-rw-rw-   0        0        0     2550 2023-06-21 06:11:12.000000 decoratory-0.1.4.13/License.txt
--rw-rw-rw-   0        0        0    43876 2023-06-21 06:36:38.026307 decoratory-0.1.4.13/PKG-INFO
--rw-rw-rw-   0        0        0    42250 2023-06-21 06:36:06.000000 decoratory-0.1.4.13/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-21 06:11:12.000000 decoratory-0.1.4.13/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 06:36:37.972896 decoratory-0.1.4.13/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-21 06:36:37.995039 decoratory-0.1.4.13/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.4.13/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     5467 2023-06-21 06:36:06.000000 decoratory-0.1.4.13/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.4.13/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.4.13/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12308 2023-06-20 14:08:32.000000 decoratory-0.1.4.13/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    37282 2023-06-19 16:25:39.000000 decoratory-0.1.4.13/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7939 2023-06-20 14:08:32.000000 decoratory-0.1.4.13/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0     9932 2023-06-19 15:55:21.000000 decoratory-0.1.4.13/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-21 06:36:38.010670 decoratory-0.1.4.13/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    43876 2023-06-21 06:36:37.000000 decoratory-0.1.4.13/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-21 06:36:37.000000 decoratory-0.1.4.13/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:36:37.000000 decoratory-0.1.4.13/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 06:36:37.000000 decoratory-0.1.4.13/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 06:36:38.026307 decoratory-0.1.4.13/Unittest/
--rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.4.13/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23859 2023-06-20 14:08:32.000000 decoratory-0.1.4.13/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.4.13/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10729 2023-06-20 08:56:59.000000 decoratory-0.1.4.13/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0     9098 2023-06-19 16:25:39.000000 decoratory-0.1.4.13/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-21 06:36:38.026307 decoratory-0.1.4.13/setup.cfg
--rw-rw-rw-   0        0        0     4447 2023-06-21 06:36:06.000000 decoratory-0.1.4.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/
+-rw-rw-rw-   0        0        0     2550 2023-06-21 06:11:12.000000 decoratory-0.1.5.6/License.txt
+-rw-rw-rw-   0        0        0    46030 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    44405 2023-06-21 10:46:42.000000 decoratory-0.1.5.6/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-21 06:11:12.000000 decoratory-0.1.5.6/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.830328 decoratory-0.1.5.6/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.890770 decoratory-0.1.5.6/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.5.6/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     5466 2023-06-21 11:44:05.000000 decoratory-0.1.5.6/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.5.6/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.5.6/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12412 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    37318 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7993 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10853 2023-06-21 10:48:51.000000 decoratory-0.1.5.6/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.900859 decoratory-0.1.5.6/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    46030 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.920957 decoratory-0.1.5.6/Unittest/
+-rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.5.6/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23858 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.5.6/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10729 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10193 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     4446 2023-06-21 11:44:05.000000 decoratory-0.1.5.6/setup.py
```

### Comparing `decoratory-0.1.4.13/License.txt` & `decoratory-0.1.5.6/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/PKG-INFO` & `decoratory-0.1.5.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.4.13
+Version: 0.1.5.6
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -36,18 +36,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: License.txt
 
 
 .. _top:
 
+
 ==============================================================================
 Decoratory
 ==============================================================================
 
+
 **Introduction**
 
 The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
@@ -66,14 +68,15 @@
 In particular, there is a *comprehensive unit test* for each module, which
 can be executed from the command line using the ``--test`` option. ::
 
     python -m decoratory --test
 
 .. _toc:
 
+
 **Package Contents**
 
 The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
@@ -383,32 +386,32 @@
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
 
 * (optional) ``before`` call functionality
 
-and/or
+and/or an
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an
 
 * (optional) ``replace`` call functionality.
 
 This generic Wrapper is all the more broadly applicable, the more flexibly
 these three activities can be formulated. All three decorator parameters,
 ``before``, ``after`` and ``replace``, can be combined with each other and
 support both single callables and (nested) lists of ``F``-types
 (imported from module decoratory.basic, see `F signature`_ below for details).
-In addition, ``replace`` supports passing results from successive
-replacement calls through an optional keyword argument named ``result``
-(defaut value is ``None``).
+In addition, ``replace`` supports passing a result object from successive
+replacement calls through an optional keyword argument named ``result`` with
+a defaut value, e.g. ``result=None``.
 
-Even without any of these arguments, such a *do nothing wrapper* can be used
+Even without any of these arguments, such an *empty wrapper* can be used
 to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
@@ -449,26 +452,71 @@
 
 .. _F signature:
 
 While ``before`` calls ``print_message`` with its default parameters the
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``.
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the
 passing of any function with optional positional and keyword parameters.
-Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")``
+Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
-A rather more complex example illustrates the replacement of the original
-functionality with a sequence of replacement functionalities, passing a
-``result`` object of type ``int`` between successive calls.
+The idea behind the ``replace`` option is not so much to replace the complete
+original functionality, because you could simply create your own functionality
+for that but to wrap the original functionality, e.g. according to the principle:
+
+#. Edit the call parameters for the original functionality
+#. Execute the original functionality with these modified call parameters
+#. Edit the result and return this modified result
+
+This could then look like this:
+
+.. code-block:: python
+
+    # *** example_wrapper.py - enclose and replacing original function
+
+    # Case 3: Decoration with replace functionality
+    def replace_wrapper(value: str="replace"):
+        # 1. Edit the call parameters for the original functionality
+        value = value.upper()
+        # 2. Execute original functionality with modified call parameters
+        result = some_function.substitute.callee(value)             # (1)
+        # 3. Edit the result and return this modified result
+        return f"result: '{result}'"
+
+    @Wrapper(replace=replace_wrapper)
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+        return value
+
+    result = some_function()        # value = 'REPLACE'
+    print(result)                   # result: 'REPLACE'
+
+The first output ``value = 'REPLACE'`` comes from the original function
+``some_function()`` but using parameters modified by the
+``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
+of the ``return`` modified by the ``replace_wrapper()``. Please note the line
+marked with ``(1)`` in the ``replace_wrapper()``: It is very important
+to avoid self-recursions:
+
+    **Hint** --- Avoidance of self-recursion in the replace wrapper
+
+    *In the replace wrapper, the undecorated version of the original
+    functionality must always be called. It is accessible via the*
+    ``substitute.callee`` *method of the wrapper!*
+
+For the sake of completeness, a rather more complex example illustrates
+the replacement of the original functionality with a sequence of replacement
+functionalities, passing a ``result`` object of type ``int`` between
+successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
-    # Case 3: Decoration with before, after and multiple replacements
+    # Case 4: Decoration with before, after and multiple replacements
     def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
@@ -501,15 +549,15 @@
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
-    # Case 4: Decoration of a class always refers to __init__
+    # Case 5: Decoration of a class always refers to __init__
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
@@ -524,15 +572,15 @@
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
-    # Case 5: Define a private wrapper library
+    # Case 6: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
     # Multiple decorations for specialized functionality encapsulation
     @before_wrapper
     @after_wrapper
     def some_function(value: str = "original"):
@@ -1045,14 +1093,19 @@
 it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.5.*, Build: 2023-06-21**
+
+- Pre production state, version 0.9.* for module
+    - wrapper [ ``python -m decoratory.wrapper --version`` ]
+
 **Version: 0.1.4.*, Build: 2023-06-21**
 
 - A new subclass SemiSingleton for a resettable singleton
 - Accessible parameter for singleton and multiton removed
 - Additional test and documentation
 - Pre production state, version 0.9.* for modules
     - singleton [ ``python -m decoratory.singleton --version`` ]
```

### Comparing `decoratory-0.1.4.13/Readme.rst` & `decoratory-0.1.5.6/Readme.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 .. _top:
 
+
 ==============================================================================
 Decoratory
 ==============================================================================
 
+
 **Introduction**
 
 The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
@@ -27,14 +29,15 @@
 In particular, there is a *comprehensive unit test* for each module, which
 can be executed from the command line using the ``--test`` option. ::
 
     python -m decoratory --test
 
 .. _toc:
 
+
 **Package Contents**
 
 The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
@@ -344,32 +347,32 @@
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
 
 * (optional) ``before`` call functionality
 
-and/or
+and/or an
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an
 
 * (optional) ``replace`` call functionality.
 
 This generic Wrapper is all the more broadly applicable, the more flexibly
 these three activities can be formulated. All three decorator parameters,
 ``before``, ``after`` and ``replace``, can be combined with each other and
 support both single callables and (nested) lists of ``F``-types
 (imported from module decoratory.basic, see `F signature`_ below for details).
-In addition, ``replace`` supports passing results from successive
-replacement calls through an optional keyword argument named ``result``
-(defaut value is ``None``).
+In addition, ``replace`` supports passing a result object from successive
+replacement calls through an optional keyword argument named ``result`` with
+a defaut value, e.g. ``result=None``.
 
-Even without any of these arguments, such a *do nothing wrapper* can be used
+Even without any of these arguments, such an *empty wrapper* can be used
 to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
@@ -410,26 +413,71 @@
 
 .. _F signature:
 
 While ``before`` calls ``print_message`` with its default parameters the
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``.
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the
 passing of any function with optional positional and keyword parameters.
-Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")``
+Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
-A rather more complex example illustrates the replacement of the original
-functionality with a sequence of replacement functionalities, passing a
-``result`` object of type ``int`` between successive calls.
+The idea behind the ``replace`` option is not so much to replace the complete
+original functionality, because you could simply create your own functionality
+for that but to wrap the original functionality, e.g. according to the principle:
+
+#. Edit the call parameters for the original functionality
+#. Execute the original functionality with these modified call parameters
+#. Edit the result and return this modified result
+
+This could then look like this:
+
+.. code-block:: python
+
+    # *** example_wrapper.py - enclose and replacing original function
+
+    # Case 3: Decoration with replace functionality
+    def replace_wrapper(value: str="replace"):
+        # 1. Edit the call parameters for the original functionality
+        value = value.upper()
+        # 2. Execute original functionality with modified call parameters
+        result = some_function.substitute.callee(value)             # (1)
+        # 3. Edit the result and return this modified result
+        return f"result: '{result}'"
+
+    @Wrapper(replace=replace_wrapper)
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+        return value
+
+    result = some_function()        # value = 'REPLACE'
+    print(result)                   # result: 'REPLACE'
+
+The first output ``value = 'REPLACE'`` comes from the original function
+``some_function()`` but using parameters modified by the
+``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
+of the ``return`` modified by the ``replace_wrapper()``. Please note the line
+marked with ``(1)`` in the ``replace_wrapper()``: It is very important
+to avoid self-recursions:
+
+    **Hint** --- Avoidance of self-recursion in the replace wrapper
+
+    *In the replace wrapper, the undecorated version of the original
+    functionality must always be called. It is accessible via the*
+    ``substitute.callee`` *method of the wrapper!*
+
+For the sake of completeness, a rather more complex example illustrates
+the replacement of the original functionality with a sequence of replacement
+functionalities, passing a ``result`` object of type ``int`` between
+successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
-    # Case 3: Decoration with before, after and multiple replacements
+    # Case 4: Decoration with before, after and multiple replacements
     def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
@@ -462,15 +510,15 @@
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
-    # Case 4: Decoration of a class always refers to __init__
+    # Case 5: Decoration of a class always refers to __init__
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
@@ -485,15 +533,15 @@
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
-    # Case 5: Define a private wrapper library
+    # Case 6: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
     # Multiple decorations for specialized functionality encapsulation
     @before_wrapper
     @after_wrapper
     def some_function(value: str = "original"):
@@ -1006,14 +1054,19 @@
 it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.5.*, Build: 2023-06-21**
+
+- Pre production state, version 0.9.* for module
+    - wrapper [ ``python -m decoratory.wrapper --version`` ]
+
 **Version: 0.1.4.*, Build: 2023-06-21**
 
 - A new subclass SemiSingleton for a resettable singleton
 - Accessible parameter for singleton and multiton removed
 - Additional test and documentation
 - Pre production state, version 0.9.* for modules
     - singleton [ ``python -m decoratory.singleton --version`` ]
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory/__main__.py` & `decoratory-0.1.5.6/Sources/decoratory/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.4.13"
+__version__ = "0.1.5.6"
 __date__ = "2023-06-21"
-__time__ = "08:36:06"
+__time__ = "13:44:05"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory/banner.py` & `decoratory-0.1.5.6/Sources/decoratory/banner.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/Sources/decoratory/basic.py` & `decoratory-0.1.5.6/Sources/decoratory/basic.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/Sources/decoratory/multiton.py` & `decoratory-0.1.5.6/Sources/decoratory/multiton.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     Methods
     -------
         None.
 
     Examples
     --------
 
+    # -------------------------------------------------------------------------
     from decoratory.multiton import Multiton
 
     @Multiton(key=lambda spec, name: name)
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
@@ -124,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-20"
-__time__ = "16:08:29"
+__version__ = "0.9.0.2"
+__date__ = "2023-06-21"
+__time__ = "12:46:42"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -179,15 +180,15 @@
         Sets the internal dictionary of instances
 
     reset(self) -> None:            (if resettable=True, only!)
         Resets the multiton instance dictionary
     """
 
     def __init__(self,
-                 substitute: type = None,
+                 substitute: Union[type, callable, None] = None,
                  *args: object,
                  key: Union[F, callable, object, None] = None,
                  resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a multiton.
 
         Parameters:
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory/observer.py` & `decoratory-0.1.5.6/Sources/decoratory/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,17 +409,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.2"
-__date__ = "2023-06-19"
-__time__ = "18:25:39"
+__version__ = "0.1.3.3"
+__date__ = "2023-06-21"
+__time__ = "12:46:42"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -603,18 +603,18 @@
     -------
         None.
     """
 
     BaseClass = BaseObservable
 
     def __init__(self,
-                 substitute: Union[callable, type] = None,
+                 substitute: Union[type, callable, None] = None,
                  *args: object,
-                 observers: Union[list, F, callable, str] = None,
-                 methods: Union[list, F, callable, str] = None,
+                 observers: Union[list, callable, F, str, None] = None,
+                 methods: Union[list, callable, F, str, None] = None,
                  activate: Activation = Activation.AFTER,
                  **kwargs: object) -> None:
         """Observable (Publisher, Subject).
 
         Parameters:
             substitute (callable|type: Callable|Type to be made an observable
             observers (list|F|callable|str): (List of) callable(s) of observers
@@ -785,18 +785,18 @@
     -------
         None.
    """
 
     BaseClass = BaseObserver
 
     def __init__(self,
-                 substitute: Union[callable, type] = None,
+                 substitute: Union[type, callable, None] = None,
                  *args: object,
-                 observables: Union[list, X, callable, str] = None,
-                 methods: Union[list, X, callable, str] = None,
+                 observables: Union[list, callable, X, str, None] = None,
+                 methods: Union[list, callable, X, str, None] = None,
                  **kwargs: object) -> None:
         """**Observer** (Subscriber, Object)
 
         Parameters:
             substitute (callable|type: Callable|Type to be made an observable
             observables (list|X|callable|str): (List of) callable(s) of observables
             methods (list|X|callable|str): (List of) callable(s) of as strings
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory/singleton.py` & `decoratory-0.1.5.6/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,26 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-20"
-__time__ = "16:08:29"
+__version__ = "0.9.0.2"
+__date__ = "2023-06-21"
+__time__ = "12:46:42"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
+from typing import Union
 from decoratory.basic import F
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Singleton:
     """**Singleton**
@@ -119,19 +120,19 @@
 
     Methods
     -------
     get_instance(self) -> object:
         Return the singleton instance (primary instance)
 
     reset(self) -> None:            (if resettable=True, only!)
-        Resets the singleton instance
+        Resets the singleton instance (None)
     """
 
     def __init__(self,
-                 substitute: object = None,
+                 substitute: Union[type, callable, None] = None,
                  *args: object,
                  resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a singleton.
 
         Parameters:
             substitute (object): A type to be made a singleton
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory/wrapper.py` & `decoratory-0.1.5.6/Sources/decoratory/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,75 +29,95 @@
     Methods
     -------
         None.
 
     Examples
     --------
 
+    # -------------------------------------------------------------------------
     from decoratory.wrapper import Wrapper
-    from decoratory.basic import F
 
     # Case 1: Dynamic decoration with decorator arguments, only
     def some_function(value: str = "original"):
         print(f"value = '{value}'")
 
+    # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
-    # Case 2: Static decoration with before and after functionalities
+    # -------------------------------------------------------------------------
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    # Case 2: Decoration with before and after functionalities
     def print_message(message: str = "ENTER"):
         print(message)
 
     @Wrapper(before=print_message, after=F(print_message, "LEAVE"))
     def some_function(value: str = "original"):
         print(f"value = '{value}'")
 
-    # Function call with decoration: before and after
     some_function()                 # ENTER
                                     # value = 'original'
                                     # LEAVE
 
-    # Case 3: Decoration with before, after and multiple replacements
-    def print_message(message: str = "BEFORE"):
+    # Case 3: Decoration with replace functionality
+    def replace_wrapper(value: str="replace"):
+        # 1. Edit the call parameters for the original functionality
+        value = value.upper()
+        # 2. Execute original functionality with modified call parameters
+        result = some_function.substitute.callee(value)             # (1)
+        # 3. Edit the result and return this modified result
+        return f"result: '{result}'"
+
+    @Wrapper(replace=replace_wrapper)
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+        return value
+
+    result = some_function()        # value = 'REPLACE'
+    print(result)                   # result: 'REPLACE'
+
+    # Case 4: Decoration with before, after and multiple replacements
+    def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
 
-    @Wrapper(before=F(print_message, "ENTER"),
+    @Wrapper(before=F(print, "ENTER"), # Python's print()
              replace=[F(replacement_printer, 1, result=0),
                       F(replacement_printer, 3),
                       F(replacement_printer, 5)],
              after=F(print_message, "LEAVE"))
-    def default_printer(message: str = "DEFAULT"):
+    def result_printer(message: str = "UNKNOWN"):
         print(message)
 
-    # Function call with decoration: before, after and replacement
-    default_printer()               # ENTER         (before)
+    result_printer()                # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
 
-    # Case 4: Decoration of a class always refers to __init__
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
+    # Case 5: Decoration of a class always refers to __init__
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
-    # Case 5: Define a private wrapper library
+    # Case 6: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
     # Multiple decorations for specialized functionality encapsulation
     @before_wrapper
     @after_wrapper
     def some_function(value: str = "original"):
@@ -116,25 +136,26 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.7"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.9.0.2"
+__date__ = "2023-06-21"
+__time__ = "12:48:50"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
+from typing import Union
 from decoratory.basic import F, Parser
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Wrapper:
     """**Wrapper**
@@ -157,19 +178,19 @@
 
     Methods
     -------
         None.
     """
 
     def __init__(self,
-                 substitute: callable or type = None,
+                 substitute: Union[type, callable, None] = None,
                  *args: object,
-                 before: callable or list = None,
-                 replace: callable or list = None,
-                 after: callable or list = None,
+                 before: Union[callable, list, None] = None,
+                 replace: Union[callable, list, None] = None,
+                 after: Union[callable, list, None] = None,
                  **kwargs: object) -> None:
         """Set up a wrapper.
 
         Parameters:
             substitute (object): A type to be made a wrapper.
             before (object): (List of) callable(s) to be executed before
             replace (object): (List of) callable(s) replacing the substitute
@@ -200,17 +221,17 @@
         else:  # *** Wrapper ***
             # Action BEFORE
             if self.__get__before():
                 for before in self.__get__before():
                     before.eval()
 
             # Delegation vs. REPLACE
+            result = None
             if self.__get__replace():
                 # Replacement
-                result = None
                 if args or kwargs:
                     for replace in self.__get__replace():
                         d = replace.callee.__kwdefaults__
                         if d and 'result' in d:
                             d['result'] = result
                         result = F(replace.callee, *args, **kwargs).eval()
                 else:
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.5.6/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.4.13
+Version: 0.1.5.6
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -36,18 +36,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: License.txt
 
 
 .. _top:
 
+
 ==============================================================================
 Decoratory
 ==============================================================================
 
+
 **Introduction**
 
 The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
@@ -66,14 +68,15 @@
 In particular, there is a *comprehensive unit test* for each module, which
 can be executed from the command line using the ``--test`` option. ::
 
     python -m decoratory --test
 
 .. _toc:
 
+
 **Package Contents**
 
 The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
@@ -383,32 +386,32 @@
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
 
 * (optional) ``before`` call functionality
 
-and/or
+and/or an
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an
 
 * (optional) ``replace`` call functionality.
 
 This generic Wrapper is all the more broadly applicable, the more flexibly
 these three activities can be formulated. All three decorator parameters,
 ``before``, ``after`` and ``replace``, can be combined with each other and
 support both single callables and (nested) lists of ``F``-types
 (imported from module decoratory.basic, see `F signature`_ below for details).
-In addition, ``replace`` supports passing results from successive
-replacement calls through an optional keyword argument named ``result``
-(defaut value is ``None``).
+In addition, ``replace`` supports passing a result object from successive
+replacement calls through an optional keyword argument named ``result`` with
+a defaut value, e.g. ``result=None``.
 
-Even without any of these arguments, such a *do nothing wrapper* can be used
+Even without any of these arguments, such an *empty wrapper* can be used
 to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
@@ -449,26 +452,71 @@
 
 .. _F signature:
 
 While ``before`` calls ``print_message`` with its default parameters the
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``.
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the
 passing of any function with optional positional and keyword parameters.
-Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")``
+Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
-A rather more complex example illustrates the replacement of the original
-functionality with a sequence of replacement functionalities, passing a
-``result`` object of type ``int`` between successive calls.
+The idea behind the ``replace`` option is not so much to replace the complete
+original functionality, because you could simply create your own functionality
+for that but to wrap the original functionality, e.g. according to the principle:
+
+#. Edit the call parameters for the original functionality
+#. Execute the original functionality with these modified call parameters
+#. Edit the result and return this modified result
+
+This could then look like this:
+
+.. code-block:: python
+
+    # *** example_wrapper.py - enclose and replacing original function
+
+    # Case 3: Decoration with replace functionality
+    def replace_wrapper(value: str="replace"):
+        # 1. Edit the call parameters for the original functionality
+        value = value.upper()
+        # 2. Execute original functionality with modified call parameters
+        result = some_function.substitute.callee(value)             # (1)
+        # 3. Edit the result and return this modified result
+        return f"result: '{result}'"
+
+    @Wrapper(replace=replace_wrapper)
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+        return value
+
+    result = some_function()        # value = 'REPLACE'
+    print(result)                   # result: 'REPLACE'
+
+The first output ``value = 'REPLACE'`` comes from the original function
+``some_function()`` but using parameters modified by the
+``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
+of the ``return`` modified by the ``replace_wrapper()``. Please note the line
+marked with ``(1)`` in the ``replace_wrapper()``: It is very important
+to avoid self-recursions:
+
+    **Hint** --- Avoidance of self-recursion in the replace wrapper
+
+    *In the replace wrapper, the undecorated version of the original
+    functionality must always be called. It is accessible via the*
+    ``substitute.callee`` *method of the wrapper!*
+
+For the sake of completeness, a rather more complex example illustrates
+the replacement of the original functionality with a sequence of replacement
+functionalities, passing a ``result`` object of type ``int`` between
+successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
-    # Case 3: Decoration with before, after and multiple replacements
+    # Case 4: Decoration with before, after and multiple replacements
     def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
@@ -501,15 +549,15 @@
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
-    # Case 4: Decoration of a class always refers to __init__
+    # Case 5: Decoration of a class always refers to __init__
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
@@ -524,15 +572,15 @@
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
-    # Case 5: Define a private wrapper library
+    # Case 6: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
     # Multiple decorations for specialized functionality encapsulation
     @before_wrapper
     @after_wrapper
     def some_function(value: str = "original"):
@@ -1045,14 +1093,19 @@
 it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.5.*, Build: 2023-06-21**
+
+- Pre production state, version 0.9.* for module
+    - wrapper [ ``python -m decoratory.wrapper --version`` ]
+
 **Version: 0.1.4.*, Build: 2023-06-21**
 
 - A new subclass SemiSingleton for a resettable singleton
 - Accessible parameter for singleton and multiton removed
 - Additional test and documentation
 - Pre production state, version 0.9.* for modules
     - singleton [ ``python -m decoratory.singleton --version`` ]
```

### Comparing `decoratory-0.1.4.13/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.1.5.6/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/Unittest/test_basic.py` & `decoratory-0.1.5.6/Unittest/test_basic.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/Unittest/test_multiton.py` & `decoratory-0.1.5.6/Unittest/test_multiton.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.10"
-__date__ = "2023-06-20"
-__time__ = "16:08:29"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-21"
+__time__ = "13:37:48"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.1.4.13/Unittest/test_observer.py` & `decoratory-0.1.5.6/Unittest/test_observer.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.4.13/Unittest/test_singleton.py` & `decoratory-0.1.5.6/Unittest/test_singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.9"
-__date__ = "2023-06-20"
-__time__ = "10:56:59"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-21"
+__time__ = "13:37:48"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.1.4.13/Unittest/test_wrapper.py` & `decoratory-0.1.5.6/Unittest/test_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.7"
-__date__ = "2023-06-19"
-__time__ = "18:25:39"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-21"
+__time__ = "13:37:48"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -50,47 +50,47 @@
         # Result list
         res = list()
 
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__}: '{txt}'")
 
-        Printer = Wrapper(printer, "Customized text")
+        wrp_printer = Wrapper(printer, "Customized text")
 
         # ---------------------------------------------------------------------
-        # Basic checks
-        self.assertTrue(isinstance(Printer, Wrapper))
+        # Checks
+        self.assertTrue(isinstance(wrp_printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
-        Printer()
+        wrp_printer()
         self.assertListEqual(res, ["printer: 'Customized text'"])
 
-        Printer = Wrapper(printer, txt="Customized phrase")
+        wrp_printer = Wrapper(printer, txt="Customized phrase")
 
         res.clear()
-        Printer()
+        wrp_printer()
         self.assertListEqual(res, ["printer: 'Customized phrase'"])
 
     def test_decoration_nobrackets(self):
         """Unittest: Wrapper without brackets"""
 
         # Result list
         res = list()
 
         @Wrapper
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["printer: 'Default text'"])
 
     def test_decoration_empty_brackets(self):
         """Unittest: Wrapper with empty brackets"""
 
@@ -99,18 +99,18 @@
 
         @Wrapper()
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["printer: 'Default text'"])
 
     def test_decoration_before_after(self):
         """Unittest: Wrapper with before and after activities"""
 
@@ -127,18 +127,18 @@
 
         @Wrapper(before=before_printer, after=after_printer)
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["before_printer: 'BEFORE'",
                                    "printer: 'Default text'",
                                    "after_printer: 'AFTER'"])
 
     def test_decoration_replace(self):
@@ -153,22 +153,53 @@
 
         @Wrapper(replace=replace_printer)
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["replace_printer: 'REPLACE'"])
 
+    def test_decoration_replace_wrapper(self):
+        """Unittest: Wrapper with replace wrapper"""
+
+        # Result list
+        res = list()
+
+        def replace_wrapper(value: str = "replace"):
+            """The replace wrapper"""
+            # 1. Edit the call parameters for the original functionality
+            value = value.upper()
+            # 2. Execute original functionality with modified call parameters
+            result = printer.substitute.callee(value)  # (1)
+            # 3. Edit the result and return this modified result
+            return f"result: '{result}'"
+
+        @Wrapper(replace=replace_wrapper)
+        def printer(txt: str = "Default text"):
+            """The default printer"""
+            res.append(f"{printer.__name__}: '{txt}'")
+            return txt
+
+        # ---------------------------------------------------------------------
+        # Checks
+        self.assertTrue(isinstance(printer, Wrapper))
+
+        # Call
+        res.clear()
+        res.append(printer())
+        self.assertListEqual(res, ["printer: 'REPLACE'",
+                                   "result: 'REPLACE'"])
+
     def test_decoration_before_after_lists(self):
         """Unittest: Wrapper with list of before and after activities"""
 
         # Result list
         res = list()
 
         def before_printer(txt: str = "Before text"):
@@ -186,18 +217,18 @@
                         F(after_printer, "Text01"),
                         F(after_printer, txt="Text02")])
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__:14s}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["before_printer: 'Text01'",
                                    "before_printer: 'Text02'",
                                    "before_printer: 'Before text'",
                                    "printer       : 'Default text'",
                                    "after_printer : 'After text'",
@@ -233,18 +264,18 @@
                           F(replace_printer, 3),
                           F(replace_printer, 4)])
         def printer(txt: str = "Default text"):
             """The default printer"""
             res.append(f"{printer.__name__:14s}: '{txt}'")
 
         # ---------------------------------------------------------------------
-        # Basic checks
+        # Checks
         self.assertTrue(isinstance(printer, Wrapper))
 
-        # Basic call
+        # Call
         res.clear()
         printer()
         self.assertListEqual(res, ["before_printer : 'First text'",
                                    "before_printer : 'Before text'",
                                    "replace_printer: result = 1",
                                    "replace_printer: result = 3",
                                    "replace_printer: result = 6",
```

### Comparing `decoratory-0.1.4.13/setup.py` & `decoratory-0.1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.4.13"
+__version__ = "0.1.5.6"
 __date__ = "2023-06-21"
-__time__ = "08:36:06"
+__time__ = "13:44:05"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
```

