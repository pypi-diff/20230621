# Comparing `tmp/ast_scope-0.4.0.tar.gz` & `tmp/ast_scope-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_scope-0.4.0.tar", last modified: Tue Jun 13 18:37:26 2023, max compression
+gzip compressed data, was "ast_scope-0.4.1.tar", last modified: Wed Jun 21 06:00:42 2023, max compression
```

## Comparing `ast_scope-0.4.0.tar` & `ast_scope-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.600108 ast_scope-0.4.0/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.4.0/LICENSE
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 18:37:26.600108 ast_scope-0.4.0/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.4.0/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.596109 ast_scope-0.4.0/ast_scope/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 06:23:11.000000 ast_scope-0.4.0/ast_scope/annotate.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     7848 2023-06-13 06:26:29.000000 ast_scope-0.4.0/ast_scope/annotator.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/graph.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/group_similar_constructs.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3507 2023-06-13 18:35:03.000000 ast_scope-0.4.0/ast_scope/pull_scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2677 2023-06-13 18:35:49.000000 ast_scope-0.4.0/ast_scope/scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/utils.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.596109 ast_scope-0.4.0/ast_scope.egg-info/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      709 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/SOURCES.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/dependency_links.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/requires.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/top_level.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 18:37:26.600108 ast_scope-0.4.0/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 18:37:12.000000 ast_scope-0.4.0/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.600108 ast_scope-0.4.0/tests/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/argument_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/assignment_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/basic_scope_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/class_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/comprehension_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/dependency_graph_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      356 2023-06-13 06:26:41.000000 ast_scope-0.4.0/tests/exception_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/function_frame_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/lambda_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/nonlocal_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/special_symbols_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-21 06:00:42.886938 ast_scope-0.4.1/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.4.1/LICENSE
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3809 2023-06-21 06:00:42.886938 ast_scope-0.4.1/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.4.1/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-21 06:00:42.882938 ast_scope-0.4.1/ast_scope/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.4.1/ast_scope/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 06:23:11.000000 ast_scope-0.4.1/ast_scope/annotate.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     7848 2023-06-13 06:26:29.000000 ast_scope-0.4.1/ast_scope/annotator.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.4.1/ast_scope/graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.4.1/ast_scope/group_similar_constructs.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3507 2023-06-13 18:35:03.000000 ast_scope-0.4.1/ast_scope/pull_scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2722 2023-06-21 06:00:17.000000 ast_scope-0.4.1/ast_scope/scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.4.1/ast_scope/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-21 06:00:42.882938 ast_scope-0.4.1/ast_scope.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3809 2023-06-21 06:00:42.000000 ast_scope-0.4.1/ast_scope.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      709 2023-06-21 06:00:42.000000 ast_scope-0.4.1/ast_scope.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-21 06:00:42.000000 ast_scope-0.4.1/ast_scope.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-21 06:00:42.000000 ast_scope-0.4.1/ast_scope.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-21 06:00:42.000000 ast_scope-0.4.1/ast_scope.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-21 06:00:42.886938 ast_scope-0.4.1/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-21 06:00:22.000000 ast_scope-0.4.1/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-21 06:00:42.886938 ast_scope-0.4.1/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/argument_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/assignment_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/basic_scope_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/class_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/comprehension_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/dependency_graph_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      356 2023-06-13 06:26:41.000000 ast_scope-0.4.1/tests/exception_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/function_frame_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/lambda_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/nonlocal_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/special_symbols_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.4.1/tests/utils.py
```

### Comparing `ast_scope-0.4.0/LICENSE` & `ast_scope-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/PKG-INFO` & `ast_scope-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: ast_scope
-Version: 0.4.0
-Summary: Annotates a Python AST with the scope of symbols.
-Home-page: https://github.com/kavigupta/ast_scope
-Author: Kavi Gupta
-Author-email: ast_scope@kavigupta.org
-License: UNKNOWN
-Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # ast_scope
 
 This package is an implementation of Python's lexical scoping rules. It's interface is simple, you pass in an AST object to the `annotate` function, and it provides a mapping from each node in the tree that represents a symbol to the containing scope.
 
 ## Example Usage: Get Global Symbols
 
@@ -113,9 +94,7 @@
 ```
 # run the annotator
 scope_info = ast_scope.annotate(tree)
 scope_x = scope_info[last_x]
 ```
 
 You should get a `FunctionScope` object which contains a bunch of information about the other variables, etc., in the scope, but also `scope_x.function_node`, a pointer to the node containing the `def` statement for `f`.
