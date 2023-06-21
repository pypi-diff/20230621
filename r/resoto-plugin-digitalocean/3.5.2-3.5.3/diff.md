# Comparing `tmp/resoto-plugin-digitalocean-3.5.2.tar.gz` & `tmp/resoto-plugin-digitalocean-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.5.2.tar", last modified: Tue Jun 13 13:11:38 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.5.3.tar", last modified: Wed Jun 21 14:23:34 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.5.2.tar` & `resoto-plugin-digitalocean-3.5.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.988960 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43638 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.988960 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:08:56.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43858 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:52.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/neighbor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25525 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.5.2/PKG-INFO` & `resoto-plugin-digitalocean-3.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.5.2/pyproject.toml` & `resoto-plugin-digitalocean-3.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean"
 description = "Resoto DigitalOcean Collector Plugin"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.2",
+    "resotolib==3.5.3",
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from typing import Optional, List, Tuple
+from typing import Optional, List, Tuple, cast
 
 from resoto_plugin_digitalocean.client import StreamingWrapper, get_team_credentials
 from resoto_plugin_digitalocean.collector import DigitalOceanTeamCollector
 from resoto_plugin_digitalocean.resources import DigitalOceanResource, DigitalOceanTeam
-from resoto_plugin_digitalocean.config import DigitalOceanCollectorConfig
+from resoto_plugin_digitalocean.config import (
+    DigitalOceanCollectorConfig,
+    DigitalOceanTeamCredentials,
+    DigitalOceanSpacesKeys,
+)
 from resoto_plugin_digitalocean.utils import dump_tag
 from resotolib.config import Config
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.core.actions import CoreFeedback
 from resotolib.logger import log
 from resotolib.graph import Graph
 from resotolib.baseresources import BaseResource
