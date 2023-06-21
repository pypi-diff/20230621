# Comparing `tmp/pull-request-codecommit-0.5.1.tar.gz` & `tmp/pull_request_codecommit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pull-request-codecommit-0.5.1.tar", last modified: Mon Mar  6 09:17:29 2023, max compression
+gzip compressed data, was "pull_request_codecommit-0.5.2.tar", max compression
```

## Comparing `pull-request-codecommit-0.5.1.tar` & `pull_request_codecommit-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-06 09:17:29.280885 pull-request-codecommit-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/pull_request_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/pull_request_codecommit/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/aws/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/pull_request_codecommit/git/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/commits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/git/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request_codecommit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pull_request_codecommit/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-06 09:17:29.000000 pull-request-codecommit-0.5.1/pull_request_codecommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-06 09:17:29.280885 pull-request-codecommit-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:17:29.276885 pull-request-codecommit-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/tests/test_git_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/tests/test_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-06 09:17:04.000000 pull-request-codecommit-0.5.1/tests/test_repository.py
+-rw-r--r--   0        0        0     1052 2023-06-21 11:18:06.514315 pull_request_codecommit-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0     2336 2023-06-21 11:18:07.170313 pull_request_codecommit-0.5.2/pull_request_codecommit/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/aws/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/aws/client.py
+-rw-r--r--   0        0        0     1513 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/config.py
+-rw-r--r--   0        0        0      139 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/__init__.py
+-rw-r--r--   0        0        0     2033 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/client.py
+-rw-r--r--   0        0        0      401 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/commit.py
+-rw-r--r--   0        0        0     1681 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/commits.py
+-rw-r--r--   0        0        0     1232 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/message.py
+-rw-r--r--   0        0        0     1571 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/remote.py
+-rw-r--r--   0        0        0     1452 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request.py
+-rw-r--r--   0        0        0     2826 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_codecommit.py
+-rw-r--r--   0        0        0     2793 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_proposal.py
+-rw-r--r--   0        0        0     1495 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/repository.py
+-rw-r--r--   0        0        0      972 2023-06-21 11:18:07.170313 pull_request_codecommit-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 pull_request_codecommit-0.5.2/PKG-INFO
```

### Comparing `pull-request-codecommit-0.5.1/LICENSE.md` & `pull_request_codecommit-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/__init__.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional
 
 import click
 
 from .pull_request import PullRequest
 from .repository import Repository
 
+__version__ = "0.5.2"
+
 
 @click.command()
 @click.option("-r", "--repository-path", default=None)
 @click.option("-b", "--branch", default=None)
 @click.option("--auto-merge/--no-auto-merge", default=False)
 def main(
     repository_path: Optional[str], branch: Optional[str], auto_merge: bool
```

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/aws/client.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/aws/client.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/config.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/config.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/git/client.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/git/client.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/git/commits.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/git/commits.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/git/message.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/git/message.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/git/remote.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/git/remote.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request_codecommit.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_codecommit.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/pull_request_proposal.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_proposal.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pull_request_codecommit/repository.py` & `pull_request_codecommit-0.5.2/pull_request_codecommit/repository.py`

 * *Files identical despite different names*

### Comparing `pull-request-codecommit-0.5.1/pyproject.toml` & `pull_request_codecommit-0.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pull-request-codecommit"
-version = "0.5.1"
+version = "0.5.2"
 description = "pull-request-codecommit creates a PR within CodeCommit based on your commit messages."
 authors = ["Joris Conijn <joris@conijnonline.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.3"
@@ -21,10 +21,20 @@
 xenon = "^0.9.0"
 radon = "^5.1.0"
 
 [tool.poetry.scripts]
 pull-request-codecommit = "pull_request_codecommit:main"
 git-pr = "pull_request_codecommit:main"
 
+[tool.semantic_release]
+version_variable = [
+    "pull_request_codecommit/__init__.py:__version__",
+    "pyproject.toml:version"
+]
+branch = "main"
+upload_to_pypi = true
+upload_to_release = true
+build_command = "pip install poetry && poetry build"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

