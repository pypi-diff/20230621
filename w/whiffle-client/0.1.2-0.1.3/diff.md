# Comparing `tmp/whiffle_client-0.1.2.tar.gz` & `tmp/whiffle_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/app/dist/.tmp-h4b32k12/whiffle_client-0.1.2.tar", last modified: Tue Jun 20 10:17:12 2023, max compression
+gzip compressed data, was "/app/dist/.tmp-xiwz3ys9/whiffle_client-0.1.3.tar", last modified: Wed Jun 21 06:54:00 2023, max compression
```

## Comparing `whiffle_client-0.1.2.tar` & `whiffle_client-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-20 10:03:07.000000 whiffle_client-0.1.2/LICENCE.txt
--rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1079 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      780 2023-06-20 10:06:11.000000 whiffle_client-0.1.2/README.md
--rw-rw-r--   0 root         (0) root         (0)      740 2023-06-20 10:16:02.000000 whiffle_client-0.1.2/USER_README.md
--rw-rw-r--   0 root         (0) root         (0)      681 2023-06-20 10:16:07.000000 whiffle_client-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/tests/
--rw-rw-r--   0 root         (0) root         (0)     3259 2023-06-16 12:41:36.000000 whiffle_client-0.1.2/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client/
--rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/client.py
--rw-rw-r--   0 root         (0) root         (0)     1855 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client/resources/
--rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/resources/example_generic_params.json
--rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-20 10:03:07.000000 whiffle_client-0.1.3/LICENCE.txt
+-rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      780 2023-06-20 10:06:11.000000 whiffle_client-0.1.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)      994 2023-06-21 06:51:29.000000 whiffle_client-0.1.3/USER_README.md
+-rw-rw-r--   0 root         (0) root         (0)      681 2023-06-21 06:53:36.000000 whiffle_client-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)     3502 2023-06-20 16:15:11.000000 whiffle_client-0.1.3/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client/
+-rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/client.py
+-rw-rw-r--   0 root         (0) root         (0)     2515 2023-06-20 16:14:16.000000 whiffle_client-0.1.3/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client/resources/
+-rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/resources/example_generic_params.json
+-rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.3/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 06:54:00.000000 whiffle_client-0.1.3/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.1.2/LICENCE.txt` & `whiffle_client-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.2/PKG-INFO` & `whiffle_client-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
@@ -15,14 +15,19 @@
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
 
+The client polls the progress of the task until it has finished. The task will run in the background if you abort the client.
+You can list the most recent tasks by executing,
+
+`whiffle tasks-list`
+
 If you need an access token or you have any questions, please reach out to <support@whiffle.nl>.
 
 ## Command-line interface
 
 ### List the configuration
 
 `whiffle config-list`
@@ -30,7 +35,11 @@
 ### Change the token in the configuration
 
 `whiffle config-edit user.token <your_token>`
 
 ### Run a task
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
+
+### List tasks
+
+`whiffle tasks-list <number of tasks>`
```

### Comparing `whiffle_client-0.1.2/README.md` & `whiffle_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.2/USER_README.md` & `whiffle_client-0.1.3/USER_README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,31 @@
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
 
+The client polls the progress of the task until it has finished. The task will run in the background if you abort the client.
+You can list the most recent tasks by executing,
+
+`whiffle tasks-list`
+
 If you need an access token or you have any questions, please reach out to <support@whiffle.nl>.
 
 ## Command-line interface
 
 ### List the configuration
 
 `whiffle config-list`
 
 ### Change the token in the configuration
 
 `whiffle config-edit user.token <your_token>`
 
 ### Run a task
 
-`whiffle run <path_to_the_task_specification.[json|yaml]>`
+`whiffle run <path_to_the_task_specification.[json|yaml]>`
+
+### List tasks
+
+`whiffle tasks-list <number of tasks>`
```

### Comparing `whiffle_client-0.1.2/pyproject.toml` & `whiffle_client-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "whiffle_client"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python based web client to interact with Whiffle services"
 readme = "USER_README.md"
 
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `whiffle_client-0.1.2/tests/test_client.py` & `whiffle_client-0.1.3/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,7 +102,15 @@
     def test_run_task(self, mocker):
         mock_new_task_response(mocker)
         mock = mocker.patch(
             "whiffle_client.Client.communicate",
         )
         runner.invoke(whiffle, ["run", default_task_path])
         mock.assert_called_once()
+
+    def test_run_task(self, mocker):
+        mock_new_task_response(mocker)
+        mock = mocker.patch(
+            "whiffle_client.Client.get_tasks",
+        )
+        runner.invoke(whiffle, ["tasks-list"])
+        mock.assert_called_once()
```

### Comparing `whiffle_client-0.1.2/whiffle_client/client.py` & `whiffle_client-0.1.3/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.2/whiffle_client/entrypoints.py` & `whiffle_client-0.1.3/whiffle_client/entrypoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,35 @@
 
 @click.group()
 def whiffle():
     pass
 
 
 @whiffle.command()
+@click.argument("number_of_tasks", default=10)
+def tasks_list(number_of_tasks):
+    number_of_tasks = int(number_of_tasks)
+    client = Client()
+    tasks = client.get_tasks()
+    click.echo(
+        "{:33}{:11}{:16} {:16} progress".format(
+            "task id", "status", "start time", "finish time"
+        )
+    )
+    for task in tasks[-number_of_tasks:]:
+        finished = task["finished"]
+        if finished == None:
+            task["finished"] = ""
+        click.echo(
+            "{task_id:33}{task_status:11}{received:17.16}{finished:17.16}{processed_steps}/{total_steps}".format(
+                **task
+            )
+        )
+
+@whiffle.command()
 @click.argument("file_path")
 def run(file_path) -> str:
     """Run task type given a set of parameters.
 
     \b
     Parameters
     ----------
```

### Comparing `whiffle_client-0.1.2/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.1.3/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.2/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.1.3/whiffle_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
@@ -15,14 +15,19 @@
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
 
+The client polls the progress of the task until it has finished. The task will run in the background if you abort the client.
+You can list the most recent tasks by executing,
+
+`whiffle tasks-list`
+
 If you need an access token or you have any questions, please reach out to <support@whiffle.nl>.
 
 ## Command-line interface
 
 ### List the configuration
 
 `whiffle config-list`
@@ -30,7 +35,11 @@
 ### Change the token in the configuration
 
 `whiffle config-edit user.token <your_token>`
 
 ### Run a task
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
+
+### List tasks
+
+`whiffle tasks-list <number of tasks>`
```

