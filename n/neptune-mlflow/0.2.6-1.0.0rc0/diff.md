# Comparing `tmp/neptune-mlflow-0.2.6.tar.gz` & `tmp/neptune_mlflow-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neptune-mlflow-0.2.6.tar", last modified: Wed Sep  8 07:40:25 2021, max compression
+gzip compressed data, was "neptune_mlflow-1.0.0rc0.tar", max compression
```

## Comparing `neptune-mlflow-0.2.6.tar` & `neptune_mlflow-1.0.0rc0.tar`

### file list

```diff
@@ -1,30 +1,16 @@
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       63 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/MANIFEST.in
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      816 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/PKG-INFO
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     3802 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/README.md
--rw-rw-r--   0 rafal     (1000) rafal     (1000)        6 2021-09-08 07:40:22.000000 neptune-mlflow-0.2.6/VERSION
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     1543 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/git_version.py
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      596 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/neptune_mlflow/__init__.py
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     5775 2021-09-08 07:37:09.000000 neptune-mlflow-0.2.6/neptune_mlflow/data_loader.py
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     1304 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/neptune_mlflow/sync.py
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      816 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/PKG-INFO
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      599 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/SOURCES.txt
--rw-rw-r--   0 rafal     (1000) rafal     (1000)        1 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/dependency_links.txt
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       55 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/entry_points.txt
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       77 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/requires.txt
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       43 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow.egg-info/top_level.txt
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/neptune_mlflow_plugin/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     1220 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/neptune_mlflow_plugin/__init__.py
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       77 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/requirements.txt
--rw-rw-r--   0 rafal     (1000) rafal     (1000)       61 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/setup.cfg
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     2806 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/setup.py
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/tests/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      596 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/tests/__init__.py
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      596 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow/__init__.py
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     3288 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow/test_data_loader.py
-drwxrwxr-x   0 rafal     (1000) rafal     (1000)        0 2021-09-08 07:40:25.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow_plugin/
--rw-rw-r--   0 rafal     (1000) rafal     (1000)      596 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow_plugin/__init__.py
--rw-rw-r--   0 rafal     (1000) rafal     (1000)     1418 2021-08-26 18:16:34.000000 neptune-mlflow-0.2.6/tests/neptune_mlflow_plugin/test_plugin.py
+-rw-r--r--   0        0        0      178 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     2497 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/README.md
+-rw-r--r--   0        0        0     2558 2023-06-21 16:40:15.663216 neptune_mlflow-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2581 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/__init__.py
+-rw-r--r--   0        0        0     3287 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/artifact_strategy.py
+-rw-r--r--   0        0        0      873 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/components/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/components/config.py
+-rw-r--r--   0        0        0     3308 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/components/exporter.py
+-rw-r--r--   0        0        0     3150 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/components/fetcher.py
+-rw-r--r--   0        0        0     2139 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/neptune_exporter.py
+-rw-r--r--   0        0        0     2470 2023-06-21 16:40:03.027019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/orchestrator.py
+-rw-r--r--   0        0        0     1655 2023-06-21 16:40:03.031019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/sync.py
+-rw-r--r--   0        0        0     1334 2023-06-21 16:40:03.031019 neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/version.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 neptune_mlflow-1.0.0rc0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neptune-mlflow-0.2.6/neptune_mlflow/__init__.py` & `neptune_mlflow-1.0.0rc0/src/neptune_mlflow_exporter/impl/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2023, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+__all__ = ["NeptuneExporter", "__version__"]
+
+from neptune_mlflow_exporter.impl.neptune_exporter import NeptuneExporter
+from neptune_mlflow_exporter.impl.version import __version__
```

### Comparing `neptune-mlflow-0.2.6/setup.py` & `neptune_mlflow-1.0.0rc0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,100 @@
-#
-# Copyright (c) 2020, Neptune Labs Sp. z o.o.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-
-import os
-
-from setuptools import find_packages, setup
-
-import git_version
-
-
-def version():
-    try:
-        with open('VERSION') as f:
-            return f.readline().strip()
-    except IOError:
-        return '0.0.0'
-
-
-def main():
-    root_dir = os.path.dirname(__file__)
-
-    with open(os.path.join(root_dir, 'requirements.txt')) as f:
-        requirements = [r.strip() for r in f]
-        setup(
-            name='neptune-mlflow',
-            version=version(),
-            url='https://github.com/neptune-ai/neptune-mlflow',
-            license='Apache License 2.0',
-            author='neptune.ai',
-            author_email='contact@neptune.ai',
-            description='Neptune MLFlow',
-            long_description=__doc__,
-            packages=find_packages(),
-            platforms='any',
-            install_requires=requirements,
-            entry_points={
-                'neptune.plugins': "mlflow = neptune_mlflow_plugin:sync"
-            },
-            cmdclass={
-                'git_version': git_version.GitVersion,
-            },
-            classifiers=[
-                # As from http://pypi.python.org/pypi?%3Aaction=list_classifiers
-                # 'Development Status :: 1 - Planning',
-                # 'Development Status :: 2 - Pre-Alpha',
-                # 'Development Status :: 3 - Alpha',
-                'Development Status :: 4 - Beta',
-                # 'Development Status :: 5 - Production/Stable',
-                # 'Development Status :: 6 - Mature',
-                # 'Development Status :: 7 - Inactive',
-                'Environment :: Console',
-                'Intended Audience :: Developers',
-                'License :: OSI Approved :: Apache Software License',
-                'Operating System :: POSIX',
-                'Operating System :: MacOS',
-                'Operating System :: Unix',
-                'Operating System :: Microsoft :: Windows',
-                'Programming Language :: Python',
-                'Programming Language :: Python :: 2',
-                'Programming Language :: Python :: 3',
-                'Topic :: Software Development :: Libraries :: Python Modules',
-            ]
-        )
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+pattern = "default-unprefixed"
+
+[tool.poetry.dependencies]
+python = "^3.7"
+
+# Python lack of functionalities from future versions
+importlib-metadata = { version = "*", python = "<3.8" }
+
+mlflow = ">=1.24.0"
+# dev
+pre-commit = { version = "*", optional = true }
+pytest = { version = ">=5.0", optional = true }
+pytest-cov = { version = "2.10.1", optional = true }
+neptune = { version = ">=1.0.0", optional = true }
+tensorflow = { version = ">2.0.0", optional = true }
+
+[tool.poetry.extras]
+dev = [
+    "pre-commit",
+    "pytest",
+    "pytest-cov",
+    "neptune",
+    "tensorflow",
+]
+
+[tool.poetry]
+authors = ["neptune.ai <contact@neptune.ai>"]
+description = "neptune.ai MLflow integration library"
+repository = "https://github.com/neptune-ai/neptune-mlflow"
+homepage = "https://neptune.ai/"
+documentation = "https://docs.neptune.ai/integrations/mlflow/"
+include = ["CHANGELOG.md"]
+license = "Apache License 2.0"
+name = "neptune-mlflow"
+readme = "README.md"
+version = "1.0.0-rc.0"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: Apache Software License",
+    "Natural Language :: English",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX",
+    "Operating System :: Unix",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+keywords = [
+    "MLOps",
+    "ML Experiment Tracking",
+    "ML Model Registry",
+    "ML Model Store",
+    "ML Metadata Store",
+]
+packages = [
+    { include = "neptune_mlflow_exporter", from = "src" },
+]
+
+[tool.poetry.urls]
+"Tracker" = "https://github.com/neptune-ai/neptune-mlflow/issues"
+"Documentation" = "https://docs.neptune.ai/integrations/mlflow/"
+
+[tool.black]
+line-length = 120
+target-version = ['py37', 'py38', 'py39', 'py310']
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | build
+  | dist
+)/
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 120
+force_grid_wrap = 2
+
+[tool.flake8]
+max-line-length = 120
+extend-ignore = "E203"
 
-
-if __name__ == "__main__":
-    main()
+[tool.poetry.plugins."neptune.plugins"]
+"mlflow" = "neptune_mlflow_exporter:sync"
```

