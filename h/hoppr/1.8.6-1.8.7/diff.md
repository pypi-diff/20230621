# Comparing `tmp/hoppr-1.8.6.tar.gz` & `tmp/hoppr-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.6.tar", max compression
+gzip compressed data, was "hoppr-1.8.7.tar", max compression
```

## Comparing `hoppr-1.8.6.tar` & `hoppr-1.8.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-06-14 22:06:45.000000 hoppr-1.8.6/LICENSE
--rw-r--r--   0        0        0     1214 2023-06-14 22:06:45.000000 hoppr-1.8.6/README.md
--rw-r--r--   0        0        0     1035 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11010 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10697 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10272 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     4387 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4113 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6368 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7961 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4418 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5673 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4606 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/in_toto.py
--rw-r--r--   0        0        0     3357 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17448 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/py.typed
--rw-r--r--   0        0        0     4018 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5023 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    27309 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-06-14 22:06:45.000000 hoppr-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-21 21:07:06.000000 hoppr-1.8.7/LICENSE
+-rw-r--r--   0        0        0     1214 2023-06-21 21:07:06.000000 hoppr-1.8.7/README.md
+-rw-r--r--   0        0        0     1035 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11010 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10697 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10932 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4387 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     4113 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6368 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7961 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4833 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5673 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4606 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3357 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17448 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/py.typed
+-rw-r--r--   0        0        0     4018 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5023 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    27309 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-06-21 21:07:06.000000 hoppr-1.8.7/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-06-21 21:07:06.000000 hoppr-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.7/PKG-INFO
```

### Comparing `hoppr-1.8.6/LICENSE` & `hoppr-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/README.md` & `hoppr-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/__init__.py` & `hoppr-1.8.7/hoppr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.6"
+__version__ = "1.8.7"
```

### Comparing `hoppr-1.8.6/hoppr/base_plugins/collector.py` & `hoppr-1.8.7/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.7/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/cli/hopctl.py` & `hoppr-1.8.7/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/constants.py` & `hoppr-1.8.7/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.7/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import requests
 
 from packageurl import PackageURL
 from requests.auth import HTTPBasicAuth
 
 import hoppr.net
+import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import BatchCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
@@ -40,20 +41,18 @@
         artifact_string = ".".join([artifact_string, purl.qualifiers.get("arch")])
 
     return artifact_string
 
 
 def _is_rpm_repo(repo_url: str) -> bool:
     url = RepositoryUrl(url=repo_url) / "repodata/repomd.xml"
-
     basic_auth = None
     creds = Credentials.find(repo_url)
     if creds is not None:
         basic_auth = HTTPBasicAuth(username=creds.username, password=creds.password.get_secret_value())
-
     for attempt in range(3):
         if attempt > 0:
             sleep(5)
 
         resp = requests.get(f"{url}", auth=basic_auth, allow_redirects=False, stream=True, verify=True, timeout=60)
         if resp.status_code < 300:
             return True
@@ -73,14 +72,26 @@
         if pattern in parsed_url.netloc or fnmatch.fnmatch(name=parsed_url.netloc, pat=pattern):
             proxy = "_none_"
             break
 
     return proxy
 
 
+def _clear_cache(search_root: Path):
+    """
+    Clear the cache for a given Path.
+    """
+    temp_paths = list(search_root.rglob("hoppr-tmp-*"))
+    for folder in temp_paths:
+        if os.path.isdir(folder):
+            shutil.rmtree(folder, ignore_errors=True)
+        else:
+            folder.unlink()
+
+
 class CollectDnfPlugin(BatchCollectorPlugin):
     """
     Collector plugin for DNF packages
     """
 
     required_commands: list[str] = ["dnf"]
     supported_purl_types: list[str] = ["rpm"]
@@ -111,22 +122,20 @@
         ]
 
     def _get_component_download_url(self, purl: PackageURL) -> str:
         artifact = _artifact_string(purl)
 
         command = [*self.base_command, "repoquery", "--location", artifact]
         run_result = self.run_command(command, self.password_list)
-
         # If RPM URL not found, no need to try downloading it
         if run_result.returncode != 0 or len(run_result.stdout.decode("utf-8")) == 0:
             msg = f"{self.required_commands[0]} failed to locate package for {purl}"
             self.get_logger().debug(msg=msg, indent_level=2)
 
             raise HopprPluginError(msg)
-
         # Taking the first URL if multiple are returned
         return run_result.stdout.decode("utf-8").strip().split("\n")[0]
 
     def _get_found_repo(self, found_url: str) -> str | None:
         """
         Identify the repository associated with the specified URL
         """
@@ -136,18 +145,21 @@
         return __version__
 
     @hoppr_process
     def pre_stage_process(self) -> Result:
         repo_config = ConfigParser()
         repo_config["main"] = dict(cachedir=f"{self.config_file.parent / 'cache'}")
 
