# Comparing `tmp/flatland-railway-extension-0.2.6.tar.gz` & `tmp/flatland-railway-extension-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flatland-railway-extension-0.2.6.tar", last modified: Tue Jun 20 20:26:46 2023, max compression
+gzip compressed data, was "dist\flatland-railway-extension-0.2.7.tar", last modified: Wed Jun 21 05:11:06 2023, max compression
```

## Comparing `flatland-railway-extension-0.2.6.tar` & `flatland-railway-extension-0.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/
--rw-rw-rw-   0        0        0     1214 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      405 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    14346 2023-05-09 20:30:03.000000 flatland-railway-extension-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/
--rw-rw-rw-   0        0        0     3133 2023-06-01 07:54:21.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/FlatlandEnvironmentHelper.py
--rw-rw-rw-   0        0        0    18867 2023-06-20 20:24:51.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/FlatlandGraphBuilder.py
--rw-rw-rw-   0        0        0     7805 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/RailroadSwitchAnalyser.py
--rw-rw-rw-   0        0        0     9991 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/RailroadSwitchCluster.py
--rw-rw-rw-   0        0        0       25 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/
--rw-rw-rw-   0        0        0    21375 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/DynamicAgent.py
--rw-rw-rw-   0        0        0      686 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/DynamicsResourceData.py
--rw-rw-rw-   0        0        0    10121 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandDynamics.py
--rw-rw-rw-   0        0        0     4829 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
--rw-rw-rw-   0        0        0     8950 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandResourceAllocator.py
--rw-rw-rw-   0        0        0     1682 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/InfrastructureData.py
--rw-rw-rw-   0        0        0     1511 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
--rw-rw-rw-   0        0        0     8028 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
--rw-rw-rw-   0        0        0     5009 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/RollingStock.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/data_exports/
--rw-rw-rw-   0        0        0     6857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/data_exports/__init__.py
--rw-rw-rw-   0        0        0     7031 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_dynamics.py
--rw-rw-rw-   0        0        0     4913 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_extensions.py
--rw-rw-rw-   0        0        0     3981 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_graph.py
--rw-rw-rw-   0        0        0     2857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
--rw-rw-rw-   0        0        0     6927 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/
--rw-rw-rw-   0        0        0     5982 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
--rw-rw-rw-   0        0        0     6048 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/FlatlandRenderer.py
--rw-rw-rw-   0        0        0     2200 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/__init__.py
--rw-rw-rw-   0        0        0      248 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.6/flatland_railway_extension/utils/cached_methods.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/
--rw-rw-rw-   0        0        0      405 2023-06-20 20:26:45.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1952 2023-06-20 20:26:45.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:26:45.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-20 20:26:45.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-20 20:26:45.000000 flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 20:26:46.000000 flatland-railway-extension-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-06-20 20:25:52.000000 flatland-railway-extension-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/
+-rw-rw-rw-   0        0        0     1214 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    14346 2023-05-09 20:30:03.000000 flatland-railway-extension-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/
+-rw-rw-rw-   0        0        0     3133 2023-06-01 07:54:21.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/FlatlandEnvironmentHelper.py
+-rw-rw-rw-   0        0        0    18554 2023-06-21 05:08:13.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/FlatlandGraphBuilder.py
+-rw-rw-rw-   0        0        0     7805 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/RailroadSwitchAnalyser.py
+-rw-rw-rw-   0        0        0     9991 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/RailroadSwitchCluster.py
+-rw-rw-rw-   0        0        0       25 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/
+-rw-rw-rw-   0        0        0    21375 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/DynamicAgent.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/DynamicsResourceData.py
+-rw-rw-rw-   0        0        0    10121 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandDynamics.py
+-rw-rw-rw-   0        0        0     4829 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
+-rw-rw-rw-   0        0        0     8950 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandResourceAllocator.py
+-rw-rw-rw-   0        0        0     1682 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/InfrastructureData.py
+-rw-rw-rw-   0        0        0     1511 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
+-rw-rw-rw-   0        0        0     8028 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
+-rw-rw-rw-   0        0        0     5009 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/RollingStock.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/data_exports/
+-rw-rw-rw-   0        0        0     6857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/data_exports/__init__.py
+-rw-rw-rw-   0        0        0     7031 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_dynamics.py
+-rw-rw-rw-   0        0        0     4913 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_extensions.py
+-rw-rw-rw-   0        0        0     3981 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_graph.py
+-rw-rw-rw-   0        0        0     2857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
+-rw-rw-rw-   0        0        0     6927 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/
+-rw-rw-rw-   0        0        0     5982 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
+-rw-rw-rw-   0        0        0     6048 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/FlatlandRenderer.py
+-rw-rw-rw-   0        0        0     2200 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.7/flatland_railway_extension/utils/cached_methods.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-06-21 05:11:05.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:11:05.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-21 05:11:05.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-21 05:11:05.000000 flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:11:06.000000 flatland-railway-extension-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-06-21 05:09:47.000000 flatland-railway-extension-0.2.7/setup.py
```

### Comparing `flatland-railway-extension-0.2.6/LICENSE` & `flatland-railway-extension-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/README.md` & `flatland-railway-extension-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/FlatlandEnvironmentHelper.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/FlatlandEnvironmentHelper.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/FlatlandGraphBuilder.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/FlatlandGraphBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,16 @@
                     possible_transitions = env.rail.get_transitions(*from_position, from_direction)
                     nbr_possible_transitions = fast_count_nonzero(possible_transitions)
                     if nbr_possible_transitions > 0:
                         actions = {}
                         for to_direction in range(4):
                             actions.update({to_direction: RailEnvActions.MOVE_FORWARD})
                         if nbr_possible_transitions == 1:
