# Comparing `tmp/task_timer_birdhouses-1.0.0.tar.gz` & `tmp/task_timer_birdhouses-1.0.1.tar.gz`

## Comparing `task_timer_birdhouses-1.0.0.tar` & `task_timer_birdhouses-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/.gitattributes
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/src/task_timer_birdhouses/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/src/task_timer_birdhouses/task_timer.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/LICENSE
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/README.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/.gitattributes
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/src/task_timer_birdhouses/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/src/task_timer_birdhouses/task_timer.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/README.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 task_timer_birdhouses-1.0.1/PKG-INFO
```

### Comparing `task_timer_birdhouses-1.0.0/src/task_timer_birdhouses/task_timer.py` & `task_timer_birdhouses-1.0.1/src/task_timer_birdhouses/task_timer.py`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-1.0.0/.gitignore` & `task_timer_birdhouses-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-1.0.0/LICENSE` & `task_timer_birdhouses-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-1.0.0/README.md` & `task_timer_birdhouses-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,27 @@
     print(TaskTimer.get_upcoming_actions())
 
     # Output
     {'send_email': 'June 21, 2023, 02:11 AM'}
 
 In the example above, 'send_email' is the action we're scheduling, and 3600 is the number of seconds until the action will be executed.
 
+### Other use cases
+If you just want to add the sleep time in seconds to the current time you can do this:
 
+        task_timer = TaskTimer('test', 5)
+
+        print(task_timer)
+        # Output
+        2023-06-21 13:03:53.582599
+
+        print(task_timer.human_friendly())
+        # Output
+        June 21, 2023, 02:11 AM
+
+This might be useful if you use a different setup for executing your functions, and you only want to display the time a function will be executed.
 ## Installation
 
 This package can be installed using pip:
 
 ```bash
 pip install task-timer-birdhouses
```

### Comparing `task_timer_birdhouses-1.0.0/pyproject.toml` & `task_timer_birdhouses-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "task_timer_birdhouses"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="birdhouses", email="peerdenhoed@hotmail.nl" },
 ]
 description = "You can use `TaskTimer` to automatically calculate and execute when a given function will be executed based on a specified duration in seconds."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `task_timer_birdhouses-1.0.0/PKG-INFO` & `task_timer_birdhouses-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task_timer_birdhouses
-Version: 1.0.0
+Version: 1.0.1
 Summary: You can use `TaskTimer` to automatically calculate and execute when a given function will be executed based on a specified duration in seconds.
 Project-URL: Homepage, https://github.com/birdhouses/TaskTimer
 Project-URL: Bug Tracker, https://github.com/birdhouses/TaskTimer/issues
 Author-email: birdhouses <peerdenhoed@hotmail.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,14 +43,27 @@
     print(TaskTimer.get_upcoming_actions())
 
     # Output
     {'send_email': 'June 21, 2023, 02:11 AM'}
 
 In the example above, 'send_email' is the action we're scheduling, and 3600 is the number of seconds until the action will be executed.
 
+### Other use cases
+If you just want to add the sleep time in seconds to the current time you can do this:
 
+        task_timer = TaskTimer('test', 5)
+
+        print(task_timer)
+        # Output
+        2023-06-21 13:03:53.582599
+
+        print(task_timer.human_friendly())
+        # Output
+        June 21, 2023, 02:11 AM
+
+This might be useful if you use a different setup for executing your functions, and you only want to display the time a function will be executed.
 ## Installation
 
 This package can be installed using pip:
 
 ```bash
 pip install task-timer-birdhouses
```

