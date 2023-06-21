# Comparing `tmp/raphtory-0.4.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/raphtory-0.4.1-cp310-cp310-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6275234 bytes, number of entries: 7
--rw-r--r--  4.6 unx     9622 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/METADATA
--rw-r--r--  4.6 unx      134 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      522 b- defN 23-Jun-07 19:27 raphtory/__init__.py
--rw-r--r--  4.6 unx     7399 b- defN 23-Jun-07 19:27 raphtory/vis.py
--rw-r--r--  4.6 unx     1994 b- defN 23-Jun-07 19:27 raphtory/nullmodels.py
--rwxr-xr-x  4.6 unx 19520856 b- defN 23-Jun-07 19:27 raphtory/raphtory.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      547 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/RECORD
-7 files, 19541074 bytes uncompressed, 6274280 bytes compressed:  67.9%
+Zip file size: 3920249 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9622 b- defN 23-Jun-21 12:19 raphtory-0.4.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      104 b- defN 23-Jun-21 12:19 raphtory-0.4.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     4131 b- defN 23-Jun-21 12:19 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx      522 b- defN 23-Jun-21 12:19 raphtory/__init__.py
+-rw-r--r--  4.6 unx     7399 b- defN 23-Jun-21 12:19 raphtory/vis.py
+-rwxr-xr-x  4.6 unx 11496283 b- defN 23-Jun-21 12:19 raphtory/raphtory.cpython-310-darwin.so
+-rw-r--r--  4.6 unx      537 b- defN 23-Jun-21 12:19 raphtory-0.4.1.dist-info/RECORD
+7 files, 11518598 bytes uncompressed, 3919315 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.4.0.dist-info/METADATA
+Filename: raphtory-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.4.0.dist-info/WHEEL
+Filename: raphtory-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: raphtory/__init__.py
+Filename: raphtory/nullmodels.py
 Comment: 
 
-Filename: raphtory/vis.py
+Filename: raphtory/__init__.py
 Comment: 
 
-Filename: raphtory/nullmodels.py
+Filename: raphtory/vis.py
 Comment: 
 
-Filename: raphtory/raphtory.pypy39-pp73-x86_64-linux-gnu.so
+Filename: raphtory/raphtory.cpython-310-darwin.so
 Comment: 
 
-Filename: raphtory-0.4.0.dist-info/RECORD
+Filename: raphtory-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raphtory/nullmodels.py

```diff
@@ -1,56 +1,94 @@
 """
-Generate null models for a graph.
+Generate randomised reference models for a temporal graph edgelist
 """
 
 import pandas as pd
 
 def shuffle_column(graph_df:pd.DataFrame, col_number=None, col_name=None, inplace=False):
     """
-    returns a dataframe with a given column shuffled
+    Returns an edgelist with a given column shuffled. Exactly one of col_number or col_name should be specified.
+
+    Args:
+        graph_df (pd.DataFrame): The input DataFrame representing the timestamped edgelist.
+        col_number (int, optional): The column number to shuffle. Default is None.
+        col_name (str, optional): The column name to shuffle. Default is None.
+        inplace (bool, optional): If True, shuffles the column in-place. Otherwise, creates a copy of the DataFrame. Default is False.
+
+    Returns:
+        pd.DataFrame: The shuffled DataFrame with the specified column.
+
+    Raises:
+        AssertionError: If neither col_number nor col_name is provided.
+        AssertionError: If both col_number and col_name are provided.
+
     """
     assert col_number is not None or col_name is not None, f"No column number or name provided."
     assert not (col_name is not None and col_number is not None), f"Cannot have both a column number and a column name."
 
     if inplace:
         df = graph_df
     else:
         df = graph_df.copy()
 
     no_events = len(df)
 
     if col_number is not None:
-        col = df[[col_number]].sample(n=no_events)
+        col = df[df.columns[col_number]].sample(n=no_events)
         col.reset_index(inplace=True,drop=True)
-        df[[col_number]] = col
+        df[df.columns[col_number]] = col
     if col_name is not None:
         col = df[col_name].sample(n=no_events)
         col.reset_index(inplace=True,drop=True)
-    
+        df[col_name]=col
     return df
 
 def shuffle_multiple_columns(graph_df:pd.DataFrame, col_numbers:list=None, col_names:list=None, inplace=False):
     """
-    returns a dataframe with a given columns shuffled.
+    Returns an edgelist with given columns shuffled. Exactly one of col_numbers or col_names should be specified.
+
+    Args:
+        graph_df (pd.DataFrame): The input DataFrame representing the graph.
+        col_numbers (list, optional): The list of column numbers to shuffle. Default is None.
+        col_names (list, optional): The list of column names to shuffle. Default is None.
+        inplace (bool, optional): If True, shuffles the columns in-place. Otherwise, creates a copy of the DataFrame. Default is False.
+
+    Returns:
+        pd.DataFrame: The shuffled DataFrame with the specified columns.
+
+    Raises:
+        AssertionError: If neither col_numbers nor col_names are provided.
+        AssertionError: If both col_numbers and col_names are provided.
+
     """
     assert col_numbers is not None or col_names is not None, f"No column numbers or names provided."
     assert not (col_names is not None and col_numbers is not None), f"Cannot have both column numbers and column names."
 
     if col_numbers is not None:
         for n in col_numbers:
             df = shuffle_column(graph_df, col_number=n, inplace=inplace)
     if col_names is not None:
         for name in col_names:
             df = shuffle_column(graph_df, col_name=name)
-    
     return df
     
 def permuted_timestamps_model(graph_df:pd.DataFrame, time_col:int=None, time_name:str=None, inplace=False, sorted=False):
     """
-    returns a dataframe with the time column shuffled
+    Returns a DataFrame with the time column shuffled.
+
+    Args:
+        graph_df (pd.DataFrame): The input DataFrame representing the graph.
+        time_col (int, optional): The column number of the time column to shuffle. Default is None.
+        time_name (str, optional): The column name of the time column to shuffle. Default is None.
+        inplace (bool, optional): If True, shuffles the time column in-place. Otherwise, creates a copy of the DataFrame. Default is False.
+        sorted (bool, optional): If True, sorts the DataFrame by the shuffled time column. Default is False.
+
+    Returns:
+        pd.DataFrame or None: The shuffled DataFrame with the time column, or None if inplace=True.
+
     """
     shuffled_df = shuffle_column(graph_df, time_col, time_name, inplace)
 
     if sorted:
         shuffled_df.sort_values(by=time_name if time_name else shuffled_df.columns[time_col], inplace=True)
     
     if inplace:
```

