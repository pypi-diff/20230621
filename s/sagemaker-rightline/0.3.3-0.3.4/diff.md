# Comparing `tmp/sagemaker-rightline-0.3.3.tar.gz` & `tmp/sagemaker-rightline-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.3.tar", last modified: Wed Jun 21 15:25:14 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.4.tar", last modified: Wed Jun 21 16:40:52 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.3.tar` & `sagemaker-rightline-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 15:25:07.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    30827 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.426530 sagemaker-rightline-0.3.4/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 16:40:44.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 16:40:52.000000 sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:40:52.430530 sagemaker-rightline-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30149 2023-06-21 16:40:36.000000 sagemaker-rightline-0.3.4/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.3/LICENSE` & `sagemaker-rightline-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/PKG-INFO` & `sagemaker-rightline-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,16 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
-  - `StepInputOutputAsExpected`
+  - `StepOutputsMatchInputsAsExpected`
+  - `StepCallbackSqsQueueExists`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -126,14 +127,15 @@
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
     StepOutputsMatchInputsAsExpected,
+    StepCallbackSqsQueueExists,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -208,14 +210,15 @@
                 "output": {
                     "step_name": "sm_processing_step_sklearn",
                     "output_name": "output-1",
                 },
             }
         ]
     ),
+    StepCallbackSqsQueueExists(),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.3/README.md` & `sagemaker-rightline-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,16 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
-  - `StepInputOutputAsExpected`
+  - `StepOutputsMatchInputsAsExpected`
+  - `StepCallbackSqsQueueExists`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -81,14 +82,15 @@
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
     StepOutputsMatchInputsAsExpected,
+    StepCallbackSqsQueueExists,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -163,14 +165,15 @@
                 "output": {
                     "step_name": "sm_processing_step_sklearn",
                     "output_name": "output-1",
                 },
             }
         ]
     ),
