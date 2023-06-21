# Comparing `tmp/no_implicit_optional-1.3.tar.gz` & `tmp/no_implicit_optional-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_implicit_optional-1.3.tar", last modified: Mon Dec 26 06:10:45 2022, max compression
+gzip compressed data, was "no_implicit_optional-1.4.tar", last modified: Wed Jun 21 06:39:50 2023, max compression
```

## Comparing `no_implicit_optional-1.3.tar` & `no_implicit_optional-1.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 shantanu   (502) staff       (20)        0 2022-12-26 06:10:45.823612 no_implicit_optional-1.3/
--rw-r--r--   0 shantanu   (502) staff       (20)     1069 2022-09-07 03:42:21.000000 no_implicit_optional-1.3/LICENSE
--rw-r--r--   0 shantanu   (502) staff       (20)      526 2022-12-26 06:10:45.823290 no_implicit_optional-1.3/PKG-INFO
--rw-r--r--   0 shantanu   (502) staff       (20)     1857 2022-12-26 06:07:28.000000 no_implicit_optional-1.3/README.md
-drwxr-xr-x   0 shantanu   (502) staff       (20)        0 2022-12-26 06:10:45.822365 no_implicit_optional-1.3/no_implicit_optional.egg-info/
--rw-r--r--   0 shantanu   (502) staff       (20)      526 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/PKG-INFO
--rw-r--r--   0 shantanu   (502) staff       (20)      316 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/SOURCES.txt
--rw-r--r--   0 shantanu   (502) staff       (20)        1 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/dependency_links.txt
--rw-r--r--   0 shantanu   (502) staff       (20)       67 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/entry_points.txt
--rw-r--r--   0 shantanu   (502) staff       (20)        7 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/requires.txt
--rw-r--r--   0 shantanu   (502) staff       (20)       21 2022-12-26 06:10:45.000000 no_implicit_optional-1.3/no_implicit_optional.egg-info/top_level.txt
--rw-r--r--   0 shantanu   (502) staff       (20)    11598 2022-12-26 06:03:22.000000 no_implicit_optional-1.3/no_implicit_optional.py
--rw-r--r--   0 shantanu   (502) staff       (20)       38 2022-12-26 06:10:45.823680 no_implicit_optional-1.3/setup.cfg
--rw-r--r--   0 shantanu   (502) staff       (20)      745 2022-12-26 06:10:12.000000 no_implicit_optional-1.3/setup.py
+drwxr-xr-x   0 shantanu   (502) staff       (20)        0 2023-06-21 06:39:50.610956 no_implicit_optional-1.4/
+-rw-r--r--   0 shantanu   (502) staff       (20)      103 2022-09-07 03:42:10.000000 no_implicit_optional-1.4/.gitignore
+-rw-r--r--   0 shantanu   (502) staff       (20)      469 2023-06-21 06:39:04.000000 no_implicit_optional-1.4/CHANGELOG.md
+-rw-r--r--   0 shantanu   (502) staff       (20)     1069 2022-09-07 03:42:21.000000 no_implicit_optional-1.4/LICENSE
+-rw-r--r--   0 shantanu   (502) staff       (20)      526 2023-06-21 06:39:50.610661 no_implicit_optional-1.4/PKG-INFO
+-rw-r--r--   0 shantanu   (502) staff       (20)     1857 2022-12-26 06:07:28.000000 no_implicit_optional-1.4/README.md
+-rw-r--r--   0 shantanu   (502) staff       (20)       42 2022-11-14 18:36:45.000000 no_implicit_optional-1.4/mypy.ini
+drwxr-xr-x   0 shantanu   (502) staff       (20)        0 2023-06-21 06:39:50.610072 no_implicit_optional-1.4/no_implicit_optional.egg-info/
+-rw-r--r--   0 shantanu   (502) staff       (20)      526 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/PKG-INFO
+-rw-r--r--   0 shantanu   (502) staff       (20)      349 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/SOURCES.txt
+-rw-r--r--   0 shantanu   (502) staff       (20)        1 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/dependency_links.txt
+-rw-r--r--   0 shantanu   (502) staff       (20)       67 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/entry_points.txt
+-rw-r--r--   0 shantanu   (502) staff       (20)        7 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/requires.txt
+-rw-r--r--   0 shantanu   (502) staff       (20)       21 2023-06-21 06:39:50.000000 no_implicit_optional-1.4/no_implicit_optional.egg-info/top_level.txt
+-rw-r--r--   0 shantanu   (502) staff       (20)    11659 2023-06-21 06:38:03.000000 no_implicit_optional-1.4/no_implicit_optional.py
+-rw-r--r--   0 shantanu   (502) staff       (20)       38 2023-06-21 06:39:50.611021 no_implicit_optional-1.4/setup.cfg
+-rw-r--r--   0 shantanu   (502) staff       (20)      745 2023-06-21 06:38:22.000000 no_implicit_optional-1.4/setup.py
```

### Comparing `no_implicit_optional-1.3/LICENSE` & `no_implicit_optional-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `no_implicit_optional-1.3/PKG-INFO` & `no_implicit_optional-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no_implicit_optional
-Version: 1.3
+Version: 1.4
 Summary: A codemod to make your implicit optional type hints PEP 484 compliant.
 Home-page: https://github.com/hauntsaninja/no_implicit_optional
 Author: Shantanu Jain
 Author-email: hauntsaninja@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `no_implicit_optional-1.3/README.md` & `no_implicit_optional-1.4/README.md`

 * *Files identical despite different names*

### Comparing `no_implicit_optional-1.3/no_implicit_optional.egg-info/PKG-INFO` & `no_implicit_optional-1.4/no_implicit_optional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-implicit-optional
-Version: 1.3
+Version: 1.4
 Summary: A codemod to make your implicit optional type hints PEP 484 compliant.
 Home-page: https://github.com/hauntsaninja/no_implicit_optional
 Author: Shantanu Jain
 Author-email: hauntsaninja@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `no_implicit_optional-1.3/no_implicit_optional.py` & `no_implicit_optional-1.4/no_implicit_optional.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,20 +162,22 @@
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--use-union-or",
         action="store_true",
         help="Whether to use PEP 604 `X | None` syntax instead of `Optional[X]`",
     )
-    parser.add_argument("path")
+    parser.add_argument("path", nargs="+")
     args = parser.parse_args()
 
-    base = os.path.abspath(args.path)
-    root = base if os.path.isdir(base) else os.path.dirname(base)
-    files = gather_files([base], include_stubs=True)
+    bases = list(map(os.path.abspath, args.path))
+    root = os.path.commonpath(bases)
+    root = os.path.dirname(root) if os.path.isfile(root) else root
+
+    files = gather_files(bases, include_stubs=True)
     try:
         result = parallel_exec_transform_with_prettyprint(
             NoImplicitOptionalCommand(CodemodContext(), use_union_or=args.use_union_or),
             files,
             repo_root=root,
         )
     except KeyboardInterrupt:
```

### Comparing `no_implicit_optional-1.3/setup.py` & `no_implicit_optional-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="no_implicit_optional",
-    version="1.3",
+    version="1.4",
     author="Shantanu Jain",
     author_email="hauntsaninja@gmail.com",
     description="A codemod to make your implicit optional type hints PEP 484 compliant.",
     url="https://github.com/hauntsaninja/no_implicit_optional",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

