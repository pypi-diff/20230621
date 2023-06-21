# Comparing `tmp/rembg-2.0.46.tar.gz` & `tmp/rembg-2.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.46.tar", last modified: Tue Jun 20 14:39:00 2023, max compression
+gzip compressed data, was "rembg-2.0.47.tar", last modified: Wed Jun 21 17:29:54 2023, max compression
```

## Comparing `rembg-2.0.46.tar` & `rembg-2.0.47.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.949127 rembg-2.0.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 14:37:51.000000 rembg-2.0.46/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 14:37:51.000000 rembg-2.0.46/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-20 14:39:00.949127 rembg-2.0.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-20 14:37:51.000000 rembg-2.0.46/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-20 14:37:51.000000 rembg-2.0.46/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.949127 rembg-2.0.46/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-20 14:39:00.949127 rembg-2.0.46/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.945127 rembg-2.0.46/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.949127 rembg-2.0.46/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-20 14:37:51.000000 rembg-2.0.46/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.945127 rembg-2.0.46/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 14:39:00.000000 rembg-2.0.46/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 14:39:00.949127 rembg-2.0.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-20 14:37:51.000000 rembg-2.0.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.949127 rembg-2.0.46/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-20 14:37:51.000000 rembg-2.0.46/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-20 14:37:51.000000 rembg-2.0.46/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 17:28:48.000000 rembg-2.0.47/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-21 17:28:48.000000 rembg-2.0.47/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 17:29:54.925344 rembg-2.0.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-21 17:28:48.000000 rembg-2.0.47/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 17:28:48.000000 rembg-2.0.47/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 17:29:54.925344 rembg-2.0.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-21 17:28:48.000000 rembg-2.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 17:28:48.000000 rembg-2.0.47/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-21 17:28:48.000000 rembg-2.0.47/versioneer.py
```

### Comparing `rembg-2.0.46/LICENSE.txt` & `rembg-2.0.47/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/PKG-INFO` & `rembg-2.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.46
+Version: 2.0.47
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.46/README.md` & `rembg-2.0.47/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/bg.py` & `rembg-2.0.47/rembg/bg.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,16 @@
     cutout = np.clip(cutout * 255, 0, 255).astype(np.uint8)
     cutout = Image.fromarray(cutout)
 
     return cutout
 
 
 def naive_cutout(img: PILImage, mask: PILImage) -> PILImage:
-    empty = Image.new("RGBA", (img.size), 0)
-    cutout = Image.composite(img, empty, mask)
-    return cutout
+    img.putalpha(mask)
+    return img
 
 
 def get_concat_v_multi(imgs: List[PILImage]) -> PILImage:
     pivot = imgs.pop(0)
     for im in imgs:
         pivot = get_concat_v(pivot, im)
     return pivot
```

### Comparing `rembg-2.0.46/rembg/cli.py` & `rembg-2.0.47/rembg/cli.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/commands/b_command.py` & `rembg-2.0.47/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/commands/i_command.py` & `rembg-2.0.47/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/commands/p_command.py` & `rembg-2.0.47/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/commands/s_command.py` & `rembg-2.0.47/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/session_factory.py` & `rembg-2.0.47/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/__init__.py` & `rembg-2.0.47/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/base.py` & `rembg-2.0.47/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/dis_anime.py` & `rembg-2.0.47/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/dis_general_use.py` & `rembg-2.0.47/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/sam.py` & `rembg-2.0.47/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/silueta.py` & `rembg-2.0.47/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/u2net.py` & `rembg-2.0.47/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.47/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.47/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg/sessions/u2netp.py` & `rembg-2.0.47/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/rembg.egg-info/PKG-INFO` & `rembg-2.0.47/rembg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.46
+Version: 2.0.47
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.46/rembg.egg-info/SOURCES.txt` & `rembg-2.0.47/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/setup.py` & `rembg-2.0.47/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.46/tests/test_remove.py` & `rembg-2.0.47/tests/test_remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             image = image_path.read_bytes()
 
             actual = remove(image, session=new_session(model), **kwargs.get(model, {}).get(picture, {}))
             actual_hash = hash_img(Image.open(BytesIO(actual)))
 
             expected_path = Path(here / "results" / f"{picture}.{model}.png")
             # Uncomment to update the expected results
-            # f = open(expected_path, "ab")
+            # f = open(expected_path, "wb")
             # f.write(actual)
             # f.close()
 
             expected = expected_path.read_bytes()
             expected_hash = hash_img(Image.open(BytesIO(expected)))
 
             print(f"image_path: {image_path}")
```

### Comparing `rembg-2.0.46/versioneer.py` & `rembg-2.0.47/versioneer.py`

 * *Files identical despite different names*

