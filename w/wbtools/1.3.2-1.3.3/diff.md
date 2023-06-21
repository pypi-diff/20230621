# Comparing `tmp/wbtools-1.3.2.tar.gz` & `tmp/wbtools-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbtools-1.3.2.tar", last modified: Thu Aug 11 17:57:10 2022, max compression
+gzip compressed data, was "wbtools-1.3.3.tar", last modified: Wed Jun 21 15:34:18 2023, max compression
```

## Comparing `wbtools-1.3.2.tar` & `wbtools-1.3.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1060 2021-09-21 20:01:07.000000 wbtools-1.3.2/LICENSE
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2813 2022-08-11 17:57:10.527550 wbtools-1.3.2/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2306 2022-03-11 05:13:49.000000 wbtools-1.3.2/README.md
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2022-08-11 17:57:10.527550 wbtools-1.3.2/setup.cfg
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1034 2022-08-11 16:33:02.000000 wbtools-1.3.2/setup.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.519549 wbtools-1.3.2/tests/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      686 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/config_reader.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.519549 wbtools-1.3.2/tests/db/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/db/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1050 2021-10-13 16:58:22.000000 wbtools-1.3.2/tests/db/test_afp.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1061 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/db/test_antibody.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1025 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/db/test_expression.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1915 2022-03-11 05:13:49.000000 wbtools-1.3.2/tests/db/test_generic.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/tests/lib/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/tests/lib/entity_extraction/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/entity_extraction/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1923 2022-03-11 05:13:49.000000 wbtools-1.3.2/tests/lib/entity_extraction/test_email_addresses.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2342 2021-10-01 23:54:11.000000 wbtools-1.3.2/tests/lib/entity_extraction/test_generic.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2455 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/entity_extraction/test_new_variations.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1178 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/test_literature_index.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      510 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/test_scraping.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2803 2022-03-11 05:13:49.000000 wbtools-1.3.2/tests/lib/test_text_preprocessing.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2148 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/lib/test_text_similarity.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/tests/literature/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/tests/literature/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     6196 2022-06-24 02:07:29.000000 wbtools-1.3.2/tests/literature/test_corpus.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     8408 2022-03-11 05:13:49.000000 wbtools-1.3.2/tests/literature/test_paper.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/wbtools/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/wbtools/db/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3317 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/abstract_manager.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    74360 2022-08-11 16:19:01.000000 wbtools-1.3.2/wbtools/db/afp.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1526 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/antibody.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1877 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/dbmanager.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      528 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/expression.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2399 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/db/gene.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    15770 2021-10-01 16:17:39.000000 wbtools-1.3.2/wbtools/db/generic.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     7164 2021-10-01 16:57:39.000000 wbtools-1.3.2/wbtools/db/paper.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     5930 2022-01-24 21:54:08.000000 wbtools-1.3.2/wbtools/db/person.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/lib/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/lib/email/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/email/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1203 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/email/generic.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/lib/nlp/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1881 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/common.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      684 2022-03-08 18:09:18.000000 wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/email_addresses.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     9003 2021-10-01 16:15:02.000000 wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/ntt_extractor.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      764 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/variations.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/lib/nlp/literature_index/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/literature_index/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      310 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/literature_index/abstract_index.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2624 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/literature_index/textpresso.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3924 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/text_preprocessing.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1652 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/nlp/text_similarity.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     4175 2022-03-11 05:13:49.000000 wbtools-1.3.2/wbtools/lib/scraping.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      581 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/lib/timeout.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.527550 wbtools-1.3.2/wbtools/literature/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/literature/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    15517 2022-03-11 05:13:49.000000 wbtools-1.3.2/wbtools/literature/corpus.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    19080 2022-06-24 01:58:48.000000 wbtools-1.3.2/wbtools/literature/paper.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1941 2021-09-21 20:01:07.000000 wbtools-1.3.2/wbtools/literature/person.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-08-11 17:57:10.523550 wbtools-1.3.2/wbtools.egg-info/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2813 2022-08-11 17:57:10.000000 wbtools-1.3.2/wbtools.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1737 2022-08-11 17:57:10.000000 wbtools-1.3.2/wbtools.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2022-08-11 17:57:10.000000 wbtools-1.3.2/wbtools.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      155 2022-08-11 17:57:10.000000 wbtools-1.3.2/wbtools.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       14 2022-08-11 17:57:10.000000 wbtools-1.3.2/wbtools.egg-info/top_level.txt
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.010314 wbtools-1.3.3/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1060 2021-09-21 20:01:07.000000 wbtools-1.3.3/LICENSE
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2813 2023-06-21 15:34:18.010314 wbtools-1.3.3/PKG-INFO
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2306 2022-03-11 05:13:49.000000 wbtools-1.3.3/README.md
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2023-06-21 15:34:18.010314 wbtools-1.3.3/setup.cfg
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1034 2023-06-21 15:20:42.000000 wbtools-1.3.3/setup.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.002314 wbtools-1.3.3/tests/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      686 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/config_reader.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/tests/db/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/db/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1050 2021-10-13 16:58:22.000000 wbtools-1.3.3/tests/db/test_afp.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1061 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/db/test_antibody.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1025 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/db/test_expression.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1915 2022-03-11 05:13:49.000000 wbtools-1.3.3/tests/db/test_generic.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/tests/lib/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/tests/lib/entity_extraction/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/entity_extraction/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1923 2022-03-11 05:13:49.000000 wbtools-1.3.3/tests/lib/entity_extraction/test_email_addresses.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2342 2021-10-01 23:54:11.000000 wbtools-1.3.3/tests/lib/entity_extraction/test_generic.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2455 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/entity_extraction/test_new_variations.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1178 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/test_literature_index.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      510 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/test_scraping.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2803 2022-03-11 05:13:49.000000 wbtools-1.3.3/tests/lib/test_text_preprocessing.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2148 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/lib/test_text_similarity.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/tests/literature/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/tests/literature/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     6196 2022-06-24 02:07:29.000000 wbtools-1.3.3/tests/literature/test_corpus.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     8408 2022-03-11 05:13:49.000000 wbtools-1.3.3/tests/literature/test_paper.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools/db/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     3317 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/abstract_manager.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    74398 2023-06-21 15:19:44.000000 wbtools-1.3.3/wbtools/db/afp.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1526 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/antibody.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1877 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/dbmanager.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      528 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/expression.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2399 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/db/gene.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    15770 2021-10-01 16:17:39.000000 wbtools-1.3.3/wbtools/db/generic.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     7164 2021-10-01 16:57:39.000000 wbtools-1.3.3/wbtools/db/paper.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     5930 2022-01-24 21:54:08.000000 wbtools-1.3.3/wbtools/db/person.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools/lib/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools/lib/email/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/email/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1203 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/email/generic.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools/lib/nlp/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1881 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/common.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.010314 wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      684 2022-03-08 18:09:18.000000 wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/email_addresses.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     9003 2021-10-01 16:15:02.000000 wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/ntt_extractor.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      764 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/variations.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.010314 wbtools-1.3.3/wbtools/lib/nlp/literature_index/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/literature_index/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      310 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/literature_index/abstract_index.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2624 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/literature_index/textpresso.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     3924 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/text_preprocessing.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1652 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/nlp/text_similarity.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     4175 2022-03-11 05:13:49.000000 wbtools-1.3.3/wbtools/lib/scraping.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      581 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/lib/timeout.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.010314 wbtools-1.3.3/wbtools/literature/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/literature/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    15517 2022-03-11 05:13:49.000000 wbtools-1.3.3/wbtools/literature/corpus.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    19080 2022-06-24 01:58:48.000000 wbtools-1.3.3/wbtools/literature/paper.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1941 2021-09-21 20:01:07.000000 wbtools-1.3.3/wbtools/literature/person.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2023-06-21 15:34:18.006314 wbtools-1.3.3/wbtools.egg-info/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2813 2023-06-21 15:34:17.000000 wbtools-1.3.3/wbtools.egg-info/PKG-INFO
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1737 2023-06-21 15:34:18.000000 wbtools-1.3.3/wbtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2023-06-21 15:34:17.000000 wbtools-1.3.3/wbtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      155 2023-06-21 15:34:17.000000 wbtools-1.3.3/wbtools.egg-info/requires.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)       14 2023-06-21 15:34:17.000000 wbtools-1.3.3/wbtools.egg-info/top_level.txt
```

### Comparing `wbtools-1.3.2/LICENSE` & `wbtools-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/PKG-INFO` & `wbtools-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbtools
-Version: 1.3.2
+Version: 1.3.3
 Summary: Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP functions
 Home-page: https://github.com/WormBase/wbtools
 Author: Valerio Arnaboldi
 Author-email: valearna@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wbtools-1.3.2/README.md` & `wbtools-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/setup.py` & `wbtools-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wbtools",
