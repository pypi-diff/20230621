# Comparing `tmp/cpp-automation-utility-0.0.4.tar.gz` & `tmp/cpp-automation-utility-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpp-automation-utility-0.0.4.tar", last modified: Wed May 31 23:40:47 2023, max compression
+gzip compressed data, was "cpp-automation-utility-0.0.5.tar", last modified: Wed Jun 21 00:17:37 2023, max compression
```

## Comparing `cpp-automation-utility-0.0.4.tar` & `cpp-automation-utility-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.296694 cpp-automation-utility-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 23:40:47.296694 cpp-automation-utility-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.293694 cpp-automation-utility-0.0.4/cau/
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/cau_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.293694 cpp-automation-utility-0.0.4/cau/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.294694 cpp-automation-utility-0.0.4/cau/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)     9416 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/Clang.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/Git.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.295694 cpp-automation-utility-0.0.4/cau/wrappers/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Coverage.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Git.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:40:47.296694 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 23:40:47.000000 cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 23:40:47.296694 cpp-automation-utility-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1162 2023-05-31 23:40:38.000000 cpp-automation-utility-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.418174 cpp-automation-utility-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-21 00:17:37.418174 cpp-automation-utility-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.415174 cpp-automation-utility-0.0.5/cau/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/cau_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.415174 cpp-automation-utility-0.0.5/cau/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.416174 cpp-automation-utility-0.0.5/cau/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)     9416 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/Clang.py
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/Git.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.417174 cpp-automation-utility-0.0.5/cau/wrappers/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Git.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:37.418174 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-21 00:17:37.000000 cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 00:17:37.418174 cpp-automation-utility-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-06-21 00:17:27.000000 cpp-automation-utility-0.0.5/setup.py
```

### Comparing `cpp-automation-utility-0.0.4/LICENSE` & `cpp-automation-utility-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/PKG-INFO` & `cpp-automation-utility-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.4/README.md` & `cpp-automation-utility-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/cau_cli.py` & `cpp-automation-utility-0.0.5/cau/cau_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,16 @@
 @cau.timer
 def clean(build_directory: str, all_files: bool, only_build: bool, only_conan: bool):
     """
     Clean project of build files
     """
     conan = cau.Conan(build_directory=build_directory)
     if all_files:
-        result = all(method() for method in (conan.clean_build, conan.clean_conan))
+        results = [method() for method in (conan.clean_build, conan.clean_conan)]
+        result = all(results)
     elif only_build:
         result = conan.clean_build()
     elif only_conan:
         result = conan.clean_conan()
     else:
         sys.exit(0)
     sys.exit(0 if result else 1)
```

### Comparing `cpp-automation-utility-0.0.4/cau/tests/conftest.py` & `cpp-automation-utility-0.0.5/cau/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/tests/test_cli.py` & `cpp-automation-utility-0.0.5/cau/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/timer.py` & `cpp-automation-utility-0.0.5/cau/timer.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/Clang.py` & `cpp-automation-utility-0.0.5/cau/wrappers/Clang.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/Conan.py` & `cpp-automation-utility-0.0.5/cau/wrappers/Conan.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,26 @@
     build_directory: pathlib.Path = attrs.field(
         factory=lambda: pathlib.Path("build"),
         converter=pathlib.Path,
         validator=attrs.validators.instance_of(pathlib.Path),
         on_setattr=[attrs.setters.convert, attrs.setters.validate]
     )
     build_type: str = attrs.field(factory=lambda: "Debug", converter=str, validator=attrs.validators.instance_of(str))
-    platform: str = attrs.field(factory=lambda: "linux", converter=str, validator=attrs.validators.instance_of(str))
+    platform: str = attrs.field(
+        factory=lambda: "linux",
+        converter=str,
+        validator=attrs.validators.instance_of(str),
+        on_setattr=[
+            lambda self, _, platform: self._on_platform_set(platform), attrs.setters.convert, attrs.setters.validate
+        ]
+    )
 
     def __attrs_post_init__(self):
         _ = self._on_home_set(self.home)
+        _ = self._on_platform_set(self.platform)
 
     @property
     def profile(self) -> str:
         """
         Conan profile to use when building based on platform and build type
 
         Returns:
@@ -106,7 +114,11 @@
             logger.error("Could not remove %s due to %s", directory, ex.args)
             return False
         return True
 
     def _on_home_set(self, home: pathlib.Path) -> pathlib.Path:
         os.environ["CONAN_HOME"] = str(home)
         return home
+
+    def _on_platform_set(self, platform: pathlib.Path) -> pathlib.Path:
+        os.environ["PLATFORM"] = str(platform)
+        return platform
```

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/Git.py` & `cpp-automation-utility-0.0.5/cau/wrappers/Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/tests/conftest.py` & `cpp-automation-utility-0.0.5/cau/wrappers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Conan.py` & `cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Conan.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,27 @@
     def test_conan_home_is_set_via_setter(self):
         """
         Asserts CONAN_HOME is properly set via setter
         """
         self.conan.home = pathlib.Path("someawkwardpath")
         assert os.environ.get("CONAN_HOME") == str(self.conan.home)
 
+    def test_platform_is_set_on_init(self):
+        """
+        Asserts PLATFORM environment variable is properly set on init
+        """
+        assert os.environ.get("PLATFORM") == str(self.conan.platform)
+
+    def test_platform_is_set_via_setter(self):
+        """
+        Asserts PLATFORM environment variable is properly set via setter
+        """
+        self.conan.platform = pathlib.Path("win64")
+        assert os.environ.get("PLATFORM") == str(self.conan.platform)
+
     @pytest.mark.usefixtures("successful_process")
     def test_restore(self):
         """
         Asserts that if the restore was successful, error code of 0 is returned
         """
         result = self.conan.restore()
         assert result.returncode == 0
```

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Coverage.py` & `cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Coverage.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Git.py` & `cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cau/wrappers/tests/test_Tidy.py` & `cpp-automation-utility-0.0.5/cau/wrappers/tests/test_Tidy.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/PKG-INFO` & `cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.4/cpp_automation_utility.egg-info/SOURCES.txt` & `cpp-automation-utility-0.0.5/cpp_automation_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.4/setup.py` & `cpp-automation-utility-0.0.5/setup.py`

 * *Files identical despite different names*

