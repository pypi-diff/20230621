# Comparing `tmp/cloud_tpu_diagnostics-0.1.0.tar.gz` & `tmp/cloud_tpu_diagnostics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_tpu_diagnostics-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cloud_tpu_diagnostics-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cloud_tpu_diagnostics-0.1.0.tar` & `cloud_tpu_diagnostics-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     3438 2023-06-07 20:57:00.513979 cloud_tpu_diagnostics-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-06-07 20:57:00.505979 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/__init__.py
--rw-r--r--   0        0        0      206 2023-06-07 20:57:00.501978 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/configuration.py
--rw-r--r--   0        0        0       56 2023-06-07 20:57:00.497978 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/diagnostic.py
--rw-r--r--   0        0        0      400 2023-06-07 20:57:00.469976 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/config/debug_configuration.py
--rw-r--r--   0        0        0      346 2023-06-07 20:57:00.477976 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/config/diagnostic_configuration.py
--rw-r--r--   0        0        0      973 2023-06-07 20:57:00.473976 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/config/stack_trace_configuration.py
--rw-r--r--   0        0        0     1279 2023-06-07 20:57:00.465975 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/debug.py
--rw-r--r--   0        0        0      478 2023-06-07 20:57:00.493978 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/diagnose.py
--rw-r--r--   0        0        0     2384 2023-06-07 20:57:00.481977 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/stack_trace.py
--rw-r--r--   0        0        0      203 2023-06-07 20:57:00.489977 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/util/default.py
--rw-r--r--   0        0        0     2235 2023-06-07 20:57:00.485977 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/util/stack_trace_test_util.py
--rw-r--r--   0        0        0     1377 2023-06-07 20:57:00.457975 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/tests/debug_test.py
--rw-r--r--   0        0        0     5219 2023-06-07 20:57:00.461975 cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/tests/stack_trace_test.py
--rw-r--r--   0        0        0     1064 2023-06-07 20:57:00.509979 cloud_tpu_diagnostics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 cloud_tpu_diagnostics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3699 2023-06-21 18:52:59.709841 cloud_tpu_diagnostics-0.1.1/README.md
+-rw-r--r--   0        0        0       93 2023-06-21 18:52:59.701840 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-21 18:52:59.697840 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/configuration.py
+-rw-r--r--   0        0        0       56 2023-06-21 18:52:59.693839 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/diagnostic.py
+-rw-r--r--   0        0        0      400 2023-06-21 18:52:59.669837 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/config/debug_configuration.py
+-rw-r--r--   0        0        0      346 2023-06-21 18:52:59.677838 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/config/diagnostic_configuration.py
+-rw-r--r--   0        0        0      973 2023-06-21 18:52:59.673838 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/config/stack_trace_configuration.py
+-rw-r--r--   0        0        0     1310 2023-06-21 18:52:59.665837 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/debug.py
+-rw-r--r--   0        0        0      478 2023-06-21 18:52:59.689839 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/diagnose.py
+-rw-r--r--   0        0        0     2554 2023-06-21 18:52:59.677838 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/stack_trace.py
+-rw-r--r--   0        0        0      203 2023-06-21 18:52:59.685839 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/util/default.py
+-rw-r--r--   0        0        0     2235 2023-06-21 18:52:59.681838 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/util/stack_trace_test_util.py
+-rw-r--r--   0        0        0     2474 2023-06-21 18:52:59.653836 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/tests/debug_test.py
+-rw-r--r--   0        0        0     1158 2023-06-21 18:52:59.661836 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/tests/diagnose_test.py
+-rw-r--r--   0        0        0     6272 2023-06-21 18:52:59.657836 cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/tests/stack_trace_test.py
+-rw-r--r--   0        0        0     1064 2023-06-21 18:52:59.705840 cloud_tpu_diagnostics-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 cloud_tpu_diagnostics-0.1.1/PKG-INFO
```

### Comparing `cloud_tpu_diagnostics-0.1.0/README.md` & `cloud_tpu_diagnostics-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -47,15 +47,20 @@
 ##### Scenario 3: Collect stack traces on faults and upload on cloud
 
 ```
 stack_trace_config = stack_trace_configuration.StackTraceConfig(
                       collect_stack_trace=True,
                       stack_trace_to_cloud=True)
 ```
