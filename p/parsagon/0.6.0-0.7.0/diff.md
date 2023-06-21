# Comparing `tmp/parsagon-0.6.0.tar.gz` & `tmp/parsagon-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.6.0.tar", last modified: Tue Jun 20 07:17:13 2023, max compression
+gzip compressed data, was "parsagon-0.7.0.tar", last modified: Wed Jun 21 21:20:22 2023, max compression
```

## Comparing `parsagon-0.6.0.tar` & `parsagon-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.475489 parsagon-0.6.0/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-20 07:17:13.475125 parsagon-0.6.0/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 07:00:10.000000 parsagon-0.6.0/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1220 2023-06-20 07:14:01.000000 parsagon-0.6.0/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-20 07:17:13.475588 parsagon-0.6.0/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.463320 parsagon-0.6.0/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.6.0/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.469691 parsagon-0.6.0/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.6.0/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.6.0/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.6.0/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010    10607 2023-06-19 04:36:28.000000 parsagon-0.6.0/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     5625 2023-06-20 03:50:17.000000 parsagon-0.6.0/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.6.0/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.474752 parsagon-0.6.0/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.6.0/src/parsagon/tests/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.474360 parsagon-0.6.0/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010      141 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      319 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.822281 parsagon-0.7.0/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-21 21:20:22.821592 parsagon-0.7.0/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.0/README.md
+-rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-21 07:48:34.000000 parsagon-0.7.0/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-21 21:20:22.822496 parsagon-0.7.0/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.810031 parsagon-0.7.0/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.0/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.816205 parsagon-0.7.0/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.7.0/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.7.0/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.0/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010    10507 2023-06-21 19:40:39.000000 parsagon-0.7.0/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     6683 2023-06-21 20:28:30.000000 parsagon-0.7.0/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.0/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.820764 parsagon-0.7.0/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.0/src/parsagon/tests/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.819899 parsagon-0.7.0/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.6.0/PKG-INFO` & `parsagon-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.6.0
+Version: 0.7.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.6.0/README.md` & `parsagon-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.6.0/pyproject.toml` & `parsagon-0.7.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,49 +6,40 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.6.0"
+version = "0.7.0"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    # Also change requirements.in
     'selenium == 4.9.1',
     'lxml == 4.9.2',
-    'webdriver-manager == 3.8.6',
     'httpx == 0.24.1',
 
     # Used only in pipeline code execution
     'pandas==1.4.2',
-    'requests==2.27.1',
-    'SQLAlchemy==1.4.31',
-    'psycopg2==2.9.3',
     'PyVirtualDisplay==3.0',
     'selenium-wire==5.1.0',
     'cssselect==1.1.0',
     'undetected-chromedriver==3.1.5.post4',
     'jsonpath-ng==1.5.3',
-    'dbfread==2.0.7',
-    'geopandas==0.12.1',
     'usaddress==0.5.10',
     'simplejson==3.19.1',
 ]
 
 [project.urls]
 "Homepage" = "https://parsagon.io"
 
 [project.scripts]
