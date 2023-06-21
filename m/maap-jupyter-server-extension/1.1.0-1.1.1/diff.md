# Comparing `tmp/maap_jupyter_server_extension-1.1.0.tar.gz` & `tmp/maap_jupyter_server_extension-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maap_jupyter_server_extension-1.1.0.tar", last modified: Thu Jun  8 15:57:37 2023, max compression
+gzip compressed data, was "maap_jupyter_server_extension-1.1.1.tar", last modified: Wed Jun 21 21:24:49 2023, max compression
```

## Comparing `maap_jupyter_server_extension-1.1.0.tar` & `maap_jupyter_server_extension-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:37.000452 maap_jupyter_server_extension-1.1.0/
--rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/CHANGELOG.md
--rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.1.0/LICENSE
--rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.1.0/MANIFEST.in
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-08 15:57:36.999711 maap_jupyter_server_extension-1.1.0/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.1.0/README.md
--rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.1.0/conftest.py
--rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.1.0/install.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.969290 maap_jupyter_server_extension-1.1.0/jupyter-config/
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.976730 maap_jupyter_server_extension-1.1.0/jupyter-config/nb-config/
--rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.0/jupyter-config/nb-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.977435 maap_jupyter_server_extension-1.1.0/jupyter-config/server-config/
--rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.0/jupyter-config/server-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.980002 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/
--rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/__init__.py
--rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/_version.py
--rw-r--r--   0 mlucas     (502) staff       (20)    23457 2023-06-07 23:49:22.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/handlers.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.982735 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/
--rw-r--r--   0 mlucas     (502) staff       (20)    21024 2023-06-08 15:54:52.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/build_log.json
--rw-r--r--   0 mlucas     (502) staff       (20)     2890 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/package.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.992518 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/
--rw-r--r--   0 mlucas     (502) staff       (20)     3775 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js
--rw-r--r--   0 mlucas     (502) staff       (20)     2459 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)    28001 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js
--rw-r--r--   0 mlucas     (502) staff       (20)    26958 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)      172 2023-06-08 15:54:52.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style.js
--rw-r--r--   0 mlucas     (502) staff       (20)     4630 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js
--rw-r--r--   0 mlucas     (502) staff       (20)     1832 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)    12088 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js
--rw-r--r--   0 mlucas     (502) staff       (20)    13835 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.995221 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     1749 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/SOURCES.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/dependency_links.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-08 15:53:58.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/not-zip-safe
--rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/requires.txt
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/top_level.txt
--rw-r--r--   0 mlucas     (502) staff       (20)     2748 2023-06-08 15:52:14.000000 maap_jupyter_server_extension-1.1.0/package.json
--rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.1.0/pyproject.toml
--rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-06-08 15:57:37.000623 maap_jupyter_server_extension-1.1.0/setup.cfg
--rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-06-05 22:15:51.000000 maap_jupyter_server_extension-1.1.0/setup.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.996418 maap_jupyter_server_extension-1.1.0/src/
--rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.0/src/handler.ts
--rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.0/src/index.ts
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.998636 maap_jupyter_server_extension-1.1.0/style/
--rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/base.css
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/index.css
--rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/index.js
--rw-r--r--   0 mlucas     (502) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.1.0/tsconfig.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.049524 maap_jupyter_server_extension-1.1.1/
+-rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.1/CHANGELOG.md
+-rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.1.1/LICENSE
+-rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.1.1/MANIFEST.in
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-21 21:24:49.049182 maap_jupyter_server_extension-1.1.1/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.1.1/README.md
+-rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.1.1/conftest.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.1.1/install.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.008027 maap_jupyter_server_extension-1.1.1/jupyter-config/
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.016607 maap_jupyter_server_extension-1.1.1/jupyter-config/nb-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.1/jupyter-config/nb-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.017438 maap_jupyter_server_extension-1.1.1/jupyter-config/server-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.1/jupyter-config/server-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.020506 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/__init__.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/_version.py
+-rw-r--r--   0 mlucas     (502) staff       (20)    23364 2023-06-21 20:37:50.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/handlers.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.021855 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/
+-rw-r--r--   0 mlucas     (502) staff       (20)     2890 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/package.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.032983 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/
+-rw-r--r--   0 mlucas     (502) staff       (20)     3534 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/747.2bf2ef3d0194bd67f235.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      914 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/763.4aa969c065d4b676c2e7.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     6520 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/remoteEntry.101e412232bc8eb4a92f.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      172 2023-06-21 21:24:47.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/style.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     2452 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.036545 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     1154 2023-06-21 21:24:49.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-21 21:23:52.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/not-zip-safe
+-rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/requires.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-06-21 21:24:48.000000 maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/top_level.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)     2748 2023-06-21 21:15:13.000000 maap_jupyter_server_extension-1.1.1/package.json
+-rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.1.1/pyproject.toml
+-rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-06-21 21:24:49.049629 maap_jupyter_server_extension-1.1.1/setup.cfg
+-rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-06-05 22:15:51.000000 maap_jupyter_server_extension-1.1.1/setup.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.038089 maap_jupyter_server_extension-1.1.1/src/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.1/src/handler.ts
+-rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.1/src/index.ts
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-21 21:24:49.048687 maap_jupyter_server_extension-1.1.1/style/
+-rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.1/style/base.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.1/style/index.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.1/style/index.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.1.1/tsconfig.json
+-rw-r--r--   0 mlucas     (502) staff       (20)   222486 2023-06-21 21:24:35.000000 maap_jupyter_server_extension-1.1.1/yarn.lock
```

### Comparing `maap_jupyter_server_extension-1.1.0/LICENSE` & `maap_jupyter_server_extension-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/MANIFEST.in` & `maap_jupyter_server_extension-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/PKG-INFO` & `maap_jupyter_server_extension-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap_jupyter_server_extension
-Version: 1.1.0
+Version: 1.1.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.1.0/README.md` & `maap_jupyter_server_extension-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/__init__.py` & `maap_jupyter_server_extension-1.1.1/jupyter_server_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/_version.py` & `maap_jupyter_server_extension-1.1.1/jupyter_server_extension/_version.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/handlers.py` & `maap_jupyter_server_extension-1.1.1/jupyter_server_extension/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,25 +188,25 @@
         for k, v in params.items():
             params[k] = v[0].decode("utf-8")
         return params
 
     def get(self):
         print("JOB SUBMIT")
 