-This configuration will temporary collect stack traces inside `/tmp/debugging` directory on TPU host if there is a fault or process hang. Additionally, the traces collected in TPU host memory will be uploaded to Google Cloud Logging, which will make it easier to troubleshoot and fix the problems.
+This configuration will temporary collect stack traces inside `/tmp/debugging` directory on TPU host if there is a fault or process hang. Additionally, the traces collected in TPU host memory will be uploaded to Google Cloud Logging, which will make it easier to troubleshoot and fix the problems. You can view the traces in [Logs Explorer](https://cloud.google.com/logging/docs/view/logs-explorer-interface) using the following query:
+
+```
+logName="projects/<project_name>/logs/tpu.googleapis.com%2Fruntime_monitor"
+jsonPayload.verb="stacktraceanalyzer"
+```
 
 By default, stack traces will be collected every 10 minutes. In order to change the duration between two stack trace collection events, add the following configuration:
 
 ```
 stack_trace_config = stack_trace_configuration.StackTraceConfig(
                       collect_stack_trace=True,
                       stack_trace_to_cloud=True,
```

### Comparing `cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/config/stack_trace_configuration.py` & `cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/config/stack_trace_configuration.py`

 * *Files identical despite different names*

### Comparing `cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/debug.py` & `cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def stop_debugging(debug_config):
   """Context manager to debug and identify errors."""
   if (
       debug_config.stack_trace_config is not None
       and debug_config.stack_trace_config.collect_stack_trace
   ):
-    disable_stack_trace_dumping()
+    disable_stack_trace_dumping(debug_config.stack_trace_config)
 
 
 def send_user_signal(stack_trace_interval_seconds):
   """Send SIGUSR1 signal to non-daemon threads after every stack_trace_interval_seconds seconds."""
   while True:
     time.sleep(stack_trace_interval_seconds)
     for thread in threading.enumerate():
```

### Comparing `cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/stack_trace.py` & `cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/stack_trace.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,19 +37,26 @@
     faulthandler.register(
         signal.SIGUSR1, all_threads=False, file=_stack_trace_file_obj
     )
   except Exception as e:  # pylint: disable=broad-exception-caught
     logger.error("Error in enabling dumping of stack trace.", e)
 
 
-def disable_stack_trace_dumping():
-  """Disable faulthandler and unregister user signals."""
+def disable_stack_trace_dumping(stack_trace_config):
+  """Disable faulthandler and unregister user signals.
+
+  Args:
+    stack_trace_config: configuration object for stack trace collection
+  """
   try:
     global _stack_trace_file_obj
-    if _stack_trace_file_obj is not None:
+    if (
+        stack_trace_config.stack_trace_to_cloud
+        and _stack_trace_file_obj is not None
+    ):
       _stack_trace_file_obj.close()
       _stack_trace_file_obj = None
 
     faulthandler.unregister(signal.SIGUSR1)
     faulthandler.disable()
   except Exception as e:  # pylint: disable=broad-exception-caught
     logger.error("Error in disabling dumping of stack trace.", e)
```

### Comparing `cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/src/util/stack_trace_test_util.py` & `cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/src/util/stack_trace_test_util.py`

 * *Files identical despite different names*

### Comparing `cloud_tpu_diagnostics-0.1.0/cloud_tpu_diagnostics/tests/stack_trace_test.py` & `cloud_tpu_diagnostics-0.1.1/cloud_tpu_diagnostics/tests/stack_trace_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import faulthandler
 import os
 import shutil
 import signal
 import subprocess
 import sys
 import textwrap
 import unittest
 from absl.testing import absltest
+from cloud_tpu_diagnostics.src.config import stack_trace_configuration
+from cloud_tpu_diagnostics.src.stack_trace import disable_stack_trace_dumping
+from cloud_tpu_diagnostics.src.stack_trace import enable_stack_trace_dumping
 from cloud_tpu_diagnostics.src.util import default
 
 class StackTraceTest(absltest.TestCase):
 
   def setUp(self):
     super().setUp()
     package_dir = '/'.join(os.path.dirname(__file__).split('/')[:-1])
@@ -76,14 +80,33 @@
 
   def testCollectStackTraceFalseNoTraceCollectedOnConsole(self):
     process = self.run_python_code('', False, False)
     _, stderr = process.communicate()
     self.assertEmpty(stderr)
     self.assertFalse(os.path.exists(default.STACK_TRACE_DIR_DEFAULT))
 
+  def testEnableStackTraceDumpingFaulthandlerEnabled(self):
+    stack_trace_config = stack_trace_configuration.StackTraceConfig(
+        collect_stack_trace=True, stack_trace_to_cloud=True
+    )
+    with self.assertLogs(level='INFO') as log:
+      enable_stack_trace_dumping(stack_trace_config)
+    self.assertEqual(faulthandler.is_enabled(), True)
+    self.assertRegex(
+        log.output[0], 'Stack trace will be written in: /tmp/debugging/'
+    )
+
+  def testDisableStackTraceDumpingFaulthandlerDisabled(self):
+    stack_trace_config = stack_trace_configuration.StackTraceConfig(
+        collect_stack_trace=True, stack_trace_to_cloud=True
+    )
+    enable_stack_trace_dumping(stack_trace_config)
+    disable_stack_trace_dumping(stack_trace_config)
+    self.assertEqual(faulthandler.is_enabled(), False)
+
   def check_fatal_error(self, line_number, error, signal_name, log_to_cloud):
     header = r'Stack \(most recent call first\)'
     regex = ''
     if error:
       regex = """
           {error}
           """
```

### Comparing `cloud_tpu_diagnostics-0.1.0/pyproject.toml` & `cloud_tpu_diagnostics-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cloud-tpu-diagnostics"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Cloud TPU Team", email="cloud-tpu-eng@google.com" },
 ]
 description = "Monitor, debug and profile the jobs running on Cloud TPU."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
