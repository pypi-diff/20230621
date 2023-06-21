# Comparing `tmp/pygrc-0.2.0.tar.gz` & `tmp/pygrc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrc-0.2.0.tar", last modified: Tue Feb  7 06:21:33 2023, max compression
+gzip compressed data, was "pygrc-0.3.0.tar", last modified: Wed Jun 21 08:28:11 2023, max compression
```

## Comparing `pygrc-0.2.0.tar` & `pygrc-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 06:21:33.823305 pygrc-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-07 06:21:26.000000 pygrc-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-07 06:21:26.000000 pygrc-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-02-07 06:21:33.823305 pygrc-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-02-07 06:21:26.000000 pygrc-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 06:21:33.823305 pygrc-0.2.0/pygrc/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-07 06:21:26.000000 pygrc-0.2.0/pygrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-02-07 06:21:26.000000 pygrc-0.2.0/pygrc/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-02-07 06:21:26.000000 pygrc-0.2.0/pygrc/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-07 06:21:26.000000 pygrc-0.2.0/pygrc/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 06:21:33.823305 pygrc-0.2.0/pygrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-02-07 06:21:33.000000 pygrc-0.2.0/pygrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-07 06:21:33.000000 pygrc-0.2.0/pygrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 06:21:33.000000 pygrc-0.2.0/pygrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-07 06:21:33.000000 pygrc-0.2.0/pygrc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-07 06:21:33.000000 pygrc-0.2.0/pygrc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 06:21:33.823305 pygrc-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-07 06:21:26.000000 pygrc-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 06:21:33.823305 pygrc-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-07 06:21:26.000000 pygrc-0.2.0/tests/test_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:28:11.161960 pygrc-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 08:28:01.000000 pygrc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 08:28:01.000000 pygrc-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-21 08:28:11.161960 pygrc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 08:28:01.000000 pygrc-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:28:11.161960 pygrc-0.3.0/pygrc/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 08:28:01.000000 pygrc-0.3.0/pygrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 08:28:01.000000 pygrc-0.3.0/pygrc/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-21 08:28:01.000000 pygrc-0.3.0/pygrc/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-21 08:28:01.000000 pygrc-0.3.0/pygrc/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:28:11.161960 pygrc-0.3.0/pygrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-21 08:28:11.000000 pygrc-0.3.0/pygrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 08:28:11.000000 pygrc-0.3.0/pygrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:28:11.000000 pygrc-0.3.0/pygrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 08:28:11.000000 pygrc-0.3.0/pygrc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 08:28:11.000000 pygrc-0.3.0/pygrc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:28:11.161960 pygrc-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-21 08:28:01.000000 pygrc-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:28:11.161960 pygrc-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 08:28:01.000000 pygrc-0.3.0/tests/test_fit.py
```

### Comparing `pygrc-0.2.0/LICENSE` & `pygrc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrc-0.2.0/pygrc/fit.py` & `pygrc-0.3.0/pygrc/fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Copyright (c) 2023 Aman Desai. All rights reserved.
 """
-import iminuit
-from iminuit import cost
 from iminuit import Minuit
 from iminuit.cost import LeastSquares
 import numpy as np
 import typing as tp
 import matplotlib.pyplot as plt
 
 
 class Fit:
     """
     Class to make fitting easier
     relies on iminuit for fitting
     """
+
     def __init__(
         self,
         data_x: tp.Sequence,
         data_y: tp.Sequence,
         *args: tp.Union[float, tp.Sequence[float]]
     ):
         """
