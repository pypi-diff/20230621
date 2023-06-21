# Comparing `tmp/biblatex2bibtex-0.0.2.tar.gz` & `tmp/biblatex2bibtex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biblatex2bibtex-0.0.2.tar", last modified: Wed Oct 26 21:25:51 2022, max compression
+gzip compressed data, was "dist/biblatex2bibtex-0.0.3.tar", last modified: Wed Jun 21 07:16:17 2023, max compression
```

## Comparing `biblatex2bibtex-0.0.2.tar` & `biblatex2bibtex-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.2/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.2/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1590 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)      710 2022-10-26 05:06:53.000000 biblatex2bibtex-0.0.2/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      514 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.2/pyproject.toml
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1837 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.2/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     2663 2022-10-26 21:23:57.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex/__init__.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1017 2022-10-26 21:22:29.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex/cli.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex/data/
--rw-r--r--   0 florianm  (1000) florianm  (1000)    14802 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex/data/biblatex2bibtex.conf
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1590 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      470 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       61 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/entry_points.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      282 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       16 2022-10-26 21:25:51.000000 biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.3/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.3/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1530 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/PKG-INFO
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      650 2022-10-26 21:29:21.000000 biblatex2bibtex-0.0.3/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      514 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.3/pyproject.toml
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1837 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.3/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     3037 2023-06-21 07:15:56.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex/__init__.py
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1017 2023-06-21 07:14:14.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex/cli.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex/data/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)    14802 2022-10-26 04:10:19.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex/data/biblatex2bibtex.conf
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1530 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      470 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       61 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/entry_points.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      282 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       16 2023-06-21 07:16:17.000000 biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/top_level.txt
```

### Comparing `biblatex2bibtex-0.0.2/LICENSE` & `biblatex2bibtex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biblatex2bibtex-0.0.2/PKG-INFO` & `biblatex2bibtex-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblatex2bibtex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert biblatex files to bibtex.
 Home-page: https://github.com/fmatter/biblatex2bibtex
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/biblatex2bibtex/issues
 Keywords: biblatex,bibtex
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,12 +30,8 @@
 
 Convert biblatex files to bibtex.
 
 **Note: you need [`biber`](https://github.com/plk/biber).**
 
 Usage:
 
-`biblatex2bibtex /path/to/biblatex_file.bib` (will create `/path/to/biblatex_file_out.bib`)
-
-or 
-
-`biblatex2bibtex /path/to/biblatex_file.bib /path/to/bibtex_file.bib`
+`biblatex2bibtex /path/to/biblatex_file1.bib /path/to/biblatex_file2.bib --output /path/to/bibtex_file.bib`
```

### Comparing `biblatex2bibtex-0.0.2/README.md` & `biblatex2bibtex-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,12 +7,8 @@
 
 Convert biblatex files to bibtex.
 
 **Note: you need [`biber`](https://github.com/plk/biber).**
 
 Usage:
 
-`biblatex2bibtex /path/to/biblatex_file.bib` (will create `/path/to/biblatex_file_out.bib`)
-
-or 
-
-`biblatex2bibtex /path/to/biblatex_file.bib /path/to/bibtex_file.bib`
+`biblatex2bibtex /path/to/biblatex_file1.bib /path/to/biblatex_file2.bib --output /path/to/bibtex_file.bib`
```

### Comparing `biblatex2bibtex-0.0.2/pyproject.toml` & `biblatex2bibtex-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biblatex2bibtex-0.0.2/setup.cfg` & `biblatex2bibtex-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	bibtex
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = biblatex2bibtex
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/biblatex2bibtex/issues
 url = https://github.com/fmatter/biblatex2bibtex
-version = 0.0.2
+version = 0.0.3
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `biblatex2bibtex-0.0.2/src/biblatex2bibtex/__init__.py` & `biblatex2bibtex-0.0.3/src/biblatex2bibtex/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 import subprocess
 from pathlib import Path
 import bibtexparser
 import colorlog
 import pkg_resources
 from pybtex.database.input import bibtex
 
@@ -14,29 +15,40 @@
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 log.propagate = True
 log.addHandler(handler)
 
 
 __author__ = "Florian Matter"
-__email__ = "florianmatter@gmail.com"
-__version__ = "0.0.2"
+__email__ = "fmatter@mailbox.org"
+__version__ = "0.0.3"
+
+macro_expr = re.compile(r"\\.*?\{(?P<content>.*?)\}")
+
+
+def remove_macros(s):
+    return macro_expr.sub(r"\g<content>", s)
 
 
 def preprocess(biblatex_file):
     biblatex_file = Path(biblatex_file)
     bib_data = bibtex.Parser().parse_file(biblatex_file)
     for entry in bib_data.entries.values():
         if entry.type == "collection":
             entry.fields["booktitle"] = entry.fields["title"]
     temp_file = (
         biblatex_file.parent / f"{biblatex_file.stem}_temp{biblatex_file.suffix}"
     )
     bib_data.to_file(temp_file)
 
+    with open(temp_file, "r", encoding="utf-8") as f:
+        content = remove_macros(f.read())
+    with open(temp_file, "w", encoding="utf-8") as f:
+        f.write(content)
+
     conf_file = pkg_resources.resource_filename(
         "biblatex2bibtex", "data/biblatex2bibtex.conf"
     )
     subprocess.run(
         f"biber --tool --configfile={conf_file} --output-resolve --output-file='{temp_file}' {temp_file}",
         shell=True,
         check=True,
@@ -45,41 +57,41 @@
     return temp_file
 
 
 def modify(temp_file):
     with open(temp_file, "r", encoding="utf-8") as bibtex_file:
         bib_database = bibtexparser.load(bibtex_file)
 
-    for i in bib_database.entries:
-        i["title"] = i["title"].replace("{", "").replace("}", "")
-        if "booktitle" in i:
-            i["booktitle"] = i["booktitle"].replace("{", "").replace("}", "")
-        if "pages" in i:
-            i["pages"] = i["pages"].replace("--", "–")
+    for entry in bib_database.entries:
+        entry["title"] = entry["title"].replace("{", "").replace("}", "")
+        if "booktitle" in entry:
+            entry["booktitle"] = entry["booktitle"].replace("{", "").replace("}", "")
+        if "pages" in entry:
+            entry["pages"] = entry["pages"].replace("--", "–")
         replace = {
             "date": "year",
             "location": "address",
             "journaltitle": "journal",
             "issue": "number",
             "origdate": "year",
             "school": "institution",
             "maintitle": "booktitle",
         }
         for k, v in replace.items():
-            if k in i:
-                i[v] = i[k]
-                del i[k]
-        if "note" in i and i["note"] == "\\textsc{ms}":
-            del i["note"]
-            i["howpublished"] = "Manuscript"
+            if k in entry:
+                entry[v] = entry[k]
+                del entry[k]
+        if "note" in entry and entry["note"] == "\\textsc{ms}":
+            del entry["note"]
+            entry["howpublished"] = "Manuscript"
     temp_file.unlink()
     return bib_database
 
-def convert(biblatex_files, bibtex_output):
 
+def convert(biblatex_files, bibtex_output):
     temp_files = []
     for biblatex_file in biblatex_files:
         temp_files.append(preprocess(biblatex_file))
 
     databases = []
     for temp_file in temp_files:
         databases.append(modify(temp_file))
```

### Comparing `biblatex2bibtex-0.0.2/src/biblatex2bibtex/cli.py` & `biblatex2bibtex-0.0.3/src/biblatex2bibtex/cli.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import biblatex2bibtex
 import argparse
 import logging
+import sys
 from pathlib import Path
 from biblatex2bibtex import convert
-import sys
+
 
 log = logging.getLogger(__name__)
 
 
 def main():
-
     parser = argparse.ArgumentParser(description="convert biblatex to bibtex files")
     parser.add_argument(
         "biblatexfiles", nargs="+", help="biblatex file(s) to be converted", type=str
     )
     parser.add_argument(
         "--output", nargs="?", help="bibtex output file", type=str, default=None
     )
```

### Comparing `biblatex2bibtex-0.0.2/src/biblatex2bibtex/data/biblatex2bibtex.conf` & `biblatex2bibtex-0.0.3/src/biblatex2bibtex/data/biblatex2bibtex.conf`

 * *Files identical despite different names*

### Comparing `biblatex2bibtex-0.0.2/src/biblatex2bibtex.egg-info/PKG-INFO` & `biblatex2bibtex-0.0.3/src/biblatex2bibtex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblatex2bibtex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert biblatex files to bibtex.
 Home-page: https://github.com/fmatter/biblatex2bibtex
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/biblatex2bibtex/issues
 Keywords: biblatex,bibtex
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,12 +30,8 @@
 
 Convert biblatex files to bibtex.
 
 **Note: you need [`biber`](https://github.com/plk/biber).**
 
 Usage:
 
-`biblatex2bibtex /path/to/biblatex_file.bib` (will create `/path/to/biblatex_file_out.bib`)
-
-or 
-
-`biblatex2bibtex /path/to/biblatex_file.bib /path/to/bibtex_file.bib`
+`biblatex2bibtex /path/to/biblatex_file1.bib /path/to/biblatex_file2.bib --output /path/to/bibtex_file.bib`
```

