# Comparing `tmp/logger_color-0.0.6.tar.gz` & `tmp/logger_color-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_color-0.0.6.tar", last modified: Fri Oct 28 05:10:16 2022, max compression
+gzip compressed data, was "logger_color-0.0.7.tar", last modified: Wed Jun 21 12:08:08 2023, max compression
```

## Comparing `logger_color-0.0.6.tar` & `logger_color-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-28 05:10:16.487874 logger_color-0.0.6/
--rw-rw-rw-   0        0        0     1091 2022-07-14 18:32:10.000000 logger_color-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     5153 2022-10-28 05:10:16.487874 logger_color-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4235 2022-10-28 05:08:33.000000 logger_color-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-28 05:10:16.477775 logger_color-0.0.6/logger_color/
--rw-rw-rw-   0        0        0     1331 2022-10-28 05:08:33.000000 logger_color-0.0.6/logger_color/__init__.py
--rw-rw-rw-   0        0        0     3444 2022-10-28 04:42:54.000000 logger_color-0.0.6/logger_color/cformatter.py
--rw-rw-rw-   0        0        0     6101 2022-10-28 05:08:33.000000 logger_color-0.0.6/logger_color/clogger.py
--rw-rw-rw-   0        0        0     2354 2022-10-28 05:08:33.000000 logger_color-0.0.6/logger_color/functions.py
--rw-rw-rw-   0        0        0        0 2022-07-14 18:32:30.000000 logger_color-0.0.6/logger_color/py.typed
-drwxrwxrwx   0        0        0        0 2022-10-28 05:10:16.487874 logger_color-0.0.6/logger_color.egg-info/
--rw-rw-rw-   0        0        0     5153 2022-10-28 05:10:16.000000 logger_color-0.0.6/logger_color.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-10-28 05:10:16.000000 logger_color-0.0.6/logger_color.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-28 05:10:16.000000 logger_color-0.0.6/logger_color.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-10-28 05:10:16.000000 logger_color-0.0.6/logger_color.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-28 05:10:16.487874 logger_color-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1318 2022-10-28 05:08:33.000000 logger_color-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:08:08.055608 logger_color-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2022-07-14 18:32:10.000000 logger_color-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     5165 2023-06-21 12:08:08.055608 logger_color-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4235 2023-06-21 12:07:59.000000 logger_color-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 12:08:08.046607 logger_color-0.0.7/logger_color/
+-rw-rw-rw-   0        0        0     1337 2023-06-21 12:06:11.000000 logger_color-0.0.7/logger_color/__init__.py
+-rw-rw-rw-   0        0        0     3444 2022-10-28 04:42:54.000000 logger_color-0.0.7/logger_color/cformatter.py
+-rw-rw-rw-   0        0        0     6357 2023-06-21 12:04:13.000000 logger_color-0.0.7/logger_color/clogger.py
+-rw-rw-rw-   0        0        0     2354 2022-10-28 05:08:33.000000 logger_color-0.0.7/logger_color/functions.py
+-rw-rw-rw-   0        0        0        0 2022-07-14 18:32:30.000000 logger_color-0.0.7/logger_color/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-21 12:08:08.053609 logger_color-0.0.7/logger_color.egg-info/
+-rw-rw-rw-   0        0        0     5165 2023-06-21 12:08:07.000000 logger_color-0.0.7/logger_color.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-21 12:08:08.000000 logger_color-0.0.7/logger_color.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:08:07.000000 logger_color-0.0.7/logger_color.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 12:08:07.000000 logger_color-0.0.7/logger_color.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 12:08:08.056606 logger_color-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1318 2023-06-21 12:07:30.000000 logger_color-0.0.7/setup.py
```

### Comparing `logger_color-0.0.6/LICENSE.txt` & `logger_color-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logger_color-0.0.6/PKG-INFO` & `logger_color-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: logger_color
-Version: 0.0.6
+Version: 0.0.7
 Summary: Different logging levels for stram (terminal) and file. Color the log messages. Has additional levels for diagnostics: DIAG_INFO, DIAG_WARNING.
-Home-page: https://github.com/vladimirs-git/logger
+Home-page: https://github.com/vladimirs-git/logger-color
 Author: Vladimir Prusakov
 Author-email: vladimir.prusakovs@gmail.com
 License: MIT
