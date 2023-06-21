# Comparing `tmp/pygeoweaver-0.6.9.tar.gz` & `tmp/pygeoweaver-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.9.tar", last modified: Sun Jun  4 16:14:15 2023, max compression
+gzip compressed data, was "pygeoweaver-0.7.1.tar", last modified: Wed Jun 21 05:23:30 2023, max compression
```

## Comparing `pygeoweaver-0.6.9.tar` & `pygeoweaver-0.7.1.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.484549 pygeoweaver-0.6.9/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/download_gw.bat
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/download_gw.sh
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/start.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/stop.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 16:14:15.000000 pygeoweaver-0.6.9/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:15.488549 pygeoweaver-0.6.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-04 16:14:05.000000 pygeoweaver-0.6.9/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/download_gw.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/download_gw.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/java_bin.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/java_bin.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/jdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/sc_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/start.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/stop.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 05:23:30.000000 pygeoweaver-0.7.1/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 05:23:30.832518 pygeoweaver-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:30.828518 pygeoweaver-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-21 05:23:18.000000 pygeoweaver-0.7.1/test/test_server.py
```

### Comparing `pygeoweaver-0.6.9/LICENSE` & `pygeoweaver-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.9/PKG-INFO` & `pygeoweaver-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.9
+Version: 0.7.1
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.9/README.md` & `pygeoweaver-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.9/pygeoweaver/__main__.py` & `pygeoweaver-0.7.1/pygeoweaver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 """
 The main function of pygeoweaver
 To run in CLI mode. 
 """
-from pygeoweaver import detail_host, detail_process, detail_workflow, export_workflow, \
-    show_history, import_workflow, list_hosts, list_processes, list_workflows, \
-    start, stop, reset_password, run_process, run_worklfow, helpwith
+from pygeoweaver import (
+    detail_host,
+    detail_process,
+    detail_workflow,
+    export_workflow,
+    show_history,
+    import_workflow,
+    list_hosts,
+    list_processes,
+    list_workflows,
+    start,
+    stop,
+    reset_password,
+    run_process,
+    run_workflow,
+    helpwith,
+)
 from pygeoweaver.server import show
-from pygeoweaver.utils import check_java
 
 
 def main():
     # start geoweaver
     # start()
     # stop geoweaver
     # stop()
     # list resources
-    #list_hosts()
-    #list_processes()
+    # list_hosts()
+    # list_processes()
     # list_workflows()
     # show history
-    #show_history("ll3u3W78eOEfklxhBJ")
+    # show_history("ll3u3W78eOEfklxhBJ")
     # detail host
     # detail_host("100001")
     # detail process
     # detail_process("7pxu8c")
-    #detail_workflow("5jnhcrq33znbu2mue9v2")
+    # detail_workflow("5jnhcrq33znbu2mue9v2")
     # import workflow
-    #import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
+    # import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
     # export workflow
     # export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
     # run process
-    # run_process(process_id="7zwnvx", host_id="100001", password="xxx", environment="",)
+    # run_process(process_id="7zwnvx", host_id="100001", )
     # run workflow by id
-    # run_worklfow(workflow_id="9sszomwhiiusakodb1ft", host_list="100001", password_list="xxx", 
+    # run_worklfow(workflow_id="9sszomwhiiusakodb1ft", host_list="100001", password_list="xxx",
     #              environment_list="",)
+    # run_workflow(workflow_id="9sszomwhiiusakodb1ft", host_list="100001", )
     # run workflow by zip path
 
     # run workflow by folder path
 
     # reset localhost password for Geoweaver
     # reset_password()
-    show()
+    # show()
     # helpwith()
     # check_java()
+    pass
 
 
 if __name__ == "__main__":
-     main()
+    main()
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver/sc_detail.py` & `pygeoweaver-0.7.1/pygeoweaver/sc_detail.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,71 @@
 """
 Detail subcommand
 """
 
 import subprocess
