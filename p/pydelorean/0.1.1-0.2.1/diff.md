# Comparing `tmp/pydelorean-0.1.1.tar.gz` & `tmp/pydelorean-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-0.1.1.tar", last modified: Sun Jun 11 13:18:39 2023, max compression
+gzip compressed data, was "pydelorean-0.2.1.tar", last modified: Tue Jun 20 23:53:29 2023, max compression
```

## Comparing `pydelorean-0.1.1.tar` & `pydelorean-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.152165 pydelorean-0.1.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-0.1.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-06-11 13:18:39.152165 pydelorean-0.1.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-11 13:16:27.000000 pydelorean-0.1.1/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.149165 pydelorean-0.1.1/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1946 2023-06-10 12:13:51.000000 pydelorean-0.1.1/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3071 2023-06-10 16:40:07.000000 pydelorean-0.1.1/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-10 12:14:10.000000 pydelorean-0.1.1/pydelorean/errors.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-0.1.1/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      937 2023-06-10 12:22:30.000000 pydelorean-0.1.1/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-06-11 13:13:52.000000 pydelorean-0.1.1/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-10 12:13:51.000000 pydelorean-0.1.1/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-10 16:47:52.000000 pydelorean-0.1.1/pydelorean/tree/types.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.150165 pydelorean-0.1.1/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      422 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       27 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-06-11 13:18:39.000000 pydelorean-0.1.1/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-06-11 13:18:39.152165 pydelorean-0.1.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      943 2023-06-11 13:18:28.000000 pydelorean-0.1.1/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-11 13:18:39.151165 pydelorean-0.1.1/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-0.1.1/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-0.2.1/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-06-20 23:53:29.511133 pydelorean-0.2.1/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-12 11:33:27.000000 pydelorean-0.2.1/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1974 2023-06-20 23:44:32.000000 pydelorean-0.2.1/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3903 2023-06-20 23:53:14.000000 pydelorean-0.2.1/pydelorean/delorean.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1311 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-06-12 11:40:12.000000 pydelorean-0.2.1/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      400 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-06-20 23:53:29.511133 pydelorean-0.2.1/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-06-20 23:46:05.000000 pydelorean-0.2.1/setup.py
```

### Comparing `pydelorean-0.1.1/LICENSE` & `pydelorean-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.1/PKG-INFO` & `pydelorean-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.1.1
+Version: 0.2.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.2.1.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -101,7 +102,8 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
+
```

### Comparing `pydelorean-0.1.1/README.rst` & `pydelorean-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.1/pydelorean/__init__.py` & `pydelorean-0.2.1/pydelorean/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from .delorean import mdtreeify, findMetadata
 from .tree.types import MarkdownForest
+from .utils import FileType
 import re
 
 def treeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
     """Converts a markdown document into a MarkdownForest object.
 
     Args:
         name (str, optional): Name of the document.
```

### Comparing `pydelorean-0.1.1/pydelorean/delorean.py` & `pydelorean-0.2.1/pydelorean/delorean.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-""" This file contains the main functions for the mdforest package.
+""" This file contains the main functions for the delorean package.
 """
     
 import re
 
 import frontmatter
 from treelib import Tree
-
+from .utils import *
 from .tree.types import MarkdownForest, TextNode, HeaderNode, Node
 from .parser import *
 
 # ==================================================================================================
 #                                           TREEIFY
 # ==================================================================================================
 
@@ -49,16 +49,37 @@
     Converts markdown file to a MarkdownForest
     """
     
     meta, cont = findMetadata(md)
     
     backlinks = findBacklinks(cont)
     tags = findTags(cont)
-    parser = MarkdownParser(name, cont)
-    tree = parser.parse()
+    
+    if cont == "":
+        # If the file is empty, just create a root node
+        tree = Tree()
+        tree.create_node(tag=name, identifier="root").identifier
+    else:
+        # Based on the file type specified by the user, choose a parser
+        if 'type' in kwargs:
+            if kwargs['type'] == FileType.MARKDOWN:
+                parser = MarkdownParser(name, cont)
+            elif kwargs['type'] == FileType.RESTRUCTUREDTEXT:
+                parser = RestructuredParser(name, cont)
+            elif kwargs['type'] == FileType.TXT:
+                parser = TextParser(name, cont)
+            elif kwargs['type'] == FileType.YAML:
+                parser = YAMLParser(name, cont)
+            else:
+                raise ValueError("Invalid file type.")
+        else:
+            parser = MarkdownParser(name, cont)
+            
+        tree = parser.parse()
+    
     returnForest = MarkdownForest(tree, name, metadata=meta)
     
     for backlink in backlinks:
         returnForest.add_backlink(backlink)
     for tag in tags:
         returnForest.add_tag(tag)
```

### Comparing `pydelorean-0.1.1/pydelorean/parser/parser.py` & `pydelorean-0.2.1/pydelorean/parser/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,8 +29,26 @@
         super().__init__(document_name, text)
         
     def parse(self) -> Tree:
         HEADER_PATTERN = r'^(\S.*)\n[=~`\'^"-]+$'
         
         tree = buildTree(self.text, self.document_name, header_pattern=HEADER_PATTERN)
         return tree
+        
+
+class TextParser(Parser):
+    
+    def __init__(self, document_name:str, text:str):
+        super().__init__(document_name, text)
+        
+    def parse(self) -> Tree:
+        pass
+
+
+class YAMLParser(Parser):
+    
+    def __init__(self, document_name:str, text:str):
+        super().__init__(document_name, text)
+        
+    def parse(self) -> Tree:
+        pass
```

### Comparing `pydelorean-0.1.1/pydelorean/parser/utils.py` & `pydelorean-0.2.1/pydelorean/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.1/pydelorean/tree/types.py` & `pydelorean-0.2.1/pydelorean/tree/types.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.1.1/pydelorean.egg-info/PKG-INFO` & `pydelorean-0.2.1/pydelorean.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.1.1
+Version: 0.2.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.1.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.2.1.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -101,7 +102,8 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
+
```

### Comparing `pydelorean-0.1.1/setup.py` & `pydelorean-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '0.1.1'
+VERSION = '0.2.1'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/delorean",
     packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser'],
     tests_require = ['unittest'],
-    install_requires = ['python-frontmatter', 'treelib'],
+    install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
     download_url = 'https://github.com/kj3moraes/delorean/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

