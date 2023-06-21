# Comparing `tmp/depmanager-0.1.3.tar.gz` & `tmp/depmanager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depmanager-0.1.3.tar", last modified: Mon Jun 12 20:23:18 2023, max compression
+gzip compressed data, was "depmanager-0.1.4.tar", last modified: Wed Jun 21 05:33:08 2023, max compression
```

## Comparing `depmanager-0.1.3.tar` & `depmanager-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.425627 depmanager-0.1.3/
--rw-rw-rw-   0        0        0     1085 2023-02-24 16:42:27.000000 depmanager-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    12517 2023-06-12 20:23:18.424624 depmanager-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10663 2023-06-12 20:22:31.000000 depmanager-0.1.3/README.md
--rw-rw-rw-   0        0        0     1056 2023-06-12 20:22:31.000000 depmanager-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 20:23:18.426629 depmanager-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.332627 depmanager-0.1.3/src/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.337627 depmanager-0.1.3/src/depmanager/
--rw-rw-rw-   0        0        0      149 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.368630 depmanager-0.1.3/src/depmanager/api/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/api/__init__.py
--rw-rw-rw-   0        0        0     7819 2023-06-03 14:27:48.000000 depmanager-0.1.3/src/depmanager/api/builder.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.399626 depmanager-0.1.3/src/depmanager/api/internal/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/api/internal/__init__.py
--rw-rw-rw-   0        0        0     4689 2023-04-04 21:53:30.000000 depmanager-0.1.3/src/depmanager/api/internal/common.py
--rw-rw-rw-   0        0        0     6216 2023-06-03 13:54:25.000000 depmanager-0.1.3/src/depmanager/api/internal/database_common.py
--rw-rw-rw-   0        0        0     2382 2023-05-22 18:14:20.000000 depmanager-0.1.3/src/depmanager/api/internal/database_local.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 16:16:08.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_folder.py
--rw-rw-rw-   0        0        0     2709 2023-05-22 16:16:08.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_ftp.py
--rw-rw-rw-   0        0        0    10198 2023-06-12 19:29:09.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_server.py
--rw-rw-rw-   0        0        0    10245 2023-05-22 19:47:09.000000 depmanager-0.1.3/src/depmanager/api/internal/dependency.py
--rw-rw-rw-   0        0        0    10809 2023-06-12 19:29:00.000000 depmanager-0.1.3/src/depmanager/api/internal/system.py
--rw-rw-rw-   0        0        0     1187 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/api/local.py
--rw-rw-rw-   0        0        0     6386 2023-06-12 19:57:40.000000 depmanager-0.1.3/src/depmanager/api/package.py
--rw-rw-rw-   0        0        0     1652 2023-05-22 21:20:13.000000 depmanager-0.1.3/src/depmanager/api/recipe.py
--rw-rw-rw-   0        0        0     3229 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/api/remotes.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.402626 depmanager-0.1.3/src/depmanager/cmake/
--rw-rw-rw-   0        0        0     3259 2023-04-07 21:42:17.000000 depmanager-0.1.3/src/depmanager/cmake/DepManager.cmake
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.420630 depmanager-0.1.3/src/depmanager/command/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/__init__.py
--rw-rw-rw-   0        0        0     2820 2023-06-03 13:50:57.000000 depmanager-0.1.3/src/depmanager/command/build.py
--rw-rw-rw-   0        0        0      858 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/get.py
--rw-rw-rw-   0        0        0     1514 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/info.py
--rw-rw-rw-   0        0        0     4735 2023-06-12 19:44:48.000000 depmanager-0.1.3/src/depmanager/command/pack.py
--rw-rw-rw-   0        0        0     5511 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/command/remote.py
--rw-rw-rw-   0        0        0     1770 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.351629 depmanager-0.1.3/src/depmanager.egg-info/
--rw-rw-rw-   0        0        0    12517 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1149 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/top_level.txt
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:08.770912 depmanager-0.1.4/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1085 2023-02-24 16:42:27.000000 depmanager-0.1.4/LICENSE
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    12334 2023-06-21 05:33:08.765911 depmanager-0.1.4/PKG-INFO
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    10835 2023-06-19 18:53:02.000000 depmanager-0.1.4/README.md
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1058 2023-06-19 19:04:44.000000 depmanager-0.1.4/pyproject.toml
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)       38 2023-06-21 05:33:08.773915 depmanager-0.1.4/setup.cfg
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:06.791635 depmanager-0.1.4/src/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/__init__.py
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:06.896628 depmanager-0.1.4/src/depmanager/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)      149 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/__init__.py
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:07.573328 depmanager-0.1.4/src/depmanager/api/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/api/__init__.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     7841 2023-06-18 18:54:30.000000 depmanager-0.1.4/src/depmanager/api/builder.py
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:08.315708 depmanager-0.1.4/src/depmanager/api/internal/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/api/internal/__init__.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     4689 2023-04-04 21:53:30.000000 depmanager-0.1.4/src/depmanager/api/internal/common.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     6216 2023-06-03 13:54:25.000000 depmanager-0.1.4/src/depmanager/api/internal/database_common.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     2382 2023-05-22 18:14:20.000000 depmanager-0.1.4/src/depmanager/api/internal/database_local.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1688 2023-05-22 16:16:08.000000 depmanager-0.1.4/src/depmanager/api/internal/database_remote_folder.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     2709 2023-05-22 16:16:08.000000 depmanager-0.1.4/src/depmanager/api/internal/database_remote_ftp.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    10198 2023-06-12 19:29:09.000000 depmanager-0.1.4/src/depmanager/api/internal/database_remote_server.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    11356 2023-06-19 19:15:24.000000 depmanager-0.1.4/src/depmanager/api/internal/dependency.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    10809 2023-06-12 19:29:00.000000 depmanager-0.1.4/src/depmanager/api/internal/system.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1261 2023-06-19 19:04:44.000000 depmanager-0.1.4/src/depmanager/api/local.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     6386 2023-06-12 19:57:40.000000 depmanager-0.1.4/src/depmanager/api/package.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1652 2023-05-22 21:20:13.000000 depmanager-0.1.4/src/depmanager/api/recipe.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     7067 2023-06-21 05:32:45.000000 depmanager-0.1.4/src/depmanager/api/remotes.py
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:08.380709 depmanager-0.1.4/src/depmanager/cmake/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     3259 2023-04-07 21:42:17.000000 depmanager-0.1.4/src/depmanager/cmake/DepManager.cmake
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:08.709913 depmanager-0.1.4/src/depmanager/command/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/command/__init__.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     2820 2023-06-03 13:50:57.000000 depmanager-0.1.4/src/depmanager/command/build.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)      858 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/command/get.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1514 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/command/info.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     4735 2023-06-12 19:44:48.000000 depmanager-0.1.4/src/depmanager/command/pack.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     5494 2023-06-19 18:53:02.000000 depmanager-0.1.4/src/depmanager/command/remote.py
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1770 2023-03-21 22:46:02.000000 depmanager-0.1.4/src/depmanager/manager.py
+drwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        0 2023-06-21 05:33:07.200948 depmanager-0.1.4/src/depmanager.egg-info/
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)    12334 2023-06-21 05:33:05.000000 depmanager-0.1.4/src/depmanager.egg-info/PKG-INFO
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)     1149 2023-06-21 05:33:06.000000 depmanager-0.1.4/src/depmanager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)        1 2023-06-21 05:33:05.000000 depmanager-0.1.4/src/depmanager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)       70 2023-06-21 05:33:05.000000 depmanager-0.1.4/src/depmanager.egg-info/entry_points.txt
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)       27 2023-06-21 05:33:06.000000 depmanager-0.1.4/src/depmanager.egg-info/requires.txt
+-rwxrwxrwx   0 argawaen  (1000) argawaen  (1000)       20 2023-06-21 05:33:06.000000 depmanager-0.1.4/src/depmanager.egg-info/top_level.txt
```

### Comparing `depmanager-0.1.3/LICENSE` & `depmanager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/PKG-INFO` & `depmanager-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,7 @@
-Metadata-Version: 2.1
-Name: depmanager
-Version: 0.1.3
-Summary: Simple Dependency manager
-Author-email: Silmaen <genteur.slayer@laposte.net>
-License: MIT License
-        
-        Copyright (c) 2023 Silmaen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Silmaen/DepManager
-Keywords: dependency,setuptools,development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DepManager
 
 Depmanager is a minimalistic tool to manage dependencies (also known as third-party
 libraries) of a C++ Project. It works closely with cmake tool.
 
 It allow to store dependencies in a distant repository to share builds with other and
 have a local cache project-independent.
