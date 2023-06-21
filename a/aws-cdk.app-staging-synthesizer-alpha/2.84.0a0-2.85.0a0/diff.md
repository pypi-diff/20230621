# Comparing `tmp/aws-cdk.app-staging-synthesizer-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.app-staging-synthesizer-alpha-2.85.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer-", last modified: Tue Jun 13 23:47:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer-", last modified: Wed Jun 21 13:32:27 2023, max compression
```

## Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0.tar` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25587 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24567 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1949 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
--rw-r--r--   0 root         (0) root         (0)   177977 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78091 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25587 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:06.000000 aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24658 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
+-rw-r--r--   0 root         (0) root         (0)   186549 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81210 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/LICENSE` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/PKG-INFO` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-staging-synthesizer-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: Cdk synthesizer for with app-scoped staging stack
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -347,16 +347,16 @@
 ```
 
 Or you can roll your own staging resources from scratch, as long as it implements `IStagingResources`.
 
 ```python
 @jsii.implements(IStagingResources)
 class CustomStagingStack(Stack):
-    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
     def add_file(self, *, sourceHash, executable=None, fileName=None, packaging=None, deployTime=None):
         return FileStagingLocation(
             bucket_name="myBucket",
             assume_role_arn="myArn",
             dependency_stack=self
         )
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/README.md` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -320,16 +320,16 @@
 ```
 
 Or you can roll your own staging resources from scratch, as long as it implements `IStagingResources`.
 
 ```python
 @jsii.implements(IStagingResources)
 class CustomStagingStack(Stack):
-    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
     def add_file(self, *, sourceHash, executable=None, fileName=None, packaging=None, deployTime=None):
         return FileStagingLocation(
             bucket_name="myBucket",
             assume_role_arn="myArn",
             dependency_stack=self
         )
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/setup.py` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.app-staging-synthesizer-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.85.0.a0",
     "description": "Cdk synthesizer for with app-scoped staging stack",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.app_staging_synthesizer_alpha",
         "aws_cdk.app_staging_synthesizer_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.app_staging_synthesizer_alpha._jsii": [
-            "app-staging-synthesizer-alpha@2.84.0-alpha.0.jsii.tgz"
+            "app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.app_staging_synthesizer_alpha": [
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

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,16 +321,16 @@
 ```
 
 Or you can roll your own staging resources from scratch, as long as it implements `IStagingResources`.
 
 ```python
 @jsii.implements(IStagingResources)
 class CustomStagingStack(Stack):
-    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
     def add_file(self, *, sourceHash, executable=None, fileName=None, packaging=None, deployTime=None):
         return FileStagingLocation(
             bucket_name="myBucket",
             assume_role_arn="myArn",
             dependency_stack=self
         )
@@ -504,37 +504,40 @@
     @builtins.classmethod
     def default_resources(
         cls,
         *,
         bootstrap_qualifier: typing.Optional[builtins.str] = None,
         deployment_identities: typing.Optional["DeploymentIdentities"] = None,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional["BootstrapRole"] = None,
         image_asset_publishing_role: typing.Optional["BootstrapRole"] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
     ) -> "AppStagingSynthesizer":
         '''(experimental) Use the Default Staging Resources, creating a single stack per environment this app is deployed in.
 
         :param bootstrap_qualifier: (experimental) Qualifier to disambiguate multiple bootstrapped environments in the same account. This qualifier is only used to reference bootstrapped resources. It will not be used in the creation of app-specific staging resources: ``appId`` is used for that instead. Default: - Value of context key '@aws-cdk/core:bootstrapQualifier' if set, otherwise ``DEFAULT_QUALIFIER``
         :param deployment_identities: (experimental) What roles to use to deploy applications. These are the roles that have permissions to interact with CloudFormation on your behalf. By default these are the standard bootstrapped CDK roles, but you can customize them or turn them off and use the CLI credentials to deploy. Default: - The standard bootstrapped CDK roles
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
 
         :stability: experimental
         '''
         options = DefaultResourcesOptions(
             bootstrap_qualifier=bootstrap_qualifier,
             deployment_identities=deployment_identities,
             app_id=app_id,
+            auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
         )
 
@@ -1184,35 +1187,38 @@
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/app-staging-synthesizer-alpha.DefaultStagingStackOptions",
     jsii_struct_bases=[],
     name_mapping={
         "app_id": "appId",
+        "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
     },
 )
 class DefaultStagingStackOptions:
     def __init__(
         self,
         *,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) User configurable options to the DefaultStagingStack.
 
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
 
         :stability: experimental
@@ -1221,22 +1227,25 @@
         Example::
 
             default_staging_stack = DefaultStagingStack.factory(app_id="my-app-id")
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__09dbc6ce5bcfd58fa48337caac574e10727d4bf9a43dc89866fbe7541b026219)
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "app_id": app_id,
         }
