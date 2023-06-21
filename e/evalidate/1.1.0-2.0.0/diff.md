# Comparing `tmp/evalidate-1.1.0.tar.gz` & `tmp/evalidate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-1.1.0.tar", last modified: Thu Jun 15 17:26:21 2023, max compression
+gzip compressed data, was "evalidate-2.0.0.tar", last modified: Wed Jun 21 16:19:19 2023, max compression
```

## Comparing `evalidate-1.1.0.tar` & `evalidate-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    11506 2023-06-15 17:26:21.318591 evalidate-1.1.0/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     8896 2023-06-15 17:25:08.000000 evalidate-1.1.0/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     7363 2023-06-15 16:52:05.000000 evalidate-1.1.0/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2406 2023-06-15 17:02:24.000000 evalidate-1.1.0/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    11506 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-1.1.0/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-15 17:26:21.318591 evalidate-1.1.0/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:03:02.000000 evalidate-1.1.0/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12056 2023-06-21 16:19:19.914970 evalidate-2.0.0/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     9286 2023-06-21 16:05:39.000000 evalidate-2.0.0/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/evalidate/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4103 2023-06-21 15:16:03.000000 evalidate-2.0.0/evalidate/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 16:18:12.000000 evalidate-2.0.0/evalidate/security.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-21 16:19:19.914970 evalidate-2.0.0/evalidate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12056 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-2.0.0/evalidate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-21 16:19:19.000000 evalidate-2.0.0/evalidate.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-21 16:19:19.914970 evalidate-2.0.0/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:03:02.000000 evalidate-2.0.0/setup.py
```

### Comparing `evalidate-1.1.0/PKG-INFO` & `evalidate-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 1.1.0
+Version: 2.0.0
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
         
+        ## Upgrade warning
+        Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+        
         ## Purpose
         Originally it's developed for filtering complex data structures e.g. 
         
         Find cheap smartphones available for sale:
         ```python
         category="smartphones" and price<300 and stock>0
         ```
@@ -58,75 +61,93 @@
         ## Exceptions
         Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
         inherit from base exception class `EvalException`.
         
         ## Configure validation
         Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
         
-        ### Allowing other nodes (operations)
         
-        Evalidate has built-in set of python operations, which are considered 'safe' (from author point of view). 
-        Code is considered valid only if all of it's operations are in this list. You can override this list by adding argument `nodes` like:
-        ```python
-        Expr('2*2', nodes=['Mult']).eval()
-        ```
+        ### EvalModel - using custom security model
+        EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
         
-        If you want to start from blank whitelist (discard built-in whitelist), use `Expr(expression, blank=True, nodes=[...])` and then add each node manually (only what you really need) 
+        You can create custom empty model (and extend it later):
+        my_model = evalidate.EvalModel()
+        (nothing is allowed by default, even `1+2` will not be considered as safe code)
         
-        ### Allowing function calls
-        Evalidate does not allow any function calls by default.
+        or you may start from `base_eval_mode` and extend it:
+        ~~~python
+        from evalidate import Expr, base_eval_model
         
-        To enable `int()` function, need to allow 'Call' node and add this function to list of allowed function:
-        ```python
-        Expr('int(36.6)', nodes=['Call'], funcs=['int']).eval()
-        ```
-        If you want to call str methods:
-        ```python
-        Expr('name.startswith("John")', nodes=['Attribute', 'Call'], attrs=['startswith']).eval(dict(name='John Doe'))
-        ```
+        my_model = base_eval_model.clone()
+        my_model.nodes.append('Mult')
+        
+        Expr('2*2', model=my_model).eval()
+        ~~~
+        
+        To enable `int()` function, need to allow `'Call'` node and add this function to list of allowed function:
+        
+        ~~~python
+        my_model.nodes.append('Call')
+        my_model.allowed_functions.append('int')
+        
+        Expr('int(36.6)', model=my_model).eval()
+        ~~~
+        
+        Or, to call attributes:
+        ~~~python
+        m = evalidate.base_eval_model.clone()
+        m.nodes.extend(['Call', 'Attribute'])
+        m.attributes.append('startswith')
+        
+        
+        src = '"abcdef".startswith("abc")'
+        r = evalidate.Expr(src, model=m).eval()
+        ~~~
         
         But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
         
         
         ### Exporting my functions to eval code
-        ~~~
+        ~~~python
         def one():
           return 1
         
-        Expr('one()', nodes=['Call'], my_funcs={"one": one}).eval()
+        m = base_eval_model.clone()
+        m.nodes.append('Call')
+        Expr('one()', model=m).eval()
         ~~~
         
         ## Improve speed by using native eval() with validated code
         Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
         
