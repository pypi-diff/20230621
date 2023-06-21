# Comparing `tmp/pyright-1.1.314.tar.gz` & `tmp/pyright-1.1.315.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyright-1.1.314.tar", last modified: Wed Jun 14 03:47:17 2023, max compression
+gzip compressed data, was "pyright-1.1.315.tar", last modified: Wed Jun 21 13:59:52 2023, max compression
```

## Comparing `pyright-1.1.314.tar` & `pyright-1.1.315.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:47:17.521147 pyright-1.1.314/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 03:47:06.000000 pyright-1.1.314/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 03:47:06.000000 pyright-1.1.314/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-14 03:47:17.521147 pyright-1.1.314/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-14 03:47:06.000000 pyright-1.1.314/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-14 03:47:06.000000 pyright-1.1.314/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:47:17.521147 pyright-1.1.314/pyright/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/_mureq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/langserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-14 03:47:06.000000 pyright-1.1.314/pyright/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:47:17.521147 pyright-1.1.314/pyright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 03:47:17.000000 pyright-1.1.314/pyright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 03:47:06.000000 pyright-1.1.314/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:47:17.521147 pyright-1.1.314/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-06-14 03:47:06.000000 pyright-1.1.314/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:59:52.144504 pyright-1.1.315/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 13:59:40.000000 pyright-1.1.315/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 13:59:40.000000 pyright-1.1.315/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-21 13:59:52.144504 pyright-1.1.315/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-21 13:59:40.000000 pyright-1.1.315/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-21 13:59:40.000000 pyright-1.1.315/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:59:52.144504 pyright-1.1.315/pyright/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/_mureq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/langserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-21 13:59:40.000000 pyright-1.1.315/pyright/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:59:52.144504 pyright-1.1.315/pyright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 13:59:52.000000 pyright-1.1.315/pyright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 13:59:40.000000 pyright-1.1.315/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:59:52.144504 pyright-1.1.315/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-06-21 13:59:40.000000 pyright-1.1.315/setup.py
```

### Comparing `pyright-1.1.314/LICENSE` & `pyright-1.1.315/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/PKG-INFO` & `pyright-1.1.315/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.314
+Version: 1.1.315
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.314
+    rev: v1.1.315
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
@@ -120,14 +120,15 @@
 
 If neither of them are set it defaults to `~/.cache`
 
 ### Force Node Env
 
 Set `PYRIGHT_PYTHON_GLOBAL_NODE` to any non-truthy value, i.e. anything apart from 1, t, on, or true.
 e.g. `off`
+You can optionnaly choose the version of node used by setting `PYRIGHT_PYTHON_NODE_VERSION` to the desired version
 
 ### Modify Node Env Location
 
 Set `PYRIGHT_PYTHON_ENV_DIR` to a valid [nodeenv](https://github.com/ekalinin/nodeenv) directory. e.g. `~/.cache/nodeenv`
 
 ### Ignore Warnings
```

### Comparing `pyright-1.1.314/README.md` & `pyright-1.1.315/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.314
+    rev: v1.1.315
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
@@ -94,14 +94,15 @@
 
 If neither of them are set it defaults to `~/.cache`
 
 ### Force Node Env
 
 Set `PYRIGHT_PYTHON_GLOBAL_NODE` to any non-truthy value, i.e. anything apart from 1, t, on, or true.
 e.g. `off`
+You can optionnaly choose the version of node used by setting `PYRIGHT_PYTHON_NODE_VERSION` to the desired version
 
 ### Modify Node Env Location
 
 Set `PYRIGHT_PYTHON_ENV_DIR` to a valid [nodeenv](https://github.com/ekalinin/nodeenv) directory. e.g. `~/.cache/nodeenv`
 
 ### Ignore Warnings
```

### Comparing `pyright-1.1.314/pyright/__init__.py` & `pyright-1.1.315/pyright/__init__.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/_mureq.py` & `pyright-1.1.315/pyright/_mureq.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/_utils.py` & `pyright-1.1.315/pyright/_utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/cli.py` & `pyright-1.1.315/pyright/cli.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/errors.py` & `pyright-1.1.315/pyright/errors.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/langserver.py` & `pyright-1.1.315/pyright/langserver.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/node.py` & `pyright-1.1.315/pyright/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 log: logging.Logger = logging.getLogger(__name__)
 
 ENV_DIR: Path = get_env_dir()
 BINARIES_DIR: Path = get_bin_dir(env_dir=ENV_DIR)
 USE_GLOBAL_NODE = env_to_bool('PYRIGHT_PYTHON_GLOBAL_NODE', default=True)
+NODE_VERSION = os.environ.get('PYRIGHT_PYTHON_NODE_VERSION', default=None)
 VERSION_RE = re.compile(r'\d+\.\d+\.\d+')
 
 
 def _ensure_available(target: Target) -> Binary:
     """Ensure the target node executable is available"""
     path = None
     if USE_GLOBAL_NODE:
@@ -53,15 +54,15 @@
 def _ensure_node_env(target: Target) -> Path:
     log.debug('Checking for nodeenv %s binary', target)
 
     path = BINARIES_DIR.joinpath(target + _postfix_for_target(target))
 
     log.debug('Using %s path for binary', path)
 
-    if path.exists():
+    if path.exists() and not NODE_VERSION:
         log.debug('Binary at %s exists, skipping nodeenv installation', path)
     else:
         log.debug('Installing nodeenv as a binary at %s could not be found', path)
         _install_node_env()
 
     if not path.exists():
         raise errors.BinaryNotFound(path=path, target=target)
@@ -82,15 +83,19 @@
 
     log.debug('Global target binary: %s not found', target)
     return None
 
 
 def _install_node_env() -> None:
     log.debug('Installing nodeenv to %s', ENV_DIR)
-    args = [sys.executable, '-m', 'nodeenv', str(ENV_DIR)]
+    args = [sys.executable, '-m', 'nodeenv']
+    if NODE_VERSION:
+        log.debug(f"Using user specified node version: {NODE_VERSION}")
+        args += ["--node", NODE_VERSION, "--force"]
+    args.append(str(ENV_DIR))
     log.debug('Running command with args: %s', args)
     subprocess.run(args, check=True)
 
 
 def run(
     target: Target, *args: str, **kwargs: Any
 ) -> Union['subprocess.CompletedProcess[bytes]', 'subprocess.CompletedProcess[str]']:
```

### Comparing `pyright-1.1.314/pyright/types.py` & `pyright-1.1.315/pyright/types.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright/utils.py` & `pyright-1.1.315/pyright/utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.314/pyright.egg-info/PKG-INFO` & `pyright-1.1.315/pyright.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.314
+Version: 1.1.315
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.314
+    rev: v1.1.315
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
@@ -120,14 +120,15 @@
 
 If neither of them are set it defaults to `~/.cache`
 
 ### Force Node Env
 
 Set `PYRIGHT_PYTHON_GLOBAL_NODE` to any non-truthy value, i.e. anything apart from 1, t, on, or true.
 e.g. `off`
+You can optionnaly choose the version of node used by setting `PYRIGHT_PYTHON_NODE_VERSION` to the desired version
 
 ### Modify Node Env Location
 
 Set `PYRIGHT_PYTHON_ENV_DIR` to a valid [nodeenv](https://github.com/ekalinin/nodeenv) directory. e.g. `~/.cache/nodeenv`
 
 ### Ignore Warnings
```

### Comparing `pyright-1.1.314/setup.py` & `pyright-1.1.315/setup.py`

 * *Files identical despite different names*