+        if auto_delete_staging_assets is not None:
+            self._values["auto_delete_staging_assets"] = auto_delete_staging_assets
         if deploy_time_file_asset_lifetime is not None:
             self._values["deploy_time_file_asset_lifetime"] = deploy_time_file_asset_lifetime
         if file_asset_publishing_role is not None:
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
@@ -1257,14 +1266,25 @@
         :stability: experimental
         '''
         result = self._values.get("app_id")
         assert result is not None, "Required property 'app_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def auto_delete_staging_assets(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("auto_delete_staging_assets")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def deploy_time_file_asset_lifetime(
         self,
     ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) The lifetime for deploy time file assets.
 
         Assets that are only necessary at deployment time (for instance,
         CloudFormation templates and Lambda source code bundles) will be
@@ -1345,25 +1365,27 @@
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/app-staging-synthesizer-alpha.DefaultStagingStackProps",
     jsii_struct_bases=[DefaultStagingStackOptions, _aws_cdk_ceddda9d.StackProps],
     name_mapping={
         "app_id": "appId",
+        "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
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
         "qualifier": "qualifier",
         "deploy_role_arn": "deployRoleArn",
     },
 )
@@ -1371,45 +1393,49 @@
     DefaultStagingStackOptions,
     _aws_cdk_ceddda9d.StackProps,
 ):
     def __init__(
         self,
         *,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
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
         qualifier: builtins.str,
         deploy_role_arn: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Default Staging Stack Properties.
 
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
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
         :param qualifier: (experimental) The qualifier used to specialize strings. Shouldn't be necessary but who knows what people might do.
         :param deploy_role_arn: (experimental) The ARN of the deploy action role, if given. This role will need permissions to read from to the staging resources. Default: - The CLI credentials are assumed, no additional permissions are granted.
 
         :stability: experimental
@@ -1428,60 +1454,66 @@
             
             default_staging_stack_props = app_staging_synthesizer_alpha.DefaultStagingStackProps(
                 app_id="appId",
                 qualifier="qualifier",
             
                 # the properties below are optional
                 analytics_reporting=False,
+                auto_delete_staging_assets=False,
                 cross_region_references=False,
                 deploy_role_arn="deployRoleArn",
                 deploy_time_file_asset_lifetime=cdk.Duration.minutes(30),
                 description="description",
                 env=cdk.Environment(
                     account="account",
                     region="region"
                 ),
                 file_asset_publishing_role=bootstrap_role,
                 image_asset_publishing_role=bootstrap_role,
                 image_asset_version_count=123,
                 permissions_boundary=permissions_boundary,
                 stack_name="stackName",
                 staging_bucket_name="stagingBucketName",
+                suppress_template_indentation=False,
                 synthesizer=stack_synthesizer,
                 tags={
                     "tags_key": "tags"
                 },
                 termination_protection=False
             )
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ac9f132bcac8375ac08c16bf3c9bb7407b641e71cfd23cea8b50befa3cf79bbf)
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
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
             check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
             check_type(argname="argument deploy_role_arn", value=deploy_role_arn, expected_type=type_hints["deploy_role_arn"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "app_id": app_id,
             "qualifier": qualifier,
         }
+        if auto_delete_staging_assets is not None:
+            self._values["auto_delete_staging_assets"] = auto_delete_staging_assets
         if deploy_time_file_asset_lifetime is not None:
             self._values["deploy_time_file_asset_lifetime"] = deploy_time_file_asset_lifetime
         if file_asset_publishing_role is not None:
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
@@ -1496,14 +1528,16 @@
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
         if deploy_role_arn is not None:
@@ -1522,14 +1556,25 @@
         :stability: experimental
         '''
         result = self._values.get("app_id")
         assert result is not None, "Required property 'app_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def auto_delete_staging_assets(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("auto_delete_staging_assets")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def deploy_time_file_asset_lifetime(
         self,
     ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) The lifetime for deploy time file assets.
 
         Assets that are only necessary at deployment time (for instance,
         CloudFormation templates and Lambda source code bundles) will be
