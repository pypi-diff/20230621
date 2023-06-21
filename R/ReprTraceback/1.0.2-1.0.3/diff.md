# Comparing `tmp/ReprTraceback-1.0.2.tar.gz` & `tmp/ReprTraceback-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReprTraceback-1.0.2.tar", last modified: Tue Jun 20 04:35:34 2023, max compression
+gzip compressed data, was "ReprTraceback-1.0.3.tar", last modified: Wed Jun 21 08:09:14 2023, max compression
```

## Comparing `ReprTraceback-1.0.2.tar` & `ReprTraceback-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 04:35:34.884982 ReprTraceback-1.0.2/
--rw-rw-rw-   0        0        0     1879 2023-06-20 04:35:34.884982 ReprTraceback-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1479 2023-06-20 04:14:06.000000 ReprTraceback-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 04:35:34.875961 ReprTraceback-1.0.2/ReprTraceback/
--rw-rw-rw-   0        0        0     3745 2023-06-20 04:14:06.000000 ReprTraceback-1.0.2/ReprTraceback/ReprTraceback.py
--rw-rw-rw-   0        0        0        0 2023-06-20 04:32:24.000000 ReprTraceback-1.0.2/ReprTraceback/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 04:35:34.883976 ReprTraceback-1.0.2/ReprTraceback.egg-info/
--rw-rw-rw-   0        0        0     1879 2023-06-20 04:35:34.000000 ReprTraceback-1.0.2/ReprTraceback.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-20 04:35:34.000000 ReprTraceback-1.0.2/ReprTraceback.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 04:35:34.000000 ReprTraceback-1.0.2/ReprTraceback.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 04:35:34.000000 ReprTraceback-1.0.2/ReprTraceback.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 04:35:34.884982 ReprTraceback-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      582 2023-06-20 04:35:27.000000 ReprTraceback-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.056437 ReprTraceback-1.0.3/
+-rw-rw-rw-   0        0        0     1898 2023-06-21 08:09:14.056437 ReprTraceback-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2023-06-20 04:41:42.000000 ReprTraceback-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.042914 ReprTraceback-1.0.3/ReprTraceback/
+-rw-rw-rw-   0        0        0     3414 2023-06-21 08:06:34.000000 ReprTraceback-1.0.3/ReprTraceback/ReprTraceback.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 04:32:24.000000 ReprTraceback-1.0.3/ReprTraceback/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.054935 ReprTraceback-1.0.3/ReprTraceback.egg-info/
+-rw-rw-rw-   0        0        0     1898 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-21 08:09:14.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 08:09:14.057448 ReprTraceback-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-06-21 08:09:06.000000 ReprTraceback-1.0.3/setup.py
```

### Comparing `ReprTraceback-1.0.2/PKG-INFO` & `ReprTraceback-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReprTraceback
-Version: 1.0.2
+Version: 1.0.3
 Summary: Improve stack traces with the values associated with each argument in each frame.
 Home-page: https://github.com/NateRiz/ReprTraceback
 Author: NateRiz
 Author-email: natezriz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 pip install ReprTraceback
 ```
 
 
 ## Usage
 Import and Init ReprTraceback.
 ```python
-import ReprTraceback
+from ReprTraceback import ReprTraceback
 
 # Call the init() function to set up the new traceback handler
 ReprTraceback.init()
 
 # ...
 # Your code here
 # ...
```

### Comparing `ReprTraceback-1.0.2/README.md` & `ReprTraceback-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 pip install ReprTraceback
 ```
 
 
 ## Usage
 Import and Init ReprTraceback.
 ```python
-import ReprTraceback
+from ReprTraceback import ReprTraceback
 
 # Call the init() function to set up the new traceback handler
 ReprTraceback.init()
 
 # ...
 # Your code here
 # ...
```

### Comparing `ReprTraceback-1.0.2/ReprTraceback/ReprTraceback.py` & `ReprTraceback-1.0.3/ReprTraceback/ReprTraceback.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 def repr_exception_handler(type_, value, exc_tb):
     tb_gen = tb._walk_tb_with_full_positions(exc_tb)
     traceback = ReprTraceback.extract_from_extended_frame_gen(tb_gen)
 
     for item in ReprTraceback.from_list(traceback).format():
         print(item, file=sys.stderr, end="")
     print(F"{type_.__name__}: {value}", file=sys.stderr)
-
-
 class ReprFrameSummary(tb.FrameSummary):
