# Comparing `tmp/cerebrium-1.1.1.tar.gz` & `tmp/cerebrium-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.1.tar", max compression
+gzip compressed data, was "cerebrium-1.1.2.tar", max compression
```

## Comparing `cerebrium-1.1.1.tar` & `cerebrium-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-13 21:26:20.075493 cerebrium-1.1.1/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-13 21:26:20.075493 cerebrium-1.1.1/README.md
--rw-r--r--   0        0        0      330 2023-06-13 21:31:24.282792 cerebrium-1.1.1/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     9110 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/cli.py
--rw-r--r--   0        0        0    31667 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/conduit.py
--rw-r--r--   0        0        0     5049 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/errors.py
--rw-r--r--   0        0        0    11299 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8540 2023-06-13 21:26:20.079493 cerebrium-1.1.1/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-13 21:26:20.079493 cerebrium-1.1.1/cerebrium/utils.py
--rw-r--r--   0        0        0     2546 2023-06-13 21:31:24.282792 cerebrium-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-21 15:33:31.298231 cerebrium-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-21 15:33:31.298231 cerebrium-1.1.2/README.md
+-rw-r--r--   0        0        0      330 2023-06-21 15:37:17.443700 cerebrium-1.1.2/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    10122 2023-06-21 15:33:31.298231 cerebrium-1.1.2/cerebrium/cli.py
+-rw-r--r--   0        0        0    31667 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5049 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8540 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/utils.py
+-rw-r--r--   0        0        0     2546 2023-06-21 15:37:17.443700 cerebrium-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.2/PKG-INFO
```

### Comparing `cerebrium-1.1.1/LICENSE` & `cerebrium-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/README.md` & `cerebrium-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/cli.py` & `cerebrium-1.1.2/cerebrium/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import requests
 import zipfile
 import tempfile
 import yaspin
 import time
+import yaml
 from termcolor import colored
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 from cerebrium import __version__ as cerebrium_version
 
 app = typer.Typer()
 env = os.getenv("ENV", "prod")
@@ -40,24 +41,50 @@
 def login(
     private_api_key: str = typer.Argument(
         ...,
         help="Private API key for the user. Sets the environment variable CEREBRIUM_API_KEY.",
     )
 ):
     """
-    Set private API key for the user as an environment variable
+    Set private API key for the user in ~/.cerebrium/config.yaml
     """
-    os.environ["CEREBRIUM_API_KEY"] = private_api_key
+    config_path = os.path.expanduser("~/.cerebrium/config.yaml")
+    os.makedirs(os.path.dirname(config_path), exist_ok=True)
+    config = yaml.full_load(open(config_path, "r"))
+    if config is None:
+        config = {"api_key": private_api_key}
+    else:
+        config["api_key"] = private_api_key
+    with open(config_path, "w") as f:
+        yaml.dump(config, f)
+    print("✅  Logged in successfully.")
+
+
+def get_api_key():
+    config_path = os.path.expanduser("~/.cerebrium/config.yaml")
+    if not os.path.exists(config_path):
+        print(
+            "Please login using 'cerebrium login <private_api_key>' or specify the API key using the --api-key flag."
+        )
+        sys.exit(1)
+    config = yaml.full_load(open(config_path, "r"))
+    if config is None or "api_key" not in config:
+        print(
+            "Please login using 'cerebrium login <private_api_key>' or specify the API key using the --api-key flag."
+        )
+        sys.exit(1)
+    return config["api_key"]
 
 
 @app.command()
 def deploy(
     name: str = typer.Argument(..., help="Name of the builder deployment."),
-    api_key: str = typer.Argument(
-        ..., envvar="CEREBRIUM_API_KEY", help="Private API key for the user."
+    api_key: str = typer.Option(
+        "", 
+        help="Private API key for the user."
     ),
     hardware: str = typer.Option(
         "GPU",
         help="Hardware to use for the builder deployment. Can be one of 'CPU', 'GPU' or 'A10'.",
     ),
     init_debug: bool = typer.Option(
         False,
@@ -72,28 +99,32 @@
         help="Log level for the builder deployment. Can be one of 'DEBUG' or 'INFO'",
     ),
 ):
     """
     Deploy a builder deployment to Cerebrium
     """
     print(f"Deploying {name} with {hardware} hardware to Cerebrium...")
+    if not api_key:
+        api_key = get_api_key()
 
     requirements_hash = "REQUIREMENTS_FILE_DOESNT_EXIST"
     pkglist_hash = "PKGLIST_FILE_DOESNT_EXIST"
 
     # Check if main.py exists
     if not os.path.exists("./main.py"):
         print("main.py not found in current directory. This file is required.")
         sys.exit(1)
 
     # Check main.py for a predict function
     with open("./main.py", "r") as f:
         main_py = f.read()
         if "def predict(" not in main_py:
-            print("main.py does not contain a predict function. This function is required.")
+            print(
+                "main.py does not contain a predict function. This function is required."
+            )
             sys.exit(1)
 
     # Calc MD5 hash of ./requirements.txt
     if os.path.exists("./requirements.txt"):
         with open("./requirements.txt", "rb") as f:
             requirements_hash = hashlib.md5(f.read()).hexdigest()
```

### Comparing `cerebrium-1.1.1/cerebrium/conduit.py` & `cerebrium-1.1.2/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/core.py` & `cerebrium-1.1.2/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/errors.py` & `cerebrium-1.1.2/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/flow.py` & `cerebrium-1.1.2/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/logging/arize.py` & `cerebrium-1.1.2/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/logging/base.py` & `cerebrium-1.1.2/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/logging/censius.py` & `cerebrium-1.1.2/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/models/base.py` & `cerebrium-1.1.2/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/models/sklearn.py` & `cerebrium-1.1.2/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/cerebrium/requests.py` & `cerebrium-1.1.2/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.1/pyproject.toml` & `cerebrium-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.1.1/PKG-INFO` & `cerebrium-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

