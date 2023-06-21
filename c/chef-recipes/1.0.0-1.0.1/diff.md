# Comparing `tmp/chef_recipes-1.0.0.tar.gz` & `tmp/chef_recipes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chef_recipes-1.0.0.tar", max compression
+gzip compressed data, was "chef_recipes-1.0.1.tar", max compression
```

## Comparing `chef_recipes-1.0.0.tar` & `chef_recipes-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,31 @@
--rw-r--r--   0        0        0      748 2023-06-21 13:21:33.905239 chef_recipes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-12 13:25:24.244733 chef_recipes-1.0.0/src/python/chef/__init__.py
--rw-r--r--   0        0        0      645 2023-06-19 15:18:02.823243 chef_recipes-1.0.0/src/python/chef/api/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-19 17:16:18.642244 chef_recipes-1.0.0/src/python/chef/api/categories.py
--rw-r--r--   0        0        0     1172 2023-06-19 14:03:07.526945 chef_recipes-1.0.0/src/python/chef/api/common.py
--rw-r--r--   0        0        0     1777 2023-06-21 06:08:54.409100 chef_recipes-1.0.0/src/python/chef/api/images.py
--rw-r--r--   0        0        0      856 2023-06-20 07:51:43.135386 chef_recipes-1.0.0/src/python/chef/api/ingredients.py
--rw-r--r--   0        0        0     1358 2023-06-20 07:51:32.853550 chef_recipes-1.0.0/src/python/chef/api/recipes.py
--rw-r--r--   0        0        0      733 2023-06-19 17:16:18.671243 chef_recipes-1.0.0/src/python/chef/api/tags.py
--rw-r--r--   0        0        0     8049 2023-06-21 08:37:20.902732 chef_recipes-1.0.0/src/python/chef/controllers.py
--rw-r--r--   0        0        0     1907 2023-06-21 09:07:09.838201 chef_recipes-1.0.0/src/python/chef/images.py
--rw-r--r--   0        0        0     2143 2023-06-21 12:43:53.141300 chef_recipes-1.0.0/src/python/chef/main.py
--rw-r--r--   0        0        0     5868 2023-06-20 13:41:42.301568 chef_recipes-1.0.0/src/python/chef/models.py
--rw-r--r--   0        0        0     3114 2023-06-19 14:05:22.906763 chef_recipes-1.0.0/src/python/chef/schemas.py
--rw-r--r--   0        0        0      634 2023-06-20 08:50:33.632068 chef_recipes-1.0.0/src/python/chef/session.py
--rw-r--r--   0        0        0     1234 2023-06-21 12:43:05.219090 chef_recipes-1.0.0/src/python/chef/settings.py
--rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 chef_recipes-1.0.0/setup.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chef_recipes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-06-21 14:51:29.141089 chef_recipes-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0   105536 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-404c746c.woff2
+-rw-r--r--   0        0        0   181852 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-brands-400-e523f49c.ttf
+-rw-r--r--   0        0        0    60520 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-4e96a7e0.ttf
+-rw-r--r--   0        0        0    23940 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-regular-400-6a274e76.woff2
+-rw-r--r--   0        0        0   388460 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-03f2986c.ttf
+-rw-r--r--   0        0        0   154228 2023-06-21 13:00:13.873177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-solid-900-d76fb4e8.woff2
+-rw-r--r--   0        0        0     4960 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-0db31bef.woff2
+-rw-r--r--   0        0        0    10556 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/fa-v4compatibility-86a687cf.ttf
+-rw-r--r--   0        0        0     9197 2023-06-21 13:00:13.869177 chef_recipes-1.0.1/src/js/chef/dist/assets/favicon-464b3816.png
+-rw-r--r--   0        0        0   314577 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/index-70f2750d.css
+-rw-r--r--   0        0        0   484824 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/assets/index-b3f57f4a.js
+-rw-r--r--   0        0        0   119596 2023-06-21 13:00:13.463184 chef_recipes-1.0.1/src/js/chef/dist/favicon.ico
+-rw-r--r--   0        0        0      419 2023-06-21 13:00:13.874177 chef_recipes-1.0.1/src/js/chef/dist/index.html
+-rw-r--r--   0        0        0        1 2023-06-21 14:51:25.825143 chef_recipes-1.0.1/src/python/chef/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-19 15:18:02.823243 chef_recipes-1.0.1/src/python/chef/api/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-19 17:16:18.642244 chef_recipes-1.0.1/src/python/chef/api/categories.py
+-rw-r--r--   0        0        0     1172 2023-06-19 14:03:07.526945 chef_recipes-1.0.1/src/python/chef/api/common.py
+-rw-r--r--   0        0        0     1777 2023-06-21 06:08:54.409100 chef_recipes-1.0.1/src/python/chef/api/images.py
+-rw-r--r--   0        0        0      856 2023-06-20 07:51:43.135386 chef_recipes-1.0.1/src/python/chef/api/ingredients.py
+-rw-r--r--   0        0        0     1358 2023-06-20 07:51:32.853550 chef_recipes-1.0.1/src/python/chef/api/recipes.py
+-rw-r--r--   0        0        0      733 2023-06-19 17:16:18.671243 chef_recipes-1.0.1/src/python/chef/api/tags.py
+-rw-r--r--   0        0        0     8049 2023-06-21 08:37:20.902732 chef_recipes-1.0.1/src/python/chef/controllers.py
+-rw-r--r--   0        0        0     1907 2023-06-21 09:07:09.838201 chef_recipes-1.0.1/src/python/chef/images.py
+-rw-r--r--   0        0        0     2143 2023-06-21 12:43:53.141300 chef_recipes-1.0.1/src/python/chef/main.py
+-rw-r--r--   0        0        0     5868 2023-06-20 13:41:42.301568 chef_recipes-1.0.1/src/python/chef/models.py
+-rw-r--r--   0        0        0     3114 2023-06-19 14:05:22.906763 chef_recipes-1.0.1/src/python/chef/schemas.py
+-rw-r--r--   0        0        0      634 2023-06-20 08:50:33.632068 chef_recipes-1.0.1/src/python/chef/session.py
+-rw-r--r--   0        0        0     1234 2023-06-21 12:43:05.219090 chef_recipes-1.0.1/src/python/chef/settings.py
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 chef_recipes-1.0.1/setup.py
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chef_recipes-1.0.1/PKG-INFO
```

### Comparing `chef_recipes-1.0.0/pyproject.toml` & `chef_recipes-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "chef-recipes"
-version = "1.0.0"
+version = "1.0.1"
 description = "Home recipe management app."
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 
 packages = [
     { include = "chef", from = "src/python" }
 ]
 
