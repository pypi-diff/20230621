# Comparing `tmp/task_timer_birdhouses-0.0.1.tar.gz` & `tmp/task_timer_birdhouses-0.0.2.tar.gz`

## Comparing `task_timer_birdhouses-0.0.1.tar` & `task_timer_birdhouses-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/src/task_timer_birdhouses/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/src/task_timer_birdhouses/task_timer.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/LICENSE
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/src/task_timer_birdhouses/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/src/task_timer_birdhouses/task_timer.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/LICENSE
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.2/PKG-INFO
```

### Comparing `task_timer_birdhouses-0.0.1/src/task_timer_birdhouses/task_timer.py` & `task_timer_birdhouses-0.0.2/src/task_timer_birdhouses/task_timer.py`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.1/.gitignore` & `task_timer_birdhouses-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.1/LICENSE` & `task_timer_birdhouses-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.1/README.md` & `task_timer_birdhouses-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 `TaskTimer` is a Python class used to schedule and keep track of upcoming actions. You can use `TaskTimer` to automatically calculate when a given action will be executed based on a specified duration in seconds.
 
 # Usage
 To use the TaskTimer class, you need to initialize an instance of the class with an action and the amount of seconds until the action will be executed.
 
     from task_timer import TaskTimer
 
-# Initialize a new ActionScheduler
+# Initialize a new TaskTimer
     task_timer = TaskTimer('send_email', 3600)
 
 # Print the next action time in a human-friendly format
     print(task_timer.human_friendly())
 
 # Print the next action time as a datetime object
     print(str(task_timer))
```

### Comparing `task_timer_birdhouses-0.0.1/pyproject.toml` & `task_timer_birdhouses-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "task_timer_birdhouses"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="birdhouses", email="peerdenhoed@hotmail.nl" },
 ]
 description = "You can use `TaskTimer` to automatically calculate when a given task will be executed based on a specified duration in seconds."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `task_timer_birdhouses-0.0.1/PKG-INFO` & `task_timer_birdhouses-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task_timer_birdhouses
-Version: 0.0.1
+Version: 0.0.2
 Summary: You can use `TaskTimer` to automatically calculate when a given task will be executed based on a specified duration in seconds.
 Project-URL: Homepage, https://github.com/birdhouses/TaskTimer
 Project-URL: Bug Tracker, https://github.com/birdhouses/TaskTimer/issues
 Author-email: birdhouses <peerdenhoed@hotmail.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 `TaskTimer` is a Python class used to schedule and keep track of upcoming actions. You can use `TaskTimer` to automatically calculate when a given action will be executed based on a specified duration in seconds.
 
 # Usage
 To use the TaskTimer class, you need to initialize an instance of the class with an action and the amount of seconds until the action will be executed.
 
     from task_timer import TaskTimer
 
-# Initialize a new ActionScheduler
+# Initialize a new TaskTimer
     task_timer = TaskTimer('send_email', 3600)
 
 # Print the next action time in a human-friendly format
     print(task_timer.human_friendly())
 
 # Print the next action time as a datetime object
     print(str(task_timer))
```

