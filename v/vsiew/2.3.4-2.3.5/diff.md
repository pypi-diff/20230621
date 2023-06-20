# Comparing `tmp/vsiew-2.3.4.tar.gz` & `tmp/vsiew-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.4.tar", last modified: Tue Jun 20 16:09:44 2023, max compression
+gzip compressed data, was "vsiew-2.3.5.tar", last modified: Tue Jun 20 23:06:58 2023, max compression
```

## Comparing `vsiew-2.3.4.tar` & `vsiew-2.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:09:44.885129 vsiew-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 16:09:22.000000 vsiew-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 16:09:44.885129 vsiew-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 16:09:22.000000 vsiew-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:09:44.885129 vsiew-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 16:09:22.000000 vsiew-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:09:44.881129 vsiew-2.3.4/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 16:09:22.000000 vsiew-2.3.4/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 16:09:22.000000 vsiew-2.3.4/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 16:09:22.000000 vsiew-2.3.4/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-20 16:09:22.000000 vsiew-2.3.4/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:09:44.885129 vsiew-2.3.4/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 16:09:44.000000 vsiew-2.3.4/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.292692 vsiew-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 23:06:32.000000 vsiew-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 23:06:58.292692 vsiew-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 23:06:32.000000 vsiew-2.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:06:58.292692 vsiew-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 23:06:32.000000 vsiew-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.288692 vsiew-2.3.5/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.288692 vsiew-2.3.5/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.4/LICENSE` & `vsiew-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.4/PKG-INFO` & `vsiew-2.3.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.4
+Version: 2.3.5
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.4/setup.py` & `vsiew-2.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.4/vsiew/__init__.py` & `vsiew-2.3.5/vsiew/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -52,15 +52,34 @@
         and t.f_locals['self'].value == 'vsiew:update_packages'
     ) or (
         'pkg_main_name' in t.f_locals and t.f_locals['pkg_main_name'] == 'vsiew.__main__'
     ):
         update_check = True
         break
 else:
-    update_check = len(sys.argv) > 0 and (Path(sys.executable).parent / 'Scripts') in Path(sys.argv[0]).parents
+    import site
+
+    parents = Path(sys.argv[0]).parents
+
+    update_check = False
+
+    if len(sys.argv) > 0:
+        for folder in [
+            Path(site_pack) for site_pack in (
+                *site.getsitepackages(),
+                site.getusersitepackages()
+            ) if 'site-packages' in site_pack
+        ]:
+            if (
+                folder in parents and 'Lib' not in folder.parts
+            ) or any(
+                x / 'Scripts' for x in (folder.parent.parent, folder.parent)
+            ):
+                update_check = True
+                break
 
 
 if update_check:
     __all__.append('update_packages')
 
     # vsiew
     def update_packages() -> None:
```

### Comparing `vsiew-2.3.4/vsiew/init.py` & `vsiew-2.3.5/vsiew/init.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.4/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.5/vsiew.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.4
+Version: 2.3.5
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