-                            for to_direction in [(from_direction + i) % 4 for i in range(-1, 2)]:
-                                if possible_transitions[to_direction]:
-                                    if to_direction < from_direction:
-                                        actions.update({to_direction: RailEnvActions.MOVE_LEFT})
-                                    if to_direction > from_direction:
-                                        actions.update({to_direction: RailEnvActions.MOVE_RIGHT})
+                            actions.update({(from_direction - 1) % 4: RailEnvActions.MOVE_LEFT})
+                            actions.update({(from_direction + 1) % 4: RailEnvActions.MOVE_RIGHT})
 
                         for to_direction in range(4):
                             if possible_transitions[to_direction] == 1:
                                 new_position = get_new_position(from_position, to_direction)
                                 from_vertex_name = '{}_{}_{}'.format(from_position[0], from_position[1], from_direction)
                                 to_vertex_name = '{}_{}_{}'.format(new_position[0], new_position[1], to_direction)
                                 graph.add_edge(from_vertex_name,
```

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/RailroadSwitchAnalyser.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/RailroadSwitchAnalyser.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/RailroadSwitchCluster.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/RailroadSwitchCluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/DynamicAgent.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/DynamicAgent.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/DynamicsResourceData.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/DynamicsResourceData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandDynamics.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandDynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/FlatlandResourceAllocator.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/FlatlandResourceAllocator.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/InfrastructureData.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/InfrastructureData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/environments/RollingStock.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/environments/RollingStock.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_dynamics.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_dynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_extensions.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_extensions.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_graph.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_graph.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/examples/demo_simple_flatland_navigation.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/examples/demo_simple_flatland_navigation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/utils/FlatlandRenderer.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/utils/FlatlandRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension/utils/ShortestPathNextStepObservation.py` & `flatland-railway-extension-0.2.7/flatland_railway_extension/utils/ShortestPathNextStepObservation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/flatland_railway_extension.egg-info/SOURCES.txt` & `flatland-railway-extension-0.2.7/flatland_railway_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.6/setup.py` & `flatland-railway-extension-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # twine upload dist/*
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='flatland-railway-extension',
-    version='0.2.6',
+    version='0.2.7',
     author='Adrian Egli',
     author_email="3dhelp@gmail.com",
     description='Extends Flatland Railway Simulator with helpful features.',
     url='https://github.com/aiAdrian/flatland_railway_extension',
     keywords='flatland, railway, extension, dynamics, simulation, multi-agent, reinforcement learning',
     python_requires='>=3.6, <4',
     packages=find_packages('.'),
```

