# Comparing `tmp/powervaultpy-0.0.4.tar.gz` & `tmp/powervaultpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powervaultpy-0.0.4.tar", last modified: Mon Jun 19 00:14:18 2023, max compression
+gzip compressed data, was "powervaultpy-0.0.5.tar", last modified: Tue Jun 20 22:32:05 2023, max compression
```

## Comparing `powervaultpy-0.0.4.tar` & `powervaultpy-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.740920 powervaultpy-0.0.4/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-19 00:14:18.740512 powervaultpy-0.0.4/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1478 2023-06-19 00:08:35.000000 powervaultpy-0.0.4/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-19 00:14:18.741030 powervaultpy-0.0.4/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.726480 powervaultpy-0.0.4/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.729976 powervaultpy-0.0.4/src/powervaultpy/
--rw-r--r--   0 adam       (501) staff       (20)       47 2023-06-17 23:03:23.000000 powervaultpy-0.0.4/src/powervaultpy/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7249 2023-06-19 00:06:05.000000 powervaultpy-0.0.4/src/powervaultpy/powervault.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-19 00:14:18.739508 powervaultpy-0.0.4/src/powervaultpy.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      273 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       99 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       13 2023-06-19 00:14:18.000000 powervaultpy-0.0.4/src/powervaultpy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:32:05.762438 powervaultpy-0.0.5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-20 22:32:05.762438 powervaultpy-0.0.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1478 2023-06-20 22:32:02.000000 powervaultpy-0.0.5/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-20 22:32:05.762438 powervaultpy-0.0.5/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:32:05.761438 powervaultpy-0.0.5/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:32:05.762438 powervaultpy-0.0.5/src/powervaultpy/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-20 22:25:16.000000 powervaultpy-0.0.5/src/powervaultpy/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7756 2023-06-20 22:29:39.000000 powervaultpy-0.0.5/src/powervaultpy/powervault.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:32:05.762438 powervaultpy-0.0.5/src/powervaultpy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-20 22:32:05.000000 powervaultpy-0.0.5/src/powervaultpy.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      273 2023-06-20 22:32:05.000000 powervaultpy-0.0.5/src/powervaultpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-20 22:32:05.000000 powervaultpy-0.0.5/src/powervaultpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-20 22:32:05.000000 powervaultpy-0.0.5/src/powervaultpy.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-06-20 22:32:05.000000 powervaultpy-0.0.5/src/powervaultpy.egg-info/top_level.txt
```

### Comparing `powervaultpy-0.0.4/PKG-INFO` & `powervaultpy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

### Comparing `powervaultpy-0.0.4/pyproject.toml` & `powervaultpy-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powervaultpy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `powervaultpy-0.0.4/src/powervaultpy/powervault.py` & `powervaultpy-0.0.5/src/powervaultpy/powervault.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,29 @@
             and "units" in units_response
             and units_response["units"] is not None
         ):
             return units_response["units"]
 
         _LOGGER.error("Failed to retrieve units")
 
+        def get_unit(self, unit_id: int) -> any:
+            """Get the unit details from the API."""
+            url = f"{self._base_url}/unit/{unit_id}"
+            unit_response = self._read_response(self._session.get(url), url)
+
+            _LOGGER.debug("Unit: %s", unit_response)
+
+            if (
+                unit_response is not None
+                and "unit" in units_response
+            ):
+                return units_response["unit"]
+
+            _LOGGER.error("Failed to retrieve unit")
+
     def get_account(self) -> any:
         """Get the user's account data from the API."""
         url = f"{self._base_url}/customerAccount"
 
         account_response = self._read_response(self._session.get(url), url)
 
         _LOGGER.debug("Account: %s", account_response)
```

### Comparing `powervaultpy-0.0.4/src/powervaultpy.egg-info/PKG-INFO` & `powervaultpy-0.0.5/src/powervaultpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

