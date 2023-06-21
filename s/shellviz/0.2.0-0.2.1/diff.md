# Comparing `tmp/shellviz-0.2.0.tar.gz` & `tmp/shellviz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellviz-0.2.0.tar", max compression
+gzip compressed data, was "shellviz-0.2.1.tar", max compression
```

## Comparing `shellviz-0.2.0.tar` & `shellviz-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1060 2023-04-12 06:44:46.797833 shellviz-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-12 06:44:46.797887 shellviz-0.2.0/README.md
--rw-r--r--   0        0        0      345 2023-06-07 05:26:07.245241 shellviz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6425 2023-06-07 05:25:27.881642 shellviz-0.2.0/shellviz/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-03 07:43:34.292945 shellviz-0.2.0/shellviz/__main__.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 shellviz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-12 06:44:46.797833 shellviz-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-12 06:44:46.797887 shellviz-0.2.1/README.md
+-rw-r--r--   0        0        0      396 2023-06-21 06:45:33.001993 shellviz-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6425 2023-06-07 05:25:27.881642 shellviz-0.2.1/shellviz/__init__.py
+-rw-r--r--   0        0        0     1830 2023-06-21 06:44:49.219968 shellviz-0.2.1/shellviz/console.py
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 shellviz-0.2.1/PKG-INFO
```

### Comparing `shellviz-0.2.0/LICENSE.txt` & `shellviz-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellviz-0.2.0/shellviz/__init__.py` & `shellviz-0.2.1/shellviz/__init__.py`

 * *Files identical despite different names*

### Comparing `shellviz-0.2.0/shellviz/__main__.py` & `shellviz-0.2.1/shellviz/console.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-#!/usr/bin/python3
+#!/usr/bin/env python
 
-# Usage: python -m shellviz [options] data
+# Usage: sv [options] data
 # Data can be piped in or passed as an argument.
-# e.g. python -m shellviz [options] '[1, 2, 3]'
-# e.g. python -m shellviz [options] < data.json
+# e.g. sv [options] '[1, 2, 3]'
+# e.g. sv [options] < data.json
 # options:
 #  -h, --help            show this help message and exit
 #  -i ID, --id=ID        ID of the visualization to update
+#  -d, --domain          The domain of a self-hosted shellviz server. Defaults to https://shellviz.com
+#  -k, --key             The API key for the shellviz server. Not required if using the free tier
+#  -I, --instance        The id of an existing instance to use. If not provided, a new instance will be created
+
 
 
 import argparse
 import sys
-from . import visualize
+from . import Shellviz
+
 
+def main(args=None):
+    if args is None:
+        args = sys.argv[1:]
 
-def main():
     # Define and parse command-line arguments
     parser = argparse.ArgumentParser(description='Process data for shellviz')
-    parser.add_argument('-i', '--id', type=int, help='ID of the visualization to update')
+    parser.add_argument('-i', '--id', type=str, help='ID of the visualization to update')
+    parser.add_argument('-d', '--domain', type=str, help='The domain of a self-hosted shellviz server. Defaults to https://shellviz.com')
+    parser.add_argument('-k', '--key', type=str, help='The API key for the shellviz server. Not required if using the free tier')
+    parser.add_argument('-I', '--instance', type=str, help='The id of an existing instance to use. If not provided, a new instance will be created')
     parser.add_argument('data', nargs='?', help='Data to process; may be passed from input redirection (e.g. shellviz < data.json), piped (e.g. cat data.son | shellviz) or passed as an argument (e.g. shellviz "[1, 2, 3]")')
-    args = parser.parse_args()
+    args = parser.parse_args(args)
 
+    sv = Shellviz(domain=args.domain, key=args.key, id=args.instance)
     data = args.data or sys.stdin.read()
-    id = args.id
-
-    result = visualize(data, id)
-    print(result)
-
+    result = sv.visualize(data, args.id)
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":  # pragma: no cover
+    main()
```

