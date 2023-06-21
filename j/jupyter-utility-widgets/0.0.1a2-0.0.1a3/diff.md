# Comparing `tmp/jupyter-utility-widgets-0.0.1a2.tar.gz` & `tmp/jupyter-utility-widgets-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.1a2.tar", last modified: Tue Jun 20 17:05:29 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.1a3.tar", last modified: Wed Jun 21 05:40:00 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.1a2.tar` & `jupyter-utility-widgets-0.0.1a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/file_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/filter_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/specgram.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/specgram_examiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/numpy_parameter_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.977386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/file_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/filter_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/specgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/specgram_examiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/utility/numpy_parameter_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:40:00.977386 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 05:40:00.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-21 05:40:00.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:40:00.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 05:40:00.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 05:40:00.000000 jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 05:39:42.000000 jupyter-utility-widgets-0.0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 05:40:00.981386 jupyter-utility-widgets-0.0.1a3/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.1a2/LICENSE` & `jupyter-utility-widgets-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/PKG-INFO` & `jupyter-utility-widgets-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a2
+Version: 0.0.1a3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a2/README.md` & `jupyter-utility-widgets-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/file_explorer.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/file_explorer.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/filter_design.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/filter_design.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/base.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,17 @@
             self.axes = [axes]
         else:
             self.axes = list(axes.reshape(-1,))
         children = [self.fig.canvas]
 
         super().__init__(children, **kwargs)
 
+
     def update(self, data=None):
-        self.fig.canvas.draw()
+        self.fig.canvas.draw_idle()
         self.fig.canvas.flush_events()
     
     @abstractmethod
     def select(self, x=None, y=None, z=None):
         raise NotImplementedError()
```

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/lines.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/lines.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/specgram.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/figures/specgram.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/filter.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/filter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/specgram_examiner.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/plot/specgram_examiner.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/numpy_parameter_converter.py` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets/utility/numpy_parameter_converter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a2
+Version: 0.0.1a3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/SOURCES.txt` & `jupyter-utility-widgets-0.0.1a3/jupyter_utility_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