-from pygeoweaver.utils import download_geoweaver_jar, get_geoweaver_jar_path, get_root_dir
+
+import requests
+from . import constants
+
+from pygeoweaver.utils import (
+    download_geoweaver_jar,
+    get_geoweaver_jar_path,
+    get_java_bin_path,
+    get_root_dir,
+)
 
 
 def detail_workflow(workflow_id):
     if not workflow_id:
         raise RuntimeError("Workflow id is missing")
     download_geoweaver_jar()
-    subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "detail", f"--workflow-id={workflow_id}"], 
-                   cwd=f"{get_root_dir()}/")
+    subprocess.run(
+        [
+            get_java_bin_path(),
+            "-jar",
+            get_geoweaver_jar_path(),
+            "detail",
+            f"--workflow-id={workflow_id}",
+        ],
+        cwd=f"{get_root_dir()}/",
+    )
 
 
 def detail_process(process_id):
     if not process_id:
         raise RuntimeError("Process id is missing")
     download_geoweaver_jar()
-    subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "detail", f"--process-id={process_id}"], 
-                   cwd=f"{get_root_dir()}/")
+    subprocess.run(
+        [
+            get_java_bin_path(),
+            "-jar",
+            get_geoweaver_jar_path(),
+            "detail",
+            f"--process-id={process_id}",
+        ],
+        cwd=f"{get_root_dir()}/",
+    )
+
 
 def detail_host(host_id):
     if not host_id:
         raise RuntimeError("Host id is missing")
     download_geoweaver_jar()
-    subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "detail", f"--host-id={host_id}"], 
-                   cwd=f"{get_root_dir()}/")
+    subprocess.run(
+        [
+            get_java_bin_path(),
+            "-jar",
+            get_geoweaver_jar_path(),
+            "detail",
+            f"--host-id={host_id}",
+        ],
+        cwd=f"{get_root_dir()}/",
+    )
+
+
+def get_process_code(process_id):
+    r = requests.post(
+        f"{constants.GEOWEAVER_DEFAULT_ENDPOINT_URL}/web/detail",
+        data={"type": "process", "id": process_id},
+    ).json()
+    return r["code"]
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver/sc_import.py` & `pygeoweaver-0.7.1/pygeoweaver/sc_import.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 import subprocess
-from pygeoweaver.utils import download_geoweaver_jar, get_geoweaver_jar_path, get_root_dir
+from pygeoweaver.utils import (
+    download_geoweaver_jar,
+    get_geoweaver_jar_path,
+    get_java_bin_path,
+    get_root_dir,
+)
 
 
 def import_workflow(workflow_zip_file_path):
-  """
-  Usage: <main class> import workflow <workflow_zip_file_path>
-  import a workflow from file
-        <workflow_zip_file_path>
-          Geoweaver workflow zip file path
-  """
-  if not workflow_zip_file_path:
+    """
+    Usage: <main class> import workflow <workflow_zip_file_path>
+    import a workflow from file
+          <workflow_zip_file_path>
+            Geoweaver workflow zip file path
+    """
+    if not workflow_zip_file_path:
         raise RuntimeError("Workflow zip file path is missing")
-  download_geoweaver_jar()
-  subprocess.run(["java", "-jar", get_geoweaver_jar_path(), "import", 
-                  "workflow", workflow_zip_file_path], cwd=f"{get_root_dir()}/")
+    download_geoweaver_jar()
+    subprocess.run(
+        [
+            get_java_bin_path(),
+            "-jar",
+            get_geoweaver_jar_path(),
+            "import",
+            "workflow",
+            workflow_zip_file_path,
+        ],
+        cwd=f"{get_root_dir()}/",
+    )
 
+def import_workflow_from_github(git_repo_url):
+    pass
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver/server.py` & `pygeoweaver-0.7.1/pygeoweaver/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 import os
+import socket
 import subprocess
 import webbrowser
 from pygeoweaver.constants import GEOWEAVER_DEFAULT_ENDPOINT_URL
