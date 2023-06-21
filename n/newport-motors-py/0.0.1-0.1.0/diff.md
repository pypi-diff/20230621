# Comparing `tmp/newport-motors-py-0.0.1.tar.gz` & `tmp/newport-motors-py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport-motors-py-0.0.1.tar", last modified: Sun Jun 18 09:33:18 2023, max compression
+gzip compressed data, was "newport-motors-py-0.1.0.tar", last modified: Wed Jun 21 03:25:22 2023, max compression
```

## Comparing `newport-motors-py-0.0.1.tar` & `newport-motors-py-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1067 2023-06-18 08:47:09.000000 newport-motors-py-0.0.1/LICENSE
--rw-rw-r--   0 adam      (1000) adam      (1000)      495 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/PKG-INFO
--rw-rw-r--   0 adam      (1000) adam      (1000)     4367 2023-06-18 08:47:09.000000 newport-motors-py-0.0.1/README.md
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors/
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors/GUI/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1612 2023-05-15 00:20:57.000000 newport-motors-py-0.0.1/newport_motors/GUI/CustomNumeric.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      141 2023-05-15 01:50:46.000000 newport-motors-py-0.0.1/newport_motors/GUI/InstrumentGUI.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      982 2023-06-05 00:14:07.000000 newport-motors-py-0.0.1/newport_motors/GUI/LinearUI.py
--rw-rw-r--   0 adam      (1000) adam      (1000)     2206 2023-06-07 05:22:30.000000 newport-motors-py-0.0.1/newport_motors/GUI/TipTiltUI.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors/Mocks/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1637 2023-05-11 05:05:38.000000 newport-motors-py-0.0.1/newport_motors/Mocks/motor.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors/Motors/
--rw-rw-r--   0 adam      (1000) adam      (1000)     7395 2023-06-10 00:24:39.000000 newport-motors-py-0.0.1/newport_motors/Motors/instrument.py
--rw-rw-r--   0 adam      (1000) adam      (1000)    11499 2023-06-10 00:27:37.000000 newport-motors-py-0.0.1/newport_motors/Motors/motor.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors/USBs/
--rw-rw-r--   0 adam      (1000) adam      (1000)     3779 2023-06-10 00:28:40.000000 newport-motors-py-0.0.1/newport_motors/USBs/USBs.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      139 2023-05-11 23:39:01.000000 newport-motors-py-0.0.1/newport_motors/__init__.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/newport_motors_py.egg-info/
--rw-rw-r--   0 adam      (1000) adam      (1000)      495 2023-06-18 09:33:18.000000 newport-motors-py-0.0.1/newport_motors_py.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1000) adam      (1000)      562 2023-06-18 09:33:18.000000 newport-motors-py-0.0.1/newport_motors_py.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)        1 2023-06-18 09:33:18.000000 newport-motors-py-0.0.1/newport_motors_py.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)     2248 2023-06-18 09:33:18.000000 newport-motors-py-0.0.1/newport_motors_py.egg-info/requires.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)       97 2023-06-18 09:33:18.000000 newport-motors-py-0.0.1/newport_motors_py.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)       38 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/setup.cfg
--rw-rw-r--   0 adam      (1000) adam      (1000)     1931 2023-06-18 09:33:14.000000 newport-motors-py-0.0.1/setup.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-18 09:33:18.392613 newport-motors-py-0.0.1/tests/
--rw-rw-r--   0 adam      (1000) adam      (1000)     1129 2023-06-05 00:14:03.000000 newport-motors-py-0.0.1/tests/test_motor.py
--rw-rw-r--   0 adam      (1000) adam      (1000)     1198 2023-05-29 06:25:23.000000 newport-motors-py-0.0.1/tests/test_motor_mock.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1067 2023-06-18 08:47:09.000000 newport-motors-py-0.1.0/LICENSE
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/PKG-INFO
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4199 2023-06-21 03:22:07.000000 newport-motors-py-0.1.0/README.md
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/GUI/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1612 2023-05-15 00:20:57.000000 newport-motors-py-0.1.0/newport_motors/GUI/CustomNumeric.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      141 2023-05-15 01:50:46.000000 newport-motors-py-0.1.0/newport_motors/GUI/InstrumentGUI.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      982 2023-06-05 00:14:07.000000 newport-motors-py-0.1.0/newport_motors/GUI/LinearUI.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)     2206 2023-06-07 05:22:30.000000 newport-motors-py-0.1.0/newport_motors/GUI/TipTiltUI.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/Mocks/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1637 2023-05-11 05:05:38.000000 newport-motors-py-0.1.0/newport_motors/Mocks/motor.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/Motors/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     7395 2023-06-10 00:24:39.000000 newport-motors-py-0.1.0/newport_motors/Motors/instrument.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)    11499 2023-06-10 00:27:37.000000 newport-motors-py-0.1.0/newport_motors/Motors/motor.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors/USBs/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     3779 2023-06-10 00:28:40.000000 newport-motors-py-0.1.0/newport_motors/USBs/USBs.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      211 2023-06-19 13:13:53.000000 newport-motors-py-0.1.0/newport_motors/__init__.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/newport_motors_py.egg-info/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     4659 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1000) adam      (1000)      586 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)        1 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)       60 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1000) adam      (1000)      109 2023-06-21 03:25:22.000000 newport-motors-py-0.1.0/newport_motors_py.egg-info/top_level.txt
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/pyvisa_mock/
+-rw-rw-r--   0 adam      (1000) adam      (1000)       87 2023-06-21 03:15:09.000000 newport-motors-py-0.1.0/pyvisa_mock/__init__.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)       38 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/setup.cfg
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1893 2023-06-21 03:15:37.000000 newport-motors-py-0.1.0/setup.py
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2023-06-21 03:25:22.172807 newport-motors-py-0.1.0/tests/
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1125 2023-06-19 12:49:39.000000 newport-motors-py-0.1.0/tests/test_motor.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)     1178 2023-06-19 13:05:28.000000 newport-motors-py-0.1.0/tests/test_motor_mock.py
```

### Comparing `newport-motors-py-0.0.1/LICENSE` & `newport-motors-py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/README.md` & `newport-motors-py-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -91,13 +91,12 @@
    sudo modprobe ftdi_sio vendor=0x104d:3008 product=3008
    sudo sh -c 'echo "104d 3008" > /sys/bus/usb-serial/drivers/ftdi_sio/new_id'
 fi
 ```
 Since this has `sudo` commands, you will need to enter your password the first time you open a new terminal.
 
 ## Sim mode:
-Uses https://github.com/microsoft/pyvisa-mock
+Uses https://github.com/microsoft/pyvisa-mock. If you wish to use it you must install it from source (and possibly change `python_requires` in `setup.py`). 
 
-## install
-To use the sim env with pyvisa mock, you must manually change a line in the pyvisa file to correctly find the mock package. Change line 2820 in `highlevel.py` to use "pyvisa" instead of "pyvisa_". Then, when running in sim, create the resource manager like `pyvisa.ResourceManager(visa_library="@-mock")` and if for real use `pyvisa.ResourceManager(visa_library="@-py")`
+The pyvisa_mock package is defined in this package and is correctly re-exported with `pip install .`.
```

