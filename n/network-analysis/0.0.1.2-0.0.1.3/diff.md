# Comparing `tmp/network-analysis-0.0.1.2.tar.gz` & `tmp/network-analysis-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-analysis-0.0.1.2.tar", last modified: Thu Jun  8 20:43:10 2023, max compression
+gzip compressed data, was "network-analysis-0.0.1.3.tar", last modified: Tue Jun 20 23:43:12 2023, max compression
```

## Comparing `network-analysis-0.0.1.2.tar` & `network-analysis-0.0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/network_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/networkanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/networkanalysis/ergm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/ergm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/ergm/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/src/network_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 23:43:12.000000 network-analysis-0.0.1.3/src/network_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 23:43:12.000000 network-analysis-0.0.1.3/src/network_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:43:12.000000 network-analysis-0.0.1.3/src/network_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 23:43:12.000000 network-analysis-0.0.1.3/src/network_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 23:43:12.000000 network-analysis-0.0.1.3/src/network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/src/networkanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/src/networkanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/src/networkanalysis/ergm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/src/networkanalysis/ergm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/src/networkanalysis/ergm/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/src/networkanalysis/ergm/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/src/networkanalysis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:43:12.341830 network-analysis-0.0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-20 23:43:02.000000 network-analysis-0.0.1.3/tests/test_statistics.py
```

### Comparing `network-analysis-0.0.1.2/LICENCE` & `network-analysis-0.0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `network-analysis-0.0.1.2/PKG-INFO` & `network-analysis-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.1.2/pyproject.toml` & `network-analysis-0.0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "network-analysis"
-version = "0.0.1.2"
+version = "0.0.1.3"
 authors = [
   { name="Gabriel Fortin-Leblanc", email="gabriel.fortin-leblanc@umontreal.ca" },
 ]
 description = "Work in progress..."
 readme = "README.md"
+dependencies = [
+    "scipy == 1.10.1",
+    "networkx == 3.0",
+    "numpy == 1.24.2",
+    "scikit-learn == 1.2.2"
+]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `network-analysis-0.0.1.2/src/network_analysis.egg-info/PKG-INFO` & `network-analysis-0.0.1.3/src/network_analysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.1.2/src/networkanalysis/ergm/simulate.py` & `network-analysis-0.0.1.3/src/networkanalysis/ergm/simulate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 """This module is used to simulate graphs from a exponential random graph
 models.
 """
 import random
 import warnings
+from typing import Dict, List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 
-from ..statistics import CachedStatsComp
+from ..statistics import CachedStatsComp, StatsComp
 
 
 def simulate(
-    ngraphs,
-    param,
-    stats_comp,
-    init,
-    burnin=0,
-    thin=1,
-    summary=False,
-    warn=None,
-    return_cache=False,
-):
+    ngraphs: int,
+    param: np.ndarray,
+    stats_comp: callable,
+    init: Union[nx.Graph, int],
+    burnin: int = 0,
+    thin: int = 1,
+    summary: bool = False,
+    warn: Optional[int] = None,
+    return_statscomp: bool = False,
+) -> Union[
+    List[nx.Graph],
+    Tuple[List[nx.Graph], StatsComp],
+    Tuple[List[nx.Graph], CachedStatsComp],
+    Tuple[List[nx.Graph], Dict, StatsComp],
+    Tuple[List[nx.Graph], Dict, CachedStatsComp],
+]:
     """Simulate ngraphs graphs with respect to the param and the sufficient
     statistics.
 
     :param ngraphs: The number of graphs to simulate.
     :type ngraphs: Integer.
     :param param: The parameter of the model.
     :type param: Numpy array.
     :param stats_comp: The sufficient statistics computer.
     :type stats_comp: A callable object.
     :param init: The initial graph to start the chain, or the number of nodes.
-    :type init: NetworkX graph., optional
+    :type init: NetworkX graph, optional.
     :param burnin: The number of graphs to burn. If none is given, then no
         graphs will be burned., defaults to None
     :type burnin: int, optional
     :param thin: The thinning factor. By default, None is given.
     :type thin: int, optional.
     :param summary: A flag for requesting to collect information about the
         chain such as the acceptance rate. By default, False is given.
     :type summary: Boolean.
     :param warn: If an integer passed, then a warning is thrown if the
         graphs are near-empty or near-complete for this number of interation.
     :type warn: An integer, optional.
+    :param return_statscomp: A flag for requesting to return the sufficient
+        statistics computer. By default, False is given.
+    :type return_statscomp: Boolean.
+    :return: The simulated graphs and the sufficient statistics computer if
+        requested. It also returns the summary if requested.
+    :rtype: A list of NetworkX graphs, and optionally a dictionary and a
+        callable object.
     """