@@ -26,43 +30,65 @@
 
         It is responsible for querying the cloud APIs for remote resources and adding
         them to the plugin graph.
         The graph root (self.graph.root) must always be followed by one or more
         accounts. An account must always be followed by a region.
         A region can contain arbitrary resources.
         """
-        tokens = Config.digitalocean.api_tokens
-        spaces_access_keys: List[str] = Config.digitalocean.spaces_access_keys
-        spaces_keys: List[Tuple[Optional[str], Optional[str]]] = []
+
         assert self.core_feedback, "core_feedback is not set"  # will be set by the outer collector plugin
 
-        def spaces_keys_valid(keys: List[str]) -> bool:
-            return all([len(key.split(":")) == 2 for key in keys])
+        def from_legacy_config() -> List[DigitalOceanTeamCredentials]:
+            tokens: List[str] = Config.digitalocean.api_tokens
+            spaces_access_keys: List[str] = Config.digitalocean.spaces_access_keys
+            spaces_keys: List[Tuple[Optional[str], Optional[str]]] = []
+
+            def spaces_keys_valid(keys: List[str]) -> bool:
+                return all([len(key.split(":")) == 2 for key in keys])
+
+            if not spaces_keys_valid(spaces_access_keys):
+                log.warning("DigitalOcean Spaces access keys must be provided in pairs of access_key:secret_key")
+            else:
+
+                def key_to_tuple(key: str) -> Tuple[str, str]:
+                    splitted = key.split(":")
+                    return splitted[0], splitted[1]
+
+                spaces_keys = [key_to_tuple(key) for key in spaces_access_keys]
+
+            if len(tokens) != len(spaces_access_keys):
+                log.warning(
+                    "The number of DigitalOcean API tokens and DigitalOcean Spaces access keys must be equal."
+                    + "Missing or extra spaces access keys will be ignored."
+                )
+                spaces_keys = spaces_keys[: len(tokens)]
+                spaces_keys.extend([(None, None)] * (len(tokens) - len(spaces_keys)))
+
+            result = []
+            for token, space_key_tuple in zip(tokens, spaces_keys):
+                if (access_key := space_key_tuple[0]) and (secret_key := space_key_tuple[1]):
+                    keys = DigitalOceanSpacesKeys(access_key=access_key, secret_key=secret_key)
+                else:
+                    keys = None
+                result.append(DigitalOceanTeamCredentials(api_token=token, spaces_keys=keys))
+
+            return result
 
-        if not spaces_keys_valid(spaces_access_keys):
-            log.warn("DigitalOcean Spaces access keys must be provided in pairs of access_key:secret_key")
+        if credentials_conf := Config.digitalocean.credentials:
+            credentials = cast(List[DigitalOceanTeamCredentials], credentials_conf)
         else:
+            credentials = from_legacy_config()
 
-            def key_to_tuple(key: str) -> Tuple[str, str]:
-                splitted = key.split(":")
-                return splitted[0], splitted[1]
-
-            spaces_keys = [key_to_tuple(key) for key in spaces_access_keys]
-
-        if len(tokens) != len(spaces_access_keys):
-            log.warn(
-                "The number of DigitalOcean API tokens and DigitalOcean Spaces access keys must be equal."
-                + "Missing or extra spaces access keys will be ignored."
+        log.info(f"plugin: collecting DigitalOcean resources for {len(credentials)} teams")
+        for c in credentials:
+            client = StreamingWrapper(
+                c.api_token,
+                c.spaces_keys.access_key if c.spaces_keys else None,
+                c.spaces_keys.secret_key if c.spaces_keys else None,
             )
-            spaces_keys = spaces_keys[: len(tokens)]
-            spaces_keys.extend([(None, None)] * (len(tokens) - len(spaces_keys)))
-
-        log.info(f"plugin: collecting DigitalOcean resources for {len(tokens)} teams")
-        for token, space_key_tuple in zip(tokens, spaces_keys):
-            client = StreamingWrapper(token, space_key_tuple[0], space_key_tuple[1])
             team_graph = self.collect_team(client, self.core_feedback.with_context("digitalocean"))
             if team_graph:
                 self.graph.merge(team_graph)
 
     def collect_team(self, client: StreamingWrapper, feedback: CoreFeedback) -> Optional[Graph]:
         """Collects an individual team."""
         team_id = client.get_team_id()
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             url = urljoin(self.do_api_endpoint, url)
             log.debug(f"fetching {url}")
             json_response = validate_status(requests.get(url, headers=self.headers, allow_redirects=True)).json()
             payload = json_response.get(payload_object_name, [])
             result.extend(payload if isinstance(payload, list) else [payload])
 
         log.debug(f"DO request {path} returned {len(result)} items")
+        result = [item for item in result if item is not None]
         return result
 
     @retry
     def delete(self, path: str, resource_id: Optional[str]) -> bool:
         resource_id_path = f"/{resource_id}" if resource_id else ""
         url = f"{self.do_api_endpoint}{path}{resource_id_path}"
         log.debug(f"deleting {url}")
@@ -151,14 +152,19 @@
 
     def list_project_resources(self, project_id: str) -> List[Json]:
         return self._fetch(f"/projects/{project_id}/resources", "resources")
 
     def list_droplets(self) -> List[Json]:
         return self._fetch("/droplets", "droplets")
 
+    def list_droplets_neighbors_ids(self) -> List[List[str]]:
+        json_obj = self._fetch("/reports/droplet_neighbors_ids", "neighbor_ids")
+        result = [[str(id) for id in droplet_ids] for droplet_ids in json_obj if isinstance(droplet_ids, list)]
+        return result
+
     def list_regions(self) -> List[Json]:
         return self._fetch("/regions", "regions")
 
     def list_volumes(self) -> List[Json]:
         return self._fetch("/volumes", "volumes")
 
     def list_databases(self) -> List[Json]:
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from typing import Tuple, Type, List, Dict, Callable, Any, Optional, cast
 
 from prometheus_client import Summary
 
 from resotolib.baseresources import BaseResource, EdgeType, InstanceStatus, VolumeStatus
 from resotolib.graph import Graph
 from resotolib.types import Json
+from hashlib import sha256
 from .client import StreamingWrapper
 from .resources import (
     DigitalOceanDroplet,
     DigitalOceanDropletSize,
+    DigitalOceanDropletNeighborhood,
     DigitalOceanProject,
     DigitalOceanRegion,
     DigitalOceanTeam,
     DigitalOceanVolume,
     DigitalOceanDatabase,
     DigitalOceanVPC,
     DigitalOceanKubernetesCluster,
@@ -27,15 +29,14 @@
     DigitalOceanApp,
     DigitalOceanCdnEndpoint,
     DigitalOceanCertificate,
     DigitalOceanContainerRegistry,
     DigitalOceanContainerRegistryRepository,
     DigitalOceanContainerRegistryRepositoryTag,
     DigitalOceanSSHKey,
-    DigitalOceanTag,
     DigitalOceanDomain,
     DigitalOceanDomainRecord,
     DigitalOceanFirewall,
     DigitalOceanAlertPolicy,
 )
 from .utils import (
     iso2datetime,
@@ -56,20 +57,21 @@
     app_id,
     cdn_endpoint_id,
     certificate_id,
     container_registry_id,
     container_registry_repository_id,
     container_registry_repository_tag_id,
     ssh_key_id,
-    tag_id,
     domain_id,
     domain_record_id,
     firewall_id,
     alert_policy_id,
     parse_tag,
+    parse_tags,
+    droplet_neighborhood_id,
 )
 
 log = logging.getLogger("resoto." + __name__)
 
 metrics_collect_projects = Summary(
     "resoto_plugin_digitalocean_collect_projects_seconds",
     "Time it took the collect_projects() method",
@@ -130,18 +132,15 @@
     "resoto_plugin_digitalocean_collect_container_registry_seconds",
     "Time it took the collect_container_registry() method",
 )
 metrics_collect_ssh_keys = Summary(
     "resoto_plugin_digitalocean_collect_ssh_keys_seconds",
     "Time it took the collect_ssh_keys() method",
 )
-metrics_collect_tags = Summary(
-    "resoto_plugin_digitalocean_collect_tags_seconds",
-    "Time it took the collect_tags() method",
-)
+
 metrics_collect_domains = Summary(
     "resoto_plugin_digitalocean_collect_domains_seconds",
     "Time it took the collect_domains() method",
 )
 metrics_collect_domains_records = Summary(
     "resoto_plugin_digitalocean_collect_domains_records_seconds",
     "Time it took the collect_domains_records() method",
@@ -180,15 +179,14 @@
         # they were included by --do-collect or excluded by --do-no-collect
         self.mandatory_collectors: List[Tuple[str, Callable[..., None]]] = [("regions", self.collect_regions)]
         # Global collectors are resources that are either specified on a global level
         # as opposed to a per zone or per region level or they are zone/region
         # resources that provide a aggregatedList() function returning all resources
         # for all zones/regions.
         self.global_collectors: List[Tuple[str, Callable[..., None]]] = [
-            ("tags", self.collect_tags),
             ("vpcs", self.collect_vpcs),
             ("instances", self.collect_droplets),
             ("volumes", self.collect_volumes),
             ("databases", self.collect_databases),
             ("k8s_clusters", self.collect_k8s_clusters),
             ("snapshots", self.collect_snapshots),
             ("load_balancers", self.collect_load_balancers),
@@ -268,15 +266,16 @@
 
         # The following are default attributes that are passed to every
         # BaseResource() if found in `result`
         def extract_tags(result: Dict[str, Any]) -> Dict[str, Optional[str]]:
             raw_tags = result.get("tags", [])
             raw_tags = raw_tags if raw_tags else []
             tags = [parse_tag(tag) for tag in raw_tags if tag]
-            return dict(tags) if tags else {}
+            tags_ = [tag for tag in tags if tag]
+            return dict(tags_) if tags_ else {}
 
         kwargs = {
             "id": str(result.get("id")),
             "tags": extract_tags(result),
             "name": result.get("name"),
             "ctime": iso2datetime(result.get("created_at")),
             "mtime": iso2datetime(result.get("updated_at")),
@@ -454,24 +453,18 @@
                 "image_slug": "slug",
                 "is_public": "public",
                 "min_disk_size": "min_disk_size",
                 "image_type": "type",
                 "size_gigabytes": lambda image: int(math.ceil(image.get("size_gigabytes"))),
                 "description": "description",
                 "image_status": "status",
+                "tags": lambda image: parse_tags(image.get("tags", []) or []),
             },
             search_map={
                 "_region": ["urn", lambda image: region_id(image["region"])],
-                "__tags": [
-                    "urn",
-                    lambda image: list(map(lambda tag: tag_id(tag), image.get("tags", []) or [])),
-                ],
-            },
-            predecessors={
-                EdgeType.default: ["__tags"],
             },
         )
 
         def get_size(droplet: Json) -> Json:
             size = droplet["size"]
             size["region"] = droplet["region"]["slug"]
             return cast(Json, size)
@@ -505,39 +498,70 @@
             instances,
             resource_class=DigitalOceanDroplet,
             attr_map={
                 "id": lambda i: str(i["id"]),
                 "urn": lambda d: droplet_id(d["id"]),
                 "instance_status": lambda d: instance_status_map.get(d["status"], InstanceStatus.UNKNOWN),
                 "instance_cores": "vcpus",
+                "instance_type": "size_slug",
                 "instance_memory": lambda d: d["memory"] / 1024.0,
                 "droplet_backup_ids": lambda d: list(map(str, d.get("backup_ids", []) or [])),
                 "is_locked": "locked",
                 "droplet_features": "features",
                 "droplet_image": lambda d: d["image"]["slug"],
+                "tags": lambda instance: parse_tags(instance.get("tags", []) or []),
             },
             search_map={
                 "_region": [
                     "urn",
                     lambda droplet: region_id(droplet["region"]["slug"]),
                 ],
                 "__vpcs": ["urn", lambda droplet: vpc_id(droplet["vpc_uuid"])],
                 "__images": ["urn", lambda droplet: image_id(droplet["image"]["id"])],
                 "__sizes": ["urn", lambda droplet: size_id(droplet["size"]["slug"])],
-                "__tags": [
-                    "urn",
-                    lambda d: list(map(lambda tag: tag_id(tag), d.get("tags", []))),
-                ],
             },
             predecessors={
-                EdgeType.default: ["__vpcs", "__images", "__sizes", "__tags"],
+                EdgeType.default: ["__vpcs", "__images", "__sizes"],
                 EdgeType.delete: ["__vpcs"],
             },
         )
 
+        neighborhoods = self.client.list_droplets_neighbors_ids()
+        neighbors_json = []
+        for neighbors in neighborhoods:
+            m = sha256()
+            neighbors = sorted(neighbors)
+            m.update(DigitalOceanDropletNeighborhood.kind.encode())
+            for droplet in neighbors or []:
+                m.update(droplet.encode())
+            id = m.hexdigest()[0:16]
+            neighbors_json.append(
+                {
+                    "droplets": neighbors,
+                    "id": id,
+                }
+            )
+        instances_to_region = {str(droplet["id"]): region_id(droplet["region"]["slug"]) for droplet in instances}
+        self.collect_resource(
+            neighbors_json,
+            resource_class=DigitalOceanDropletNeighborhood,
+            attr_map={
+                "id": "id",
+                "urn": lambda n: droplet_neighborhood_id(n["id"]),
+                "droplets": "droplets",
+            },
+            search_map={
+                "_region": ["urn", lambda neighbor: instances_to_region[neighbor["droplets"][0]]],
+                "__droplets": ["urn", lambda neighbor: [droplet_id(id) for id in neighbor["droplets"]]],
+            },
+            successors={
+                EdgeType.default: ["__droplets"],
+            },
+        )
+
     @metrics_collect_regions.time()
     def collect_regions(self) -> None:
         regions = self.client.list_regions()
         self.collect_resource(
             regions,
             resource_class=DigitalOceanRegion,
             attr_map={
@@ -569,26 +593,23 @@
                 "urn": lambda r: volume_id(r["id"]),
                 "volume_size": "size_gigabytes",
                 "description": "description",
                 "filesystem_type": "filesystem_type",
                 "filesystem_label": "filesystem_label",
                 "volume_status": extract_volume_status,
                 "ondemand_cost": lambda v: v["size_gigabytes"] * DO_VOLUME_COST_GB_PER_HOUR,
+                "tags": lambda volume: parse_tags(volume.get("tags", []) or []),
             },
             search_map={
                 "__users": [
                     "urn",
                     lambda vol: list(map(lambda id: droplet_id(id), vol["droplet_ids"])),
                 ],
-                "__tags": [
-                    "urn",
-                    lambda v: list(map(lambda tag: tag_id(tag), v.get("tags", []) or [])),
-                ],
             },
-            predecessors={EdgeType.default: ["__users", "__tags"]},
+            predecessors={EdgeType.default: ["__users"]},
             successors={EdgeType.delete: ["__users"]},
         )
 
     @metrics_collect_databases.time()
     def collect_databases(self) -> None:
         # this mapping was taken from the digitalocean web console.
         dbtype_to_size = {
@@ -623,25 +644,22 @@
                 "name": lambda db: database_id(db["name"]),
                 "db_type": "engine",
                 "db_status": "status",
                 "db_version": "version",
                 "db_endpoint": lambda db: db.get("connection", {}).get("host", ""),
                 "instance_type": "size",
                 "volume_size": lambda db: dbtype_to_size.get(db.get("size", ""), 0),
+                "tags": lambda db: parse_tags(db.get("tags", []) or []),
             },
             search_map={
                 "_region": ["urn", lambda db: region_id(db["region"])],
                 "__vpcs": ["urn", lambda db: vpc_id(db["private_network_uuid"])],
-                "__tags": [
-                    "urn",
-                    lambda db: list(map(lambda tag: tag_id(tag), db.get("tags", []) or [])),
-                ],
             },
             predecessors={
-                EdgeType.default: ["__vpcs", "__tags"],
+                EdgeType.default: ["__vpcs"],
                 EdgeType.delete: ["__vpcs"],
             },
         )
 
     @metrics_collect_vpcs.time()
     def collect_vpcs(self) -> None:
         vpcs = self.client.list_vpcs()
@@ -754,28 +772,25 @@
             attr_map={
                 "id": lambda s: str(s["id"]),
                 "urn": lambda s: snapshot_id(s["id"]),
                 "volume_size": lambda vol: vol["min_disk_size"],
                 "snapshot_size_gigabytes": lambda vol: int(math.ceil(vol.get("size_gigabytes"))),
                 "resource_id": "resource_id",
                 "resource_type": "resource_type",
+                "tags": lambda s: parse_tags(s.get("tags", []) or []),
             },
             search_map={
                 "_region": ["urn", lambda s: get_region(s)],
                 "__available_regions": [
                     "urn",
                     lambda s: [region_id(region) for region in s["regions"]],
                 ],
                 "__resource": ["urn", lambda s: get_resource_id(s)],
-                "__tags": [
-                    "urn",
-                    lambda s: list(map(lambda tag: tag_id(tag), s.get("tags", []) or [])),
-                ],
             },
-            predecessors={EdgeType.default: ["__resource", "__tags", "__available_regions"]},
+            predecessors={EdgeType.default: ["__resource", "__available_regions"]},
         )
 
     @metrics_collect_load_balancers.time()
     def collect_load_balancers(self) -> None:
         loadbalancers = self.client.list_load_balancers()
 
         def get_nr_nodes(lb: Json) -> int:
@@ -1009,26 +1024,14 @@
                 "id": lambda k: str(k["id"]),
                 "urn": lambda k: ssh_key_id(k["id"]),
                 "public_key": "public_key",
                 "fingerprint": "fingerprint",
             },
         )
 
-    @metrics_collect_tags.time()
-    def collect_tags(self) -> None:
-        tags = self.client.list_tags()
-        self.collect_resource(
-            tags,
-            resource_class=DigitalOceanTag,
-            attr_map={
-                "id": "name",
-                "urn": lambda t: tag_id(t["name"]),
-            },
-        )
-
     @metrics_collect_domains.time()
     def collect_domains(self) -> None:
         domains = self.client.list_domains()
         self.collect_resource(
             domains,
             resource_class=DigitalOceanDomain,
             attr_map={
@@ -1077,27 +1080,21 @@
         self.collect_resource(
             firewalls,
             resource_class=DigitalOceanFirewall,
             attr_map={
                 "id": "id",
                 "urn": lambda f: firewall_id(f["id"]),
                 "firewall_status": "status",
+                "tags": lambda f: parse_tags(f.get("tags", []) or []),
             },
             search_map={
                 "__droplets": [
                     "urn",
                     lambda f: list(map(lambda id: droplet_id(id), f.get("droplet_ids", []) or [])),
                 ],
-                "__tags": [
-                    "urn",
-                    lambda f: list(map(lambda id: tag_id(id), f.get("tags", []) or [])),
-                ],
-            },
-            predecessors={
-                EdgeType.default: ["__tags"],
             },
             successors={
                 EdgeType.default: ["__droplets"],
             },
         )
 
     @metrics_collect_alert_policies.time()
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,22 @@
     BaseBucket,
     BaseEndpoint,
     BaseCertificate,
     BaseKeyPair,
     BaseDNSZone,
     BaseDNSRecord,
     ModelReference,
+    PhantomBaseResource,
 )
 from resotolib.graph import Graph
 import time
 
+from resotolib.types import Json
+from resotolib.json import to_json as _to_json
+
 log = logging.getLogger("resoto." + __name__)
 
 
 @define(eq=False, slots=False)
 class DigitalOceanResource(BaseResource):
     """A class that implements the abstract method delete() as well as update_tag()
     and delete_tag().