-    version="1.3.2",
+    version="1.3.3",
     author="Valerio Arnaboldi",
     author_email="valearna@caltech.edu",
     description="Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP "
                 "functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WormBase/wbtools",
```

### Comparing `wbtools-1.3.2/tests/config_reader.py` & `wbtools-1.3.3/tests/config_reader.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/db/test_afp.py` & `wbtools-1.3.3/tests/db/test_afp.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/db/test_antibody.py` & `wbtools-1.3.3/tests/db/test_antibody.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/db/test_expression.py` & `wbtools-1.3.3/tests/db/test_expression.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/db/test_generic.py` & `wbtools-1.3.3/tests/db/test_generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/entity_extraction/test_email_addresses.py` & `wbtools-1.3.3/tests/lib/entity_extraction/test_email_addresses.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/entity_extraction/test_generic.py` & `wbtools-1.3.3/tests/lib/entity_extraction/test_generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/entity_extraction/test_new_variations.py` & `wbtools-1.3.3/tests/lib/entity_extraction/test_new_variations.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/test_literature_index.py` & `wbtools-1.3.3/tests/lib/test_literature_index.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/test_text_preprocessing.py` & `wbtools-1.3.3/tests/lib/test_text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/lib/test_text_similarity.py` & `wbtools-1.3.3/tests/lib/test_text_similarity.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/literature/test_corpus.py` & `wbtools-1.3.3/tests/literature/test_corpus.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/tests/literature/test_paper.py` & `wbtools-1.3.3/tests/literature/test_paper.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/abstract_manager.py` & `wbtools-1.3.3/wbtools/db/abstract_manager.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/afp.py` & `wbtools-1.3.3/wbtools/db/afp.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
         with self.get_cursor() as curs:
             person_db_manager = self.get_db_manager(cls=WBPersonDBManager)
             curs.execute("select afp_contributor.afp_contributor, count(DISTINCT afp_contributor.joinkey) from "
                          "afp_contributor join afp_lasttouched on afp_contributor.joinkey = afp_lasttouched.joinkey "
                          "join afp_version on afp_contributor.joinkey = afp_version.joinkey "
                          "where afp_version.afp_version = '2' "
                          "group by afp_contributor.afp_contributor order by count(DISTINCT afp_contributor.joinkey) "
-                         "desc OFFSET {} LIMIT {}".format(from_offset, count))
+                         "desc, afp_contributor.afp_contributor desc OFFSET {} LIMIT {}".format(from_offset, count))
             res = curs.fetchall()
             if res:
                 return [(person_db_manager.get_email(row[0]), row[1]) for row in res]
             else:
                 return []
 
     def get_num_unique_emailed_addresses(self):
