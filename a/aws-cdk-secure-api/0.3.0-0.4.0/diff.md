# Comparing `tmp/aws-cdk-secure-api-0.3.0.tar.gz` & `tmp/aws-cdk-secure-api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-secure-api-0.3.0.tar", last modified: Wed May 17 18:45:25 2023, max compression
+gzip compressed data, was "aws-cdk-secure-api-0.4.0.tar", last modified: Wed Jun 21 19:16:49 2023, max compression
```

## Comparing `aws-cdk-secure-api-0.3.0.tar` & `aws-cdk-secure-api-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.623929 aws-cdk-secure-api-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-17 18:45:25.623929 aws-cdk-secure-api-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.615928 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/api_construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.619928 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/ssm_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.615928 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 18:45:25.000000 aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.619928 aws-cdk-secure-api-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/aws_cdk_secure_api.aws.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/aws_cdk_secure_api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4918 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-17 18:45:25.623929 aws-cdk-secure-api-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.619928 aws-cdk-secure-api-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:45:25.623929 aws-cdk-secure-api-0.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 18:45:16.000000 aws-cdk-secure-api-0.3.0/tests/unit/test_aws_cdk_secure_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21983 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/api_construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/ssm_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 19:16:49.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4918 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/unit/test_aws_cdk_secure_api.py
```

### Comparing `aws-cdk-secure-api-0.3.0/CONTRIBUTING.rst` & `aws-cdk-secure-api-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/HISTORY.rst` & `aws-cdk-secure-api-0.4.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/LICENSE` & `aws-cdk-secure-api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/PKG-INFO` & `aws-cdk-secure-api-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -34,36 +34,52 @@
         
         An unofficial `AWS CDK v2`_ Construct Library for Secure REST APIs.
         
         * Documentation: https://aws-cdk-secure-api.readthedocs.io.
         
         .. _`AWS CDK v2`: https://aws.amazon.com/about-aws/whats-new/2021/12/aws-cloud-development-kit-cdk-generally-available/
         
-        Secure Rest Api
-        ---------------
-        
-        The ``SecureRestApi`` construct creates a (public) REST API secured behind an API key, which needs to be
-        specified in the ``x-api-key`` header for all requests.
-        
         Install
         -------
         
         .. code-block:: console
         
             pip install aws-cdk-secure-api
         
+        Constructs
+        ----------
+        
+        * ``SecureRestApi`` - A construct to create a (public) REST API secured behind an API key, which needs to be
+          specified in the ``x-api-key`` header for all requests.
+        
+        * ``IAMSecureRestApi`` - A construct to create a (public) REST API secured behind `AWS IAM authentication`_, which
+          requires IAM credentials `to be signed`_ and included in all requests.
+        
+        .. _to be signed: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control-iam.html
+        
         Features
         --------
         
-        * A CDK Construct which sets up a `RestApi`_ secured behind an API key.
-        * An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
-          a free service) as needed.
-        * Local cache for the API key, so that API calls are not needed in future
-          CDK deployments.
-        * Helper methods for ``SecureRestApi``, to make it easier to
+        * A CDK Construct which sets up a `RestApi`_ secured behind (one of):
+        
+          * API key
+        
+            * An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
+              a free service) as needed.
+        
+            * Local cache for the API key, so that API calls are not needed in future
+              CDK deployments.
+        
+          * `AWS IAM authentication`_
+        
+            * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+        
+            * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
+        
+        * Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
           integrate a method for an AWS Lambda function for example.
         
         .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
         .. _`auto-generated`: https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetRandomPassword.html
         
         Usage
         -----
@@ -106,14 +122,46 @@
         .. code:: python3
         
             # GET /path1
             api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
             # PUT /path2, POST /path2
             api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
         
+        The ``IAMSecureRestApi`` construct represents a Secure REST API in Amazon API Gateway,
+        which requires IAM Authorization.
+        
+        **Using a custom-named resource**:
+        
+        .. code:: python3
+        
+            from aws_cdk.aws_apigateway import StageOptions
+            from aws_cdk.aws_lambda import Function, Runtime
+        
+            from aws_cdk_secure_api import Http, IAMConfig, IAMSecureRestApi
+        
+            # noinspection PyTypeChecker
+            py_runtime: Runtime = Runtime.PYTHON_3_10
+        
+            get_handler = Function(self, 'lambda1', runtime=py_runtime, ...)
+            put_handler = Function(self, 'lambda2', runtime=py_runtime, ...)
+        
+            api = IAMSecureRestApi(
+                self, 'api',
+                rest_api_name='My IAM Secure Service',
+                # optional: specify the name of secret to store IAM User Credentials
+                config=IAMConfig(secret_name='my-stack/iam-user-access-keys'),
+                # optional: specify a deployment stage
+                deploy_options=StageOptions(stage_name='dev')
+            )
+        
+            # GET /path1
+            api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
+            # PUT /path2, POST /path2
+            api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
+        
         AWS Profile
         -----------
         
         Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
         
             cdk deploy --profile my-aws-profile
         