@@ -66,14 +70,17 @@
                 credentials.spaces_access_key,
                 credentials.spaces_secret_key,
             )
             return client.delete(delete_uri_path, self.id)
 
         raise NotImplementedError
 
+    def to_json(self) -> Json:
+        return _to_json(self, strip_nulls=True, keep_untouched=set(["tags"]))
+
 
 @define(eq=False, slots=False)
 class DigitalOceanTeam(DigitalOceanResource, BaseAccount):
     """DigitalOcean Team"""
 
     kind: ClassVar[str] = "digitalocean_team"
     reference_kinds: ClassVar[ModelReference] = {
@@ -98,15 +105,14 @@
                 "digitalocean_vpc",
                 "digitalocean_project",
                 "digitalocean_region",
                 "digitalocean_resource",
                 "digitalocean_snapshot",
                 "digitalocean_space",
                 "digitalocean_ssh_key",
-                "digitalocean_tag",
                 "digitalocean_volume",
             ],
             "delete": [],
         }
     }
 
 
@@ -223,14 +229,25 @@
         return "/droplets"
 
     def tag_resource_name(self) -> Optional[str]:
         return "droplet"
 
 
 @define(eq=False, slots=False)
+class DigitalOceanDropletNeighborhood(DigitalOceanResource, PhantomBaseResource):
+    """A DigitalOcean Droplet Neighborhood Resource
+
+    Represents a physical hardware server where droplets can be placed.
+    """
+
+    kind: ClassVar[str] = "digitalocean_droplet_neighborhood"
+    droplets: Optional[List[str]] = None
+
+
+@define(eq=False, slots=False)
 class DigitalOceanKubernetesCluster(DigitalOceanResource, BaseResource):
     """DigitalOcean Kubernetes Cluster"""
 
     kind: ClassVar[str] = "digitalocean_kubernetes_cluster"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
             "default": ["digitalocean_droplet"],
