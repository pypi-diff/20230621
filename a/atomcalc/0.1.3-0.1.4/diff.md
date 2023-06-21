# Comparing `tmp/atomcalc-0.1.3.tar.gz` & `tmp/atomcalc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcalc-0.1.3.tar", max compression
+gzip compressed data, was "atomcalc-0.1.4.tar", max compression
```

## Comparing `atomcalc-0.1.3.tar` & `atomcalc-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      182 2023-06-21 20:23:28.554489 atomcalc-0.1.3/atomcalc/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-21 19:20:53.765656 atomcalc-0.1.3/atomcalc/Decay.py
--rw-r--r--   0        0        0     1531 2023-06-21 19:20:53.766656 atomcalc-0.1.3/atomcalc/Laser.py
--rw-r--r--   0        0        0      457 2023-06-21 19:20:53.762652 atomcalc-0.1.3/atomcalc/Level.py
--rw-r--r--   0        0        0      876 2023-06-21 19:20:53.792679 atomcalc-0.1.3/atomcalc/plot_pulse.py
--rw-r--r--   0        0        0    24121 2023-06-21 19:20:54.536355 atomcalc-0.1.3/atomcalc/System.py
--rw-r--r--   0        0        0      627 2023-06-21 20:25:50.071992 atomcalc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1142 2023-06-21 18:51:17.200721 atomcalc-0.1.3/README.md
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 atomcalc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      182 2023-06-21 20:30:09.840587 atomcalc-0.1.4/atomcalc/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-21 19:20:53.765656 atomcalc-0.1.4/atomcalc/Decay.py
+-rw-r--r--   0        0        0     1531 2023-06-21 19:20:53.766656 atomcalc-0.1.4/atomcalc/Laser.py
+-rw-r--r--   0        0        0      457 2023-06-21 19:20:53.762652 atomcalc-0.1.4/atomcalc/Level.py
+-rw-r--r--   0        0        0      876 2023-06-21 19:20:53.792679 atomcalc-0.1.4/atomcalc/plot_pulse.py
+-rw-r--r--   0        0        0    24121 2023-06-21 19:20:54.536355 atomcalc-0.1.4/atomcalc/System.py
+-rw-r--r--   0        0        0      619 2023-06-21 20:32:20.305976 atomcalc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1142 2023-06-21 18:51:17.200721 atomcalc-0.1.4/README.md
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 atomcalc-0.1.4/PKG-INFO
```

### Comparing `atomcalc-0.1.3/atomcalc/Decay.py` & `atomcalc-0.1.4/atomcalc/Decay.py`

 * *Files identical despite different names*

### Comparing `atomcalc-0.1.3/atomcalc/Laser.py` & `atomcalc-0.1.4/atomcalc/Laser.py`

 * *Files identical despite different names*

### Comparing `atomcalc-0.1.3/atomcalc/plot_pulse.py` & `atomcalc-0.1.4/atomcalc/plot_pulse.py`

 * *Files identical despite different names*

### Comparing `atomcalc-0.1.3/atomcalc/System.py` & `atomcalc-0.1.4/atomcalc/System.py`

 * *Files identical despite different names*

### Comparing `atomcalc-0.1.3/pyproject.toml` & `atomcalc-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atomcalc"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Moritz Wilke"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.5,<3.12"
 numpy = "^1.24.3"
@@ -23,8 +23,8 @@
 ipython = "^7.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
-homepage="https://atomcalc.github.io/AtomCalc/"
+Source = "https://github.com/pypa/flit"
```

### Comparing `atomcalc-0.1.3/README.md` & `atomcalc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `atomcalc-0.1.3/PKG-INFO` & `atomcalc-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomcalc
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Moritz Wilke
 Requires-Python: >=3.8.5,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

