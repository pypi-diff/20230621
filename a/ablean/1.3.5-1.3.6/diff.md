# Comparing `tmp/ablean-1.3.5.tar.gz` & `tmp/ablean-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablean-1.3.5.tar", last modified: Tue Jun 20 10:20:44 2023, max compression
+gzip compressed data, was "ablean-1.3.6.tar", last modified: Wed Jun 21 01:32:09 2023, max compression
```

## Comparing `ablean-1.3.5.tar` & `ablean-1.3.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.472756 ablean-1.3.5/
--rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.5/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.300584 ablean-1.3.5/.vscode/
--rw-rw-rw-   0        0        0     1442 2023-04-20 14:13:20.000000 ablean-1.3.5/.vscode/launch.json
--rw-rw-rw-   0        0        0    55778 2023-06-20 10:20:44.472756 ablean-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.318037 ablean-1.3.5/ablean/
--rw-rw-rw-   0        0        0      930 2023-06-20 10:20:31.000000 ablean-1.3.5/ablean/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.371460 ablean-1.3.5/ablean/commands/
--rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.5/ablean/commands/__init__.py
--rw-rw-rw-   0        0        0    12595 2022-06-05 10:53:45.000000 ablean-1.3.5/ablean/commands/backtest.py
--rw-rw-rw-   0        0        0    10248 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/commands/create_project.py
--rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.5/ablean/commands/download.py
--rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.5/ablean/commands/init.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.379490 ablean-1.3.5/ablean/components/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.396826 ablean-1.3.5/ablean/components/config/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/cli_config_manager.py
--rw-rw-rw-   0        0        0    13701 2022-06-06 10:41:19.000000 ablean-1.3.5/ablean/components/config/lean_config_manager.py
--rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/output_config_manager.py
--rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/project_config_manager.py
--rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.5/ablean/components/config/storage.py
--rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/lean_runner.py
--rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/module_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.429169 ablean-1.3.5/ablean/components/util/
--rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.5/ablean/components/util/__init__.py
--rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/logger.py
--rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/name_extraction.py
--rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/name_generator.py
--rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/path_manager.py
--rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/platform_manager.py
--rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.5/ablean/components/util/project_manager.py
--rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/temp_manager.py
--rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/xml_manager.py
--rw-rw-rw-   0        0        0     4445 2022-06-06 06:09:31.000000 ablean-1.3.5/ablean/constants.py
--rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/container.py
--rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.5/ablean/data_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.439354 ablean-1.3.5/ablean/icons/
--rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/icons/icon.icns
--rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/icons/icon.ico
--rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.5/ablean/main.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.463267 ablean-1.3.5/ablean/models/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/__init__.py
--rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/errors.py
--rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/modules.py
--rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/options.py
--rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/pydantic.py
--rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/utils.py
--rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/myclick.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.342254 ablean-1.3.5/ablean.egg-info/
--rw-rw-rw-   0        0        0    55778 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      302 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      913 2022-06-05 05:44:09.000000 ablean-1.3.5/pub.ps1
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.470762 ablean-1.3.5/scripts/
--rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.5/scripts/readme.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:20:44.473756 ablean-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.189117 ablean-1.3.6/
+-rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.6/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.129460 ablean-1.3.6/.vscode/
+-rw-rw-rw-   0        0        0     1442 2023-04-20 14:13:20.000000 ablean-1.3.6/.vscode/launch.json
+-rw-rw-rw-   0        0        0    55778 2023-06-21 01:32:09.189117 ablean-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.133949 ablean-1.3.6/ablean/
+-rw-rw-rw-   0        0        0      930 2023-06-21 01:31:16.000000 ablean-1.3.6/ablean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.157568 ablean-1.3.6/ablean/commands/
+-rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.6/ablean/commands/__init__.py
+-rw-rw-rw-   0        0        0    12595 2022-06-05 10:53:45.000000 ablean-1.3.6/ablean/commands/backtest.py
+-rw-rw-rw-   0        0        0    10248 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/commands/create_project.py
+-rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.6/ablean/commands/download.py
+-rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.6/ablean/commands/init.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.159963 ablean-1.3.6/ablean/components/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.164986 ablean-1.3.6/ablean/components/config/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/config/cli_config_manager.py
+-rw-rw-rw-   0        0        0    14072 2023-06-21 01:14:02.000000 ablean-1.3.6/ablean/components/config/lean_config_manager.py
+-rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/config/output_config_manager.py
+-rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/config/project_config_manager.py
+-rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.6/ablean/components/config/storage.py
+-rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/lean_runner.py
+-rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/module_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.171986 ablean-1.3.6/ablean/components/util/
+-rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.6/ablean/components/util/__init__.py
+-rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/logger.py
+-rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/name_extraction.py
+-rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/name_generator.py
+-rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/path_manager.py
+-rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/platform_manager.py
+-rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.6/ablean/components/util/project_manager.py
+-rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/temp_manager.py
+-rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/components/util/xml_manager.py
+-rw-rw-rw-   0        0        0     4485 2023-06-21 00:58:59.000000 ablean-1.3.6/ablean/constants.py
+-rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/container.py
+-rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.6/ablean/data_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.183137 ablean-1.3.6/ablean/icons/
+-rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/icons/icon.icns
+-rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/icons/icon.ico
+-rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.6/ablean/main.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.187116 ablean-1.3.6/ablean/models/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/__init__.py
+-rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/errors.py
+-rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/modules.py
+-rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/options.py
+-rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/pydantic.py
+-rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/models/utils.py
+-rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.6/ablean/myclick.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.155587 ablean-1.3.6/ablean.egg-info/
+-rw-rw-rw-   0        0        0    55778 2023-06-21 01:32:08.000000 ablean-1.3.6/ablean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-06-21 01:32:09.000000 ablean-1.3.6/ablean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 01:32:08.000000 ablean-1.3.6/ablean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-21 01:32:08.000000 ablean-1.3.6/ablean.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      302 2023-06-21 01:32:08.000000 ablean-1.3.6/ablean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 01:32:08.000000 ablean-1.3.6/ablean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      913 2022-06-05 05:44:09.000000 ablean-1.3.6/pub.ps1
+drwxrwxrwx   0        0        0        0 2023-06-21 01:32:09.188117 ablean-1.3.6/scripts/
+-rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.6/scripts/readme.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 01:32:09.190250 ablean-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.6/setup.py
```

### Comparing `ablean-1.3.5/.gitignore` & `ablean-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/.vscode/launch.json` & `ablean-1.3.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/PKG-INFO` & `ablean-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.5
+Version: 1.3.6
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ablean-1.3.5/README.md` & `ablean-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/__init__.py` & `ablean-1.3.6/ablean/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The version is always set to "dev" in the Git repository. When a new release is ready,
 # a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
 # package to PyPI with the version of the tag.