+
 include = [
-    { path = "src/js/chef/dist/*", format = "wheel" },
-    { path = "src/js/chef/dist/assets/*", format = "wheel" }
+    { path = "src/js/chef/dist/*", format = ["sdist", "wheel"] },
+    { path = "src/js/chef/dist/assets/*", format = ["sdist", "wheel"] }
 ]
 
 
 [tool.poetry.scripts]
 chef = "chef.main:serve"
 
 [tool.poetry.dependencies]
```

### Comparing `chef_recipes-1.0.0/src/python/chef/api/__init__.py` & `chef_recipes-1.0.1/src/python/chef/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/categories.py` & `chef_recipes-1.0.1/src/python/chef/api/categories.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/common.py` & `chef_recipes-1.0.1/src/python/chef/api/common.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/images.py` & `chef_recipes-1.0.1/src/python/chef/api/images.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/ingredients.py` & `chef_recipes-1.0.1/src/python/chef/api/ingredients.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/recipes.py` & `chef_recipes-1.0.1/src/python/chef/api/recipes.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/api/tags.py` & `chef_recipes-1.0.1/src/python/chef/api/tags.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/controllers.py` & `chef_recipes-1.0.1/src/python/chef/controllers.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/images.py` & `chef_recipes-1.0.1/src/python/chef/images.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/main.py` & `chef_recipes-1.0.1/src/python/chef/main.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/models.py` & `chef_recipes-1.0.1/src/python/chef/models.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/schemas.py` & `chef_recipes-1.0.1/src/python/chef/schemas.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/session.py` & `chef_recipes-1.0.1/src/python/chef/session.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/src/python/chef/settings.py` & `chef_recipes-1.0.1/src/python/chef/settings.py`

 * *Files identical despite different names*

### Comparing `chef_recipes-1.0.0/setup.py` & `chef_recipes-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'uvicorn>=0.22.0,<0.23.0']
 
 entry_points = \
 {'console_scripts': ['chef = chef.main:serve']}
 
 setup_kwargs = {
     'name': 'chef-recipes',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Home recipe management app.',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `chef_recipes-1.0.0/PKG-INFO` & `chef_recipes-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chef-recipes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Home recipe management app.
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

