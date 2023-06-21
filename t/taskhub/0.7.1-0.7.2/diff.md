# Comparing `tmp/taskhub-0.7.1.tar.gz` & `tmp/taskhub-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\taskhub-0.7.1.tar", last modified: Tue Jun 20 08:25:59 2023, max compression
+gzip compressed data, was "dist\taskhub-0.7.2.tar", last modified: Wed Jun 21 03:15:55 2023, max compression
```

## Comparing `taskhub-0.7.1.tar` & `taskhub-0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/
--rw-rw-rw-   0        0        0      291 2023-06-20 08:25:59.000000 taskhub-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 08:25:59.000000 taskhub-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      483 2023-06-20 08:02:46.000000 taskhub-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub/
--rw-rw-rw-   0        0        0        0 2023-06-20 07:32:14.000000 taskhub-0.7.1/taskhub/__init__.py
--rw-rw-rw-   0        0        0      473 2023-06-20 07:32:14.000000 taskhub-0.7.1/taskhub/connector.py
--rw-rw-rw-   0        0        0     6979 2023-06-20 08:06:58.000000 taskhub-0.7.1/taskhub/hub.py
--rw-rw-rw-   0        0        0     1345 2023-06-20 08:25:53.000000 taskhub-0.7.1/taskhub/log.py
--rw-rw-rw-   0        0        0     1013 2023-06-20 07:38:40.000000 taskhub-0.7.1/taskhub/server.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/
--rw-rw-rw-   0        0        0      291 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/test/
--rw-rw-rw-   0        0        0      432 2023-06-20 07:32:14.000000 taskhub-0.7.1/test/test.py
--rw-rw-rw-   0        0        0      901 2023-06-20 07:38:55.000000 taskhub-0.7.1/test/test_serve.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:15:55.000000 taskhub-0.7.2/
+-rw-rw-rw-   0        0        0      291 2023-06-21 03:15:55.000000 taskhub-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:15:55.000000 taskhub-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      483 2023-06-21 03:15:26.000000 taskhub-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:32:14.000000 taskhub-0.7.2/taskhub/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-06-20 07:32:14.000000 taskhub-0.7.2/taskhub/connector.py
+-rw-rw-rw-   0        0        0     6979 2023-06-20 08:06:58.000000 taskhub-0.7.2/taskhub/hub.py
+-rw-rw-rw-   0        0        0     1340 2023-06-21 03:15:37.000000 taskhub-0.7.2/taskhub/log.py
+-rw-rw-rw-   0        0        0     1013 2023-06-20 07:38:40.000000 taskhub-0.7.2/taskhub/server.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/
+-rw-rw-rw-   0        0        0      291 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 03:15:55.000000 taskhub-0.7.2/taskhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:15:55.000000 taskhub-0.7.2/test/
+-rw-rw-rw-   0        0        0      432 2023-06-20 07:32:14.000000 taskhub-0.7.2/test/test.py
+-rw-rw-rw-   0        0        0      901 2023-06-20 07:38:55.000000 taskhub-0.7.2/test/test_serve.py
```

### Comparing `taskhub-0.7.1/taskhub/hub.py` & `taskhub-0.7.2/taskhub/hub.py`

 * *Files identical despite different names*

### Comparing `taskhub-0.7.1/taskhub/log.py` & `taskhub-0.7.2/taskhub/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,21 @@
         else:
             level_color = level
 
         log_time = self.formatTime(record, self.datefmt)
         message = record.getMessage()
         return f"{log_time} {level_color} {message}"
 
+
 log_name = "taskhub"
 logger = logging.getLogger(log_name)
 
 formatter = ColoredFormatter("%(asctime)s-%(levelname)s-%(message)s")
 
-file_handler = logging.FileHandler(f"/var/log/{log_name}.log")
+file_handler = logging.FileHandler(f"./{log_name}.log")
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(formatter)
 logger.addHandler(stream_handler)
```

### Comparing `taskhub-0.7.1/taskhub/server.py` & `taskhub-0.7.2/taskhub/server.py`

 * *Files identical despite different names*

### Comparing `taskhub-0.7.1/test/test_serve.py` & `taskhub-0.7.2/test/test_serve.py`

 * *Files identical despite different names*