@@ -165,15 +127,17 @@
     * Allowed proto are:
         * `ftp` supports login
         * `folder` a folder of your computer (mostly for debug or testing)
         * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
         * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
     * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
 * `del <remote>` remove the designated remote if exists.
-* `sync <remote>` push to remote all local package that does not already exist on remote.
+* `sync <remote> [--push-only|--pull-only]` push to remote all local package that does not already
+  exist on remote. Pull local package that have a newer version on the remote. If no remote given, it will use the
+  default one.
 
 ### build
 
 `depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
 
 Some option can be passed to the build system:
 
@@ -328,20 +292,21 @@
     * [ ] Add a sorting order for remotes.
     * [ ] Auto-pull if not in local.
         * [ ] Auto build recipe if neither local nor remote found.
     * [ ] Add concept of toolset.
         * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
         * [ ] Use toolset in build.
         * [ ] use toolset in queries.
-* version 0.1.4
     * [ ] Add build Date in package properties.
-    * [ ] Allow to force push/pull.
-    * [ ] Allow to sync with remote.
-        * [ ] Allow to pull local package that have newer version.
-        * [ ] Allow to push local package newer than remote or not existing in remote.
+* version 0.1.4
+    * [X] Allow to sync with remote.
+        * [X] Allow to pull local package that have newer version.
+        * [X] Allow to push local package newer than remote or not existing in remote.
+    * [X] Allow to force push/pull.
+    * [X] Bugfix: safe delete
 * version 0.1.3
     * [X] Update internal statuses when using API.
     * [X] omit -d in push/pull command.
     * [X] add progress bar in push/pull command.
     * [X] Allow single thread in build.
 * version 0.1.2
     * [X] Add possibility to force os, arch and compiler for cross compiling.
```

