# Comparing `tmp/styledlogger-0.0.5.tar.gz` & `tmp/styledlogger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.0.5.tar", last modified: Fri May  5 15:21:54 2023, max compression
+gzip compressed data, was "styledlogger-0.0.6.tar", last modified: Wed Jun 21 12:41:37 2023, max compression
```

## Comparing `styledlogger-0.0.5.tar` & `styledlogger-0.0.6.tar`

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
+drwxrwxrwx   0        0        0        0 2023-06-21 12:41:37.811881 styledlogger-0.0.6/
+-rw-rw-rw-   0        0        0     1361 2023-06-21 12:30:28.000000 styledlogger-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1791 2023-06-21 12:41:37.811881 styledlogger-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2023-06-21 12:30:28.000000 styledlogger-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 12:41:37.811881 styledlogger-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-06-21 12:40:59.000000 styledlogger-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:41:37.803337 styledlogger-0.0.6/styledlogger/
+-rw-rw-rw-   0        0        0      242 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:41:37.811881 styledlogger-0.0.6/styledlogger/classes/
+-rw-rw-rw-   0        0        0        0 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/classes/__init__.py
+-rw-rw-rw-   0        0        0      852 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/classes/printcolors.py
+-rw-rw-rw-   0        0        0      519 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/classes/printtypes.py
+-rw-rw-rw-   0        0        0     3668 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/classes/styleconfig.py
+-rw-rw-rw-   0        0        0     2607 2023-06-21 12:30:28.000000 styledlogger-0.0.6/styledlogger/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:41:37.808375 styledlogger-0.0.6/styledlogger.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-06-21 12:41:37.000000 styledlogger-0.0.6/styledlogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-06-21 12:41:37.000000 styledlogger-0.0.6/styledlogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:41:37.000000 styledlogger-0.0.6/styledlogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-21 12:41:37.000000 styledlogger-0.0.6/styledlogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 12:41:37.000000 styledlogger-0.0.6/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.0.5/LICENSE` & `styledlogger-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Boost Software License - Version 1.0 - August 17th, 2003
-
-Permission is hereby granted, free of charge, to any person or organization
-obtaining a copy of the software and accompanying documentation covered by
-this license (the "Software") to use, reproduce, display, distribute,
-execute, and transmit the Software, and to prepare derivative works of the
-Software, and to permit third-parties to whom the Software is furnished to
-do so, all subject to the following:
-
-The copyright notices in the Software and this entire statement, including
-the above license grant, this restriction and the following disclaimer,
-must be included in all copies of the Software, in whole or in part, and
-all derivative works of the Software, unless such copies or derivative
-works are solely in the form of machine-executable object code generated by
-a source language processor.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
-SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
-FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

### Comparing `styledlogger-0.0.5/PKG-INFO` & `styledlogger-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-Metadata-Version: 2.1
-Name: styledlogger
-Version: 0.0.5
-Summary: A simple, styled logging library.
-Home-page: https://github.com/SpLayzDK/StyledLogger/
-Author: ImAlek (splayzdk)
-Author-email: alek@imalek.me
-License: BSL 1.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# StyledLogger
-
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
-
-To use, simply install via `pip install styledlogger`
-
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
-
-Simple example using a logger:
-
-```py
->>> from styledlogger import StyledLogger
-
->>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
-
->>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
-
->>> logger.error("Could not fetch url 'https://example.com'")
-10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
-
->>> from styledlogger import StyleConfig
-
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
-
->>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
-```
-
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
-Contact me at mail: alek@imalek.me
+Metadata-Version: 2.1
+Name: styledlogger
+Version: 0.0.6
+Summary: A simple, styled logging library.
+Home-page: https://github.com/SpLayzDK/StyledLogger/
+Author: ImAlek (splayzdk)
+Author-email: alek@imalek.me
+License: BSL 1.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# StyledLogger
+
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
+
+To use, simply install via `pip install styledlogger`
+
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+
+---
+
+Simple example using a logger:
+
+```py
+>>> from styledlogger import StyledLogger
+
+>>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
+
+>>> logger.debug("This is just a test print")
+10:13:30 :: DEBU @ Main - This is just a test print
+
+>>> logger.error("Could not fetch url 'https://example.com'")
+10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
+
+>>> from styledlogger import StyleConfig
+
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
+>>> logger.warn("CPU usage exceeding 90%")
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
+```
+
+Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.5/README.md` & `styledlogger-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# StyledLogger
-
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
-
-To use, simply install via `pip install styledlogger`
-
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
-
-Simple example using a logger:
-
-```py
->>> from styledlogger import StyledLogger
-
->>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
-
->>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
-
->>> logger.error("Could not fetch url 'https://example.com'")
-10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
-
->>> from styledlogger import StyleConfig
-
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
-
->>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
-```
-
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+# StyledLogger
+
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
+
+To use, simply install via `pip install styledlogger`
+
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+
+---
+
+Simple example using a logger:
+
+```py
+>>> from styledlogger import StyledLogger
+
+>>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
+
+>>> logger.debug("This is just a test print")
+10:13:30 :: DEBU @ Main - This is just a test print
+
+>>> logger.error("Could not fetch url 'https://example.com'")
+10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
+
+>>> from styledlogger import StyleConfig
+
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
+>>> logger.warn("CPU usage exceeding 90%")
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
+```
+
+Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.5/styledlogger/classes/printcolors.py` & `styledlogger-0.0.6/styledlogger/classes/printcolors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-class Colors:
-    """ ANSI color codes """
-    BLACK = "\033[0;30m"
-    RED = "\033[0;31m"
-    GREEN = "\033[0;32m"
-    BROWN = "\033[0;33m"
-    BLUE = "\033[0;34m"
-    PURPLE = "\033[0;35m"
-    CYAN = "\033[0;36m"
-    LIGHT_GRAY = "\033[0;37m"
-    DARK_GRAY = "\033[1;30m"
-    LIGHT_RED = "\033[1;31m"
-    LIGHT_GREEN = "\033[1;32m"
-    YELLOW = "\033[1;33m"
-    LIGHT_BLUE = "\033[1;34m"
-    LIGHT_PURPLE = "\033[1;35m"
-    LIGHT_CYAN = "\033[1;36m"
-    LIGHT_WHITE = "\033[1;37m"
-    BOLD = "\033[1m"
-    FAINT = "\033[2m"
-    ITALIC = "\033[3m"
-    UNDERLINE = "\033[4m"
-    BLINK = "\033[5m"
-    NEGATIVE = "\033[7m"
-    CROSSED = "\033[9m"
-    RESET = "\033[0m"
-    if not __import__("sys").stdout.isatty():
-        for _ in dir():
-            if isinstance(_, str) and _[0] != "_":
-                locals()[_] = ""
+class Colors:
+    """ ANSI color codes """
+    BLACK = "\033[0;30m"
+    RED = "\033[0;31m"
+    GREEN = "\033[0;32m"
+    BROWN = "\033[0;33m"
+    BLUE = "\033[0;34m"
+    PURPLE = "\033[0;35m"
+    CYAN = "\033[0;36m"
+    LIGHT_GRAY = "\033[0;37m"
+    DARK_GRAY = "\033[1;30m"
+    LIGHT_RED = "\033[1;31m"
+    LIGHT_GREEN = "\033[1;32m"
+    YELLOW = "\033[1;33m"
+    LIGHT_BLUE = "\033[1;34m"
+    LIGHT_PURPLE = "\033[1;35m"
+    LIGHT_CYAN = "\033[1;36m"
+    LIGHT_WHITE = "\033[1;37m"
+    BOLD = "\033[1m"
+    FAINT = "\033[2m"
+    ITALIC = "\033[3m"
+    UNDERLINE = "\033[4m"
+    BLINK = "\033[5m"
+    NEGATIVE = "\033[7m"
+    CROSSED = "\033[9m"
+    RESET = "\033[0m"
+    if not __import__("sys").stdout.isatty():
+        for _ in dir():
+            if isinstance(_, str) and _[0] != "_":
+                locals()[_] = ""
```

### Comparing `styledlogger-0.0.5/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.0.6/styledlogger.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-Metadata-Version: 2.1
-Name: styledlogger
-Version: 0.0.5
-Summary: A simple, styled logging library.
-Home-page: https://github.com/SpLayzDK/StyledLogger/
-Author: ImAlek (splayzdk)
-Author-email: alek@imalek.me
-License: BSL 1.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# StyledLogger
-
-### A simple - yet beautiful logging library for Python 🐍 > 3.7
-
-To use, simply install via `pip install styledlogger`
-
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
-
-Simple example using a logger:
-
-```py
->>> from styledlogger import StyledLogger
-
->>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
-
->>> logger.debug("This is just a test print")
-9:55:30 :: DEBU @ Main - This is just a test print
-
->>> logger.error("Could not fetch url 'https://example.com'")
-10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
-
->>> from styledlogger import StyleConfig
-
->>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
-
->>> logger.warn("CPU usage exceeding 90%")
-(22/04/2023 10:01) | WARN - CPU usage exceeding 90%
-```
-
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
-Contact me at mail: alek@imalek.me
+Metadata-Version: 2.1
+Name: styledlogger
+Version: 0.0.6
+Summary: A simple, styled logging library.
+Home-page: https://github.com/SpLayzDK/StyledLogger/
+Author: ImAlek (splayzdk)
+Author-email: alek@imalek.me
+License: BSL 1.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# StyledLogger
+
+### A simple, yet beautiful logging library for Python 🐍 > 3.7
+
+To use, simply install via `pip install styledlogger`
+
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+
+---
+
+Simple example using a logger:
+
+```py
+>>> from styledlogger import StyledLogger
+
+>>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
+
+>>> logger.debug("This is just a test print")
+10:13:30 :: DEBU @ Main - This is just a test print
+
+>>> logger.error("Could not fetch url 'https://example.com'")
+10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
+
+>>> from styledlogger import StyleConfig
+
+>>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
+>>> logger.warn("CPU usage exceeding 90%")
+22/04/2023 10:01 | WARN - CPU usage exceeding 90%
+```
+
+Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+Contact me at mail: alek@imalek.me
```

