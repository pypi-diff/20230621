# Comparing `tmp/sagemaker-rightline-0.3.2.tar.gz` & `tmp/sagemaker-rightline-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.2.tar", last modified: Fri Jun 16 22:08:46 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.3.tar", last modified: Wed Jun 21 15:25:14 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.2.tar` & `sagemaker-rightline-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 22:08:39.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    30124 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 15:25:07.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30827 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 15:25:14.000000 sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:25:14.981104 sagemaker-rightline-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-06-21 15:25:03.000000 sagemaker-rightline-0.3.3/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.2/LICENSE` & `sagemaker-rightline-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/PKG-INFO` & `sagemaker-rightline-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.3.2/README.md` & `sagemaker-rightline-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/pyproject.toml` & `sagemaker-rightline-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.3/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.3/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.3/sagemaker_rightline/validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -727,49 +727,64 @@
         )
         self.inputs_outputs_expected: List[Dict[str, Dict[str, str]]] = inputs_outputs_expected
 
     @staticmethod
     def get_step_by_name(
         sagemaker_pipeline: Pipeline, step_name: str
     ) -> "ProcessingStep":  # noqa F821
-        """Get ProcessingStep by name.
+        """Get ProcessingStep, TrainingStep by name.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :param step_name: Name of Step
         :type step_name: str
         :return: ProcessingStep
         :rtype: ProcessingStep
         """
+        supported_step_types = ("Processing", "Training")
         for step in sagemaker_pipeline.steps:
-            if step.name == step_name:
+            if step.name == step_name and step.step_type.value in supported_step_types:
                 return step
-        raise ValueError(f"Step {step_name} not found in Pipeline")
+        raise ValueError(f"Processing or Training Step {step_name} not found in Pipeline.")
 
     @staticmethod
     def get_input_output_by_name(
-        step: "ProcessingStep", name: str, kind: str  # noqa F821
-    ) -> Union["ProcessingInput", "ProcessingOutput"]:
+        step: Union["ProcessingStep", "TrainingStep"], name: str, kind: str  # noqa F821
+    ) -> str:
         """Get ProcessingInput or ProcessingOutput by name.
 
         :param step: ProcessingStep
         :type step: ProcessingStep
         :param name: Name of Input or Output
         :type name: str
-        :return: ProcessingInput or ProcessingOutput
-        :rtype: Union[ProcessingInput, ProcessingOutput]
+        :param kind: Kind of Input or Output, must be one of "input" or "output"
+        :type kind: str
+        :return: Input or Output path
+        :rtype: str
         """
+        step_type = step.step_type.value
+
         if kind == "input":
-            for input in step.inputs:
-                if input.input_name == name:
-                    return input
+            if step_type == "Training":
+                input = step.inputs[name]
+                if isinstance(input, TrainingInput):
+                    return str(input.config["DataSource"]["S3DataSource"]["S3Uri"])
+                else:
+                    raise ValueError(f"Input {name} is not of type TrainingInput.")
+            else:
+                # If ProcessingStep
+                for input in step.inputs:
+                    if input.input_name == name:
+                        return str(input.source)
+                raise ValueError(f"Input {name} not found in ProcessingStep.")
+
         elif kind == "output":
             for output in step.outputs:
                 if output.output_name == name:
-                    return output
+                    return str(output.destination)
         else:
             raise ValueError(f"Kind {kind} not supported. Must be one of 'input' or 'output'.")
 
     def run(
         self,
         sagemaker_pipeline: Pipeline,
     ) -> ValidationResult:
@@ -800,13 +815,13 @@
 
             input = StepOutputsMatchInputsAsExpected.get_input_output_by_name(
                 input_step, input_name, input_kw
             )
             output = StepOutputsMatchInputsAsExpected.get_input_output_by_name(
                 output_step, output_name, output_kw
             )
-            results.append((input.source, output.destination))
+            results.append((input, output))
         return self.rule.run(
             observed=[x[0] for x in results],
             expected=[x[1] for x in results],
             validation_name=self.name,
         )
```

### Comparing `sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.3/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.3.2/tests/test_model.py` & `sagemaker-rightline-0.3.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/tests/test_rules.py` & `sagemaker-rightline-0.3.3/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.2/tests/test_validations.py` & `sagemaker-rightline-0.3.3/tests/test_validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,15 +523,15 @@
             False,
         ],
         [
             Contains,
             [
                 {
                     "train": TrainingInput(
-                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        s3_data=f"s3://{DUMMY_BUCKET}/output-4",
                         content_type="text/csv",
                     )
                 }
             ],
             "Training",
             True,
         ],
@@ -602,15 +602,15 @@
             True,
         ],
         [
             Equals,
             [
                 {
                     "train": TrainingInput(
-                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        s3_data=f"s3://{DUMMY_BUCKET}/output-4",
                         content_type="text/csv",
                     ),
                     "validation": FileSystemInput(
                         file_system_id="fs-1234",
                         file_system_type="EFS",
                         directory_path="/some/path",
                         file_system_access_mode="ro",
@@ -622,15 +622,15 @@
             True,
         ],
         [
             Equals,
             [
                 {
                     "train": TrainingInput(
-                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        s3_data=f"s3://{DUMMY_BUCKET}/output-4",
                         content_type="text/csv",
                     ),
                     "some-key": "some-value",
                     "validation": FileSystemInput(
                         file_system_id="fs-1234",
                         file_system_type="EFS",
                         directory_path="/some/path",
@@ -872,14 +872,46 @@
                         "output_name": "output-1",
                     },
                 }
             ],
             False,
             True,
         ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_training_step_sklearn",
+                        "input_name": "train",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
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
+                        "step_name": "sm_training_step_sklearn",
+                        "input_name": "validation",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            False,
+            True,
+        ],
     ],
 )
 def test_step_outputs_match_inputs_as_expected(
     sagemaker_pipeline, inputs_outputs_expected, success, raise_error
 ) -> None:
     step_outputs_validation = StepOutputsMatchInputsAsExpected(
         inputs_outputs_expected=inputs_outputs_expected,
```