+    StepCallbackSqsQueueExists(),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.3/pyproject.toml` & `sagemaker-rightline-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.4/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.4/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.4/sagemaker_rightline/validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -763,28 +763,28 @@
         """
         step_type = step.step_type.value
 
         if kind == "input":
             if step_type == "Training":
                 input = step.inputs[name]
                 if isinstance(input, TrainingInput):
-                    return str(input.config["DataSource"]["S3DataSource"]["S3Uri"])
+                    return input.config["DataSource"]["S3DataSource"]["S3Uri"]
                 else:
                     raise ValueError(f"Input {name} is not of type TrainingInput.")
             else:
                 # If ProcessingStep
                 for input in step.inputs:
                     if input.input_name == name:
-                        return str(input.source)
+                        return input.source
                 raise ValueError(f"Input {name} not found in ProcessingStep.")
 
         elif kind == "output":
             for output in step.outputs:
                 if output.output_name == name:
-                    return str(output.destination)
+                    return output.destination
         else:
             raise ValueError(f"Kind {kind} not supported. Must be one of 'input' or 'output'.")
 
     def run(
         self,
         sagemaker_pipeline: Pipeline,
     ) -> ValidationResult:
@@ -821,7 +821,77 @@
             )
             results.append((input, output))
         return self.rule.run(
             observed=[x[0] for x in results],
             expected=[x[1] for x in results],
             validation_name=self.name,
         )
+
+
+class StepCallbackSqsQueueExists(Validation):
+    """Validate whether the SQS queue targeted by a CallbackStep exists."""
+
+    def __init__(
+        self,
+        boto3_client: Union["boto3.client('sqs')", str] = "sqs",  # noqa F821
+    ) -> None:
+        """Initialize StepCallbackSqsQueueExists validation.
+
+        :param boto3_client: Boto3 client to use for checking SQS queue existence,
+        defaults to "sqs"
+        :type boto3_client: Union["boto3.client('sqs')", str], optional
+        :raises ValueError: boto3_client must be 'sqs'
+        :return: None
+        :rtype: None
+        """
+        if isinstance(boto3_client, str) and boto3_client != "sqs":
+            raise ValueError(f"boto3_client must be 'sqs', not {boto3_client}.")
+        if boto3_client:
+            self.client = (
+                boto3_client if not isinstance(boto3_client, str) else boto3.client(boto3_client)
+            )
+
+        super().__init__(
+            name="StepCallbackSqsQueueExists",
+            paths=[
+                ".steps[step_type/value==Callback].sqs_queue_url",
+            ],
+        )
+
+    def run(
+        self,
+        sagemaker_pipeline: Pipeline,
+    ) -> ValidationResult:
+        """Runs validation on Pipeline.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :return: validation result
+        :rtype: ValidationResult
+        """
+        sqs_url_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
+        exist = []
+        not_exist = []
+        for url in sqs_url_observed:
+            try:
+                _ = self.client.get_queue_attributes(
+                    QueueUrl=url,
+                )
+                exist.append(url)
+            except ClientError:
+                not_exist.append(url)
+        if not_exist:
+            return ValidationResult(
+                success=False,
+                negative=False,
+                message=f"SQS url {not_exist} does not exist.",
+                subject=str(sqs_url_observed),
+                validation_name=self.name,
+            )
+        else:
+            return ValidationResult(
+                success=True,
+                negative=False,
+                message=f"SQS url Function {exist} exists.",
+                subject=str(sqs_url_observed),
+                validation_name=self.name,
+            )
```

### Comparing `sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.4/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,16 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
-  - `StepInputOutputAsExpected`
+  - `StepOutputsMatchInputsAsExpected`
+  - `StepCallbackSqsQueueExists`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -126,14 +127,15 @@
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
     StepOutputsMatchInputsAsExpected,
+    StepCallbackSqsQueueExists,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -208,14 +210,15 @@
                 "output": {
                     "step_name": "sm_processing_step_sklearn",
                     "output_name": "output-1",
                 },
             }
         ]
     ),
+    StepCallbackSqsQueueExists(),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.3/tests/test_model.py` & `sagemaker-rightline-0.3.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/tests/test_rules.py` & `sagemaker-rightline-0.3.4/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.3/tests/test_validations.py` & `sagemaker-rightline-0.3.4/tests/test_validations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pytest
-from moto import mock_ecr, mock_iam, mock_lambda
+from moto import mock_ecr, mock_iam, mock_lambda, mock_sqs
 from sagemaker.inputs import FileSystemInput, TrainingInput
 from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
+from sagemaker.workflow.functions import Join
 from sagemaker.workflow.parameters import ParameterString
+from sagemaker.workflow.pipeline import ExecutionVariables
 
 from sagemaker_rightline.model import Validation, ValidationResult
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     ContainerImage,
     PipelineParametersAsExpected,
+    StepCallbackSqsQueueExists,
     StepImagesExist,
     StepInputsAsExpected,
     StepKmsKeyIdAsExpected,
     StepLambdaFunctionExists,
     StepNetworkConfigAsExpected,
     StepOutputsAsExpected,
     StepOutputsMatchInputsAsExpected,
@@ -21,29 +24,33 @@
     StepTagsAsExpected,
 )
 from tests.fixtures.constants import (
     TEST_ACCOUNT_ID,
     TEST_LAMBDA_FUNC_NAME,
     TEST_REGION_NAME,
     TEST_ROLE_NAME,
+    TEST_SQS_QUEUE_NAME,
+    TEST_SQS_QUEUE_URL_BASE,
 )
 from tests.fixtures.image_details import (
     IMAGE_1_REPOSITORY_NAME,
     IMAGE_1_TAG,
     IMAGE_1_URI,
     IMAGE_2_URI,
 )
 from tests.fixtures.pipeline import DUMMY_BUCKET, get_sagemaker_pipeline
 from tests.utils import (
     create_iam_role,
     create_image,
     create_lambda_function,
+    create_sqs_queue,
     ecr_client,
     iam_client,
     lambda_client,
+    sqs_client,
 )
 
 
 @pytest.fixture
 def sagemaker_pipeline():
     return get_sagemaker_pipeline()
 
@@ -107,14 +114,19 @@
 
 
 def test_step_lambda_function_exists_wrong_client() -> None:
     with pytest.raises(ValueError):
         _ = StepLambdaFunctionExists(boto3_client="not-a-boto3-client")
 
 
+def test_step_sqs_queue_exists_wrong_client() -> None:
+    with pytest.raises(ValueError):
+        _ = StepCallbackSqsQueueExists(boto3_client="not-a-boto3-client")
+
+
 def test_step_role_name_exists_wrong_client() -> None:
     with pytest.raises(ValueError):
         _ = StepRoleNameExists(boto3_client="not-a-boto3-client")
 
 
 @pytest.mark.parametrize(
     "parameters_expected,success",
@@ -775,14 +787,27 @@
                     destination=f"s3://{DUMMY_BUCKET}/output-1",
                 ),
                 ProcessingOutput(
                     output_name="output-2",
                     source="/opt/ml/processing/output/2",
                     destination=f"s3://{DUMMY_BUCKET}/output-2",
                 ),
+                ProcessingOutput(
+                    output_name="output-3",
+                    source="/opt/ml/processing/output/3",
+                    destination=Join(
+                        on="/",
+                        values=[
+                            "s3:/",
+                            DUMMY_BUCKET,
+                            ExecutionVariables.PIPELINE_EXECUTION_ID,
+                            "output-3",
+                        ],
+                    ),
+                ),
             ],
             "sm_processing_step_sklearn",
             True,
         ],
         [
             Contains,
             [
@@ -844,14 +869,30 @@
             False,
             False,
         ],
         [
             [
                 {
                     "input": {
+                        "step_name": "sm_processing_step_spark",
+                        "input_name": "input-3",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "output_name": "output-3",
+                    },
+                }
+            ],
+            True,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
                         "step_name": "sm_processing_step_sklearn",
                         "input_name": "input-1",
                     },
                     "output": {
                         "step_name": "step_doesnt_exist",
                         "output_name": "output-1",
                     },
@@ -918,7 +959,23 @@
     )
     if raise_error:
         with pytest.raises((ValueError, AttributeError)):
             _ = step_outputs_validation.run(sagemaker_pipeline)
     else:
         result = step_outputs_validation.run(sagemaker_pipeline)
         assert result.success is success
+
+
+@mock_sqs
+@mock_iam
+def test_sqs_queue_exists_positive(sqs_client, iam_client, sagemaker_pipeline) -> None:
+    with create_sqs_queue(sqs_client, iam_client, [(TEST_SQS_QUEUE_NAME, TEST_SQS_QUEUE_URL_BASE)]):
+        sqs_queue_exists = StepCallbackSqsQueueExists()
+        result = sqs_queue_exists.run(sagemaker_pipeline)
+    assert result.success
+
+
+@mock_sqs
+def test_sqs_queue_exists_negative(sqs_client, iam_client, sagemaker_pipeline) -> None:
+    sqs_queue_exists = StepCallbackSqsQueueExists()
+    result = sqs_queue_exists.run(sagemaker_pipeline)
+    assert not result.success
```

