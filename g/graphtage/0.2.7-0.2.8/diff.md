# Comparing `tmp/graphtage-0.2.7.tar.gz` & `tmp/graphtage-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphtage-0.2.7.tar", last modified: Mon Jan  9 16:37:47 2023, max compression
+gzip compressed data, was "graphtage-0.2.8.tar", last modified: Wed Jun 21 19:35:23 2023, max compression
```

## Comparing `graphtage-0.2.7.tar` & `graphtage-0.2.8.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:37:47.151258 graphtage-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-09 16:37:38.000000 graphtage-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-09 16:37:38.000000 graphtage-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-01-09 16:37:47.151258 graphtage-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-01-09 16:37:38.000000 graphtage-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:37:47.151258 graphtage-0.2.7/graphtage/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/fibonacci.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37738 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/graphtage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)    28141 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/multiset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/pydiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    24295 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-01-09 16:37:38.000000 graphtage-0.2.7/graphtage/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:37:47.151258 graphtage-0.2.7/graphtage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-09 16:37:47.000000 graphtage-0.2.7/graphtage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 16:37:47.151258 graphtage-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-01-09 16:37:38.000000 graphtage-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:37:47.151258 graphtage-0.2.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_fibonacci.py
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_graphtage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_pydiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-09 16:37:38.000000 graphtage-0.2.7/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:35:23.465860 graphtage-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-21 19:35:15.000000 graphtage-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 19:35:15.000000 graphtage-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-21 19:35:23.465860 graphtage-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-21 19:35:15.000000 graphtage-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:35:23.461860 graphtage-0.2.8/graphtage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/fibonacci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37826 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/graphtage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28141 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/multiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/pydiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24295 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-21 19:35:15.000000 graphtage-0.2.8/graphtage/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:35:23.461860 graphtage-0.2.8/graphtage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 19:35:23.000000 graphtage-0.2.8/graphtage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:35:23.465860 graphtage-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 19:35:15.000000 graphtage-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:35:23.465860 graphtage-0.2.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_fibonacci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_graphtage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_pydiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-21 19:35:15.000000 graphtage-0.2.8/test/test_xml.py
```

### Comparing `graphtage-0.2.7/LICENSE` & `graphtage-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/PKG-INFO` & `graphtage-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphtage
-Version: 0.2.7
+Version: 0.2.8
 Summary: A utility to diff tree-like files such as JSON and XML.
 Home-page: https://github.com/trailofbits/graphtage
 Author: Trail of Bits
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://trailofbits.github.io/graphtage
 Project-URL: Source, https://github.com/trailofbits/graphtage
 Project-URL: Tracker, https://github.com/trailofbits/graphtage/issues
```

### Comparing `graphtage-0.2.7/README.md` & `graphtage-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/__init__.py` & `graphtage-0.2.8/graphtage/__init__.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/__main__.py` & `graphtage-0.2.8/graphtage/__main__.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/bounds.py` & `graphtage-0.2.8/graphtage/bounds.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         if upper_bound < lower_bound:
             raise ValueError(f"Upper bound ({upper_bound!s}) must be less than lower bound ({lower_bound!s})")
         self.lower_bound: RangeValue = lower_bound
         """The lower bound of this range."""
         self.upper_bound: RangeValue = upper_bound
         """The upper bound of this range."""
 
+    def __contains__(self, subrange: "Range") -> bool:
+        return subrange.lower_bound >= self.lower_bound and subrange.upper_bound <= self.upper_bound
+
     def __eq__(self, other):
         return self.lower_bound == other.lower_bound and self.upper_bound == other.upper_bound
 
     def __lt__(self, other):
         return self.upper_bound < other.upper_bound or \
             (self.upper_bound == other.upper_bound and self.lower_bound < other.lower_bound)
```

### Comparing `graphtage-0.2.7/graphtage/csv.py` & `graphtage-0.2.8/graphtage/csv.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/edits.py` & `graphtage-0.2.8/graphtage/edits.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/expressions.py` & `graphtage-0.2.8/graphtage/expressions.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/fibonacci.py` & `graphtage-0.2.8/graphtage/fibonacci.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/formatter.py` & `graphtage-0.2.8/graphtage/formatter.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/graphtage.py` & `graphtage-0.2.8/graphtage/graphtage.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,14 +937,15 @@
     """
     def __init__(cls, name, bases, clsdict):
         if len(cls.mro()) > 2:
             # Instantiate a version of the filetype to add it to our global dicts:
             instance = cls()
             assert instance.name in FILETYPES_BY_TYPENAME
             assert instance.default_mimetype in FILETYPES_BY_MIME
+            setattr(cls, "default_instance", instance)
         super().__init__(name, bases, clsdict)
 
 
 class BuildOptions:
     """A class for passing options to tree building functions in :class:`Filetype`"""
 
     def __init__(self, *,
@@ -979,14 +980,15 @@
     """Abstract base class from which all Graphtage file formats should extend.
 
     When this class is subclassed, the subclass will automatically be added to Graphtage's filetype registry.
     This includes automatic inclusion in :mod:`graphtage`'s command line arguments and mime type auto-detection in
     :func:`get_filetype`.
 
     """
+    default_instance: "Filetype"
 
     def __init__(self, type_name: str, default_mimetype: str, *mimetypes: str):
         """Initializes a new Graphtage file format type
 
         Args:
             type_name: A short name for the :class:`Filetype`. This will be used for specifying this :class:`Filetype`
                 via command line arguments.
