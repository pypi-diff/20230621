# Comparing `tmp/computex_cli-0.1.4.tar.gz` & `tmp/computex_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.4.tar", max compression
+gzip compressed data, was "computex_cli-0.1.5.tar", max compression
```

## Comparing `computex_cli-0.1.4.tar` & `computex_cli-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      613 2023-06-19 17:17:45.415196 computex_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-08 18:28:28.160718 computex_cli-0.1.4/cxcli/__init__.py
--rw-r--r--   0        0        0     6522 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/auth.py
--rw-r--r--   0        0        0     2075 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-06-19 17:17:45.415196 computex_cli-0.1.4/cxcli/services/users.py
--rw-r--r--   0        0        0      727 2023-06-19 17:18:00.035243 computex_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-06-21 04:23:16.786796 computex_cli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/__init__.py
+-rw-r--r--   0        0        0     6742 2023-06-21 06:12:00.930141 computex_cli-0.1.5/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/auth.py
+-rw-r--r--   0        0        0     2263 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/users.py
+-rw-r--r--   0        0        0      727 2023-06-21 06:14:11.268529 computex_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.5/PKG-INFO
```

### Comparing `computex_cli-0.1.4/README.md` & `computex_cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.4/cxcli/cli.py` & `computex_cli-0.1.5/cxcli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,15 +189,20 @@
     r = DeploymentServiceV1().logs(app)
     click.echo(json.dumps(r.json(), indent=4))
 
 
 @cli.command()
 @click.option("--app")
 @click.option("--data")
+@click.option("--is-public", default=False)
+@click.option("--is-serverless", default=False)
 @refresh_credentials
-def predict(app, data):
-    r = DeploymentServiceV1().predict(app, data)
+def predict(app, data, is_public, is_serverless):
+    data_dict = json.loads(data)
+    r = DeploymentServiceV1().predict(
+        app, data_dict, is_serverless=is_serverless, is_public=is_public
+    )
     click.echo(json.dumps(r.dict(), indent=4))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `computex_cli-0.1.4/cxcli/config.py` & `computex_cli-0.1.5/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.4/cxcli/services/auth.py` & `computex_cli-0.1.5/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.4/cxcli/services/deployments.py` & `computex_cli-0.1.5/cxcli/services/deployments.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,12 +65,19 @@
     def logs(self, app_name: str):
         r = self._get(f"/{app_name}/logs")
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
         j = r.json()
         return LogsResponse(logs=j["logs"])
 
-    def predict(self, app_name: str, data: dict):
-        r = self._post(f"/{app_name}/predict", json=data)
+    def predict(
+        self,
+        app_name: str,
+        data: dict,
+        is_serverless: bool = False,
+        is_public: bool = False,
+    ):
+        params = dict(is_serverless=is_serverless, is_public=is_public)
+        r = self._post(f"/{app_name}/predict", json=data, params=params)
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
         return PredictResponse(result=r.json())
```

### Comparing `computex_cli-0.1.4/cxcli/services/service.py` & `computex_cli-0.1.5/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.4/cxcli/services/users.py` & `computex_cli-0.1.5/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.4/pyproject.toml` & `computex_cli-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `computex_cli-0.1.4/PKG-INFO` & `computex_cli-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computex-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: ComputeX CLI tool
 Author: Abate De Mey
 Author-email: abate@computex.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

