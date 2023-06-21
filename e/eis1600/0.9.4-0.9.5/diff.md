# Comparing `tmp/eis1600-0.9.4.tar.gz` & `tmp/eis1600-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.4.tar", last modified: Thu Jun  8 09:08:51 2023, max compression
+gzip compressed data, was "eis1600-0.9.5.tar", last modified: Wed Jun 21 13:43:08 2023, max compression
```

## Comparing `eis1600-0.9.4.tar` & `eis1600-0.9.5.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.148184 eis1600-0.9.4/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.4/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-08 09:08:51.148184 eis1600-0.9.4/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-06-08 08:10:00.000000 eis1600-0.9.4/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.132184 eis1600-0.9.4/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.4/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.4/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.4/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.4/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.4/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3448 2023-06-05 11:20:45.000000 eis1600-0.9.4/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.4/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.4/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.4/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-05 11:33:25.000000 eis1600-0.9.4/eis1600/gazetteers/data/toponyms_gazetteer.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.4/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.4/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.4/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.4/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.4/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.4/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.4/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.4/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.4/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.4/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.4/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11212 2023-06-08 08:03:01.000000 eis1600-0.9.4/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.4/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.4/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.4/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.4/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.4/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.4/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.4/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.4/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.4/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.4/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.4/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.4/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9595 2023-06-08 09:08:43.000000 eis1600-0.9.4/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.4/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8483 2023-05-26 10:07:04.000000 eis1600-0.9.4/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.4/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2935 2023-06-08 07:49:05.000000 eis1600-0.9.4/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.4/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6543 2023-06-08 07:58:41.000000 eis1600-0.9.4/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.4/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.4/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.4/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.4/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.4/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.4/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.4/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.4/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.4/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.148184 eis1600-0.9.4/eis1600/toponyms/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.4/eis1600/toponyms/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.4/eis1600/toponyms/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2959 2023-06-08 09:06:21.000000 eis1600-0.9.4/eis1600/toponyms/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      856 2023-06-07 09:48:13.000000 eis1600-0.9.4/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.132184 eis1600-0.9.4/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2050 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      800 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-08 09:08:51.148184 eis1600-0.9.4/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2372 2023-06-08 08:13:11.000000 eis1600-0.9.4/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.5/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-21 13:43:08.048154 eis1600-0.9.5/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-06-08 08:10:00.000000 eis1600-0.9.5/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.5/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.5/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.5/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.5/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.5/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3476 2023-06-14 10:59:59.000000 eis1600-0.9.5/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.5/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.032154 eis1600-0.9.5/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.5/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.5/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-14 10:40:04.000000 eis1600-0.9.5/eis1600/gazetteers/data/toponyms_gazetteer.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.036154 eis1600-0.9.5/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.5/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.5/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.5/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.5/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.036154 eis1600-0.9.5/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.5/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.5/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.5/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.5/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.5/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.5/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3152 2023-06-16 13:52:38.000000 eis1600-0.9.5/eis1600/helper/md_tags_to_bio.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.5/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11212 2023-06-08 08:03:01.000000 eis1600-0.9.5/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.5/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.5/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.040154 eis1600-0.9.5/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.5/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.5/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.5/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.5/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.5/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.5/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.040154 eis1600-0.9.5/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.5/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.5/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.5/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.5/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9595 2023-06-08 09:08:43.000000 eis1600-0.9.5/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.5/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8824 2023-06-14 10:59:59.000000 eis1600-0.9.5/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.5/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2935 2023-06-08 07:49:05.000000 eis1600-0.9.5/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.5/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6543 2023-06-08 07:58:41.000000 eis1600-0.9.5/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.5/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.5/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.5/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.5/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.044154 eis1600-0.9.5/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.5/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.5/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.5/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.5/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.5/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.5/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.048154 eis1600-0.9.5/eis1600/toponyms/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.5/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.5/eis1600/toponyms/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2959 2023-06-08 09:06:21.000000 eis1600-0.9.5/eis1600/toponyms/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      903 2023-06-20 14:15:34.000000 eis1600-0.9.5/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-21 13:43:08.028154 eis1600-0.9.5/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2083 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      852 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-21 13:43:07.000000 eis1600-0.9.5/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-21 13:43:08.048154 eis1600-0.9.5/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2445 2023-06-16 10:55:21.000000 eis1600-0.9.5/setup.py
```

### Comparing `eis1600-0.9.4/LICENSE` & `eis1600-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/PKG-INFO` & `eis1600-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.4
+Version: 0.9.5
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.4/README.md` & `eis1600-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/dates/Date.py` & `eis1600-0.9.5/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/dates/date_patterns.py` & `eis1600-0.9.5/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/dates/methods.py` & `eis1600-0.9.5/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.5/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/gazetteers/Toponyms.py` & `eis1600-0.9.5/eis1600/gazetteers/Toponyms.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,20 +68,20 @@
         return Toponyms.__rpl
 
     @staticmethod
     def look_up_entity(entity: str) -> Tuple[str, str, List[str], List[str]]:
         """Look up tagged entity in settlements (there is no gazetteer of provinces so far).
 
         :param str entity: The token(s) which were tagged as toponym.
-        :return: placeLabel(s) as str, URI(s) as str, list of settlement uri(s), list of province uri(s),
+        :return: placeLabel(s) as str, URI(s)-tag as str, list of settlement uri(s), list of province uri(s),
         list of settlement(s) coordinates, list of province(s) coordinates.
         """
         if entity in Toponyms.__total:
             matches = Toponyms.__df.loc[Toponyms.__df['toponyms'].str.fullmatch(entity), ['uri', 'province_uri',
                                                                                           'place_label']]
             uris = matches['uri'].to_list()
