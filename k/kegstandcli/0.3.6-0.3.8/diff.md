# Comparing `tmp/kegstandcli-0.3.6.tar.gz` & `tmp/kegstandcli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstandcli-0.3.6.tar", max compression
+gzip compressed data, was "kegstandcli-0.3.8.tar", max compression
```

## Comparing `kegstandcli-0.3.6.tar` & `kegstandcli-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.6/LICENSE
--rw-r--r--   0        0        0     6518 2023-05-04 22:42:37.058514 kegstandcli-0.3.6/README.md
--rw-r--r--   0        0        0     1545 2023-05-05 20:49:13.990234 kegstandcli-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.6/src/kegstandcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.6/src/kegstandcli/cli/__init__.py
--rw-r--r--   0        0        0    16270 2023-05-04 22:42:38.140953 kegstandcli-0.3.6/src/kegstandcli/cli/__main__.py
--rw-r--r--   0        0        0     3048 2023-05-04 22:42:38.142413 kegstandcli-0.3.6/src/kegstandcli/cli/build.py
--rw-r--r--   0        0        0     2516 2023-05-04 22:19:56.398580 kegstandcli-0.3.6/src/kegstandcli/cli/config.py
--rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.6/src/kegstandcli/cli/default_lambda.py.tmpl
--rw-r--r--   0        0        0     1959 2023-05-04 22:42:38.145141 kegstandcli-0.3.6/src/kegstandcli/cli/deploy.py
--rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.6/src/kegstandcli/cli/new.py
--rw-r--r--   0        0        0     1302 2023-05-04 22:42:38.147183 kegstandcli-0.3.6/src/kegstandcli/cli/teardown.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.6/src/kegstandcli/infra/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.6/src/kegstandcli/infra/app.py
--rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.6/src/kegstandcli/infra/cdk.json
--rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.6/src/kegstandcli/infra/stacks/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.6/src/kegstandcli/infra/stacks/lambda_rest_api.py
--rw-r--r--   0        0        0     1082 2023-05-04 22:42:37.412595 kegstandcli-0.3.6/src/kegstandcli/utils.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 kegstandcli-0.3.6/setup.py
--rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 kegstandcli-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.8/LICENSE
+-rw-r--r--   0        0        0     6581 2023-05-08 18:20:56.097880 kegstandcli-0.3.8/README.md
+-rw-r--r--   0        0        0     1545 2023-06-20 23:44:55.511652 kegstandcli-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.8/src/kegstandcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.8/src/kegstandcli/cli/__init__.py
+-rw-r--r--   0        0        0    16270 2023-05-04 22:42:38.140953 kegstandcli-0.3.8/src/kegstandcli/cli/__main__.py
+-rw-r--r--   0        0        0     3647 2023-06-20 23:46:48.735908 kegstandcli-0.3.8/src/kegstandcli/cli/build.py
+-rw-r--r--   0        0        0     2516 2023-06-20 07:09:06.056577 kegstandcli-0.3.8/src/kegstandcli/cli/config.py
+-rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.8/src/kegstandcli/cli/default_lambda.py.tmpl
+-rw-r--r--   0        0        0     1972 2023-06-18 10:54:43.324903 kegstandcli-0.3.8/src/kegstandcli/cli/deploy.py
+-rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.8/src/kegstandcli/cli/new.py
+-rw-r--r--   0        0        0      241 2023-06-20 23:46:53.763777 kegstandcli-0.3.8/src/kegstandcli/cli/rest_api_gateway_health_check.py.tmpl
+-rw-r--r--   0        0        0     1302 2023-05-04 22:42:38.147183 kegstandcli-0.3.8/src/kegstandcli/cli/teardown.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.8/src/kegstandcli/infra/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-20 23:47:10.853582 kegstandcli-0.3.8/src/kegstandcli/infra/app.py
+-rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.8/src/kegstandcli/infra/cdk.json
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/__init__.py
+-rw-r--r--   0        0        0     3989 2023-06-20 23:46:59.497383 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_backend.py
+-rw-r--r--   0        0        0     7040 2023-06-20 23:47:03.474197 kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_gateway.py
+-rw-r--r--   0        0        0     1738 2023-06-20 23:47:15.485078 kegstandcli-0.3.8/src/kegstandcli/utils.py
+-rw-r--r--   0        0        0     7899 1970-01-01 00:00:00.000000 kegstandcli-0.3.8/setup.py
+-rw-r--r--   0        0        0     7959 1970-01-01 00:00:00.000000 kegstandcli-0.3.8/PKG-INFO
```

### Comparing `kegstandcli-0.3.6/LICENSE` & `kegstandcli-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.6/README.md` & `kegstandcli-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,17 @@
 ## Roadmap
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
-- [ ] Custom domain names
-- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [x] Custom domain names
+- [ ] Support multiple repos using the same domain (and API Gateway)
+- [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -40,19 +40,20 @@
 the dependencies for the new project: ```shell > cd my-service > poetry install
 ``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
 deploy ``` You should now be able to access the API endpoint at `https:/
 /.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
 and more advanced usage, see the [official documentation](https://github.com/
 JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
 changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
-More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
-- [x] Maybe simplify the folder structure from `src/api/resources//.py` to
-`src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
-S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
-helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
+More content on [kegstand.dev](https://kegstand.dev) - [x] Custom domain names
+- [ ] Support multiple repos using the same domain (and API Gateway) - [x]
+Simplify the folder structure from `src/api/resources//.py` to `src/api/.py`
+### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
+DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination helper - [ ]
+[Record a screencast](https://asciinema.org/) for the README - [ ]
 Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
 workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
 automated API Versioning - [ ] Simple way to define/override core API/Lambda
 properties such as CPU/MEM, Python runtime version, warm pool (!), and
 concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
 Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
 and they will be applied to the generated resources - [ ] Easily add [AWS
```

### Comparing `kegstandcli-0.3.6/pyproject.toml` & `kegstandcli-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstandcli"
-version = "0.3.6"
+version = "0.3.8"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand"
 homepage = "https://kegstand.dev"
 readme = "README.md"
 packages = [
@@ -26,25 +26,25 @@
 ]
 
 [tool.poetry.scripts]
 keg = "kegstandcli.cli.__main__:kegstandcli"
 
 [tool.poetry.dependencies]
 aws-cdk-lib = "^2.67.0"
-aws-solutions-constructs-aws-apigateway-lambda = "^2.36.0"
+aws-solutions-constructs-aws-apigateway-lambda = "^2.39.0"
 boto3 = "^1.17.113"
 click = "^8.0.3"
 constructs = ">=10.0.0,<11.0.0"
 copier = "^6.2.0"  # 7.0.1 has a bug that deletes the template folder, see https://github.com/copier-org/copier/issues/1029
 pyjwt = "^2.1.0"
 python = "^3.9"
 tomlkit = "^0.11.7"
 xxhash = "^3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-subprocess = "^1.5.0"
-sentient-switchblade = "^0.3.3"
+sentient-switchblade = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/__main__.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/build.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,36 @@
 
 
 def build_command(verbose: bool, project_dir: str, config: dict):
     # Create a directory to hold the build artifacts, and make sure it is empty
     build_dir = create_empty_folder(project_dir, "dist")
 
     # Handle the different types ('modules') of build
+    if "api_gateway" in config:
+        build_api_gateway(
+            config, verbose, project_dir, create_empty_folder(build_dir, "api_gw_src")
+        )
     if "api" in config:
         build_api(
             config, verbose, project_dir, create_empty_folder(build_dir, "api_src")
         )
+    click.echo("Finished building application!")
+
+
+def build_api_gateway(config: dict, verbose: bool, project_dir: str, module_build_dir: str):
+    create_empty_folder(module_build_dir, "api")
+
+    # Inject health check endpoint
+    lambda_file = os.path.join(module_build_dir, "api", "lambda.py")
+    shutil.copyfile(
+        os.path.join(
+            os.path.dirname(os.path.abspath(__file__)), "rest_api_gateway_health_check.py.tmpl"
+        ),
+        lambda_file,
+    )
 
 
 def build_api(config: dict, verbose: bool, project_dir: str, module_build_dir: str):
     # Copy everything in the project_dir/src folder to the module_build_dir
     src_dir = os.path.join(project_dir, "src")
     shutil.copytree(src_dir, module_build_dir, dirs_exist_ok=True)
 
@@ -74,15 +92,14 @@
         f"{module_build_dir}/requirements.txt",
         "-t",
         module_build_dir,
     ]
     subprocess.run(
         install_command, check=True, stdout=subprocess.DEVNULL if not verbose else None
     )  # nosec B603
-    click.echo("Finished building application!")
 
 
 def create_empty_folder(parent_folder: str, folder_name: str):
     if folder_name == "":
         raise ValueError("folder_name cannot be empty")
 
     folder_path = os.path.join(parent_folder, folder_name)
```

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/config.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/deploy.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 @click.option(
     "--skip-build",
     is_flag=True,
     default=False,
     help="Skip building the project before deploying",
 )
 def deploy(ctx, region, hotswap, skip_build):
-    project_dir, config_file, verbose = itemgetter(
-        "project_dir", "config_file", "verbose"
+    project_dir, config_file, config, verbose = itemgetter(
+        "project_dir", "config_file", "config", "verbose"
     )(ctx.obj)
     if not skip_build:
-        build_command(verbose, project_dir, config_file)
+        build_command(verbose, project_dir, config)
 
     deploy_command(verbose, project_dir, config_file, region, hotswap)
 
 
 def deploy_command(verbose, project_dir, config_file, region, hotswap):
     # Get the dir of the kegstandcli package (one level up from here)
     kegstandcli_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
```

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/new.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/new.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.6/src/kegstandcli/cli/teardown.py` & `kegstandcli-0.3.8/src/kegstandcli/cli/teardown.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.6/src/kegstandcli/infra/app.py` & `kegstandcli-0.3.8/src/kegstandcli/infra/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,109 @@
 #!/usr/bin/env python3
-import logging
+import click
 import os
 import sys
 
 import aws_cdk as cdk
+from aws_cdk import aws_apigateway as apigw
 from aws_cdk import aws_cognito as cognito
 
 from kegstandcli.cli.config import get_kegstand_config
-from kegstandcli.infra.stacks.lambda_rest_api import LambdaRestApi
-
-logger = logging.getLogger()
-logger.setLevel(logging.INFO)
+from kegstandcli.infra.stacks.rest_api_backend import RestApiBackend
+from kegstandcli.infra.stacks.rest_api_gateway import RestApiGateway
 
 app = cdk.App()
 
 # Get the passed context
 region = app.node.try_get_context("region")
 project_dir = app.node.try_get_context("project_dir")
 config_file = app.node.try_get_context("config_file") or "kegstand.toml"
-verbose = app.node.try_get_context("verbose") or False
+verbose = app.node.try_get_context("verbose") in ["true", "True", True]
 
 # Get the Kegstand config
 config = get_kegstand_config(verbose, project_dir, config_file)
 
-logger.info("Creating app with config: %s", config)
+click.echo(f"Creating app with config: {config}")
 
 parent_stack_name = config["project"]["name"].replace(" ", "-")
 parent_stack = cdk.Stack(
     app,
     parent_stack_name,
     description=f"{config['project']['name']} v.{config['project']['version']}",
-    env={"region": region},
+    env=cdk.Environment(
+        account=os.environ["CDK_DEFAULT_ACCOUNT"],
+        region=region
+    )
 )
 
 # Create stacks/modules
 modules = {}
 
 if "cdk" in config:
-    logger.info("Creating additional resources [cdk]...")
+    click.echo("Creating additional resources [cdk]...")
     # Import the project's infra module
     project_infra_path = os.path.join(project_dir, config["cdk"]["path_to_infra"])
     sys.path.append(project_infra_path)
     from main import custom_infra  # pylint: disable=import-error
 
     custom_infra_config = custom_infra(parent_stack, region)
     modules["custom_infra"] = custom_infra_config
 
-if "api" in config:
-    logger.info("Creating stack for [api]...")
+if "api_gateway" in config:
+    click.echo("Creating stack for [api_gateway]...")
 
     user_pool = (
         cognito.UserPool.from_user_pool_id(
+            parent_stack, "UserPool", config["api_gateway"]["user_pool_id"]
+        )
+        if "user_pool_id" in config["api_gateway"]
+        else None
+    )
+
+    click.echo(f"API GW is passed a UserPool?: {user_pool is not None}")
+
+    api_gateway_construct_name = config["api_gateway"]["name"].replace(" ", "-")
+    api_gateway_construct = RestApiGateway(
+        parent_stack, api_gateway_construct_name, config, user_pool=user_pool
+    )
+
+    modules["api_gateway"] = api_gateway_construct
+
+if "api" in config:
+    click.echo("Creating stack for [api]...")
+
+    gateway = (
+        apigw.RestApi.from_rest_api_id(
+            parent_stack, "RestApiGatewayReference", config["api"]["api_gateway_id"]
+        )
+        if "api_gateway_id" in config["api"]
+        else modules["api_gateway"].api if "api_gateway" in modules else None
+    )
+    user_pool = parent_stack.node.try_find_child("UserPool") if "api_gateway" in modules else (
+        cognito.UserPool.from_user_pool_id(
             parent_stack, "UserPool", config["api"]["user_pool_id"]
         )
         if "user_pool_id" in config["api"]
         else None
     )
 
+    click.echo(f"API is passed a UserPool?: {user_pool is not None}")
+
     api_construct_name = config["api"]["name"].replace(" ", "-")
-    api_construct = LambdaRestApi(
-        parent_stack, api_construct_name, config, user_pool=user_pool
+    api_construct = RestApiBackend(
+        parent_stack, api_construct_name, config, rest_api_gw=gateway, user_pool=user_pool
     )
 
     # Add custom environment variables if provided
     if "custom_infra" in modules and "environment_variables" in modules["custom_infra"]:
         for key, value in modules["custom_infra"]["environment_variables"].items():
             api_construct.lambda_function.add_environment(key, value)
 
     modules["api"] = api_construct
 
 # Finally, we can set custom permissions between stacks if needed
 if "cdk" in config:
     from main import permissions  # pylint: disable=import-error
 
-    permissions(parent_stack, **modules)
+    permissions(parent_stack, modules)
 
 app.synth()
```

### Comparing `kegstandcli-0.3.6/src/kegstandcli/infra/stacks/lambda_rest_api.py` & `kegstandcli-0.3.8/src/kegstandcli/infra/stacks/rest_api_backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,90 @@
+import click
+
 from aws_cdk import Stack
 from aws_cdk import aws_apigateway as apigw
 from aws_cdk import aws_lambda as lambda_
-from aws_solutions_constructs import aws_apigateway_lambda as apigw_lambda
 from constructs import Construct
 
 from kegstandcli.utils import find_resource_modules
 
+MODULE_CONFIG_KEY = "api"
 
-class LambdaRestApi(Construct):
-    def __init__(self, scope: Construct, id: str, config: dict, user_pool) -> None:
+class RestApiBackend(Construct):
+    def __init__(self, scope: Construct, id: str, config: dict, rest_api_gw: apigw.RestApi, user_pool) -> None:
         super().__init__(scope, id)
 
         provision_with_authorizer = user_pool is not None
 
         # Find all the resource modules in the API source directory
         resource_modules = find_resource_modules(
-            f'{config["project_dir"]}/dist/api_src/api'
+            f'{config["project_dir"]}/dist/api_src'
         )
 
+        # Output all modules found, each module contains:
+        click.echo("API backend: Found the following resource modules:")
+        for resource in resource_modules:
+            click.echo(f" - Name: {resource['name']}")
+            click.echo(f"   Module path: {resource['module_path']}")
+            click.echo(f"   Fromlist: {resource['fromlist']}")
+            click.echo(f"   Is public: {resource['is_public']}")
+        
         powertools_layer_package = {
             "x86_64": "AWSLambdaPowertoolsPythonV2:25",
             "arm64": "AWSLambdaPowertoolsPythonV2-Arm64:25",
         }[
             "x86_64"
         ]  # TODO: make this configurable
 
-        # Official 'ApiGatewayToLambda' AWS Solution Construct
-        # https://docs.aws.amazon.com/solutions/latest/constructs/aws-apigateway-lambda.html
-        api_gateway_to_lambda = apigw_lambda.ApiGatewayToLambda(
-            self,
-            f"{id}-ApiGatewayConstruct",
-            lambda_function_props=lambda_.FunctionProps(
-                function_name=f"{id}-Function",
-                runtime=lambda_.Runtime.PYTHON_3_9,
-                handler=config["api"]["entrypoint"],
-                code=lambda_.Code.from_asset(f'{config["project_dir"]}/dist/api_src'),
-                layers=[  # Lambda Powertools: https://awslabs.github.io/aws-lambda-powertools-python/2.4.0/
-                    lambda_.LayerVersion.from_layer_version_arn(
-                        self,
-                        "PowertoolsLayer",
-                        layer_version_arn=f"arn:aws:lambda:{Stack.of(self).region}:017000801446:layer:{powertools_layer_package}",  # noqa: E501
-                    )
-                ],
-                memory_size=256,
-                tracing=lambda_.Tracing.ACTIVE,
-                environment={
-                    "LOG_LEVEL": "INFO",
-                    "POWERTOOLS_LOGGER_SAMPLE_RATE": "0.1",
-                    "POWERTOOLS_LOGGER_LOG_EVENT": "true",
-                    "POWERTOOLS_SERVICE_NAME": "authie-token-function",
-                },
-            ),
-            api_gateway_props=apigw.RestApiProps(
-                rest_api_name=f"{id}-RestApi",
-                default_method_options=apigw.MethodOptions(
-                    authorization_type=apigw.AuthorizationType.NONE
-                ),
-                deploy_options=apigw.StageOptions(
-                    logging_level=apigw.MethodLoggingLevel.INFO,
-                    metrics_enabled=True,
-                    tracing_enabled=True,
-                ),
-            ),
+        # Lambda API backend
+        self.lambda_function = lambda_.Function(
+            self, f"{id}-Backend",
+            function_name=f"{id}-Function",
+            runtime=lambda_.Runtime.PYTHON_3_9,
+            handler=config[MODULE_CONFIG_KEY]["entrypoint"],
+            code=lambda_.Code.from_asset(f'{config["project_dir"]}/dist/api_src'),
+            layers=[  # Lambda Powertools: https://awslabs.github.io/aws-lambda-powertools-python/2.4.0/
+                lambda_.LayerVersion.from_layer_version_arn(
+                    self,
+                    "PowertoolsLayer",
+                    layer_version_arn=f"arn:aws:lambda:{Stack.of(self).region}:017000801446:layer:{powertools_layer_package}",  # noqa: E501
+                )
+            ],
+            memory_size=256,
+            tracing=lambda_.Tracing.ACTIVE,
+            environment={
+                "LOG_LEVEL": "INFO",
+                "POWERTOOLS_LOGGER_SAMPLE_RATE": "1.00", # "0.05",  # Use log level DEBUG for 5% of invocations
+                "POWERTOOLS_LOGGER_LOG_EVENT": "true",
+                "POWERTOOLS_SERVICE_NAME": f"{id}-Function",
+            },
         )
-        self.api = api_gateway_to_lambda.api_gateway
-        self.lambda_function = api_gateway_to_lambda.lambda_function
 
         self.authorizer = None
         if provision_with_authorizer:
+            click.echo("Creating Cognito authorizer for API...")
             self.authorizer = apigw.CognitoUserPoolsAuthorizer(
                 self, f"{id}-Authorizer", cognito_user_pools=[user_pool]
             )
 
         # For each resource, create API Gateway endpoints with the Lambda integration
         for resource in resource_modules:
-            resource_root = self.api.root.add_resource(resource["name"])
-            if provision_with_authorizer:
+            if provision_with_authorizer and not resource["is_public"]:
                 # Private, auth required endpoints
-                resource_root.add_proxy(
+                resource_root = rest_api_gw.root.add_resource(
+                    resource["name"],
                     default_integration=apigw.LambdaIntegration(self.lambda_function),
                     default_method_options=apigw.MethodOptions(
                         authorization_type=apigw.AuthorizationType.COGNITO,
                         authorizer=self.authorizer,  # Apply the authorizer
                     ),
                 )
+                resource_root.add_proxy()
             else:
                 # Public (no auth required) endpoints
-                resource_root.add_proxy(
+                resource_root = rest_api_gw.root.add_resource(
+                    resource["name"],
                     default_integration=apigw.LambdaIntegration(self.lambda_function)
                 )
+                resource_root.add_proxy()
 
-        self.deployment = apigw.Deployment(self, f"{id}-Deployment", api=self.api)
+        self.deployment = apigw.Deployment(self, f"{id}-Deployment", api=rest_api_gw)
```

### Comparing `kegstandcli-0.3.6/setup.py` & `kegstandcli-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,31 @@
  'kegstandcli.infra.stacks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0',
- 'aws-solutions-constructs-aws-apigateway-lambda>=2.36.0,<3.0.0',
+ 'aws-solutions-constructs-aws-apigateway-lambda>=2.39.0,<3.0.0',
  'boto3>=1.17.113,<2.0.0',
  'click>=8.0.3,<9.0.0',
  'constructs>=10.0.0,<11.0.0',
  'copier>=6.2.0,<7.0.0',
  'pyjwt>=2.1.0,<3.0.0',
  'tomlkit>=0.11.7,<0.12.0',
  'xxhash>=3.2.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
 
 setup_kwargs = {
     'name': 'kegstandcli',
-    'version': '0.3.6',
+    'version': '0.3.8',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [x] Custom domain names\n- [ ] Support multiple repos using the same domain (and API Gateway)\n- [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['kegstandcli', 'kegstandcli.cli', 'kegstandcli.infra',
 'kegstandcli.infra.stacks'] package_data = \ {'': ['*']} install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0', 'aws-solutions-constructs-aws-apigateway-
-lambda>=2.36.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
+lambda>=2.39.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
 'constructs>=10.0.0,<11.0.0', 'copier>=6.2.0,<7.0.0', 'pyjwt>=2.1.0,<3.0.0',
 'tomlkit>=0.11.7,<0.12.0', 'xxhash>=3.2.0,<4.0.0'] entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
-setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.6', 'description': "The
+setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.8', 'description': "The
 Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
 'long_description': '\n
                            \n \n_[Kegstand_logo]\n\n
 \n\n
 **** The Developer\'s Toolbelt For Accelerating Mean Time To Party on AWS ****
 \n
        Created by Jens_Roland and fueled by a non-zero amount of alcohol
@@ -56,21 +56,22 @@
 service\n> poetry install\n```\n\nFinally, to build and deploy the service to
 AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to
 access the API endpoint at `https://.execute-api..amazonaws.com/prod/
 hello`.\n\n## Documentation\n\nFor further examples and more advanced usage,
 see the [official documentation](https://github.com/JensRoland/kegstand/blob/
 main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and
 features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on
-[kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [x] Maybe
-simplify the folder structure from `src/api/resources//.py` to `src/
-api/.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions:
-S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ]
-Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the
-README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ]
-GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ]
+[kegstand.dev](https://kegstand.dev)\n- [x] Custom domain names\n- [ ] Support
+multiple repos using the same domain (and API Gateway)\n- [x] Simplify the
+folder structure from `src/api/resources//.py` to `src/api/.py`\n\n### Pre-
+1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
+DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n-
+[ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ]
+Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub
+Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ]
 Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/
 override core API/Lambda properties such as CPU/MEM, Python runtime version,
 warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no
 API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags
 in the Kegstand config and they will be applied to the generated resources\n-
 [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/
 dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI]
```

### Comparing `kegstandcli-0.3.6/PKG-INFO` & `kegstandcli-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstandcli
-Version: 0.3.6
+Version: 0.3.8
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aws-cdk-lib (>=2.67.0,<3.0.0)
-Requires-Dist: aws-solutions-constructs-aws-apigateway-lambda (>=2.36.0,<3.0.0)
+Requires-Dist: aws-solutions-constructs-aws-apigateway-lambda (>=2.39.0,<3.0.0)
 Requires-Dist: boto3 (>=1.17.113,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: constructs (>=10.0.0,<11.0.0)
 Requires-Dist: copier (>=6.2.0,<7.0.0)
 Requires-Dist: pyjwt (>=2.1.0,<3.0.0)
 Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
@@ -119,16 +119,17 @@
 ## Roadmap
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
-- [ ] Custom domain names
-- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [x] Custom domain names
+- [ ] Support multiple repos using the same domain (and API Gateway)
+- [x] Simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.6 Summary: The Developer's
+Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.8 Summary: The Developer's
 Toolbelt For Accelerating Mean-Time-To-Party on AWS Home-page: https://
 kegstand.dev License: MIT Author: JensRoland Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Requires-Dist: aws-cdk-lib (>=2.67.0,<3.0.0)
-Requires-Dist: aws-solutions-constructs-aws-apigateway-lambda (>=2.36.0,<3.0.0)
+Requires-Dist: aws-solutions-constructs-aws-apigateway-lambda (>=2.39.0,<3.0.0)
 Requires-Dist: boto3 (>=1.17.113,<2.0.0) Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: constructs (>=10.0.0,<11.0.0) Requires-Dist: copier
 (>=6.2.0,<7.0.0) Requires-Dist: pyjwt (>=2.1.0,<3.0.0) Requires-Dist: tomlkit
 (>=0.11.7,<0.12.0) Requires-Dist: xxhash (>=3.2.0,<4.0.0) Project-URL:
 Repository, https://github.com/jensroland/kegstand Description-Content-Type:
 text/markdown
                                 [Kegstand_logo]
@@ -59,19 +59,20 @@
 the dependencies for the new project: ```shell > cd my-service > poetry install
 ``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
 deploy ``` You should now be able to access the API endpoint at `https:/
 /.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
 and more advanced usage, see the [official documentation](https://github.com/
 JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
 changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
-More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
-- [x] Maybe simplify the folder structure from `src/api/resources//.py` to
-`src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
-S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
-helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
+More content on [kegstand.dev](https://kegstand.dev) - [x] Custom domain names
+- [ ] Support multiple repos using the same domain (and API Gateway) - [x]
+Simplify the folder structure from `src/api/resources//.py` to `src/api/.py`
+### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS,
+DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination helper - [ ]
+[Record a screencast](https://asciinema.org/) for the README - [ ]
 Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
 workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
 automated API Versioning - [ ] Simple way to define/override core API/Lambda
 properties such as CPU/MEM, Python runtime version, warm pool (!), and
 concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
 Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
 and they will be applied to the generated resources - [ ] Easily add [AWS
```