-Download-URL: https://github.com/vladimirs-git/logger/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.7.tar.gz
 Keywords: logging
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -70,15 +70,15 @@
 
     pip install git+https://github.com/vladimirs-git/logger-color
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.6.tar.gz
+    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.7.tar.gz
 
 
 start_logging()
 ---------------
 **start_logging(filename, mode, level, level_file, color, debug)** - Start logging
 with the specified parameters
```

### Comparing `logger_color-0.0.6/README.rst` & `logger_color-0.0.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     pip install git+https://github.com/vladimirs-git/logger-color
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.6.tar.gz
+    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.7.tar.gz
 
 
 start_logging()
 ---------------
 **start_logging(filename, mode, level, level_file, color, debug)** - Start logging
 with the specified parameters
```

### Comparing `logger_color-0.0.6/logger_color/__init__.py` & `logger_color-0.0.7/logger_color/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     "error",
     "info",
     "start_logging",
     "warning",
 ]
 
 __title__ = "logger_color"
-__version__ = "0.0.6"
-__date__ = "2022-10-28"
+__version__ = "0.0.7"
+__date__ = "2023-06-21"
 
 __summary__ = "Different logging levels for stram (terminal) and file. Color the log messages. " \
               "Has additional levels for diagnostics: DIAG_INFO, DIAG_WARNING."
 __author__ = "Vladimir Prusakov"
 __email__ = "vladimir.prusakovs@gmail.com"
-__url__ = "https://github.com/vladimirs-git/logger"
+__url__ = "https://github.com/vladimirs-git/logger-color"
 __download_url__ = f"{__url__}/archive/refs/tags/{__version__}.tar.gz"
 __license__ = "MIT"
```

### Comparing `logger_color-0.0.6/logger_color/cformatter.py` & `logger_color-0.0.7/logger_color/cformatter.py`

 * *Files identical despite different names*

### Comparing `logger_color-0.0.6/logger_color/clogger.py` & `logger_color-0.0.7/logger_color/clogger.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,17 +133,23 @@
             handler = logger.handlers[0]
             logger.removeHandler(handler)
 
     @staticmethod
     def _check_dir_write(path: str) -> None:
         """Check directory write permission"""
         if not os.path.exists(path):
-            raise OSError(f"absent {path=}")
+            raise OSError(f"Directory does not exist: {path}")
         if not os.access(path, os.W_OK):
-            raise OSError(f"write permission error {path=}")
+            try:
+                test_file = os.path.join(path, ".write_test")
+                with open(test_file, "w") as f:
+                    pass
+                os.remove(test_file)
+            except OSError:
+                raise OSError(f"No write permission for directory: {path}")
 
     def _add_stream_handler(self) -> None:
         """Adds StreamHandler to Logger"""
         logger = logging.getLogger()
         formatter = self._init_formatter(level=self.level, color=self.color)
         handler = logging.StreamHandler(stream=sys.stdout)
         handler.setLevel(self.level)
```

### Comparing `logger_color-0.0.6/logger_color/functions.py` & `logger_color-0.0.7/logger_color/functions.py`

 * *Files identical despite different names*

### Comparing `logger_color-0.0.6/logger_color.egg-info/PKG-INFO` & `logger_color-0.0.7/logger_color.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: logger-color
-Version: 0.0.6
+Version: 0.0.7
 Summary: Different logging levels for stram (terminal) and file. Color the log messages. Has additional levels for diagnostics: DIAG_INFO, DIAG_WARNING.
-Home-page: https://github.com/vladimirs-git/logger
+Home-page: https://github.com/vladimirs-git/logger-color
 Author: Vladimir Prusakov
 Author-email: vladimir.prusakovs@gmail.com
 License: MIT
-Download-URL: https://github.com/vladimirs-git/logger/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.7.tar.gz
 Keywords: logging
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -70,15 +70,15 @@
 
     pip install git+https://github.com/vladimirs-git/logger-color
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.6.tar.gz
+    pip install https://github.com/vladimirs-git/logger-color/archive/refs/tags/0.0.7.tar.gz
 
 
 start_logging()
 ---------------
 **start_logging(filename, mode, level, level_file, color, debug)** - Start logging
 with the specified parameters
```

### Comparing `logger_color-0.0.6/setup.py` & `logger_color-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pathlib
 
 from setuptools import setup, find_packages  # type: ignore
 
 import logger_color as package
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 PACKAGE = package.__title__
 PACKAGE_ = package.__title__.lower().replace("-", "_")  # PEP 503 normalization
 ROOT = pathlib.Path(__file__).parent.resolve()
 README = "README.rst"
 
 if __name__ == "__main__":
     setup(
```

