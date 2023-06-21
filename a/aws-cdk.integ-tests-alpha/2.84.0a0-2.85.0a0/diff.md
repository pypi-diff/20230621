# Comparing `tmp/aws-cdk.integ-tests-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.integ-tests-alpha-2.85.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.84.0a0.tar", last modified: Tue Jun 13 23:46:46 2023, max compression
+gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.85.0a0.tar", last modified: Wed Jun 21 13:32:08 2023, max compression
```

## Comparing `aws-cdk.integ-tests-alpha-2.84.0a0.tar` & `aws-cdk.integ-tests-alpha-2.85.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    16319 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15326 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1862 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/
--rw-r--r--   0 root         (0) root         (0)   225405 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146957 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16319 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:46.000000 aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    16501 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15508 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/
+-rw-r--r--   0 root         (0) root         (0)   227828 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   147040 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.85.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16501 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/LICENSE` & `aws-cdk.integ-tests-alpha-2.85.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.85.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -89,16 +89,16 @@
 ### IntegTest
 
 Suppose you have a simple stack, that only encapsulates a Lambda function with a
 certain handler:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
@@ -107,16 +107,16 @@
 You may want to test this stack under different conditions. For example, we want
 this stack to be deployed correctly, regardless of the architecture we choose
 for the Lambda function. In particular, it should work for both `ARM_64` and
 `X86_64`. So you can create an `IntegTestCase` that exercises both scenarios:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/README.md` & `aws-cdk.integ-tests-alpha-2.85.0a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 ### IntegTest
 
 Suppose you have a simple stack, that only encapsulates a Lambda function with a
 certain handler:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
@@ -80,16 +80,16 @@
 You may want to test this stack under different conditions. For example, we want
 this stack to be deployed correctly, regardless of the architecture we choose
 for the Lambda function. In particular, it should work for both `ARM_64` and
 `X86_64`. So you can create an `IntegTestCase` that exercises both scenarios:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/setup.py` & `aws-cdk.integ-tests-alpha-2.85.0a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.integ-tests-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.85.0.a0",
     "description": "CDK Integration Testing Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.integ_tests_alpha",
         "aws_cdk.integ_tests_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.integ_tests_alpha._jsii": [
-            "integ-tests-alpha@2.84.0-alpha.0.jsii.tgz"
+            "integ-tests-alpha@2.85.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.integ_tests_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.84.0",
+        "aws-cdk-lib==2.85.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk/integ_tests_alpha/__init__.py` & `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 ### IntegTest
 
 Suppose you have a simple stack, that only encapsulates a Lambda function with a
 certain handler:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
@@ -81,16 +81,16 @@
 You may want to test this stack under different conditions. For example, we want
 this stack to be deployed correctly, regardless of the architecture we choose
 for the Lambda function. In particular, it should work for both `ARM_64` and
 `X86_64`. So you can create an `IntegTestCase` that exercises both scenarios:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
@@ -3037,14 +3037,15 @@
         stack_update_workflow: typing.Optional[builtins.bool] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
@@ -3056,14 +3057,15 @@
         :param stack_update_workflow: Run update workflow on this test case This should only be set to false to test scenarios that are not possible to test as part of the update workflow. Default: true
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
 
         :stability: experimental
         '''
         if __debug__:
@@ -3079,14 +3081,15 @@
             stack_update_workflow=stack_update_workflow,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -3129,14 +3132,15 @@
         "stack_update_workflow": "stackUpdateWorkflow",
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
     },
 )
 class IntegTestCaseStackProps(
     _aws_cdk_cloud_assembly_schema_ceddda9d.TestOptions,
@@ -3153,14 +3157,15 @@
         stack_update_workflow: typing.Optional[builtins.bool] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Properties of an integration test case stack.
 
         :param allow_destroy: List of CloudFormation resource types in this stack that can be destroyed as part of an update without failing the test. This list should only include resources that for this specific integration test we are sure will not cause errors or an outage if destroyed. For example, maybe we know that a new resource will be created first before the old resource is destroyed which prevents any outage. e.g. ['AWS::IAM::Role'] Default: - do not allow destruction of any resources on update
@@ -3171,14 +3176,15 @@
         :param stack_update_workflow: Run update workflow on this test case This should only be set to false to test scenarios that are not possible to test as part of the update workflow. Default: true
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
 
         :stability: experimental
         :exampleMetadata: infused
 
@@ -3209,14 +3215,15 @@
             check_type(argname="argument stack_update_workflow", value=stack_update_workflow, expected_type=type_hints["stack_update_workflow"])
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if allow_destroy is not None:
             self._values["allow_destroy"] = allow_destroy
         if cdk_command_options is not None:
@@ -3237,14 +3244,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
 
@@ -3438,14 +3447,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -5263,14 +5285,15 @@
     stack_update_workflow: typing.Optional[builtins.bool] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -5290,14 +5313,15 @@
     stack_update_workflow: typing.Optional[builtins.bool] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -89,16 +89,16 @@
 ### IntegTest
 
 Suppose you have a simple stack, that only encapsulates a Lambda function with a
 certain handler:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
@@ -107,16 +107,16 @@
 You may want to test this stack under different conditions. For example, we want
 this stack to be deployed correctly, regardless of the architecture we choose
 for the Lambda function. In particular, it should work for both `ARM_64` and
 `X86_64`. So you can create an `IntegTestCase` that exercises both scenarios:
 
 ```python
 class StackUnderTest(Stack):
-    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, architecture=None, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, architecture=architecture, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
         lambda_.Function(self, "Handler",
             runtime=lambda_.Runtime.NODEJS_14_X,
             handler="index.handler",
             code=lambda_.Code.from_asset(path.join(__dirname, "lambda-handler")),
             architecture=architecture
         )
```

### Comparing `aws-cdk.integ-tests-alpha-2.84.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt` & `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
 src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
 src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
 src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
 src/aws_cdk/integ_tests_alpha/__init__.py
 src/aws_cdk/integ_tests_alpha/py.typed
 src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
-src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.85.0-alpha.0.jsii.tgz
```