```

### Comparing `cloud_tpu_diagnostics-0.1.0/PKG-INFO` & `cloud_tpu_diagnostics-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-tpu-diagnostics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Monitor, debug and profile the jobs running on Cloud TPU.
 Keywords: 
 Author-email: Cloud TPU Team <cloud-tpu-eng@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -62,15 +62,20 @@
 ##### Scenario 3: Collect stack traces on faults and upload on cloud
 
 ```
 stack_trace_config = stack_trace_configuration.StackTraceConfig(
                       collect_stack_trace=True,
                       stack_trace_to_cloud=True)
 ```
-This configuration will temporary collect stack traces inside `/tmp/debugging` directory on TPU host if there is a fault or process hang. Additionally, the traces collected in TPU host memory will be uploaded to Google Cloud Logging, which will make it easier to troubleshoot and fix the problems.
+This configuration will temporary collect stack traces inside `/tmp/debugging` directory on TPU host if there is a fault or process hang. Additionally, the traces collected in TPU host memory will be uploaded to Google Cloud Logging, which will make it easier to troubleshoot and fix the problems. You can view the traces in [Logs Explorer](https://cloud.google.com/logging/docs/view/logs-explorer-interface) using the following query:
+
+```
+logName="projects/<project_name>/logs/tpu.googleapis.com%2Fruntime_monitor"
+jsonPayload.verb="stacktraceanalyzer"
+```
 
 By default, stack traces will be collected every 10 minutes. In order to change the duration between two stack trace collection events, add the following configuration:
 
 ```
 stack_trace_config = stack_trace_configuration.StackTraceConfig(
                       collect_stack_trace=True,
                       stack_trace_to_cloud=True,
```

