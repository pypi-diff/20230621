# Comparing `tmp/clld_morphology_plugin-0.0.8.tar.gz` & `tmp/clld_morphology_plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clld_morphology_plugin-0.0.8.tar", last modified: Sun Jun 18 05:56:22 2023, max compression
+gzip compressed data, was "dist/clld_morphology_plugin-0.0.9.tar", last modified: Wed Jun 21 09:11:23 2023, max compression
```

## Comparing `clld_morphology_plugin-0.0.8.tar` & `clld_morphology_plugin-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2023-06-18 05:56:14.000000 clld_morphology_plugin-0.0.8/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.8/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       96 2022-11-06 02:18:58.000000 clld_morphology_plugin-0.0.8/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     4621 2023-02-27 21:55:48.000000 clld_morphology_plugin-0.0.8/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      555 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.8/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1746 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.8/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3168 2023-06-18 05:55:06.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/__init__.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     8511 2023-03-26 15:39:42.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/datatables.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      942 2023-02-23 22:32:53.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/interfaces.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    22443 2023-03-26 15:39:42.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/models.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/static/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-05-28 17:41:45.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/static/clld-morphology.css
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1332 2023-03-26 16:41:39.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      258 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3400 2023-03-07 22:54:59.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/gloss/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2725 2023-03-26 15:38:27.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/gloss/detail_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      580 2023-03-26 15:36:33.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      317 2023-03-07 06:12:04.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1894 2023-03-07 22:55:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      309 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2719 2023-03-07 22:55:32.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-06-06 03:10:04.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      790 2023-03-07 22:55:44.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      288 2021-12-26 08:07:46.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     6615 2023-03-07 22:53:56.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      243 2022-02-23 14:45:24.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5737 2023-03-07 22:55:37.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-03-13 15:46:33.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/index_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-05-10 14:17:26.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphology_util.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      625 2023-03-07 22:55:16.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      345 2023-02-23 22:42:05.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1172 2023-03-07 22:55:10.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-05-31 20:53:58.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2128 2023-06-14 22:03:57.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     6266 2023-03-07 22:54:21.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      249 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/index_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    13923 2023-06-09 23:08:57.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/util.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2297 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      224 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       23 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2023-06-21 09:11:14.000000 clld_morphology_plugin-0.0.9/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.9/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       96 2022-11-06 02:18:58.000000 clld_morphology_plugin-0.0.9/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     4621 2023-02-27 21:55:48.000000 clld_morphology_plugin-0.0.9/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      555 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.9/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1746 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.9/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3168 2023-06-21 09:10:16.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     9799 2023-06-20 17:55:30.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/datatables.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      942 2023-02-23 22:32:53.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/interfaces.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    23038 2023-06-20 15:49:24.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/models.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/static/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-05-28 17:41:45.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/static/clld-morphology.css
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/derivationalprocess/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1332 2023-03-26 16:41:39.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      258 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/derivationalprocess/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/form/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3400 2023-03-07 22:54:59.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/form/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/form/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/gloss/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2725 2023-03-26 15:38:27.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/gloss/detail_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalcategory/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      580 2023-03-26 15:36:33.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      317 2023-03-07 06:12:04.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalcategory/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalvalue/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1894 2023-03-07 22:55:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      309 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalvalue/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/lexeme/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2719 2023-03-07 22:55:32.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/lexeme/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-06-06 03:10:04.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/lexeme/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/meaning/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      790 2023-03-07 22:55:44.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/meaning/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      288 2021-12-26 08:07:46.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/meaning/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morph/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6780 2023-06-20 18:24:02.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morph/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      243 2022-02-23 14:45:24.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morph/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morpheme/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5737 2023-03-07 22:55:37.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morpheme/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-03-13 15:46:33.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morpheme/index_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-05-10 14:17:26.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphology_util.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphophonologicalchange/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      625 2023-03-07 22:55:16.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      345 2023-02-23 22:42:05.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphophonologicalchange/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/pos/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1628 2023-06-20 20:48:10.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/pos/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-05-31 20:53:58.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/pos/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/stem/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2128 2023-06-14 22:03:57.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/stem/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/stem/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/wordform/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6266 2023-03-07 22:54:21.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/wordform/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      249 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/wordform/index_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    13923 2023-06-09 23:08:57.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/util.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2297 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      224 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       23 2023-06-21 09:11:23.000000 clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/top_level.txt
```

### Comparing `clld_morphology_plugin-0.0.8/LICENSE` & `clld_morphology_plugin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/PKG-INFO` & `clld_morphology_plugin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld_morphology_plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Short description of package.
 Home-page: https://github.com/fmatter/clld-morphology-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-morphology-plugin/issues
 Keywords: web,pyramid,pylons
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_morphology_plugin-0.0.8/README.md` & `clld_morphology_plugin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/pyproject.toml` & `clld_morphology_plugin-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/setup.cfg` & `clld_morphology_plugin-0.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	pylons
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = clld_morphology_plugin
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/clld-morphology-plugin/issues
 url = https://github.com/fmatter/clld-morphology-plugin