-parsagon-create = "parsagon.main:create_cli"
-parsagon-detail = "parsagon.main:detail_cli"
-parsagon-run = "parsagon.main:run_cli"
+parsagon = "parsagon.main:main"
```

### Comparing `parsagon-0.6.0/src/parsagon/api.py` & `parsagon-0.7.0/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.6.0/src/parsagon/custom_function.py` & `parsagon-0.7.0/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.6.0/src/parsagon/executor.py` & `parsagon-0.7.0/src/parsagon/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import lxml.html
 from selenium import webdriver
 import seleniumwire.undetected_chromedriver as uc
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.select import Select
-from webdriver_manager.chrome import ChromeDriverManager
 
 from parsagon.api import get_interaction_element_id, scrape_page
 from parsagon.custom_function import CustomFunction
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,15 +30,14 @@
     """
     Executes code produced by GPT with the proper context.  Records custom_function usage along the way.
     """
 
     def __init__(self):
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument("--start-maximized")
-        # ChromeDriverManager().install(),
         seleniumwire_options = {"disable_capture": True}
         self.driver = uc.Chrome(options=chrome_options, seleniumwire_options=seleniumwire_options)
         self.max_elem_id = 0
         self.execution_context = {
             "goto": self.goto,
             "click_elem": self.click_elem,
             "fill_input": self.fill_input,
```

### Comparing `parsagon-0.6.0/src/parsagon/main.py` & `parsagon-0.7.0/src/parsagon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,113 @@
 import argparse
 import json
 import logging
 import logging.config
 
+from parsagon import settings
 from parsagon.api import (
     get_program_sketches,
     create_pipeline,
     delete_pipeline,
     create_custom_function,
     get_pipeline,
     get_pipelines,
     get_pipeline_code,
     APIException,
 )
 from parsagon.executor import Executor, custom_functions_to_descriptions
-from parsagon.settings import get_logging_config
 
 logger = logging.getLogger(__name__)
 
 
-def create_cli():
+def configure_logging(verbose):
+    logging.config.dictConfig(settings.get_logging_config("DEBUG" if verbose else "INFO"))
+
+
+def main():
     parser = argparse.ArgumentParser(
-        prog="parsagon-create",
-        description="Scrapes and interacts with web pages based on natural language.",
+        prog="parsagon", description="Scrapes and interacts with web pages based on natural language.", add_help=False
     )
+    parser.add_argument("-v", "--verbose", action="store_true", help="run the task in verbose mode")
+    subparsers = parser.add_subparsers()
 
-    parser.add_argument(
+    # Create
+    parser_create = subparsers.add_parser("create", description="Creates a program.")
+    parser_create.add_argument(
         "task",
         metavar="task",
         type=str,
         help="natural language description of the task to run, optionally with numbered steps.",
     )
-    parser.add_argument("-v", "--verbose", action="store_true", help="run the task in verbose mode")
-    parser.add_argument(
-        "-p", "--program", type=str, help="the name of the program to create (otherwise user input is required)"
+    parser_create.add_argument(
+        "-p",
+        "--program",
+        dest="program_name",
+        type=str,
+        help="the name of the program to create (otherwise user input is required)",
     )
+    parser_create.set_defaults(func=create)
 
-    args = parser.parse_args()
-    task = args.task
-    verbose = args.verbose
-    pipeline_name = args.program
-    create(task, pipeline_name, verbose=verbose)
-
+    # Detail
+    parser_detail = subparsers.add_parser(
+        "detail",
+        description="Outputs details of a created program.",
+    )
+    parser_detail.add_argument(
+        "-p",
+        "--program",
+        dest="program_name",
+        type=str,
+        help="the name of the program",
+    )
+    parser_detail.set_defaults(func=detail)
 
-def configure_logging(verbose):
-    logging.config.dictConfig(get_logging_config("DEBUG" if verbose else "INFO"))
+    # Run
+    parser_run = subparsers.add_parser(
+        "run",
+        description="Runs a created program.",
+    )
+    parser_run.add_argument(
+        "program_name",
+        type=str,
+        help="the name of the program to run",
+    )
+    parser_run.add_argument(
+        "--variables",
+        type=json.loads,
+        default="{}",
+        help="a JSON object mapping variables to values",
+    )
+    parser_run.set_defaults(func=run)
 
+    # Delete
+    parser_delete = subparsers.add_parser(
+        "delete",
+        description="Deletes a program.",
+    )
+    parser_delete.add_argument(
+        "program_name",
+        type=str,
+        help="the name of the program to run",
+    )
+    parser_delete.set_defaults(func=delete)
 
-def create(task, pipeline_name=None, verbose=False):
+    args = parser.parse_args()
+    kwargs = vars(args)
+    func = kwargs.pop("func")
+    verbose = kwargs["verbose"]
     configure_logging(verbose)
 
+    if func:
+        return func(**kwargs)
+    else:
+        parser.print_help()
+
+
+def create(task, program_name=None, verbose=False):
     logger.info("Launched with task description:\n%s", task)
 
     logger.info("Analyzing task description...")
     program_sketches = get_program_sketches(task)
 
     full_program = program_sketches["full"]
     abridged_program = program_sketches["abridged"]
@@ -62,24 +116,24 @@
 
     # Execute the abridged program to gather examples
     executor = Executor()
     executor.execute(abridged_program)
 
     # The user must select a name
     while True:
-        if not pipeline_name:
-            pipeline_name = input("Name this program, or press enter without typing a name to DISCARD: ")
-        if pipeline_name:
-            logger.info(f"Saving program as {pipeline_name}")
+        if not program_name:
+            program_name = input("Name this program, or press enter without typing a name to DISCARD: ")
+        if program_name:
+            logger.info(f"Saving program as {program_name}")
             try:
-                pipeline = create_pipeline(pipeline_name, task, full_program)
+                pipeline = create_pipeline(program_name, task, full_program)
             except APIException as e:
-                if isinstance(e.value, list) and "Pipeline with name already exists" in e.value:
+                if isinstance(e.value, list) and "Program with name already exists" in e.value:
                     logger.info("A program with this name already exists. Please choose another name.")
-                    pipeline_name = None
+                    program_name = None
                     continue
                 else:
                     raise e
             pipeline_id = pipeline["id"]
             try:
                 for call_id, custom_function in executor.custom_functions.items():
                     debug_suffix = f" ({custom_function.name})"
@@ -98,71 +152,56 @@
         else:
             logger.info("Discarded program.")
             break
 
     logger.info("Done.")
 
 
-def detail_cli():
-    parser = argparse.ArgumentParser(
-        prog="parsagon-detail",
-        description="Outputs details of a created program.",
-    )
-    parser.add_argument(
-        "--program",
-        type=str,
-        help="the name of the program",
-    )
-    args = parser.parse_args()
-    pipeline_name = args.program
-    return detail(pipeline_name)
-
-
-def detail(pipeline_name=None):
-    if pipeline_name:
-        data = [get_pipeline(pipeline_name)]
+def detail(program_name=None, verbose=False):
+    if program_name:
+        data = [get_pipeline(program_name)]
     else:
         data = get_pipelines()
     for pipeline in data:
-        print(f"Program: {pipeline['name']}\nDescription: {pipeline['description']}\nVariables: {pipeline['variables']}\n")
-
-
-def run_cli():
-    parser = argparse.ArgumentParser(
-        prog="parsagon-run",
-        description="Runs a created program.",
-    )
-    parser.add_argument(
-        "program",
-        type=str,
-        help="the name of the program to run",
-    )
-    parser.add_argument(
-        "--variables",
-        type=json.loads,
-        default="{}",
-        help="a JSON object mapping variables to values",
-    )
-    parser.add_argument("-v", "--verbose", action="store_true", help="run the task in verbose mode")
-    args = parser.parse_args()
-    pipeline_name = args.program
-    variables = args.variables
-    verbose = args.verbose
-    return run(pipeline_name, variables=variables, environment="LOCAL", verbose=verbose)
+        print(
+            f"Program: {pipeline['name']}\nDescription: {pipeline['description']}\nVariables: {pipeline['variables']}\n"
+        )
 
 
-def run(pipeline_name, variables={}, environment="LOCAL", verbose=False):
+def run(program_name, variables={}, environment="LOCAL", verbose=False):
     """
     Executes pipeline code
     """
-    configure_logging(verbose)
-    logger.info("Preparing to run program %s", pipeline_name)
-    code = get_pipeline_code(pipeline_name, variables, environment)["code"]
+    logger.info("Preparing to run program %s", program_name)
+    try:
+        code = get_pipeline_code(program_name, variables, environment)["code"]
+    except APIException as e:
+        if isinstance(e.value, dict) and e.value.get("detail") == "Not found.":
+            logger.error("Error: A program with this name does not exist.")
+            return
+        else:
+            raise e
+
     logger.info("Running program...")
-    globals_locals = {}
+    globals_locals = {"PARSAGON_API_KEY": settings.API_KEY}
     try:
         exec(code, globals_locals, globals_locals)
     finally:
         if "driver" in globals_locals:
             globals_locals["driver"].quit()
     logger.info("Done.")
     return globals_locals["output"]
+
+
+def delete(program_name, verbose=False):
+    logger.info("Preparing to delete program %s", program_name)
+    try:
+        pipeline_id = get_pipeline(program_name)["id"]
+    except APIException as e:
+        if isinstance(e.value, dict) and e.value.get("detail") == "Not found.":
+            logger.error("Error: A program with this name does not exist.")
+            return
+        else:
+            raise e
+    logger.info("Deleting program...")
+    delete_pipeline(pipeline_id)
+    logger.info("Done.")
```

### Comparing `parsagon-0.6.0/src/parsagon/settings.py` & `parsagon-0.7.0/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.6.0/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.0/src/parsagon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.6.0
+Version: 0.7.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

