# Comparing `tmp/harvey-cd-0.23.0.tar.gz` & `tmp/harvey-cd-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harvey-cd-0.23.0.tar", last modified: Thu Mar 30 05:51:15 2023, max compression
+gzip compressed data, was "harvey-cd-0.24.0.tar", last modified: Tue Jun 20 22:26:40 2023, max compression
```

## Comparing `harvey-cd-0.23.0.tar` & `harvey-cd-0.24.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.902322 harvey-cd-0.23.0/harvey/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.906322 harvey-cd-0.23.0/harvey/repos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/repos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/repos/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/repos/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/repos/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/repos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.906322 harvey-cd-0.23.0/harvey/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/utils/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/harvey/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.906322 harvey-cd-0.23.0/harvey_cd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 05:51:15.000000 harvey-cd-0.23.0/harvey_cd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.898322 harvey-cd-0.23.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/test/unit/repos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/repos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/repos/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/test_webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:51:15.910322 harvey-cd-0.23.0/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-30 05:50:26.000000 harvey-cd-0.23.0/test/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.490586 harvey-cd-0.24.0/harvey/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.490586 harvey-cd-0.24.0/harvey/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/repos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/repos/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/repos/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/repos/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/repos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.490586 harvey-cd-0.24.0/harvey/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/utils/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/harvey/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.490586 harvey-cd-0.24.0/harvey_cd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 22:26:40.000000 harvey-cd-0.24.0/harvey_cd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.486586 harvey-cd-0.24.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/test/unit/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/repos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/repos/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/test_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:26:40.494586 harvey-cd-0.24.0/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-20 22:25:37.000000 harvey-cd-0.24.0/test/unit/utils/test_utils.py
```

### Comparing `harvey-cd-0.23.0/LICENSE` & `harvey-cd-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/PKG-INFO` & `harvey-cd-0.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harvey-cd
-Version: 0.23.0
+Version: 0.24.0
 Summary: The lightweight Docker Compose deployment platform.
 Home-page: http://github.com/justintime50/harvey
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -78,14 +78,15 @@
 ### Things to Know
 
 - Harvey will shallow clone your project to the most recent commit
 - Harvey expects the container name to match the GitHub repository name exactly, otherwise the healthcheck will fail
 - Harvey does not handle renamed or transferred repos for you. If you rename a repo, you may need to intervene manually to shut down the old container, remove it from Harvey, and startup the new one initially on your own
 - Initial deployments are not gracefully handled. Because Harvey requires no configuration for a project, it assumes everything is already setup on the server. This means that on an initial deploy, you will need to set environment variables on your server, migrate databases, and whatever else may be required, at which point you may need to redeploy the project for the changes to take affect
 - Harvey automatically rotates log files and keeps them for 2 weeks before purging them