-version = 0.0.8
+version = 0.0.9
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/__init__.py` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from clld_morphology_plugin import datatables
 from clld_morphology_plugin import interfaces
 from clld_morphology_plugin import models
 
 
 __author__ = "Florian Matter"
 __email__ = "florianmatter@gmail.com"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def includeme(config):
     config.registry.settings["mako.directories"].insert(
         1, "clld_morphology_plugin:templates"
     )
     config.add_static_view(
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/datatables.py` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/datatables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from clld.db.models.common import Language
+from clld.db.models.common import Language, Contribution
 from clld.web.datatables.base import Col
 from clld.web.datatables.base import DataTable
 from clld.web.datatables.base import LinkCol
 from clld.web.util.helpers import icon
 from sqlalchemy import and_
 from sqlalchemy.orm import joinedload
 from clld_morphology_plugin import models
@@ -45,14 +45,15 @@
         return True
 
 
 class Wordforms(DataTable):
 
     __constraints__ = [
         Language,
+        Contribution,
         models.Lexeme,
         models.Morph,
         models.POS,
         models.Inflection,
         models.Stem,
     ]
 
@@ -74,14 +75,16 @@
                 joinedload(models.Wordform.slices)
             )
             return query.filter(
                 models.Wordform.slices.any(models.WordformPart.morph == self.morph)
             )
         if self.language:
             return query.filter(models.Wordform.language == self.language)
+        if self.contribution:
+            return query.filter(models.Wordform.contribution_pk == self.contribution.pk)
         if self.stem:
             return query.filter(
                 models.Wordform.formstems.any(models.WordformStem.stem == self.stem)
             )
         if self.pos:
             return query.filter(models.Wordform.pos == self.pos)
         if self.lexeme:
@@ -126,21 +129,23 @@
             )
         cols.append(AudioCol(self, "Audio"))
         return cols
 
 
 class Forms(DataTable):
 
-    __constraints__ = [Language, models.Wordform]
+    __constraints__ = [Language, models.Wordform, Contribution]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Form.language))
 
         if self.language:
             return query.filter(models.Form.language == self.language)
+        if self.contribution:
+            return query.filter(models.Form.contribution_pk == self.contribution.pk)
         if self.wordform:
             query = query.join(models.FormPart).options(
                 joinedload(models.Form.formslices)
             )
             return query.filter(
                 models.Form.formslices.any(models.FormPart.wordform == self.wordform)
             )
@@ -154,63 +159,83 @@
                 self, "language", model_col=Language.name, get_obj=lambda i: i.language
             ),
         ]
 
 
 class Morphs(DataTable):
 
-    __constraints__ = [Language]
+    __constraints__ = [Language, models.POS, Contribution]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Morph.language))
 
         if self.language:
             return query.filter(models.Morph.language == self.language)
+        if self.pos:
+            return query.filter(models.Morph.pos == self.pos)
+        if self.contribution:
+            return query.filter(models.Morph.contribution_pk == self.contribution.pk)
+
         return query
 
     def col_defs(self):
