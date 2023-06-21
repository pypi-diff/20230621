# Comparing `tmp/docker_tags_getter-0.3.3.tar.gz` & `tmp/docker_tags_getter-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_tags_getter-0.3.3.tar", max compression
+gzip compressed data, was "docker_tags_getter-0.3.4.tar", max compression
```

## Comparing `docker_tags_getter-0.3.3.tar` & `docker_tags_getter-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      260 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/README.rst
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/api/v2/__init__.py
--rw-r--r--   0        0        0      704 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/api/v2/repositories_api.py
--rw-r--r--   0        0        0      722 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/api/v2/tags_api.py
--rw-r--r--   0        0        0      348 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/cli/cli.py
--rw-r--r--   0        0        0     3206 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/cli/repo.py
--rw-r--r--   0        0        0     2488 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/cli/repos.py
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/config/__init__.py
--rw-r--r--   0        0        0      196 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/config/headers_config.py
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/fetcher/__init__.py
--rw-r--r--   0        0        0      417 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/fetcher/api_fetcher.py
--rw-r--r--   0        0        0        0 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/filters/__init__.py
--rw-r--r--   0        0        0      142 2023-06-19 07:22:55.908807 docker_tags_getter-0.3.3/docker_tags_getter/filters/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      955 2023-06-19 07:22:55.912807 docker_tags_getter-0.3.3/docker_tags_getter/filters/__pycache__/tags_filter.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/filters/tags_filter.py
--rw-r--r--   0        0        0      113 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/docker_tags_getter/main.py
--rw-r--r--   0        0        0      806 2023-06-19 07:22:14.556058 docker_tags_getter-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 docker_tags_getter-0.3.3/setup.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 docker_tags_getter-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-06-21 07:31:45.934357 docker_tags_getter-0.3.4/README.rst
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/api/v2/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/api/v2/repositories_api.py
+-rw-r--r--   0        0        0      722 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/api/v2/tags_api.py
+-rw-r--r--   0        0        0      348 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/cli/cli.py
+-rw-r--r--   0        0        0     3494 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/cli/repo.py
+-rw-r--r--   0        0        0     2488 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/cli/repos.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/config/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/config/headers_config.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/fetcher/__init__.py
+-rw-r--r--   0        0        0      417 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/fetcher/api_fetcher.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/filters/__init__.py
+-rw-r--r--   0        0        0      142 2023-06-21 07:32:27.107098 docker_tags_getter-0.3.4/docker_tags_getter/filters/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      955 2023-06-21 07:32:27.107098 docker_tags_getter-0.3.4/docker_tags_getter/filters/__pycache__/tags_filter.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/filters/tags_filter.py
+-rw-r--r--   0        0        0      113 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/docker_tags_getter/main.py
+-rw-r--r--   0        0        0      806 2023-06-21 07:31:45.938357 docker_tags_getter-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 docker_tags_getter-0.3.4/setup.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 docker_tags_getter-0.3.4/PKG-INFO
```

### Comparing `docker_tags_getter-0.3.3/docker_tags_getter/api/v2/repositories_api.py` & `docker_tags_getter-0.3.4/docker_tags_getter/api/v2/repositories_api.py`

 * *Files identical despite different names*

### Comparing `docker_tags_getter-0.3.3/docker_tags_getter/api/v2/tags_api.py` & `docker_tags_getter-0.3.4/docker_tags_getter/api/v2/tags_api.py`

 * *Files identical despite different names*

### Comparing `docker_tags_getter-0.3.3/docker_tags_getter/cli/repo.py` & `docker_tags_getter-0.3.4/docker_tags_getter/cli/repo.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,19 @@
         show_default=False
     ),
     filter: bool = typer.Option(
         None, "--filter", "-f",
         help="[b]The tags[/] will be filtered.",
         show_default=False
     ),
+    full_name: bool = typer.Option(
+        None, "--full-name", "-fn",
+        help="[b]The tags[/] will be shown with their [b]namespace and repository[/].",
+        show_default=False
+    ),
 ):
     """
     [green b]All tags[/] will be returned for the [yellow b]namespace[/].
     """
     if namespace is None:
         console.print(f"[red b][ERROR] Please, give the namespace name!!![/]")
         return
@@ -70,10 +75,14 @@
     if filter:
         if 'latest' in tags:
             tags.remove('latest')
 
         tags_filter = TagsFilter()
         tags = tags_filter.filter_list(tags)
 
+    prefix = ''
+    if full_name:
+        prefix = f'{namespace}/{repository}:'
+
     for tag in tags:
-        console.print(tag)
+        console.print(f'{prefix}{tag}')
```

### Comparing `docker_tags_getter-0.3.3/docker_tags_getter/cli/repos.py` & `docker_tags_getter-0.3.4/docker_tags_getter/cli/repos.py`

 * *Files identical despite different names*

### Comparing `docker_tags_getter-0.3.3/docker_tags_getter/filters/__pycache__/tags_filter.cpython-310.pyc` & `docker_tags_getter-0.3.4/docker_tags_getter/filters/__pycache__/tags_filter.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 19 07:22:14 2023 UTC, .py size: 308 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2602 9064 3401 0000  o.......&..d4...
+00000000: 6f0d 0d0a 0000 0000 61a7 9264 3401 0000  o.......a..d4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 2a00 0000 6500  .....@...s*...e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
```

### Comparing `docker_tags_getter-0.3.3/pyproject.toml` & `docker_tags_getter-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-tags-getter"
-version = "0.3.3"
+version = "0.3.4"
 description = "docker_tags_getter will help you to get tags from your docker repository."
 authors = ["Kostiantyn Klochko <kostya_klochko@ukr.net>"]
 readme = "README.rst"
 license = "LGPL-3.0-or-later"
 packages = [{include = "docker_tags_getter"}]
 repository = "https://gitlab.com/KKlochko/docker_tags_getter"
 keywords = ["cli", "docker", "repos", "tags"]
```

### Comparing `docker_tags_getter-0.3.3/setup.py` & `docker_tags_getter-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['requests>=2.31.0,<3.0.0', 'rich>=13.4.2,<14.0.0', 'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['dtg = docker_tags_getter.main:main']}
 
 setup_kwargs = {
     'name': 'docker-tags-getter',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'docker_tags_getter will help you to get tags from your docker repository.',
     'long_description': 'docker_tags_getter\n==================\n\ndocker_tags_getter is the application that will help you to get tags from yours docker repository.\n\nAuthor\n======\n\nKostiantyn Klochko (c) 2023\n\nLicense\n=======\n\nUnder the GNU Lesser General Public License v3.0 or later.\n\n',
     'author': 'Kostiantyn Klochko',
     'author_email': 'kostya_klochko@ukr.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/KKlochko/docker_tags_getter',
```

### Comparing `docker_tags_getter-0.3.3/PKG-INFO` & `docker_tags_getter-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-tags-getter
-Version: 0.3.3
+Version: 0.3.4
 Summary: docker_tags_getter will help you to get tags from your docker repository.
 Home-page: https://gitlab.com/KKlochko/docker_tags_getter
 License: LGPL-3.0-or-later
 Keywords: cli,docker,repos,tags
 Author: Kostiantyn Klochko
 Author-email: kostya_klochko@ukr.net
 Requires-Python: >=3.9,<4.0
```

