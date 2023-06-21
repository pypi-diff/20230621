# Comparing `tmp/cvat-cli-2.4.6.tar.gz` & `tmp/cvat-cli-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.4.6.tar", last modified: Wed Jun 14 19:57:32 2023, max compression
+gzip compressed data, was "cvat-cli-2.4.7.tar", last modified: Wed Jun 21 13:51:10 2023, max compression
```

## Comparing `cvat-cli-2.4.6.tar` & `cvat-cli-2.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/README.md
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-04-14 14:12:32.000000 cvat-cli-2.4.6/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/cvat_cli/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/src/cvat_cli/__init__.py
--rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2151 2022-11-18 08:29:30.000000 cvat-cli-2.4.6/src/cvat_cli/__main__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-04-05 10:02:25.000000 cvat-cli-2.4.6/src/cvat_cli/cli.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-04-05 10:02:25.000000 cvat-cli-2.4.6/src/cvat_cli/parser.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:53:41.000000 cvat-cli-2.4.6/src/cvat_cli/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:57:32.167224 cvat-cli-2.4.6/src/cvat_cli.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/entry_points.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:57:32.000000 cvat-cli-2.4.6/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/README.md
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-04-14 14:12:32.000000 cvat-cli-2.4.7/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.643545 cvat-cli-2.4.7/src/
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/src/cvat_cli/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2229 2023-06-17 07:46:59.000000 cvat-cli-2.4.7/src/cvat_cli/__main__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-04-05 10:02:25.000000 cvat-cli-2.4.7/src/cvat_cli/cli.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13469 2023-06-17 07:46:59.000000 cvat-cli-2.4.7/src/cvat_cli/parser.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-21 13:40:56.000000 cvat-cli-2.4.7/src/cvat_cli/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/src/cvat_cli.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.4.6/PKG-INFO` & `cvat-cli-2.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.6
+Version: 2.4.7
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cvat-cli-2.4.6/README.md` & `cvat-cli-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.6/setup.py` & `cvat-cli-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.6/src/cvat_cli/__main__.py` & `cvat-cli-2.4.7/src/cvat_cli/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,21 +33,25 @@
 def build_client(parsed_args: SimpleNamespace, logger: logging.Logger) -> Client:
     config = Config(verify_ssl=not parsed_args.insecure)
 
     url = parsed_args.server_host
     if parsed_args.server_port:
         url += f":{parsed_args.server_port}"
 
-    return Client(
+    client = Client(
         url=url,
         logger=logger,
         config=config,
         check_server_version=False,  # version is checked after auth to support versions < 2.3
     )
 
+    client.organization_slug = parsed_args.organization
+
+    return client
+
 
 def main(args: List[str] = None):
     actions = {
         "create": CLI.tasks_create,
         "delete": CLI.tasks_delete,
         "ls": CLI.tasks_list,
         "frames": CLI.tasks_frames,
```

### Comparing `cvat-cli-2.4.6/src/cvat_cli/cli.py` & `cvat-cli-2.4.7/src/cvat_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.6/src/cvat_cli/parser.py` & `cvat-cli-2.4.7/src/cvat_cli/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,23 @@
     parser.add_argument(
         "--server-port",
         type=int,
         default=None,
         help="port (default: 80 for http and 443 for https connections)",
     )
     parser.add_argument(
+        "--organization",
+        "--org",
+        metavar="SLUG",
+        help="""short name (slug) of the organization
+                to use when listing or creating resources;
+                set to blank string to use the personal workspace
+                (default: list all accessible objects, create in personal workspace)""",
+    )
+    parser.add_argument(
         "--debug",
         action="store_const",
         dest="loglevel",
         const=logging.DEBUG,
         default=logging.INFO,
         help="show debug output",
     )
```

### Comparing `cvat-cli-2.4.6/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.4.7/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.6
+Version: 2.4.7
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