-__version__ = "1.3.5"
+__version__ = "1.3.6"
```

### Comparing `ablean-1.3.5/ablean/commands/__init__.py` & `ablean-1.3.6/ablean/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/commands/backtest.py` & `ablean-1.3.6/ablean/commands/backtest.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/commands/create_project.py` & `ablean-1.3.6/ablean/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/commands/download.py` & `ablean-1.3.6/ablean/commands/download.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/commands/init.py` & `ablean-1.3.6/ablean/commands/init.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/__init__.py` & `ablean-1.3.6/ablean/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/config/__init__.py` & `ablean-1.3.6/ablean/components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/config/cli_config_manager.py` & `ablean-1.3.6/ablean/components/config/cli_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/config/lean_config_manager.py` & `ablean-1.3.6/ablean/components/config/lean_config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 import re
 from pathlib import Path
 from typing import Any, Dict, Optional, List
 
 import json5
 
 from ablean.components.config.cli_config_manager import CLIConfigManager
 from ablean.components.config.project_config_manager import ProjectConfigManager
 from ablean.components.module_manager import ModuleManager
 from ablean.components.config.storage import Storage
 from ablean.components.util.logger import Logger
-from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME, GUI_PRODUCT_INSTALL_ID
+from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME, ENV_LEAN_PATH_NAME, GUI_PRODUCT_INSTALL_ID
 from ablean.models.errors import MoreInfoError
 from ablean.models.utils import DebuggingMethod
 
 
 class LeanConfigManager:
     """The LeanConfigManager class contains utilities to work with files containing LEAN engine configuration."""
 
@@ -64,30 +65,40 @@
         if self._default_path is not None:
             return self._default_path
 
         if self._lean_config_path is not None:
             return self._lean_config_path
 
         # Recurse upwards in the directory tree until we find a Lean config file
-        current_dir = Path.cwd()
-        while True:
-            target_file = current_dir / DEFAULT_LEAN_CONFIG_FILE_NAME
+        list = self.get_search_paths()
+        for current_dir in list:
+            target_file = os.path.join(current_dir, DEFAULT_LEAN_CONFIG_FILE_NAME)
             if target_file.exists():
                 self._lean_config_path = target_file
                 self.store_known_lean_config_path(self._lean_config_path)
                 return self._lean_config_path
