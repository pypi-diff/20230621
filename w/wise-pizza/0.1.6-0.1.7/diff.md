# Comparing `tmp/wise-pizza-0.1.6.tar.gz` & `tmp/wise-pizza-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.6.tar", last modified: Fri Jun 16 14:51:16 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.7.tar", last modified: Wed Jun 21 19:18:10 2023, max compression
```

## Comparing `wise-pizza-0.1.6.tar` & `wise-pizza-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.029416 wise-pizza-0.1.6/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-16 14:51:16.028910 wise-pizza-0.1.6/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-16 14:51:16.029573 wise-pizza-0.1.6/setup.cfg
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-16 14:50:01.000000 wise-pizza-0.1.6/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.024210 wise-pizza-0.1.6/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-16 14:01:51.000000 wise-pizza-0.1.6/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-16 13:55:29.000000 wise-pizza-0.1.6/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-16 14:51:16.028144 wise-pizza-0.1.6/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-16 14:51:15.000000 wise-pizza-0.1.6/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.260544 wise-pizza-0.1.7/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-21 19:18:10.260021 wise-pizza-0.1.7/PKG-INFO
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/README.md
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-21 19:18:10.260655 wise-pizza-0.1.7/setup.cfg
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-21 19:17:15.000000 wise-pizza-0.1.7/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.255498 wise-pizza-0.1.7/wise_pizza/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/explain.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/find_alpha.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3917 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/make_matrix.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/plotting.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/segment_data.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/slicer.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/solver.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-21 14:24:36.000000 wise-pizza-0.1.7/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-21 19:18:10.259169 wise-pizza-0.1.7/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-21 19:18:09.000000 wise-pizza-0.1.7/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.6/LICENSE` & `wise-pizza-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/PKG-INFO` & `wise-pizza-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.6/README.md` & `wise-pizza-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/setup.py` & `wise-pizza-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.6",
+    version="0.1.7",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.6/wise_pizza/explain.py` & `wise-pizza-0.1.7/wise_pizza/explain.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza/find_alpha.py` & `wise-pizza-0.1.7/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza/make_matrix.py` & `wise-pizza-0.1.7/wise_pizza/make_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,18 @@
     # TODO: do a  nested sparse regression fit to form groups of dim values, pos, neg, null
     # TODO: first calculate the matrix size, scale down max_depth if matrix too big
     if force_dim is None:
         dims = list(dim_df.columns)
     else:
         assert force_dim in dim_df.columns
         dims = [c for c in dim_df.columns if c != force_dim]
+
+    # drop dimensions with only one value, for clarity
+    dims = [d for d in dims  if len(dim_df[d].unique()) > 1]
+
     defs = []
     mats = []
     dims_range_min = min(len(dims), max(1, min_depth))
     dims_range_max = min(len(dims) + 1, max_depth + 1)
     dims_range = range(dims_range_min, dims_range_max)
     for num_dims in tqdm(dims_range) if verbose else dims_range:
         for these_dims in itertools.combinations(dims, num_dims):
```

### Comparing `wise-pizza-0.1.6/wise_pizza/plotting.py` & `wise-pizza-0.1.7/wise_pizza/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from wise_pizza.slicer import SliceFinder
 
 pio.templates.default = "plotly_white"
 
 import numpy as np
 import pandas as pd
-from IPython.display import Image
+from IPython.display import Image, display
 
 
 def plot_split_segments(
     sf_size: SliceFinder,
     sf_avg: SliceFinder,
     plot_is_static: bool = False,
     width: int = 2000,
@@ -287,32 +287,35 @@
         x=data["naive_avg"],
         y=data.index,
         orientation="h",
         name="Diff in averages",
         marker_color="#ff685f",
     )
 
-    fig = make_subplots(
-        rows=2,
-        cols=1,
-        shared_yaxes=False,
-        subplot_titles=["", "Normalised difference in averages"],
-    )
+    fig = go.Figure()
+    fig2 = go.Figure()
 
-    fig.add_trace(trace1, 1, 1)
-    fig.add_trace(trace2, 2, 1)
-    fig["layout"]["yaxis2"].update(autorange="reversed")
+    fig.add_trace(trace1)
+    fig.update_layout(title="Segments contributing most to the change")
+    fig2.add_trace(trace2)
+    fig2["layout"]["yaxis"].update(autorange="reversed")
+    fig2.update_layout(title="Normalised difference in average")
+
+    fig2.update_layout(width=width, height=height)
 
     fig.update_layout(
         title="Segments contributing most to the change",
         #         showlegend = True,
         **waterfall_layout_args(sf, width, height)
     )
 
     if plot_is_static:
         # Convert the figure to a static image
         image_bytes = to_image(fig, format="png", scale=2)
+        image_bytes2 = to_image(fig2, format="png", scale=2)
 
         # Display the static image in the Jupyter notebook
-        return Image(image_bytes, width=width, height=height)
+        display(Image(image_bytes, width=width, height=height))
+        display(Image(image_bytes2, width=width, height=height))
     else:
         fig.show()
+        fig2.show()
```

### Comparing `wise-pizza-0.1.6/wise_pizza/segment_data.py` & `wise-pizza-0.1.7/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza/slicer.py` & `wise-pizza-0.1.7/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza/solver.py` & `wise-pizza-0.1.7/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza/utils.py` & `wise-pizza-0.1.7/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.6/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.7/wise_pizza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