-        return [
+        cols = [
             LinkCol(self, "name"),
             Col(self, "description"),
             LinkCol(
                 self, "language", model_col=Language.name, get_obj=lambda i: i.language
             ),
             Col(self, "morph_type", choices=["prefix", "suffix", "root", "infix"]),
         ]
+        if not self.pos:
+            cols.append(
+                LinkCol(
+                    self,
+                    "part of speech",
+                    # model_col=models.POS.name,
+                    get_obj=lambda i: i.pos,
+                )
+            )
+        return cols
+
 
 
 class Morphemes(DataTable):
-    __constraints__ = [Language]
+    __constraints__ = [Language, Contribution]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Morpheme.language))
 
         if self.language:
             return query.filter(models.Morpheme.language == self.language)
+        if self.contribution:
+            return query.filter(models.Morpheme.contribution_pk == self.contribution.pk)
         return query
 
     def col_defs(self):
         return [
             LinkCol(self, "name"),
             Col(self, "description"),
             LinkCol(
                 self, "language", model_col=Language.name, get_obj=lambda i: i.language
             ),
         ]
 
 
 class Stems(DataTable):
-    __constraints__ = [Language, models.Morph]
+    __constraints__ = [Language, Contribution, models.Morph]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Stem.language))
         query = query.join(models.StemPart).options(joinedload(models.Stem.slices))
 
         if self.language:
             return query.filter(models.Stem.language == self.language)
+        if self.contribution:
+            return query.filter(models.Stem.contribution_pk == self.contribution.pk)
         if self.morph:
             return query.filter(
                 models.Stem.slices.any(models.StemPart.morph == self.morph)
             )
         return query
 
     def col_defs(self):
@@ -250,19 +275,23 @@
 
 class Glosses(DataTable):
     def col_defs(self):
         return [LinkCol(self, "name")]
 
 
 class Lexemes(DataTable):
-    __constraints__ = [Language, models.POS]
+    __constraints__ = [Language, models.POS, Contribution]
 
     def base_query(self, query):
         if self.pos:
             return query.filter(models.Lexeme.pos == self.pos)
