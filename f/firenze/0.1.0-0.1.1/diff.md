# Comparing `tmp/firenze-0.1.0.tar.gz` & `tmp/firenze-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firenze-0.1.0.tar", max compression
+gzip compressed data, was "firenze-0.1.1.tar", max compression
```

## Comparing `firenze-0.1.0.tar` & `firenze-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-20 22:32:23.212365 firenze-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1188 2023-06-20 22:31:18.532522 firenze-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-30 17:30:18.195622 firenze-0.1.0/firenze/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-20 22:31:35.520481 firenze-0.1.0/firenze/cli.py
--rw-r--r--   0        0        0       51 2023-06-18 00:25:42.769340 firenze-0.1.0/firenze/exceptions.py
--rw-r--r--   0        0        0     3935 2023-06-20 23:15:00.821191 firenze-0.1.0/firenze/notebook.py
--rw-r--r--   0        0        0      812 2023-06-20 23:29:26.814815 firenze-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 firenze-0.1.0/setup.py
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 firenze-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-20 22:32:23.212365 firenze-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1362 2023-06-20 23:51:36.311324 firenze-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 17:30:18.195622 firenze-0.1.1/firenze/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-20 22:31:35.520481 firenze-0.1.1/firenze/cli.py
+-rw-r--r--   0        0        0       51 2023-06-18 00:25:42.769340 firenze-0.1.1/firenze/exceptions.py
+-rw-r--r--   0        0        0     3935 2023-06-20 23:15:00.821191 firenze-0.1.1/firenze/notebook.py
+-rw-r--r--   0        0        0      812 2023-06-20 23:53:14.787071 firenze-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 firenze-0.1.1/setup.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 firenze-0.1.1/PKG-INFO
```

### Comparing `firenze-0.1.0/LICENSE.md` & `firenze-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `firenze-0.1.0/README.md` & `firenze-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 ```bash
 pip install firenze
 ```
 
 Suppose you have a very simple notebook that runs a "Hello, World!"
 
-![A notebook in jupyter](docs/img/hello_world_in_jupyter.png)
+![A notebook in jupyter](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_in_jupyter.png?raw=true)
 
 You can execute it right away with `firenze` through
 ```bash
 firenze docs/notebooks/hello_world.ipynb
 ```
 and the output html will be, as expected:
 
-![Hello, World! output](docs/img/hello_world_output.png)
+![Hello, World! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_output.png?raw=true)
 
 You can also send parameters and `firenze` will automatically modify the variable:
 
 ```bash
 firenze docs/notebooks/hello_world.ipynb name=Firenze
 ```
 
-![Hello, Firenze! output](docs/img/hello_world_with_parameters.png)
+![Hello, Firenze! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_with_parameters.png?raw=true)
 
 ## As a Docker Image
 This is still in the making, but one idea is to call `firenze` as a docker image with a notebook
 and a `requirements.txt`, so the notebook execution can be easily deployed to remote servers.
```

### Comparing `firenze-0.1.0/firenze/cli.py` & `firenze-0.1.1/firenze/cli.py`

 * *Files identical despite different names*

### Comparing `firenze-0.1.0/firenze/notebook.py` & `firenze-0.1.1/firenze/notebook.py`

 * *Files identical despite different names*

### Comparing `firenze-0.1.0/pyproject.toml` & `firenze-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firenze"
-version = "0.1.0"
+version = "0.1.1"
 description = "A lean executor for jupyter notebooks."
 authors = ["Pablo Alcain <pabloalcain@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `firenze-0.1.0/setup.py` & `firenze-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'nbformat>=5.8.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['firenze = firenze.cli:execute_notebook']}
 
 setup_kwargs = {
     'name': 'firenze',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A lean executor for jupyter notebooks.',
-    'long_description': '# Firenze\n\nFirenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML\nfile. You can also parameterize the notebooks without any modification to the notebook itself.\nIt supports local files and `s3` paths, both for the notebook and for the output.\n\n## As a Library\nYou can use `firenze` as a library in your own project. Install it through `pip`\n\n```bash\npip install firenze\n```\n\nSuppose you have a very simple notebook that runs a "Hello, World!"\n\n![A notebook in jupyter](docs/img/hello_world_in_jupyter.png)\n\nYou can execute it right away with `firenze` through\n```bash\nfirenze docs/notebooks/hello_world.ipynb\n```\nand the output html will be, as expected:\n\n![Hello, World! output](docs/img/hello_world_output.png)\n\nYou can also send parameters and `firenze` will automatically modify the variable:\n\n```bash\nfirenze docs/notebooks/hello_world.ipynb name=Firenze\n```\n\n![Hello, Firenze! output](docs/img/hello_world_with_parameters.png)\n\n## As a Docker Image\nThis is still in the making, but one idea is to call `firenze` as a docker image with a notebook\nand a `requirements.txt`, so the notebook execution can be easily deployed to remote servers.\n',
+    'long_description': '# Firenze\n\nFirenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML\nfile. You can also parameterize the notebooks without any modification to the notebook itself.\nIt supports local files and `s3` paths, both for the notebook and for the output.\n\n## As a Library\nYou can use `firenze` as a library in your own project. Install it through `pip`\n\n```bash\npip install firenze\n```\n\nSuppose you have a very simple notebook that runs a "Hello, World!"\n\n![A notebook in jupyter](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_in_jupyter.png?raw=true)\n\nYou can execute it right away with `firenze` through\n```bash\nfirenze docs/notebooks/hello_world.ipynb\n```\nand the output html will be, as expected:\n\n![Hello, World! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_output.png?raw=true)\n\nYou can also send parameters and `firenze` will automatically modify the variable:\n\n```bash\nfirenze docs/notebooks/hello_world.ipynb name=Firenze\n```\n\n![Hello, Firenze! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_with_parameters.png?raw=true)\n\n## As a Docker Image\nThis is still in the making, but one idea is to call `firenze` as a docker image with a notebook\nand a `requirements.txt`, so the notebook execution can be easily deployed to remote servers.\n',
     'author': 'Pablo Alcain',
     'author_email': 'pabloalcain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `firenze-0.1.0/PKG-INFO` & `firenze-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firenze
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lean executor for jupyter notebooks.
 License: MIT
 Author: Pablo Alcain
 Author-email: pabloalcain@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,29 +30,29 @@
 
 ```bash
 pip install firenze
 ```
 
 Suppose you have a very simple notebook that runs a "Hello, World!"
 
-![A notebook in jupyter](docs/img/hello_world_in_jupyter.png)
+![A notebook in jupyter](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_in_jupyter.png?raw=true)
 
 You can execute it right away with `firenze` through
 ```bash
 firenze docs/notebooks/hello_world.ipynb
 ```
 and the output html will be, as expected:
 
-![Hello, World! output](docs/img/hello_world_output.png)
+![Hello, World! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_output.png?raw=true)
 
 You can also send parameters and `firenze` will automatically modify the variable:
 
 ```bash
 firenze docs/notebooks/hello_world.ipynb name=Firenze
 ```
 
-![Hello, Firenze! output](docs/img/hello_world_with_parameters.png)
+![Hello, Firenze! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_with_parameters.png?raw=true)
 
 ## As a Docker Image
 This is still in the making, but one idea is to call `firenze` as a docker image with a notebook
 and a `requirements.txt`, so the notebook execution can be easily deployed to remote servers.
```