@@ -1719,14 +1764,27 @@
 
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
 
@@ -2516,46 +2574,88 @@
 
     def __repr__(self) -> str:
         return "StagingRoles(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class UsingAppStagingSynthesizer(
+    _constructs_77d1e7e8.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-cdk/app-staging-synthesizer-alpha.UsingAppStagingSynthesizer",
+):
+    '''(experimental) This is a dummy construct meant to signify that a stack is utilizing the AppStagingSynthesizer.
+
+    It does not do anything, and is not meant
+    to be created on its own. This construct will be a part of the
+    construct tree only and not the Cfn template. The construct tree is
+    then encoded in the AWS::CDK::Metadata resource of the stack and
+    injested in our metrics like every other construct.
+
+    :stability: experimental
+    :exampleMetadata: fixture=_generated
+
+    Example::
+
+        # The code below shows an example of how to instantiate this type.
+        # The values are placeholders you should change.
+        import aws_cdk.app_staging_synthesizer_alpha as app_staging_synthesizer_alpha
+        
+        using_app_staging_synthesizer = app_staging_synthesizer_alpha.UsingAppStagingSynthesizer(self, "MyUsingAppStagingSynthesizer")
+    '''
+
+    def __init__(self, scope: _constructs_77d1e7e8.Construct, id: builtins.str) -> None:
+        '''
+        :param scope: -
+        :param id: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2450a25d8e0af64a0996ad931b80e0eac3d8b11c4c148ebd044357f128d25670)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        jsii.create(self.__class__, self, [scope, id])
+
+
 @jsii.data_type(
     jsii_type="@aws-cdk/app-staging-synthesizer-alpha.DefaultResourcesOptions",
     jsii_struct_bases=[AppStagingSynthesizerOptions, DefaultStagingStackOptions],
     name_mapping={
         "bootstrap_qualifier": "bootstrapQualifier",
         "deployment_identities": "deploymentIdentities",
         "app_id": "appId",
+        "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
     },
 )
 class DefaultResourcesOptions(AppStagingSynthesizerOptions, DefaultStagingStackOptions):
     def __init__(
         self,
         *,
         bootstrap_qualifier: typing.Optional[builtins.str] = None,
         deployment_identities: typing.Optional[DeploymentIdentities] = None,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for stackPerEnv static method.
 
         :param bootstrap_qualifier: (experimental) Qualifier to disambiguate multiple bootstrapped environments in the same account. This qualifier is only used to reference bootstrapped resources. It will not be used in the creation of app-specific staging resources: ``appId`` is used for that instead. Default: - Value of context key '@aws-cdk/core:bootstrapQualifier' if set, otherwise ``DEFAULT_QUALIFIER``
         :param deployment_identities: (experimental) What roles to use to deploy applications. These are the roles that have permissions to interact with CloudFormation on your behalf. By default these are the standard bootstrapped CDK roles, but you can customize them or turn them off and use the CLI credentials to deploy. Default: - The standard bootstrapped CDK roles
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
 
         :stability: experimental
@@ -2572,26 +2672,29 @@
             )
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__29102b1165011d046c95963e887fe565a9300d7ed93d8499af73ef05f0e32e60)
             check_type(argname="argument bootstrap_qualifier", value=bootstrap_qualifier, expected_type=type_hints["bootstrap_qualifier"])
             check_type(argname="argument deployment_identities", value=deployment_identities, expected_type=type_hints["deployment_identities"])
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "app_id": app_id,
         }
         if bootstrap_qualifier is not None:
             self._values["bootstrap_qualifier"] = bootstrap_qualifier
         if deployment_identities is not None:
             self._values["deployment_identities"] = deployment_identities
+        if auto_delete_staging_assets is not None:
+            self._values["auto_delete_staging_assets"] = auto_delete_staging_assets
         if deploy_time_file_asset_lifetime is not None:
             self._values["deploy_time_file_asset_lifetime"] = deploy_time_file_asset_lifetime
         if file_asset_publishing_role is not None:
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
@@ -2643,14 +2746,25 @@
         :stability: experimental
         '''
         result = self._values.get("app_id")
         assert result is not None, "Required property 'app_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def auto_delete_staging_assets(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("auto_delete_staging_assets")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def deploy_time_file_asset_lifetime(
         self,
     ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) The lifetime for deploy time file assets.
 
         Assets that are only necessary at deployment time (for instance,
         CloudFormation templates and Lambda source code bundles) will be
