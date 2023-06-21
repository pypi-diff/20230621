# Comparing `tmp/docbuild-0.1.114.tar.gz` & `tmp/docbuild-0.1.115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.114.tar", last modified: Thu Jun 15 12:30:09 2023, max compression
+gzip compressed data, was "docbuild-0.1.115.tar", last modified: Wed Jun 21 13:59:01 2023, max compression
```

## Comparing `docbuild-0.1.114.tar` & `docbuild-0.1.115.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.801814 docbuild-0.1.114/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-15 12:30:09.801577 docbuild-0.1.114/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.114/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.789097 docbuild-0.1.114/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-15 12:30:03.000000 docbuild-0.1.114/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.114/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.114/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.114/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7390 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.797883 docbuild-0.1.114/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.114/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.114/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.114/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.114/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.114/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.114/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.800983 docbuild-0.1.114/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.114/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    15947 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)    24827 2023-06-15 12:29:48.000000 docbuild-0.1.114/docbuild/visual_detection/borderless_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.114/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16336 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.794365 docbuild-0.1.114/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-15 12:30:09.801982 docbuild-0.1.114/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-15 12:29:57.000000 docbuild-0.1.114/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-21 13:59:01.830603 docbuild-0.1.115/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-21 13:59:01.830434 docbuild-0.1.115/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.115/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-21 13:59:01.825394 docbuild-0.1.115/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-21 13:58:54.000000 docbuild-0.1.115/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.115/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.115/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.115/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7390 2023-06-21 13:45:12.000000 docbuild-0.1.115/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-21 13:59:01.828093 docbuild-0.1.115/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.115/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.115/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.115/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.115/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.115/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.115/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-06-15 12:27:28.000000 docbuild-0.1.115/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-21 13:59:01.830177 docbuild-0.1.115/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.115/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    15947 2023-06-21 13:44:14.000000 docbuild-0.1.115/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)    25710 2023-06-21 13:24:49.000000 docbuild-0.1.115/docbuild/visual_detection/borderless_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.115/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16336 2023-06-21 13:52:42.000000 docbuild-0.1.115/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-21 13:59:01.826771 docbuild-0.1.115/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-21 13:59:01.000000 docbuild-0.1.115/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-21 13:59:01.000000 docbuild-0.1.115/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-21 13:59:01.000000 docbuild-0.1.115/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-21 13:59:01.000000 docbuild-0.1.115/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-21 13:59:01.000000 docbuild-0.1.115/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-21 13:59:01.830649 docbuild-0.1.115/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-21 13:58:27.000000 docbuild-0.1.115/setup.py
```

### Comparing `docbuild-0.1.114/PKG-INFO` & `docbuild-0.1.115/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.114
+Version: 0.1.115
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.114/docbuild/graph.py` & `docbuild-0.1.115/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/hocr_parser.py` & `docbuild-0.1.115/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/page_creator.py` & `docbuild-0.1.115/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.115/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.115/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.115/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/textract_parser.py` & `docbuild-0.1.115/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/utils.py` & `docbuild-0.1.115/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.115/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild/visual_detection/borderless_table_extraction.py` & `docbuild-0.1.115/docbuild/visual_detection/borderless_table_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class BorderLessTableExtractor:
     def __init__(self):
         pass
 
 
-class Column:
+class LineColumn:
     def __init__(self, lines: list[Line]):
         self.lines = lines
         self.bounding_box = BoundingBox.compose_bounding_boxes(
             [line.bounding_box for line in lines]
         )
 
 
@@ -184,27 +184,27 @@
                 close_under_line_index = map_line_to_line_index[under_line]
                 nodes[line_index].add_neighbor(nodes[close_under_line_index])
                 nodes[close_under_line_index].add_neighbor(nodes[line_index])
 
         graph = Graph(nodes=nodes)
         return graph
 
-    def convert_cc_to_column(self, cc: list[Node]) -> Column:
+    def convert_cc_to_column(self, cc: list[Node]) -> LineColumn:
         lines = [node.data for node in cc]
-        column = Column(lines=lines)
+        column = LineColumn(lines=lines)
         return column
 
     def filter_connected_components(self, ccs: list[list[Node]]) -> list[list[Node]]:
         filtered_ccs = []
         for cc in ccs:
             if len(cc) >= 3:
                 filtered_ccs.append(cc)
         return filtered_ccs
 
-    def extract_columns(self):
+    def extract_columns(self) -> list[LineColumn]:
         lines = ColumnLineFilter(lines=self.lines).filter_lines()
         graph = self.get_graph(lines)
         connected_components = graph.get_connected_components()
         connected_components = self.filter_connected_components(connected_components)
         columns = [self.convert_cc_to_column(cc) for cc in connected_components]
         return columns
 
