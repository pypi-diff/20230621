# Comparing `tmp/clinvar-tsv-0.5.0.tar.gz` & `tmp/clinvar-tsv-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinvar-tsv-0.5.0.tar", last modified: Wed May  3 10:52:53 2023, max compression
+gzip compressed data, was "clinvar-tsv-0.6.0.tar", last modified: Wed Jun 21 10:30:12 2023, max compression
```

## Comparing `clinvar-tsv-0.5.0.tar` & `clinvar-tsv-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/clinvar_tsv/
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/clinvar_tsv/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/parse_clinvar_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-92148661.xml
--rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-in-context-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-spta1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-in-context-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-spta1.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_parse_xml_small.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_parse_xml_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/clinvar_tsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 10:30:12.862610 clinvar-tsv-0.6.0/clinvar_tsv/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/clinvar_tsv/parse_clinvar_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 10:30:12.000000 clinvar-tsv-0.6.0/clinvar_tsv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:30:12.858610 clinvar-tsv-0.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/clinvar-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/clinvar-92148661.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/clinvar-in-context-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/clinvar-spta1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/parsed-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/parsed-in-context-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/data/parsed-spta1.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/test_merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/test_parse_xml_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/tests/test_parse_xml_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-21 10:30:08.000000 clinvar-tsv-0.6.0/versioneer.py
```

### Comparing `clinvar-tsv-0.5.0/LICENSE` & `clinvar-tsv-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/PKG-INFO` & `clinvar-tsv-0.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml/badge.svg)](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/bihealth/clinvar-tsv/branch/main/graph/badge.svg?token=287XB5P11T)](https://codecov.io/gh/bihealth/clinvar-tsv)
+[![Package Version](https://img.shields.io/pypi/v/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
+[![Python Versions](https://img.shields.io/pypi/pyversions/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
 
 # Clinvar-TSV
 
 The code in this repository allows to first download,t hen convert ClinVar XML files into TSV files (one for b37 and b38).
 The TSV files will contain one entry for each ClinVar `<ReferenceClinVarAssertion>` entry with important information extracted from ClinVar.
 The code is used by [bihealth/varfish-db-downloader](https://github.com/bihealth/varfish-db-downloader).
 
@@ -61,14 +63,26 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+## [0.6.0](https://www.github.com/bihealth/clinvar-tsv/compare/v0.5.0...v0.6.0) (2023-06-21)
+
+
+### Features
+
+* allow providing clinvar version ([#17](https://www.github.com/bihealth/clinvar-tsv/issues/17)) ([dd80f2d](https://www.github.com/bihealth/clinvar-tsv/commit/dd80f2d10fceab350c61fa8de61bbe6264ad2008))
+
+
+### Documentation
+
+* adding badges to README ([#15](https://www.github.com/bihealth/clinvar-tsv/issues/15)) ([6e7ac01](https://www.github.com/bihealth/clinvar-tsv/commit/6e7ac013be4c0c7c34df41b69594581a7b8116f9))
+
 ## [0.5.0](https://www.github.com/bihealth/clinvar-tsv/compare/v0.4.1...v0.5.0) (2023-05-03)
 
 
 ### Features
 
 * export structural variants ([#13](https://www.github.com/bihealth/clinvar-tsv/issues/13)) ([db44d87](https://www.github.com/bihealth/clinvar-tsv/commit/db44d8739f6f619266f806611950f339b0842352))
```

### Comparing `clinvar-tsv-0.5.0/README.md` & `clinvar-tsv-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [![CI](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml/badge.svg)](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/bihealth/clinvar-tsv/branch/main/graph/badge.svg?token=287XB5P11T)](https://codecov.io/gh/bihealth/clinvar-tsv)
+[![Package Version](https://img.shields.io/pypi/v/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
+[![Python Versions](https://img.shields.io/pypi/pyversions/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
 
 # Clinvar-TSV
 
 The code in this repository allows to first download,t hen convert ClinVar XML files into TSV files (one for b37 and b38).
 The TSV files will contain one entry for each ClinVar `<ReferenceClinVarAssertion>` entry with important information extracted from ClinVar.
 The code is used by [bihealth/varfish-db-downloader](https://github.com/bihealth/varfish-db-downloader).
```

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/Snakefile` & `clinvar-tsv-0.6.0/clinvar_tsv/Snakefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+import os
 import os.path
 
+#: ClinVar version to download.
+CLINVAR_VERSION = os.environ.get("CLINVAR_VERSION")
+
 #: Path to b37/b38 FASTA file
 REF = {
     'b37': config.get('b37_path', '/dev/null'),
     'b38': config.get('b38_path', '/dev/null'),
 }
 
 
@@ -14,35 +18,25 @@
             size=("small", "sv"),
             build=("b37", "b38"),
             ext=(".gz", ".gz.tbi", ".gz.md5", ".gz.tbi.md5"),
         )
 
 
 rule download_xml:
-    output: "downloads/ClinVarFullRelease_00-latest.xml.gz"
-    shell:
-        r"""
-        wget -c -N -O {output} ftp://ftp.ncbi.nlm.nih.gov/pub/clinvar/xml/ClinVarFullRelease_00-latest.xml.gz \
-        2> {output}.log
-        """
-
-
-rule download_txt:
-    output: "downloads/variant_summary.txt.gz"
+    output: "downloads/ClinVarFullRelease_{clinvar_version}.xml.gz"
     shell:
         r"""
-        wget -c -N -O {output} ftp://ftp.ncbi.nlm.nih.gov/pub/clinvar/tab_delimited/variant_summary.txt.gz \
+        wget -c -N -O {output} https://ftp.ncbi.nlm.nih.gov/pub/clinvar/xml/weekly_release/ClinVarFullRelease_{wildcards.clinvar_version}.xml.gz \
         2> {output}.log
         """
 
 
 rule parse_clinvar:
     input:
-        release_xml="downloads/ClinVarFullRelease_00-latest.xml.gz",
-        summary="downloads/variant_summary.txt.gz",
+        release_xml=f"downloads/ClinVarFullRelease_{CLINVAR_VERSION}.xml.gz"
     output:
         b37_small="parsed/clinvar_table_raw.b37.tsv",
         b37_sv="parsed/clinvar_sv.b37.tsv",
         b38_small="parsed/clinvar_table_raw.b38.tsv",
         b38_sv="parsed/clinvar_sv.b38.tsv",
     shell:
         r"""
```

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/__main__.py` & `clinvar-tsv-0.6.0/clinvar_tsv/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,12 +178,13 @@
     parser_merge_tsvs.add_argument("--output-tsv", required=True, help="Path to output TSV file.")
     parser_merge_tsvs.add_argument(
         "--clinvar-version", required=True, help="String to put as clinvar version"
     )
     parser_merge_tsvs.set_defaults(func=run_merge_tsvs)
 
     args = parser.parse_args(argv)
+    os.environ["CLINVAR_VERSION"] = args.clinvar_version
     return run(args)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/common.py` & `clinvar-tsv-0.6.0/clinvar_tsv/common.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/merge_tsvs.py` & `clinvar-tsv-0.6.0/clinvar_tsv/merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/normalize.py` & `clinvar-tsv-0.6.0/clinvar_tsv/normalize.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv/parse_clinvar_xml.py` & `clinvar-tsv-0.6.0/clinvar_tsv/parse_clinvar_xml.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv.egg-info/PKG-INFO` & `clinvar-tsv-0.6.0/clinvar_tsv.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml/badge.svg)](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/bihealth/clinvar-tsv/branch/main/graph/badge.svg?token=287XB5P11T)](https://codecov.io/gh/bihealth/clinvar-tsv)
+[![Package Version](https://img.shields.io/pypi/v/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
+[![Python Versions](https://img.shields.io/pypi/pyversions/clinvar-tsv.svg)](https://pypi.org/project/clinvar-tsv)
 
 # Clinvar-TSV
 
 The code in this repository allows to first download,t hen convert ClinVar XML files into TSV files (one for b37 and b38).
 The TSV files will contain one entry for each ClinVar `<ReferenceClinVarAssertion>` entry with important information extracted from ClinVar.
 The code is used by [bihealth/varfish-db-downloader](https://github.com/bihealth/varfish-db-downloader).
 
@@ -61,14 +63,26 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+## [0.6.0](https://www.github.com/bihealth/clinvar-tsv/compare/v0.5.0...v0.6.0) (2023-06-21)
+
+
+### Features
+
+* allow providing clinvar version ([#17](https://www.github.com/bihealth/clinvar-tsv/issues/17)) ([dd80f2d](https://www.github.com/bihealth/clinvar-tsv/commit/dd80f2d10fceab350c61fa8de61bbe6264ad2008))
+
+
+### Documentation
+
+* adding badges to README ([#15](https://www.github.com/bihealth/clinvar-tsv/issues/15)) ([6e7ac01](https://www.github.com/bihealth/clinvar-tsv/commit/6e7ac013be4c0c7c34df41b69594581a7b8116f9))
+
 ## [0.5.0](https://www.github.com/bihealth/clinvar-tsv/compare/v0.4.1...v0.5.0) (2023-05-03)
 
 
 ### Features
 
 * export structural variants ([#13](https://www.github.com/bihealth/clinvar-tsv/issues/13)) ([db44d87](https://www.github.com/bihealth/clinvar-tsv/commit/db44d8739f6f619266f806611950f339b0842352))
```

### Comparing `clinvar-tsv-0.5.0/clinvar_tsv.egg-info/SOURCES.txt` & `clinvar-tsv-0.6.0/clinvar_tsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/setup.cfg` & `clinvar-tsv-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/setup.py` & `clinvar-tsv-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/conftest.py` & `clinvar-tsv-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/clinvar-74722873.xml` & `clinvar-tsv-0.6.0/tests/data/clinvar-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/clinvar-92148661.xml` & `clinvar-tsv-0.6.0/tests/data/clinvar-92148661.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/clinvar-in-context-74722873.xml` & `clinvar-tsv-0.6.0/tests/data/clinvar-in-context-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/clinvar-spta1.xml` & `clinvar-tsv-0.6.0/tests/data/clinvar-spta1.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/parsed-74722873.37.tsv` & `clinvar-tsv-0.6.0/tests/data/parsed-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/parsed-in-context-74722873.37.tsv` & `clinvar-tsv-0.6.0/tests/data/parsed-in-context-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/data/parsed-spta1.37.tsv` & `clinvar-tsv-0.6.0/tests/data/parsed-spta1.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/test_merge_tsvs.py` & `clinvar-tsv-0.6.0/tests/test_merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/test_parse_xml_small.py` & `clinvar-tsv-0.6.0/tests/test_parse_xml_small.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/tests/test_parse_xml_sv.py` & `clinvar-tsv-0.6.0/tests/test_parse_xml_sv.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.5.0/versioneer.py` & `clinvar-tsv-0.6.0/versioneer.py`

 * *Files identical despite different names*