-from pygeoweaver.utils import check_ipython, check_os, download_geoweaver_jar, get_logger, get_module_absolute_path, \
-    get_root_dir
+from pygeoweaver.jdk_utils import check_java
+from pygeoweaver.utils import (
+    check_ipython,
+    check_os,
+    download_geoweaver_jar,
+    get_logger,
+    get_module_absolute_path,
+    get_root_dir,
+)
 
 """
 This module provides function to start and stop Geoweaver server.
 If it detects the current environment is Jupyter notebook, it will 
 open Geoweaver GUI in the output cell (if gui is not disabld.)
 
 """
 
 logger = get_logger(__name__)
 
 
 def start(force=False):
     download_geoweaver_jar(overwrite=force)
+    check_java()
+
     if check_os() == 3:
-        subprocess.run([f'{get_module_absolute_path()}/start.bat'], cwd=f"{get_root_dir()}/")
+        subprocess.run(
+            [f"{get_module_absolute_path()}/start.bat"], cwd=f"{get_root_dir()}/"
+        )
     else:
-        subprocess.run([f'{get_module_absolute_path()}/start.sh'], cwd=f"{get_root_dir()}/")
+        subprocess.run(
+            [f"{get_module_absolute_path()}/start.sh"], cwd=f"{get_root_dir()}/"
+        )
 
 
 def stop():
+    check_java()
     if check_os() == 3:
-        subprocess.run([f'{get_module_absolute_path()}/stop.bat'], cwd=f"{get_root_dir()}/", shell=True)
+        subprocess.run(
+            [f"{get_module_absolute_path()}/stop.bat"],
+            cwd=f"{get_root_dir()}/",
+            shell=True,
+        )
     else:
-        subprocess.run([f'{get_module_absolute_path()}/stop.sh'], cwd=f"{get_root_dir()}/", shell=True)
+        subprocess.run(
+            [f"{get_module_absolute_path()}/stop.sh"],
+            cwd=f"{get_root_dir()}/",
+            shell=True,
+        )
 
 
 def show(geoweaver_url=GEOWEAVER_DEFAULT_ENDPOINT_URL):
     download_geoweaver_jar()  # check if geoweaver is initialized
+    check_java()
     if check_ipython():
         logger.info("enter ipython block")
         from IPython.display import IFrame
-        return IFrame(src=geoweaver_url, width='100%', height='500px')
+
+        logger.warning("This only works when the Jupyter is visited from localhost!")
+        return IFrame(src=geoweaver_url, width="100%", height="500px")
     else:
         logger.info("enter self opening block")
         webbrowser.open(geoweaver_url)
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver/start.bat` & `pygeoweaver-0.7.1/pygeoweaver/start.bat`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.9/pygeoweaver/start.sh` & `pygeoweaver-0.7.1/pygeoweaver/start.sh`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 
 echo "Stop running Geoweaver if any.."
-pkill -f geoweaver
+pkill -f geoweaver.jar
 
 echo "Check Java.."
-
+touch ~/.bashrc && source ~/.bashrc
 
 echo "Start Geoweaver.."
 nohup java -jar ~/geoweaver.jar > ~/geoweaver.log &
 
 STATUS=0
 counter=0
 until [ $STATUS == 302 ] || [ $counter == 20 ]
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.7.1/pygeoweaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.9
+Version: 0.7.1
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.9/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.7.1/pygeoweaver.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 pyproject.toml
 setup.cfg
 pygeoweaver/__init__.py
 pygeoweaver/__main__.py
 pygeoweaver/constants.py
 pygeoweaver/download_gw.bat
 pygeoweaver/download_gw.sh
+pygeoweaver/java_bin.bat
+pygeoweaver/java_bin.sh
+pygeoweaver/jdk_utils.py
+pygeoweaver/sc_create.py
 pygeoweaver/sc_detail.py
 pygeoweaver/sc_export.py
