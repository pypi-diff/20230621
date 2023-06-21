# Comparing `tmp/parsing-2.0.0.tar.gz` & `tmp/parsing-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsing-2.0.0.tar", last modified: Tue Aug 31 22:11:01 2021, max compression
+gzip compressed data, was "parsing-2.0.1.tar", last modified: Wed Jun 21 16:11:26 2023, max compression
```

## Comparing `parsing-2.0.0.tar` & `parsing-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 22:11:01.753851 parsing-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-08-31 22:10:56.000000 parsing-2.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-31 22:10:56.000000 parsing-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-31 22:10:56.000000 parsing-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5213 2021-08-31 22:11:01.753851 parsing-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2021-08-31 22:10:56.000000 parsing-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 22:11:01.749851 parsing-2.0.0/parsing/
--rw-r--r--   0 runner    (1001) docker     (121)     6326 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7301 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)    67923 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/automaton.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15970 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/glrparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11107 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/grammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/introspection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/lrparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/module_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 22:11:01.753851 parsing-2.0.0/parsing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 22:11:01.753851 parsing-2.0.0/parsing/tests/specs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/a.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/b.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/d.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/h.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/specs/i.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2021-08-31 22:10:56.000000 parsing-2.0.0/parsing/tests/test_codestyle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 22:11:01.749851 parsing-2.0.0/parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5213 2021-08-31 22:11:01.000000 parsing-2.0.0/parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      726 2021-08-31 22:11:01.000000 parsing-2.0.0/parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-31 22:11:01.000000 parsing-2.0.0/parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-31 22:11:01.000000 parsing-2.0.0/parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-31 22:11:01.000000 parsing-2.0.0/parsing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      786 2021-08-31 22:10:56.000000 parsing-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-31 22:11:01.753851 parsing-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2021-08-31 22:10:56.000000 parsing-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 16:11:22.000000 parsing-2.0.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 16:11:22.000000 parsing-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 16:11:22.000000 parsing-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-21 16:11:26.210492 parsing-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-21 16:11:22.000000 parsing-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.206492 parsing-2.0.1/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68232 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/automaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/glrparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/lrparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/module_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing/tests/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/h.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/test_codestyle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-21 16:11:22.000000 parsing-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:11:26.210492 parsing-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-21 16:11:22.000000 parsing-2.0.1/setup.py
```

### Comparing `parsing-2.0.0/LICENSE` & `parsing-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/PKG-INFO` & `parsing-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: parsing
-Version: 2.0.0
-Summary: A pure-Python module that implements an LR(1) parser generator, as well as CFSM and GLR parser drivers.
+Version: 2.0.1
+Summary: LR(1) parser generator for Python
 Home-page: http://www.canonware.com/Parsing/
 Author: Jason Evans
 Author-email: jasone@canonware.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Text Processing :: General
@@ -120,9 +119,7 @@
 
 Additionally, trying to set private attributes may raise:
   * AttributeError
 
 Author: Jason Evans jasone@canonware.com
 
 Github repo: http://github.com/MagicStack/parsing
-
-
```

### Comparing `parsing-2.0.0/README.rst` & `parsing-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/__init__.py` & `parsing-2.0.1/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/_version.py` & `parsing-2.0.1/parsing/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # The commit message MUST contain a properly formatted release
 # log, and the commit must be signed.
 #
 # The release automation will: build and test the packages for the
 # supported platforms, publish the packages on PyPI, merge the PR
 # to the target branch, create a Git tag pointing to the commit.
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
```

### Comparing `parsing-2.0.0/parsing/ast.py` & `parsing-2.0.1/parsing/ast.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/automaton.py` & `parsing-2.0.1/parsing/automaton.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,26 @@
 
 class Spec(interfaces.Spec):
     """
     The Spec class contains the read-only data structures that the Parser
     class needs in order to parse input.  Parser generation results in a
     Spec instance, which can then be shared by multiple Parser instances."""
 
+    __deletable__ = [
+        '_itemSets',
+        '_itemSetsHash',
+        '_nonterms',
+        '_precedences',
+        '_productions',
+        '_startSym',
+        '_startProd',
+        '_startState',
+        '_tokens',
+    ]
+
     _sym2spec: dict[type[Symbol], SymbolSpec]
 
     def sym_spec(self, sym: Symbol) -> SymbolSpec:
         return self._sym2spec[type(sym)]
 
     def actions(self) -> list[ActionState]:
         return self._action