+- Because we use threads, you cannot kill an ongoing deployment because you cannot reliably kill a thread
 
 ### Harvey Configuration
 
 #### Configuration Criteria
 
 - Each repo either needs a `.harvey.yml` file in the root directory stored in git (which will be used whenever a GitHub webhook fires) or a `data` key passed into the webhook delivered to Harvey (via something like GitHub Actions). This can be accomplished by using something like [workflow-webhook](https://github.com/distributhor/workflow-webhook) or another homegrown solution (requires the entire webhook payload from GitHub. Harvey will always fallback to the `.harvey.yml` file if there is no `data` key present)
 - You can specify one of `deploy` or `pull` as the `deployment_type` to run (`deploy` is the default)
@@ -177,14 +178,15 @@
 - `/deploy` (POST) - Deploy a project with data from a GitHub webhook
 - `/projects` (GET) - Retrieve a list of projects
 - `/projects/{project_name}/lock` (PUT) - Locks the deployments of a project
 - `/projects/{project_name}/unlock` (PUT) - Unlocks the deployments of a project
 - `/projects/{project_name}/webhook` (GET) - Retrieves the current webhook of a project
 - `/locks` (GET) - Retrieve a list of locks
 - `/locks/{project_name}` (GET) - Retrieve the lock status of a project
+- `/threads` (GET) - Retrieves a list of threads (named after projects) running via Harvey. A thread indicates an ongoing deployment
 
 #### Example API Calls
 
 ```bash
 # Retrieve a list of deployments
 curl -X GET http://127.0.0.1:5000/deployments
```

### Comparing `harvey-cd-0.23.0/README.md` & `harvey-cd-0.24.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 ### Things to Know
 
 - Harvey will shallow clone your project to the most recent commit
 - Harvey expects the container name to match the GitHub repository name exactly, otherwise the healthcheck will fail
 - Harvey does not handle renamed or transferred repos for you. If you rename a repo, you may need to intervene manually to shut down the old container, remove it from Harvey, and startup the new one initially on your own
 - Initial deployments are not gracefully handled. Because Harvey requires no configuration for a project, it assumes everything is already setup on the server. This means that on an initial deploy, you will need to set environment variables on your server, migrate databases, and whatever else may be required, at which point you may need to redeploy the project for the changes to take affect
 - Harvey automatically rotates log files and keeps them for 2 weeks before purging them
+- Because we use threads, you cannot kill an ongoing deployment because you cannot reliably kill a thread
 
 ### Harvey Configuration
 
 #### Configuration Criteria
 
 - Each repo either needs a `.harvey.yml` file in the root directory stored in git (which will be used whenever a GitHub webhook fires) or a `data` key passed into the webhook delivered to Harvey (via something like GitHub Actions). This can be accomplished by using something like [workflow-webhook](https://github.com/distributhor/workflow-webhook) or another homegrown solution (requires the entire webhook payload from GitHub. Harvey will always fallback to the `.harvey.yml` file if there is no `data` key present)
 - You can specify one of `deploy` or `pull` as the `deployment_type` to run (`deploy` is the default)
@@ -162,14 +163,15 @@
 - `/deploy` (POST) - Deploy a project with data from a GitHub webhook
 - `/projects` (GET) - Retrieve a list of projects
 - `/projects/{project_name}/lock` (PUT) - Locks the deployments of a project
 - `/projects/{project_name}/unlock` (PUT) - Unlocks the deployments of a project
 - `/projects/{project_name}/webhook` (GET) - Retrieves the current webhook of a project
 - `/locks` (GET) - Retrieve a list of locks
 - `/locks/{project_name}` (GET) - Retrieve the lock status of a project
+- `/threads` (GET) - Retrieves a list of threads (named after projects) running via Harvey. A thread indicates an ongoing deployment
 
 #### Example API Calls
 
 ```bash
 # Retrieve a list of deployments
 curl -X GET http://127.0.0.1:5000/deployments
```

### Comparing `harvey-cd-0.23.0/harvey/api.py` & `harvey-cd-0.24.0/harvey/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,46 +71,48 @@
         message = 'Server-side error.'
         status_code = 500
         payload_json = request.json
         payload_data = request.data  # We need this to properly decode the webhook secret
         signature = request.headers.get('X-Hub-Signature-256')
 
         if payload_json:
-            logger.info(f'Webhook received for: {Webhook.repo_full_name(payload_json)}')
+            repo_full_name = Webhook.repo_full_name(payload_json)
+            logger.info(f'Webhook received for: {repo_full_name}')
 
             # The `ref` field from GitHub looks like `refs/heads/main`, so we split on the final
             # slash to get the branch name and check against the user-allowed list of branches.
             branch_name = payload_json['ref'].rsplit('/', 1)[-1]
             tag_commit = 'refs/tags'
 
             if Config.webhook_secret and not Webhook.validate_webhook_secret(payload_data, signature):
                 message = 'The X-Hub-Signature did not match the WEBHOOK_SECRET.'
                 status_code = 403
             elif (branch_name in Config.allowed_branches) or (
                 Config.deploy_on_tag and tag_commit in payload_json['ref']
             ):
                 Thread(
+                    name=repo_full_name,
                     target=Deployment.run_deployment,
                     args=(payload_json,),
                 ).start()
 
-                message = f'Started deployment for {Webhook.repo_full_name(payload_json)}'
+                message = f'Started deployment for {repo_full_name}'
                 status_code = 200
                 success = True
 
                 logger.info(message)
 
                 update_webhook(
-                    project_name=Webhook.repo_full_name(payload_json),
+                    project_name=repo_full_name,
                     webhook=payload_json,
                 )
             else:
                 message = (
                     'Harvey received a webhook event for a branch that is not included in the'
-                    f' ALLOWED_BRANCHES for {Webhook.repo_full_name(payload_json)}.'
+                    f' ALLOWED_BRANCHES for {repo_full_name}.'
                 )
                 status_code = 422
 
                 logger.error(message)
         else:
             message = 'Malformed or missing JSON data in webhook.'
             status_code = 422
```

### Comparing `harvey-cd-0.23.0/harvey/app.py` & `harvey-cd-0.24.0/harvey/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import subprocess  # nosec
-from threading import Thread
+import threading
 from typing import (
     Any,
     Dict,
     Optional,
 )
 
 import requests_unixsocket  # type: ignore
@@ -162,15 +162,16 @@
 def redeploy_project_endpoint(project_name):
     """Redeploy a project based on local webhook data stored in the database from a previous deploy."""
     try:
         webhook = retrieve_webhook(project_name)
         if not webhook:
             raise HarveyError(f'Webhook does not exist for {project_name}')
         else:
-            Thread(
+            threading.Thread(
+                name=project_name,
                 target=Deployment.run_deployment,
                 args=(webhook,),
             ).start()
             return create_response_dict(
                 f'Redeploying {project_name}...',
                 success=True,
                 status_code=200,
@@ -241,28 +242,39 @@
     try:
         return retrieve_lock(project_name)
     except Exception as error:
         log_error(error)
         return abort(404)
 
 
+@APP.route('/threads', methods=['GET'])
+@Api.check_api_key
+def retrieve_threads_endpoint():
+    """Retrieves a list of running threads for Harvey. Threads indicate ongoing deployments."""
+    threads = []
+    for thread in threading.enumerate():
+        threads.append(thread.name)
+
+    return {'threads': threads}
+
+
 def bootstrap(debug_mode):
     """Bootstrap the Harvey instance on startup.
 
     Any task required for Harvey to work that only needs to be instantiated once should go here.
     """
     setup_logger()
 
     # Ensure the correct Docker Compose version is available
     docker_compose_version = subprocess.check_output(  # nosec
         ['docker-compose', '--version'],
-        stdin=None,
-        stderr=None,
+        stderr=subprocess.STDOUT,
+        text=True,
         timeout=3,
-    ).decode('UTF-8')
+    )
     if REQUIRED_DOCKER_COMPOSE_VERSION not in docker_compose_version:
         raise HarveyError(f'Harvey requires Docker Compose {REQUIRED_DOCKER_COMPOSE_VERSION}.')
 
     # Setup Sentry
     if Config.sentry_url:
         sentry_sdk.init(
             Config.sentry_url,
```

### Comparing `harvey-cd-0.23.0/harvey/config.py` & `harvey-cd-0.24.0/harvey/config.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/containers.py` & `harvey-cd-0.24.0/harvey/containers.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import docker  # type: ignore
 import woodchips
 
 from harvey.config import Config
 from harvey.errors import HarveyError
 from harvey.utils.deployments import kill_deployment
+from harvey.utils.utils import get_utc_timestamp
 
 
 class Container:
     @staticmethod
     def create_client():
         """Creates a Docker client to use for connections."""
         logger = woodchips.get(Config.logger_name)
@@ -112,15 +113,15 @@
         """Determines if the container was recently restarted or not within the last minute by getting the
         difference of datetimes between now and the container's start time. If it's greater than 60 seconds,
         we know the container didn't restart with this deploy.
 
         Docker appears to store dates in RFC 3339 Nano and UTC time so we chop off the ending digits and
         convert to a Python datetime here for comparison.
         """
-        now = datetime.datetime.now(datetime.timezone.utc)
+        now = get_utc_timestamp()
         container_start_datetime = datetime.datetime.strptime(
             container_dictionary['attrs']['State'].get('StartedAt', '')[:-4], '%Y-%m-%dT%H:%M:%S.%f'
         ).replace(tzinfo=datetime.timezone.utc)
         container_age_difference = now - container_start_datetime
 
         grace_period_seconds = 60.0
         container_restarted_recently = container_age_difference.total_seconds() <= grace_period_seconds
```

### Comparing `harvey-cd-0.23.0/harvey/deployments.py` & `harvey-cd-0.24.0/harvey/deployments.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     lookup_project_lock,
     update_project_lock,
 )
 from harvey.utils.deployments import (
     kill_deployment,
     succeed_deployment,
 )
+from harvey.utils.utils import get_utc_timestamp
 from harvey.webhooks import Webhook
 
 
 class Deployment:
     @staticmethod
     def initialize_deployment(webhook: Dict[str, Any]) -> Tuple[Dict[str, Any], str, datetime.datetime]:
         """Initialize the setup for a deployment by cloning or pulling the project
@@ -44,15 +45,15 @@
                         ' deployments.'
                     ),
                     webhook,
                 )
         except Exception:
             logger.error('Could not determine project lock status!')
 
-        start_time = datetime.datetime.utcnow()
+        start_time = get_utc_timestamp()
 
         _ = update_project_lock(
             project_name=Webhook.repo_full_name(webhook),
             locked=True,
             system_lock=True,
         )
         store_deployment_details(webhook)
@@ -72,36 +73,35 @@
         if deployment_type not in Config.supported_deployments:
             kill_deployment(
                 message='Harvey could not run since there was no acceptable deployment specified.',
                 webhook=webhook,
             )
 
         deployment_started_message = (
-            f'{Message.work_emoji} Harvey has started a deployment ({deployment_type}) for'
-            f' `{Webhook.repo_full_name(webhook)}`.'
+            f'{Message.work_emoji} Harvey started a {deployment_type} for `{Webhook.repo_full_name(webhook)}`.'
         )
         if Config.use_slack:
             Message.send_slack_message(deployment_started_message)
 
         preamble = (
-            f'Harvey v{Config.harvey_version} ({deployment_type.title()} Deployment)\n'
+            f'{Webhook.repo_full_name(webhook)} {deployment_type.title()}\n'
+            f'Harvey: v{Config.harvey_version}\n'
             f'Deployment Started: {start_time}\n'
             f'Deployment ID: {Webhook.repo_commit_id(webhook)}'
         )
         logger.info(preamble)
 
-        configuration = f'Configuration:\n{json.dumps(config, indent=4)}' if Config.log_level == 'DEBUG' else ''
-        commit_details = (
-            f'New commit by: {Webhook.repo_commit_author(webhook)} to {Webhook.repo_full_name(webhook)}.\n'
-            f'Commit Details: {Webhook.repo_commit_message(webhook)}'
-        )
-        git_output = git if Config.log_level == 'DEBUG' else ''
-        execution_time = f'Startup execution time: {datetime.datetime.utcnow() - start_time}'
+        configuration = f'\n\nConfiguration:\n{json.dumps(config, indent=4)}' if Config.log_level == 'DEBUG' else ''
+        commit_details = f'Commit author: {Webhook.repo_commit_author(webhook)}'
+        if Config.log_level == 'DEBUG':
+            commit_details += f'\nCommit Details: {Webhook.repo_commit_message(webhook)}'
+        git_output = f'\n\n{git}' if Config.log_level == 'DEBUG' else ''
+        execution_time = f'Startup execution time: {get_utc_timestamp() - start_time}'
 
-        output = f'{preamble}\n\n{configuration}\n\n{commit_details}\n\n{git_output}\n\n{execution_time}'
+        output = f'{preamble}{configuration}\n\n{commit_details}{git_output}\n\n{execution_time}'
         logger.debug(f'{Webhook.repo_full_name(webhook)} {execution_time}')
 
         return config, output, start_time
 
     @staticmethod
     def run_deployment(webhook: Dict[str, Any]):
         """After receiving a webhook, spin up a deployment based on the config.
@@ -113,15 +113,15 @@
             webhook_config, webhook_output, start_time = Deployment.initialize_deployment(webhook)
             deployment = webhook_config.get('deployment_type', Config.default_deployment).lower()
 
             if deployment == 'deploy':
                 deploy_output = Deployment.deploy(webhook_config, webhook, webhook_output)
 
                 healthcheck = webhook_config.get('healthcheck')
-                healthcheck_messages = 'Healthchecks:\n'
+                healthcheck_messages = ''
                 docker_client = Container.create_client()
 
                 if healthcheck:
                     container_healthcheck_statuses = {}
                     for container in healthcheck:
                         container_healthcheck = Container.run_container_healthcheck(docker_client, container, webhook)
                         container_healthcheck_statuses[container] = container_healthcheck
@@ -132,15 +132,15 @@
                         healthcheck_messages += healthcheck_message
 
                     healthcheck_values = container_healthcheck_statuses.values()
                     all_healthchecks_passed = any(healthcheck_values) and list(healthcheck_values)[0] is True
                 else:
                     all_healthchecks_passed = True  # Set to true here since we cannot determine, won't kill the deploy
 
-                end_time = datetime.datetime.utcnow()
+                end_time = get_utc_timestamp()
                 execution_time = f'Deployment execution time: {end_time - start_time}'
                 logger.debug(f'{Webhook.repo_full_name(webhook)} {execution_time}')
                 final_output = f'{webhook_output}\n{deploy_output}\n{execution_time}\n{healthcheck_messages}\n'
 
                 if all_healthchecks_passed or not healthcheck:
                     succeed_deployment(final_output, webhook)
                 else:
@@ -158,15 +158,15 @@
                 succeed_deployment(final_output, webhook)
             else:
                 kill_deployment(f'deployment_type invalid, must be one of {Config.supported_deployments}', webhook)
         except Exception as error:
             # We wrap this entire block in a try/catch in an attempt to catch anything that bubbles to the
             # top before hitting sentry as this function is the top-level function called when a thread has
             # been spawned.
-            kill_deployment(f'Deployment failed: {error}.', webhook)
+            kill_deployment(str(error), webhook)
 
     @staticmethod
     def open_project_config(webhook: Dict[str, Any]):
         """Open the project's config file to assign deployment variables.
 
         Project configs look like the following:
         {
@@ -205,15 +205,15 @@
     def deploy(config: Dict[str, Any], webhook: Dict[str, Any], output: str) -> str:
         """Build Stage, used for `deploy` deployments.
 
         This flow doesn't use the Docker API but instead runs `docker compose` commands.
         """
         logger = woodchips.get(Config.logger_name)
 
-        start_time = datetime.datetime.utcnow()
+        start_time = get_utc_timestamp()
 
         repo_path = os.path.join(Config.projects_path, Webhook.repo_full_name(webhook))
 
         docker_compose_yml = 'docker-compose.yml'
         docker_compose_yaml = 'docker-compose.yaml'
         docker_compose_prod_yml = 'docker-compose-prod.yml'
         docker_compose_prod_yaml = 'docker-compose-prod.yaml'
@@ -247,49 +247,46 @@
                 'docker',
                 'compose',
                 '-f', default_compose_filepath,
                 '-f', prod_compose_filepath,
                 'up', '-d',
                 '--build',
                 '--force-recreate',
-                '--quiet-pull',
             ]
             # fmt: on
         else:
             # fmt: off
             compose_command = [
                 'docker',
                 'compose',
                 '-f', default_compose_filepath,
                 'up', '-d',
                 '--build',
                 '--force-recreate',
-                '--quiet-pull',
             ]
             # fmt: on
 
         try:
             compose_output = subprocess.check_output(  # nosec
                 compose_command,
-                stdin=None,
-                stderr=None,
+                stderr=subprocess.STDOUT,
+                text=True,
                 timeout=Config.operation_timeout,
             )
-            decoded_output = compose_output.decode('UTF-8')
-            execution_time = f'Deploy stage execution time: {datetime.datetime.utcnow() - start_time}'
-            final_output = f'{decoded_output}\n{execution_time}'
+            execution_time = f'Deploy stage execution time: {get_utc_timestamp() - start_time}'
+            final_output = f'{compose_output}\n{execution_time}'
             logger.info(final_output)
         except subprocess.TimeoutExpired:
             final_output = 'Harvey timed out deploying!'
             kill_deployment(
                 message=final_output,
                 webhook=webhook,
             )
         except subprocess.CalledProcessError as error:
-            final_output = f'{output}\nHarvey could not finish the deploy: {error}'
+            final_output = f'{output}\nHarvey could not finish the deploy: {error.output}'
             kill_deployment(
                 message=final_output,
                 webhook=webhook,
                 raise_error=True,
             )
 
         return final_output
```

### Comparing `harvey-cd-0.23.0/harvey/git.py` & `harvey-cd-0.24.0/harvey/git.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,82 +26,79 @@
 
         return output
 
     @staticmethod
     def clone_repo(project_path: str, webhook: Dict[str, Any]) -> str:
         """Clone a repo into the Harvey projects folder."""
         logger = woodchips.get(Config.logger_name)
-        decoded_output = ''
+        command_output = ''
 
         try:
             command = ['git', 'clone', '--depth=1', Webhook.repo_url(webhook), project_path]
             command_output = Git._git_subprocess(command)
-            decoded_output = command_output.decode()
-            logger.debug(decoded_output)
+            logger.debug(command_output)
         except subprocess.TimeoutExpired:
             kill_deployment(
                 message='Harvey timed out during git clone operation.',
                 webhook=webhook,
             )
         except subprocess.CalledProcessError as error:
-            final_output = f'Harvey could not clone due to error: {error} {Webhook.repo_full_name(webhook)}.'
+            final_output = f'Harvey could not clone due to error: {error.output} {Webhook.repo_full_name(webhook)}.'
             kill_deployment(
                 message=final_output,
                 webhook=webhook,
                 raise_error=True,
             )
 
-        return decoded_output
+        return command_output
 
     @staticmethod
     def pull_repo(project_path: str, webhook: Dict[str, Any], pull_attempt: int = 1) -> str:
         """Pull updates for a repo in the Harvey projects folder."""
         logger = woodchips.get(Config.logger_name)
-        decoded_output = ''
+        command_output = ''
 
         try:
             command = ['git', '-C', project_path, 'pull', '--rebase']
             command_output = Git._git_subprocess(command)
-            decoded_output = command_output.decode()
-            logger.debug(f'{decoded_output}')
+            logger.debug(f'{command_output}')
         except subprocess.TimeoutExpired:
             kill_deployment(
                 message='Harvey timed out during git pull operation.',
                 webhook=webhook,
             )
         except subprocess.CalledProcessError:
             # The biggest offender of this operation failing is local, uncommitted changes.
             # Try stashing and retry again before failing.
             logger.error(f'Harvey could not pull {Webhook.repo_full_name(webhook)}.')
             logger.info(f'Attempting to stash {Webhook.repo_full_name(webhook)} before pulling again...')
 
             try:
                 command = ['git', '-C', project_path, 'stash']
                 command_output = Git._git_subprocess(command)
-                decoded_output = command_output.decode()
-                logger.debug(f'{decoded_output}')
+                logger.debug(f'{command_output}')
             except (subprocess.CalledProcessError, subprocess.TimeoutExpired):
                 kill_deployment(
                     message='Harvey could not stash local changes!',
                     webhook=webhook,
                     raise_error=True,
                 )
 
             # Recursively call this function again so we can try pulling after a stash when we fail the first time.
             # Must use an int here vs bool so we don't have an infinite loop.
             if pull_attempt == 1:
                 pull_attempt += 1
-                decoded_output = Git.pull_repo(project_path, webhook, pull_attempt)
+                command_output = Git.pull_repo(project_path, webhook, pull_attempt)
 
-        return decoded_output
+        return command_output
 
     @staticmethod
-    def _git_subprocess(command: List[str]) -> bytes:
+    def _git_subprocess(command: List[str]) -> str:
         """Runs a git command via subprocess."""
         command_output = subprocess.check_output(  # nosec
             command,
-            stdin=None,
-            stderr=None,
+            stderr=subprocess.STDOUT,
+            text=True,
             timeout=Config.operation_timeout,
         )
 
         return command_output
```

### Comparing `harvey-cd-0.23.0/harvey/locks.py` & `harvey-cd-0.24.0/harvey/locks.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/messages.py` & `harvey-cd-0.24.0/harvey/messages.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/repos/deployments.py` & `harvey-cd-0.24.0/harvey/repos/deployments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import datetime
 from typing import (
     Any,
     Dict,
     List,
 )
 
 import flask
 import woodchips
 from sqlitedict import SqliteDict  # type: ignore
 
 from harvey.config import Config
 from harvey.errors import HarveyError
 from harvey.utils.api_utils import get_page_size
+from harvey.utils.utils import get_utc_timestamp
 from harvey.webhooks import Webhook
 
 
 DATABASE_TABLE_NAME = 'deployments'
 
 
 def store_deployment_details(webhook: Dict[str, Any], final_output: str = 'NA'):
@@ -24,28 +24,30 @@
     A project ID consists of the `project_name@commit_id`.
     """
     logger = woodchips.get(Config.logger_name)
 
     logger.debug(f'Storing deployment details for {Webhook.repo_full_name(webhook)}...')
 
     with SqliteDict(filename=Config.database_file, tablename=DATABASE_TABLE_NAME) as database_table:
-        # Naively check the logs for an indicator of the status being success
-        if 'success' in final_output.lower() or 'succeeded' in final_output.lower():
+        if 'deployment succeeded' in final_output.lower():
             deployment_status = 'Success'
         elif final_output == 'NA':
             deployment_status = 'In-Progress'
         else:
             deployment_status = 'Failure'
 
-        now = str(datetime.datetime.utcnow())
+        now = str(get_utc_timestamp())
+
+        deployment_runtime = final_output.partition('Deployment execution time: ')[2].split('\n\n')[0]
 
         attempt: Dict[str, Any] = {
             'log': final_output,
             'status': deployment_status,
             'timestamp': now,
+            'runtime': deployment_runtime if deployment_runtime else None,
         }
 
         if database_table.get(Webhook.deployment_id(webhook)):
             attempts = database_table[Webhook.deployment_id(webhook)].get('attempts', [])
         else:
             attempts = []
 
@@ -72,14 +74,16 @@
 
 def retrieve_deployment(deployment_id: str) -> Dict[str, Any]:
     """Retrieve a deployment's details from a given `deployment_id`."""
     with SqliteDict(filename=Config.database_file, tablename=DATABASE_TABLE_NAME) as database_table:
         for key, value in database_table.items():
             transformed_key = key.split('@')
             if deployment_id == f'{transformed_key[0]}-{transformed_key[1]}':
+                if value.get('attempts'):
+                    value['attempts'] = sorted(value['attempts'], key=lambda x: x['attempt'], reverse=True)
                 return value
 
     raise HarveyError(f'Could not retrieve deployment details for {deployment_id}!')
 
 
 def retrieve_deployments(request: flask.Request) -> Dict[str, List[Any]]:
     """Retrieve a list of deployments until the pagination limit is reached."""
@@ -88,17 +92,21 @@
     page_size = get_page_size(request)
     project_name = request.args.get('project')
 
     with SqliteDict(filename=Config.database_file, tablename=DATABASE_TABLE_NAME) as database_table:
         for _, value in database_table.items():
             # If a project name is provided, only return deployments for that project
             if project_name and value['project'] == project_name:
+                if value.get('attempts'):
+                    value['attempts'] = sorted(value['attempts'], key=lambda x: x['attempt'], reverse=True)
                 deployments['deployments'].append(value)
             # This block is for a generic list of deployments (all deployments)
             elif not project_name:
+                if value.get('attempts'):
+                    value['attempts'] = sorted(value['attempts'], key=lambda x: x['attempt'], reverse=True)
                 deployments['deployments'].append(value)
             # If a project name was specified but doesn't match, don't add to list
             else:
                 pass
 
     sorted_deployments = sorted(deployments['deployments'], key=lambda i: i['timestamp'], reverse=True)[:page_size]
     deployments['total_count'] = len(
```

### Comparing `harvey-cd-0.23.0/harvey/repos/locks.py` & `harvey-cd-0.24.0/harvey/repos/locks.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/repos/projects.py` & `harvey-cd-0.24.0/harvey/repos/projects.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/repos/webhooks.py` & `harvey-cd-0.24.0/harvey/repos/webhooks.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey/utils/deployments.py` & `harvey-cd-0.24.0/harvey/utils/deployments.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 from harvey.webhooks import Webhook
 
 
 def kill_deployment(message: str, webhook: Dict[str, Any], raise_error: Optional[bool] = False):
     """Log output, send message, and cleanup on deployment failure."""
     logger = woodchips.get(Config.logger_name)
 
-    error_message = f'{Webhook.repo_full_name(webhook)} deployment failed: {message}'
-    logger.error(error_message)
+    error_message = f'{Message.failure_emoji} `{Webhook.repo_full_name(webhook)}` deployment failed!'
+    logger.error(_strip_emojis_from_logs(error_message))
 
-    store_deployment_details(webhook, _strip_emojis_from_logs(error_message))
+    deployment_logs = error_message + '\n' + message
+    store_deployment_details(webhook, _strip_emojis_from_logs(deployment_logs))
 
     if Config.use_slack:
         Message.send_slack_message(error_message)
 
     # Only unlock deployments that were locked by the system and not a user to preserve their preferences
     deployment_lock = lookup_project_lock(project_name=Webhook.repo_full_name(webhook))
     if deployment_lock.get('system_lock'):
@@ -41,22 +42,22 @@
     sys.exit(1)
 
 
 def succeed_deployment(message: str, webhook: Dict[str, Any]):
     """Log output, send message, and cleanup on deployment success."""
     logger = woodchips.get(Config.logger_name)
 
-    success_message = f'{Webhook.repo_full_name(webhook)} deployment succeeded!'
-    logger.info(success_message)
+    success_message = f'{Message.success_emoji} `{Webhook.repo_full_name(webhook)}` deployment succeeded!'
+    logger.info(_strip_emojis_from_logs(success_message))
 
-    deployment_logs = message + success_message
+    deployment_logs = success_message + '\n' + message
     store_deployment_details(webhook, _strip_emojis_from_logs(deployment_logs))
 
     if Config.use_slack:
-        Message.send_slack_message(deployment_logs)
+        Message.send_slack_message(success_message)
 
     _ = update_project_lock(project_name=Webhook.repo_full_name(webhook), locked=False)
 
     sys.exit(1)
 
 
 def _strip_emojis_from_logs(output: str) -> str:
```

### Comparing `harvey-cd-0.23.0/harvey/utils/utils.py` & `harvey-cd-0.24.0/harvey/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 import woodchips
 
 from harvey.config import Config
 
 
 def format_project_name(project_name: str) -> str:
     """Formats a project name for use throughout Harvey."""
@@ -15,7 +17,12 @@
     will also log directly to uWSGI's logs so we don't do that to avoid double logging.
     """
     logger = woodchips.Logger(
         name=Config.logger_name,
         level=Config.log_level,
     )
     logger.log_to_console(formatter='%(asctime)s - %(module)s.%(funcName)s - %(levelname)s - %(message)s')
+
+
+def get_utc_timestamp():
+    """Returns the UTC timestamp of right now."""
+    return datetime.datetime.now(datetime.timezone.utc)
```

### Comparing `harvey-cd-0.23.0/harvey/webhooks.py` & `harvey-cd-0.24.0/harvey/webhooks.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/harvey_cd.egg-info/PKG-INFO` & `harvey-cd-0.24.0/harvey_cd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harvey-cd
-Version: 0.23.0
+Version: 0.24.0
 Summary: The lightweight Docker Compose deployment platform.
 Home-page: http://github.com/justintime50/harvey
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -78,14 +78,15 @@
 ### Things to Know
 
 - Harvey will shallow clone your project to the most recent commit
 - Harvey expects the container name to match the GitHub repository name exactly, otherwise the healthcheck will fail
 - Harvey does not handle renamed or transferred repos for you. If you rename a repo, you may need to intervene manually to shut down the old container, remove it from Harvey, and startup the new one initially on your own
 - Initial deployments are not gracefully handled. Because Harvey requires no configuration for a project, it assumes everything is already setup on the server. This means that on an initial deploy, you will need to set environment variables on your server, migrate databases, and whatever else may be required, at which point you may need to redeploy the project for the changes to take affect
 - Harvey automatically rotates log files and keeps them for 2 weeks before purging them
+- Because we use threads, you cannot kill an ongoing deployment because you cannot reliably kill a thread
 
 ### Harvey Configuration
 
 #### Configuration Criteria
 
 - Each repo either needs a `.harvey.yml` file in the root directory stored in git (which will be used whenever a GitHub webhook fires) or a `data` key passed into the webhook delivered to Harvey (via something like GitHub Actions). This can be accomplished by using something like [workflow-webhook](https://github.com/distributhor/workflow-webhook) or another homegrown solution (requires the entire webhook payload from GitHub. Harvey will always fallback to the `.harvey.yml` file if there is no `data` key present)
 - You can specify one of `deploy` or `pull` as the `deployment_type` to run (`deploy` is the default)
@@ -177,14 +178,15 @@
 - `/deploy` (POST) - Deploy a project with data from a GitHub webhook
 - `/projects` (GET) - Retrieve a list of projects
 - `/projects/{project_name}/lock` (PUT) - Locks the deployments of a project
 - `/projects/{project_name}/unlock` (PUT) - Unlocks the deployments of a project
 - `/projects/{project_name}/webhook` (GET) - Retrieves the current webhook of a project
 - `/locks` (GET) - Retrieve a list of locks
 - `/locks/{project_name}` (GET) - Retrieve the lock status of a project
+- `/threads` (GET) - Retrieves a list of threads (named after projects) running via Harvey. A thread indicates an ongoing deployment
 
 #### Example API Calls
 
 ```bash
 # Retrieve a list of deployments
 curl -X GET http://127.0.0.1:5000/deployments
```

### Comparing `harvey-cd-0.23.0/harvey_cd.egg-info/SOURCES.txt` & `harvey-cd-0.24.0/harvey_cd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/setup.py` & `harvey-cd-0.24.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 REQUIREMENTS = [
-    'docker == 6.0.*',
+    'docker == 6.1.*',
     'flask == 2.*',
     'python-dotenv == 0.21.*',
     'pyyaml == 6.*',
     'requests == 2.*',
     'requests_unixsocket == 0.3.*',
     'sentry-sdk == 1.*',
     'slackclient == 2.*',
@@ -31,15 +31,15 @@
     'types-PyYAML',
     'types-requests',
     'wheel == 0.40.*',
 ]
 
 setuptools.setup(
     name='harvey-cd',
-    version='0.23.0',
+    version='0.24.0',
     description='The lightweight Docker Compose deployment platform.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/harvey',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
```

### Comparing `harvey-cd-0.23.0/test/unit/conftest.py` & `harvey-cd-0.24.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/repos/deployments.py` & `harvey-cd-0.24.0/test/unit/repos/deployments.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/test_api.py` & `harvey-cd-0.24.0/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/test_app.py` & `harvey-cd-0.24.0/test/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/test_containers.py` & `harvey-cd-0.24.0/test/unit/test_containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import datetime
 from unittest.mock import (
     Mock,
     patch,
 )
 
 from harvey.containers import Container
+from harvey.utils.utils import get_utc_timestamp
 
 
-MOCK_RFC_3339_TIME = datetime.datetime.now(datetime.timezone.utc).isoformat()[:-4]
+MOCK_RFC_3339_TIME = get_utc_timestamp().isoformat()[:-4]
 
 
 @patch('logging.Logger.debug')
 @patch('docker.from_env')
 def test_create_client(mock_client, mock_logger):
     _ = Container.create_client()
```

### Comparing `harvey-cd-0.23.0/test/unit/test_deployments.py` & `harvey-cd-0.24.0/test/unit/test_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import datetime
 import subprocess
 from unittest.mock import (
     ANY,
     mock_open,
     patch,
 )
 
 from harvey.deployments import Deployment
+from harvey.utils.utils import get_utc_timestamp
 
 
 MOCK_OUTPUT = 'mock output'
-MOCK_TIME = datetime.datetime.utcnow()
+MOCK_TIME = get_utc_timestamp()
 
 
 def mock_config(deployment_type='deploy', prod_compose=False):
     """A mock configuration object similar to what would be stored in `harvey.yaml`."""
     mock_config = {
         'deployment': deployment_type,
         'prod_compose': prod_compose,
@@ -149,18 +149,17 @@
             'compose',
             '-f',
             ANY,
             'up',
             '-d',
             '--build',
             '--force-recreate',
-            '--quiet-pull',
         ],
-        stdin=None,
-        stderr=None,
+        stderr=-2,
+        text=True,
         timeout=300,
     )
 
 
 @patch('os.path.exists', return_value=True)
 @patch('harvey.deployments.kill_deployment')
 @patch('subprocess.check_output', side_effect=subprocess.TimeoutExpired(cmd='subprocess.check_output', timeout=0.1))
@@ -169,15 +168,15 @@
 
     mock_utils_kill.assert_called_once()
 
 
 @patch('os.path.exists', return_value=True)
 @patch('harvey.deployments.kill_deployment')
 @patch(
-    'subprocess.check_output', side_effect=subprocess.CalledProcessError(returncode=1, cmd='subprocess.check_output')
+    'subprocess.check_output', side_effect=subprocess.CalledProcessError(cmd='subprocess.check_output', returncode=1)
 )
 def test_deploy_stage_subprocess_error(mock_subprocess, mock_utils_kill, mock_path_exists, mock_webhook):  # noqa
     _ = Deployment.deploy(mock_config('deploy'), dict(mock_webhook), MOCK_OUTPUT)
 
     mock_utils_kill.assert_called_once()
 
 
@@ -197,13 +196,12 @@
             ANY,
             '-f',
             ANY,
             'up',
             '-d',
             '--build',
             '--force-recreate',
-            '--quiet-pull',
         ],
-        stdin=None,
-        stderr=None,
+        stderr=-2,
+        text=True,
         timeout=300,
     )
```

### Comparing `harvey-cd-0.23.0/test/unit/test_git.py` & `harvey-cd-0.24.0/test/unit/test_git.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 @patch('subprocess.check_output')
 def test_clone_repo(mock_subprocess, mock_logger, mock_project_path, mock_webhook):
     Git.clone_repo(mock_project_path, mock_webhook)
 
     mock_logger.assert_called()
     mock_subprocess.assert_called_once_with(
         ['git', 'clone', '--depth=1', 'https://test-url.com', 'harvey/projects/test_user/test-repo-name'],
-        stdin=None,
-        stderr=None,
+        stderr=-2,
+        text=True,
         timeout=300,
     )
 
 
 @patch('harvey.git.kill_deployment')
 @patch('subprocess.check_output', side_effect=subprocess.TimeoutExpired(cmd='subprocess.check_output', timeout=0.1))
 def test_clone_repo_subprocess_timeout(mock_subprocess, mock_utils_kill, mock_project_path, mock_webhook):
     Git.clone_repo(mock_project_path, mock_webhook)
 
     mock_utils_kill.assert_called_once()
 
 
 @patch('harvey.git.kill_deployment')
 @patch(
-    'subprocess.check_output', side_effect=subprocess.CalledProcessError(returncode=1, cmd='subprocess.check_output')
+    'subprocess.check_output', side_effect=subprocess.CalledProcessError(cmd='subprocess.check_output', returncode=1)
 )
 def test_clone_repo_process_error(mock_subprocess, mock_utils_kill, mock_project_path, mock_webhook):
     Git.clone_repo(mock_project_path, mock_webhook)
 
     mock_utils_kill.assert_called_once()
 
 
@@ -57,31 +57,31 @@
 @patch('subprocess.check_output')
 def test_pull_repo(mock_subprocess, mock_logger, mock_project_path, mock_webhook):
     Git.pull_repo(mock_project_path, mock_webhook)
 
     mock_logger.assert_called()
     mock_subprocess.assert_called_once_with(
         ['git', '-C', 'harvey/projects/test_user/test-repo-name', 'pull', '--rebase'],
-        stdin=None,
-        stderr=None,
+        stderr=-2,
+        text=True,
         timeout=300,
     )
 
 
 @patch('harvey.git.kill_deployment')
 @patch('subprocess.check_output', side_effect=subprocess.TimeoutExpired(cmd='subprocess.check_output', timeout=0.1))
 def test_pull_repo_subprocess_timeout(mock_subprocess, mock_utils_kill, mock_project_path, mock_webhook):
     Git.pull_repo(mock_project_path, mock_webhook)
 
     mock_utils_kill.assert_called_once()
 
 
 @patch('harvey.git.kill_deployment')
 @patch(
-    'subprocess.check_output', side_effect=subprocess.CalledProcessError(returncode=1, cmd='subprocess.check_output')
+    'subprocess.check_output', side_effect=subprocess.CalledProcessError(cmd='subprocess.check_output', returncode=1)
 )
 def test_pull_repo_process_error(mock_subprocess, mock_utils_kill, mock_project_path, mock_webhook):
     # TODO: We need to test here that the `stash` command gets called, unsure how to do this since
     # we first have to make `subprocess.check_output` fail then run it again - mocking that
     # in a test seems difficult
     Git.pull_repo(mock_project_path, mock_webhook)
```

### Comparing `harvey-cd-0.23.0/test/unit/test_messages.py` & `harvey-cd-0.24.0/test/unit/test_messages.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/test_webhooks.py` & `harvey-cd-0.24.0/test/unit/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `harvey-cd-0.23.0/test/unit/utils/test_utils.py` & `harvey-cd-0.24.0/test/unit/utils/test_utils.py`

 * *Files identical despite different names*