-    def __init__(self, f_back, f_code, local_global_lookup, filename, lineno, name, lookup_line=True, locals=None,
+    def __init__(self, f_back, f_code, filename, lineno, name, lookup_line=True, locals=None,
                  line=None, end_lineno=None, colno=None, end_colno=None):
         super().__init__(filename, lineno, name, lookup_line=lookup_line, locals=locals, line=line,
                          end_lineno=end_lineno, colno=colno, end_colno=end_colno)
         self.f_back = f_back
         self.f_code = f_code
-        self.local_global_lookup = local_global_lookup
 
 
 class ReprTraceback(tb.StackSummary):
     @classmethod
     def extract_from_extended_frame_gen(klass, frame_gen, *, limit=None,
                                         lookup_lines=True):
         if limit is None:
@@ -45,50 +42,47 @@
             co = f.f_code
             filename = co.co_filename
             name = co.co_name
 
             fnames.add(filename)
             linecache.lazycache(filename, f.f_globals)
             # Must defer line lookups until we have called checkcache.
+            f_locals = f.f_locals
             f_back = f.f_back
             f_code = f.f_code
-            local_global_lookup = f.f_globals
-            local_global_lookup.update(f.f_locals)
             result.append(
-                ReprFrameSummary(f_back, f_code, local_global_lookup, filename, lineno, name, lookup_line=False,
-                                 locals=None, end_lineno=end_lineno, colno=colno, end_colno=end_colno))
+                ReprFrameSummary(f_back, f_code, filename, lineno, name, lookup_line=False,
+                                 locals=f_locals, end_lineno=end_lineno, colno=colno, end_colno=end_colno))
         for filename in fnames:
             linecache.checkcache(filename)
         # If immediate lookup was desired, trigger lookups now.
         if lookup_lines:
             for f in result:
                 formatted_line = ReprTraceback.get_formatted_function_exception(f)
                 if formatted_line:
                     f._line = formatted_line
                 f.line
+                f.locals.clear()
         return result
 
     @staticmethod
     def get_formatted_function_exception(current_frame: ReprFrameSummary):
         if current_frame.f_back is None:
             return ""
-        # print(current_frame.f_back.f_locals)
-        func = current_frame.local_global_lookup[current_frame.f_code.co_name]
-        argspec = inspect.getfullargspec(func)
-        argument_names = list(argspec.args)
-        if argspec.varargs:
-            argument_names.append(argspec.varargs)
-        if argspec.varkw:
-            argument_names.append(argspec.varkw)
+        args, varargs, kwargs = inspect.getargs(current_frame.f_code)
+        argument_names = list(args)
+        if varargs:
+            argument_names.append(varargs)
+        if kwargs:
+            argument_names.append(kwargs)
 
         arg_pairs = []
         for name in argument_names:
-            value = current_frame.local_global_lookup[name] if name in current_frame.local_global_lookup else "?"
+            value = current_frame.locals.get(name, "?")
             arg_pairs.append((name, value))
 
-
         return F"{current_frame.f_code.co_name}(" + ", ".join(
             [F"{arg_name}={arg_value}" for arg_name, arg_value in arg_pairs]) + ")"
 
 
 def init():
     sys.excepthook = repr_exception_handler
```

### Comparing `ReprTraceback-1.0.2/ReprTraceback.egg-info/PKG-INFO` & `ReprTraceback-1.0.3/ReprTraceback.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReprTraceback
-Version: 1.0.2
+Version: 1.0.3
 Summary: Improve stack traces with the values associated with each argument in each frame.
 Home-page: https://github.com/NateRiz/ReprTraceback
 Author: NateRiz
 Author-email: natezriz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 pip install ReprTraceback
 ```
 
 
 ## Usage
 Import and Init ReprTraceback.
 ```python
-import ReprTraceback
+from ReprTraceback import ReprTraceback
 
 # Call the init() function to set up the new traceback handler
 ReprTraceback.init()
 
 # ...
 # Your code here
 # ...
```

### Comparing `ReprTraceback-1.0.2/setup.py` & `ReprTraceback-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ReprTraceback',
-    version='1.0.2',
+    version='1.0.3',
     description='Improve stack traces with the values associated with each argument in each frame.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='NateRiz',
     author_email='natezriz@gmail.com',
     url='https://github.com/NateRiz/ReprTraceback',
     packages=find_packages(),
```

