# Comparing `tmp/huawei-solar-2.2.7b7.tar.gz` & `tmp/huawei-solar-2.2.7b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.2.7b7.tar", last modified: Tue Jun 20 09:56:04 2023, max compression
+gzip compressed data, was "huawei-solar-2.2.7b8.tar", last modified: Wed Jun 21 06:44:37 2023, max compression
```

## Comparing `huawei-solar-2.2.7b7.tar` & `huawei-solar-2.2.7b8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     7719 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.010492 huawei-solar-2.2.7b7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.016492 huawei-solar-2.2.7b7/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    24953 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    18080 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22487 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    42679 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.017492 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7719 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-06-20 09:56:04.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.018492 huawei-solar-2.2.7b7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-21 06:44:37.417512 huawei-solar-2.2.7b8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.408512 huawei-solar-2.2.7b8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.414512 huawei-solar-2.2.7b8/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    24956 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22487 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    42679 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.415512 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 06:44:37.000000 huawei-solar-2.2.7b8/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:44:37.416512 huawei-solar-2.2.7b8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)    16324 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-21 06:44:23.000000 huawei-solar-2.2.7b8/tox.ini
```

### Comparing `huawei-solar-2.2.7b7/.gitignore` & `huawei-solar-2.2.7b8/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/.gitlab-ci.yml` & `huawei-solar-2.2.7b8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/.pre-commit-config.yaml` & `huawei-solar-2.2.7b8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/LICENSE.md` & `huawei-solar-2.2.7b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/PKG-INFO` & `huawei-solar-2.2.7b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b7
+Version: 2.2.7b8
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.7b7/README.md` & `huawei-solar-2.2.7b8/README.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/bridge_tst.py` & `huawei-solar-2.2.7b8/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/pyproject.toml` & `huawei-solar-2.2.7b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/setup.cfg` & `huawei-solar-2.2.7b8/setup.cfg`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/__init__.py` & `huawei-solar-2.2.7b8/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/bridge.py` & `huawei-solar-2.2.7b8/src/huawei_solar/bridge.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/exceptions.py` & `huawei-solar-2.2.7b8/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/files.py` & `huawei-solar-2.2.7b8/src/huawei_solar/files.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/huawei_solar.py` & `huawei-solar-2.2.7b8/src/huawei_solar/huawei_solar.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
                 "Received %s: backing off reading for %0.1f seconds after %d tries",
                 sys.exc_info()[0],
                 details["wait"],
                 details["tries"],
             )
 
         def on_backoff_with_reconnect(details):
-            if details.tries % 2 == 0:
+            if details["tries"] % 3 == 0:
                 asyncio.create_task(self._reconnect())
                 LOGGER.debug(
                     "Received %s: reconnecting and backing off reading for %0.1f seconds after %d tries",
                     sys.exc_info()[0],
                     details["wait"],
                     details["tries"],
                 )
```

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/modbus.py` & `huawei-solar-2.2.7b8/src/huawei_solar/modbus.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/register_names.py` & `huawei-solar-2.2.7b8/src/huawei_solar/register_names.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/register_values.py` & `huawei-solar-2.2.7b8/src/huawei_solar/register_values.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar/registers.py` & `huawei-solar-2.2.7b8/src/huawei_solar/registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar.egg-info/PKG-INFO` & `huawei-solar-2.2.7b8/src/huawei_solar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b7
+Version: 2.2.7b8
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.7b7/src/huawei_solar.egg-info/SOURCES.txt` & `huawei-solar-2.2.7b8/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/test.py` & `huawei-solar-2.2.7b8/test.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/conftest.py` & `huawei-solar-2.2.7b8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/mock_huawei_solar.py` & `huawei-solar-2.2.7b8/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/test__registers__peak_periods.py` & `huawei-solar-2.2.7b8/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/test__registers__time_of_use.py` & `huawei-solar-2.2.7b8/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/test_huawei_solar.py` & `huawei-solar-2.2.7b8/tests/test_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tests/test_registers.py` & `huawei-solar-2.2.7b8/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b7/tox.ini` & `huawei-solar-2.2.7b8/tox.ini`

 * *Files identical despite different names*

