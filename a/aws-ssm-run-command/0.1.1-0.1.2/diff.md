# Comparing `tmp/aws_ssm_run_command-0.1.1.tar.gz` & `tmp/aws_ssm_run_command-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_run_command-0.1.1.tar", last modified: Mon Jun 19 03:41:12 2023, max compression
+gzip compressed data, was "aws_ssm_run_command-0.1.2.tar", last modified: Wed Jun 21 14:18:55 2023, max compression
```

## Comparing `aws_ssm_run_command-0.1.1.tar` & `aws_ssm_run_command-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.367284 aws_ssm_run_command-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-19 03:41:12.367097 aws_ssm_run_command-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2979 2023-06-19 03:39:39.000000 aws_ssm_run_command-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.361865 aws_ssm_run_command-0.1.1/aws_ssm_run_command/
--rw-r--r--   0 sanhehu    (501) staff       (20)      331 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-19 03:32:02.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.363579 aws_ssm_run_command-0.1.1/aws_ssm_run_command/better_boto/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-19 02:18:57.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/better_boto/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-06-19 02:33:36.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/better_boto/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4635 2023-06-19 02:33:22.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/better_boto/aws_ssm_send_command.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.364035 aws_ssm_run_command-0.1.1/aws_ssm_run_command/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.365408 aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:13:56.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       92 2023-06-19 03:34:31.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7974 2023-06-19 03:30:56.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/run_command_on_one_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      147 2023-06-19 03:34:15.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/run_command_on_one_ec2_api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.365876 aws_ssm_run_command-0.1.1/aws_ssm_run_command/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.366412 aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-18 23:14:42.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.362861 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-19 03:41:12.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1101 2023-06-19 03:41:12.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 03:41:12.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-19 03:41:12.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-19 03:41:12.000000 aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      990 2023-06-19 03:36:56.000000 aws_ssm_run_command-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      445 2023-06-19 03:40:42.000000 aws_ssm_run_command-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       36 2023-06-19 03:31:19.000000 aws_ssm_run_command-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 03:41:12.367351 aws_ssm_run_command-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 03:41:12.366670 aws_ssm_run_command-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      618 2023-06-19 03:35:27.000000 aws_ssm_run_command-0.1.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.155211 aws_ssm_run_command-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-21 14:18:55.155083 aws_ssm_run_command-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2979 2023-06-19 03:39:39.000000 aws_ssm_run_command-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.150489 aws_ssm_run_command-0.1.2/aws_ssm_run_command/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      331 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-21 14:13:12.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-19 03:32:02.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.152260 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-19 02:18:57.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-06-19 02:33:36.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5165 2023-06-21 14:15:03.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/aws_ssm_send_command.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.152510 aws_ssm_run_command-0.1.2/aws_ssm_run_command/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.153563 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:13:56.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       92 2023-06-19 03:34:31.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7974 2023-06-19 03:30:56.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/run_command_on_one_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      147 2023-06-19 03:34:15.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/run_command_on_one_ec2_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154059 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154475 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-18 23:14:42.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.151125 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1101 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1317 2023-06-21 14:16:13.000000 aws_ssm_run_command-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      445 2023-06-19 03:40:42.000000 aws_ssm_run_command-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       36 2023-06-19 03:31:19.000000 aws_ssm_run_command-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-21 14:18:55.155251 aws_ssm_run_command-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154817 aws_ssm_run_command-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      618 2023-06-19 03:35:27.000000 aws_ssm_run_command-0.1.2/tests/test_api.py
```

### Comparing `aws_ssm_run_command-0.1.1/AUTHORS.rst` & `aws_ssm_run_command-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/LICENSE.txt` & `aws_ssm_run_command-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/PKG-INFO` & `aws_ssm_run_command-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_ssm_run_command
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_ssm_run_command-project
-Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_ssm_run_command-0.1.1/README.rst` & `aws_ssm_run_command-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command/better_boto/aws_ssm_send_command.py` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/aws_ssm_send_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -118,25 +118,37 @@
         return dataclasses.asdict(self)
 
 
 def wait_until_command_succeeded(
     ssm_client: "SSMClient",
     command_id: str,
     instance_id: str,
+    raises: bool = True,
     delays: int = 3,
     timeout: int = 60,
     verbose: bool = True,
 ) -> CommandInvocation:
     """
     After you call send_command_ API, you can use this function to wait until
     it succeeds. If it fails, it will raise an exception.
 
     Reference:
 
     - get_command_invocation_
+
+    :param ssm_client:
+    :param command_id: the SSM run command "command_id", it is from the
+        ssm_client.send_command(...) response
+    :param instance_id: ec2 instance id
+    :param raises: if True, then raises error if command failed,
+        otherwise, just return the :class:`CommandInvocation` represents the failed
+        invocation.
+    :param delays:
+    :param timeout:
+    :param verbose:
     """
     for _ in Waiter(delays=delays, timeout=timeout, verbose=verbose):
         command_invocation = CommandInvocation.get(
             ssm_client=ssm_client,
             command_id=command_id,
             instance_id=instance_id,
         )
@@ -145,12 +157,15 @@
             return command_invocation
         elif command_invocation.Status in [
             CommandInvocationStatusEnum.Cancelled.value,
             CommandInvocationStatusEnum.TimedOut.value,
             CommandInvocationStatusEnum.Failed.value,
             CommandInvocationStatusEnum.Cancelling.value,
         ]:
-            raise CommandInvocationFailedError(
-                f"Command failed, status: {command_invocation.Status}"
-            )
+            if raises:
+                raise CommandInvocationFailedError(
+                    f"Command failed, status: {command_invocation.Status}"
+                )
+            else:
+                return command_invocation
         else:
             pass
```

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command/paths.py` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command/paths.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command/patterns/run_command_on_one_ec2.py` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/run_command_on_one_ec2.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/pytest_cov_helper.py` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command/vendor/waiter.py` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/PKG-INFO` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-ssm-run-command
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_ssm_run_command-project
-Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_ssm_run_command-0.1.1/aws_ssm_run_command.egg-info/SOURCES.txt` & `aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/release-history.rst` & `aws_ssm_run_command-0.1.2/release-history.rst`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.2 (2023-06-21)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- add ``raises`` argument to ``aws_ssm_run_command.api.better_boto.wait_until_command_succeeded`` function. Allow user to specify whether to raise an exception if the command fails. Default to ``True``.
+
+
 0.1.1 (2023-06-18)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 - First release
 - Add the following public api:
     - ``aws_ssm_run_command.api.better_boto.CommandInvocationFailedError``
     - ``aws_ssm_run_command.api.better_boto.send_command``
     - ``aws_ssm_run_command.api.better_boto.CommandInvocationStatusEnum``
```

### Comparing `aws_ssm_run_command-0.1.1/requirements-doc.txt` & `aws_ssm_run_command-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/setup.py` & `aws_ssm_run_command-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.1/tests/test_api.py` & `aws_ssm_run_command-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

