# Comparing `tmp/preprocessing_helper-1.2.6.tar.gz` & `tmp/preprocessing_helper-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocessing_helper-1.2.6.tar", last modified: Mon Oct 31 14:18:36 2022, max compression
+gzip compressed data, was "preprocessing_helper-1.2.7.tar", last modified: Wed Jun 21 10:03:23 2023, max compression
```

## Comparing `preprocessing_helper-1.2.6.tar` & `preprocessing_helper-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:18:36.882186 preprocessing_helper-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-31 14:18:36.882186 preprocessing_helper-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-10-31 14:18:36.882186 preprocessing_helper-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:18:36.878186 preprocessing_helper-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:18:36.882186 preprocessing_helper-1.2.6/src/preprocessing_helper/
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/src/preprocessing_helper/FileNameGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/src/preprocessing_helper/RawDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/src/preprocessing_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/src/preprocessing_helper/db_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6167 2022-10-31 14:18:26.000000 preprocessing_helper-1.2.6/src/preprocessing_helper/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:18:36.882186 preprocessing_helper-1.2.6/src/preprocessing_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-31 14:18:36.000000 preprocessing_helper-1.2.6/src/preprocessing_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-31 14:18:36.000000 preprocessing_helper-1.2.6/src/preprocessing_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 14:18:36.000000 preprocessing_helper-1.2.6/src/preprocessing_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-31 14:18:36.000000 preprocessing_helper-1.2.6/src/preprocessing_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:23.235309 preprocessing_helper-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-21 10:03:23.239309 preprocessing_helper-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-21 10:03:23.239309 preprocessing_helper-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:23.235309 preprocessing_helper-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:23.235309 preprocessing_helper-1.2.7/src/preprocessing_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/src/preprocessing_helper/FileNameGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/src/preprocessing_helper/RawDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/src/preprocessing_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/src/preprocessing_helper/db_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-21 10:03:14.000000 preprocessing_helper-1.2.7/src/preprocessing_helper/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:23.235309 preprocessing_helper-1.2.7/src/preprocessing_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-21 10:03:23.000000 preprocessing_helper-1.2.7/src/preprocessing_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-21 10:03:23.000000 preprocessing_helper-1.2.7/src/preprocessing_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:23.000000 preprocessing_helper-1.2.7/src/preprocessing_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 10:03:23.000000 preprocessing_helper-1.2.7/src/preprocessing_helper.egg-info/top_level.txt
```

### Comparing `preprocessing_helper-1.2.6/setup.py` & `preprocessing_helper-1.2.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name='preprocessing_helper',
-    version='1.2.6',
+    version='1.2.7',
     description="",
     long_description=README,
     packages=setuptools.find_packages(where="src"),
     author="Joshua Spear",
     author_email="josh.spear9@gmail.com",
     long_description_content_type="text/markdown",
     url="",
```

### Comparing `preprocessing_helper-1.2.6/src/preprocessing_helper/FileNameGenerator.py` & `preprocessing_helper-1.2.7/src/preprocessing_helper/FileNameGenerator.py`

 * *Files identical despite different names*

### Comparing `preprocessing_helper-1.2.6/src/preprocessing_helper/RawDataLoader.py` & `preprocessing_helper-1.2.7/src/preprocessing_helper/RawDataLoader.py`

 * *Files identical despite different names*

### Comparing `preprocessing_helper-1.2.6/src/preprocessing_helper/db_misc.py` & `preprocessing_helper-1.2.7/src/preprocessing_helper/db_misc.py`

 * *Files identical despite different names*

### Comparing `preprocessing_helper-1.2.6/src/preprocessing_helper/misc.py` & `preprocessing_helper-1.2.7/src/preprocessing_helper/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -156,8 +156,39 @@
 
     Returns:
         List[str]: List of column names containing one of the substrings found
         in the list sub_str_lst
     """
     sub_str_regex = "|".join(sub_str_lst)
     slct_cols = list(df.columns[df.columns.str.contains(sub_str_regex)])
-    return slct_cols
+    return slct_cols
+
+def pd_slct_sub_df(super_cols:pd.DataFrame, sub_cols:pd.DataFrame
+                   ) -> pd.Series:
+    """Function to provide indicies of "super_cols" which match the inidicies 
+    of "sub_cols". The output can then be used to subset super_cols over 
+    multiple columns
+
+    Args:
+        super_cols (pd.DataFrame): Dataframe to derive indicies from
+        sub_cols (pd.DataFrame): Dataframe to derive truth values based on 
+        inclusion
+
+    Raises:
+        Exception: pd.Series of dimension (len(super_cols),1) where True 
+        indications a non-position dependent match between super_cols and 
+        sub_cols
+
+    Returns:
+        pd.Series[bool]: Exception raised if columns between the two dataframes 
+        don't match
+    """
+    if set(super_cols.columns) != set(sub_cols):
+        raise Exception("Input dataframes must contain equal values")
+    # Order identically
+    sub_cols = sub_cols[super_cols.columns]
+    idx_subset = (
+        (super_cols.astype(str).apply(lambda x: "_".join(x), axis=1)).isin(
+            (sub_cols.astype(str).apply(lambda x: "_".join(x), axis=1))
+        )
+    )
+    return idx_subset
```

