# Comparing `tmp/psbs-0.1.2.tar.gz` & `tmp/psbs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.1.2.tar", last modified: Mon Jun 19 18:16:36 2023, max compression
+gzip compressed data, was "psbs-0.1.3.tar", last modified: Wed Jun 21 13:29:02 2023, max compression
```

## Comparing `psbs-0.1.2.tar` & `psbs-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-19 18:16:36.527165 psbs-0.1.2/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.2/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-19 18:16:36.527278 psbs-0.1.2/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.2/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-19 18:16:36.524714 psbs-0.1.2/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.2/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.2/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.2/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.2/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     1146 2023-06-18 20:24:47.000000 psbs-0.1.2/psbs/extension.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-19 18:16:36.526932 psbs-0.1.2/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.1.2/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3025 2023-06-18 20:24:47.000000 psbs-0.1.2/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.2/psbs/gister.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4116 2023-06-18 19:37:14.000000 psbs-0.1.2/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-19 00:52:39.000000 psbs-0.1.2/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1651 2023-06-19 00:52:46.000000 psbs-0.1.2/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1548 2023-06-18 20:02:25.000000 psbs-0.1.2/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.2/psbs/templatebuilder.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.2/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.2/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-19 18:16:36.526452 psbs-0.1.2/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      474 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-19 18:16:36.000000 psbs-0.1.2/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-19 18:16:36.527655 psbs-0.1.2/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1239 2023-06-19 18:14:54.000000 psbs-0.1.2/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-21 13:29:02.326917 psbs-0.1.3/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.3/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-21 13:29:02.327036 psbs-0.1.3/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.3/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-21 13:29:02.323718 psbs-0.1.3/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.3/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.3/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.3/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.3/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1146 2023-06-18 20:24:47.000000 psbs-0.1.3/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-21 13:29:02.326614 psbs-0.1.3/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.1.3/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3025 2023-06-18 20:24:47.000000 psbs-0.1.3/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.3/psbs/gister.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4116 2023-06-18 19:37:14.000000 psbs-0.1.3/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-19 00:52:39.000000 psbs-0.1.3/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1794 2023-06-21 13:24:36.000000 psbs-0.1.3/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1548 2023-06-18 20:02:25.000000 psbs-0.1.3/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.3/psbs/templatebuilder.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.3/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.3/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-21 13:29:02.325981 psbs-0.1.3/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      474 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-21 13:29:02.000000 psbs-0.1.3/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-21 13:29:02.327454 psbs-0.1.3/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1239 2023-06-21 13:27:44.000000 psbs-0.1.3/setup.py
```

### Comparing `psbs-0.1.2/LICENSE` & `psbs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/PKG-INFO` & `psbs-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.1.2
+Version: 0.1.3
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.3.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.1.2/README.md` & `psbs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/example.txt` & `psbs-0.1.3/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/extension.py` & `psbs-0.1.3/psbs/extension.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/extensions/images.py` & `psbs-0.1.3/psbs/extensions/images.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/gister.py` & `psbs-0.1.3/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/project.py` & `psbs-0.1.3/psbs/project.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/psbs.py` & `psbs-0.1.3/psbs/psbs.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/psparser.py` & `psbs-0.1.3/psbs/psparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 
 
 def split_ps(input_str):
     input_redacted = redact(input_str)
     sections = {
         "prelude": [],
         "tags": [],
+        "mappings": [],
         "objects": [],
         "legend": [],
         "sounds": [],
         "collisionlayers": [],
         "rules": [],
         "winconditions": [],
         "levels": [],
     }
+    optional_sections = ["tags","mappings"]
     section_headers = list(sections.keys())[1:]
     headers = re.finditer(
         r"^(" + "|".join(section_headers) + ") *$",
         input_redacted,
         flags=re.IGNORECASE | re.MULTILINE,
     )
 
@@ -40,16 +42,17 @@
         content = re.sub(r"^(=*) *", "", content, flags=re.MULTILINE)
         sections[section].append(content.strip())
         section = header.group().strip().lower()
         start = header.span()[1]
     content = input_str[start:]
     content = re.sub(r"^(=*) *", "", content, flags=re.MULTILINE)
     sections[section].append(content.strip())
-    if not sections["tags"]:
-        del sections["tags"]
+    for optional_section in optional_sections:
+        if not sections[optional_section]:
+            del sections[optional_section]
 
     return sections
 
 
 def get_engine(input_str):
     start_str = "http"
     end_str = "editor.html"
```

### Comparing `psbs-0.1.2/psbs/template.py` & `psbs-0.1.3/psbs/template.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/templatebuilder.py` & `psbs-0.1.3/psbs/templatebuilder.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/token.py` & `psbs-0.1.3/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs/utils.py` & `psbs-0.1.3/psbs/utils.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.2/psbs.egg-info/PKG-INFO` & `psbs-0.1.3/psbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.1.2
+Version: 0.1.3
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.3.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.1.2/setup.py` & `psbs-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.1.2',
+    version='0.1.3',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.2.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.3.tar.gz',
     license='MIT',
     packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
```