-    stats_comp = CachedStatsComp(stats_comp)
 
     if type(init) is int:
         peek = nx.random_graphs.binomial_graph(init, 0.5)
     else:
         peek = init.copy()
     peek_stats = stats_comp(peek)
     nodes = list(peek.nodes())
@@ -103,12 +116,12 @@
 
         graphs[i] = peek.copy()
 
     # Return phase
     return_objects = [graphs[burnin::thin]]
     if summary:
         return_objects.append({"rate": naccepted / nits})
-    if return_cache:
+    if return_statscomp:
         return_objects.append(stats_comp)
     return (
         tuple(return_objects) if len(return_objects) > 1 else return_objects[0]
     )
```

### Comparing `network-analysis-0.0.1.2/src/networkanalysis/statistics.py` & `network-analysis-0.0.1.3/src/networkanalysis/statistics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 """This module contains classes and functions to compute statistics on
 networks.
 """
-import copy
+from __future__ import annotations
+
 from collections import OrderedDict
-from typing import Any
+from typing import Callable, List, Union
 
 import networkx as nx
 import numpy as np
 from scipy.special import comb
 
+__all__ = [
+    "NEdges",
+    "GWD",
+    "GWESP",
+    "KStars",
+    "InKStars",
+    "OutKStars",
+    "Mutuals",
+    "gwd",
+    "gwesp",
+    "kstars",
+    "in_kstars",
+    "out_kstars",
+    "mutuals",
+    "stats_transform",
+    "StatsComp",
+    "CachedStatsComp",
+]
+
 
-def gwd(graph, decay):
+def gwd(graph: nx.Graph, decay: float) -> float:
     """Compute the geometrically weighted degree of the simple graph.
 
     :param graph: The graph.
     :type graph: NetworkX simple graph.
     :param decay: The decay parameter.
     :type decay: Positive float.
     :return: The geometrically weighted degree.
@@ -22,15 +42,15 @@
     """
     degrees = np.array([d for _, d in graph.degree()])
     uniques, counts = np.unique(degrees, return_counts=True)
     weighted_degrees = (1 - (1 - np.exp(-decay)) ** uniques) * counts
     return np.exp(decay) * weighted_degrees.sum()
 
 
-def gwesp(graph, decay):
+def gwesp(graph: nx.Graph, decay: float) -> float:
     """Compute the geometrically weighted edgewise shared partners of the
     graph.
 
     :param graph: The graph.
     :type graph: NetworkX simple graph.
     :param decay: The decay parameter.
     :type decay: Positive float.
@@ -45,59 +65,59 @@
     )
     weighted_ew_shared_partners = (
         1 - (1 - np.exp(-decay)) ** uniques
     ) * counts
     return np.exp(decay) * weighted_ew_shared_partners.sum()
 
 
-def kstars(graph, k):
+def kstars(graph: nx.Graph, k: int) -> int:
     """Count the number of k-stars of the undirected graph.
 
     :param graph: The graph.
     :type graph: NetworkX undirected graph.
     :param k: The number of branch of a star.
     :type k: Integer strictly greater than 0.
     :return: The number of k-stars the graph contains.
     :rtype: Integer.
     """
     degrees = np.array([d for _, d in graph.degree()])
     return comb(degrees, k).sum()
 
 
-def in_kstars(graph, k):
+def in_kstars(graph: nx.DiGraph, k: int) -> int:
     """Count the number of in k-stars of the directed graph. An in k-star in
     composed of arcs pointing towards its center.
 
     :param graph: The graph.
     :type graph: NetworkX directed graph.
     :param k: The number of branch of a star.
     :type k: Integer strictly greater than 0.
     :return: The number of in k-stars the graph contains.
     :rtype: Integer.
     """
     degrees = np.array([d for _, d in graph.in_degree()])
     return comb(degrees, k).sum()
 
 
-def out_kstars(graph, k):
+def out_kstars(graph: nx.DiGraph, k: int) -> int:
     """Count the number of out k-stars of the directed graph. An out k-star in
     composed of arcs pointing towards its border.
 
     :param graph: The graph.
     :type graph: NetworkX directed graph.
     :param k: The number of branch of a star.
     :type k: Integer strictly greater than 0.
     :return: The number of out k-stars the graph contains.
     :rtype: Integer.
     """
     degrees = np.array([d for _, d in graph.out_degree()])
     return comb(degrees, k).sum()
 
 
-def mutuals(graph):
+def mutuals(graph: Union[nx.Graph, nx.DiGraph]) -> int:
     """Count the number of pairs of nodes in the graph that has a mutual
     connection. In a undirected multigraph, two nodes have a mutual connection
     if there are at least two edges between them. In a directed graph, two arcs
     between two nodes must be of opposite direction for having a mutual
     connection.
 
     :param graph: The graph.