-
-
```

### Comparing `ast_scope-0.4.0/README.md` & `ast_scope-0.4.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,118 @@
-
-# ast_scope
-
-This package is an implementation of Python's lexical scoping rules. It's interface is simple, you pass in an AST object to the `annotate` function, and it provides a mapping from each node in the tree that represents a symbol to the containing scope.
-
-## Example Usage: Get Global Symbols
-
-Let's say you have the code
-
-```
-code = """
-def f():
-    x = 3
-    lambda z: theta
-    return x + y
-"""
-```
-
-and you want to determine which global variables are referenced by it. All you need to do is run
-
-```
-import ast
-import ast_scope
-tree = ast.parse(code)
-scope_info = ast_scope.annotate(tree)
-global_variables = sorted(scope_info.global_scope.symbols_in_frame)
-```
-
-Once you have executed this code, `global_variables` will be bound to `['f', 'theta', 'y']`.
-
-## Example Usage: Get Dependency Graph
-
-Let's say you have the code
-
-```
-code = """
-def hailstone(n):
-    if n == 1:
-        return 1
-    if n % 2 == 0:
-        return hailstone(n // 2)
-    if n % 2 == 1:
-        return hailstone(3 * n + 1)
-
-def mapper(f, lst):
-    return list(map(f, lst))
-
-def lrange(n):
-    return list(range(n))
-
-def main():
-    return mapper(hailstone, lrange(20))
-"""
-```
-
-and you want to find the dependency graph. You can run
-
-```
-import ast
-import ast_scope
-tree = ast.parse(code)
-scope_info = ast_scope.annotate(tree)
-graph = scope_info.static_dependency_graph
-```
-
-which results in the following directed graph of dependencies between top-level functions (rendering using networkx):
-
-<img src="img/dependency_graph_example.png">
-
-See the documentation for some caveats.
-
-## Example usage: find a specific symbol's scope
-
-Take the following code:
-
-```
-code = """
-def f(x):
-    def g(x): return x()
-    return g(lambda: x)
-"""
-```
-
-First, parse the code and identify the node (in practice, you'd probably have this always).
-
-```
-import ast, ast_scope
-tree = ast.parse(code)
-last_x = tree.body[0].body[-1].value.args[0].body
-```
-
-If you want to find the scope in which the last `x` could be found, just run the annotator and look up it's scope!
-
-```
-# run the annotator
-scope_info = ast_scope.annotate(tree)
-scope_x = scope_info[last_x]
-```
-
-You should get a `FunctionScope` object which contains a bunch of information about the other variables, etc., in the scope, but also `scope_x.function_node`, a pointer to the node containing the `def` statement for `f`.
+Metadata-Version: 2.1
+Name: ast_scope
+Version: 0.4.1
+Summary: Annotates a Python AST with the scope of symbols.
+Home-page: https://github.com/kavigupta/ast_scope
+Author: Kavi Gupta
+Author-email: ast_scope@kavigupta.org
+License: UNKNOWN
+Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
+Description: 
+        # ast_scope
+        
+        This package is an implementation of Python's lexical scoping rules. It's interface is simple, you pass in an AST object to the `annotate` function, and it provides a mapping from each node in the tree that represents a symbol to the containing scope.
+        
+        ## Example Usage: Get Global Symbols
+        
+        Let's say you have the code
+        
+        ```
+        code = """
+        def f():
+            x = 3
+            lambda z: theta
+            return x + y
+        """
+        ```
+        
+        and you want to determine which global variables are referenced by it. All you need to do is run
+        
+        ```
+        import ast
+        import ast_scope
+        tree = ast.parse(code)
+        scope_info = ast_scope.annotate(tree)
+        global_variables = sorted(scope_info.global_scope.symbols_in_frame)
+        ```
+        
+        Once you have executed this code, `global_variables` will be bound to `['f', 'theta', 'y']`.
+        
+        ## Example Usage: Get Dependency Graph
+        
+        Let's say you have the code
+        
+        ```
+        code = """
+        def hailstone(n):
+            if n == 1:
+                return 1
+            if n % 2 == 0:
+                return hailstone(n // 2)
+            if n % 2 == 1:
+                return hailstone(3 * n + 1)
+        
+        def mapper(f, lst):
+            return list(map(f, lst))
+        
+        def lrange(n):
+            return list(range(n))
+        
+        def main():
+            return mapper(hailstone, lrange(20))
+        """
+        ```
+        
+        and you want to find the dependency graph. You can run
+        
+        ```
+        import ast
+        import ast_scope
+        tree = ast.parse(code)
+        scope_info = ast_scope.annotate(tree)
+        graph = scope_info.static_dependency_graph
+        ```
+        
+        which results in the following directed graph of dependencies between top-level functions (rendering using networkx):
+        
+        <img src="img/dependency_graph_example.png">
+        
+        See the documentation for some caveats.
+        
+        ## Example usage: find a specific symbol's scope
+        
+        Take the following code:
+        
+        ```
+        code = """
+        def f(x):
+            def g(x): return x()
+            return g(lambda: x)
+        """
+        ```
+        
+        First, parse the code and identify the node (in practice, you'd probably have this always).
+        
+        ```
+        import ast, ast_scope
+        tree = ast.parse(code)
+        last_x = tree.body[0].body[-1].value.args[0].body
+        ```
+        
+        If you want to find the scope in which the last `x` could be found, just run the annotator and look up it's scope!
+        
+        ```
+        # run the annotator
+        scope_info = ast_scope.annotate(tree)
+        scope_x = scope_info[last_x]
+        ```
+        
+        You should get a `FunctionScope` object which contains a bunch of information about the other variables, etc., in the scope, but also `scope_x.function_node`, a pointer to the node containing the `def` statement for `f`.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
```

### Comparing `ast_scope-0.4.0/ast_scope/annotate.py` & `ast_scope-0.4.1/ast_scope/annotate.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope/annotator.py` & `ast_scope-0.4.1/ast_scope/annotator.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope/graph.py` & `ast_scope-0.4.1/ast_scope/graph.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope/group_similar_constructs.py` & `ast_scope-0.4.1/ast_scope/group_similar_constructs.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope/pull_scope.py` & `ast_scope-0.4.1/ast_scope/pull_scope.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope/scope.py` & `ast_scope-0.4.1/ast_scope/scope.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,26 @@
     variables = attr.ib(attr.Factory(set))
     functions = attr.ib(attr.Factory(set))
     classes = attr.ib(attr.Factory(set))
     import_statements = attr.ib(attr.Factory(set))
     exceptions = attr.ib(attr.Factory(set))
 
     @property
+    def node_to_symbol(self):
+        result = {}
+        result.update({var: var.arg for var in self.arguments})
+        result.update({var: var.id for var in self.variables})
+        result.update({var: var.name for var in self.functions | self.classes})
+        result.update({var: name_of_alias(var) for var in self.import_statements})
+        result.update({var: var.name for var in self.exceptions})
+        return result
+
+    @property
     def all_symbols(self):
-        arguments = {var.arg for var in self.arguments}
-        var_names = {var.id for var in self.variables}
-        block_definitions = {var.name for var in self.functions | self.classes}
-        import_statements = {name_of_alias(var) for var in self.import_statements}
-        exceptions = {var.name for var in self.exceptions}
-        return (
-            arguments | var_names | block_definitions | import_statements | exceptions
-        )
+        return set(self.node_to_symbol.values())
 
 
 class Scope(abc.ABC):
     def __init__(self):
         self.variables = Variables()
 
     def add_argument(self, node):
```

### Comparing `ast_scope-0.4.0/ast_scope/utils.py` & `ast_scope-0.4.1/ast_scope/utils.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/ast_scope.egg-info/SOURCES.txt` & `ast_scope-0.4.1/ast_scope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/setup.py` & `ast_scope-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ast_scope", # Replace with your own username
-    version="0.4.0",
+    version="0.4.1",
     author="Kavi Gupta",
     author_email="ast_scope@kavigupta.org",
     description="Annotates a Python AST with the scope of symbols.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/ast_scope",
     download_url="https://github.com/kavigupta/ast_scope/archive/0.3.1.zip",
```

### Comparing `ast_scope-0.4.0/tests/argument_tests.py` & `ast_scope-0.4.1/tests/argument_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/assignment_tests.py` & `ast_scope-0.4.1/tests/assignment_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/basic_scope_tests.py` & `ast_scope-0.4.1/tests/basic_scope_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/class_tests.py` & `ast_scope-0.4.1/tests/class_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/comprehension_tests.py` & `ast_scope-0.4.1/tests/comprehension_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/dependency_graph_tests.py` & `ast_scope-0.4.1/tests/dependency_graph_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/function_frame_tests.py` & `ast_scope-0.4.1/tests/function_frame_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/lambda_test.py` & `ast_scope-0.4.1/tests/lambda_test.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/nonlocal_tests.py` & `ast_scope-0.4.1/tests/nonlocal_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.4.0/tests/utils.py` & `ast_scope-0.4.1/tests/utils.py`

 * *Files identical despite different names*