@@ -27,19 +26,19 @@
             data_y (tuple): input data on y axis
             *args (float): Takes initial parameter values
 
 
         """
         self.args = args
         print(type(data_x))
-        if 'numpy' not in str(type(data_x)):
+        if "numpy" not in str(type(data_x)):
             self.data_x = data_x.to_numpy()
         else:
             self.data_x = data_x
-        if 'numpy' not in str(type(data_y)):
+        if "numpy" not in str(type(data_y)):
             self.data_y = data_y.to_numpy()
         else:
             self.data_y = data_y
 
     def fit_lsq(
         self,
         function: tp.Callable,
@@ -74,36 +73,36 @@
             m.fixed = bools
         print(m.limits)
         m.migrad()
         m.hesse()
         m.minos()
         return m
 
-    def get_profile(self,m: Minuit, par: str):
+    def get_profile(self, m: Minuit, par: str):
         """
         function to get profile curve for a given parameter
         Args:
             m: iminuit object
             par (str): name of the parameter
         """
 
         plt.rcParams["figure.dpi"] = 300
         plt.rcParams["savefig.dpi"] = 300
 
         if par not in m.pos2var:
             raise ValueError("Please Enter a valid variable")
         fig, ax = plt.subplots()
         data = m.draw_mnprofile(par, band=True, text=False)
-        ax.plot(data[0],data[1])
+        ax.plot(data[0], data[1])
         ax.set_xlabel(par)
         ax.set_ylabel("Least Square")
         ax.set_title("Log Likelihood for parameter " + par)
         fig.savefig(par + "_profile.pdf")
 
-    def draw_contours(self,m: Minuit, var: tp.Union[str, tp.Sequence[str]]):
+    def draw_contours(self, m: Minuit, var: tp.Union[str, tp.Sequence[str]]):
         """
         function to get profile curve for a given parameter
         Args:
             m: iminuit object
             par (list): name of the parameters. At least 2 required.
         """
```

### Comparing `pygrc-0.2.0/pygrc/plot.py` & `pygrc-0.3.0/pygrc/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Copyright (c) 2023 Aman Desai. All rights reserved.
 """
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sb
 from pygrc.reader import Reader
-import iminuit
 import numpy as np
 from iminuit import Minuit
 import typing as tp
 
+
 class Plot:
     """Class for Generating Matplotlib Plots"""
 
     def __init__(self):
         """ """
         self.units_dict: dict = {
             "Rad": "kpc",
@@ -22,15 +22,17 @@
             "Vgas": "km/s",
             "Vdisk": "km/s",
             "Vbul": "km/s",
             "SBdisk": "L/pc2",
             "SBbul": "L/pc2",
         }
 
-    def plot(self, data: pd.DataFrame, column_x: str, column_y: str):
+    def plot(
+        self, data: pd.DataFrame, column_x: str, column_y: str
+    ):  # , save_name: str =""):
         """
         function to plot data on x axis and y axis.
         Args:
             data  :  pd.DataFrame
             column_x: name of dataframe's column for x axis
             column_y: name of dataframe's column for y axis
 
@@ -67,15 +69,23 @@
             + column_x
             + " "
             + self.units_dict[column_x]
         )
         fig.savefig(column_x + "_" + column_y + ".pdf")
         plt.show()
 
-    def overlap(self, data: pd.DataFrame, column_x: str, column_y: list, y_label: str = ""):
+    def overlap(
+        self,
+        data: pd.DataFrame,
+        column_x: str,
+        column_y: list,
+        x_label: str = "",
+        y_label: str = "",
+        save_name: str = "",
+    ):
         """
         function to plot two differeny y data on the same x axis.
         Args:
             data  :  pd.DataFrame
             column_x (str): name of dataframe's column for x axis
             column_y (list): name of dataframe's column for y axis
             y_label (str): label for the y axis
@@ -97,18 +107,20 @@
                 data[column_x],
                 data[column_y],
                 linestyle="none",
                 marker="o",
                 label=column_y,
             )
             ax.set_xlim(min_x, max_x * 1.1)
-            ax.set_xlabel(column_x + " " + self.units_dict[column_x])
+            # ax.set_xlabel(column_x + " " + self.units_dict[column_x])
+            ax.set_xlabel(x_label)
             ax.set_ylabel(y_label)
+            ax.set_title(save_name)
             plt.legend()