@@ -2749,103 +2863,112 @@
         self,
         scope: _aws_cdk_ceddda9d.App,
         id: builtins.str,
         *,
         qualifier: builtins.str,
         deploy_role_arn: typing.Optional[builtins.str] = None,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
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
         :param qualifier: (experimental) The qualifier used to specialize strings. Shouldn't be necessary but who knows what people might do.
         :param deploy_role_arn: (experimental) The ARN of the deploy action role, if given. This role will need permissions to read from to the staging resources. Default: - The CLI credentials are assumed, no additional permissions are granted.
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
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
             type_hints = typing.get_type_hints(_typecheckingstub__ca741a4572a1f95a8d82e9d029388b8a2d72acacb69715277b6a785b4968e662)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DefaultStagingStackProps(
             qualifier=qualifier,
             deploy_role_arn=deploy_role_arn,
             app_id=app_id,
+            auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
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
 
     @jsii.member(jsii_name="factory")
     @builtins.classmethod
     def factory(
         cls,
         *,
         app_id: builtins.str,
+        auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
     ) -> IStagingResourcesFactory:
         '''(experimental) Return a factory that will create DefaultStagingStacks.
 
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
+        :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
 
         :stability: experimental
         '''
         options = DefaultStagingStackOptions(
             app_id=app_id,
+            auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
         )
 
@@ -2979,14 +3102,15 @@
     "DeploymentIdentities",
     "FileStagingLocation",
     "IStagingResources",
     "IStagingResourcesFactory",
     "ImageStagingLocation",
     "ObtainStagingResourcesContext",
     "StagingRoles",
+    "UsingAppStagingSynthesizer",
 ]
 
 publication.publish()
 
 def _typecheckingstub__95a4aa84673edcde5f9edcbb6e0abc3d396e902014631ead660cc26b087ff3aa(
     _stack: _aws_cdk_ceddda9d.Stack,
 ) -> None:
@@ -3046,37 +3170,40 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__09dbc6ce5bcfd58fa48337caac574e10727d4bf9a43dc89866fbe7541b026219(
     *,
     app_id: builtins.str,
+    auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ac9f132bcac8375ac08c16bf3c9bb7407b641e71cfd23cea8b50befa3cf79bbf(
     *,
     app_id: builtins.str,
+    auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
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
     qualifier: builtins.str,
     deploy_role_arn: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
@@ -3124,19 +3251,27 @@
     *,
     docker_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__2450a25d8e0af64a0996ad931b80e0eac3d8b11c4c148ebd044357f128d25670(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__29102b1165011d046c95963e887fe565a9300d7ed93d8499af73ef05f0e32e60(
     *,
     bootstrap_qualifier: typing.Optional[builtins.str] = None,
     deployment_identities: typing.Optional[DeploymentIdentities] = None,
     app_id: builtins.str,
+    auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
@@ -3145,24 +3280,26 @@
 def _typecheckingstub__ca741a4572a1f95a8d82e9d029388b8a2d72acacb69715277b6a785b4968e662(
     scope: _aws_cdk_ceddda9d.App,
     id: builtins.str,
     *,
     qualifier: builtins.str,
     deploy_role_arn: typing.Optional[builtins.str] = None,
     app_id: builtins.str,
+    auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
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

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-staging-synthesizer-alpha
-Version: 2.84.0a0
+Version: 2.85.0a0
 Summary: Cdk synthesizer for with app-scoped staging stack
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -347,16 +347,16 @@
 ```
 
 Or you can roll your own staging resources from scratch, as long as it implements `IStagingResources`.
 
 ```python
 @jsii.implements(IStagingResources)
 class CustomStagingStack(Stack):
-    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None):
-        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary)
+    def __init__(self, scope, id, *, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+        super().__init__(scope, id, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
 
     def add_file(self, *, sourceHash, executable=None, fileName=None, packaging=None, deployTime=None):
         return FileStagingLocation(
             bucket_name="myBucket",
             assume_role_arn="myArn",
             dependency_stack=self
         )
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.84.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt` & `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
 src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
 src/aws_cdk/app_staging_synthesizer_alpha/py.typed
 src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
-src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz
```

