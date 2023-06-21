# Comparing `tmp/iceberg-dsl-0.0.1.tar.gz` & `tmp/iceberg-dsl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg-dsl-0.0.1.tar", last modified: Wed Jun 21 20:29:14 2023, max compression
+gzip compressed data, was "iceberg-dsl-0.0.2.tar", last modified: Wed Jun 21 20:33:16 2023, max compression
```

## Comparing `iceberg-dsl-0.0.1.tar` & `iceberg-dsl-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:29:14.478449 iceberg-dsl-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3186 2023-06-21 20:29:14.479447 iceberg-dsl-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2044 2023-06-21 20:29:02.000000 iceberg-dsl-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 20:29:14.455457 iceberg-dsl-0.0.1/iceberg/
--rw-rw-rw-   0        0        0      169 2023-06-21 20:15:15.000000 iceberg-dsl-0.0.1/iceberg/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.1/iceberg/geometry.py
--rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.1/iceberg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:29:14.477453 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/
--rw-rw-rw-   0        0        0     3186 2023-06-21 20:29:14.000000 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-21 20:29:14.000000 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:29:14.000000 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-21 20:29:14.000000 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:29:14.000000 iceberg-dsl-0.0.1/iceberg_dsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-06-21 20:29:14.482444 iceberg-dsl-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-06-21 20:28:46.000000 iceberg-dsl-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.383538 iceberg-dsl-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3186 2023-06-21 20:33:16.383538 iceberg-dsl-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2044 2023-06-21 20:29:02.000000 iceberg-dsl-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.353821 iceberg-dsl-0.0.2/iceberg/
+-rw-rw-rw-   0        0        0      169 2023-06-21 20:33:05.000000 iceberg-dsl-0.0.2/iceberg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.359821 iceberg-dsl-0.0.2/iceberg/core/
+-rw-rw-rw-   0        0        0      177 2023-06-11 16:49:29.000000 iceberg-dsl-0.0.2/iceberg/core/__init__.py
+-rw-rw-rw-   0        0        0     6192 2023-06-21 18:45:19.000000 iceberg-dsl-0.0.2/iceberg/core/drawable.py
+-rw-rw-rw-   0        0        0    12151 2023-06-21 18:31:42.000000 iceberg-dsl-0.0.2/iceberg/core/properties.py
+-rw-rw-rw-   0        0        0     3637 2023-06-21 18:42:22.000000 iceberg-dsl-0.0.2/iceberg/core/renderer.py
+-rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.2/iceberg/geometry.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.371807 iceberg-dsl-0.0.2/iceberg/primitives/
+-rw-rw-rw-   0        0        0      264 2023-06-21 07:45:12.000000 iceberg-dsl-0.0.2/iceberg/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1124 2023-06-21 07:44:59.000000 iceberg-dsl-0.0.2/iceberg/primitives/filters.py
+-rw-rw-rw-   0        0        0     4244 2023-06-21 07:51:02.000000 iceberg-dsl-0.0.2/iceberg/primitives/latex.py
+-rw-rw-rw-   0        0        0    11915 2023-06-21 18:52:10.000000 iceberg-dsl-0.0.2/iceberg/primitives/layout.py
+-rw-rw-rw-   0        0        0     3691 2023-06-11 16:28:19.000000 iceberg-dsl-0.0.2/iceberg/primitives/shapes.py
+-rw-rw-rw-   0        0        0     1612 2023-06-21 18:52:45.000000 iceberg-dsl-0.0.2/iceberg/primitives/svg.py
+-rw-rw-rw-   0        0        0     2227 2023-06-21 07:27:18.000000 iceberg-dsl-0.0.2/iceberg/primitives/text.py
+-rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.2/iceberg/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.382527 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/
+-rw-rw-rw-   0        0        0     3186 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2023-06-21 20:33:16.385609 iceberg-dsl-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-06-21 20:31:57.000000 iceberg-dsl-0.0.2/setup.py
```

### Comparing `iceberg-dsl-0.0.1/LICENSE` & `iceberg-dsl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.1/PKG-INFO` & `iceberg-dsl-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-dsl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A compositional diagramming tool for Python.
 Home-page: https://github.com/revalo/iceberg
 Author: Shreyas Kapur
 Author-email: srkp@berkeley.edu
 Maintainer: Shreyas Kapur
 Maintainer-email: srkp@berkeley.edu
 License: MIT
```

### Comparing `iceberg-dsl-0.0.1/README.md` & `iceberg-dsl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.1/iceberg/geometry.py` & `iceberg-dsl-0.0.2/iceberg/geometry.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.1/iceberg/utils.py` & `iceberg-dsl-0.0.2/iceberg/utils.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.1/iceberg_dsl.egg-info/PKG-INFO` & `iceberg-dsl-0.0.2/iceberg_dsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-dsl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A compositional diagramming tool for Python.
 Home-page: https://github.com/revalo/iceberg
 Author: Shreyas Kapur
 Author-email: srkp@berkeley.edu
 Maintainer: Shreyas Kapur
 Maintainer-email: srkp@berkeley.edu
 License: MIT
```

### Comparing `iceberg-dsl-0.0.1/setup.cfg` & `iceberg-dsl-0.0.2/setup.cfg`

 * *Files identical despite different names*