## Comparing `raphtory-0.4.0.dist-info/METADATA` & `raphtory-0.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3
 Requires-Dist: pyvis >=0.3.2
 Requires-Dist: networkx >=2.6.3
 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.4.0 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.4.1 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 Requires-Dist:
 networkx >=2.6.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis' Requires-Dist:
 networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib >=3.4.3 ; extra ==
 'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis' Provides-Extra: vis
 Summary: Python package for raphtory, a temporal graph library Keywords:
```

## Comparing `raphtory-0.4.0.dist-info/RECORD` & `raphtory-0.4.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-raphtory-0.4.0.dist-info/METADATA,sha256=uxQyVeZnJbhNZjLPqjaDWaKq82pFekMRm-lUSYPgGLw,9622
-raphtory-0.4.0.dist-info/WHEEL,sha256=hmjWNhwmKrGfL4b8FvVMOP1Hp2Rqx0PvxihnXHTxbNs,134
+raphtory-0.4.1.dist-info/METADATA,sha256=JqC6zK8OVmM1efnUA3jPrr9nlQu8EXbd3YLNUZe7cfs,9622
+raphtory-0.4.1.dist-info/WHEEL,sha256=8TtlGJJst1YFZIGnHrmXaO3gsuQsoC5oG7RuQLiddtI,104
+raphtory/nullmodels.py,sha256=vRbtQ9og5iwoZyommsxpCTq2t9BW6WfrzhUNpYbETjY,4131
 raphtory/__init__.py,sha256=qyIfwQjNBTdjQeZfzlsDga5Zbt_wLJalT67VRlLwLKU,522
 raphtory/vis.py,sha256=CGUptPkNNp4-VFbKSKCNm-w6H-aq7a5VNxrmn6YpTxk,7399
-raphtory/nullmodels.py,sha256=2YS1-uIsaVk1W-dpDzXXXJKrewYrSBA5H-QHe9NiIZY,1994
-raphtory/raphtory.pypy39-pp73-x86_64-linux-gnu.so,sha256=0zUKaSvUXPw7IMesGNQGQseEg5kceJAYrRyMXJnsgMs,19520856
-raphtory-0.4.0.dist-info/RECORD,,
+raphtory/raphtory.cpython-310-darwin.so,sha256=MmluVX0EHCjigY3LSdMW4mKaDFwmVbBO4pK45m6Q0X8,11496283
+raphtory-0.4.1.dist-info/RECORD,,
```