@@ -1380,31 +1392,32 @@
         # first set.
         done = False
         while not done:
             done = True
             for name in self._nonterms:
                 nonterm = self._nonterms[name]
                 for prod in nonterm.productions:
-                    # Merge epsilon if there is an empty production.
-                    if len(prod.rhs) == 0:
-                        if not nonterm.firstSetMerge(epsilon):
-                            done = False
-
+                    mergeEpsilon = True
                     # Iterate through the RHS and merge the first sets into
                     # this symbol's, until a preceding symbol's first set does
                     # not contain epsilon.
                     for elm in prod.rhs:
-                        containsEpsilon = False
+                        hasEpsilon = False
                         for elmSym in elm.firstSet:
-                            if not nonterm.firstSetMerge(elmSym):
-                                done = False
                             if elmSym == epsilon:
-                                containsEpsilon = True
-                        if not containsEpsilon:
+                                hasEpsilon = True
+                            elif not nonterm.firstSetMerge(elmSym):
+                                done = False
+                        if not hasEpsilon:
+                            mergeEpsilon = False
                             break
+                    # Merge epsilon if it was in the first set of every symbol.
+                    if mergeEpsilon:
+                        if not nonterm.firstSetMerge(epsilon):
+                            done = False
 
     # Compute the follow sets for all symbols.
     def _followSets(self) -> None:
         self._startSym.followSet = {epsilon}
 
         # Repeat the following loop until no more symbols can be added to any
         # follow set.
```

### Comparing `parsing-2.0.0/parsing/errors.py` & `parsing-2.0.1/parsing/errors.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/glrparser.py` & `parsing-2.0.1/parsing/glrparser.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/grammar.py` & `parsing-2.0.1/parsing/grammar.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/interfaces.py` & `parsing-2.0.1/parsing/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/lrparser.py` & `parsing-2.0.1/parsing/lrparser.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/module_spec.py` & `parsing-2.0.1/parsing/module_spec.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/specs/a.py` & `parsing-2.0.1/parsing/tests/specs/a.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/specs/b.py` & `parsing-2.0.1/parsing/tests/specs/b.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/specs/d.py` & `parsing-2.0.1/parsing/tests/specs/d.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/specs/h.py` & `parsing-2.0.1/parsing/tests/specs/h.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/specs/i.py` & `parsing-2.0.1/parsing/tests/specs/i.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/test_basic.py` & `parsing-2.0.1/parsing/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing/tests/test_codestyle.py` & `parsing-2.0.1/parsing/tests/test_codestyle.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/parsing.egg-info/PKG-INFO` & `parsing-2.0.1/parsing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: parsing
-Version: 2.0.0
-Summary: A pure-Python module that implements an LR(1) parser generator, as well as CFSM and GLR parser drivers.
+Version: 2.0.1
+Summary: LR(1) parser generator for Python
 Home-page: http://www.canonware.com/Parsing/
 Author: Jason Evans
 Author-email: jasone@canonware.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Text Processing :: General
@@ -120,9 +119,7 @@
 
 Additionally, trying to set private attributes may raise:
   * AttributeError
 
 Author: Jason Evans jasone@canonware.com
 
 Github repo: http://github.com/MagicStack/parsing
-
-
```

### Comparing `parsing-2.0.0/parsing.egg-info/SOURCES.txt` & `parsing-2.0.1/parsing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsing-2.0.0/pyproject.toml` & `parsing-2.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 [project]
-requires-python = ">=3.7"
+name = "parsing"
+description = "LR(1) parser generator for Python"
+requires-python = ">=3.7.0"
+dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 79
@@ -26,11 +29,9 @@
 no_implicit_optional = true
 warn_unused_ignores = true
 warn_return_any = true
 no_implicit_reexport = true
 strict_equality = true
 
 [[tool.mypy.overrides]]
-module = [
-    "parsing.tests.*",
-]
+module = ["parsing.tests.*"]
 ignore_errors = true
```

### Comparing `parsing-2.0.0/setup.py` & `parsing-2.0.1/setup.py`

 * *Files identical despite different names*

