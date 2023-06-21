# Comparing `tmp/scutls-0.2.6.tar.gz` & `tmp/scutls-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.6.tar", max compression
+gzip compressed data, was "scutls-0.2.7.tar", max compression
```

## Comparing `scutls-0.2.6.tar` & `scutls-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      583 2023-06-16 21:11:31.148249 scutls-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-16 21:11:42.503322 scutls-0.2.6/scutls/__init__.py
--rw-r--r--   0        0        0     6447 2023-06-16 20:58:58.224143 scutls-0.2.6/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.6/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.6/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.6/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.6/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     5324 2023-06-16 20:48:21.500529 scutls-0.2.6/scutls/barcode.py
--rw-r--r--   0        0        0     1114 2023-06-16 20:42:39.857306 scutls-0.2.6/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.6/scutls/download.py
--rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.6/scutls/fastq.py
--rw-r--r--   0        0        0     9373 2023-06-16 21:10:25.736248 scutls-0.2.6/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.6/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-06-21 04:45:30.024217 scutls-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-21 04:45:43.775153 scutls-0.2.7/scutls/__init__.py
+-rw-r--r--   0        0        0     6447 2023-06-16 20:58:58.224143 scutls-0.2.7/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.7/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.7/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.7/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.7/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.2.7/scutls/barcode.py
+-rw-r--r--   0        0        0     1114 2023-06-16 20:42:39.857306 scutls-0.2.7/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.7/scutls/download.py
+-rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.7/scutls/fastq.py
+-rw-r--r--   0        0        0     9520 2023-06-21 04:17:41.657295 scutls-0.2.7/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.7/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.7/PKG-INFO
```

### Comparing `scutls-0.2.6/pyproject.toml` & `scutls-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.6"
+version = "0.2.7"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.2.6/scutls/arguments.py` & `scutls-0.2.7/scutls/arguments.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.7/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.7/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/assets/genome_ucsc.json` & `scutls-0.2.7/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/barcode.py` & `scutls-0.2.7/scutls/barcode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import argparse
 import functools
 from multiprocessing import Pool
 from Bio import SeqIO, bgzf
 from Bio.Seq import Seq
-from .util import fastq_chunk_interval, fastq_contain_barcode, get_search_pattern, fastq_locate_barcode
+from .util import fastq_chunk_interval, fastq_contain_barcode, get_search_pattern, fastq_locate_barcode, special_search_character
 import os
 import regex
 
 def barcode(input = None, output = None, output2 = None, contain = None, locate = None, pos = 0, error = 1, mismatch_only = False, rc_barcode = False, nproc = 1):
     """barcode subcommand
     Paramters
     ---------
 
     input : str
         input file name, auto detects .gz
     output : str
         output file name, auto detects .gz, contains fastq that contains specified barcode via contain
     contain: str
-        barcode to detect, if multiple barcode, separate with comma: "AATTCCC,AGGGCCC,CCGGCG"
+        barcode to detect, if multiple barcodess, separate with comma: "AATTCCC,AGGGCCC,CCGGCG", if pattern contains special characters including "()", "{}", "*", "=", the pattern will be passed as searching pattern
         # optional for "contain" sub-command:
         error: int
             allowed nucleotide mismatches (can be INDELs) when searching regex pattern, default to 1
         mismatch_only: bool
             if true, only mismatches (INDELs excluded) are allowed when searching regex pattern, default to False
         nproc: int
             number of parallel jobs, default to 1
@@ -42,15 +42,20 @@
         print("scutls fastq: warning: use 'scutls contain -h' for usage")
     # use True since args can be either None or False
     # arguments.py defines requirments of each argument
 
     # check if input fastq contains specified barcode:
     if contain:
         # prepare search pattern
-        barcode_pattern = get_search_pattern(pattern = contain, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
+        for character in special_search_character:
+            if character in contain:
+                barcode_pattern = contain 
+                break
+            else:
+                barcode_pattern = get_search_pattern(pattern = contain, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
         
         # print("barcode_pattern: ", barcode_pattern)
 
         # multiprocessing
         if not output == None:
             print("Saving to " + output + " ...")
         else:
@@ -92,15 +97,20 @@
                 SeqIO.write(fastq_non_hit, output2, "fastq")
         
         print("Done!")
 
     # check if input fastq contains specified barcode
     if locate:
         # prepare search pattern
-        barcode_pattern = get_search_pattern(pattern = locate, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
+        for character in special_search_character:
+            if character in locate:
+                barcode_pattern = locate 
+                break
+        else:
+            barcode_pattern = get_search_pattern(pattern = locate, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
 
         # multiprocessing
         intervals = fastq_chunk_interval(input, nproc = nproc)
         p = Pool(nproc)
         res_list = p.map_async(
             functools.partial(
                 fastq_locate_barcode,
```

### Comparing `scutls-0.2.6/scutls/cli.py` & `scutls-0.2.7/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/download.py` & `scutls-0.2.7/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/fastq.py` & `scutls-0.2.7/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.6/scutls/util.py` & `scutls-0.2.7/scutls/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,9 +239,12 @@
                 pos_start = [match.start() for match in matches]
                 if not len(pos_start) == 0:
                     res.append([record.id, pos_start[pos], len(record.seq)])
                 else:
                     res.append([record.id, "NA", len(record.seq)])
     return(res)
 
+# if containing the following characters, the pattern will be passed directly to regex:
+special_search_character = ["{", "}", "(", ")", "*", "="]
+
 if __name__ == "__main__":
     update_ensembl_release()
```

### Comparing `scutls-0.2.6/setup.py` & `scutls-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.6/PKG-INFO` & `scutls-0.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.6
+Version: 0.2.7
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

