# Comparing `tmp/tg_bot_ml-0.0.2.tar.gz` & `tmp/tg_bot_ml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bot_ml-0.0.2.tar", last modified: Wed Jun 21 06:58:33 2023, max compression
+gzip compressed data, was "tg_bot_ml-0.0.3.tar", last modified: Wed Jun 21 07:03:35 2023, max compression
```

## Comparing `tg_bot_ml-0.0.2.tar` & `tg_bot_ml-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 06:58:33.030071 tg_bot_ml-0.0.2/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.2/LICENSE
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 06:58:33.030071 tg_bot_ml-0.0.2/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.2/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       79 2023-06-21 06:58:33.030071 tg_bot_ml-0.0.2/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1238 2023-06-21 06:58:21.000000 tg_bot_ml-0.0.2/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 06:58:33.026071 tg_bot_ml-0.0.2/tg_bot_ml/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.2/tg_bot_ml/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3206 2023-06-20 15:20:02.000000 tg_bot_ml-0.0.2/tg_bot_ml/img_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1410 2023-06-20 09:32:12.000000 tg_bot_ml-0.0.2/tg_bot_ml/table_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2109 2023-06-20 09:00:14.000000 tg_bot_ml-0.0.2/tg_bot_ml/tg_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.2/tg_bot_ml/utils.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 06:58:33.030071 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 06:58:32.000000 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-21 06:58:32.000000 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-21 06:58:32.000000 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       62 2023-06-21 06:58:32.000000 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-21 06:58:32.000000 tg_bot_ml-0.0.2/tg_bot_ml.egg-info/top_level.txt
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.3/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       23 2023-06-19 15:42:10.000000 tg_bot_ml-0.0.3/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       79 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-21 07:03:28.000000 tg_bot_ml-0.0.3/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/tg_bot_ml/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-19 15:44:53.000000 tg_bot_ml-0.0.3/tg_bot_ml/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3206 2023-06-20 15:20:02.000000 tg_bot_ml-0.0.3/tg_bot_ml/img_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1410 2023-06-20 09:32:12.000000 tg_bot_ml-0.0.3/tg_bot_ml/table_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2109 2023-06-20 09:00:14.000000 tg_bot_ml-0.0.3/tg_bot_ml/tg_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-19 21:27:48.000000 tg_bot_ml-0.0.3/tg_bot_ml/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-21 07:03:35.770920 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-21 07:03:35.000000 tg_bot_ml-0.0.3/tg_bot_ml.egg-info/top_level.txt
```

### Comparing `tg_bot_ml-0.0.2/LICENSE` & `tg_bot_ml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.2/PKG-INFO` & `tg_bot_ml-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_bot_ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

### Comparing `tg_bot_ml-0.0.2/setup.py` & `tg_bot_ml-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 from distutils.core import setup
 setup(
   name = 'tg_bot_ml',
   packages = ['tg_bot_ml'],
-  version = '0.0.2',
+  version = '0.0.3',
   license='GPLv3',
   description = 'Simple telegram bot for logging ML statistics.',
   author = 'Dmitry',
   author_email = 'michalych2014@yandex.ru',
   url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats.git', 
   download_url = 'https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip',
   keywords = ['Telegram', 'Bot', 'ML', 'Machine Learning', 'Logger'],
   install_requires=[
           'pandas',
           'numpy',
           'matplotlib',
           'pyTelegramBotAPI',
           'pyyaml',
           'opencv-python', 
+          'tabulate'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',  
     'Programming Language :: Python :: 3',      
     'Programming Language :: Python :: 3.4',
```

### Comparing `tg_bot_ml-0.0.2/tg_bot_ml/img_bot.py` & `tg_bot_ml-0.0.3/tg_bot_ml/img_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.2/tg_bot_ml/table_bot.py` & `tg_bot_ml-0.0.3/tg_bot_ml/table_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.2/tg_bot_ml/tg_bot.py` & `tg_bot_ml-0.0.3/tg_bot_ml/tg_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.2/tg_bot_ml/utils.py` & `tg_bot_ml-0.0.3/tg_bot_ml/utils.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.2/tg_bot_ml.egg-info/PKG-INFO` & `tg_bot_ml-0.0.3/tg_bot_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-bot-ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple telegram bot for logging ML statistics.
 Home-page: https://github.com/DmitryAsdre/telegram-ml-bot-stats.git
 Download-URL: https://github.com/DmitryAsdre/telegram-ml-bot-stats/archive/refs/heads/main.zip
 Author: Dmitry
 Author-email: michalych2014@yandex.ru
 License: GPLv3
 Keywords: Telegram,Bot,ML,Machine Learning,Logger
```

