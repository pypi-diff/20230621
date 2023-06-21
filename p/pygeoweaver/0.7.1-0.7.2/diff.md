# Comparing `tmp/pygeoweaver-0.7.1.tar.gz` & `tmp/pygeoweaver-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.7.1.tar", last modified: Wed Jun 21 05:23:30 2023, max compression
+gzip compressed data, was "pygeoweaver-0.7.2.tar", last modified: Wed Jun 21 05:38:30 2023, max compression
```

## Comparing `pygeoweaver-0.7.1.tar` & `pygeoweaver-0.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/download_gw.bat
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/download_gw.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/java_bin.bat
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/java_bin.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/jdk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/start.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/stop.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 05:23:30.832518 pygeoweaver-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.229150 pygeoweaver-0.7.2/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/download_gw.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/download_gw.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/java_bin.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/java_bin.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/jdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/sc_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/start.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/stop.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.229150 pygeoweaver-0.7.2/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 05:38:30.000000 pygeoweaver-0.7.2/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:30.233150 pygeoweaver-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 05:38:19.000000 pygeoweaver-0.7.2/test/test_server.py
```

### Comparing `pygeoweaver-0.7.1/LICENSE` & `pygeoweaver-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/PKG-INFO` & `pygeoweaver-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.1
+Version: 0.7.2
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PyGeoWeaver
 
 ### Description
```

### Comparing `pygeoweaver-0.7.1/README.md` & `pygeoweaver-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/__main__.py` & `pygeoweaver-0.7.2/pygeoweaver/__main__.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/jdk_utils.py` & `pygeoweaver-0.7.2/pygeoweaver/jdk_utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_create.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import requests
 import pandas as pd
 from pydantic import BaseModel
 
-from . import constants
+from pygeoweaver.constants import *
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     get_geoweaver_jar_path,
     get_java_bin_path,
     get_root_dir,
     check_ipython,
 )
@@ -59,17 +59,17 @@
         name=name,
         code=code,
         owner=owner,
         confidential=confidential,
     )
     data_json = process.json()
     r = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/add/process",
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/add/process",
         data=data_json,
-        headers=constants.COMMON_API_HEADER,
+        headers=COMMON_API_HEADER,
     )
     if check_ipython() and r.ok:
         df = pd.DataFrame(json.loads(data_json).items(), columns=["Key", "Value"])
         return df
     else:
         return r.json()
 
@@ -129,15 +129,15 @@
         edges=edges,
         name=name,
         nodes=nodes,
         owner=owner,
     )
     data_json = workflow.json()
     r = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/add/workflow",
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/add/workflow",
         data=data_json,
-        headers=constants.COMMON_API_HEADER,
+        headers=COMMON_API_HEADER,
     )
     if check_ipython():
         return pd.DataFrame(json.loads(data_json).items(), columns=["Key", "Value"])
     else:
         return r.json()
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_detail.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_detail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Detail subcommand
 """
 
 import subprocess
 
 import requests
-from . import constants
+from pygeoweaver.constants import *
 
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     get_geoweaver_jar_path,
     get_java_bin_path,
     get_root_dir,
 )
@@ -61,11 +61,11 @@
         ],
         cwd=f"{get_root_dir()}/",
     )
 
 
 def get_process_code(process_id):
     r = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
         data={"type": "process", "id": process_id},
     ).json()
     return r["code"]
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_export.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_find.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_find.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
-from . import constants
+from pygeoweaver.constants import *
 import pandas as pd
 
 
 def get_process_by_name(process_name):
     response = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
     )
     process_list = response.json()
 
     matching_processes = []
 
     for process in process_list:
         if process["name"] == process_name:
@@ -18,15 +18,15 @@
     pd.set_option("display.max_rows", None)  # Display all rows
     pd.set_option("display.expand_frame_repr", False)  # Prevent truncation of columns
     pd.DataFrame(matching_processes)
 
 
 def get_process_by_id(process_id):
     response = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
     )
     process_list = response.json()
 
     matching_processes = []
 
     for process in process_list:
         if process["id"] == process_id:
@@ -35,15 +35,15 @@
     pd.set_option("display.max_rows", None)  # Display all rows
     pd.set_option("display.expand_frame_repr", False)  # Prevent truncation of columns
     pd.DataFrame(matching_processes)
 
 
 def get_process_by_language(language):
     response = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/list", data={"type": "process"}
     )
     process_list = response.json()
 
     matching_processes = []
 
     for process in process_list:
         if process["lang"] == language:
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_help.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_history.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 
 import pandas as pd
 import requests
 
-from . import constants
+from pygeoweaver.constants import *
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     get_geoweaver_jar_path,
     get_java_bin_path,
     get_root_dir,
 )
 
@@ -31,15 +31,15 @@
     :param process_id: str    :type process_id: str
     """
     if not process_id:
         raise Exception("please pass `process_id` as a parameter to the function.")
     download_geoweaver_jar()
     try:
         r = requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/logs",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/logs",
             data={"type": "process", "id": process_id},
         ).json()
         df = pd.DataFrame(r)
         df["history_begin_time"] = pd.to_datetime(df["history_begin_time"], unit="ms")
         df["history_end_time"] = pd.to_datetime(df["history_end_time"], unit="ms")
         return df
     except Exception as e:
