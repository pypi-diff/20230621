# Comparing `tmp/pictorus-0.0.7.tar.gz` & `tmp/pictorus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.0.7.tar", last modified: Tue Jun 13 16:19:32 2023, max compression
+gzip compressed data, was "pictorus-0.0.8.tar", last modified: Wed Jun 21 04:43:14 2023, max compression
```

## Comparing `pictorus-0.0.7.tar` & `pictorus-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.7/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.7/.gitignore
--rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.7/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.7/LICENSE
--rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.7/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.7/README.md
--rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.7/script/setup
--rw-r--r--   0        0        0       61 2023-06-13 16:18:46.133398 pictorus-0.0.7/src/pictorus/__init__.py
--rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.7/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     3147 2023-06-06 15:52:56.896505 pictorus-0.0.7/src/pictorus/config.py
--rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.7/src/pictorus/constants.py
--rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.7/src/pictorus/logging.py
--rw-r--r--   0        0        0     5040 2023-06-13 16:18:36.750543 pictorus-0.0.7/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.7/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.7/src/pictorus/systemd.py
--rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.7/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.7/src/pictorus/version_manager.py
--rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.7/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.7/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-06-21 04:42:19.636723 pictorus-0.0.8/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.8/.gitignore
+-rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.0.8/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.8/LICENSE
+-rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.0.8/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.8/README.md
+-rw-r--r--   0        0        0      829 2023-06-21 04:42:19.637210 pictorus-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.8/script/setup
+-rw-r--r--   0        0        0       61 2023-06-21 04:42:39.631742 pictorus-0.0.8/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.8/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     3297 2023-06-21 04:42:19.637658 pictorus-0.0.8/src/pictorus/config.py
+-rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.8/src/pictorus/constants.py
+-rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.8/src/pictorus/logging.py
+-rw-r--r--   0        0        0     5041 2023-06-21 04:42:19.638038 pictorus-0.0.8/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.8/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.8/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.8/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3328 2023-06-21 04:42:19.638345 pictorus-0.0.8/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0     8967 2023-06-21 04:42:19.638752 pictorus-0.0.8/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.0.8/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 pictorus-0.0.8/PKG-INFO
```

### Comparing `pictorus-0.0.7/.gitignore` & `pictorus-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/LICENSE` & `pictorus-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/PUB_README.md` & `pictorus-0.0.8/PUB_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Pictorus Device Manager
-Python library for managing devices connected to a [Pictorus](https://pictor.us) account
+# Pictorus Device Manager (Beta)
+Python library for managing devices connected to a [Pictorus Beta](https://pictor.us) account
 
 ## Installation
 `sudo pip3 install pictorus`
 
 Note: The package is installed/run using `sudo` so it can create and manage the required systemd services on your machine. You can install/run without `sudo`. This will still let you register your device, but you may need to manually configure `pictorus-device-manager` to run using your preferred process manager.
 
 ## Usage
```

### Comparing `pictorus-0.0.7/README.md` & `pictorus-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/pyproject.toml` & `pictorus-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 name = "pictorus"
 authors = [{ name = "Pictorus Inc", email = "contact@pictor.us" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dynamic = ["version", "description"]
-dependencies = ["awsiotsdk~=1.11.5", "requests~=2.26.0", "semver~=3.0.0"]
-requires-python = ">=3.7"
+dependencies = ["awsiotsdk~=1.11.5", "requests~=2.26.0", "semver~=2.13.0"]
+requires-python = ">=3.6"
 readme = "PUB_README.md"
 
 [project.scripts]
 pictorus-cli = "pictorus.pictorus_cli:main"
 pictorus-device-manager = "pictorus.pictorus_device_manager:main"
 
 [project.urls]
 Home = "https://pictor.us"
 
 [project.optional-dependencies]
 dev = ["black==22.3.0"]
-test = ["responses==0.22.0", "pytest==7.2.1"]
+test = ["responses==0.17.0", "pytest==7.0.1"]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.black]
 line-length = 100
```

### Comparing `pictorus-0.0.7/src/pictorus/app_manager.py` & `pictorus-0.0.8/src/pictorus/app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/src/pictorus/config.py` & `pictorus-0.0.8/src/pictorus/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Common configuration defs """
 import json
 import os
 from enum import Enum
+from getpass import getuser
 
 
 class Environment(Enum):
     """Backend environment to communicate with"""
 
     CI = "ci"
     LOCAL = "local"
@@ -18,15 +19,17 @@
 API_PREFIX = {
     Environment.CI: "http://127.0.0.1:5000",
     Environment.LOCAL: "http://127.0.0.1:5000",
     Environment.TEST: "https://api.test.pictor.us",
     Environment.PROD: "https://api.pictor.us",
 }[PICTORUS_ENV]
 
-DEVICE_MGR_DIR = os.path.expanduser("~/.pictorus/device_manager")
+# Some linux distros seem to resolve the incorrect path
+# as sudo unless the username is explicitly passed in
+DEVICE_MGR_DIR = os.path.expanduser(f"~{getuser()}/.pictorus/device_manager")
 APP_ASSETS_DIR = os.path.join(DEVICE_MGR_DIR, "apps/")
 
 CONFIG_PATH = os.path.join(DEVICE_MGR_DIR, "config.json")
 APP_MANIFEST_PATH = os.path.join(DEVICE_MGR_DIR, "app_manifest.json")
 
 
 class Config:
```

### Comparing `pictorus-0.0.7/src/pictorus/pictorus_cli.py` & `pictorus-0.0.8/src/pictorus/pictorus_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 """ CLI entrypoint for pictorus device manager """
 import argparse
 from getpass import getpass
 import platform
 import socket
 import sys
```

### Comparing `pictorus-0.0.7/src/pictorus/pictorus_device_manager.py` & `pictorus-0.0.8/src/pictorus/pictorus_device_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/src/pictorus/systemd.py` & `pictorus-0.0.8/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/src/pictorus/telemetry_manager.py` & `pictorus-0.0.8/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.7/src/pictorus/version_manager.py` & `pictorus-0.0.8/src/pictorus/version_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import time
 import subprocess as sp
 from threading import Thread
-from semver import Version
+from semver import VersionInfo
 
 import requests
 
 import pictorus
 from pictorus.logging import get_logger
 from pictorus.config import Config
 
@@ -55,18 +55,18 @@
             logger.debug("Could not check if there is a new version of pip available.")
             self._transient_check_fail = True
             return None
 
         self._transient_check_fail = False
 
         latest_version = response.json()["info"]["version"]
-        latest_version = Version.parse(latest_version)
+        latest_version = VersionInfo.parse(latest_version)
 
         current_version = self._last_installed or pictorus.__version__
-        current_version = Version.parse(current_version)
+        current_version = VersionInfo.parse(current_version)
         if current_version < latest_version:
             return str(latest_version)
 
         return None
 
     def install_version(self, version: str):
         """Attempt to install latest version of pictorus package"""
```

### Comparing `pictorus-0.0.7/tests/pictorus/test_app_manager.py` & `pictorus-0.0.8/tests/pictorus/test_app_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,16 +110,16 @@
     def test_starts_app_on_update(self, m_shadow_req, _, __, m_telem, m_popen):
         config.run_app = True
         new_build_id = "newfoo"
         new_params_hash = "newparams123"
         version_url = "http://foo.bar/baz"
         params_url = "http://foo.bar/params.json"
 
-        responses.get(version_url, body="")
-        responses.get(params_url, body="")
+        responses.add(responses.GET, version_url, body="")
+        responses.add(responses.GET, params_url, body="")
 
         m_write = mock_open()
         version_data = {
             "build_hash": new_build_id,
             "app_bin_url": version_url,
             "params_hash": new_params_hash,
             "params_url": params_url,
@@ -135,15 +135,15 @@
             m_telem.return_value.start_listening.assert_called_once_with(new_build_id)
             assert_correct_app_start(m_popen)
             assert config.run_app is True
 
             handle = m_write()
             handle.write.assert_called_once_with(json.dumps(manifest_data))
 
-        assert m_shadow_req.mock_calls[1].kwargs["state"].reported["app_version"] == manifest_data
+        assert m_shadow_req.mock_calls[1][2]["state"].reported["app_version"] == manifest_data
 
     def test_set_telemetry_ttl(self, m_telem, _):
         ttl_s = 99
         set_ttl_cmd = json.dumps(
             {"type": CmdType.SET_TELEMETRY_TLL.value, "data": {"ttl_s": ttl_s}}
         )
         with AppManager(Mock()) as mgr:
@@ -158,15 +158,15 @@
             {"type": CmdType.SET_LOG_LEVEL.value, "data": {"log_level": log_level.value}}
         )
         with AppManager(Mock()) as mgr:
             m_popen.reset_mock()
             mgr._on_cmd_request("req", set_ttl_cmd)
             assert_correct_app_start(m_popen, log_level=log_level)
 
-        assert m_shadow_req.mock_calls[1].kwargs["state"].reported["log_level"] == log_level.value
+        assert m_shadow_req.mock_calls[1][2]["state"].reported["log_level"] == log_level.value
 
     @responses.activate
     @patch("pictorus.app_manager.run")
     def test_set_upload_logs(self, m_run, _, __):
         upload_url = "https://example.com/upload"
 
         upload_logs_cmd = json.dumps(
@@ -174,15 +174,15 @@
                 "type": CmdType.UPLOAD_LOGS.value,
                 "data": {
                     "upload_dest": {"url": upload_url, "fields": {"foo": "bar"}},
                     "line_count": 500,
                 },
             }
         )
-        responses.post(upload_url, body="")
+        responses.add(responses.POST, upload_url, body="")
         m_mqtt = Mock()
         with AppManager(m_mqtt) as mgr:
             mgr._on_retained_cmd("ret", upload_logs_cmd)
             m_run.assert_called_once_with(
                 ["journalctl", "-u", "pictorus", "-n", "500", "--no-pager"],
                 check=True,
                 stdout=ANY,
@@ -204,39 +204,35 @@
         expected_err = {"err_type": "Foo", "message": "Bar"}
 
         with AppManager(Mock()) as mgr, patch(
             "builtins.open", mock_open(read_data=json.dumps(expected_err))
         ):
             # Error should get cleared on init
             assert (
-                m_shadow_req.call_args.kwargs["state"].reported["error_log"]
-                == AppManager.EMPTY_ERROR
+                m_shadow_req.call_args[1]["state"].reported["error_log"] == AppManager.EMPTY_ERROR
             )
             app_complete.set()
 
             # Wait for app to get marked as stopped
             wait_for_condition(lambda: not mgr.app_is_running)
 
         m_remove.assert_called_once_with(AppManager.ERROR_LOG_PATH)
-        assert m_shadow_req.call_args.kwargs["state"].reported["error_log"] == expected_err
+        assert m_shadow_req.call_args[1]["state"].reported["error_log"] == expected_err
 
     @patch("pictorus.app_manager.iotshadow.UpdateShadowRequest")
     def test_sets_default_error_on_unexpected_crash(self, m_shadow_req, _, m_popen):
         app_complete = threading.Event()
         m_popen.return_value.wait.return_value = app_complete
         self.m_exists.side_effect = lambda p: p != AppManager.ERROR_LOG_PATH
         config.run_app = True
 
         with AppManager(Mock()) as mgr:
             # Error should get cleared on init
             assert (
-                m_shadow_req.call_args.kwargs["state"].reported["error_log"]
-                == AppManager.EMPTY_ERROR
+                m_shadow_req.call_args[1]["state"].reported["error_log"] == AppManager.EMPTY_ERROR
             )
             app_complete.set()
 
             # Wait for app to get marked as stopped
             wait_for_condition(lambda: not mgr.app_is_running)
 
-        assert (
-            m_shadow_req.call_args.kwargs["state"].reported["error_log"] == AppManager.NO_LOG_ERROR
-        )
+        assert m_shadow_req.call_args[1]["state"].reported["error_log"] == AppManager.NO_LOG_ERROR
```

### Comparing `pictorus-0.0.7/tests/pictorus/test_version_manager.py` & `pictorus-0.0.8/tests/pictorus/test_version_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import sys
 from unittest import TestCase, mock
 import responses
 from subprocess import CalledProcessError
 
-from semver import Version
+from semver import VersionInfo
 
 import pictorus as pictorus
 from pictorus.version_manager import VersionManager
 
 
 class TestVersionManager(TestCase):
     def setUp(self):
         self.vm = VersionManager()
-        self.version = Version.parse(pictorus.__version__)
+        self.version = VersionInfo.parse(pictorus.__version__)
 
     @responses.activate
     def test_check_for_newer_version_has_new_version(self):
         new_version = self.version.bump_minor()
-        responses.get(
-            "https://pypi.org/pypi/pictorus/json", json={"info": {"version": str(new_version)}}
+        responses.add(
+            responses.GET,
+            "https://pypi.org/pypi/pictorus/json",
+            json={"info": {"version": str(new_version)}},
         )
         assert self.vm.check_for_newer_version() == str(new_version)
 
     @responses.activate
     def test_check_for_newer_version_no_update(self):
-        responses.get(
-            "https://pypi.org/pypi/pictorus/json", json={"info": {"version": pictorus.__version__}}
+        responses.add(
+            responses.GET,
+            "https://pypi.org/pypi/pictorus/json",
+            json={"info": {"version": pictorus.__version__}},
         )
         assert self.vm.check_for_newer_version() is None
 
     @responses.activate
     def test_check_for_newer_version_request_failure(self):
-        responses.get("https://pypi.org/pypi/pictorus/json", status=500)
+        responses.add(responses.GET, "https://pypi.org/pypi/pictorus/json", status=500)
         assert self.vm.check_for_newer_version() is None
         assert self.vm._transient_check_fail is True
 
     @responses.activate
     def test_check_for_newer_version_uses_cached_version_from_last_update(self):
         new_version = self.version.bump_minor()
-        responses.get(
-            "https://pypi.org/pypi/pictorus/json", json={"info": {"version": str(new_version)}}
+        responses.add(
+            responses.GET,
+            "https://pypi.org/pypi/pictorus/json",
+            json={"info": {"version": str(new_version)}},
         )
         self.vm._last_installed = str(new_version)
         assert self.vm.check_for_newer_version() is None
 
     @mock.patch("pictorus.version_manager.sp.check_call")
     def test_install_version_success(self, m_check_call):
         version = "1.2.3"
```

### Comparing `pictorus-0.0.7/PKG-INFO` & `pictorus-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.5
 Requires-Dist: requests~=2.26.0
-Requires-Dist: semver~=3.0.0
+Requires-Dist: semver~=2.13.0
 Requires-Dist: black==22.3.0 ; extra == "dev"
-Requires-Dist: responses==0.22.0 ; extra == "test"
-Requires-Dist: pytest==7.2.1 ; extra == "test"
+Requires-Dist: responses==0.17.0 ; extra == "test"
+Requires-Dist: pytest==7.0.1 ; extra == "test"
 Project-URL: Home, https://pictor.us
 Provides-Extra: dev
 Provides-Extra: test
 
-# Pictorus Device Manager
-Python library for managing devices connected to a [Pictorus](https://pictor.us) account
+# Pictorus Device Manager (Beta)
+Python library for managing devices connected to a [Pictorus Beta](https://pictor.us) account
 
 ## Installation
 `sudo pip3 install pictorus`
 
 Note: The package is installed/run using `sudo` so it can create and manage the required systemd services on your machine. You can install/run without `sudo`. This will still let you register your device, but you may need to manually configure `pictorus-device-manager` to run using your preferred process manager.
 
 ## Usage
```

