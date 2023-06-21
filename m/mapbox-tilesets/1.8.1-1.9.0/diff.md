# Comparing `tmp/mapbox-tilesets-1.8.1.tar.gz` & `tmp/mapbox-tilesets-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mapbox-tilesets-1.8.1.tar", last modified: Mon Aug 29 19:42:11 2022, max compression
+gzip compressed data, was "dist/mapbox-tilesets-1.9.0.tar", last modified: Wed Jun 21 21:26:50 2023, max compression
```

## Comparing `mapbox-tilesets-1.8.1.tar` & `mapbox-tilesets-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    14658 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    14299 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      767 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/scripts/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    26880 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/scripts/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6048 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/mapbox_tilesets/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14658 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-08-29 19:42:11.000000 mapbox-tilesets-1.8.1/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1595 2022-08-29 19:41:05.000000 mapbox-tilesets-1.8.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15036 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      767 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    29264 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6046 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/mapbox_tilesets/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15395 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      924 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1594 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 21:26:50.000000 mapbox-tilesets-1.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3045 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_activity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5265 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_create.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_delete.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6170 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_estimate_area.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4178 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8142 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2052 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_publish.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11664 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_sources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_tilejson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_update.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2506 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_update_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_validate_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_cli_view_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      826 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_file_validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2023-06-21 21:25:23.000000 mapbox-tilesets-1.9.0/tests/test_version_documentation.py
```

### Comparing `mapbox-tilesets-1.8.1/LICENSE.md` & `mapbox-tilesets-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.8.1/PKG-INFO` & `mapbox-tilesets-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mapbox-tilesets
-Version: 1.8.1
-Summary: CLI for interacting with and preparing data for the Tilesets API
-Home-page: https://github.com/mapbox/tilesets-cli
-Author: Mapbox
-Author-email: sam@mapbox.com
-License: BSD-2
-Description-Content-Type: text/markdown
-Provides-Extra: estimate-area
-Provides-Extra: test
-License-File: LICENSE.md
-
 # tilesets-cli
 
 [![Build Status](https://travis-ci.com/mapbox/tilesets-cli.svg?token=wqR3RcWUEprcQ1ttsgiP&branch=master)](https://travis-ci.com/mapbox/tilesets-cli) [![codecov](https://codecov.io/gh/mapbox/tilesets-cli/branch/master/graph/badge.svg?token=YBTKyc2o3j)](https://codecov.io/gh/mapbox/tilesets-cli)
 
 CLI for interacting with and preparing data for the [Mapbox Tiling Service](https://docs.mapbox.com/mapbox-tiling-service/overview/).
 
 📚 If you have a question that isn't answered here, please refer to the complete [Mapbox Tiling Service documentation](https://docs.mapbox.com/mapbox-tiling-service/overview/).
@@ -90,14 +77,16 @@
   * [`update`](#update)
   * [`delete`](#delete)
   * [`status`](#status)
   * [`job`](#job)
   * [`jobs`](#jobs)
   * [`list`](#list)
   * [`tilejson`](#tilejson)
+* Activity
+  * [`list-activity`](#list-activity)
 
 ### upload-source
 
 ```shell
 tilesets upload-source <username> <source_id> <file>
 ```
 
@@ -410,7 +399,23 @@
 ```
 tilesets tilejson <tileset_id>
 ```
 
 Flags:
 
 * `--secure`: By default, resource URLs in the retrieved TileJSON (such as in the "tiles" array) will use the HTTP scheme. Include this query parameter in your request to receive HTTPS resource URLs instead.
+
+### list-activity
+
+Lists total request counts for a user's tilesets in the past 30 days. Returns a pagination key `next` if there are more results than the return limit that can be passed into another command as the `start` argument.
+
+```shell
+tilesets list-activity <account>
+```
+
+Flags:
+
+* `--sortby [requests|modified]` [optional]: Sorting key (default: requests)
+* `--orderby [asc|desc]` [optional]: Ordering key (default: desc)
+* `--limit [1-500]` [optional]: The maximum number of results to return (default: 100)
+* `--indent` [optional]: Indent size for JSON output.
+* `--start` [optional]: Pagination key from the `next` value in a response that has more results than the limit.
```

### Comparing `mapbox-tilesets-1.8.1/README.md` & `mapbox-tilesets-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: mapbox-tilesets
+Version: 1.9.0
+Summary: CLI for interacting with and preparing data for the Tilesets API
+Home-page: https://github.com/mapbox/tilesets-cli
+Author: Mapbox
+Author-email: sam@mapbox.com
+License: BSD-2
+Description-Content-Type: text/markdown
+Provides-Extra: estimate-area
+Provides-Extra: test
+License-File: LICENSE.md
+
 # tilesets-cli
 
 [![Build Status](https://travis-ci.com/mapbox/tilesets-cli.svg?token=wqR3RcWUEprcQ1ttsgiP&branch=master)](https://travis-ci.com/mapbox/tilesets-cli) [![codecov](https://codecov.io/gh/mapbox/tilesets-cli/branch/master/graph/badge.svg?token=YBTKyc2o3j)](https://codecov.io/gh/mapbox/tilesets-cli)
 
 CLI for interacting with and preparing data for the [Mapbox Tiling Service](https://docs.mapbox.com/mapbox-tiling-service/overview/).
 
 📚 If you have a question that isn't answered here, please refer to the complete [Mapbox Tiling Service documentation](https://docs.mapbox.com/mapbox-tiling-service/overview/).
@@ -77,14 +90,16 @@
   * [`update`](#update)
   * [`delete`](#delete)
   * [`status`](#status)
   * [`job`](#job)
   * [`jobs`](#jobs)
   * [`list`](#list)
   * [`tilejson`](#tilejson)
+* Activity
+  * [`list-activity`](#list-activity)
 
 ### upload-source
 
 ```shell
 tilesets upload-source <username> <source_id> <file>
 ```
 
@@ -397,7 +412,23 @@
 ```
 tilesets tilejson <tileset_id>
 ```
 
 Flags:
 
 * `--secure`: By default, resource URLs in the retrieved TileJSON (such as in the "tiles" array) will use the HTTP scheme. Include this query parameter in your request to receive HTTPS resource URLs instead.
+
+### list-activity
+
+Lists total request counts for a user's tilesets in the past 30 days. Returns a pagination key `next` if there are more results than the return limit that can be passed into another command as the `start` argument.
+
+```shell
+tilesets list-activity <account>
+```
+
+Flags:
+
+* `--sortby [requests|modified]` [optional]: Sorting key (default: requests)
+* `--orderby [asc|desc]` [optional]: Ordering key (default: desc)
+* `--limit [1-500]` [optional]: The maximum number of results to return (default: 100)
+* `--indent` [optional]: Indent size for JSON output.
+* `--start` [optional]: Pagination key from the `next` value in a response that has more results than the limit.
```

### Comparing `mapbox-tilesets-1.8.1/mapbox_tilesets/errors.py` & `mapbox-tilesets-1.9.0/mapbox_tilesets/errors.py`

 * *Files identical despite different names*

### Comparing `mapbox-tilesets-1.8.1/mapbox_tilesets/scripts/cli.py` & `mapbox-tilesets-1.9.0/mapbox_tilesets/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tilesets command line interface"""
 import builtins
 import json
 import tempfile
+from urllib.parse import urlencode, urlparse, parse_qs
 
 import click
 import cligj
 import base64
 import re
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
@@ -795,7 +796,84 @@
             {
                 "km2": area,
                 "precision": precision,
                 "pricing_docs": "For more information, visit https://www.mapbox.com/pricing/#tilesets",
             }
         )
     )
+
+
+@cli.command("list-activity")
+@click.argument("username", required=True, type=str)
+@click.option(
+    "--sortby",
+    required=False,
+    type=click.Choice(["requests", "modified"]),
+    default="requests",
+    help="Sort the results by request count or modified timestamps (default: 'requests')",
+)
+@click.option(
+    "--orderby",
+    required=False,
+    type=click.Choice(["asc", "desc"]),
+    default="desc",
+    help="Order results by asc or desc for the sort key (default: 'desc')",
+)
+@click.option(
+    "--limit",
+    required=False,
+    type=click.IntRange(1, 500),
+    default=100,
+    help="The maximum number of results to return, from 1 to 500 (default: 100)",
+)
+@click.option(
+    "--start",
+    required=False,
+    type=str,
+    help="Pagination key from the `next` value in a response that has more results than the limit.",
+)
+@click.option("--token", "-t", required=False, type=str, help="Mapbox access token")
+@click.option("--indent", type=int, default=None, help="Indent for JSON output")
+def list_activity(
+    username,
+    sortby=None,
+    orderby=None,
+    limit=None,
+    start=None,
+    token=None,
+    indent=None,
+):
+    """List tileset activity for an account. The response is an ordered array of data about the user's tilesets and their
+    total requests over the past 30 days. The sorting and ordering can be configured through cli arguments, defaulting to
+    descending request counts.
+
+    tilesets list-activity <username>
+    """
+    mapbox_api = utils._get_api()
+    mapbox_token = utils._get_token(token)
+    s = utils._get_session()
+
+    params = {
+        "access_token": mapbox_token,
+        "sortby": sortby,
+        "orderby": orderby,
+        "limit": limit,
+        "start": start,
+    }
+    params = {k: v for k, v in params.items() if v}
+    query_string = urlencode(params)
+    url = f"{mapbox_api}/activity/v1/{username}/tilesets?{query_string}"
+
+    r = s.get(url)
+    if r.status_code == 200:
+        if r.headers.get("Link"):
+            url = re.findall(r"<(.*)>;", r.headers.get("Link"))[0]
+            query = urlparse(url).query
+            start = parse_qs(query)["start"][0]
+
+        result = {
+            "data": r.json(),
+            "next": start,
+        }
+        click.echo(json.dumps(result, indent=indent))
+    else:
+        raise errors.TilesetsError(r.text)
```

### Comparing `mapbox-tilesets-1.8.1/mapbox_tilesets/utils.py` & `mapbox-tilesets-1.9.0/mapbox_tilesets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import json
 
 
 def load_module(modulename):
     """Dynamically imports a module and throws a readable exception if not found"""
     try:
         module = importlib.import_module(modulename)
-    except (ImportError):
+    except ImportError:
         raise ValueError(
             f"Couldn't find {modulename}. Check installation steps in the readme for help: https://github.com/mapbox/tilesets-cli/blob/master/README.md"
         ) from None
 
     return module
```

### Comparing `mapbox-tilesets-1.8.1/mapbox_tilesets.egg-info/PKG-INFO` & `mapbox-tilesets-1.9.0/mapbox_tilesets.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapbox-tilesets
-Version: 1.8.1
+Version: 1.9.0
 Summary: CLI for interacting with and preparing data for the Tilesets API
 Home-page: https://github.com/mapbox/tilesets-cli
 Author: Mapbox
 Author-email: sam@mapbox.com
 License: BSD-2
 Description-Content-Type: text/markdown
 Provides-Extra: estimate-area
@@ -90,14 +90,16 @@
   * [`update`](#update)
   * [`delete`](#delete)
   * [`status`](#status)
   * [`job`](#job)
   * [`jobs`](#jobs)
   * [`list`](#list)
   * [`tilejson`](#tilejson)
+* Activity
+  * [`list-activity`](#list-activity)
 
 ### upload-source
 
 ```shell
 tilesets upload-source <username> <source_id> <file>
 ```
 
@@ -410,7 +412,23 @@
 ```
 tilesets tilejson <tileset_id>
 ```
 
 Flags:
 
 * `--secure`: By default, resource URLs in the retrieved TileJSON (such as in the "tiles" array) will use the HTTP scheme. Include this query parameter in your request to receive HTTPS resource URLs instead.
+
+### list-activity
+
+Lists total request counts for a user's tilesets in the past 30 days. Returns a pagination key `next` if there are more results than the return limit that can be passed into another command as the `start` argument.
+
+```shell
+tilesets list-activity <account>
+```
+
+Flags:
+
+* `--sortby [requests|modified]` [optional]: Sorting key (default: requests)
+* `--orderby [asc|desc]` [optional]: Ordering key (default: desc)
+* `--limit [1-500]` [optional]: The maximum number of results to return (default: 100)
+* `--indent` [optional]: Indent size for JSON output.
+* `--start` [optional]: Pagination key from the `next` value in a response that has more results than the limit.
```

### Comparing `mapbox-tilesets-1.8.1/setup.py` & `mapbox-tilesets-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     zip_safe=False,
     extras_require={
         "estimate-area": [
             "supermercado~=0.2.0",
         ],
         "test": [
             "codecov",
-            "pytest==4.6.11",
+            "pytest==6.2.5",
             "pytest-cov",
             "pre-commit",
             "black==22.3.0",
             "pep8",
             "supermercado~=0.2.0",
             "toml==0.10.2",
         ],
```