+        # Clear out cache before starting the pre_stage_process
+        search_root = self.config_file.parent / "cache"
+        _clear_cache(search_root)
+
         for idx, repo in enumerate(self.context.repositories[PurlType.RPM]):
             temp_repo = f"hoppr-tmp-{idx}"
             creds = Credentials.find(f"{repo.url}")
-
             if not _is_rpm_repo(f"{repo.url}"):
                 self.get_logger().warning(
                     f"Repo {repo.url} is not an RPM repository (repomd.xml file not found), will not be searched"
                 )
                 continue
 
             self.get_logger().debug(f"Creating repo {temp_repo} for url {repo.url}")
@@ -179,30 +191,28 @@
                     repo_config.add_section(section)
                     repo_config[section] = dict(system_repos[section])
 
         try:
             # Create repo config dir in user directory
             config_dir = self.config_file.parent
             config_dir.mkdir(parents=True, exist_ok=True)
-
             with self.config_file.open(mode="w+", encoding="utf-8") as repo_file:
                 repo_config.write(repo_file, space_around_delimiters=False)
         except OSError as ex:
             return Result.fail(f"Unable to write DNF repository config file: {ex}")
 
         # Populate user DNF cache
         command = [
             *self.base_command,
             "check-update",
             "makecache",
         ]
-
         # Generate cache to use when downloading components
         result = self.run_command(command, self.password_list)
-
+        self.get_logger().debug(msg=(f"Return Code: {result.returncode}"), indent_level=2)
         if result.returncode != 0:
             return Result.fail(message="Failed to populate DNF cache.")
 
         return Result.success()
 
     @hoppr_rerunner
     def collect(self, comp: Component) -> Result:
@@ -281,8 +291,11 @@
 
         if self.config_file.exists():
             try:
                 self.config_file.unlink()
             except FileNotFoundError as ex:
                 return Result.fail(f"Failed to remove temporary DNF config file: {ex}")
 
+        # Clear cache at the end of the post stage process
+        _clear_cache(search_root)
+
         return Result.success()
```

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
 
         self.manifest_repos: list[str] = []
         self.password_list: list[str] = []
         self.base_command = [self.required_commands[0], "-m", "pip"]
+        # Allow users to define their own pip command...
+        # i.e. python3.6 -m pip
+        if self.config is not None:
+            if "pip_command" in self.config:
+                self.base_command = str(self.config["pip_command"]).split(" ", maxsplit=-1)
 
     def _run_cmd_wrapper(  # pylint: disable=too-many-arguments
         self, command, password_list, param: str, pkg_format: str, log_if_error: str
     ) -> bool:
         """
         Run command utility for discrete function calls - required for DO-178C Level-A branch isolation coverage
         """
@@ -107,15 +112,20 @@
             "--dest",
             f"{target_dir}",
             f"{purl.name}=={purl.version}",
         ]
 
         base_error_msg = f"Failed to download {purl.name} version {purl.version}"
 
-        if self.collect_binary_only(command, password_list, base_error_msg):  # pylint: disable=no-else-return
+        collection_type = "ANY"
+
+        if self.config is not None and "type" in self.config:
+            collection_type = str(self.config["type"]).lower()
+
+        if (collection_type != "source") and self.collect_binary_only(command, password_list, base_error_msg):
             self.set_collection_params(comp, repo_url, target_dir)
             return Result.success(return_obj=comp)
-        elif self.collect_source(command, password_list, base_error_msg):  # pylint: disable=no-else-return
+        if (collection_type != "binary") and self.collect_source(command, password_list, base_error_msg):
             self.set_collection_params(comp, repo_url, target_dir)
             return Result.success(return_obj=comp)
-        else:
-            return Result.retry(f"{base_error_msg} as either binary or source.")
+
+        return Result.retry(f"{base_error_msg} with collection type: {collection_type}.")
```

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.7/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.7/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.7/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.7/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.7/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.7/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/in_toto.py` & `hoppr-1.8.7/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/main.py` & `hoppr-1.8.7/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/mem_logger.py` & `hoppr-1.8.7/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/__init__.py` & `hoppr-1.8.7/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/__main__.py` & `hoppr-1.8.7/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/base.py` & `hoppr-1.8.7/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/credentials.py` & `hoppr-1.8.7/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/manifest.py` & `hoppr-1.8.7/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/transfer.py` & `hoppr-1.8.7/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/models/types.py` & `hoppr-1.8.7/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/net.py` & `hoppr-1.8.7/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/oci_artifacts.py` & `hoppr-1.8.7/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/plugin_utils.py` & `hoppr-1.8.7/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/processor.py` & `hoppr-1.8.7/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.7/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.7/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/result.py` & `hoppr-1.8.7/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/hoppr/utils.py` & `hoppr-1.8.7/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.6/pyproject.toml` & `hoppr-1.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.6"
+version = "1.8.7"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.6/PKG-INFO` & `hoppr-1.8.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.6
+Version: 1.8.7
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