@@ -152,19 +200,23 @@
         
           * *Note:* this output will not show up if ``override_endpoint_name`` is disabled
             in the ``config`` parameter.
         
         * ``APIKey`` - The API key for the endpoint, which needs to be specified
           as a value in an HTTP request's ``x-api-key`` header.
         
+        * ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
+          stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
+        
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
         
+        .. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
         .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
```

### Comparing `aws-cdk-secure-api-0.3.0/README.rst` & `aws-cdk-secure-api-0.4.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -24,36 +24,52 @@
 
 An unofficial `AWS CDK v2`_ Construct Library for Secure REST APIs.
 
 * Documentation: https://aws-cdk-secure-api.readthedocs.io.
 
 .. _`AWS CDK v2`: https://aws.amazon.com/about-aws/whats-new/2021/12/aws-cloud-development-kit-cdk-generally-available/
 
-Secure Rest Api
----------------
-
-The ``SecureRestApi`` construct creates a (public) REST API secured behind an API key, which needs to be
-specified in the ``x-api-key`` header for all requests.
-
 Install
 -------
 
 .. code-block:: console
 
     pip install aws-cdk-secure-api
 
+Constructs
+----------
+
+* ``SecureRestApi`` - A construct to create a (public) REST API secured behind an API key, which needs to be
+  specified in the ``x-api-key`` header for all requests.
+
+* ``IAMSecureRestApi`` - A construct to create a (public) REST API secured behind `AWS IAM authentication`_, which
+  requires IAM credentials `to be signed`_ and included in all requests.
+
+.. _to be signed: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control-iam.html
+
 Features
 --------
 
-* A CDK Construct which sets up a `RestApi`_ secured behind an API key.
-* An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
-  a free service) as needed.
-* Local cache for the API key, so that API calls are not needed in future
-  CDK deployments.
-* Helper methods for ``SecureRestApi``, to make it easier to
+* A CDK Construct which sets up a `RestApi`_ secured behind (one of):
+
+  * API key
+
+    * An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
+      a free service) as needed.
+
+    * Local cache for the API key, so that API calls are not needed in future
+      CDK deployments.
+
+  * `AWS IAM authentication`_
+
+    * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+
+    * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
+
+* Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
   integrate a method for an AWS Lambda function for example.
 
 .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
 .. _`auto-generated`: https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetRandomPassword.html
 
 Usage
 -----
@@ -96,14 +112,46 @@
 .. code:: python3
 
     # GET /path1
     api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
     # PUT /path2, POST /path2
     api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
 
+The ``IAMSecureRestApi`` construct represents a Secure REST API in Amazon API Gateway,
+which requires IAM Authorization.
+
+**Using a custom-named resource**:
+
+.. code:: python3
+
+    from aws_cdk.aws_apigateway import StageOptions
+    from aws_cdk.aws_lambda import Function, Runtime
+
+    from aws_cdk_secure_api import Http, IAMConfig, IAMSecureRestApi
+
+    # noinspection PyTypeChecker
+    py_runtime: Runtime = Runtime.PYTHON_3_10
+
+    get_handler = Function(self, 'lambda1', runtime=py_runtime, ...)
+    put_handler = Function(self, 'lambda2', runtime=py_runtime, ...)
+
+    api = IAMSecureRestApi(
+        self, 'api',
+        rest_api_name='My IAM Secure Service',
+        # optional: specify the name of secret to store IAM User Credentials
+        config=IAMConfig(secret_name='my-stack/iam-user-access-keys'),
+        # optional: specify a deployment stage
+        deploy_options=StageOptions(stage_name='dev')
+    )
+
+    # GET /path1
+    api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
+    # PUT /path2, POST /path2
+    api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
+
 AWS Profile
 -----------
 
 Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
 
     cdk deploy --profile my-aws-profile
 
@@ -142,14 +190,18 @@
 
   * *Note:* this output will not show up if ``override_endpoint_name`` is disabled
     in the ``config`` parameter.
 
 * ``APIKey`` - The API key for the endpoint, which needs to be specified
   as a value in an HTTP request's ``x-api-key`` header.
 
+* ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
+  stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
+
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
 
+.. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
 .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
 .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
