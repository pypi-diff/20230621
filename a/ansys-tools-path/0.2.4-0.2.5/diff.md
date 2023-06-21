# Comparing `tmp/ansys_tools_path-0.2.4.tar.gz` & `tmp/ansys_tools_path-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.2.4.tar` & `ansys_tools_path-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/LICENSE
--rw-r--r--   0        0        0     4691 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/README.rst
--rw-r--r--   0        0        0     1843 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      919 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    26062 2023-05-25 07:10:14.342738 ansys_tools_path-0.2.4/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4691 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/README.rst
+-rw-r--r--   0        0        0     1843 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    26232 2023-06-21 10:32:19.720650 ansys_tools_path-0.2.5/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.5/PKG-INFO
```

### Comparing `ansys_tools_path-0.2.4/LICENSE` & `ansys_tools_path-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.4/README.rst` & `ansys_tools_path-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.4/pyproject.toml` & `ansys_tools_path-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.4"
+version = "0.2.5"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys_tools_path-0.2.4/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.2.5/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.4/src/ansys/tools/path/misc.py` & `ansys_tools_path-0.2.5/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.4/src/ansys/tools/path/path.py` & `ansys_tools_path-0.2.5/src/ansys/tools/path/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,17 @@
             "Unable to create settings directory.\n"
             "Will be unable to cache product executable locations"
         )
 
 CONFIG_FILE = os.path.join(SETTINGS_DIR, CONFIG_FILE_NAME)
 
 
-def _get_installed_windows_versions(supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def _get_installed_windows_versions(
+    supported_versions=SUPPORTED_ANSYS_VERSIONS,
+):  # pragma: no cover
     """Get the AWP_ROOT environment variable values for supported versions."""
 
     # The student version overwrites the AWP_ROOT env var
     # (if it is installed later)
     # However the priority should be given to the non-student version.
     awp_roots = []
     awp_roots_student = []
@@ -99,15 +101,15 @@
 
     for path in LINUX_DEFAULT_DIRS:
         if os.path.isdir(path):
             return path
     return None  # pragma: no cover
 
 
-def _get_default_windows_base_path():
+def _get_default_windows_base_path():  # pragma: no cover
     """Get the default base path of the Ansys unified install on windows."""
 
     base_path = os.path.join(os.environ["PROGRAMFILES"], "ANSYS INC")
     if not os.path.exists(base_path):
         LOG.debug(f"The supposed 'base_path'{base_path} does not exist. No available ansys found.")
         return None
     return base_path
@@ -261,15 +263,15 @@
 
     >>> find_mechanical()
     (/usr/ansys_inc/v231/aisol/.workbench, 23.1)
     """
     ans_path, version = _get_unified_install_base_for_version(version, supported_versions)
     if not ans_path or not version:
         return "", ""
-    if is_windows():
+    if is_windows():  # pragma: no cover
         mechanical_bin = os.path.join(ans_path, "aisol", "bin", "winx64", f"AnsysWBU.exe")
     else:
         mechanical_bin = os.path.join(ans_path, "aisol", ".workbench")
     return mechanical_bin, int(version) / 10
 
 
 def find_mapdl(version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
@@ -341,15 +343,15 @@
 def is_valid_executable_path(product: str, exe_loc: str):
     if product == "mapdl":
         return (
             os.path.isfile(exe_loc)
             and re.search(r"ansys\d\d\d", os.path.basename(os.path.normpath(exe_loc))) is not None
         )
     elif product == "mechanical":
-        if is_windows():
+        if is_windows():  # pragma: no cover
             return (
                 os.path.isfile(exe_loc)
                 and re.search("AnsysWBU.exe", os.path.basename(os.path.normpath(exe_loc)))
                 is not None
             )
         return (
             os.path.isfile(exe_loc)
@@ -358,50 +360,46 @@
     raise Exception("unexpected application")
 
 
 def _is_common_executable_path(product: str, exe_loc: str) -> bool:
     if product == "mapdl":
         path = os.path.normpath(exe_loc)
         path = path.split(os.sep)
-        if (
-            re.search(r"v(\d\d\d)", exe_loc) is not None
-            and re.search(r"ansys(\d\d\d)", exe_loc) is not None
-        ):
-            equal_version = (
-                re.search(r"v(\d\d\d)", exe_loc)[1] == re.search(r"ansys(\d\d\d)", exe_loc)[1]
-            )
-        else:
-            equal_version = False
-
+        # Look for all v(\d\d\d) to catch the last one
+        # in case the user has placed the installation folder inside a folder called for example (/ansys/v211)
+        v_version = re.findall(r"v(\d\d\d)", exe_loc)
+        ansys_version = re.findall(r"ansys(\d\d\d)", exe_loc, re.IGNORECASE)
         return (
-            is_valid_executable_path("mapdl", exe_loc)
-            and re.search(r"v\d\d\d", exe_loc)
+            len(v_version) != 0
+            and len(ansys_version) != 0
+            and v_version[-1] == ansys_version[-1]
+            and is_valid_executable_path("mapdl", exe_loc)
             and "ansys" in path
             and "bin" in path
-            and equal_version
         )
+
     elif product == "mechanical":
         path = os.path.normpath(exe_loc)
         path = path.split(os.sep)
 
-        is_valid_path = is_valid_executable_path(exe_loc)
+        is_valid_path = is_valid_executable_path("mechanical", exe_loc)
 
-        if is_windows():
+        if is_windows():  # pragma: no cover
             return (
                 is_valid_path
-                and re.search(r"v\d\d\d", exe_loc)
+                and re.search(r"v\d\d\d", exe_loc) is not None
                 and "aisol" in path
-                and "bin" in path
+                and ("bin" in path or "Bin" in path)
                 and "winx64" in path
-                and "AnsysWBU.exe" in path
+                and ("AnsysWBU.exe" in path or "ANSYSWBU.exe" in path)
             )
 
         return (
             is_valid_path
-            and re.search(r"v\d\d\d", exe_loc)
+            and re.search(r"v\d\d\d", exe_loc) is not None
             and "aisol" in path
             and ".workbench" in path
         )
     else:
         raise Exception("unexpected application")
 
 
@@ -485,17 +483,16 @@
 
     if is_valid_executable_path(product, exe_loc):
         _check_uncommon_executable_path(product, exe_loc)
 
         _change_default_path(product, exe_loc)
         return exe_loc
 
-    if exe_loc is not None:
-        if is_valid_executable_path(product, exe_loc):
-            return exe_loc
+    if is_valid_executable_path(product, exe_loc):
+        return exe_loc
     if allow_prompt:
         exe_loc = _prompt_path(product)
     return exe_loc
 
 
 def save_mechanical_path(exe_loc=None, allow_prompt=True):  # pragma: no cover
     """Find the Mechanical path or query user.
```

### Comparing `ansys_tools_path-0.2.4/PKG-INFO` & `ansys_tools_path-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