### Comparing `newport-motors-py-0.0.1/newport_motors/GUI/CustomNumeric.py` & `newport-motors-py-0.1.0/newport_motors/GUI/CustomNumeric.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/GUI/LinearUI.py` & `newport-motors-py-0.1.0/newport_motors/GUI/LinearUI.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/GUI/TipTiltUI.py` & `newport-motors-py-0.1.0/newport_motors/GUI/TipTiltUI.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/Mocks/motor.py` & `newport-motors-py-0.1.0/newport_motors/Mocks/motor.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/Motors/instrument.py` & `newport-motors-py-0.1.0/newport_motors/Motors/instrument.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/Motors/motor.py` & `newport-motors-py-0.1.0/newport_motors/Motors/motor.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors/USBs/USBs.py` & `newport-motors-py-0.1.0/newport_motors/USBs/USBs.py`

 * *Files identical despite different names*

### Comparing `newport-motors-py-0.0.1/newport_motors_py.egg-info/SOURCES.txt` & `newport-motors-py-0.1.0/newport_motors_py.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 newport_motors/Motors/motor.py
 newport_motors/USBs/USBs.py
 newport_motors_py.egg-info/PKG-INFO
 newport_motors_py.egg-info/SOURCES.txt
 newport_motors_py.egg-info/dependency_links.txt
 newport_motors_py.egg-info/requires.txt
 newport_motors_py.egg-info/top_level.txt
+pyvisa_mock/__init__.py
 tests/test_motor.py
 tests/test_motor_mock.py
```

### Comparing `newport-motors-py-0.0.1/setup.py` & `newport-motors-py-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 import setuptools
 import os
 import codecs
 import re
 
-# with open("README.md", "r", encoding="utf-8") as fh:
-#     long_description = fh.read()
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+# long_description = "A python package for operating multiple newport motors in an optical setup"
 