-        #test_request = {"algo_id": "test_algo", "username": "anonymous", "queue": "geospec-job_worker-32gb"}
         kwargs = self.args_to_dict()
         #maap = MAAP(not_self_signed=False)
         maap = MAAP(maap_host=maap_api(self.request.host))
         resp = maap.submitJob(**kwargs)
         #logger.debug(resp)
-        status_code = resp['http_status_code']
-        print("PRINT RESPONSE")
-        print(resp)
+        
+        # status_code = resp['http_status_code']
+        status_code = resp.response_code
+        job_id = resp.id
         if status_code == 200:
-            result = 'JobID is {}'.format(resp['job_id'])
+            result = 'JobID is {}'.format(job_id)
             self.finish({"status_code": status_code, "response": result})
         elif status_code == 400:
             self.finish({"status_code": status_code, "response": resp['result']})
         else:
             self.finish({"status_code": status_code, "response": resp['status']})
```

### Comparing `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/package.json` & `maap_jupyter_server_extension-1.1.1/jupyter_server_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.101e412232bc8eb4a92f.js'}}",*

 * * "'version'": "'1.1.1'"}*

```diff
@@ -40,15 +40,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.38858848937d208638ab.js",
+            "load": "static/remoteEntry.101e412232bc8eb4a92f.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_server_extension"
                 },
@@ -93,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/PKG-INFO` & `maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap-jupyter-server-extension
-Version: 1.1.0
+Version: 1.1.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/SOURCES.txt` & `maap_jupyter_server_extension-1.1.1/maap_jupyter_server_extension.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,30 +4,26 @@
 README.md
 conftest.py
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
+yarn.lock
 jupyter-config/nb-config/dps_jupyter_server_extension.json
 jupyter-config/server-config/dps_jupyter_server_extension.json
 jupyter_server_extension/__init__.py
 jupyter_server_extension/_version.py
 jupyter_server_extension/handlers.py
-jupyter_server_extension/labextension/build_log.json
 jupyter_server_extension/labextension/package.json
-jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js
-jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map
-jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js
-jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js.map
+jupyter_server_extension/labextension/static/747.2bf2ef3d0194bd67f235.js
+jupyter_server_extension/labextension/static/763.4aa969c065d4b676c2e7.js
+jupyter_server_extension/labextension/static/remoteEntry.101e412232bc8eb4a92f.js
 jupyter_server_extension/labextension/static/style.js
-jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js
-jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map
-jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js
-jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map
+jupyter_server_extension/labextension/static/third-party-licenses.json
 maap_jupyter_server_extension.egg-info/PKG-INFO
 maap_jupyter_server_extension.egg-info/SOURCES.txt
 maap_jupyter_server_extension.egg-info/dependency_links.txt
 maap_jupyter_server_extension.egg-info/not-zip-safe
 maap_jupyter_server_extension.egg-info/requires.txt
 maap_jupyter_server_extension.egg-info/top_level.txt
 src/handler.ts
```

### Comparing `maap_jupyter_server_extension-1.1.0/package.json` & `maap_jupyter_server_extension-1.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `maap_jupyter_server_extension-1.1.0/pyproject.toml` & `maap_jupyter_server_extension-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/setup.py` & `maap_jupyter_server_extension-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/src/handler.ts` & `maap_jupyter_server_extension-1.1.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/src/index.ts` & `maap_jupyter_server_extension-1.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.1.0/tsconfig.json` & `maap_jupyter_server_extension-1.1.1/tsconfig.json`

 * *Files identical despite different names*

