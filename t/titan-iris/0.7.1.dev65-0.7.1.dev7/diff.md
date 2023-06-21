# Comparing `tmp/titan-iris-0.7.1.dev65.tar.gz` & `tmp/titan-iris-0.7.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.7.1.dev65.tar", last modified: Wed Jun 21 11:11:32 2023, max compression
+gzip compressed data, was "titan-iris-0.7.1.dev7.tar", last modified: Wed Jun 21 09:07:39 2023, max compression
```

## Comparing `titan-iris-0.7.1.dev65.tar` & `titan-iris-0.7.1.dev7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.320076 titan-iris-0.7.1.dev65/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 11:11:32.320076 titan-iris-0.7.1.dev65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 11:11:32.320076 titan-iris-0.7.1.dev65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.316076 titan-iris-0.7.1.dev65/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.316076 titan-iris-0.7.1.dev65/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.316076 titan-iris-0.7.1.dev65/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27220 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.316076 titan-iris-0.7.1.dev65/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.320076 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 11:11:32.000000 titan-iris-0.7.1.dev65/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:11:32.320076 titan-iris-0.7.1.dev65/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 11:11:07.000000 titan-iris-0.7.1.dev65/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.420360 titan-iris-0.7.1.dev7/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 09:07:39.000000 titan-iris-0.7.1.dev7/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:07:39.424360 titan-iris-0.7.1.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 09:07:22.000000 titan-iris-0.7.1.dev7/tests/test_sdk.py
```

### Comparing `titan-iris-0.7.1.dev65/.gitignore` & `titan-iris-0.7.1.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/Dockerfile` & `titan-iris-0.7.1.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/PKG-INFO` & `titan-iris-0.7.1.dev7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: titan-iris
-Version: 0.7.1.dev65
-Description-Content-Type: text/markdown
-
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
 The backend takes one of the following supported models and uses it to finetune similar, smaller models. The training signals from the teacher model improve the performance of the student model on edge cases, and allow you to use cheaper, more readily-available unlabelled data.
```

### Comparing `titan-iris-0.7.1.dev65/README.md` & `titan-iris-0.7.1.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: titan-iris
+Version: 0.7.1.dev7
+Description-Content-Type: text/markdown
+
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
 The backend takes one of the following supported models and uses it to finetune similar, smaller models. The training signals from the teacher model improve the performance of the student model on edge cases, and allow you to use cheaper, more readily-available unlabelled data.
```

### Comparing `titan-iris-0.7.1.dev65/setup.py` & `titan-iris-0.7.1.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/config.yaml` & `titan-iris-0.7.1.dev7/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/gradio/run.py` & `titan-iris-0.7.1.dev7/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/main.py` & `titan-iris-0.7.1.dev7/src/iris/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import typer
 import yaml
 from trogon import Trogon
 from typer.main import get_group
 import iris.sdk as sdk
 
-from .sdk.utils import exception_to_json_error, json_output_decorator, valid_qlora
+from .sdk.utils import exception_to_json_error, json_output_decorator
 
 logger = getLogger(__name__)
 logger.setLevel(sdk.conf_mgr.LOG_LEVEL)
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                   sdk CLI Module                                                     #
 
@@ -140,172 +140,132 @@
 SUBSET_ARG = typer.Option(None, "--subset", "-ss", help="The subset of a dataset to optimize on")
 NAME_ARG = typer.Option(
     "",
     "--name",
     "-n",
     help="The name to use for this job. Visible in the TitanML Hub.",
 )
+FILE_ARG = typer.Option(
+    "",
+    "--file",
+    "-f",
+    help="Load the options from a config file",
+    callback=conf_callback,
+    is_eager=True,
+)
+TEST_ARG = typer.Option(
+    False,
+    "--short-run",
+    "-s",
+    help="Truncates the run after 1 batch and 1 epoch. \
+            Will provide bad results, but useful to check that the model and dataset choices are valid.",
+)
 NUM_LABELS_ARG = typer.Option(
     None,
     "--num-labels",
     "-nl",
-    help="Number of labels. Required for sequence_classification tasks.",
+    help="Number of labels. Required for task sequence_classification",
 )
 