### Comparing `depmanager-0.1.3/pyproject.toml` & `depmanager-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "depmanager"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Silmaen", email = "genteur.slayer@laposte.net" }
 ]
 description = "Simple Dependency manager"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -15,15 +15,15 @@
     #   5 - Production/Stable
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["dependency", "setuptools", "development"]
+keywords = ["dependency", "development", "cmake", "C++"]
 dependencies = [
     "requests",
     "requests-toolbelt",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Silmaen/DepManager"
```

### Comparing `depmanager-0.1.3/src/depmanager/api/builder.py` & `depmanager-0.1.4/src/depmanager/api/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Tools for building packages.
 """
 import platform
-from shutil import rmtree
 from pathlib import Path
+from shutil import rmtree
 from sys import stderr
+
 from depmanager.api.internal.system import LocalSystem, Props
 from depmanager.api.local import LocalManager
 
 
 def try_run(cmd):
     """
     Safe run of commands.
@@ -105,15 +106,15 @@
             out += F" -DCMAKE_CXX_COMPILER={self.cross_info['CXX_COMPILER']}"
         if rec.settings["os"].lower() in ["linux"]:
             out += " -DCMAKE_SKIP_INSTALL_RPATH=ON -DCMAKE_POSITION_INDEPENDENT_CODE=ON"
         for key, val in rec.cache_variables.items():
             out += F" -D{key}={val}"
         return out
 
-    def build_all(self, forced:bool = False):
+    def build_all(self, forced: bool = False):
         """
         Do the build of recipes.
         """
         for rec in self.recipes:
             #
             #
             if rec.kind == "header":
@@ -212,10 +213,10 @@
             if cont:
                 rec.install()
                 p.to_edp_file(self.temp / 'install' / "edp.info")
                 # copy to repository
                 self.local.import_folder(self.temp / 'install')
             # clean Temp
             rec.clean()
-            rmtree(self.temp)
+            rmtree(self.temp, ignore_errors=True)
             if not cont:
                 exit(-666)
```

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/common.py` & `depmanager-0.1.4/src/depmanager/api/internal/common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/database_common.py` & `depmanager-0.1.4/src/depmanager/api/internal/database_common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/database_local.py` & `depmanager-0.1.4/src/depmanager/api/internal/database_local.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/database_remote_folder.py` & `depmanager-0.1.4/src/depmanager/api/internal/database_remote_folder.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/database_remote_ftp.py` & `depmanager-0.1.4/src/depmanager/api/internal/database_remote_ftp.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/database_remote_server.py` & `depmanager-0.1.4/src/depmanager/api/internal/database_remote_server.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/dependency.py` & `depmanager-0.1.4/src/depmanager/api/internal/dependency.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,40 @@
 
     def __gt__(self, other):
         return other < self
 
     def __ge__(self, other):
         return self == other or self > other
 
+    def version_greater(self, other_version):
+        """
+        Compare Version number
+        :param other_version:
+        :return: True if self greater than other version
+        """
+        if type(other_version) == str:
+            compare = other_version
+        elif isinstance(other_version, Props):
+            compare = other_version.version
+        elif isinstance(other_version, Dependency):
+            compare = other_version.properties.version
+        else:
+            compare = str(other_version)
+        if self.version != compare:
+            self_version_item = self.version.split(".")
+            other_version_item = compare.split(".")
+            for i in range(min(len(self_version_item), len(other_version_item))):
+                if self_version_item[i] != other_version_item[i]:
+                    try:
+                        return int(self_version_item[i]) > int(other_version_item[i])
+                    except:
+                        return self_version_item[i] > other_version_item[i]
+            return len(self_version_item) > len(other_version_item)
+        return False
+
     def from_dict(self, data: dict):
         """
         Create props from a dictionary.
         :param data: The input dictionary.
         """
         self.name = "*"
         if "name" in data:
@@ -187,15 +213,15 @@
         idata = data.replace("[", "")
         idata = idata.replace("]", "")
         idata = idata.replace(",", "")
         idata = idata.replace("  ", "")
         idata = idata.replace("/", " ")
         items = idata.split()
         if len(items) != 6:
-            print(f"WARNING: Bad Line format: '{data}': {items}", file = stderr)
+            print(f"WARNING: Bad Line format: '{data}': {items}", file=stderr)
             return
         self.name = items[0]
         self.version = items[1]
         self.arch = items[2]
         self.kind = items[3]
         self.os = items[4]
         self.compiler = items[5].split("-", 1)[0]
```

### Comparing `depmanager-0.1.3/src/depmanager/api/internal/system.py` & `depmanager-0.1.4/src/depmanager/api/internal/system.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/local.py` & `depmanager-0.1.4/src/depmanager/api/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from pathlib import Path
 
 
 class LocalManager:
     """
     Local manager.
     """
-    version = "0.1.3"
+    version = "0.1.4"
 
-    def __init__(self, system=None):
+    def __init__(self, system=None, verbosity: int = 0):
         from depmanager.api.internal.system import LocalSystem
+        self.verbosity = verbosity
         if isinstance(system, LocalSystem):
             self.__sys = system
         else:
-            self.__sys = LocalSystem()
+            self.__sys = LocalSystem(verbosity=verbosity)
         self.root_path = Path(__file__).resolve().parent.parent
 
     def get_sys(self):
         """
         Access to internal system.
         :return: Internal system.
         """
```

### Comparing `depmanager-0.1.3/src/depmanager/api/package.py` & `depmanager-0.1.4/src/depmanager/api/package.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/api/recipe.py` & `depmanager-0.1.4/src/depmanager/api/recipe.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/cmake/DepManager.cmake` & `depmanager-0.1.4/src/depmanager/cmake/DepManager.cmake`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/command/build.py` & `depmanager-0.1.4/src/depmanager/command/build.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/command/get.py` & `depmanager-0.1.4/src/depmanager/command/get.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/command/info.py` & `depmanager-0.1.4/src/depmanager/command/info.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/command/pack.py` & `depmanager-0.1.4/src/depmanager/command/pack.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager/command/remote.py` & `depmanager-0.1.4/src/depmanager/command/remote.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 class RemoteCommand:
     """
     Managing remotes
     """
 
     def __init__(self, verbosity=0, system=None):
         from depmanager.api.remotes import RemotesManager
-        self.remote_instance = RemotesManager(system)
+        self.remote_instance = RemotesManager(system, verbosity)
         self.verbosity = verbosity
 
     def list(self):
         """
         Lists the defined remotes.
         """
         remotes = self.remote_instance.get_remote_list()
         for key, value in remotes.items():
             default = [' ', '*'][value.default]
             if self.verbosity == 0:
                 print(F" {default} {key}")
             else:
-                print(F" {default} [ {['OFFLINE', 'ONLINE '][value.valid_shape]} ] {key} - {value.kind}, {value.destination}")
+                print(
+                        F" {default} [ {['OFFLINE', 'ONLINE '][value.valid_shape]} ] {key} - {value.kind}, {value.destination}")
 
     def add(self, name: str, url: str, default: bool = False, login: str = "", passwd: str = ""):
         """
         Add a remote to the list or modify the existing one.
         :param name: Remote's name.
         :param url: Remote's url
         :param default: If this remote should become the new default
@@ -65,41 +66,23 @@
         :param name: Remote's name.
         """
         if type(name) != str or name in ["", None]:
             print(f"ERROR please give a name for removing a remote.", file=stderr)
             exit(-666)
         self.remote_instance.remove_remote(name)
 
-    def sync(self, name: str, default: bool = False):
+    def sync(self, name: str, default: bool = False, pull_newer: bool = True, push_newer: bool = True):
         """
-        Synchronize local with given remote (push to server all unexisting package).
+        Synchronize local with given remote (push/pull with server all newer package).
         :param name: Remote's name.
         :param default: If using default remote
+        :param pull_newer: Pull images if newer version exists
+        :param push_newer: Push images if newer version exists
         """
-        remote_db = self.remote_instance.get_safe_remote(name, default)
-        if remote_db is None:
-            print(f"ERROR remote {name} not found.", file=stderr)
-            exit(-666)
-        local_db = self.remote_instance.get_local()
-        all_local = local_db.query({
-            "name": "*",
-            "version": "*",
-            "os": "*",
-            "arch": "*",
-            "kind": "*",
-            "compiler": "*"
-        })
-        for single_local in all_local:
-            if len(remote_db.query(single_local)) > 0:
-                print(f"Package {single_local.properties.get_as_str()} Already on server.")
-                continue
-            print(f"==> Push Package {single_local.properties.get_as_str()} to server.")
-            local_db.pack(single_local, self.remote_instance.get_temp_dir(), "tgz")
-            dep_path = self.remote_instance.get_temp_dir() / (single_local.get_path().name + ".tgz")
-            remote_db.push(single_local, dep_path)
+        self.remote_instance.sync_remote(name, default, pull_newer, push_newer)
 
 
 def remote(args, system=None):
     """
     Remote entrypoint.
     :param args: Command Line Arguments.
     :param system: The local system
@@ -110,15 +93,24 @@
     if args.what == "list":
         rem.list()
     elif args.what == "add":
         rem.add(args.name, args.url, args.default, args.login, args.passwd)
     elif args.what == "del":
         rem.delete(args.name)
     elif args.what == "sync":
-        rem.sync(args.name, args.default)
+        do_pull = True
+        do_push = True
+        if args.push_only:
+            do_pull = False
+        if args.pull_only:
+            do_push = False
+        if not (do_push or do_pull):
+            print("ERROR: push-only & pull-only are mutually exclusive.", file=stderr)
+            exit(1)
+        rem.sync(args.name, args.default, do_pull, do_push)
 
 
 def add_remote_parameters(sub_parsers):
     """
     Definition of remote parameters.
     :param sub_parsers: The parent parser.
     """
@@ -145,8 +137,20 @@
     )
     info_parser.add_argument(
             "--passwd", "-p",
             type=str,
             default="",
             help="Password."
     )
+    info_parser.add_argument(
+            "--push-only",
+            action="store_true",
+            default=False,
+            help="Do only the push actions in sync."
+    )
+    info_parser.add_argument(
+            "--pull-only",
+            action="store_true",
+            default=False,
+            help="Do only the pull actions in sync."
+    )
     info_parser.set_defaults(func=remote)
```

### Comparing `depmanager-0.1.3/src/depmanager/manager.py` & `depmanager-0.1.4/src/depmanager/manager.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.3/src/depmanager.egg-info/PKG-INFO` & `depmanager-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,351 +1,354 @@
-Metadata-Version: 2.1
-Name: depmanager
-Version: 0.1.3
-Summary: Simple Dependency manager
-Author-email: Silmaen <genteur.slayer@laposte.net>
-License: MIT License
-        
-        Copyright (c) 2023 Silmaen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Silmaen/DepManager
-Keywords: dependency,setuptools,development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DepManager
-
-Depmanager is a minimalistic tool to manage dependencies (also known as third-party
-libraries) of a C++ Project. It works closely with cmake tool.
-
-It allow to store dependencies in a distant repository to share builds with other and
-have a local cache project-independent.
-
-## Installation
-
-Depmanager is written in python so in the following we assume you have a
-working python installation designated as `<python>` with `pip` installed.
-
-### pip
-
-To install dep manager simply use `<python> -m pip  install depmanager`
-
-See the page on Pypi: [depmanager](https://pypi.org/project/depmanager/).
-
-### From source
-
-Prerequisite: python module 'build' install it with `<python> -m pip install build`
-
-Clone the gitHub repository.
-
-In the source root do:
-
-```powershell
-<python> -m build
-<python> -m pip install dist/depmanager-x.y.z-py3-none-any.whl
-```
-
-## Commandline use
-
-### Get help
-
-For any command or sub-command adding `--help` or `-h` to get help
-on parameters or usage.
-
-### Generalities
-
-In the base commande you can find:
-
-| command | subcommands                 | description                        |
-|---------|-----------------------------|------------------------------------|
-| info    | basedir, cmakedir, version  | info on local instance             |
-| get     |                             | Get the config package             |
-| pack    | pull, push, add, del, query | Manage packages                    |
-| remote  | list, add, del              | Manage the list of distant servers |
-| build   |                             | Build a new package                |
-
-In the following, `<query>` designate something representing the dependency's description.
-The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
-<type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
-
-Valid values for `type`: `shared`, `static`, `header`.
-
-Valid values for `os` : `Windows`, `Linux` (default: host os)
-
-Valid values for `arch` : `x86_64`, `aarch64` (default: host arch)
-
-Valid values for `comiler` : `gnu`, `msvc` (default: `gnu`)
-Note: clang compiler stands for `gnu` while clang-cl stands for `msvc`.
-
-Also, we will designate `<remote>` as a description a remote server, syntax reads: `[-n <name>|-d]`.
-If nothing given, we assume 'local'. If `-d` given, use the default remote, else use the remote by
-its name.
-
-If the name does not exist, it will fall back to default then to local.
-
-## Base commands
-
-### info
-
-subcommands:
-
-* `version` gives the version of the local manager.
-* `basedir` gives the path to the local data of the manager
-* `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
-
-### get
-
-`depmanager get <query>`
-
-Get path to cmake config of the 'best' package given by the query information.
-
-The command will only search in the local cache. This does not intent for human use but more for
-cmake integration.
-
-### pack
-
-Actions on packages.
-
-#### query
-
-`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if
-nothing given) and print the result.
-
-#### add, del
-
-`depmanager pack add <location>` Will add a package to the local database. `<location>` can be a
-folder, then it must contain a properly formatted `edp.info` file. Or an archive (.zip, .tgz or .tar.gz
-file format allowed). The uncompressed archive must contain a properly formatted `edp.info` file.
-
-`depmanager pack del <query>` Will remove from local cache all package matching the query.
-
-#### push, pull
-
-`depmanager pack [push|pull] <query> <remote> [--force(-f)]` will synchronize Local cache with the remote.
-The `query` must be precise enough to match one and only one package. `remote` must be valid.
-
-`push` will look for the package in local cache that match the query and send it to the given remote.
-
-`pull` will look for the package in given remote that match the query and bring it to the local cache.
-
-If `--force` is given, The transfert occurs even if the package already exists in the destination.
-
-### remote
-
-Manage the list of remote servers
-subcommands:
-
-* `list` lists the defined remote server.
-* `add` adds a new remote to the list.
-    * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
-    * Mandatory. If name already exists it will modify the existing one.
-    * Allowed proto are:
-        * `ftp` supports login
-        * `folder` a folder of your computer (mostly for debug or testing)
-        * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
-        * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
-    * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
-* `del <remote>` remove the designated remote if exists.
-* `sync <remote>` push to remote all local package that does not already exist on remote.
-
-### build
-
-`depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
-
-Some option can be passed to the build system:
-
-* `--single-thread`: on some low-end devices (such as RaspberryPi) single thread build is recommended.
-* `--force`, `-f`: Force the build even if the dependency already exists
-* `--cross-c`: redefine the C compiler
-* `--cross-cxx`: redefine the C++ compiler
-* `--cross-arch`: redefine the architecture
-* `--cross-os`: redefine the OS
-
-## Using package with cmake
-
-### Include depmanager to cmake
-
-To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
-to the cmake folder of this installation.
-
-Here is a small cmake code snippet to initialize depmanager in cmake.
-
-```cmake
-# add HINTS or PATH to find the executable if not in the PATH
-find_program(EDEPMANAGER depmanager) 
-if (${EDEPMANAGER} STREQUAL EDEPMANAGER-NOTFOUND)
-    message(FATAL_ERROR "Dependency manager not found.")
-else()
-    execute_process(COMMAND ${EDEPMANAGER} info cmakedir
-            OUTPUT_VARIABLE depmanager_path)
-    string(STRIP ${depmanager_path} depmanager_path)
-    list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
-    include(DepManager)
-endif()
-```
-
-### Find packages
-
-With depmanager initialized in cmake, it provides an alternative to classical `find_package`
-of cmake by `dm_find_package`
-
-```cmake
-dm_find_package(
-   package
-   [QUIET] [TRACE] [REQUIRED]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-)
-```
-
-`package` is the package name to find.
-
-`version` is the exact version to match (wildcard are allowed). By default, find the
-latest one.
-
-`kind` is used to force library kind (`shared`, `static`, `header`). By default it return
-the first found.
-
-If `REQUIRED` set, the function will give an error if no package found.
-(same as original `find_package`)
-
-If `QUIET` set, only errors are written. (same as original `find_package`). In opposition,
-if `TRACE` set, many more debug message displayed.
-
-`target_arch`, `target_os`, `target_compiler` are used in the query. If not set, default
-values are `CMAKE_SYSTEM_PROCESSOR`, `CMAKE_SYSTEM_NAME` and `CMAKE_CXX_COMPILER_ID`
-
-**LIMITATION:** it requires the library name is the package name. So no multi lib or lib with different name.
-
-### Load package
-
-This command is similar to the previous one, but does not directly do a cmake's `find_package`.
-It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
-
-```cmake
-dm_load_package(
-   package
-   [QUIET] [TRACE]
-   [VERSION version]
-   [KIND kind]
-   [ARCH target_arch]
-   [OS target_os]
-   [COMPILER target_compiler]
-)
-```
-
-After call this command, the cmake user has to call for needed `find_package`.
-
-## Create you own package
-
-Depmanager allow you to create your own packages by defining recipes. Then run
-`depmanager build <location of recipes>`
-The program will then build and add dependencies to the local cache.
-
-The location can contain as many recipe in any number of files.
-
-### The recipe
-
-During build, Depmanager will look in all `.py` file for class that inherits from
-depmanager.api.recipe.Recipe.
-
-As for dependency usage, build also rely on cmake for building.
-
-The builder will use the provided recipe in the following workflow:
-
-* Init recipe
-* Call `recipe.source()`
-* Call `recipe.configure()`
-* Initialize options based on recipe data
-* Run cmake configure
-* For all configuration (mostly 'Debug', 'Release')
-    * build target `install`
-* Call `recipe.install()`
-* Generate edp.info file
-* Import into local cache
-* Clean Temporary
-
-Here is a small example
-
-```python
-"""
-Small recipe example
-"""
-from depmanager.api.recipe import Recipe
-
-
-class MyAwesomeLib(Recipe):
-    """
-    Awesome lib
-    """
-    name = "awesome_lib"  # lib name
-    version = "0.0.1.foo"  # lib version
-    source_dir = "src"  # where to fine the sources (especially) the CmakeList.txt
-    kind = "static"  # the lib's kind
-
-
-class AnotherAwesomeLib(MyAwesomeLib):
-    """
-    Shared version of previous one
-    """
-    kind = "shared"
-```
-
-## Roadmap
-
-First of all in the roadmap is to use this tool in C++ project to get feedback.
-
-Among things:
-
-* version 0.2.0
-    * [ ] Do query across multiple source (local then remote).
-    * [ ] Add a sorting order for remotes.
-    * [ ] Auto-pull if not in local.
-        * [ ] Auto build recipe if neither local nor remote found.
-    * [ ] Add concept of toolset.
-        * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
-        * [ ] Use toolset in build.
-        * [ ] use toolset in queries.
-* version 0.1.4
-    * [ ] Add build Date in package properties.
-    * [ ] Allow to force push/pull.
-    * [ ] Allow to sync with remote.
-        * [ ] Allow to pull local package that have newer version.
-        * [ ] Allow to push local package newer than remote or not existing in remote.
-* version 0.1.3
-    * [X] Update internal statuses when using API.
-    * [X] omit -d in push/pull command.
-    * [X] add progress bar in push/pull command.
-    * [X] Allow single thread in build.
-* version 0.1.2
-    * [X] Add possibility to force os, arch and compiler for cross compiling.
-    * [X] Adapt build system to search dependency in the forced environment.
-* version 0.1.1
-    * [X] Add remote 'srv' Type: a dedicated dependency server.
-    * [X] Add remote 'srvs' Type: a dedicated dependency server with secure connexion.
+Metadata-Version: 2.1
+Name: depmanager
+Version: 0.1.4
+Summary: Simple Dependency manager
+Author-email: Silmaen <genteur.slayer@laposte.net>
+License: MIT License
+        
+        Copyright (c) 2023 Silmaen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/Silmaen/DepManager
+Keywords: dependency,development,cmake,C++
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DepManager
+
+Depmanager is a minimalistic tool to manage dependencies (also known as third-party
+libraries) of a C++ Project. It works closely with cmake tool.
+
+It allow to store dependencies in a distant repository to share builds with other and
+have a local cache project-independent.
+
+## Installation
+
+Depmanager is written in python so in the following we assume you have a
+working python installation designated as `<python>` with `pip` installed.
+
+### pip
+
+To install dep manager simply use `<python> -m pip  install depmanager`
+
+See the page on Pypi: [depmanager](https://pypi.org/project/depmanager/).
+
+### From source
+
+Prerequisite: python module 'build' install it with `<python> -m pip install build`
+
+Clone the gitHub repository.
+
+In the source root do:
+
+```powershell
+<python> -m build
+<python> -m pip install dist/depmanager-x.y.z-py3-none-any.whl
+```
+
+## Commandline use
+
+### Get help
+
+For any command or sub-command adding `--help` or `-h` to get help
+on parameters or usage.
+
+### Generalities
+
+In the base commande you can find:
+
+| command | subcommands                 | description                        |
+|---------|-----------------------------|------------------------------------|
+| info    | basedir, cmakedir, version  | info on local instance             |
+| get     |                             | Get the config package             |
+| pack    | pull, push, add, del, query | Manage packages                    |
+| remote  | list, add, del              | Manage the list of distant servers |
+| build   |                             | Build a new package                |
+
+In the following, `<query>` designate something representing the dependency's description.
+The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
+<type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
+
+Valid values for `type`: `shared`, `static`, `header`.
+
+Valid values for `os` : `Windows`, `Linux` (default: host os)
+
+Valid values for `arch` : `x86_64`, `aarch64` (default: host arch)
+
+Valid values for `comiler` : `gnu`, `msvc` (default: `gnu`)
+Note: clang compiler stands for `gnu` while clang-cl stands for `msvc`.
+
+Also, we will designate `<remote>` as a description a remote server, syntax reads: `[-n <name>|-d]`.
+If nothing given, we assume 'local'. If `-d` given, use the default remote, else use the remote by
+its name.
+
+If the name does not exist, it will fall back to default then to local.
+
+## Base commands
+
+### info
+
+subcommands:
+
+* `version` gives the version of the local manager.
+* `basedir` gives the path to the local data of the manager
+* `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
+
+### get
+
+`depmanager get <query>`
+
+Get path to cmake config of the 'best' package given by the query information.
+
+The command will only search in the local cache. This does not intent for human use but more for
+cmake integration.
+
+### pack
+
+Actions on packages.
+
+#### query
+
+`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if
+nothing given) and print the result.
+
+#### add, del
+
+`depmanager pack add <location>` Will add a package to the local database. `<location>` can be a
+folder, then it must contain a properly formatted `edp.info` file. Or an archive (.zip, .tgz or .tar.gz
+file format allowed). The uncompressed archive must contain a properly formatted `edp.info` file.
+
+`depmanager pack del <query>` Will remove from local cache all package matching the query.
+
+#### push, pull
+
+`depmanager pack [push|pull] <query> <remote> [--force(-f)]` will synchronize Local cache with the remote.
+The `query` must be precise enough to match one and only one package. `remote` must be valid.
+
+`push` will look for the package in local cache that match the query and send it to the given remote.
+
+`pull` will look for the package in given remote that match the query and bring it to the local cache.
+
+If `--force` is given, The transfert occurs even if the package already exists in the destination.
+
+### remote
+
+Manage the list of remote servers
+subcommands:
+
+* `list` lists the defined remote server.
+* `add` adds a new remote to the list.
+    * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
+    * Mandatory. If name already exists it will modify the existing one.
+    * Allowed proto are:
+        * `ftp` supports login
+        * `folder` a folder of your computer (mostly for debug or testing)
+        * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
+        * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
+    * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
+* `del <remote>` remove the designated remote if exists.
+* `sync <remote> [--push-only|--pull-only]` push to remote all local package that does not already
+  exist on remote. Pull local package that have a newer version on the remote. If no remote given, it will use the
+  default one.
+
+### build
+
+`depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
+
+Some option can be passed to the build system:
+
+* `--single-thread`: on some low-end devices (such as RaspberryPi) single thread build is recommended.
+* `--force`, `-f`: Force the build even if the dependency already exists
+* `--cross-c`: redefine the C compiler
+* `--cross-cxx`: redefine the C++ compiler
+* `--cross-arch`: redefine the architecture
+* `--cross-os`: redefine the OS
+
+## Using package with cmake
+
+### Include depmanager to cmake
+
+To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
+to the cmake folder of this installation.
+
+Here is a small cmake code snippet to initialize depmanager in cmake.
+
+```cmake
+# add HINTS or PATH to find the executable if not in the PATH
+find_program(EDEPMANAGER depmanager) 
+if (${EDEPMANAGER} STREQUAL EDEPMANAGER-NOTFOUND)
+    message(FATAL_ERROR "Dependency manager not found.")
+else()
+    execute_process(COMMAND ${EDEPMANAGER} info cmakedir
+            OUTPUT_VARIABLE depmanager_path)
+    string(STRIP ${depmanager_path} depmanager_path)
+    list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
+    include(DepManager)
+endif()
+```
+
+### Find packages
+
+With depmanager initialized in cmake, it provides an alternative to classical `find_package`
+of cmake by `dm_find_package`
+
+```cmake
+dm_find_package(
+   package
+   [QUIET] [TRACE] [REQUIRED]
+   [VERSION version]
+   [KIND kind]
+   [ARCH target_arch]
+   [OS target_os]
+   [COMPILER target_compiler]
+)
+```
+
+`package` is the package name to find.
+
+`version` is the exact version to match (wildcard are allowed). By default, find the
+latest one.
+
+`kind` is used to force library kind (`shared`, `static`, `header`). By default it return
+the first found.
+
+If `REQUIRED` set, the function will give an error if no package found.
+(same as original `find_package`)
+
+If `QUIET` set, only errors are written. (same as original `find_package`). In opposition,
+if `TRACE` set, many more debug message displayed.
+
+`target_arch`, `target_os`, `target_compiler` are used in the query. If not set, default
+values are `CMAKE_SYSTEM_PROCESSOR`, `CMAKE_SYSTEM_NAME` and `CMAKE_CXX_COMPILER_ID`
+
+**LIMITATION:** it requires the library name is the package name. So no multi lib or lib with different name.
+
+### Load package
+
+This command is similar to the previous one, but does not directly do a cmake's `find_package`.
+It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
+
+```cmake
+dm_load_package(
+   package
+   [QUIET] [TRACE]
+   [VERSION version]
+   [KIND kind]
+   [ARCH target_arch]
+   [OS target_os]
+   [COMPILER target_compiler]
+)
+```
+
+After call this command, the cmake user has to call for needed `find_package`.
+
+## Create you own package
+
+Depmanager allow you to create your own packages by defining recipes. Then run
+`depmanager build <location of recipes>`
+The program will then build and add dependencies to the local cache.
+
+The location can contain as many recipe in any number of files.
+
+### The recipe
+
+During build, Depmanager will look in all `.py` file for class that inherits from
+depmanager.api.recipe.Recipe.
+
+As for dependency usage, build also rely on cmake for building.
+
+The builder will use the provided recipe in the following workflow:
+
+* Init recipe
+* Call `recipe.source()`
+* Call `recipe.configure()`
+* Initialize options based on recipe data
+* Run cmake configure
+* For all configuration (mostly 'Debug', 'Release')
+    * build target `install`
+* Call `recipe.install()`
+* Generate edp.info file
+* Import into local cache
+* Clean Temporary
+
+Here is a small example
+
+```python
+"""
+Small recipe example
+"""
+from depmanager.api.recipe import Recipe
+
+
+class MyAwesomeLib(Recipe):
+    """
+    Awesome lib
+    """
+    name = "awesome_lib"  # lib name
+    version = "0.0.1.foo"  # lib version
+    source_dir = "src"  # where to fine the sources (especially) the CmakeList.txt
+    kind = "static"  # the lib's kind
+
+
+class AnotherAwesomeLib(MyAwesomeLib):
+    """
+    Shared version of previous one
+    """
+    kind = "shared"
+```
+
+## Roadmap
+
+First of all in the roadmap is to use this tool in C++ project to get feedback.
+
+Among things:
+
+* version 0.2.0
+    * [ ] Do query across multiple source (local then remote).
+    * [ ] Add a sorting order for remotes.
+    * [ ] Auto-pull if not in local.
+        * [ ] Auto build recipe if neither local nor remote found.
+    * [ ] Add concept of toolset.
+        * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
+        * [ ] Use toolset in build.
+        * [ ] use toolset in queries.
+    * [ ] Add build Date in package properties.
+* version 0.1.4
+    * [X] Allow to sync with remote.
+        * [X] Allow to pull local package that have newer version.
+        * [X] Allow to push local package newer than remote or not existing in remote.
+    * [X] Allow to force push/pull.
+    * [X] Bugfix: safe delete
+* version 0.1.3
+    * [X] Update internal statuses when using API.
+    * [X] omit -d in push/pull command.
+    * [X] add progress bar in push/pull command.
+    * [X] Allow single thread in build.
+* version 0.1.2
+    * [X] Add possibility to force os, arch and compiler for cross compiling.
+    * [X] Adapt build system to search dependency in the forced environment.
+* version 0.1.1
+    * [X] Add remote 'srv' Type: a dedicated dependency server.
+    * [X] Add remote 'srvs' Type: a dedicated dependency server with secure connexion.
```

### Comparing `depmanager-0.1.3/src/depmanager.egg-info/SOURCES.txt` & `depmanager-0.1.4/src/depmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