@@ -266,14 +266,18 @@
         return self.optional_boxes["maximal"].get_bounding_box()
 
     def is_row_colliding(self, other_box: BoundingBox) -> bool:
         bounding_box = self.get_bounding_box()
         if bounding_box is None:
             return True
         return bounding_box.vertical_intersect(other_box)
+    
+    def is_colliding_with_other_aggregator(self, other_agg) -> bool:
+        bounding_box = self.get_bounding_box()
+        return bounding_box.intersect(other_agg.get_bounding_box())
 
     def get_intersection_percentage(self, other_box: BoundingBox) -> float:
         bounding_box = self.get_bounding_box()
         if bounding_box is None:
             return 0
         intersection_area = max(
             0,
@@ -293,14 +297,18 @@
     def add_element(self, element_box: BoundingBox, element: object = None):
         self.elements.append(element)
         self.all_boxes.append(element_box)
 
         for box in self.optional_boxes.values():
             box.expand(element_box)
 
+    def swallow_other_aggregator(self, other_agg):
+        for box, element in zip(other_agg.all_boxes, other_agg.elements):
+            self.add_element(box, element)
+
 
 class BoundingBoxTable(object):
     EMPTY_CELL = 0
 
     def __init__(self):
         self.columns = []
         self.rows = []
@@ -404,15 +412,18 @@
 
     def add_table_at_bottom(self, other_table):
         table_lowest_row = self.rows[-1].bounding_box.bottom
         first_index_below_table = [
             i
             for i, row in enumerate(other_table.rows)
             if row.bounding_box.top < table_lowest_row
-        ][0]
+        ]
+        if len(first_index_below_table) == 0:
+            return
+        first_index_below_table = first_index_below_table[0]
         self.rows = self.rows + other_table.rows[first_index_below_table:]
         self.cells = np.r_[self.cells, other_table.cells[first_index_below_table:, :]]
         for this_col, other_col in zip(self.columns, other_table.columns):
             this_col.expand(other_col.bounding_box)
 
 
 class BorderlessTableExtractor:
@@ -447,19 +458,29 @@
                     break
             if not found:
                 aggregate_columns.append(BoundingBoxAggregator())
                 aggregate_columns[-1].add_element(col.bounding_box, col)
 
         # Remove aggragators with only one element
         aggregate_columns = [agg for agg in aggregate_columns if len(agg.elements) > 1]
-        return aggregate_columns
 
-    def cluster_lines_to_tables(
-        self, aggregate_columns: list[BoundingBoxAggregator]
-    ) -> list[BoundingBoxTable]:
+        # Remove aggregators that are colliding with another aggregator
+        non_colliding_aggregators = []
+        for agg in aggregate_columns:
+            found = False
+            for other_agg in non_colliding_aggregators:
+                if agg != other_agg and agg.is_colliding_with_other_aggregator(other_agg):
+                    other_agg.swallow_other_aggregator(agg)
+                    found = True
+                    break
+            if not found:
+                non_colliding_aggregators.append(agg)
+        return non_colliding_aggregators
+    
+    def cluster_lines_to_tables(self, aggregate_columns : list[BoundingBoxAggregator]) -> list[BoundingBoxTable]:
         # Look for missing lines
         tables = []
         for agg in aggregate_columns:
             bb_table = BoundingBoxTable()
             for line in self.lines:
                 if (
                     agg.get_intersection_percentage(line.bounding_box)
@@ -470,23 +491,18 @@
         return tables
 
     def force_headers(self, table: BoundingBoxTable) -> list[list[Line]]:
         "Assumes that self.lines is sorted by top coordinate"
         potential_headers = [[] for i in range(len(table.columns))]
 
         # Find the lowest line that is above the table
-        lowest_ind = [
-            i
-            for i, line in enumerate(self.lines)
-            if line.bounding_box.bottom > table.rows[0].bounding_box.top
-        ]
-        lowest_ind = lowest_ind[-1] if len(lowest_ind) > 0 else -1
+        lines_above = [line for line in self.lines if line.bounding_box.bottom > table.rows[0].bounding_box.top]
+        lines_above.reverse()
 
-        for curr_ind in range(lowest_ind, -1, -1):
-            curr_line = self.lines[curr_ind]
+        for curr_line in lines_above:
             # check if line is aligned with a column
             columns = [
                 i
                 for i, col in enumerate(table.columns)
                 if col.bounding_box.horizontal_intersect(curr_line.bounding_box)
             ]
```

### Comparing `docbuild-0.1.114/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.115/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.115/docbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.114
+Version: 0.1.115
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.114/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.115/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.114/setup.py` & `docbuild-0.1.115/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.114",
+    version="0.1.115",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