-
+            
+        raise MoreInfoError(
+            f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
+            "https://www.lean.io/docs/lean-cli/initialization/configuration#03-Lean-Configuration",
+        )
+    
+    def get_search_paths(self):
+        current_dir = Path.cwd()
+        dirs = [current_dir]
+        while True:
             # If the parent directory is the same as the current directory we can't go up any more
             if current_dir.parent == current_dir:
-                raise MoreInfoError(
-                    f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
-                    "https://www.lean.io/docs/lean-cli/initialization/configuration#03-Lean-Configuration",
-                )
-
-            current_dir = current_dir.parent
+                break
+            current_dir = current_dir.parent              
+            dirs.append(current_dir)
+        v = os.environ.get(ENV_LEAN_PATH_NAME)
+        if  v is not None:
+            dirs.append(Path(v))
+        return dirs
 
     def set_default_lean_config_path(self, path: Path) -> None:
         """Overrides the default search for the path to the Lean config file.
 
         :param path: the path to the Lean config file to return in future calls to get_lean_config_path()
         """
         self.store_known_lean_config_path(path)
```

### Comparing `ablean-1.3.5/ablean/components/config/output_config_manager.py` & `ablean-1.3.6/ablean/components/config/output_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/config/project_config_manager.py` & `ablean-1.3.6/ablean/components/config/project_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/config/storage.py` & `ablean-1.3.6/ablean/components/config/storage.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/lean_runner.py` & `ablean-1.3.6/ablean/components/lean_runner.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/module_manager.py` & `ablean-1.3.6/ablean/components/module_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/__init__.py` & `ablean-1.3.6/ablean/components/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/logger.py` & `ablean-1.3.6/ablean/components/util/logger.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/name_extraction.py` & `ablean-1.3.6/ablean/components/util/name_extraction.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/name_generator.py` & `ablean-1.3.6/ablean/components/util/name_generator.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/path_manager.py` & `ablean-1.3.6/ablean/components/util/path_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/platform_manager.py` & `ablean-1.3.6/ablean/components/util/platform_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/project_manager.py` & `ablean-1.3.6/ablean/components/util/project_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/temp_manager.py` & `ablean-1.3.6/ablean/components/util/temp_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/components/util/xml_manager.py` & `ablean-1.3.6/ablean/components/util/xml_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/constants.py` & `ablean-1.3.6/ablean/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 # The file in which we store when we last checked for updates
 CACHE_PATH = str(Path("~/.lean/cache").expanduser())
 
 # The directory in which modules are stored
 MODULES_DIRECTORY = str(Path("~/.lean/modules").expanduser())
 
+ENV_LEAN_PATH_NAME = "ABL_LEAN_PATH"
+
 # The default name of the file containing the Lean engine configuration
 DEFAULT_LEAN_CONFIG_FILE_NAME = "lean.json"
 
 # The default name of the directory containing the market data
 DEFAULT_DATA_DIRECTORY_NAME = "data"
 
 # The name of the file in containing the project configuration
```

### Comparing `ablean-1.3.5/ablean/container.py` & `ablean-1.3.6/ablean/container.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/data_manager.py` & `ablean-1.3.6/ablean/data_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/icons/icon.icns` & `ablean-1.3.6/ablean/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/icons/icon.ico` & `ablean-1.3.6/ablean/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/main.py` & `ablean-1.3.6/ablean/main.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/__init__.py` & `ablean-1.3.6/ablean/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/errors.py` & `ablean-1.3.6/ablean/models/errors.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/modules.py` & `ablean-1.3.6/ablean/models/modules.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/options.py` & `ablean-1.3.6/ablean/models/options.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/pydantic.py` & `ablean-1.3.6/ablean/models/pydantic.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/models/utils.py` & `ablean-1.3.6/ablean/models/utils.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean/myclick.py` & `ablean-1.3.6/ablean/myclick.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/ablean.egg-info/PKG-INFO` & `ablean-1.3.6/ablean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.5
+Version: 1.3.6
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ablean-1.3.5/ablean.egg-info/SOURCES.txt` & `ablean-1.3.6/ablean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/pub.ps1` & `ablean-1.3.6/pub.ps1`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/scripts/readme.py` & `ablean-1.3.6/scripts/readme.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.5/setup.py` & `ablean-1.3.6/setup.py`

 * *Files identical despite different names*

