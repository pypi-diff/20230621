# Comparing `tmp/clinvar-tsv-0.6.1.tar.gz` & `tmp/clinvar-tsv-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinvar-tsv-0.6.1.tar", last modified: Wed Jun 21 14:07:53 2023, max compression
+gzip compressed data, was "clinvar-tsv-0.6.2.tar", last modified: Wed Jun 21 15:02:30 2023, max compression
```

## Comparing `clinvar-tsv-0.6.1.tar` & `clinvar-tsv-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/clinvar_tsv/
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/clinvar_tsv/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/clinvar_tsv/parse_clinvar_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.026894 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 14:07:52.000000 clinvar-tsv-0.6.1/clinvar_tsv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.026894 clinvar-tsv-0.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.026894 clinvar-tsv-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:53.030895 clinvar-tsv-0.6.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/clinvar-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/clinvar-92148661.xml
--rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/clinvar-in-context-74722873.xml
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/clinvar-spta1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/parsed-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/parsed-in-context-74722873.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/data/parsed-spta1.37.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/test_merge_tsvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/test_parse_xml_small.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/tests/test_parse_xml_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-21 14:07:35.000000 clinvar-tsv-0.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/clinvar_tsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/clinvar_tsv/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/clinvar_tsv/parse_clinvar_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 15:02:30.000000 clinvar-tsv-0.6.2/clinvar_tsv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.299229 clinvar-tsv-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:02:30.303230 clinvar-tsv-0.6.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-92148661.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-in-context-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/clinvar-spta1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-in-context-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/data/parsed-spta1.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_parse_xml_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/tests/test_parse_xml_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-21 15:02:26.000000 clinvar-tsv-0.6.2/versioneer.py
```

### Comparing `clinvar-tsv-0.6.1/LICENSE` & `clinvar-tsv-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/PKG-INFO` & `clinvar-tsv-0.6.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,26 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+### [0.6.2](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.1...v0.6.2) (2023-06-21)
+
+
+### Bug Fixes
+
+* failure to determine location only goes to debug level ([#22](https://www.github.com/bihealth/clinvar-tsv/issues/22)) ([76bc510](https://www.github.com/bihealth/clinvar-tsv/commit/76bc5105e6f0b26146dcaca43465c1dd59d1aee2))
+* higher verbosity in Snakemake rules ([#26](https://www.github.com/bihealth/clinvar-tsv/issues/26)) ([a3fc327](https://www.github.com/bihealth/clinvar-tsv/commit/a3fc3271a8984b39d52c8852f6fe77b05b1193c0))
+* interpret --cores argument ([#24](https://www.github.com/bihealth/clinvar-tsv/issues/24)) ([3b09803](https://www.github.com/bihealth/clinvar-tsv/commit/3b098038c47fb33bffabf94510cc9b6fee3f7d43))
+* map "low penetrance" to "uncertain significance" ([#25](https://www.github.com/bihealth/clinvar-tsv/issues/25)) ([b2708d7](https://www.github.com/bihealth/clinvar-tsv/commit/b2708d75ad37d4270c253bf6928056c7deba8d84))
+* no verbose output by default ([#27](https://www.github.com/bihealth/clinvar-tsv/issues/27)) ([0ad10cb](https://www.github.com/bihealth/clinvar-tsv/commit/0ad10cb8122480d2f46fbb6d2fba1e063be6da3c))
+* reduce tqdm progress display unless on TTY ([#21](https://www.github.com/bihealth/clinvar-tsv/issues/21)) ([770b0c8](https://www.github.com/bihealth/clinvar-tsv/commit/770b0c833a2707a88e5ee9c0f2a0eb1435defdc6))
+
 ### [0.6.1](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.0...v0.6.1) (2023-06-21)
 
 
 ### Bug Fixes
 
 * missing/problematic clinvar version ([#19](https://www.github.com/bihealth/clinvar-tsv/issues/19)) ([b11a8a4](https://www.github.com/bihealth/clinvar-tsv/commit/b11a8a435d9269031589106cf8929169893db5ef))
```

### Comparing `clinvar-tsv-0.6.1/README.md` & `clinvar-tsv-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/Snakefile` & `clinvar-tsv-0.6.2/clinvar_tsv/Snakefile`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         b37_small="parsed/clinvar_table_raw.b37.tsv",
         b37_sv="parsed/clinvar_sv.b37.tsv",
         b38_small="parsed/clinvar_table_raw.b38.tsv",
         b38_sv="parsed/clinvar_sv.b38.tsv",
     shell:
         r"""
         set -euo pipefail
+        set -x
 
         clinvar_tsv parse_xml \
             --clinvar-xml {input.release_xml} \
             --output-b37-small {output.b37_small} \
             --output-b37-sv {output.b37_sv} \
             --output-b38-small {output.b38_small} \
             --output-b38-sv {output.b38_sv} \
@@ -58,14 +59,15 @@
     input:
         tsv="parsed/clinvar_table_raw.{genome_build}.tsv",
         reference=lambda wildcards: REF[wildcards.genome_build],
     output: "normalized/clinvar_table_normalized.{genome_build}.tsv.gz",
     shell:
         r"""
         set -euo pipefail
+        set -x
 
         clinvar_tsv normalize_tsv \
             --input-tsv {input.tsv} \
             --reference {input.reference} \
             --output-tsv /dev/stdout \
         | grep -v '^$' \
         | bgzip -c \
@@ -79,14 +81,15 @@
         tsv="unmerged/clinvar_small.{genome_build}.tsv.gz",
         tbi="unmerged/clinvar_small.{genome_build}.tsv.gz.tbi",
         tsv_md5="unmerged/clinvar_small.{genome_build}.tsv.gz.md5",
         tbi_md5="unmerged/clinvar_small.{genome_build}.tsv.gz.tbi.md5",
     shell:
         r"""
         set -euo pipefail
+        set -x
 
         cat \
             <(zcat {input} | head -n 1) \
             <(zcat {input} | tail -n +2 | sort -k2,2V -k3,3n -k4,4n -k11,11) \
         | bgzip -c \
         > {output.tsv}
         tabix -S 1 -s 2 -b 3 -e 4 -f {output.tsv}
@@ -104,14 +107,15 @@
         tsv_md5="unmerged/clinvar_sv.{genome_build}.tsv.gz.md5",
         tbi_md5="unmerged/clinvar_sv.{genome_build}.tsv.gz.tbi.md5",
     params:
         clinvar_version=config.get("clinvar_version", ".")
     shell:
         r"""
         set -euo pipefail
+        set -x
 
         cat \
             <(cat {input} | head -n 1) \
             <(cat {input} | tail -n +2 | sort -k2,2V -k3,3n -k4,4n -k11,11) \
         | bgzip -c \
         > {output.tsv}
         tabix -S 1 -s 2 -b 3 -e 4 -f {output.tsv}
@@ -129,14 +133,15 @@
         tsv_md5="output/clinvar_{size}.{genome_build}.tsv.gz.md5",
         tbi_md5="output/clinvar_{size}.{genome_build}.tsv.gz.tbi.md5",
     params:
         clinvar_version=config.get("clinvar_version", ".")
     shell:
         r"""
         set -euo pipefail
+        set -x
 
         zcat {input} \
         | clinvar_tsv merge_tsvs \
             --clinvar-version {params.clinvar_version} \
             --input-tsv /dev/stdin \
             --output-tsv /dev/stdout \
         | bgzip -c \
```

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/__main__.py` & `clinvar-tsv-0.6.2/clinvar_tsv/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         "config": {
             "b37_path": args.b37_path,
             "b38_path": args.b38_path,
             "debug": args.debug,
             "clinvar_version": args.clinvar_version,
         },
         "printshellcmds": True,
-        "verbose": True,
+        "verbose": args.verbose,
         "force_incomplete": True,
-        "cores": 8,
+        "cores": args.cores,
     }
     print(f"Running snakemake {kwargs}")
     return not snakemake.snakemake(**kwargs)
 
 
 def open_maybe_gzip(path, mode):
     if path.endswith(".gz"):
@@ -111,21 +111,24 @@
 
     # -----------------------------------------------------------------------
     # Command: main
     # -----------------------------------------------------------------------
 
     parser_main = subparsers.add_parser("main", help="Run the full process pipeline")
     parser_main.add_argument(
+        "--verbose", default=False, action="store_true", help="Enable verbose output"
+    )
+    parser_main.add_argument(
         "--b37-path", required=True, help="Path to GRCh37 FAI-indexed FASTA file."
     )
     parser_main.add_argument(
         "--b38-path", required=True, help="Path to GRCh38 FAI-indexed FASTA file."
     )
     parser_main.add_argument("--work-dir", default=os.getcwd(), help="Path to working directory")
-    parser_main.add_argument("--cores", default=1, type=int, help="Number of cores to use")
+    parser_main.add_argument("--cores", default=8, type=int, help="Number of cores to use")
     parser_main.add_argument(
         "--debug", default=False, action="store_true", help="Enables debugging helps"
     )
     parser_main.add_argument(
         "--clinvar-version", required=True, help="String to put as clinvar version"
     )
     parser_main.set_defaults(func=run_main)
```

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/common.py` & `clinvar-tsv-0.6.2/clinvar_tsv/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,14 +554,15 @@
         "risk factor",
         "uncertain",
         "unknown",
         "untested",
         "variant of unknown significance",
         "associated with leiomyomas",
         "conflicting data from submitters",
+        "low penetrance",
     ),
     1: (
         "likely pathogenic",
         # below: other
         "affects",
         "association",
         "confers sensitivity",
```

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/merge_tsvs.py` & `clinvar-tsv-0.6.2/clinvar_tsv/merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/normalize.py` & `clinvar-tsv-0.6.2/clinvar_tsv/normalize.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv/parse_clinvar_xml.py` & `clinvar-tsv-0.6.2/clinvar_tsv/parse_clinvar_xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Reference on clinvar XML tag:
 
 - ftp://ftp.ncbi.nlm.nih.gov/pub/clinvar/clinvar_submission.xsd
 - ftp://ftp.ncbi.nlm.nih.gov/pub/clinvar/tab_delimited/README
 """
 
 import json
+import sys
 import xml.etree.ElementTree as ET
 
 import binning
 import cattr
 from logzero import logger
 import tqdm
 
@@ -77,15 +78,17 @@
         out_files = {
             "GRCh37": {"small": self.out_b37_small, "sv": self.out_b37_sv},
             "GRCh38": {"small": self.out_b38_small, "sv": self.out_b38_sv},
         }
         for d in out_files.values():
             for out_file in d.values():
                 print(TSV_HEADER, file=out_file)
-        with tqdm.tqdm(unit="rcvs") as progress:
+        # Reduce the progress bar refresh rate if we're not in a TTY
+        mininterval = 0.1 if sys.stdout.isatty() else 60
+        with tqdm.tqdm(unit="rcvs", mininterval=mininterval) as progress:
             for event, elem in ET.iterparse(self.input):
                 if elem.tag == "ClinVarSet" and event == "end":
                     self.rcvs += 1
                     clinvar_set = ClinVarSet.from_element(elem)
                     if clinvar_set.ref_cv_assertion.observed_in:
                         origin = clinvar_set.ref_cv_assertion.observed_in.origin
                     else:
@@ -118,15 +121,15 @@
                                                     location.outer_stop,
                                                     location.inner_stop,
                                                 ),
                                                 int,
                                                 TypeError,
                                             )
                                         except TypeError:
-                                            logger.info(
+                                            logger.debug(
                                                 "Cannot determine location from %s", measure
                                             )
                                             continue
                                         row = [
                                             build,
                                             location.chrom,
                                             start,
```

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv.egg-info/PKG-INFO` & `clinvar-tsv-0.6.2/clinvar_tsv.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-tsv
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python 3 library for accessing and managing BioMedical sheets
 Home-page: https://github.com/bihealth/clinvar-tsv
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,26 @@
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
 
 
 # Changelog
 
+### [0.6.2](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.1...v0.6.2) (2023-06-21)
+
+
+### Bug Fixes
+
+* failure to determine location only goes to debug level ([#22](https://www.github.com/bihealth/clinvar-tsv/issues/22)) ([76bc510](https://www.github.com/bihealth/clinvar-tsv/commit/76bc5105e6f0b26146dcaca43465c1dd59d1aee2))
+* higher verbosity in Snakemake rules ([#26](https://www.github.com/bihealth/clinvar-tsv/issues/26)) ([a3fc327](https://www.github.com/bihealth/clinvar-tsv/commit/a3fc3271a8984b39d52c8852f6fe77b05b1193c0))
+* interpret --cores argument ([#24](https://www.github.com/bihealth/clinvar-tsv/issues/24)) ([3b09803](https://www.github.com/bihealth/clinvar-tsv/commit/3b098038c47fb33bffabf94510cc9b6fee3f7d43))
+* map "low penetrance" to "uncertain significance" ([#25](https://www.github.com/bihealth/clinvar-tsv/issues/25)) ([b2708d7](https://www.github.com/bihealth/clinvar-tsv/commit/b2708d75ad37d4270c253bf6928056c7deba8d84))
+* no verbose output by default ([#27](https://www.github.com/bihealth/clinvar-tsv/issues/27)) ([0ad10cb](https://www.github.com/bihealth/clinvar-tsv/commit/0ad10cb8122480d2f46fbb6d2fba1e063be6da3c))
+* reduce tqdm progress display unless on TTY ([#21](https://www.github.com/bihealth/clinvar-tsv/issues/21)) ([770b0c8](https://www.github.com/bihealth/clinvar-tsv/commit/770b0c833a2707a88e5ee9c0f2a0eb1435defdc6))
+
 ### [0.6.1](https://www.github.com/bihealth/clinvar-tsv/compare/v0.6.0...v0.6.1) (2023-06-21)
 
 
 ### Bug Fixes
 
 * missing/problematic clinvar version ([#19](https://www.github.com/bihealth/clinvar-tsv/issues/19)) ([b11a8a4](https://www.github.com/bihealth/clinvar-tsv/commit/b11a8a435d9269031589106cf8929169893db5ef))
```

### Comparing `clinvar-tsv-0.6.1/clinvar_tsv.egg-info/SOURCES.txt` & `clinvar-tsv-0.6.2/clinvar_tsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/setup.cfg` & `clinvar-tsv-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/setup.py` & `clinvar-tsv-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/conftest.py` & `clinvar-tsv-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/clinvar-74722873.xml` & `clinvar-tsv-0.6.2/tests/data/clinvar-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/clinvar-92148661.xml` & `clinvar-tsv-0.6.2/tests/data/clinvar-92148661.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/clinvar-in-context-74722873.xml` & `clinvar-tsv-0.6.2/tests/data/clinvar-in-context-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/clinvar-spta1.xml` & `clinvar-tsv-0.6.2/tests/data/clinvar-spta1.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/parsed-74722873.37.tsv` & `clinvar-tsv-0.6.2/tests/data/parsed-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/parsed-in-context-74722873.37.tsv` & `clinvar-tsv-0.6.2/tests/data/parsed-in-context-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/data/parsed-spta1.37.tsv` & `clinvar-tsv-0.6.2/tests/data/parsed-spta1.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/test_merge_tsvs.py` & `clinvar-tsv-0.6.2/tests/test_merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/test_parse_xml_small.py` & `clinvar-tsv-0.6.2/tests/test_parse_xml_small.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/tests/test_parse_xml_sv.py` & `clinvar-tsv-0.6.2/tests/test_parse_xml_sv.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.6.1/versioneer.py` & `clinvar-tsv-0.6.2/versioneer.py`

 * *Files identical despite different names*

