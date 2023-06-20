# Comparing `tmp/task_timer_birdhouses-0.0.4.tar.gz` & `tmp/task_timer_birdhouses-0.0.5.tar.gz`

## Comparing `task_timer_birdhouses-0.0.4.tar` & `task_timer_birdhouses-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/.gitattributes
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/src/task_timer_birdhouses/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/src/task_timer_birdhouses/task_timer.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/LICENSE
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/.gitattributes
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/src/task_timer_birdhouses/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/src/task_timer_birdhouses/task_timer.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/LICENSE
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 task_timer_birdhouses-0.0.5/PKG-INFO
```

### Comparing `task_timer_birdhouses-0.0.4/src/task_timer_birdhouses/task_timer.py` & `task_timer_birdhouses-0.0.5/src/task_timer_birdhouses/task_timer.py`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.4/.gitignore` & `task_timer_birdhouses-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.4/LICENSE` & `task_timer_birdhouses-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.4/README.md` & `task_timer_birdhouses-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `task_timer_birdhouses-0.0.4/pyproject.toml` & `task_timer_birdhouses-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "task_timer_birdhouses"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="birdhouses", email="peerdenhoed@hotmail.nl" },
 ]
 description = "You can use `TaskTimer` to automatically calculate when a given task will be executed based on a specified duration in seconds."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `task_timer_birdhouses-0.0.4/PKG-INFO` & `task_timer_birdhouses-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task_timer_birdhouses
-Version: 0.0.4
+Version: 0.0.5
 Summary: You can use `TaskTimer` to automatically calculate when a given task will be executed based on a specified duration in seconds.
 Project-URL: Homepage, https://github.com/birdhouses/TaskTimer
 Project-URL: Bug Tracker, https://github.com/birdhouses/TaskTimer/issues
 Author-email: birdhouses <peerdenhoed@hotmail.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