```

### Comparing `graphtage-0.2.7/graphtage/json.py` & `graphtage-0.2.8/graphtage/json.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/levenshtein.py` & `graphtage-0.2.8/graphtage/levenshtein.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
         self.edit_matrix: List[List[Optional[Edit]]] = [
             [None] * (len(self.from_seq) + 1) for _ in range(len(self.to_seq) + 1)
         ]
         self.path_costs = np.full((len(self.to_seq) + 1, len(self.from_seq) + 1), 0, dtype=np.uint16)
         self.costs = np.full((len(self.to_seq) + 1, len(self.from_seq) + 1), 0, dtype=np.uint64)
         self._fringe_row: int = -1
         self._fringe_col: int = 0
+        self._last_fringe: List[Tuple[int, int]] = []
         super().__init__(
             from_node=from_node,
             to_node=to_node,
             constant_cost=constant_cost,
             cost_upper_bound=cost_upper_bound
         )
         self.__edits: Optional[List[Edit]] = None
@@ -181,14 +182,15 @@
             yield row, col
             row -= 1
             col += 1
 
     def _next_fringe(self) -> bool:
         if self.is_complete():
             return False
+        self._last_fringe = list(self._fringe_diagonal())
         self._fringe_row += 1
         if self._fringe_row >= len(self.to_seq) + 1:
             self._fringe_row = len(self.to_seq)
             self._fringe_col += 1
         for row, col in self._fringe_diagonal():
             self._add_node(row, col)
         if self._fringe_col >= len(self.from_seq):
@@ -316,17 +318,19 @@
                 _ = self.edits()
             cost = int(self.costs[len(self.to_seq)][len(self.from_seq)])
             return Range(cost, cost)
         else:
             if self._fringe_row <= 0:
                 return base_bounds
             return Range(
-                max(base_bounds.lower_bound, min(
+                max(base_bounds.lower_bound, min(min(
                     int(self.costs[row][col]) for row, col in self._fringe_diagonal()
-                )),
+                ), min(
+                    int(self.costs[row][col]) for row, col in self._last_fringe
+                ))),
                 base_bounds.upper_bound
             )
 
     def _cleanup(self):
         if self.bounds().definitive() and self.edit_matrix is not None:
             if self.__edits is None:
                 self.edits()
```

### Comparing `graphtage-0.2.7/graphtage/matching.py` & `graphtage-0.2.8/graphtage/matching.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/multiset.py` & `graphtage-0.2.8/graphtage/multiset.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/plist.py` & `graphtage-0.2.8/graphtage/plist.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/printer.py` & `graphtage-0.2.8/graphtage/printer.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/progress.py` & `graphtage-0.2.8/graphtage/progress.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/pydiff.py` & `graphtage-0.2.8/graphtage/pydiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,18 @@
         elif isinstance(obj, int):
             new_node = IntegerNode(obj)
         elif isinstance(obj, float):
             new_node = FloatNode(obj)
         elif isinstance(obj, str):
             new_node = StringNode(obj)
         elif isinstance(obj, bytes):
-            new_node = StringNode(obj.decode('utf-8'))
+            try:
+                new_node = StringNode(obj.decode('utf-8'))
+            except UnicodeDecodeError:
+                new_node = ListNode(map(IntegerNode, obj))
         elif isinstance(obj, DictValue):
             stack.append((obj, [], [obj.value, obj.key]))
         elif isinstance(obj, PyObjMember):
             stack.append((obj, [], [obj.value]))
         elif isinstance(obj, dict):
             stack.append(({}, [], [DictValue(key=k, value=v) for k, v in reversed(list(obj.items()))]))
         elif isinstance(python_obj, (list, tuple)):
```

### Comparing `graphtage-0.2.7/graphtage/search.py` & `graphtage-0.2.8/graphtage/search.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/sequences.py` & `graphtage-0.2.8/graphtage/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     @repeat_until_tightened
     def tighten_bounds(self) -> bool:
         for edit in self._sub_edits:
             prev_bounds = edit.bounds()
             if edit.tighten_bounds():
                 new_bounds = edit.bounds()
                 if prev_bounds.lower_bound > new_bounds.lower_bound or prev_bounds.upper_bound < new_bounds.upper_bound:
-                    log.warning(f"The most recent call to `tighten_bounds()` on edit {edit} tightened its bounds from {prev_bounds} to {new_bounds}")
+                    log.warning(f"The most recent call to `tighten_bounds()` on edit {edit} tightened its bounds from "
+                                f"{prev_bounds} to {new_bounds}")
                 return True
         return False
 
     def bounds(self) -> Range:
         lb = 0
         ub = 0
         for edit in self.edits():
```

### Comparing `graphtage-0.2.7/graphtage/tree.py` & `graphtage-0.2.8/graphtage/tree.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/utils.py` & `graphtage-0.2.8/graphtage/utils.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/version.py` & `graphtage-0.2.8/graphtage/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 deploying to PyPI.
 
 If :const:`True`, the git branch will be included in the version string.
 
 """
 
 
-__version__: Tuple[Union[int, str], ...] = (0, 2, 7)
+__version__: Tuple[Union[int, str], ...] = (0, 2, 8)
 
 if DEV_BUILD:
     branch_name = git_branch()
     if branch_name is None:
         __version__ = __version__ + ('git',)
     else:
         __version__ = __version__ + ('git', branch_name)
```

### Comparing `graphtage-0.2.7/graphtage/xml.py` & `graphtage-0.2.8/graphtage/xml.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage/yaml.py` & `graphtage-0.2.8/graphtage/yaml.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/graphtage.egg-info/PKG-INFO` & `graphtage-0.2.8/graphtage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphtage
-Version: 0.2.7
+Version: 0.2.8
 Summary: A utility to diff tree-like files such as JSON and XML.
 Home-page: https://github.com/trailofbits/graphtage
 Author: Trail of Bits
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://trailofbits.github.io/graphtage
 Project-URL: Source, https://github.com/trailofbits/graphtage
 Project-URL: Tracker, https://github.com/trailofbits/graphtage/issues
```

### Comparing `graphtage-0.2.7/graphtage.egg-info/SOURCES.txt` & `graphtage-0.2.8/graphtage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 test/test_fibonacci.py
 test/test_formatting.py
 test/test_graphtage.py
 test/test_levenshtein.py
 test/test_matching.py
 test/test_pydiff.py
 test/test_search.py
-test/test_utils.py
+test/test_utils.py
+test/test_xml.py
```

### Comparing `graphtage-0.2.7/setup.py` & `graphtage-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,30 +32,38 @@
         'Tracker': 'https://github.com/trailofbits/graphtage/issues',
     },
     author='Trail of Bits',
     version=get_version_string(),
     packages=find_packages(exclude=['test']),
     python_requires='>=3.7',
     install_requires=[
-        'colorama',
-        'intervaltree',
-        'json5==0.9.5',
-        'numpy>=1.19.4',
-        'PyYAML',
-        'scipy>=1.4.0',
-        'tqdm',
-        'typing_extensions>=3.7.4.3'
+        "colorama",
+        "intervaltree",
+        "json5==0.9.5",
+        "numpy>=1.19.4",
+        "PyYAML",
+        "scipy>=1.4.0",
+        "tqdm",
+        "typing_extensions>=3.7.4.3"
     ],
     entry_points={
         'console_scripts': [
             'graphtage = graphtage.__main__:main'
         ]
     },
     extras_require={
-        "dev": ["flake8", "Sphinx", "pytest", "sphinx_rtd_theme==0.4.3", "twine"]
+        "dev": [
+            "flake8",
+            "Sphinx",
+            "pytest",
+            "sphinx_rtd_theme==1.2.2",
+            "twine",
+            # workaround for https://github.com/python/importlib_metadata/issues/406:
+            "importlib_metadata<5; python_version == '3.7'"
+        ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `graphtage-0.2.7/test/test_bounds.py` & `graphtage-0.2.8/test/test_bounds.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_expressions.py` & `graphtage-0.2.8/test/test_expressions.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_fibonacci.py` & `graphtage-0.2.8/test/test_fibonacci.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_formatting.py` & `graphtage-0.2.8/test/test_formatting.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_graphtage.py` & `graphtage-0.2.8/test/test_graphtage.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_levenshtein.py` & `graphtage-0.2.8/test/test_levenshtein.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_matching.py` & `graphtage-0.2.8/test/test_matching.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_pydiff.py` & `graphtage-0.2.8/test/test_pydiff.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_search.py` & `graphtage-0.2.8/test/test_search.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.7/test/test_utils.py` & `graphtage-0.2.8/test/test_utils.py`

 * *Files identical despite different names*