```

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/__init__.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 :copyright: (c) 2022 by Ritvik Nag.
 :license:MIT, see LICENSE for more details.
 """
 
 __all__ = [
     'Config',
     'Http',
+    'IAMConfig',
+    'IAMSecureRestApi',
     'SecureRestApi',
 ]
 
 import logging
 
-from .api_construct import SecureRestApi
-from .models import Config, Http
+from .api_construct import IAMSecureRestApi, SecureRestApi
+from .models import Config, Http, IAMConfig
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 # http://docs.python.org/3.3/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger('aws_cdk_secure_api').addHandler(logging.NullHandler())
```

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/client_cache.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/client_cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/secrets_manager.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/aws/ssm_parameter_store.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/ssm_parameter_store.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/cache.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api/models.py` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -40,14 +40,21 @@
         default_factory=lambda: apigateway.QuotaSettings(
             limit=10000000,
             period=apigateway.Period.MONTH,
         ),
     )
 
 
+@dataclass
+class IAMConfig(Config):
+    # secret name to hold the IAM User Credentials (Access Keys) for
+    # invoking the Rest API.
+    secret_name: str | None = None
+
+
 # noinspection PyArgumentList
 class Http(Enum):
     """Enum class to represent an HTTP method."""
     OPTIONS = auto()
     GET = auto()
     HEAD = auto()
     PUT = auto()
```

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/PKG-INFO` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -34,36 +34,52 @@
         
         An unofficial `AWS CDK v2`_ Construct Library for Secure REST APIs.
         
         * Documentation: https://aws-cdk-secure-api.readthedocs.io.
         
         .. _`AWS CDK v2`: https://aws.amazon.com/about-aws/whats-new/2021/12/aws-cloud-development-kit-cdk-generally-available/
         
-        Secure Rest Api
-        ---------------
-        
-        The ``SecureRestApi`` construct creates a (public) REST API secured behind an API key, which needs to be
-        specified in the ``x-api-key`` header for all requests.
-        
         Install
         -------
         
         .. code-block:: console
         
             pip install aws-cdk-secure-api
         
+        Constructs
+        ----------
+        
+        * ``SecureRestApi`` - A construct to create a (public) REST API secured behind an API key, which needs to be
+          specified in the ``x-api-key`` header for all requests.
+        
+        * ``IAMSecureRestApi`` - A construct to create a (public) REST API secured behind `AWS IAM authentication`_, which
+          requires IAM credentials `to be signed`_ and included in all requests.
+        
+        .. _to be signed: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-access-control-iam.html
+        
         Features
         --------
         
-        * A CDK Construct which sets up a `RestApi`_ secured behind an API key.
-        * An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
-          a free service) as needed.
-        * Local cache for the API key, so that API calls are not needed in future
-          CDK deployments.
-        * Helper methods for ``SecureRestApi``, to make it easier to
+        * A CDK Construct which sets up a `RestApi`_ secured behind (one of):
+        
+          * API key
+        
+            * An API key is `auto-generated`_ and stored in SSM Parameter Store (which is
+              a free service) as needed.
+        
+            * Local cache for the API key, so that API calls are not needed in future
+              CDK deployments.
+        
+          * `AWS IAM authentication`_
+        
+            * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+        
+            * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
+        
+        * Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
           integrate a method for an AWS Lambda function for example.
         
         .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
         .. _`auto-generated`: https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_GetRandomPassword.html
         
         Usage
         -----
@@ -106,14 +122,46 @@
         .. code:: python3
         
             # GET /path1
             api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
             # PUT /path2, POST /path2
             api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
         
+        The ``IAMSecureRestApi`` construct represents a Secure REST API in Amazon API Gateway,
+        which requires IAM Authorization.
+        
+        **Using a custom-named resource**:
+        
+        .. code:: python3
+        
+            from aws_cdk.aws_apigateway import StageOptions
+            from aws_cdk.aws_lambda import Function, Runtime
+        
+            from aws_cdk_secure_api import Http, IAMConfig, IAMSecureRestApi
+        
+            # noinspection PyTypeChecker
+            py_runtime: Runtime = Runtime.PYTHON_3_10
+        
+            get_handler = Function(self, 'lambda1', runtime=py_runtime, ...)
+            put_handler = Function(self, 'lambda2', runtime=py_runtime, ...)
+        
+            api = IAMSecureRestApi(
+                self, 'api',
+                rest_api_name='My IAM Secure Service',
+                # optional: specify the name of secret to store IAM User Credentials
+                config=IAMConfig(secret_name='my-stack/iam-user-access-keys'),
+                # optional: specify a deployment stage
+                deploy_options=StageOptions(stage_name='dev')
+            )
+        
+            # GET /path1
+            api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
+            # PUT /path2, POST /path2
+            api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
+        
         AWS Profile
         -----------
         
         Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
         
             cdk deploy --profile my-aws-profile
         
@@ -152,19 +200,23 @@
         
           * *Note:* this output will not show up if ``override_endpoint_name`` is disabled
             in the ``config`` parameter.
         
         * ``APIKey`` - The API key for the endpoint, which needs to be specified
           as a value in an HTTP request's ``x-api-key`` header.
         
+        * ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
+          stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
+        
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
         
+        .. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
         .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
```

### Comparing `aws-cdk-secure-api-0.3.0/aws_cdk_secure_api.egg-info/SOURCES.txt` & `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/Makefile` & `aws-cdk-secure-api-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/aws_cdk_secure_api.aws.rst` & `aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.aws.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/aws_cdk_secure_api.rst` & `aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/conf.py` & `aws-cdk-secure-api-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/installation.rst` & `aws-cdk-secure-api-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/docs/make.bat` & `aws-cdk-secure-api-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/setup.py` & `aws-cdk-secure-api-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.3.0/tests/unit/test_aws_cdk_secure_api.py` & `aws-cdk-secure-api-0.4.0/tests/unit/test_aws_cdk_secure_api.py`

 * *Files identical despite different names*