-long_description = "A python package for operating multiple newport motors in an optical setup"
-    
 here = os.path.abspath(os.path.dirname(__file__))
+
+
 def read(*parts):
-    with codecs.open(os.path.join(here, *parts), 'r') as fp:
+    with codecs.open(os.path.join(here, *parts), "r") as fp:
         return fp.read()
 
+
 def find_version(*file_paths):
     version_file = read(*file_paths)
     version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
+
 # DEPENDENCIES
 # 1. What are the required dependencies?
-with open('requirements.txt') as f:
+with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 # 2. What dependencies required to run the unit tests? (i.e. `pytest --remote-data`)
 # tests_require = ['pytest', 'pytest-cov', 'pytest-remotedata']
 
 
 setuptools.setup(
     name="newport-motors-py",
     version=find_version("newport_motors", "__init__.py"),
     description="A python package for operating newport motors",
     long_description=long_description,
-    # long_description_content_type="text/markdown",
-    
+    long_description_content_type="text/markdown",
     author="Adam Taras",
     author_email="adam.taras@sydney.edu.au",
     url="https://github.com/ataras2/newport_motors",
-    
     project_urls={
         "Bug Tracker": "https://github.com/ataras2/newport_motors/issues",
     },
-    
     # package_dir={"": "src"},
-    packages=["newport_motors", 
-              "newport_motors/GUI", 
-              "newport_motors/Motors", 
-              "newport_motors/Mocks", 
-              "newport_motors/USBs"],
-    
+    packages=[
+        "newport_motors",
+        "newport_motors/GUI",
+        "newport_motors/Motors",
+        "newport_motors/Mocks",
+        "newport_motors/USBs",
+        "pyvisa_mock",
+    ],
     install_requires=install_requires,
-    
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-
     # packages = ["src"] + setuptools.find_namespace_packages(where = "src")
 )
```

### Comparing `newport-motors-py-0.0.1/tests/test_motor.py` & `newport-motors-py-0.1.0/tests/test_motor.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 
 class Test_M100D:
     def test_nothing(self):
         pass
 
     def test_ctor(self):
-        M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@-mock"))
+        M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@mock"))
 
     def test_move(self):
-        m = M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@-mock"))
+        m = M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@mock"))
         m.set_absolute_position(0.2, M100D.AXES.U)
 
         assert m.get_current_pos[0] == 0.2
 
     def test_read(self):
-        m = M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@-mock"))
+        m = M100D("MOCK0::mock1::INSTR", ResourceManager(visa_library="@mock"))
         p = m.read_pos(M100D.AXES.U)
 
         assert isinstance(p, float)
         assert p > -0.75 and p < 0.75
 
 
 class Test_LS16P:
     def test_nothing(self):
         pass
 
     def test_ctor(self):
-        LS16P("MOCK0::mock2::INSTR", ResourceManager(visa_library="@-mock"))
+        LS16P("MOCK0::mock2::INSTR", ResourceManager(visa_library="@mock"))
```

### Comparing `newport-motors-py-0.0.1/tests/test_motor_mock.py` & `newport-motors-py-0.1.0/tests/test_motor_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,41 @@
 
 from newport_motors.Mocks.motor import Mock_M100D, Mock_LS16P
 
 
 register_resource("MOCK0::mock1::INSTR", Mock_M100D())
 register_resource("MOCK0::mock2::INSTR", Mock_LS16P())
 
-rc = ResourceManager(visa_library="@-mock")
+rc = ResourceManager(visa_library="@mock")
 M100D_resource = rc.open_resource("MOCK0::mock1::INSTR")
 LS16P_resource = rc.open_resource("MOCK0::mock2::INSTR")
 
+
 class Test_Mock_M100D:
     def test_nothing(self):
         pass
 
     def test_id(self):
         id_str = M100D_resource.query("1ID?")
         assert "M100D" in id_str
 
-    def test_get_abs_pos(self):       
+    def test_get_abs_pos(self):
         # check that the return can be converted to a float
         reply = M100D_resource.query("1TPU")
         assert "1TPU" in reply
 
         float(reply[4:])
-        
+
+
 class Test_Mock_LS16P:
     def test_nothing(self):
         pass
 
     def test_id(self):
         id_str = LS16P_resource.query("1ID?")
         assert "LS16P" in id_str
 
-    def test_get_abs_pos(self):       
+    def test_get_abs_pos(self):
         # check that the return can be converted to a float
         reply = M100D_resource.query("1TP")
         assert "1TP" in reply
-        float(reply[4:])
+        float(reply[4:])
```

