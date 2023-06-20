# Comparing `tmp/unipropic-1.1.2.tar.gz` & `tmp/unipropic-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipropic-1.1.2.tar", max compression
+gzip compressed data, was "unipropic-1.1.3.tar", max compression
```

## Comparing `unipropic-1.1.2.tar` & `unipropic-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-06 17:14:01.183754 unipropic-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1879 2023-06-06 17:14:01.183754 unipropic-1.1.2/README.md
--rw-r--r--   0        0        0      808 2023-06-06 20:23:49.252468 unipropic-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      304 2023-06-06 20:24:02.462532 unipropic-1.1.2/src/unipropic/__init__.py
--rw-r--r--   0        0        0     3461 2023-06-06 17:14:01.193755 unipropic-1.1.2/src/unipropic/config_manager.py
--rw-r--r--   0        0        0     6758 2023-06-06 18:46:22.790773 unipropic-1.1.2/src/unipropic/main.py
--rw-r--r--   0        0        0      811 2023-06-06 17:14:01.193755 unipropic-1.1.2/src/unipropic/messages.py
--rw-r--r--   0        0        0    29823 2023-06-06 20:04:59.973649 unipropic-1.1.2/src/unipropic/webdriver_handlers.py
--rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 unipropic-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 17:14:01.183754 unipropic-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1879 2023-06-06 17:14:01.183754 unipropic-1.1.3/README.md
+-rw-r--r--   0        0        0      808 2023-06-20 23:35:13.831514 unipropic-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      304 2023-06-20 23:35:17.488199 unipropic-1.1.3/src/unipropic/__init__.py
+-rw-r--r--   0        0        0     3461 2023-06-06 17:14:01.193755 unipropic-1.1.3/src/unipropic/config_manager.py
+-rw-r--r--   0        0        0     6758 2023-06-06 18:46:22.790773 unipropic-1.1.3/src/unipropic/main.py
+-rw-r--r--   0        0        0      811 2023-06-06 17:14:01.193755 unipropic-1.1.3/src/unipropic/messages.py
+-rw-r--r--   0        0        0    29780 2023-06-20 23:34:04.347821 unipropic-1.1.3/src/unipropic/webdriver_handlers.py
+-rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 unipropic-1.1.3/PKG-INFO
```

### Comparing `unipropic-1.1.2/LICENSE.txt` & `unipropic-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.2/README.md` & `unipropic-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.2/pyproject.toml` & `unipropic-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unipropic"
-version = "1.1.2"
+version = "1.1.3"
 description = "A CLI app that automatically puts a profile image in all your accounts."
 authors = ["kutu-dev"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["web", "utility", "automation", "profile"]
 homepage = "https://github.com/kutu-dev/unipropic"
 classifiers = [
```

### Comparing `unipropic-1.1.2/src/unipropic/config_manager.py` & `unipropic-1.1.3/src/unipropic/config_manager.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.2/src/unipropic/main.py` & `unipropic-1.1.3/src/unipropic/main.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.2/src/unipropic/messages.py` & `unipropic-1.1.3/src/unipropic/messages.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.2/src/unipropic/webdriver_handlers.py` & `unipropic-1.1.3/src/unipropic/webdriver_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,17 +613,17 @@
         
             Messages.info(f'Profile saved as default, you can reset it using {Messages.format_argument("forget-config")}')
             self.config_manager.set_value_by_key('firefox', str(firefox_profile_path))
         
         service: FirefoxService = FirefoxService(GeckoDriverManager().install())
         options: webdriver.FirefoxOptions = webdriver.FirefoxOptions()
         options.binary_location = self.binary_path
-        profile: webdriver.FirefoxProfile = webdriver.FirefoxProfile(firefox_profile_path)
+        options.profile = webdriver.FirefoxProfile(firefox_profile_path)
 
-        return webdriver.Firefox(service=service, options=options, firefox_profile=profile)
+        return webdriver.Firefox(service=service, options=options)
 
 class ChromeVariant(Enum):
     GOOGLE = {'display_name': 'Chrome', 'chrome_type': ChromeType.GOOGLE}
     CHROMIUM = {'display_name': 'Chromium', 'chrome_type': ChromeType.CHROMIUM}
     BRAVE = {'display_name': 'Brave', 'chrome_type': ChromeType.BRAVE}
 
 class ChromeBasedProfilePictureHandler(ProfilePictureHandler):
```

### Comparing `unipropic-1.1.2/PKG-INFO` & `unipropic-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipropic
-Version: 1.1.2
+Version: 1.1.3
 Summary: A CLI app that automatically puts a profile image in all your accounts.
 Home-page: https://github.com/kutu-dev/unipropic
 License: MIT
 Keywords: web,utility,automation,profile
 Author: kutu-dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

