# Comparing `tmp/vmt-0.0.0b8.tar.gz` & `tmp/vmt-0.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmt-0.0.0b8.tar", last modified: Tue Jun  6 19:16:29 2023, max compression
+gzip compressed data, was "vmt-0.0.0b9.tar", last modified: Mon Jun 19 02:46:47 2023, max compression
```

## Comparing `vmt-0.0.0b8.tar` & `vmt-0.0.0b9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/
--rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b8/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-06 19:16:29.952933 vmt-0.0.0b8/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b8/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-06-06 19:14:37.000000 vmt-0.0.0b8/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-06 19:16:29.952933 vmt-0.0.0b8/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/vmt/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6168 2023-06-06 19:14:23.000000 vmt-0.0.0b8/src/vmt/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6418 2023-06-05 19:50:19.000000 vmt-0.0.0b8/src/vmt/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3515 2023-05-01 04:19:25.000000 vmt-0.0.0b8/src/vmt/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b8/src/vmt/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1669 2023-04-22 05:55:06.000000 vmt-0.0.0b8/src/vmt/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b8/src/vmt/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/vmt.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-19 02:46:47.338768 vmt-0.0.0b9/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b9/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-19 02:46:47.338768 vmt-0.0.0b9/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b9/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-06-19 02:43:52.000000 vmt-0.0.0b9/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-19 02:46:47.338768 vmt-0.0.0b9/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-19 02:46:47.335435 vmt-0.0.0b9/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-19 02:46:47.338768 vmt-0.0.0b9/src/vmt/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b9/src/vmt/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b9/src/vmt/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6168 2023-06-19 02:43:30.000000 vmt-0.0.0b9/src/vmt/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6418 2023-06-05 19:50:19.000000 vmt-0.0.0b9/src/vmt/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b9/src/vmt/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3515 2023-05-01 04:19:25.000000 vmt-0.0.0b9/src/vmt/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b9/src/vmt/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1669 2023-04-22 05:55:06.000000 vmt-0.0.0b9/src/vmt/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b9/src/vmt/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b9/src/vmt/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b9/src/vmt/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-19 02:46:47.338768 vmt-0.0.0b9/src/vmt.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-06-19 02:46:47.000000 vmt-0.0.0b9/src/vmt.egg-info/top_level.txt
```

### Comparing `vmt-0.0.0b8/LICENSE` & `vmt-0.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/PKG-INFO` & `vmt-0.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vmt-0.0.0b8/README.md` & `vmt-0.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/pyproject.toml` & `vmt-0.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vmt"
-version = "0.0.0.b8"
+version = "0.0.0.b9"
 description = "Video Media Tracker. Local, and simple method for watching and tracking a video media library."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv" ]
 dependencies = [
     "python-magic",
     "loadconf",
```

### Comparing `vmt-0.0.0b8/src/vmt/__main__.py` & `vmt-0.0.0b9/src/vmt/__main__.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/build.py` & `vmt-0.0.0b9/src/vmt/build.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -162,30 +162,30 @@
     user_system = system()
     # Create our dict
     valid_dirs = {}
     # For loop to walk the user's base_dir
     for dirpath, _, filenames in os.walk(user.settings["base_dir"], followlinks=True):
         # For loop to iterate over the files to ensure the dir
         # contains a video file
+        if user_system == "Windows":
+            add_dir = dirpath.replace(user.settings["base_dir"] + "\\", "")
+        else:
+            add_dir = dirpath.replace(f'{user.settings["base_dir"]}/', "")
+        if filter_directory(add_dir, user.stored["filters_file"], args):
+            continue
         skip_dir = True
         filenames.sort()
         for file in filenames:
             if not is_media(file):
                 continue
             else:
                 skip_dir = False
                 break
         if skip_dir:
             continue
-        if user_system == "Windows":
-            add_dir = dirpath.replace(user.settings["base_dir"] + "\\", "")
-        else:
-            add_dir = dirpath.replace(f'{user.settings["base_dir"]}/', "")
-        if filter_directory(add_dir, user.stored["filters_file"], args):
-            continue
         valid_dirs[add_dir] = {}
         valid_dirs[add_dir]["watching"] = None
         title = auto_title(add_dir, user_system)
         if args.interactive:
             title = user_choice([title], user, "Title: ", auto_title=True)
         valid_dirs[add_dir]["title"] = title
         valid_dirs[add_dir]["episodes"] = filenames
```

### Comparing `vmt-0.0.0b8/src/vmt/config.py` & `vmt-0.0.0b9/src/vmt/config.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/media.py` & `vmt-0.0.0b9/src/vmt/media.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/options.py` & `vmt-0.0.0b9/src/vmt/options.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/prompts.py` & `vmt-0.0.0b9/src/vmt/prompts.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/search.py` & `vmt-0.0.0b9/src/vmt/search.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/system.py` & `vmt-0.0.0b9/src/vmt/system.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt/utils.py` & `vmt-0.0.0b9/src/vmt/utils.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b8/src/vmt.egg-info/PKG-INFO` & `vmt-0.0.0b9/src/vmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

