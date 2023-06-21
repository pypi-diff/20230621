# Comparing `tmp/Akatosh-1.7.2.tar.gz` & `tmp/Akatosh-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-1.7.2.tar", last modified: Fri Jun 16 08:13:48 2023, max compression
+gzip compressed data, was "Akatosh-1.7.3.tar", last modified: Wed Jun 21 13:17:54 2023, max compression
```

## Comparing `Akatosh-1.7.2.tar` & `Akatosh-1.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:13:48.679137 Akatosh-1.7.2/
-drwxrwxrwx   0        0        0        0 2023-06-16 08:13:48.657133 Akatosh-1.7.2/Akatosh/
--rw-rw-rw-   0        0        0      129 2023-05-17 02:07:37.000000 Akatosh-1.7.2/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    17075 2023-05-17 02:07:37.000000 Akatosh-1.7.2/Akatosh/actor.py
--rw-rw-rw-   0        0        0     1073 2023-05-17 02:07:37.000000 Akatosh-1.7.2/Akatosh/event.py
--rw-rw-rw-   0        0        0     6678 2023-05-17 02:07:37.000000 Akatosh-1.7.2/Akatosh/producer.py
--rw-rw-rw-   0        0        0    11540 2023-05-17 02:07:37.000000 Akatosh-1.7.2/Akatosh/resource.py
--rw-rw-rw-   0        0        0     1443 2023-06-16 08:12:40.000000 Akatosh-1.7.2/Akatosh/timeline.py
--rw-rw-rw-   0        0        0     2443 2023-06-16 08:12:33.000000 Akatosh-1.7.2/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:13:48.668131 Akatosh-1.7.2/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-06-16 08:13:48.000000 Akatosh-1.7.2/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-16 08:13:48.000000 Akatosh-1.7.2/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:13:48.000000 Akatosh-1.7.2/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 08:13:48.000000 Akatosh-1.7.2/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-06-16 08:13:48.677131 Akatosh-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2023-05-17 02:07:37.000000 Akatosh-1.7.2/README.md
--rw-rw-rw-   0        0        0      669 2023-06-16 08:13:01.000000 Akatosh-1.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 08:13:48.679137 Akatosh-1.7.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 08:13:48.675132 Akatosh-1.7.2/test/
--rw-rw-rw-   0        0        0      169 2023-05-17 02:07:37.000000 Akatosh-1.7.2/test/test_actor.py
--rw-rw-rw-   0        0        0      245 2023-05-17 02:07:37.000000 Akatosh-1.7.2/test/test_decorator.py
--rw-rw-rw-   0        0        0      298 2023-05-17 02:07:37.000000 Akatosh-1.7.2/test/test_resource.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.529914 Akatosh-1.7.3/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.509910 Akatosh-1.7.3/Akatosh/
+-rw-rw-rw-   0        0        0      129 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    16093 2023-06-21 13:15:43.000000 Akatosh-1.7.3/Akatosh/actor.py
+-rw-rw-rw-   0        0        0     1073 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/event.py
+-rw-rw-rw-   0        0        0     6678 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/producer.py
+-rw-rw-rw-   0        0        0    11540 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/resource.py
+-rw-rw-rw-   0        0        0     1443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/timeline.py
+-rw-rw-rw-   0        0        0     2443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.518911 Akatosh-1.7.3/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.528915 Akatosh-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-1.7.3/README.md
+-rw-rw-rw-   0        0        0      669 2023-06-21 13:16:13.000000 Akatosh-1.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:17:54.529914 Akatosh-1.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.525910 Akatosh-1.7.3/test/
+-rw-rw-rw-   0        0        0      169 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_actor.py
+-rw-rw-rw-   0        0        0      245 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_decorator.py
+-rw-rw-rw-   0        0        0      298 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_resource.py
```

### Comparing `Akatosh-1.7.2/Akatosh/actor.py` & `Akatosh-1.7.3/Akatosh/actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                     f"Current accuracy is {Mundus.accuracy}, step size cannot be smaller than {(1/pow(10, Mundus.accuracy))/2}."
                 )
             self._step = round(step, Mundus.accuracy)
         else:
             self._step = step
 
         if callable(till):
-            self._till = till
+            self._till = round(till(), Mundus.accuracy)
         elif till is not None:
             self._till = round(till, Mundus.accuracy)
         else:
             self._till = till
 
         # initialize the status
         self._status = list()
@@ -139,49 +139,31 @@
                     if callable(self.step):
                         self._time += round(self.step(), Mundus.accuracy)
                     else:
                         self._time += round(self.step, Mundus.accuracy)
                     yield self.timeline.schedule(self)
             # continuous actor with step size and end time
             elif self.step is not None and self.till is not None:
-                if callable(self.till):
-                    _till = round(self.till(), Mundus.accuracy)
-                    while True:
-                        self.action(**self.kwargs)
-                        if callable(self.step):
-                            self._time += round(self.step(), Mundus.accuracy)
-                        else:
-                            self._time += round(self.step, Mundus.accuracy)
-                        if self.time <= _till:  # type: ignore
-                            yield self.timeline.schedule(self)
-                        else:
+                while True:
+                    self.action(**self.kwargs)
+                    if callable(self.step):
+                        self._time += round(self.step(), Mundus.accuracy)
+                    else:
+                        self._time += round(self.step, Mundus.accuracy)
+                    if self.time <= self.till:  # type: ignore
+                        yield self.timeline.schedule(self)
+                    else:
+                        # if this is the last step, activate all followers
+                        if self.time >= self.till:
                             self.status.append("completed")
                             self.status.append("terminated")
                             for actor in self.followers:
                                 if actor.onhold:
                                     actor.activate(force=False)
-                            break
-                else:
-                    while True:
-                        self.action(**self.kwargs)
-                        if callable(self.step):
-                            self._time += round(self.step(), Mundus.accuracy)
-                        else:
-                            self._time += round(self.step, Mundus.accuracy)
-                        if self.time <= self.till:  # type: ignore
-                            yield self.timeline.schedule(self)
-                        else:
-                            # if this is the last step, activate all followers
-                            if self.time >= self.till:
-                                self.status.append("completed")
-                                self.status.append("terminated")
-                                for actor in self.followers:
-                                    if actor.onhold:
-                                        actor.activate(force=False)
-                            break
+                        break
 
     def deactivate(self, terminate: bool = True):
         """Deactivate the actor. If terminate is True, the actor will be terminated. If terminate is False, the actor will be put on hold.
 
         Args:
             terminate (bool, optional): if the actor should be terminated. Defaults to True.
         """
```

### Comparing `Akatosh-1.7.2/Akatosh/event.py` & `Akatosh-1.7.3/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/Akatosh/producer.py` & `Akatosh-1.7.3/Akatosh/producer.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/Akatosh/resource.py` & `Akatosh-1.7.3/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/Akatosh/timeline.py` & `Akatosh-1.7.3/Akatosh/timeline.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/Akatosh/universe.py` & `Akatosh-1.7.3/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/Akatosh.egg-info/PKG-INFO` & `Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.2
+Version: 1.7.3
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.2/PKG-INFO` & `Akatosh-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.2
+Version: 1.7.3
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.2/README.md` & `Akatosh-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.2/pyproject.toml` & `Akatosh-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "1.7.2"
+version = "1.7.3"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