-LABEL_NAMES_ARG = typer.Option(
-    None,
-    "--label-names",
-    "-ln",
-    help=(
-        "Names of token labels. Required for token_classification tasks."
-        "Specify as a mapping with no spaces: -ln 0:label1 -ln 1:label2"
-    ),
-)
-LABEL_COLUMN_ARG = typer.Option("label", "--labels-column", "-lc", help="The name of the column containing the labels.")
 TEXT_FIELDS_ARG = typer.Option(
     None,
     "--text-fields",
     "-tf",
-    help="The field(s) containing input texts. Required for sequence_classification tasks",
+    help="Text fields. Required for task sequence_classification",
 )
-BATCH_SIZE_ARG = typer.Option(
-    "4",
-    "--batch-size",
-    "-bs",
-    help="The batch size to use for training. Specifying 'auto' will use the maximum "
-    "batch_size achievable under reasonable hardware constraints.",
-)
-LEARNING_RATE_ARG = typer.Option(2e-5, "--learning-rate", "-lr", help="The learning rate to use for training.")
 
-TEST_ARG = typer.Option(
-    False,
-    "--short-run",
-    "-s",
-    help="Truncates the run after 1 batch and 1 epoch. \
-            Will provide bad results, but useful to check that the model and dataset choices are valid.",
-)
 HAS_NEGATIVE_ARG = typer.Option(
     False,
     "--has-negative",
     "-hn",
-    help="Whether the dataset includes examples which have 'no answer'. Required for question_answering tasks",
-)
-QLORA_ARG = typer.Option(
-    False,
-    "--no-qlora",
-    "-nql",
-    help="Do not use QLoRA, even when available. If not given, then QLoRA will be used " "where possible.",
-)
-# new
-TRAIN_SPLIT_NAME = typer.Option(
-    "train",
-    "--train-split-name",
-    "-tsn",
-    help="The name of the train data split",
-)
-VALID_SPLIT_NAME = typer.Option(
-    "validation",
-    "--val-split-name",
-    "-vsn",
-    help="The name of the validation data split",
-)
-JSON_ARG = typer.Option(
-    False,
-    "--json",
-    "-j",
-    help="Print output as JSON. Default: Rich output",
+    help="Has negative. Required for question_answering",
 )