+pygeoweaver/sc_find.py
 pygeoweaver/sc_help.py
 pygeoweaver/sc_history.py
 pygeoweaver/sc_import.py
 pygeoweaver/sc_interface.py
 pygeoweaver/sc_list.py
 pygeoweaver/sc_resetpassword.py
 pygeoweaver/sc_run.py
+pygeoweaver/sc_sync.py
 pygeoweaver/server.py
 pygeoweaver/start.bat
 pygeoweaver/start.sh
 pygeoweaver/stop.bat
 pygeoweaver/stop.sh
 pygeoweaver/utils.py
 pygeoweaver.egg-info/PKG-INFO
```

### Comparing `pygeoweaver-0.6.9/pyproject.toml` & `pygeoweaver-0.7.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.9"
+version = "0.7.1"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,22 +18,23 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.9"
+version = "0.7.1"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 setuptools = ">=61.0"
 requests = "2.28.2"
+pydantic = "1.10.9"
 
 [tool.poetry.scripts]
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings --cov=pygeoweaver --cov-report=html"
```

### Comparing `pygeoweaver-0.6.9/test/test_detail.py` & `pygeoweaver-0.7.1/test/test_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-
-
 from io import StringIO
 import sys
 import unittest
 from pygeoweaver.sc_detail import detail_host, detail_process, detail_workflow
 from pygeoweaver.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
 def test_detail_process(capfd):
     detail_process("not_existing_id")
     output, err = capfd.readouterr()
-    logger.debug("stdout_output"+output)
+    logger.debug("stdout_output" + output)
     assert "No process found with id: not_existing_id" in output
 
 
 def test_detail_workflow(capfd):
     detail_workflow("not_existing_id")
     output, err = capfd.readouterr()
-    logger.debug("stdout_output"+output)
+    logger.debug("stdout_output" + output)
     assert "No workflow found with id: not_existing_id" in output
 
 
 def test_detail_host(capfd):
     detail_host("not_existing_id")
     output, err = capfd.readouterr()
-    logger.debug("stdout_output"+output)
+    logger.debug("stdout_output" + output)
     assert "No host found with id: not_existing_id" in output
-
```

### Comparing `pygeoweaver-0.6.9/test/test_server.py` & `pygeoweaver-0.7.1/test/test_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,41 +13,43 @@
 from pygeoweaver.server import show
 from pygeoweaver.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
-
 class TestServer(unittest.TestCase):
-
     def test_server_start_stop(self):
         start()
         response = requests.get(GEOWEAVER_DEFAULT_ENDPOINT_URL)
-        self.assertEqual(response.status_code, 200, f"Failed to access URL: {GEOWEAVER_DEFAULT_ENDPOINT_URL}")
+        self.assertEqual(
+            response.status_code,
+            200,
+            f"Failed to access URL: {GEOWEAVER_DEFAULT_ENDPOINT_URL}",
+        )
         stop()
         with self.assertRaises(requests.exceptions.ConnectionError):
             response = requests.get(GEOWEAVER_DEFAULT_ENDPOINT_URL)
 
-        stop() # stop again should have no issue
-
+        stop()  # stop again should have no issue
 
     def test_windows(self):
-        with patch('pygeoweaver.server.checkOS') as mock_checkos:
+        with patch("pygeoweaver.server.checkOS") as mock_checkos:
             mock_checkos.return_value = 3
             with self.assertRaises(RuntimeError):
                 start()
             with self.assertRaises(RuntimeError):
                 stop()
 
     def test_show_gui(self):
-        with patch('pygeoweaver.webbrowser.open') as mock_browser_open:
+        with patch("pygeoweaver.webbrowser.open") as mock_browser_open:
             show()
             mock_browser_open.assert_called_once()
 
-            with patch('pygeoweaver.server.checkIPython') as mock_checkipython:
+            with patch("pygeoweaver.server.checkIPython") as mock_checkipython:
                 mock_checkipython.return_value = True
                 show()
                 mock_browser_open.assert_called_once()
 
+
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