@@ -564,24 +581,14 @@
     public_key: Optional[str] = None
 
     def delete_uri_path(self) -> Optional[str]:
         return "/account/keys"
 
 
 @define(eq=False, slots=False)
-class DigitalOceanTag(DigitalOceanResource, BaseResource):
-    """DigitalOcean tag"""
-
-    kind = "digitalocean_tag"
-
-    def delete_uri_path(self) -> Optional[str]:
-        return "/tags"
-
-
-@define(eq=False, slots=False)
 class DigitalOceanDomain(DigitalOceanResource, BaseDNSZone):
     """DigitalOcean domain"""
 
     kind = "digitalocean_domain"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
             "default": ["digitalocean_domain_record"],
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from datetime import datetime
-from typing import Union, Callable, Any, Dict, Optional, Tuple
+from typing import Union, Callable, Any, Dict, Optional, Tuple, List
 
 
 log = logging.getLogger("resoto." + __name__)
 
 
 def get_result_data(result: Dict[str, Any], value: Union[str, Callable[..., Any]]) -> Any:
     """Returns data from a DO API call result dict.
@@ -142,25 +142,38 @@
     return f"do:firewall:{value}"
 
 
 def alert_policy_id(value: str) -> str:
     return f"do:alert:{value}"
 
 
+def droplet_neighborhood_id(value: str) -> str:
+    return f"do:neighborhood:{value}"
+
+
 tag_value_sep: str = "--"
 
 
-def parse_tag(tag: str) -> Tuple[str, Optional[str]]:
-    if tag_value_sep in tag:
-        tag_parts = tag.split("--", 1)
-        key = tag_parts[0]
-        value = tag_parts[1] if len(tag_parts) > 1 else None
-        return (key, value)
-    else:
-        return (tag, None)
+def parse_tag(tag: str) -> Optional[Tuple[str, Optional[str]]]:
+    splitted = iter(tag.split(tag_value_sep, 1))
+    key = next(splitted, None)
+    if key is None:
+        return None
+    value = next(splitted, None)
+    return (key, value)
+
+
+def parse_tags(tags: List[str]) -> Dict[str, Optional[str]]:
+    parsed_tags = {}
+    for tag in tags:
+        if parsed_tag := parse_tag(tag):
+            key, value = parsed_tag
+            parsed_tags[key] = value
+
+    return parsed_tags
 
 
 def dump_tag(key: str, value: Optional[str]) -> str:
     if value and len(value) > 0:
         return f"{key}{tag_value_sep}{value}"
     else:
         return f"{key}"
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 test/fixtures/domain_records.py
 test/fixtures/domains.py
 test/fixtures/droplets.py
 test/fixtures/firewalls.py
 test/fixtures/floatingip.py
 test/fixtures/k8s.py
 test/fixtures/loadbalancers.py
+test/fixtures/neighbor_ids.py
 test/fixtures/projectresources.py
 test/fixtures/projects.py
 test/fixtures/regions.py
 test/fixtures/registry.py
 test/fixtures/registry_repositories.py
 test/fixtures/registry_repository_tags.py
 test/fixtures/snapshots.py
```

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # flake8: noqa F401
 from .droplets import droplets as droplets
+from .neighbor_ids import neighbor_ids as neighbor_ids
 from .regions import regions as regions
 from .volumes import volumes as volumes
 from .vpcs import vpcs as vpcs
 from .databases import databases as databases
 from .k8s import k8s as k8s
 from .snapshots import snapshots as snapshots
 from .loadbalancers import load_balancers as load_balancers
```

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.5.3/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.2/test/test_collector.py` & `resoto-plugin-digitalocean-3.5.3/test/test_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,27 @@
     DigitalOceanApp,
     DigitalOceanCdnEndpoint,
     DigitalOceanCertificate,
     DigitalOceanContainerRegistry,
     DigitalOceanContainerRegistryRepositoryTag,
     DigitalOceanContainerRegistryRepository,
     DigitalOceanSSHKey,
-    DigitalOceanTag,
     DigitalOceanDomain,
     DigitalOceanDomainRecord,
     DigitalOceanFirewall,
     DigitalOceanAlertPolicy,
+    DigitalOceanDropletNeighborhood,
 )
 from resotolib.baseresources import Cloud, EdgeType, GraphRoot, InstanceStatus, VolumeStatus
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 from resotolib.graph import sanitize
 from .fixtures import (
     droplets,
+    neighbor_ids,
     regions,
     volumes,
     vpcs,
     databases,
     k8s,
     snapshots,
     load_balancers,
@@ -166,30 +167,29 @@
 def test_collect_droplets() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_droplets": droplets,
             "list_vpcs": vpcs,
             "list_tags": tags,
+            "list_droplets_neighbors_ids": neighbor_ids,
         }
     )
     graph = prepare_graph(do_client)
 
     check_edges(graph, "do:region:fra1", "do:droplet:289110074")
     check_edges(graph, "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959", "do:droplet:289110074")
     check_edges(
         graph,
         "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959",
         "do:droplet:289110074",
         delete=True,
     )
     check_edges(graph, "do:image:101111514", "do:droplet:289110074")
     check_edges(graph, "do:size:s-1vcpu-1gb", "do:droplet:289110074")
-    check_edges(graph, "do:tag:image_tag", "do:image:101111514")
-    check_edges(graph, "do:tag:droplet_tag", "do:droplet:289110074")
     image: DigitalOceanImage = graph.search_first("urn", "do:image:101111514")  # type: ignore
     assert image.urn == "do:image:101111514"
     assert image.name == "20.04 (LTS) x64"
     assert image.distribution == "Ubuntu"
     assert image.image_slug == "ubuntu-20-04-x64"
     assert image.is_public is True
     assert image.image_type == "base"
@@ -204,47 +204,56 @@
     assert size.instance_cores == 1
     assert size.instance_memory == 1
     assert size.ondemand_cost == 0.00744
 
     droplet: DigitalOceanDroplet = graph.search_first("urn", "do:droplet:289110074")  # type: ignore
     assert droplet.urn == "do:droplet:289110074"
     assert droplet.name == "ubuntu-s-1vcpu-1gb-fra1-01"
+    assert droplet.instance_type == "s-1vcpu-1gb"
     assert droplet.instance_memory == 1
     assert droplet.instance_cores == 1
     assert droplet.instance_status == InstanceStatus.RUNNING
     assert droplet.region().urn == "do:region:fra1"  # type: ignore
     assert droplet.droplet_image == "ubuntu-20-04-x64"
     assert droplet.droplet_backup_ids == ["42"]
     assert droplet.is_locked is False
     assert droplet.ctime == datetime.datetime(2022, 3, 3, 16, 26, 55, tzinfo=datetime.timezone.utc)
     assert droplet.tags == {"droplet_tag": None}
 
+    neighborhood: DigitalOceanDropletNeighborhood = graph.search_first(
+        "kind", DigitalOceanDropletNeighborhood.kind
+    )  # type: ignore
+    assert neighborhood.droplets == ["289110074", "290075243"]
+    check_edges(graph, neighborhood.urn, "do:droplet:289110074")
+    check_edges(graph, neighborhood.urn, "do:droplet:290075243")
+    check_edges(graph, "do:region:fra1", neighborhood.urn)
+
 
 def test_collect_volumes() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_droplets": droplets,
             "list_volumes": volumes,
             "list_tags": tags,
         }
     )
     graph = prepare_graph(do_client)
 
     check_edges(graph, "do:droplet:289110074", "do:volume:631f81d2-9fc1-11ec-800c-0a58ac14d197")
-    check_edges(graph, "do:tag:volume_tag", "do:volume:631f81d2-9fc1-11ec-800c-0a58ac14d197")
     volume = cast(DigitalOceanVolume, graph.search_first("urn", "do:volume:631f81d2-9fc1-11ec-800c-0a58ac14d197"))
     assert volume.urn == "do:volume:631f81d2-9fc1-11ec-800c-0a58ac14d197"
     assert volume.name == "volume-fra1-01"
     assert volume.description == "Test volume"
     assert volume.filesystem_type == "ext4"
     assert volume.filesystem_label == "label"
     assert volume.volume_size == 1
     assert volume.volume_status == VolumeStatus.IN_USE
     assert volume.ondemand_cost == 0.000149
+    assert volume.tags == {"volume_tag": None}
 
 
 def test_collect_database() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_databases": databases,
@@ -261,24 +270,24 @@
     )
     check_edges(
         graph,
         "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959",
         "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397",
         delete=True,
     )
-    check_edges(graph, "do:tag:database_tag", "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397")
     database: DigitalOceanDatabase = graph.search_first("urn", "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397")  # type: ignore # noqa: E501
     assert database.urn == "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397"
     assert database.name == "do:dbaas:db-postgresql-fra1-82725"
     assert database.db_type == "pg"
     assert database.db_status == "online"
     assert database.db_version == "14"
     assert database.db_endpoint == "host.b.db.ondigitalocean.com"
     assert database.region().urn == "do:region:fra1"  # type: ignore
     assert database.instance_type == "db-s-1vcpu-1gb"
+    assert database.tags == {"database_tag": None}
 
 
 def test_collect_k8s_clusters() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_vpcs": vpcs,
@@ -329,21 +338,21 @@
             "list_snapshots": snapshots,
             "list_tags": tags,
         }
     )
     graph = prepare_graph(do_client)
 
     check_edges(graph, "do:droplet:289110074", "do:snapshot:103198134")
-    check_edges(graph, "do:tag:snapshot_tag", "do:snapshot:103198134")
     snapshot: DigitalOceanSnapshot = graph.search_first("urn", "do:snapshot:103198134")  # type: ignore
     assert snapshot.urn == "do:snapshot:103198134"
     assert snapshot.volume_size == 25
     assert snapshot.snapshot_size_gigabytes == 2
     assert snapshot.resource_id == "289110074"
     assert snapshot.resource_type == "droplet"
+    assert snapshot.tags == {"snapshot_tag": None}
 
 
 def test_collect_loadbalancers() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_load_balancers": load_balancers,
@@ -587,26 +596,14 @@
     ssh_key: DigitalOceanSSHKey = graph.search_first("urn", "do:ssh_key:289794")  # type: ignore
     assert ssh_key.urn == "do:ssh_key:289794"
     assert ssh_key.fingerprint == "3b:16:e4:bf:8b:00:8b:b8:59:8c:a9:d3:f0:19:fa:45"
     assert ssh_key.name == "Other Public Key"
     assert ssh_key.public_key == "ssh-rsa publickey keycomment"
 
 
-def test_collect_tags() -> None:
-    do_client = ClientMock(
-        {
-            "list_regions": regions,
-            "list_tags": tags,
-        }
-    )
-    graph = prepare_graph(do_client)
-    tag: DigitalOceanTag = graph.search_first("urn", "do:tag:droplet_tag")  # type: ignore
-    assert tag.urn == "do:tag:droplet_tag"
-
-
 def test_collect_domains() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_domains": domains,
             "list_domain_records": domain_records,
         }
@@ -641,23 +638,23 @@
             "list_regions": regions,
             "list_firewalls": firewalls,
             "list_droplets": droplets,
             "list_tags": tags,
         }
     )
     graph = prepare_graph(do_client)
-    check_edges(graph, "do:tag:firewall_tag", "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711")
     check_edges(
         graph,
         "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711",
         "do:droplet:289110074",
     )
     firewall: DigitalOceanFirewall = graph.search_first("urn", "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711")  # type: ignore # noqa: E501
     assert firewall.firewall_status == "succeeded"
     assert firewall.ctime == datetime.datetime(2022, 3, 10, 13, 10, 50, 0, datetime.timezone.utc)
+    assert firewall.tags == {"firewall_tag": None}
 
 
 def test_alert_policies() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_alert_policies": alerts,
```