+        if self.contribution:
+            return query.filter(models.Lexeme.contribution_pk == self.contribution.pk)
+        if self.language:
+            return query.filter(models.Lexeme.language == self.language)
         return query
 
     def col_defs(self):
         cols = [
             LinkCol(self, "name"),
             Col(self, "description"),
             # FormCountCol(self, "Forms", bSortable=False, bSearchable=False),
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/interfaces.py` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/interfaces.py`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/models.py` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,35 +101,48 @@
         """A list of inflectional values expressed with morphs belonging to this morpheme."""
         vallist = []
         for m in self.allomorphs:
             for val in m.inflectionalvalues:
                 vallist.append(val)
         return list(set(vallist))
 
+@implementer(interfaces.IPOS)
+class POS(Base, IdNameDescriptionMixin):
+    """A part of speech is a language-specific open or closed set of wordforms (or lexemes)"""
+
+    language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
+    language = relationship(Language, innerjoin=True)
+
 
 @implementer(interfaces.IMorph)
 class Morph(Base, PolymorphicBaseMixin, IdNameDescriptionMixin, HasSourceMixin):
     """A morph is a pairing of a sequence of segments and function, which can not be further segmented."""
 
     __table_args__ = (
         UniqueConstraint("language_pk", "id"),
         UniqueConstraint("morpheme_pk", "id"),
     )
 
+    contribution_pk = Column(Integer, ForeignKey("contribution.pk"))
+    contribution = relationship(Contribution, backref="morphs")
+
     language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
     language = relationship(Language, innerjoin=True)
     morpheme_pk = Column(Integer, ForeignKey("morpheme.pk"), nullable=True)
     morpheme = relationship(Morpheme, innerjoin=True, backref="allomorphs")
     """The right-hand separator for this morph (e.g.: ``-`` or ``>``)"""
     rsep = Column(String, nullable=True)
     """The right-hand separator for this morph (e.g.: ``-`` or ``>``)"""
     lsep = Column(String, nullable=True)
     """The morph type (e.g.: ``root`` or ``prefix``)"""
     morph_type = Column(String, nullable=True)
 
+    pos_pk = Column(Integer, ForeignKey("pos.pk"), nullable=True)
+    pos = relationship(POS, backref="morphs", innerjoin=True)
+
     @property
     def glosses(self):
         """A list of gloss sets that tokens of this morph have."""
         glosslist = []
         for fslice in self.formslices:
             g = [x.gloss for x in fslice.glosses]
             if g not in glosslist:
@@ -153,22 +166,14 @@
         for x in self.stemslices:
             for form in x.stem.wordforms:
                 if form not in formlist:
                     formlist.append(form)
         return formlist
 
 
-@implementer(interfaces.IPOS)
-class POS(Base, IdNameDescriptionMixin):
-    """A part of speech is a language-specific open or closed set of wordforms (or lexemes)"""
-
-    language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
-    language = relationship(Language, innerjoin=True)
-
-
 @implementer(interfaces.IWordform)
 class Wordform(
     Base, PolymorphicBaseMixin, IdNameDescriptionMixin, HasSourceMixin, HasFilesMixin
 ):
     """A wordform is a grammatical or morphosyntactic word. It can have a stem and bear inflectional morphology."""
 
     __table_args__ = (
@@ -310,14 +315,17 @@
 
 @implementer(interfaces.ILexeme)
 class Lexeme(Base, IdNameDescriptionMixin):
     """ "A lexeme is a 'dictionary entry'."""
 
     __table_args__ = (UniqueConstraint("language_pk", "id"),)
 
+    contribution_pk = Column(Integer, ForeignKey("contribution.pk"))
+    contribution = relationship(Contribution, backref="lexemes")
+
     language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
     language = relationship(Language, innerjoin=True)
 
     pos_pk = Column(Integer, ForeignKey("pos.pk"), nullable=True)
     pos = relationship(POS, backref="lexemes", innerjoin=True)
 
     comment = Column(Unicode)
@@ -349,18 +357,25 @@
     """A stem is the part of a wordform that is not inflected. It is associated with a lexeme, and is potentially morphologically complex."""
 
     __table_args__ = (UniqueConstraint("language_pk", "id"),)
 
     language_pk = Column(Integer, ForeignKey("language.pk"), nullable=False)
     language = relationship(Language, innerjoin=True)
 
+    contribution_pk = Column(Integer, ForeignKey("contribution.pk"))
+    contribution = relationship(Contribution, backref="stems")
+
     lexeme_pk = Column(Integer, ForeignKey("lexeme.pk"))
     lexeme = relationship(Lexeme, innerjoin=True, backref="stems")
     comment = Column(Unicode)
 
+    @property
+    def pos(self):
+        return self.lexeme.pos
+
     """The parts into which this stem can be segmented. Note that these are not necessarily morphs, as 1) there may be segments that have no meaning attached to them, 2) parts may be other stems which could be further segmentable, and 3) morphs split by infixation appear as two separate parts."""
     parts = Column(MutableList.as_mutable(PickleType), default=[])
 
     rsep = Column(String, nullable=True)
     lsep = Column(String, nullable=True)
 
     @property
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/form/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/gloss/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/gloss/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/lexeme/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/meaning/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morph/detail_html.mako`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,20 @@
                 ${h.link(request, ctx.contribution)} by
 % for contributor in ctx.contribution.primary_contributors:
 ${h.link(request, contributor)}
 % endfor
             </td>
         </tr>
         % endif
+        % if ctx.source:
+            <tr>
+                <td>Source:</td>
+                <td>${h.link(request, ctx.source)}</td>
+            </tr>
+        % endif
     </tbody>
 </table>
 
 <p>${h.text2html(h.Markup(ctx.markup_description or ""))}</p>
 
 <% gloss_sentences = {} %>
```

#### html2text {}

```diff
@@ -23,14 +23,15 @@
                        <% cogsets = [] %> % for c in ctx.cognates: % if
 Cognate set(s):        c.cognateset not in cogsets: <% cogsets.append
                        (c.cognateset) %> % endif % endfor ${h.text2html
                        ("*"+"+".join([h.link(request, c) for c in cogsets]))}
                        ${h.link(request, ctx.contribution)} by % for
 Contribution:          contributor in ctx.contribution.primary_contributors: $
                        {h.link(request, contributor)} % endfor
+Source:                ${h.link(request, ctx.source)}
 ${h.text2html(h.Markup(ctx.markup_description or ""))}
 <% gloss_sentences = {} %> % for fslice in ctx.formslices: % if hasattr
 (fslice.form, "sentence_assocs") and fslice.form.sentence_assocs: <% gloss =
 ".".join([str(x.gloss) for x in fslice.glosses]) %> <%
 gloss_sentences.setdefault(gloss, []) %> % for s in
 fslice.form.sentence_assocs: <% gloss_sentences[gloss].append(s.sentence) %> %
 endfor % endif % endfor % for sslice in ctx.stemslices: % for wf in
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morpheme/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphology_util.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphology_util.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/pos/detail_html.mako`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 % if ctx.description:
     <p>${ctx.description}</p>
 % endif
 
 <div class="tabbable">
     <ul class="nav nav-tabs">
         % if ctx.wordforms:
-            <li class='active'><a href="#forms" data-toggle="tab"> Wordforms </a></li>
+            <li class='active'><a href="#wordforms" data-toggle="tab"> Wordforms </a></li>
         % endif
         % if ctx.lexemes:
             <li class=${'' if ctx.wordforms else 'active'}><a href="#lexemes" data-toggle="tab"> Lexemes </a></li>
         % endif
+        % if ctx.morphs:
+            <li class=${'' if (ctx.lexemes + ctx.wordforms) else 'active'}><a href="#morphs" data-toggle="tab"> Morphs </a></li>
+        % endif
     </ul>
 
     <div class="tab-content" style="overflow: visible;">
 
-        <div id="forms" class="tab-pane active">
+        <div id="wordforms" class="tab-pane ${'active' if ctx.wordforms else ''}">
             ${request.get_datatable('wordforms', models.Wordform, pos=ctx).render()}
         </div>
 
-        <div id="lexemes" class="tab-pane ${'' if ctx.wordforms else 'active'}">
-            ${request.get_datatable('lexemes',models.Lexeme, pos=ctx).render()}
+        <div id="lexemes" class="tab-pane ${'' if (ctx.wordforms) else 'active'}">
+            % if ctx.wordforms:
+                ${request.get_datatable('lexemes',models.Lexeme, pos=ctx).render()}
+            % endif
+        </div>
+
+        <div id="morphs" class="tab-pane ${'' if (ctx.wordforms + ctx.lexemes) else 'active'}">
+            ${request.get_datatable('morphs',models.Morph, pos=ctx).render()}
         </div>
 
     </div>  
 </div>
 
 <p>${h.text2html(h.Markup(ctx.markup_description or ""))}</p>
```

#### html2text {}

```diff
@@ -6,11 +6,15 @@
 % if ctx.description:
 ${ctx.description}
 % endif
     * % if ctx.wordforms:
     * Wordforms
     * % endif % if ctx.lexemes:
     * wordforms else 'active'}>Lexemes
+% endif % if ctx.morphs:
+ctx.lexemes + ctx.wordforms) else 'active'}>Morphs
 % endif
 ${request.get_datatable('wordforms', models.Wordform, pos=ctx).render()}
-${request.get_datatable('lexemes',models.Lexeme, pos=ctx).render()}
+% if ctx.wordforms: ${request.get_datatable('lexemes',models.Lexeme,
+pos=ctx).render()} % endif
+${request.get_datatable('morphs',models.Morph, pos=ctx).render()}
 ${h.text2html(h.Markup(ctx.markup_description or ""))}
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/stem/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/detail_html.mako` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/templates/wordform/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/util.py` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin/util.py`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/PKG-INFO` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld-morphology-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Short description of package.
 Home-page: https://github.com/fmatter/clld-morphology-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-morphology-plugin/issues
 Keywords: web,pyramid,pylons
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/SOURCES.txt` & `clld_morphology_plugin-0.0.9/src/clld_morphology_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

