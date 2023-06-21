# Comparing `tmp/pingdat-1.2.0.tar.gz` & `tmp/pingdat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingdat-1.2.0.tar", max compression
+gzip compressed data, was "pingdat-1.3.0.tar", max compression
```

## Comparing `pingdat-1.2.0.tar` & `pingdat-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-20 01:16:06.408311 pingdat-1.2.0/LICENSE
--rw-r--r--   0        0        0     1958 2023-01-21 19:22:36.797674 pingdat-1.2.0/README.md
--rw-r--r--   0        0        0      623 2023-03-23 21:02:37.927720 pingdat-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5332 2023-03-23 21:02:37.947721 pingdat-1.2.0/src/pingdat/__init__.py
--rw-r--r--   0        0        0     2234 2023-03-23 21:02:37.967722 pingdat-1.2.0/src/pingdat/__main__.py
--rw-r--r--   0        0        0     1610 2023-03-23 21:02:37.967722 pingdat-1.2.0/src/pingdat/config.py
--rw-r--r--   0        0        0     1656 2023-03-23 03:27:34.371597 pingdat-1.2.0/src/pingdat/version.py
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 pingdat-1.2.0/setup.py
--rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 pingdat-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-19 20:51:11.000000 pingdat-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1958 2023-01-21 00:07:02.476491 pingdat-1.3.0/README.md
+-rw-r--r--   0        0        0      623 2023-06-21 00:26:07.968339 pingdat-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5332 2023-04-15 13:53:14.956309 pingdat-1.3.0/src/pingdat/__init__.py
+-rw-r--r--   0        0        0     2234 2023-04-15 13:53:14.956639 pingdat-1.3.0/src/pingdat/__main__.py
+-rw-r--r--   0        0        0     1610 2023-04-15 13:53:14.957070 pingdat-1.3.0/src/pingdat/config.py
+-rw-r--r--   0        0        0     1656 2023-03-18 01:55:35.051607 pingdat-1.3.0/src/pingdat/version.py
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 pingdat-1.3.0/setup.py
+-rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 pingdat-1.3.0/PKG-INFO
```

### Comparing `pingdat-1.2.0/LICENSE` & `pingdat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/README.md` & `pingdat-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/pyproject.toml` & `pingdat-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "pingdat"
-version = "1.2.0"
+version = "1.3.0"
 description = "A simple ping exporter for Prometheus metrics."
 authors = ["jheddings <jheddings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.2"
+requests = "^2.31.0"
 click = "^8.1.3"
 prometheus-client = "^0.16.0"
-pydantic = "^1.10.7"
+pydantic = "^1.10.9"
 pyyaml = "^6.0"
 ping3 = "^4.0.4"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.2.0"
+pre-commit = "^3.3.3"
 GitPython = "^3.1.31"
-pytest = "^7.2.2"
-coverage = "^7.2.2"
+pytest = "^7.3.2"
+coverage = "^7.2.7"
 
 [tool.poetry.scripts]
 pingdat = "pingdat.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pingdat-1.2.0/src/pingdat/__init__.py` & `pingdat-1.3.0/src/pingdat/__init__.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/src/pingdat/__main__.py` & `pingdat-1.3.0/src/pingdat/__main__.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/src/pingdat/config.py` & `pingdat-1.3.0/src/pingdat/config.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/src/pingdat/version.py` & `pingdat-1.3.0/src/pingdat/version.py`

 * *Files identical despite different names*

### Comparing `pingdat-1.2.0/setup.py` & `pingdat-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'ping3>=4.0.4,<5.0.0',
  'prometheus-client>=0.16.0,<0.17.0',
- 'pydantic>=1.10.7,<2.0.0',
+ 'pydantic>=1.10.9,<2.0.0',
  'pyyaml>=6.0,<7.0',
- 'requests>=2.28.2,<3.0.0']
+ 'requests>=2.31.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['pingdat = pingdat.__main__:main']}
 
 setup_kwargs = {
     'name': 'pingdat',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'A simple ping exporter for Prometheus metrics.',
     'long_description': '# pingdat #\n\n[![PyPI](https://img.shields.io/pypi/v/pingdat.svg)](https://pypi.org/project/pingdat)\n[![LICENSE](https://img.shields.io/github/license/jheddings/pingdat)](LICENSE)\n[![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)\n\nA Prometheus exporter for ping statistics.\n\n## Installation ##\n\nInstall the published package using pip:\n\n```shell\npip3 install pingdat\n```\n\nThis project uses `poetry` to manage dependencies and a local virtual environment.  To\nget started, clone the repository and install the dependencies with the following:\n\n```shell\npoetry install\n```\n\n### Grafana Dashboard ###\n\nA Grafana dashboard is available as #(17922)[https://grafana.com/grafana/dashboards/17922].\n\n## Usage ##\n\nRun the module and tell it which config file to use.\n\n```shell\npython3 -m pingdat --config pingdat.yaml\n```\n\nIf you are using `poetry` to manage the virtual environment, use the following:\n\n```shell\npoetry run pingdat --config pingdat.yaml\n```\n\n### Docker ###\n\n`pingdat` is available as a published Docker image.  To run, use the latest version:\nfrom Docker Hub:\n\n```shell\ndocker container run --rm --publish 9056:9056 "jheddings/pingdat:latest"\n```\n\nThe configuration file is read from `/opt/pingdat/pingdat.yaml` and may be changed\nwith arguments to the container:\n\n```shell\ndocker container run --rm --tty --publish 9056:9056 \\\n  --volume "/path/to/host/config:/etc/pingdat" \\\n  "jheddings/pingdat:latest" --config /etc/pingdat/pingdat.yaml\n```\n\n## Docker Compose ##\n\nA sample configuration is also provided for using `docker compose`.  Similar to using\nDocker directly, the configuration file can be provided on the host side.  Then,\nsimply start the cluster normally:\n\n```shell\ndocker compose up\n```\n\nOr detached as a background process:\n\n```shell\ndocker compose up --detach\n```\n\n## Configuration ##\n\nFor now, review the sample `pingdat.yaml` config file for a description of supported\nconfiguration options.\n',
     'author': 'jheddings',
     'author_email': 'jheddings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pingdat-1.2.0/PKG-INFO` & `pingdat-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pingdat
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple ping exporter for Prometheus metrics.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ping3 (>=4.0.4,<5.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pingdat #
 
 [![PyPI](https://img.shields.io/pypi/v/pingdat.svg)](https://pypi.org/project/pingdat)
 [![LICENSE](https://img.shields.io/github/license/jheddings/pingdat)](LICENSE)
 [![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)
```