-            provinces = matches['province_uri'].to_list()
+            provinces = [m for m in matches['province_uri'].to_list() if m != '']
             place = matches['place_label'].unique()
 
             return '::'.join(place), '@' + '@'.join(uris) + '@', uris, provinces
         else:
             return entity, '', [], []
```

### Comparing `eis1600-0.9.4/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.5/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.5/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-0.9.5/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/EntityTags.py` & `eis1600-0.9.5/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/Singleton.py` & `eis1600-0.9.5/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/ar_normalization.py` & `eis1600-0.9.5/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.5/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/markdown_methods.py` & `eis1600-0.9.5/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.5/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.5/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/repo.py` & `eis1600-0.9.5/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/helper/yml_to_json.py` & `eis1600-0.9.5/eis1600/helper/yml_to_json.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/UIDs.py` & `eis1600-0.9.5/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/insert_uids.py` & `eis1600-0.9.5/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/methods.py` & `eis1600-0.9.5/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/update_uids.py` & `eis1600-0.9.5/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.5/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.5/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.5/eis1600/miu/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.5/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/methods.py` & `eis1600-0.9.5/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.5/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/miu/yml_handling.py` & `eis1600-0.9.5/eis1600/miu/yml_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     """
     # We do not need to differentiate between automated and manual tags
     text_with_tags = text_with_tags.replace('Ü', '')
     tg = Toponyms.instance()
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     nas_dict = {}
-    toponyms_set: Set[str] = set()
+    settlements_set: Set[str] = set()
     provinces_set: Set[str] = set()
     nas_counter = 0
 
     m = ENTITY_TAGS_PATTERN.search(text_with_tags)
     while m:
         tag = m.group('entity')
         length = int(m.group('length'))
@@ -132,23 +132,28 @@
             try:
                 val, e_cat = get_yrs_tag_value(m.group(0))
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {file_path}')
                 return
         elif cat == 'TOPONYM':
-            place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
-            add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uri})
+            place, tag, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
+            add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': tag})
             if len(list_of_uris) == 0:
                 path, uri = split(file_path)
                 uri, ext = splitext(uri)
                 LOGGER_TOPONYMS_UNKNOWN.info(f'{uri},{entity}')
             else:
-                toponyms_set.update(list_of_uris)
-                provinces_set.update(list_of_provinces)
+                if len(list_of_provinces) > 0:
+                    settlements_set.update(list_of_uris)
+                    provinces_set.update(list_of_provinces)
+                else:
+                    # if there is no province URI that means the toponym is a province and should therefore be added
+                    # to provinces and not settlements
+                    provinces_set.update(list_of_uris)
                 if len(list_of_uris) > 1:
                     yml_handler.set_ambigious_toponyms()
         elif cat == 'ONOMASTIC':
             if tag.startswith('SHR') and entity.startswith('ب'):
                 entity = entity[1:]
                 add_to_entities_dict(entities_dict, cat, entity, tag)
             elif tag.startswith('NAS'):
@@ -167,17 +172,18 @@
         else:
             entities_dict['onomastics'] = {'nas': nas_dict}
 
     if 'onomastics' in entities_dict.keys():
         # Sort dict by keys
         entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
 
-    if toponyms_set:
-        entities_dict['settlements'] = list(toponyms_set)
-        entities_dict['edges_settlements'] = [[a, b] for a, b in combinations(toponyms_set, 2) if a != b]
+    if settlements_set:
+        entities_dict['settlements'] = list(settlements_set)
+        entities_dict['edges_settlements'] = [[a, b] for a, b in combinations(settlements_set, 2) if a != b]
+    if provinces_set:
         entities_dict['provinces'] = list(provinces_set)
         entities_dict['edges_provinces'] = [[a, b] for a, b in combinations(provinces_set, 2) if a != b]
 
     if entities_dict.get('dates'):
         dates = entities_dict.get('dates')
         birth_date = [d.get('date') for d in dates if d.get('cat') == 'B']
         death_date = [d.get('date') for d in dates if d.get('cat') == 'D']
```

### Comparing `eis1600-0.9.4/eis1600/nlp/cameltools.py` & `eis1600-0.9.5/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.5/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/nlp/utils.py` & `eis1600-0.9.5/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/onomastics/annotation.py` & `eis1600-0.9.5/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/onomastics/methods.py` & `eis1600-0.9.5/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.5/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/processing/postprocessing.py` & `eis1600-0.9.5/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/processing/preprocessing.py` & `eis1600-0.9.5/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/stats/methods.py` & `eis1600-0.9.5/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/stats/miu_stats.py` & `eis1600-0.9.5/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/toponyms/annotation.py` & `eis1600-0.9.5/eis1600/toponyms/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/toponyms/methods.py` & `eis1600-0.9.5/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.4/eis1600/toponyms/toponym_categories.py` & `eis1600-0.9.5/eis1600/toponyms/toponym_categories.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from eis1600.helper.ar_normalization import normalize_dict
 
 
 TOPONYM_CATEGORIES = {
         'ولد': 'B', 'مولد': 'B',
         'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D',
-        'حج': 'P',
-        'سمع': 'K', 'روى': 'K', 'روا': 'K', 'قرا': 'K', 'اجاز': 'K',
-        'استقر': 'O', 'انفصل': 'O', 'ولي': 'O', 'قاضي': 'O', 'أعمال': 'O',
+        'سمع': 'K', 'روى': 'K', 'روا': 'K', 'قرا': 'K', 'اجاز': 'K', 'حدث': 'K',
         'لقي': 'M',
-        'سكن': 'R', 'نزل': 'R', 'نزيل': 'R', 'من اهل': 'R', 'استوطن': 'R', 'كان من': 'R'
+        'استقر': 'O', 'انفصل': 'O', 'ولي': 'O', 'قاضي': 'O', 'نائب': 'O', 'أعمال': 'O',
+        'حج': 'P',
+        'سكن': 'R', 'نزل': 'R', 'نزيل': 'R', 'من اهل': 'R', 'استوطن': 'R', 'كان من': 'R', 'نشأ': 'R'
 }
 TOPONYM_CATEGORIES_NOR = normalize_dict(TOPONYM_CATEGORIES)
 
 AR_TOPONYM_CATEGORIES = '|'.join([denormalize(key) for key in TOPONYM_CATEGORIES.keys()])
 TOPONYM_CATEGORY_PATTERN = compile(r'\s[وف]?(?P<topo_category>' + AR_TOPONYM_CATEGORIES + r')')
```

### Comparing `eis1600-0.9.4/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.5/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.4
+Version: 0.9.5
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.4/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.5/eis1600.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
+eis1600/helper/md_tags_to_bio.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/repo.py
 eis1600/helper/yml_methods.py
 eis1600/helper/yml_to_json.py
 eis1600/helper/data/__init__.py
 eis1600/helper/data/entity_tags.csv
 eis1600/markdown/UIDs.py
```

### Comparing `eis1600-0.9.4/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.5/eis1600.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [console_scripts]
 annotate_mius = eis1600.nlp.ner_annotate_mius:main [ner]
 convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main
 disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main
 fix_miu_annotation = eis1600.helper.fix_miu_annotation:main
 insert_uids = eis1600.markdown.insert_uids:main
+md_tags_to_bio = eis1600.helper.md_tags_to_bio:main
 miu_random_revisions = eis1600.helper.miu_random_revisions:main
 miu_stats = eis1600.stats.miu_stats:main
 onomastic_annotation = eis1600.onomastics.annotation:main
 reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main
 toponym_annotation = eis1600.toponyms.annotation:main
 update_uids = eis1600.markdown.update_uids:main
 xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main
```

### Comparing `eis1600-0.9.4/setup.py` & `eis1600-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.4',
+      version='0.9.5',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
@@ -17,14 +17,15 @@
       entry_points={
           'console_scripts': [
                   'annotate_mius = eis1600.nlp.ner_annotate_mius:main [NER]',
                   'convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main',
                   'disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main',
                   'fix_miu_annotation = eis1600.helper.fix_miu_annotation:main',
                   'insert_uids = eis1600.markdown.insert_uids:main',
+                  'md_tags_to_bio = eis1600.helper.md_tags_to_bio:main',
                   'miu_random_revisions = eis1600.helper.miu_random_revisions:main',
                   'miu_stats = eis1600.stats.miu_stats:main',
                   'onomastic_annotation = eis1600.onomastics.annotation:main',
                   'toponym_annotation = eis1600.toponyms.annotation:main',
                   'reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main',
                   'update_uids = eis1600.markdown.update_uids:main',
                   'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main',
```