-        fig.savefig(column_x + "_" + "vars" + ".pdf")
+        fig.savefig(column_x + "_" + "vars" + "_" + save_name + ".pdf")
 
     def plot_all(
         self,
         data: pd.DataFrame,
     ):
         """
         function to plot all the possible plots from data.
@@ -154,57 +166,67 @@
                         + column_x
                         + " "
                         + self.units_dict[column_x]
                     )
                     fig.savefig(column_x + "_" + column_y + ".pdf")
                     plt.show()
 
-    def corr_map(data: pd.DataFrame):
+    def corr_map(self, data: pd.DataFrame):
         """
         function to plot correlation map.
         Args:
             data  :  pd.DataFrame
         """
 
         plt.rcParams["figure.dpi"] = 300
         plt.rcParams["savefig.dpi"] = 300
         m_corr = Reader.correlation(data)
         fig, ax = plt.subplots()
         sb.heatmap(m_corr, vmax=0.3, center=0, square=True, linewidths=0.5)
-        fig.savefig('correlation.pdf')
+        fig.savefig("correlation.pdf")
         plt.show()
 
-    def rotation(data: pd.DataFrame):
+    def rotation(self, data: pd.DataFrame):
         """
         function for plotting galaxy rotation curve
         Args:
             data  :  pd.DataFrame
 
         """
 
         plt.rcParams["figure.dpi"] = 300
         plt.rcParams["savefig.dpi"] = 300
         self.plot(data, "Rad", ["Vobs"])
 
-    def plot_grc(self, data: pd.DataFrame, m: Minuit,function: tp.Callable, name: str, title: str, ax):
+    def plot_grc(
+        self,
+        data: pd.DataFrame,
+        m: Minuit,
+        function: tp.Callable,
+        name: str,
+        title: str,
+        ax,
+    ):
         """
         function to plot two differeny y data on the same x axis.
         Args:
             data  (pd.DataFrame) : data
             m : Minuit  Object
             function: the definition of function without parameters values
             label: string name of the galaxy
         """
         plt.rcParams["figure.dpi"] = 300
         plt.rcParams["savefig.dpi"] = 300
         handles, labels = plt.gca().get_legend_handles_labels()
 
-        x = np.linspace(data['Rad'].min(),data['Rad'].max(),200)
+        x = np.linspace(data["Rad"].min(), data["Rad"].max(), 200)
 
-        if 'Data' not in labels:
-            ax.plot(data['Rad'],data['Vobs'],marker='o',linestyle='none',label='Data')
-        ax.plot(x, function(x,*m.values),linestyle='--',label=name)
+        if "Data" not in labels:
+            ax.plot(
+                data["Rad"], data["Vobs"], marker="o", linestyle="none", label="Data"
+            )
+        ax.plot(x, function(x, *m.values), linestyle="--", label=name)
         plt.legend()
-        ax.set_xlabel('Distance (kpc)')
-        ax.set_ylabel('Velocity (Km/s)')
+        ax.set_xlabel("Distance (kpc)")
+        ax.set_ylabel("Velocity (Km/s)")
         ax.set_title(title)
-        #plt.savefig(label+'rot.pdf')
+        plt.savefig(title + "rot_fit.pdf")
```

### Comparing `pygrc-0.2.0/pygrc/reader.py` & `pygrc-0.3.0/pygrc/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import os
 import pandas as pd
 import numpy as np
 import pathlib
 
 
 class Reader:
-    """Reader Class
-    """
+    """Reader Class"""
 
     def read(
         filepath: os.PathLike,
         columns: list = [
             "Rad",
             "Vobs",
             "errV",
```

### Comparing `pygrc-0.2.0/setup.py` & `pygrc-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md','r') as file:
     long_description = file.read()
 
 setuptools.setup(
 name="pygrc",
-version="0.2.0",
+version="0.3.0",
 description= "A package to read SPARC data for Galactic Rotation Curves",
 author="Aman Desai",
 author_email="amanmukeshdesai@gmail.com",
 maintainer="Aman Desai",
 maintainer_email="amanmukeshdesai@gmail.com",
 url = "https://github.com/amanmdesai/pygrc",
 long_description=long_description,
```

### Comparing `pygrc-0.2.0/tests/test_fit.py` & `pygrc-0.3.0/tests/test_fit.py`

 * *Files identical despite different names*