-        ~~~
+        ~~~python
         from evalidate import Expr
         
         d = dict(a=1, b=2)
         expr = Expr('a+b')
         eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
         ~~~
         
         This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
         
         Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
         
         ## Limitations
         
-        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) and returns [AST node](https://docs.python.org/3/library/ast.html#node-classes).
+        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) to get [AST node](https://docs.python.org/3/library/ast.html#node-classes) to validate it.
         
         >Warning
         >
         >It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
         
         In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
         
         
         ### evalidate.security.test_security()
-        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (addnodes/safenodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
+        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (nodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
         
         This code will never print (I hope).
         ~~~python
         from evalidate.security import test_security
         
         test_security() or print("default rules are vulnerable!")
         ~~~
@@ -217,18 +238,17 @@
         
         While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
         - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
         - user can provide source code which runs very long time and consumes many resources 
         
         
         [simpleeval](https://github.com/danthedeckie/simpleeval)
-        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
-        
+        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is few times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
         
-        evalidate is good to run short same code against different data.
+        evalidate is good to run same expression against different data.
         
         ## Benchmarking
         We use `benchmark/benchmark.py` in this repository.
         We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
         
         ~~~
         Products: 1000000 items
@@ -236,15 +256,15 @@
         evalidate_eval(): 0.326s
         test_simpleeval(): 1.824s
         test_asteval(): 26.106s
         ~~~
         
         As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
         
-        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
+        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. (Benchmark code must assume expression as unknown in advance and untrusted)
         
         
         ## Read about eval() risks
         
         - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
         - https://netsec.expert/posts/breaking-python3-eval-protections/
         - https://realpython.com/python-eval-function/
```

### Comparing `evalidate-1.1.0/README.md` & `evalidate-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ﻿# Evalidate
 Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
 
+## Upgrade warning
+Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+
 ## Purpose
 Originally it's developed for filtering complex data structures e.g. 
 
 Find cheap smartphones available for sale:
 ```python
 category="smartphones" and price<300 and stock>0
 ```
@@ -50,75 +53,93 @@
 ## Exceptions
 Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
 inherit from base exception class `EvalException`.
 
 ## Configure validation
 Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
 
-### Allowing other nodes (operations)
 
-Evalidate has built-in set of python operations, which are considered 'safe' (from author point of view). 
-Code is considered valid only if all of it's operations are in this list. You can override this list by adding argument `nodes` like:
-```python
-Expr('2*2', nodes=['Mult']).eval()
-```
+### EvalModel - using custom security model
+EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
 
-If you want to start from blank whitelist (discard built-in whitelist), use `Expr(expression, blank=True, nodes=[...])` and then add each node manually (only what you really need) 
+You can create custom empty model (and extend it later):
+my_model = evalidate.EvalModel()
+(nothing is allowed by default, even `1+2` will not be considered as safe code)
 
-### Allowing function calls
-Evalidate does not allow any function calls by default.
+or you may start from `base_eval_mode` and extend it:
+~~~python
+from evalidate import Expr, base_eval_model
 
-To enable `int()` function, need to allow 'Call' node and add this function to list of allowed function:
-```python
-Expr('int(36.6)', nodes=['Call'], funcs=['int']).eval()
-```
-If you want to call str methods:
-```python
-Expr('name.startswith("John")', nodes=['Attribute', 'Call'], attrs=['startswith']).eval(dict(name='John Doe'))
-```
+my_model = base_eval_model.clone()
+my_model.nodes.append('Mult')
+
+Expr('2*2', model=my_model).eval()
+~~~
+
+To enable `int()` function, need to allow `'Call'` node and add this function to list of allowed function:
+
+~~~python
+my_model.nodes.append('Call')
+my_model.allowed_functions.append('int')
+
+Expr('int(36.6)', model=my_model).eval()
+~~~
+
+Or, to call attributes:
+~~~python
+m = evalidate.base_eval_model.clone()
+m.nodes.extend(['Call', 'Attribute'])
+m.attributes.append('startswith')
+
+
+src = '"abcdef".startswith("abc")'
+r = evalidate.Expr(src, model=m).eval()
+~~~
 
 But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
 
 
 ### Exporting my functions to eval code
-~~~
+~~~python
 def one():
   return 1
 
-Expr('one()', nodes=['Call'], my_funcs={"one": one}).eval()
+m = base_eval_model.clone()
+m.nodes.append('Call')
+Expr('one()', model=m).eval()
 ~~~
 
 ## Improve speed by using native eval() with validated code
 Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
 
-~~~
+~~~python
 from evalidate import Expr
 
 d = dict(a=1, b=2)
 expr = Expr('a+b')
 eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
 ~~~
 
 This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
 
 Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
 
 ## Limitations
 
-evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) and returns [AST node](https://docs.python.org/3/library/ast.html#node-classes).
+evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) to get [AST node](https://docs.python.org/3/library/ast.html#node-classes) to validate it.
 
 >Warning
 >
 >It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
 
 In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
 
 
 ### evalidate.security.test_security()
-Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (addnodes/safenodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
+Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (nodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
 
 This code will never print (I hope).
 ~~~python
 from evalidate.security import test_security
 
 test_security() or print("default rules are vulnerable!")
 ~~~
@@ -209,18 +230,17 @@
 
 While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
 - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
 - user can provide source code which runs very long time and consumes many resources 
 
 
 [simpleeval](https://github.com/danthedeckie/simpleeval)
-Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
-
+Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is few times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
 
-evalidate is good to run short same code against different data.
+evalidate is good to run same expression against different data.
 
 ## Benchmarking
 We use `benchmark/benchmark.py` in this repository.
 We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
 
 ~~~
 Products: 1000000 items
@@ -228,15 +248,15 @@
 evalidate_eval(): 0.326s
 test_simpleeval(): 1.824s
 test_asteval(): 26.106s
 ~~~
 
 As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
 
-Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
+Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. (Benchmark code must assume expression as unknown in advance and untrusted)
 
 
 ## Read about eval() risks
 
 - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
 - https://netsec.expert/posts/breaking-python3-eval-protections/
 - https://realpython.com/python-eval-function/
```

### Comparing `evalidate-1.1.0/evalidate/security.py` & `evalidate-2.0.0/evalidate/security.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import ValidationException, evalidate, Expr
+from evalidate import ValidationException, Expr, EvalModel, base_eval_model
 
 simple_attacks = [
 """
 os.system("clear")
 """,
 """
 __import__('os').system('clear')
@@ -40,50 +40,63 @@
     
     # 3.11:         
     '0,0,0,0,0,0,b"BOOM",(),(),(),"","","",0,b"",b"",b"",b"",(),()'
 
 ]
 
 
-def test_attack(attack, nodes=None, blank=False, funcs=None, attrs=None, verbose=False):
+def test_attack(attack: str, model: EvalModel, verbose=False):
     '''
         test attack. return True if attack detected on validation, good. (False if passed, bad)
     '''
 
     if verbose:
         print("Testing attack code:\n{}".format(attack))
 
     try:
-        e = Expr(attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs)
+        e = Expr(attack, model=model)
         # node = evalidate(attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs)
     except ValidationException as e:
         if verbose:
             print("Good! Attack blocked: {}".format(e))
         return True
     else:
         print("Problem! Attack passed validation without exception!\nCode:\n{}".format(attack))
         return False
 
 
 
 
-def test_security(attacks=None, nodes=None, blank=False, funcs=None, attrs=None, verbose=False):
+def test_security(attacks=None, model: EvalModel = None, verbose=False):
     ''' 
     test all user-given attacks, or built-in attacks.
     Return value: True if good (all attacks detected), False if at least one attack passes validation
     '''
 
+    model = model or base_eval_model
+
     # test user-supplied attacks
     if attacks:
-        return all( [test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose) for attack in attacks] )
+        return all( [test_attack(attack=attack, model=model, verbose=verbose) for attack in attacks] )
 
 
     # test built-in set of attacks
-    if not all([test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose) for attack in simple_attacks]):
+    if not all([test_attack(attack=attack, model=model, verbose=verbose) for attack in simple_attacks]):
         return False
 
     for payload in boom_payload:
         attack = boom.format(payload=payload)
-        if not test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose):
+        if not test_attack(attack=attack, model=model, verbose=verbose):
             return False
         
-    return True
+    return True
+
+if __name__ == '__main__':
+
+    attacks = [
+        '1*2'
+    ]
+
+    model = base_eval_model.clone()
+    # model.nodes.append('Mult')
+    test_security(attacks=attacks, model=model, verbose=True)
+    test_security(model=model, verbose=True)
```

### Comparing `evalidate-1.1.0/evalidate.egg-info/PKG-INFO` & `evalidate-2.0.0/evalidate.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 1.1.0
+Version: 2.0.0
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
         
+        ## Upgrade warning
+        Version 2.0 is backward incompatible with older versions. safeeval and evalidate methods are removed, and EvalMode class is introduced.
+        
         ## Purpose
         Originally it's developed for filtering complex data structures e.g. 
         
         Find cheap smartphones available for sale:
         ```python
         category="smartphones" and price<300 and stock>0
         ```
@@ -58,75 +61,93 @@
         ## Exceptions
         Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
         inherit from base exception class `EvalException`.
         
         ## Configure validation
         Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
         
-        ### Allowing other nodes (operations)
         
-        Evalidate has built-in set of python operations, which are considered 'safe' (from author point of view). 
-        Code is considered valid only if all of it's operations are in this list. You can override this list by adding argument `nodes` like:
-        ```python
-        Expr('2*2', nodes=['Mult']).eval()
-        ```
+        ### EvalModel - using custom security model
+        EvalModel is security model for eval - list of allowed AST nodes, function calls, attributes and imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
         
-        If you want to start from blank whitelist (discard built-in whitelist), use `Expr(expression, blank=True, nodes=[...])` and then add each node manually (only what you really need) 
+        You can create custom empty model (and extend it later):
+        my_model = evalidate.EvalModel()
+        (nothing is allowed by default, even `1+2` will not be considered as safe code)
         
-        ### Allowing function calls
-        Evalidate does not allow any function calls by default.
+        or you may start from `base_eval_mode` and extend it:
+        ~~~python
+        from evalidate import Expr, base_eval_model
         
-        To enable `int()` function, need to allow 'Call' node and add this function to list of allowed function:
-        ```python
-        Expr('int(36.6)', nodes=['Call'], funcs=['int']).eval()
-        ```
-        If you want to call str methods:
-        ```python
-        Expr('name.startswith("John")', nodes=['Attribute', 'Call'], attrs=['startswith']).eval(dict(name='John Doe'))
-        ```
+        my_model = base_eval_model.clone()
+        my_model.nodes.append('Mult')
+        
+        Expr('2*2', model=my_model).eval()
+        ~~~
+        
+        To enable `int()` function, need to allow `'Call'` node and add this function to list of allowed function:
+        
+        ~~~python
+        my_model.nodes.append('Call')
+        my_model.allowed_functions.append('int')
+        
+        Expr('int(36.6)', model=my_model).eval()
+        ~~~
+        
+        Or, to call attributes:
+        ~~~python
+        m = evalidate.base_eval_model.clone()
+        m.nodes.extend(['Call', 'Attribute'])
+        m.attributes.append('startswith')
+        
+        
+        src = '"abcdef".startswith("abc")'
+        r = evalidate.Expr(src, model=m).eval()
+        ~~~
         
         But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
         
         
         ### Exporting my functions to eval code
-        ~~~
+        ~~~python
         def one():
           return 1
         
-        Expr('one()', nodes=['Call'], my_funcs={"one": one}).eval()
+        m = base_eval_model.clone()
+        m.nodes.append('Call')
+        Expr('one()', model=m).eval()
         ~~~
         
         ## Improve speed by using native eval() with validated code
         Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
         
-        ~~~
+        ~~~python
         from evalidate import Expr
         
         d = dict(a=1, b=2)
         expr = Expr('a+b')
         eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
         ~~~
         
         This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
         
         Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
         
         ## Limitations
         
-        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) and returns [AST node](https://docs.python.org/3/library/ast.html#node-classes).
+        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) to get [AST node](https://docs.python.org/3/library/ast.html#node-classes) to validate it.
         
         >Warning
         >
         >It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
         
         In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
         
         
         ### evalidate.security.test_security()
-        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (addnodes/safenodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
+        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (nodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
         
         This code will never print (I hope).
         ~~~python
         from evalidate.security import test_security
         
         test_security() or print("default rules are vulnerable!")
         ~~~
@@ -217,18 +238,17 @@
         
         While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
         - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
         - user can provide source code which runs very long time and consumes many resources 
         
         
         [simpleeval](https://github.com/danthedeckie/simpleeval)
-        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
-        
+        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is few times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
         
-        evalidate is good to run short same code against different data.
+        evalidate is good to run same expression against different data.
         
         ## Benchmarking
         We use `benchmark/benchmark.py` in this repository.
         We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
         
         ~~~
         Products: 1000000 items
@@ -236,15 +256,15 @@
         evalidate_eval(): 0.326s
         test_simpleeval(): 1.824s
         test_asteval(): 26.106s
         ~~~
         
         As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
         
-        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
+        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. (Benchmark code must assume expression as unknown in advance and untrusted)
         
         
         ## Read about eval() risks
         
         - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
         - https://netsec.expert/posts/breaking-python3-eval-protections/
         - https://realpython.com/python-eval-function/
```

### Comparing `evalidate-1.1.0/setup.py` & `evalidate-2.0.0/setup.py`

 * *Files identical despite different names*

