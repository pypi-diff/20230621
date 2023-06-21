# Comparing `tmp/mdis-0.4.tar.gz` & `tmp/mdis-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-r8vxm8o1/mdis-0.4.tar", last modified: Sun Jun 18 19:00:10 2023, max compression
+gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-ahya19el/mdis-0.5.tar", last modified: Wed Jun 21 18:34:55 2023, max compression
```

## Comparing `mdis-0.4.tar` & `mdis-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.4/LICENSE
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 19:00:10.000000 mdis-0.4/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3649 2023-06-16 20:42:33.000000 mdis-0.4/README.md
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      938 2023-06-18 18:53:24.000000 mdis-0.4/pyproject.toml
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-18 19:00:10.000000 mdis-0.4/setup.cfg
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      316 2023-06-18 18:53:19.000000 mdis-0.4/src/mdis/__init__.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2725 2023-06-18 18:51:54.000000 mdis-0.4/src/mdis/dispatcher.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      513 2023-06-18 18:42:08.000000 mdis-0.4/src/mdis/visitor.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      959 2023-06-18 18:46:15.000000 mdis-0.4/src/mdis/walker.py
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/SOURCES.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/dependency_links.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/top_level.txt
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-21 18:34:55.000000 mdis-0.5/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.5/LICENSE
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-21 18:34:55.000000 mdis-0.5/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3649 2023-06-16 20:42:33.000000 mdis-0.5/README.md
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      938 2023-06-21 18:33:13.000000 mdis-0.5/pyproject.toml
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-21 18:34:55.000000 mdis-0.5/setup.cfg
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-21 18:34:55.000000 mdis-0.5/src/
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      316 2023-06-21 18:33:23.000000 mdis-0.5/src/mdis/__init__.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2830 2023-06-20 18:26:44.000000 mdis-0.5/src/mdis/dispatcher.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      513 2023-06-18 18:42:08.000000 mdis-0.5/src/mdis/visitor.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1925 2023-06-21 12:38:09.000000 mdis-0.5/src/mdis/walker.py
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis.egg-info/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis.egg-info/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis.egg-info/SOURCES.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis.egg-info/dependency_links.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-21 18:34:55.000000 mdis-0.5/src/mdis.egg-info/top_level.txt
```

### Comparing `mdis-0.4/LICENSE` & `mdis-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mdis-0.4/PKG-INFO` & `mdis-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.4
+Version: 0.5
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
 Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mdis-0.4/README.md` & `mdis-0.5/README.md`

 * *Files identical despite different names*

### Comparing `mdis-0.4/pyproject.toml` & `mdis-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=46.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdis"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Dmitry Selyutin", email="ghostmansd@gmail.com" },
 ]
 keywords = [
     "dispatch",
     "dispather",
     "map",
```

### Comparing `mdis-0.4/src/mdis/dispatcher.py` & `mdis-0.5/src/mdis/dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,17 @@
             if module not in ("builtins",):
                 name = f"{module}.{name}"
             names.append(name)
         return f"<{', '.join(names)}>"
 
     def __call__(self, call):
         class ConcreteHook(Hook):
-            def __call__(self, dispatcher, instance):
-                return call(self=dispatcher, instance=instance)
+            def __call__(self, dispatcher, instance, *args, **kwargs):
+                return call(self=dispatcher, instance=instance,
+                    *args, **kwargs)
 
         return ConcreteHook(*tuple(self))
 
 
 class DispatcherMeta(type):
     __hooks__ = {}
 
@@ -77,19 +78,19 @@
         for (checker, hook) in cls.__hooks__.items():
             if not isinstance(checker, type) and checker(typeid):
                 return hook
         return None
 
 
 class Dispatcher(metaclass=DispatcherMeta):
-    def __call__(self, instance):
+    def __call__(self, instance, *args, **kwargs):
         for typeid in instance.__class__.__mro__:
             hook = self.__class__.dispatch(typeid=typeid)
             if hook is not None:
                 break
         if hook is None:
             hook = self.__class__.dispatch()
-        return hook(dispatcher=self, instance=instance)
+        return hook(dispatcher=self, instance=instance, *args, **kwargs)
 
     @Hook(object)
-    def dispatch_object(self, instance):
+    def dispatch_object(self, instance, *args, **kwargs):
         raise NotImplementedError()
```

### Comparing `mdis-0.4/src/mdis/visitor.py` & `mdis-0.5/src/mdis/visitor.py`

 * *Files identical despite different names*

### Comparing `mdis-0.4/src/mdis.egg-info/PKG-INFO` & `mdis-0.5/src/mdis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.4
+Version: 0.5
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
 Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