@@ -55,15 +55,15 @@
         Get list of history for a workflow using workflow id
     :param workflow_id: str
     """
     if not workflow_id:
         raise Exception("please pass `workflow_id` as a parameter to the function.")
     try:
         r = requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/logs",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/logs",
             data={"type": "workflow", "id": workflow_id},
         ).json()
         df = pd.DataFrame(r)
         df["history_begin_time"] = pd.to_datetime(df["history_begin_time"], unit="ms")
         df["history_end_time"] = pd.to_datetime(df["history_end_time"], unit="ms")
         return df
     except Exception as e:
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_import.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_list.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 import subprocess
-from . import constants
+from pygeoweaver.constants import *
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     get_geoweaver_jar_path,
     get_java_bin_path,
     get_root_dir,
     check_ipython,
 )
@@ -30,15 +30,15 @@
     )
 
 
 def list_processes_in_workflow(workflow_id):
     download_geoweaver_jar()
     payload = {"id": workflow_id, "type": "workflow"}
     r = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail", data=payload
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail", data=payload
     )
     nodes = json.loads(r.json()["nodes"])
     result = [
         {"title": item["title"], "id": item["id"].split(".")[0]} for item in nodes
     ]
 
     if check_ipython():
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_resetpassword.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_resetpassword.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_run.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     get_geoweaver_jar_path,
     get_java_bin_path,
     get_root_dir,
 )
-from . import constants
+from pygeoweaver.constants import *
 
 
 def run_process(
     *,
     process_id: str,
     host_id: str,
     password: str = None,
@@ -38,20 +38,20 @@
         if not os.path.exists(sync_path):
             print("The specified path does nto exists")
         print("Updating code on workflow with the given file path.\n")
         f = open(sync_path, "r")
         context = f.read()
         f.close()
         details = requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
             data={"type": "process", "id": process_id},
         ).json()
         details["code"] = context
         requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/edit/process",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/edit/process",
             data=json.dumps(details),
             headers={"Content-Type": "application/json"},
         )
 
     download_geoweaver_jar()
     subprocess.run(
         [
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/sc_sync.py` & `pygeoweaver-0.7.2/pygeoweaver/sc_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import json
 import zipfile
 
 import requests
 import typing
 
-from . import constants
+from pygeoweaver.constants import *
 from pygeoweaver.utils import (
     download_geoweaver_jar,
     copy_files,
 )
 
 
 def sync(process_id: str, local_path: typing.Union[str, os.PathLike], direction: str):
     print(f"Proceeding with {direction}\n")
     if direction == "download":
         if not local_path:
             raise Exception("Sync path not found.")
         r = requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
             data={"type": "process", "id": process_id},
         ).json()
         code = r["code"]
         decoded_string = code
         file_name = r["name"]
         ext = None
         if r["lang"] == "python":
@@ -36,36 +36,36 @@
         with open(os.path.join(local_path, file_name + ext), "w") as file:
             file.write(decoded_string)
         print(f"Wrote file {file_name + ext} to {local_path}")
     elif direction == "upload":
         if not local_path:
             raise Exception("Sync path not found.")
         process_prev_state = requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
             data={"type": "process", "id": process_id},
         ).json()
         with open(local_path, "r") as f:
             f_content = f.read()
             process_prev_state["code"] = f_content
         requests.post(
-            f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/edit/process",
+            f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/edit/process",
             data=json.dumps(process_prev_state),
             headers={"Content-Type": "application/json"},
         )
     else:
         raise Exception(
             "Please specify the direction to sync. Choices - [UPLOAD, DOWNLOAD]"
         )
 
 
 def sync_workflow(workflow_id: str, sync_to_path: typing.Union[str, os.PathLike]):
     download_geoweaver_jar()
     # download workflow
     r = requests.post(
-        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/downloadworkflow",
+        f"{GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/downloadworkflow",
         data={"id": workflow_id, "option": "workflowwithprocesscodeallhistory"},
     ).text
     filename = r.rsplit("/")[-1]
     home_dir = os.path.expanduser("~")
     tmp_dir = os.path.join(home_dir, "tmp")
     if not os.path.exists(tmp_dir):
         os.makedirs(tmp_dir)
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver/server.py` & `pygeoweaver-0.7.2/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/start.bat` & `pygeoweaver-0.7.2/pygeoweaver/start.bat`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/start.sh` & `pygeoweaver-0.7.2/pygeoweaver/start.sh`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver/utils.py` & `pygeoweaver-0.7.2/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.7.2/pygeoweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.7.1
+Version: 0.7.2
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PyGeoWeaver
 
 ### Description
```

### Comparing `pygeoweaver-0.7.1/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.7.2/pygeoweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/pyproject.toml` & `pygeoweaver-0.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.7,<4"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.7.1"
+version = "0.7.2"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.7,<4"
 setuptools = ">=61.0"
 requests = "2.28.2"
 pydantic = "1.10.9"
 
 [tool.poetry.scripts]
 
 [tool.pytest.ini_options]
```

### Comparing `pygeoweaver-0.7.1/test/test_detail.py` & `pygeoweaver-0.7.2/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.7.1/test/test_server.py` & `pygeoweaver-0.7.2/test/test_server.py`

 * *Files identical despite different names*

