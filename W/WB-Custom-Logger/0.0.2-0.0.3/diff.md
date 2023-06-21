# Comparing `tmp/WB Custom Logger-0.0.2.tar.gz` & `tmp/WB Custom Logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WB Custom Logger-0.0.2.tar", last modified: Wed Jun 21 05:56:29 2023, max compression
+gzip compressed data, was "WB Custom Logger-0.0.3.tar", last modified: Wed Jun 21 05:59:58 2023, max compression
```

## Comparing `WB Custom Logger-0.0.2.tar` & `WB Custom Logger-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 05:56:29.507468 WB Custom Logger-0.0.2/
--rw-rw-rw-   0        0        0      232 2023-06-21 05:56:29.506468 WB Custom Logger-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1263 2023-06-14 08:57:57.000000 WB Custom Logger-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 05:56:29.499463 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/
--rw-rw-rw-   0        0        0      232 2023-06-21 05:56:29.000000 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-21 05:56:29.000000 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 05:56:29.000000 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 05:56:29.000000 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-21 05:56:29.000000 WB Custom Logger-0.0.2/WB_Custom_Logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 05:56:29.507468 WB Custom Logger-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      443 2023-06-21 05:55:21.000000 WB Custom Logger-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:56:29.503466 WB Custom Logger-0.0.2/wb_custom_logger/
--rw-rw-rw-   0        0        0       51 2023-06-14 08:57:57.000000 WB Custom Logger-0.0.2/wb_custom_logger/__init__.py
--rw-rw-rw-   0        0        0     3898 2023-06-14 08:57:57.000000 WB Custom Logger-0.0.2/wb_custom_logger/custom_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:59:58.517586 WB Custom Logger-0.0.3/
+-rw-rw-rw-   0        0        0      232 2023-06-21 05:59:58.517586 WB Custom Logger-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1263 2023-06-14 08:57:57.000000 WB Custom Logger-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:59:58.509584 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-21 05:59:58.000000 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-21 05:59:58.000000 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:59:58.000000 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 05:59:58.000000 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-06-21 05:59:58.000000 WB Custom Logger-0.0.3/WB_Custom_Logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:59:58.518585 WB Custom Logger-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      443 2023-06-21 05:59:07.000000 WB Custom Logger-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:59:58.514585 WB Custom Logger-0.0.3/wb_custom_logger/
+-rw-rw-rw-   0        0        0       51 2023-06-14 08:57:57.000000 WB Custom Logger-0.0.3/wb_custom_logger/__init__.py
+-rw-rw-rw-   0        0        0     4024 2023-06-21 05:58:39.000000 WB Custom Logger-0.0.3/wb_custom_logger/custom_logger.py
```

### Comparing `WB Custom Logger-0.0.2/README.md` & `WB Custom Logger-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `WB Custom Logger-0.0.2/wb_custom_logger/custom_logger.py` & `WB Custom Logger-0.0.3/wb_custom_logger/custom_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,19 @@
         :return: logger
         """
         # 생성자 파라미터가 None인 경우 기본값 처리
         self.set_default()
 
         # getLogger 객체 생성 및 logging level 설정
         logger = getLogger(self.logname)
+
+        # Check handler exists
+        if len(logger.handlers) > 0:
+            return logger  # Logger already exists
+
         logger.setLevel(self.loglevel)
 
         # logtype에 따라 Handler 설정
         if self.logtype == 'FILE':
             fhandler = self.get_file_log_handler()
             logger.addHandler(fhandler)
         elif self.logtype == 'STREAM':
```

