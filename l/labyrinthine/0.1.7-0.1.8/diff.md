# Comparing `tmp/labyrinthine-0.1.7.tar.gz` & `tmp/labyrinthine-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labyrinthine-0.1.7.tar", last modified: Mon Apr  3 21:36:44 2023, max compression
+gzip compressed data, was "labyrinthine-0.1.8.tar", last modified: Wed Jun 21 20:09:53 2023, max compression
```

## Comparing `labyrinthine-0.1.7.tar` & `labyrinthine-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:36:44.425304 labyrinthine-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-03 21:36:33.000000 labyrinthine-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-03 21:36:44.425304 labyrinthine-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-03 21:36:33.000000 labyrinthine-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-03 21:36:33.000000 labyrinthine-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-03 21:36:44.425304 labyrinthine-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:36:44.421304 labyrinthine-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:36:44.421304 labyrinthine-0.1.7/src/labyrinthine/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-03 21:36:33.000000 labyrinthine-0.1.7/src/labyrinthine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-03 21:36:33.000000 labyrinthine-0.1.7/src/labyrinthine/depth_first.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:36:44.425304 labyrinthine-0.1.7/src/labyrinthine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-03 21:36:44.000000 labyrinthine-0.1.7/src/labyrinthine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 21:36:44.000000 labyrinthine-0.1.7/src/labyrinthine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:36:44.000000 labyrinthine-0.1.7/src/labyrinthine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 21:36:44.000000 labyrinthine-0.1.7/src/labyrinthine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:36:44.000000 labyrinthine-0.1.7/src/labyrinthine.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/labyrinthine/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/labyrinthine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/labyrinthine/depth_first.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/labyrinthine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/setup.cfg
```

### Comparing `labyrinthine-0.1.7/LICENSE` & `labyrinthine-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `labyrinthine-0.1.7/PKG-INFO` & `labyrinthine-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labyrinthine
-Version: 0.1.7
+Version: 0.1.8
 Summary: A no-dependency library that generates all the mazes you need.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/robertoschiavone/labyrinthine
 Project-URL: documentation, https://github.com/robertoschiavone/labyrinthine
 Project-URL: repository, https://github.com/robertoschiavone/labyrinthine.git
 Project-URL: changelog, https://github.com/robertoschiavone/labyrinthine/releases
-Keywords: Procedural Generation
+Keywords: maze,procedural-generation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labyrinthine-0.1.7/README.md` & `labyrinthine-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `labyrinthine-0.1.7/pyproject.toml` & `labyrinthine-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "labyrinthine"
-version = "0.1.7"
+version = "0.1.8"
 description = """A no-dependency library that generates all the mazes you need."""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.5"
 license = { file = "LICENSE" }
 authors = [
     { name = "Roberto Schiavone", email = "hello@robertoschiavone.io" },
 ]
 maintainers = [
     { name = "Roberto Schiavone", email = "hello@robertoschiavone.io" },
 ]
-keywords = ["Procedural Generation"]
+keywords = ["maze", "procedural-generation"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries"
 ]
 
 [project.urls]
```

### Comparing `labyrinthine-0.1.7/src/labyrinthine/depth_first.py` & `labyrinthine-0.1.8/labyrinthine/depth_first.py`

 * *Files identical despite different names*

### Comparing `labyrinthine-0.1.7/src/labyrinthine.egg-info/PKG-INFO` & `labyrinthine-0.1.8/labyrinthine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labyrinthine
-Version: 0.1.7
+Version: 0.1.8
 Summary: A no-dependency library that generates all the mazes you need.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/robertoschiavone/labyrinthine
 Project-URL: documentation, https://github.com/robertoschiavone/labyrinthine
 Project-URL: repository, https://github.com/robertoschiavone/labyrinthine.git
 Project-URL: changelog, https://github.com/robertoschiavone/labyrinthine/releases
-Keywords: Procedural Generation
+Keywords: maze,procedural-generation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

