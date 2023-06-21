# Comparing `tmp/ibott_browser_manager-1.0.4.tar.gz` & `tmp/ibott_browser_manager-1.0.5.tar.gz`

## Comparing `ibott_browser_manager-1.0.4.tar` & `ibott_browser_manager-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.DS_Store
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/readme.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/browser_manager.iml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0    11186 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/browser/__init__.py
--rw-r--r--   0        0        0    11689 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/browser/chrome.py
--rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/browser/driver_utils.py
--rw-r--r--   0        0        0    13637 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/browser/firefox.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/browser/web_elements.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/LICENSE
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    18110 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/readme.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/browser_manager.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/__init__.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/chrome.py
+-rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/driver_utils.py
+-rw-r--r--   0        0        0    13677 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/firefox.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/web_elements.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/LICENSE
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    18110 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/PKG-INFO
```

### Comparing `ibott_browser_manager-1.0.4/readme.md` & `ibott_browser_manager-1.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.4/browser/chrome.py` & `ibott_browser_manager-1.0.5/browser/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.support.wait import WebDriverWait
-from telnetlib import EC
+from selenium.webdriver.support import expected_conditions as EC
 from .driver_utils import install_chrome, ChromeDriverManager, get_chrome_version
 from .web_elements import CustomWebElement
 from selenium.webdriver import Chrome
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 import warnings
 import time
```

### Comparing `ibott_browser_manager-1.0.4/browser/driver_utils.py` & `ibott_browser_manager-1.0.5/browser/driver_utils.py`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.4/browser/firefox.py` & `ibott_browser_manager-1.0.5/browser/firefox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import time
 import warnings
 import os
-from telnetlib import EC
+from selenium.webdriver.support import expected_conditions as EC
 from web_elements import CustomWebElement
 from selenium import webdriver
 from selenium.webdriver import Firefox, FirefoxProfile
 from selenium.webdriver.common.by import By
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.support.wait import WebDriverWait
```

### Comparing `ibott_browser_manager-1.0.4/browser/web_elements.py` & `ibott_browser_manager-1.0.5/browser/web_elements.py`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.4/LICENSE` & `ibott_browser_manager-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.4/README.md` & `ibott_browser_manager-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.4/pyproject.toml` & `ibott_browser_manager-1.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "selenium", "certifi"]
+requires = ["hatchling", "selenium"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ibott_browser_manager"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name="OnameDohe", email="enrique.crespo.debenito@gmail.com" },
 ]
 description = "This packages crates a simple way to work with, Chrome and Firefox Browsers. More info in https://ibott.io/academy/"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `ibott_browser_manager-1.0.4/PKG-INFO` & `ibott_browser_manager-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott_browser_manager
-Version: 1.0.4
+Version: 1.0.5
 Summary: This packages crates a simple way to work with, Chrome and Firefox Browsers. More info in https://ibott.io/academy/
 Project-URL: Homepage, https://github.com/ecrespo66/browser_manager
 Project-URL: Bug Tracker, https://github.com/ecrespo66/browser_manager/issues
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

