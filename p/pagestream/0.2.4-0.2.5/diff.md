# Comparing `tmp/pagestream-0.2.4.tar.gz` & `tmp/pagestream-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagestream-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pagestream-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pagestream-0.2.4.tar` & `pagestream-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.4/.gitignore
--rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.4/LICENSE
--rw-r--r--   0        0        0      528 2023-06-07 14:55:50.163659 pagestream-0.2.4/README.md
--rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3490 2023-06-21 11:46:35.995248 pagestream-0.2.4/src/pagestream/__init__.py
--rwxr-xr-x   0        0        0     1023 2023-06-21 11:44:52.869586 pagestream-0.2.4/src/pagestream/cli.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pagestream-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.5/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-07 14:55:50.163659 pagestream-0.2.5/README.md
+-rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3490 2023-06-21 11:49:29.491923 pagestream-0.2.5/src/pagestream/__init__.py
+-rwxr-xr-x   0        0        0     1016 2023-06-21 11:49:05.704816 pagestream-0.2.5/src/pagestream/cli.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pagestream-0.2.5/PKG-INFO
```

### Comparing `pagestream-0.2.4/LICENSE` & `pagestream-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.4/README.md` & `pagestream-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pagestream-0.2.4/src/pagestream/__init__.py` & `pagestream-0.2.5/src/pagestream/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from re import search
 from sys import setrecursionlimit
 from logging import info, debug
 from pathlib import Path
 from pikepdf._qpdf import Pdf, Page
 
-__version__ = "v0.2.4"
+__version__ = "v0.2.5"
 
 # flatten function can recurse a lot, python limits this by default to not
 # cause overflows in the CPython implementation
 setrecursionlimit(1024 * 1024)
 
 class PDFPageStream:
     """Represents a PDF file that consists of a stream of merged PDF documents"""
```

### Comparing `pagestream-0.2.4/src/pagestream/cli.py` & `pagestream-0.2.5/src/pagestream/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3
 
 import sys
 import click
 from pathlib import Path
 import logging
-from __init__ import PDFPageStream
+from . import PDFPageStream
 
 @click.group(help="PDF pagestream utility")
 def cli() -> None:
     fmt = "%(name)s [%(levelname)s] %(message)s"
     logging.basicConfig(stream=sys.stderr, level=logging.INFO, format=fmt)
 
 @cli.command("contents", help="Show identified documents in pagestream")
```

### Comparing `pagestream-0.2.4/PKG-INFO` & `pagestream-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagestream
-Version: 0.2.4
+Version: 0.2.5
 Summary: Handle PDF pagestreams with PikePDF and split them by outline
 Author-email: Johan Schuijt <johan@ftm.nl>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pikepdf
 Requires-Dist: click
 Project-URL: Home, https://github.com/followthemoney/pagestream
```

