# Comparing `tmp/styledlogger-0.0.5.tar.gz` & `tmp/styledlogger-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.0.5.tar", last modified: Fri May  5 15:21:54 2023, max compression
+gzip compressed data, was "styledlogger-0.1.0.tar", last modified: Wed Jun 21 13:19:32 2023, max compression
```

## Comparing `styledlogger-0.0.5.tar` & `styledlogger-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 15:21:41.000000 styledlogger-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 15:21:54.656999 styledlogger-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 15:21:41.000000 styledlogger-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:21:54.656999 styledlogger-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-05 15:21:41.000000 styledlogger-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.535569 styledlogger-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-21 13:19:20.000000 styledlogger-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 13:19:32.535569 styledlogger-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-21 13:19:20.000000 styledlogger-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:19:32.535569 styledlogger-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 13:19:20.000000 styledlogger-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.531569 styledlogger-0.1.0/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.535569 styledlogger-0.1.0/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.531569 styledlogger-0.1.0/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.0.5/LICENSE` & `styledlogger-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.5/PKG-INFO` & `styledlogger-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.5
+Version: 0.1.0
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -12,37 +12,39 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # StyledLogger
 
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
 Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
+---
+
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
 >>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
+10:13:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
 
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.5/README.md` & `styledlogger-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # StyledLogger
 
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
 Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
+---
+
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
 >>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
+10:13:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
 
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.5/setup.py` & `styledlogger-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     # Basics
     name='styledlogger',
-    version='0.0.5',
+    version='0.1.0',
     description='A simple, styled logging library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # Author
     author='ImAlek (splayzdk)',
     author_email='alek@imalek.me',
```

### Comparing `styledlogger-0.0.5/styledlogger/classes/printcolors.py` & `styledlogger-0.1.0/styledlogger/classes/printcolors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     BLINK = "\033[5m"
     NEGATIVE = "\033[7m"
     CROSSED = "\033[9m"
     RESET = "\033[0m"
     if not __import__("sys").stdout.isatty():
         for _ in dir():
             if isinstance(_, str) and _[0] != "_":
-                locals()[_] = ""
+                locals()[_] = ""
```

### Comparing `styledlogger-0.0.5/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.1.0/styledlogger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.5
+Version: 0.1.0
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -12,37 +12,39 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # StyledLogger
 
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
 Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
+---
+
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
 >>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
+10:13:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
 
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

