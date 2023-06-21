# Comparing `tmp/Signal8-4.0.tar.gz` & `tmp/Signal8-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.0.tar", last modified: Mon Jun 19 21:18:18 2023, max compression
+gzip compressed data, was "Signal8-4.1.tar", last modified: Wed Jun 21 21:43:48 2023, max compression
```

## Comparing `Signal8-4.0.tar` & `Signal8-4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:18.363695 Signal8-4.0/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.0/LICENSE
--rw-rw-rw-   0        0        0     5357 2023-06-19 21:18:18.340696 Signal8-4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4859 2023-06-19 21:11:01.000000 Signal8-4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:18.247697 Signal8-4.0/Signal8/
--rw-rw-rw-   0        0        0    11783 2023-06-19 21:16:35.000000 Signal8-4.0/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.0/Signal8/__init__.py
--rw-rw-rw-   0        0        0      242 2023-06-19 21:10:10.000000 Signal8-4.0/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:18.334696 Signal8-4.0/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.0/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.0/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     1100 2023-06-19 19:38:38.000000 Signal8-4.0/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.0/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11993 2023-06-19 21:07:54.000000 Signal8-4.0/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.0/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:18.298696 Signal8-4.0/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5357 2023-06-19 21:18:17.000000 Signal8-4.0/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-19 21:18:18.000000 Signal8-4.0/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:18:17.000000 Signal8-4.0/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 21:18:17.000000 Signal8-4.0/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 21:18:18.363695 Signal8-4.0/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-19 21:17:47.000000 Signal8-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.993205 Signal8-4.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.1/LICENSE
+-rw-rw-rw-   0        0        0     4763 2023-06-21 21:43:47.990205 Signal8-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4265 2023-06-20 21:50:49.000000 Signal8-4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.872205 Signal8-4.1/Signal8/
+-rw-rw-rw-   0        0        0    11770 2023-06-21 21:42:34.000000 Signal8-4.1/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.1/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      242 2023-06-19 21:10:10.000000 Signal8-4.1/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.982206 Signal8-4.1/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.1/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.1/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1070 2023-06-20 21:36:24.000000 Signal8-4.1/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.1/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11955 2023-06-21 21:40:30.000000 Signal8-4.1/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.1/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.947203 Signal8-4.1/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4763 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 21:43:47.993205 Signal8-4.1/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-21 21:42:39.000000 Signal8-4.1/setup.py
```

### Comparing `Signal8-4.0/LICENSE` & `Signal8-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.0/PKG-INFO` & `Signal8-4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.0
+Version: 4.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -46,27 +46,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :--------------: | :--------------------------------------------: |
-|  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
+| :---------------: | :--------------------------------------------: |
+| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
+|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
-|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
 |    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
-|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
-|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
+|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
 
-Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
-
-In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
+The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-4.0/README.md` & `Signal8-4.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -34,27 +34,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :--------------: | :--------------------------------------------: |
-|  ``corners``   | ![1686604788813](image/README/1686604788813.png) |
+| :---------------: | :--------------------------------------------: |
+| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
+|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|   ``corners``    | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
-|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
 |    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
-|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
-|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
+|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
 
-Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
-
-In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
+The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-4.0/Signal8/Signal8.py` & `Signal8-4.1/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import numpy as np
 import matplotlib.path as mpath
 
 from functools import partial
 from .utils.scenario import BaseScenario
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.core import Agent, Goal, Obstacle, World
```

### Comparing `Signal8-4.0/Signal8/utils/core.py` & `Signal8-4.1/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.0/Signal8/utils/problems.py` & `Signal8-4.1/Signal8/utils/problems.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Constraints on obstacle positions
 problems = {
-    'corners': [
-        ((1, 1), (1, 0.75), (0.75, 1)),
-        ((1, -1), (1, -0.75), (0.75, -1)),
-        ((-1, -1), (-1, -0.75), (-0.75, -1)),
-        ((-1, 1), (-1, 0.75), (-0.75, 1)),
+    'left': [
+        ((-1, 0), (-1, 1))
         ],
+    'right': [
+        ((0, 1), (-1, 1))
+        ],
+    'circle':  [
+        ((0, 0), (0.5)),
+        ],
+    'balbis': [
+        
+    ],
+    'einstein_tile': [
+        
+    ],
     'quarters': [
         ((-1, -0.375), (-0.375, 0.375)),
         ((-0.375, 0.375), (0.375, 1)),
         ((0.375, 1), (-0.375, 0.375)),
         ((-0.375, 0.375), (-1, -0.375)),
         ],
     'cross': [
         ((-0.1875, 0.1875), (0, 0.7)),
         ((-0.1875, 0.1875), (-0.7, 0)),
         ((-0.7, 0), (-0.1875, 0.1875)),
         ((0, 0.7), (-0.1875, 0.1875)),
         ],
-    'circle':  [
-        ((0, 0), (0.5)),
-        ],
-    'left': [
-        ((-1, 0), (-1, 1))
-        ],
-    'right': [
-        ((0, 1), (-1, 1))
-        ],
-    'up': [
-        ((-1, 1), (0, 1))
-        ],
-    'down': [
-        ((-1, 1), (-1, 0))
+    'corners': [
+        ((1, 1), (1, 0.75), (0.75, 1)),
+        ((1, -1), (1, -0.75), (0.75, -1)),
+        ((-1, -1), (-1, -0.75), (-0.75, -1)),
+        ((-1, 1), (-1, 0.75), (-0.75, 1)),
         ],
     }
 
 def get_problem_list():
     return list(problems.keys())
 
 def get_problem_instance(instance_name):
```

### Comparing `Signal8-4.0/Signal8/utils/simple_env.py` & `Signal8-4.1/Signal8/utils/simple_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,20 @@
         
         state = np.zeros(self.state_space.shape)
         
         for i, agent in enumerate(self.world.agents):
             state[2*i : 2*i+2] = agent.state.p_pos
 
         start_idx = 2 * len(self.world.agents)
-        for i, obstacle in enumerate(self.world.large_obstacles):
-            state[start_idx + 2*i : start_idx + 2*i+2] = obstacle.state.p_pos
-        
-        start_idx = 2 * len(self.world.agents) + 2 * len(self.world.large_obstacles)
         for i, agent in enumerate(self.world.agents):
             state[start_idx + 2*i : start_idx + 2*i+2] = agent.goal.state.p_pos
+        
+        start_idx = 4 * len(self.world.agents)
+        for i, obstacle in enumerate(self.world.large_obstacles):
+            state[start_idx + 2*i : start_idx + 2*i+2] = obstacle.state.p_pos
              
         return np.concatenate(state, axis=None)
 
     def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
```

### Comparing `Signal8-4.0/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.1/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.0/Signal8.egg-info/PKG-INFO` & `Signal8-4.1/Signal8.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.0
+Version: 4.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -46,27 +46,25 @@
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
-| :--------------: | :--------------------------------------------: |
-|  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
+| :---------------: | :--------------------------------------------: |
+| ``einstein tile`` | ![1687297311148](image/README/1687297311148.png) |
+|    ``balbis``    | ![1687297455666](image/README/1687297455666.png) |
+|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
-|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
 |    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
-|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
-|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
-|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
+|     ``right``     | ![1686604851758](image/README/1686604851758.png) |
 
-Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
-
-In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
+The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-4.0/setup.py` & `Signal8-4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.0",
+    version="4.1",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