@@ -112,122 +132,150 @@
         count_edges /= 2
     return (count_edges > 1).sum()
 
 
 class NEdges:
     """Dummy callable object that mimics number_of_edges of NetworkX."""
 
-    def __call__(self, graph):
+    def __call__(self, graph: Union[nx.Graph, nx.DiGraph]) -> int:
         return graph.number_of_edges()
 
 
 class GWD:
     """Dummy callable object that mimics gwd."""
 
-    def __init__(self, decay):
+    def __init__(self, decay: float):
         self._decay = decay
 
-    def __call__(self, graph):
+    def __call__(self, graph: nx.Graph):
         return gwd(graph, self._decay)
 
 
 class GWESP:
     """Dummy callable object that mimics gwesp."""
 
-    def __init__(self, decay):
+    def __init__(self, decay: float):
         self._decay = decay
 
-    def __call__(self, graph):
+    def __call__(self, graph: nx.Graph):
         return gwesp(graph, self._decay)
 
 
 class KStars:
     """Dummy callable object that mimics kstars."""
 
-    def __init__(self, k):
+    def __init__(self, k: int):
         self._k = k
 
-    def __call__(self, graph):
+    def __call__(self, graph: nx.Graph):
         return kstars(graph, self._k)
 
 
 class InKStars:
     """Dummy callable object that mimics in_kstars."""
 
-    def __init__(self, k):
+    def __init__(self, k: int):
         self._k = k
 
-    def __call__(self, graph):
+    def __call__(self, graph: nx.DiGraph):
         return in_kstars(graph, self._k)
 
 
 class OutKStars:
     """Dummy callable object that mimics out_kstars."""
 
-    def __init__(self, k):
+    def __init__(self, k: int):
         self._k = k
 
-    def __call__(self, graph):
+    def __call__(self, graph: nx.DiGraph):
         return out_kstars(graph, self._k)
 
 
 class Mutuals:
     """Dummy callable object that mimics mutuals."""
 
-    def __call__(self, graph):
+    def __call__(self, graph: Union[nx.Graph, nx.DiGraph]):
         return mutuals(graph)
 
 
-def stats_transform(stats):
+def stats_transform(stats: List[Callable]) -> Callable:
     """Transform the list of statistics into one function that computes the
     vector of statistics from the list.
 
     :param stats: List of callable object that takes a NetworkX graph as
         argument.
     :type stats: List.
     """
 
+    # Build the function that computes the vector of statistics from the list.
     def stats_comp(graph):
         graph_stats = np.empty(
             (len(stats)),
         )
         for i, stat in enumerate(stats):
             graph_stats[i] = stat(graph)
         return graph_stats
 
     return stats_comp
 
 
 class StatsComp:
-    def __init__(self, stats):
+    """Callable object that computes a vector of statistics from a graph.
+    StatsComp can be understand as "Statistics Computer".
+    """
+
+    def __init__(self, stats: Union[List[Callable], StatsComp]):
+        """Initialize the StatsComp object.
+
+        :param stats: List of callable object that takes a NetworkX graph as
+            argument. It also accepts another StatsComp object and copy it.
+        :type stats: List of callable object or StatsComp object.
+        """
         if isinstance(stats, StatsComp):
             self._func = stats._func
             self._len = stats._len
         else:
             self._func = stats_transform(stats)
             self._len = len(stats)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self._len
 
-    def __call__(self, graph):
+    def __call__(self, graph) -> np.ndarray:
         return self._func(graph)
 
 
 class CachedStatsComp(StatsComp):
-    def __init__(self, stats, max_size=10000):
+    """StatsComp that caches the computed statistics."""
+
+    def __init__(
+        self,
+        stats: Union[List[Callable], StatsComp, CachedStatsComp],
+        max_size: int = 10000,
+    ):
+        """Initialize the CachedStatsComp object.
+
+        :param stats: List of callable object that takes a NetworkX graph as
+            argument. It also accepts another StatsComp object or even a
+            CachedStatsComp object and copy it.
+        :type stats: List of callable object, StatsComp object or
+            CachedStatsComp object.
+        :param max_size: Maximum number of graphs to cache.
+        :type max_size: Integer.
+        """
         super().__init__(stats)
 
         self._cache = OrderedDict()
         if isinstance(stats, CachedStatsComp):
             self._cache.update(stats._cache)
         self._max_size = max_size
 
-    def __call__(self, graph):
-        if graph in self._cache:
-            return self._cache[graph]
+    def __call__(self, graph: nx.Graph) -> np.ndarray:
+        h = nx.weisfeiler_lehman_graph_hash(graph)
+        if h in self._cache:
+            return self._cache[h]
 
         if len(self._cache) >= self._max_size:
             self._cache.popitem()
         stats = self._func(graph)
         self._cache[graph] = stats
         return stats
```