-
-FILE_ARG = typer.Option(
-    "",
-    "--file",
-    "-f",
-    help="Load the options from a config file",
-    callback=conf_callback,
-    is_eager=True,
+LABEL_NAMES_ARG = typer.Option(
+    None,
+    "--label-names",
+    "-ln",
+    help="Names of token labels. Required for task token_classification. \
+            Specify as a mapping with no spaces: -ln 0:label1 -ln 1:label2",
 )
 HEADERS_ARG = typer.Option(
     [],
     "--headers",
     "-H",
     help="Headers to send with the get request. \
             Should be provided as colon separated key value pairs: -h a:b -h c:d -> {a:b, c:d}",
 )
 
+BATCH_SIZE_ARG = typer.Option("16", "--batch-size", "-bs", help="The batch size to use for training.")
+LEARNING_RATE_ARG = typer.Option("2e-5", "--learning-rate", "-lr", help="The learning rate to use for training.")
+JSON_ARG = typer.Option(
+    False,
+    "--json",
+    "-j",
+    help="Print output as JSON. Default: Rich output",
+)
+
 
 @main.command()
 def post(
     model: str = MODEL_ARG,
     dataset: str = DATASET_ARG,
     task: Task = TASK_ARG,
     subset: Optional[str] = SUBSET_ARG,
     experiment_name: str = NAME_ARG,
     file: str = FILE_ARG,
     test: bool = TEST_ARG,
     num_labels: int = NUM_LABELS_ARG,
     text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
     has_negative: bool = HAS_NEGATIVE_ARG,
-    train_split_name: Optional[str] = TRAIN_SPLIT_NAME,
-    val_split_name: Optional[str] = VALID_SPLIT_NAME,
     label_names: Optional[List[str]] = LABEL_NAMES_ARG,
     headers: List[str] = HEADERS_ARG,
     json_output: bool = JSON_ARG,
-    label_column: str = LABEL_COLUMN_ARG,
-    no_qlora: bool = QLORA_ARG,
 ):
     """Submit a pipelining job (currently defaults to distillation)."""
-    dispatch("athena", **locals(), batch_size="auto", learning_rate=None, num_epochs=5)
+    dispatch("athena", **locals(), batch_size="auto", learning_rate=None, num_epochs="5")
 
 
 @main.command()
 def distil(
     model: str = MODEL_ARG,
     dataset: str = DATASET_ARG,
     task: Task = TASK_ARG,
     subset: Optional[str] = SUBSET_ARG,
     experiment_name: str = NAME_ARG,
     file: str = FILE_ARG,
     test: bool = TEST_ARG,
     num_labels: int = NUM_LABELS_ARG,
     text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
     has_negative: bool = HAS_NEGATIVE_ARG,
-    train_split_name: Optional[str] = TRAIN_SPLIT_NAME,
-    val_split_name: Optional[str] = VALID_SPLIT_NAME,
     label_names: Optional[List[str]] = LABEL_NAMES_ARG,
     headers: List[str] = HEADERS_ARG,
     json_output: bool = JSON_ARG,
-    label_column: str = LABEL_COLUMN_ARG,
-    no_qlora: bool = QLORA_ARG,
 ):
     """Submit a knowledge distillation job."""
-    dispatch("athena", **locals(), batch_size="32", learning_rate=2e-05, num_epochs=5)
+    dispatch("athena", **locals(), batch_size=None, learning_rate=None, num_epochs="5")
 
 
 @main.command()
 def finetune(
     model: str = MODEL_ARG,
     dataset: str = DATASET_ARG,
     task: Task = TASK_ARG,
     subset: Optional[str] = SUBSET_ARG,
     experiment_name: str = NAME_ARG,
     test: bool = TEST_ARG,
     num_labels: int = NUM_LABELS_ARG,
     text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
     has_negative: bool = HAS_NEGATIVE_ARG,
-    train_split_name: Optional[str] = TRAIN_SPLIT_NAME,
-    val_split_name: Optional[str] = VALID_SPLIT_NAME,
     label_names: Optional[List[str]] = LABEL_NAMES_ARG,
     headers: List[str] = HEADERS_ARG,
     batch_size: str = BATCH_SIZE_ARG,
     learning_rate: float = LEARNING_RATE_ARG,
     json_output: bool = JSON_ARG,
-    num_epochs: int = typer.Option(1, "--num-epochs", "-ne", help="The number of epochs to finetune for."),
+    num_epochs: str = typer.Option(3, "--num-epochs", "-ep", help="The number of epochs to finetune for."),
     file: str = FILE_ARG,
-    label_column: str = LABEL_COLUMN_ARG,
-    no_qlora: bool = QLORA_ARG,
 ):
     """Submit a finetuning job."""
     dispatch("pontus", **locals())
 
 
 def dispatch(
     type,
@@ -315,223 +275,167 @@
     subset,
     experiment_name,
     file,
     test,
     num_labels,
     text_fields,
     has_negative,
-    train_split_name,
-    val_split_name,
     label_names,
     headers,
     batch_size,
     learning_rate,
     num_epochs,
     json_output,
-    label_column,
-    no_qlora,
 ):
     """Dispatch a job to the TitanML platform. Distil, Post and Athena ultimately run through here."""
     # get the enum value as task
     headers = {x.partition(":")[0]: x.partition(":")[-1] for x in headers}
     task = task.value
-    # baseline flags
-    flags = {
-        "model": model,
-        "dataset": dataset,
-        "task": task,
-        "test": test,
-        "subset": subset,
-        "type": type,
-        "num_epochs": num_epochs,
-        "train_split_name": train_split_name,  # new
-        "val_split_name": val_split_name,  # new
-        "label_column": label_column,
-    }
-    # lots of argument checking
-    if experiment_name != "":
-        flags.update({"name": experiment_name})
-    if task == "sequence_classification":
-        # sequence of task specific flags
-        # if the flag shouldn't be accepted, set error_message to the error string to print.
-        # if it should be, and you want to warn, print, but don't set error_message
-        error_message = False
-        if not num_labels and not len(label_names):
-            error_message = (
-                "Please provide either the number of labels (--num-labels, -nl) or "
-                "a mapping between user labels and (integer) dataset labels."
-            )
-        elif num_labels and len(label_names) != num_labels and len(label_names):
-            error_message = (
-                "The given label map has a different number of labels to " "that specified with --num-labels"
-            )
-        elif num_labels and len(label_names):
-            print("If providing label_names, num_labels does not need to be provided.")
-        elif label_names:
-            if not all(":" in x for x in label_names):
-                error_message = (
-                    "Label names should be specified as a map from integers to labels, e.g. "
-                    "'-ln 0:Positive -ln 1:Negative ...'"
-                )
+    try:
+        # baseline flags
+        flags = {
+            "model": model,
+            "dataset": dataset,
+            "task": task,
+            "test": test,
+            "subset": subset,
+            "type": type,
+            "num_epochs": num_epochs,
+        }
+        # lots of argument checking
+        if experiment_name != "":
+            flags.update({"name": experiment_name})
+        if task == "sequence_classification":
+            # sequence of task specific flags
+            # if the flag shouldn't be accepted, set error_message to the error string to print.
+            # if it should be, and you want to warn, print, but don't set error_message
+            error_message = False
+            if num_labels is None:
+                error_message = "Please provide the number of labels (--num-labels, -nl)"
+            if text_fields is None or len(text_fields) == 0:
+                error_message = "Please provide the text fields to tokenize (--text-fields, -tf)"
+            if label_names is not None and len(label_names) > 0:
+                print("label_names is not necessary for sequence classification tasks")
+            if has_negative:
+                print("has_negative is not necessary for sequence classification tasks")
             if error_message:
-                print(error_message)
+                raise typer.Abort(error_message)
+            else:
+                flags.update({"num_labels": num_labels, "text_fields": text_fields})
+        elif task == "question_answering":
+            is_error = False
+            # sequence of task specific flags
+            # if the flag shouldn't be accepted, set is_error=True
+            # if it should be, and you want to warn, print, but don't set is_error
+            if num_labels is not None:
+                print("num_labels is not necessary for question answering tasks")
+            if text_fields is not None and len(text_fields) > 0:
+                print("text_fields is not necessary for question answering tasks")
+            if label_names is not None and len(label_names) > 0:
+                print("label_names is not necessary for question_answering tasks")
+            if is_error:
+                raise typer.Abort()
+            else:
+                flags.update({"has_negative": has_negative})
+        elif task == "glue":
+            # sequence of task specific flags
+            # if the flag shouldn't be accepted, set is_error=True
+            # if it should be, and you want to warn, print, but don't set is_error
+            is_error = False
+            if num_labels is not None:
+                print("num_labels is not necessary for glue tasks")
+            if label_names is not None and len(label_names) > 0:
+                print("label_names is not necessary for glue tasks")
+            if text_fields is not None and text_fields != []:
+                print("text_fields is not necessary for glue tasks")
+            if has_negative:
+                print("has_negative is not necessary for glue tasks")
+            if is_error:
                 raise typer.Abort()
             else:
+                pass
+        elif task == "token_classification":
+            error_message = False
+            if num_labels is not None:
+                print("num_labels is not necessary for token classification tasks")
+            if label_names is None:
+                error_message = "Please provide the label names of the tokens"
+            if not all(":" in x for x in label_names):
+                error_message = "Label names should be specified as a map, e.g. '-ln 0:PER -ln 1:ORG ...'"
+            if error_message:
+                raise typer.Abort(error_message)
+            else:
                 label_names_dict = {int(i): label for i, label in map(lambda x: x.split(":"), label_names)}
                 label_names_num = len(list(label_names_dict.keys()))
                 max_label_num = max(i for i in label_names_dict.keys())
                 min_label_num = min(i for i in label_names_dict.keys())
                 if max_label_num != (len(list(label_names_dict.keys())) - 1):
-                    print("Label names must have contiguous indices")
+                    print("Label names must have continuous indices")
                     raise typer.Abort()
 
                 if min_label_num != 0:
                     print("Label indices must start at zero")
                     raise typer.Abort()
 
                 label_names_list = [label_names_dict[i] for i in range(label_names_num)]
                 flags.update({"label_names": label_names_list})
-        if text_fields is None or len(text_fields) == 0:
-            error_message = "Please provide the text fields to tokenize (--text-fields, -tf)"
-        if has_negative:
-            print("has_negative is not necessary for sequence classification tasks")
-        if error_message:
-            print(error_message)
-            raise typer.Abort(error_message)
 
+        elif task == "language_modelling" or task == "language_modeling":
+            # sequence of task specific flags
+            # if the flag shouldn't be accepted, set error_message to the error string to print.
+            # if it should be, and you want to warn, print, but don't set error_message
+            error_message = False
+            if type == "athena":
+                error_message = "Knowledge distillation is not yet supported for language modelling."
+            if num_labels is not None:
+                print("num_labels is not necessary for language modelling tasks")
+            if label_names is not None and len(label_names) > 0:
+                print("label_names is not necessary for language modelling tasks")
+            if has_negative:
+                print("has_negative is not necessary for language modelling tasks")
+            if error_message:
+                raise typer.Abort(error_message)
+            else:
+                flags.update({"text_fields": text_fields})
         else:
-            # new: label_names
-            flags.update({"num_labels": num_labels, "text_fields": text_fields})
-    elif task == "question_answering":
-        is_error = False
-        # sequence of task specific flags
-        # if the flag shouldn't be accepted, set is_error=True
-        # if it should be, and you want to warn, print, but don't set is_error
-        if num_labels is not None:
-            print("num_labels is not necessary for question answering tasks")
-        if text_fields is not None and len(text_fields) > 0:
-            print("text_fields is not necessary for question answering tasks")
-        if label_names is not None and len(label_names) > 0:
-            print("label_names is not necessary for question_answering tasks")
-        if is_error:
-            raise typer.Abort()
-        else:
-            flags.update({"has_negative": has_negative})
-    elif task == "glue":
-        # sequence of task specific flags
-        # if the flag shouldn't be accepted, set is_error=True
-        # if it should be, and you want to warn, print, but don't set is_error
-        is_error = False
-        if num_labels is not None:
-            print("num_labels is not necessary for glue tasks")
-        if label_names is not None and len(label_names) > 0:
-            print("label_names is not necessary for glue tasks")
-        if text_fields is not None and text_fields != []:
-            print("text_fields is not necessary for glue tasks")
-        if has_negative:
-            print("has_negative is not necessary for glue tasks")
-        if is_error:
-            raise typer.Abort()
-        else:
-            pass
-    elif task == "token_classification":
-        error_message = False
-        if num_labels is not None:
-            print("num_labels is not necessary for token classification tasks")
-        if label_names is None:
-            error_message = "Please provide the label names of the tokens"
-        if not all(":" in x for x in label_names):
-            error_message = "Label names should be specified as a map, e.g. '-ln 0:PER -ln 1:ORG ...'"
-        if error_message:
-            print(error_message)
+            print(f"Unrecognised task {task}")
             raise typer.Abort()
-        else:
-            label_names_dict = {int(i): label for i, label in map(lambda x: x.split(":"), label_names)}
-            label_names_num = len(list(label_names_dict.keys()))
-            max_label_num = max(i for i in label_names_dict.keys())
-            min_label_num = min(i for i in label_names_dict.keys())
-            if max_label_num != (len(list(label_names_dict.keys())) - 1):
-                print("Label names must have contiguous indices")
-                raise typer.Abort()
 
-            if min_label_num != 0:
-                print("Label indices must start at zero")
+        if num_epochs.isdigit() and int(num_epochs) >= 99:
+            logging.warning(
+                "Woah there cowboy, that's a mighty high number of epochs you got there. "
+                "Are you sure you didn't mistype it?"
+            )
+        if batch_size:
+            if batch_size == "auto":
+                flags["batch_size"] = batch_size
+            elif "." not in batch_size and batch_size.isdigit():
+                n = int(batch_size)
+                if not ((n != 0) and (n & (n - 1) == 0)):  # Check if batch size is power of 2.
+                    print(
+                        "Note that batch sizes which are a base-2 value (2,4,16,32,64,128...) will result in faster "
+                        "training."
+                    )
+                flags["batch_size"] = int(batch_size)
+            else:
+                print(f"Unrecognised batch size format {batch_size}")
                 raise typer.Abort()
 
-            label_names_list = [label_names_dict[i] for i in range(label_names_num)]
-            flags.update({"label_names": label_names_list})
-
-    elif task == "language_modelling" or task == "language_modeling":
-        # sequence of task specific flags
-        # if the flag shouldn't be accepted, set error_message to the error string to print.
-        # if it should be, and you want to warn, print, but don't set error_message
-        error_message = False
-        if type == "athena":
-            error_message = "Knowledge distillation is not yet supported for language modelling."
-        if label_column and len(label_column):
-            if label_column != LABEL_COLUMN_ARG.default:
-                print("label_column is not necessary for language modelling tasks")
-            flags.pop("label_column")
-        if num_labels is not None:
-            print("num_labels is not necessary for language modelling tasks")
-        if label_names is not None and len(label_names) > 0:
-            print("label_names is not necessary for language modelling tasks")
-        if has_negative:
-            print("has_negative is not necessary for language modelling tasks")
-
-        if no_qlora and valid_qlora(model):  # If want to disable qlora, but qlora is available:
-            print(f"QLoRA manually disabled for {model}")
-            use_qlora = False
-        elif not no_qlora and not valid_qlora(model):  # If qlora isn't explicitly disabled, but is not available.
-            print(f"QLoRA not available for {model}. Proceeding without QLoRA.")
-            use_qlora = False
-        elif no_qlora and not valid_qlora(model):  # Qlora disabled, but it wasn't available anyways.
-            use_qlora = False
-        else:  # Qlora not explicitly disabled, and qlora is available.
-            print("QLoRA is available and will be used.")
-            use_qlora = True
+        if learning_rate:
+            try:
+                flags["learning_rate"] = float(learning_rate)
+            except ValueError:
+                print(f"Unrecognised learning rate format {batch_size}")
+                raise typer.Abort()
 
-        if error_message:
-            print(error_message)
-            raise typer.Abort()
-        else:
-            flags.update({"text_fields": text_fields, "use_qlora": use_qlora})
-    else:
-        print(f"Unrecognised task {task}")
+        # post the resulting flags
+        sdk.post(headers, **flags, json_output=json_output)
+    except Exception:
         raise typer.Abort()
 
-    if num_epochs >= 99:
-        logging.warning(
-            "Woah there cowboy, that's a mighty high number of epochs you got there. "
-            "Are you sure you didn't mistype it?"
-        )
-    if batch_size:
-        if batch_size == "auto":
-            flags["batch_size"] = batch_size
-        elif "." not in batch_size and batch_size.isdigit():
-            n = int(batch_size)
-            if not ((n != 0) and (n & (n - 1) == 0)):  # Check if batch size is power of 2.
-                print(
-                    "Note that batch sizes which are a base-2 value (2,4,16,32,64,128...) will result in faster "
-                    "training."
-                )
-            flags["batch_size"] = int(batch_size)
-        else:
-            print(f"Unrecognised batch size format {batch_size}")
-            raise typer.Abort()
-    if learning_rate:
-        try:
-            flags["learning_rate"] = float(learning_rate)
-        except ValueError:
-            print(f"Unrecognised learning rate format {batch_size}")
-            raise typer.Abort()
-
-    # post the resulting flags
-    sdk.post(headers, **flags, json_output=json_output)
-
 
 @main.command()
 def get(
     object: Object = typer.Argument("experiment", help="What type of object to get"),
     id: Optional[str] = typer.Option(
         None,
         "--id",
```

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/auth_utils.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/conf_manager.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/exception.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/iris_sdk.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/safe_convert.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/src/iris/sdk/utils.py` & `titan-iris-0.7.1.dev7/src/iris/sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
 logger = getLogger("iris.utils")
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                         Utils                                                        #
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
-
-VALID_QLORA_MODELS = ["t5", "pythia", "opt", "gptj", "gptneo"]
 # ------------------------------  Helper Function for Iris Pull, Upload and Download   ------------------------------ #
 
 
 def make_targz(local_folder_path: str):
     """Create a tar.gz archive of the local folder - make this deterministic / exclude timestamp info from gz header.
 
     Args:
@@ -235,34 +233,14 @@
             tarred.seek(0)
             reader_wrapper = CallbackIOWrapper(t.update, tarred, "read")
             response = requests.put(dst, data=reader_wrapper)
             response.raise_for_status()
             return response
 
 
-def valid_qlora(model_name: str):
-    """Cleanses an input model name and then checks if QLoRA has been implemented for it.
-
-    This is based on those available in Olympus.
-
-    Args:
-        model_name: A model name as from model_name_or_path
-
-    Returns: (Bool) Whether QLoRa is supported for the given model.
-
-    """
-
-    def clean(x: str) -> str:
-        return x.replace("-", "").replace("_", "").lower()
-
-    if any(ext in clean(model_name) for ext in VALID_QLORA_MODELS):
-        return True
-    return False
-
-
 def exception_to_json_error(e: Exception):
     """Convert an exception to a json string with the error message and type."""
     logger.error(e)
     error_dict = {"status": "failed", "error": str(e), "type": type(e).__name__}
     if hasattr(e, "status_code"):
         error_dict["status_code"] = e.status_code
     return json.dumps(error_dict, indent=4)
```

### Comparing `titan-iris-0.7.1.dev65/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.7.1.dev7/src/titan_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.1.dev65
+Version: 0.7.1.dev7
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.1.dev65/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.7.1.dev7/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/tests/test_cli.py` & `titan-iris-0.7.1.dev7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev65/tests/test_sdk.py` & `titan-iris-0.7.1.dev7/tests/test_sdk.py`

 * *Files identical despite different names*