```

### Comparing `wbtools-1.3.2/wbtools/db/antibody.py` & `wbtools-1.3.3/wbtools/db/antibody.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/dbmanager.py` & `wbtools-1.3.3/wbtools/db/dbmanager.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/expression.py` & `wbtools-1.3.3/wbtools/db/expression.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/gene.py` & `wbtools-1.3.3/wbtools/db/gene.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/generic.py` & `wbtools-1.3.3/wbtools/db/generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/paper.py` & `wbtools-1.3.3/wbtools/db/paper.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/db/person.py` & `wbtools-1.3.3/wbtools/db/person.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/email/generic.py` & `wbtools-1.3.3/wbtools/lib/email/generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/common.py` & `wbtools-1.3.3/wbtools/lib/nlp/common.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/email_addresses.py` & `wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/email_addresses.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/ntt_extractor.py` & `wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/ntt_extractor.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/entity_extraction/variations.py` & `wbtools-1.3.3/wbtools/lib/nlp/entity_extraction/variations.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/literature_index/textpresso.py` & `wbtools-1.3.3/wbtools/lib/nlp/literature_index/textpresso.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/text_preprocessing.py` & `wbtools-1.3.3/wbtools/lib/nlp/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/nlp/text_similarity.py` & `wbtools-1.3.3/wbtools/lib/nlp/text_similarity.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/scraping.py` & `wbtools-1.3.3/wbtools/lib/scraping.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/lib/timeout.py` & `wbtools-1.3.3/wbtools/lib/timeout.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/literature/corpus.py` & `wbtools-1.3.3/wbtools/literature/corpus.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/literature/paper.py` & `wbtools-1.3.3/wbtools/literature/paper.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools/literature/person.py` & `wbtools-1.3.3/wbtools/literature/person.py`

 * *Files identical despite different names*

### Comparing `wbtools-1.3.2/wbtools.egg-info/PKG-INFO` & `wbtools-1.3.3/wbtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbtools
-Version: 1.3.2
+Version: 1.3.3
 Summary: Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP functions
 Home-page: https://github.com/WormBase/wbtools
 Author: Valerio Arnaboldi
 Author-email: valearna@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wbtools-1.3.2/wbtools.egg-info/SOURCES.txt` & `wbtools-1.3.3/wbtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

