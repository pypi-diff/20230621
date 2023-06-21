# Comparing `tmp/inhandtest-0.0.56.tar.gz` & `tmp/inhandtest-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.56.tar", last modified: Thu Jun 15 06:17:55 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.57.tar", last modified: Wed Jun 21 05:35:38 2023, max compression
```

## Comparing `inhandtest-0.0.56.tar` & `inhandtest-0.0.57.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.56/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-15 06:17:55.000000 inhandtest-0.0.56/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.56/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.56/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.56/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.56/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.56/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.56/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.56/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    57431 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23845 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.56/inhandtest/exception.py
--rw-rw-rw-   0        0        0     4219 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/file.py
--rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.56/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22019 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    52646 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7726 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14792 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.56/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 05:51:48.000000 inhandtest-0.0.56/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.56/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.56/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.56/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3057 2023-06-14 06:26:03.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.56/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33875 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    28008 2023-06-15 06:16:19.000000 inhandtest-0.0.56/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1685 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.56/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 06:17:55.000000 inhandtest-0.0.56/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-06-15 06:16:19.000000 inhandtest-0.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.57/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-21 05:35:38.000000 inhandtest-0.0.57/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.57/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.57/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.57/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.57/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.57/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.57/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.57/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.57/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    57431 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23845 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.57/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.57/inhandtest/file.py
+-rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.57/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22019 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    71913 2023-06-21 03:57:22.000000 inhandtest-0.0.57/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     8072 2023-06-20 09:32:40.000000 inhandtest-0.0.57/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14792 2023-06-15 06:12:16.000000 inhandtest-0.0.57/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.57/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.57/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.57/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.57/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.57/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.57/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3057 2023-06-14 06:26:03.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.57/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.57/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    28008 2023-06-15 06:16:19.000000 inhandtest-0.0.57/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1685 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.57/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:35:38.000000 inhandtest-0.0.57/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-06-21 05:35:26.000000 inhandtest-0.0.57/setup.py
```

### Comparing `inhandtest-0.0.56/PKG-INFO` & `inhandtest-0.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.56
+Version: 0.0.57
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.56/README.md` & `inhandtest-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/dm/mqtt.py` & `inhandtest-0.0.57/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/dm/register_v1.py` & `inhandtest-0.0.57/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.57/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.57/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.57/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/base_page/base_page.py` & `inhandtest-0.0.57/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.57/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/exception.py` & `inhandtest-0.0.57/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/file.py` & `inhandtest-0.0.57/inhandtest/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,37 +27,43 @@
                 os.remove(c_path)
     elif os.path.isfile(file_path):
         os.remove(file_path)
     else:
         logging.debug(f"parameter file_path {file_path} is not exist")
 
 
-def check_file(file_path_or_file_dir, create_dir=True) -> None:
-    """校验文件夹以及文件是否存在, 如果文件夹不存在则创建，如果文件不存在则抛出异常
+def check_file(file_path) -> None:
+    """校验文件是否存在
 
-    :param file_path_or_file_dir: 文件夹路径或者文件路径
-    :param create_dir: 当检测出文件夹不存在时就创建
+    :param file_path: 文件夹路径或者文件路径
     :return:  检查到文件不存在时就抛异常FileNotFoundError
     """
-    if os.path.isdir(file_path_or_file_dir):
-        if os.path.exists(file_path_or_file_dir):
-            logging.debug(f"check dir {file_path_or_file_dir} ok")
-        else:
-            if create_dir:
-                os.mkdir(file_path_or_file_dir)
-                logging.debug(f"create dir {file_path_or_file_dir} ok")
-            else:
-                logging.exception(f"this dir {file_path_or_file_dir} not exist")
-                raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
+    if not os.path.isfile(file_path) or not os.path.exists(file_path):
+        logging.exception(f"this file {file_path} not exist")
+        raise FileNotFoundError(f"this file {file_path} not exist")
+    else:
+        logging.debug(f"check file {file_path} ok")
+
+
+def check_dir(dir_path, create_dir=True) -> None:
+    """
+
+    :param dir_path:  问价夹路径
+    :param create_dir:
+    :return:
+    """
+    if os.path.exists(dir_path):
+        logging.debug(f"check dir {dir_path} ok")
     else:
-        if not os.path.isfile(file_path_or_file_dir):
-            logging.exception(f"this file {file_path_or_file_dir} not exist")
-            raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
+        if create_dir:
+            os.makedirs(dir_path)
+            logging.debug(f"create dir {dir_path} ok")
         else:
-            logging.debug(f"check file {file_path_or_file_dir} ok")
+            logging.exception(f"this dir {dir_path} not exist")
+            raise FileNotFoundError(f"this file {dir_path} not exist")
 
 
 def generate_str_or_file(size: int or str = '48KB', file_path=None) -> str:
     """生成指定大小字符串或文件 1024KB=1MB  1024MB=1GB  1024GB=1TB
 
     :param size: int or str, int时单位为字节， str可带单位'KB'|'MB'|'GB', e.g: 49152|'48KB'...
     :param file_path: 文件全路径，ex: /$file_path/test.txt 将内容写道文件中
```

### Comparing `inhandtest-0.0.56/inhandtest/inmodbus.py` & `inhandtest-0.0.57/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/inmongodb.py` & `inhandtest-0.0.57/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/inmqtt.py` & `inhandtest-0.0.57/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/inrequest.py` & `inhandtest-0.0.57/inhandtest/inrequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # @File    : inrequest.py
 """
 封装request， 使设备和平台都能来正常调用，统一入口，token过期时也能自动更新
 
 """
 import base64
 import os
+import random
 import re
 import time
 from typing import List
 import urllib3
 import requests
 from inhandtest.exception import ParameterValueError, UsernameOrPasswordError, TimeOutError, UpgradeFailedError, \
     ResourceNotFoundError
 from inhandtest.file import file_hash
-from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict, loop_inspector
+from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict, loop_inspector, get_time_stamp, generate_string
 import logging
 
 
 class DnInterface:
     def __init__(self, username, password, host='c.inhand.com.cn'):
         """
         :param username  平台用户名
@@ -681,34 +682,343 @@
         :param host: 'star.inhandcloud.cn'|'star.inhandcloud.cn'|'star.nezha.inhand.dev'|'star.nezha.inhand.design' 平台是哪个环境,
         """
         self.host = host
         self.username = username
         self.api = InRequest(self.host, username, password, 'star')
         self.me = self.__get_me()
 
+    def __only_admin(function):
+        """只能当装饰器使用，只有admin用户才能使用
+
+        :param function:
+        :return:
+        """
+
+        def admin_user(self, *args, **kwargs):
+            if self.username != 'admin':
+                logging.exception('only admin user can use this function')
+                raise Exception('only admin user can use this function')
+            else:
+                res = function(self, *args, **kwargs)
+            return res
+
+        return admin_user
+
+    def __only_user(function):
+        """只能当装饰器使用，只有用户才能使用
+
+        :param function:
+        :return:
+        """
+
+        def _user(self, *args, **kwargs):
+            if self.username == 'admin':
+                logging.exception('only user can use this function')
+                raise Exception('only user can use this function')
+            else:
+                res = function(self, *args, **kwargs)
+            return res
+
+        return _user
+
     def __get_me(self) -> DotDict:
         """ 获取me的各种信息 包括oid
 
         :return:
         """
         response = DotDict(
             self.api.send_request('/api/v1/users/me', method='get', param={"expand": 'org'}).json().get('result'))
         return response
 
+    @__only_user
+    def send_config(self, sn: str, payload: dict, commit=True) -> dict:
+        """下发设备配置
+
+        :param sn: 设备序列号
+        :param commit: 是否提交, 在云端可以保存配置，默认是提交
+        :param payload: 配置内容，当配置中的key是随机id时， 可使用$id，下发时会自动替换成随机id
+        :return:
+        """
+
+        def switch_config(in_payload: dict) -> dict:
+            """转换配置，当配置中的key是随机id时， 可使用$id, 然后该函数会自动替换成随机id并返回
+
+            :param in_payload: 需要修正的配置项，其中需要更新的key 使用$id来替换
+            :return:
+            """
+            local_time = str(hex(int(time.time())))[2:]
+            start = f'000{random.randint(1, 9)}{local_time}'
+            in_payload = str(in_payload)
+            for i in range(0, len(re.findall('\$id', in_payload))):
+                in_payload = in_payload.replace('$id',
+                                                f'{start}{generate_string(4, uppercase=False, special_chars=False)}', 1)
+            return eval(in_payload)
+
+        payload = switch_config(payload)
+        session_id = \
+            self.api.send_request('/api/v1/config/init', 'post',
+                                  param={'deviceId': self.device_state([sn])[0].get('id')},
+                                  ).json().get('result').get('_id')
+        header = {'x-session-id': session_id}
+        resp = self.api.send_request('/api/v1/config', 'put', body=payload, header=header).json()
+        assert resp == {'result': 'ok'}, 'save config failed'
+        if commit:
+            resp = self.api.send_request('/api/v1/config/commit', 'post', header=header).json()
+            assert resp == {'result': 'ok'}, 'commit config failed'
+            logging.info(f'the device {sn} config commit success')
+        return payload
+
+    @__only_user
+    def get_config(self, sn: str, expect: dict, type_='actual') -> dict or None:
+        """获取校验备配置
+
+        :param sn: 设备序列号
+        :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
+        :param type_: actual 实际设备上传的配置
+                      group 设备所在组的配置
+                      pending 正在下发的配置
+                      target 目标配置
+                      individual 个性化配置
+        :return: 如果 expect 为None 就返回设备当前实际的配置
+        """
+        expect = {'result': {type_: expect}}
+        if expect is not None:
+            self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/config', 'get',
+                                  expect=expect)
+        else:
+            return self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/config',
+                                         'get').json().get('result').get(type_)
+
+    @__only_user
+    def clear_config(self, sn: str):
+        """清除设备配置
+
+        :param sn:
+        :return:
+        """
+        self.api.send_request(f'/api/v1/config/layer/device/{self.device_state([sn])[0].get("id")}', 'delete', expect={
+            "result": 'ok'})
+        self.get_config(sn, expect={}, type_='individual')
+
+    @__only_user
+    def copy_config(self, source_sn: str, target_sns: list):
+        """清除设备配置
+
+        :param source_sn: 源设备sn
+        :param target_sns: 目标设备sn
+        :return:
+        """
+        body = {"sourceDeviceId": self.device_state([source_sn])[0].get("id"),
+                "targetDeviceIds": [device.get('id') for device in self.device_state(target_sns)]}
+        self.api.send_request(f'/api/v1/config/layer/bulk-copy', 'post', body=body, expect={"result": 'ok'})
+
+    @__only_user
+    def create_org(self, name: str, parent_name: str or None, level=2, email='', phone='', **kwargs) -> str:
+        """创建组织, 创建2级组织时，parent_name和parent_id可以不传
+
+        :param name: 组织名称 (在实现自动化时可让名称唯一，来实现创建组织的唯一性)
+        :param parent_name: 父组织名称，如果组织名称唯一，可以传入，如果不唯一就拿第一个创建
+        :param level: 组织层级，2 二级组织，3 三级组织 4 四级组织 5 五级组织
+        :param email: 组织邮箱
+        :param phone: 组织电话
+        :param kwargs: 组织信息
+               parent_id: 父组织id，唯一id，传入它时可以不用传入parent_name
+               description: 组织描述
+        :return: 组织id
+        """
+        if level in (2, 3, 4, 5):
+            parent_level = level - 1
+            orgs = self.api.send_request('/api/v1/orgs', 'get', param={'depth': 4, 'limit': 500}).json().get('result')
+            if parent_level == 1:
+                parent_id = [org.get('_id') for org in orgs if org.get('level') == 1][0]
+            else:
+                if kwargs.get('parent_id'):
+                    parent_id = kwargs.get('parent_id')
+                else:
+                    parent_id = [org.get('_id') for org in orgs if org.get('level') == parent_level and
+                                 org.get('name') == parent_name][0]
+            body = {'name': name, 'parent': parent_id, 'phone': phone, 'email': email,
+                    'description': kwargs.get('description')}
+            logging.info(f'create org {name} success')
+            return self.api.send_request('/api/v1/orgs', 'post', body=body).json().get('result').get('_id')
+        else:
+            raise ValueError('level must be in (2, 3, 4, 5)')
+
+    @__only_user
+    def delete_org(self, name: str or list or None, _id: str or list or None):
+        """删除组织, 不能删除一级组织
+
+        :param name: 组织名称, _id 为None时，使用名称删除，搜索到名称一致的组织就全部删除
+        :param _id: 组织id, 使用id删除，精确删除
+        :return:
+        """
+        if _id:
+            if isinstance(_id, str):
+                _id = [_id]
+        else:
+            if name:
+                if isinstance(name, str):
+                    name = [name]
+                orgs = self.api.send_request('/api/v1/orgs', 'get', param={'depth': 5, 'limit': 500}).json().get(
+                    'result')
+                _id = []
+                for name_ in name:
+                    [_id.append(org.get('_id')) for org in orgs if org.get('name') == name_]
+
+        if _id:
+            for __id in _id:
+                self.api.send_request(f'/api/v1/orgs/{__id}', 'delete')
+            logging.info(f'delete org success')
+
+
+    @__only_admin
+    def org_info_in_paas(self, org_email) -> DotDict:
+        """ 获取org info
+
+        :param org_email:
+        :return:   {name: "Admin_test_new", email: "liwei@inhand.com.cn", _id: "5fb24ef9f0393a4c4fd7c8b7"}
+        """
+        orgs = \
+            self.api.send_request('/api/v1/orgs', 'get',
+                                  param={'email': org_email, 'fields': '_id,name,email', 'limit': 100}).json().get(
+                'result')
+        if orgs:
+            for org in orgs:
+                if org.get('email') == org_email:
+                    return DotDict(org)
+            else:
+                logging.exception(f'the org {org_email} not exist')
+                raise Exception(f'the org {org_email} not exist')
+        else:
+            logging.exception(f'the org {org_email} not exist')
+            raise Exception(f'the org {org_email} not exist')
+
+    @__only_admin
+    def create_license_to_org(self, org_email: str, licenses: dict):
+        """ 创建license
+
+        :param org_email: 企业邮箱
+        :param licenses: license {'slug': 'star_pro', 'period': 'year', 'periodCount':1, 'number': 1}
+        """
+        license_prices = self.api.send_request(f'/api/v1/billing/license-types/{licenses.get("slug")}/prices', 'get',
+                                               param={'verbose': 100}).json().get('result')
+        org_info = self.org_info_in_paas(org_email)
+        try:
+            license_price = [i for i in license_prices if
+                             i['period'] == licenses.get('period') and i['periodCount'] == licenses.get('periodCount')][
+                0]
+            self.api.send_request('/api/v1/billing/licenses', 'post',
+                                  body={'type': licenses.get('slug'), 'active': True, 'count': licenses.get('number'),
+                                        'oid': org_info.get('_id'), 'priceId': license_price['_id']}, code=200)
+        except Exception:
+            logging.exception(f'licenses create fail, please check the licenses info')
+            raise
+
+    @__only_admin
+    def delete_user_in_paas(self, email):
+        """ 删除用户
+
+        :param email:
+        :return:
+        """
+        users = self.api.send_request('api/v1/users', 'get', param={'email': email, 'limit': 100}).json().get('result')
+        if users:
+            for user in users:
+                if email == user.get('email'):
+                    try:
+                        self.api.send_request(f'api/v1/users/{user.get("_id")}', 'delete',
+                                              param={'oid': user.get("oid")})
+                        logging.info(f'the {email} user delete success')
+                    except Exception:
+                        logging.exception(f'the email be used by org, can not delete')
+                    break
+            else:
+                logging.info(f'the {email} user not exist')
+
+    @__only_admin
+    def create_org_in_paas(self, org_info: dict):
+        """
+
+        :param org_info:  {'email': org_email, 'password': org_password} 必填
+        :return:
+        """
+        orgs = self.api.send_request('api/v1/orgs', 'get',
+                                     param={'email': org_info.get('email'), 'limit': 100}).json().get('result')
+        org_info.update(
+            {'name': org_info.get('email'), 'bizCategory': 'OILS_GAS_CONSUMABLE_FUELS', 'countryCode': 'AL'})
+        if orgs:
+            for org in orgs:
+                if org_info.get('email') == org.get('email'):
+                    self.update_user(org_info.get('email'), password=org_info.get('password'))  # 更新密码
+                    logging.debug(f'the {org_info.get("email")} org already exist')
+                    break
+            else:
+                self.api.send_request('api/v1/orgs', 'post', body=org_info)
+                logging.debug(f'admin create {org_info.get("email")} org success')
+        else:
+            self.api.send_request('api/v1/orgs', 'post', body=org_info)
+            logging.debug(f'admin create {org_info.get("email")} org success')
+
+    @__only_admin
+    def delete_org_in_paas(self, org_info: dict):
+        """ 删除企业
+
+        :param org_info: 企业信息 {'email': org_email, 'password': org_password}
+        :return:
+        """
+        orgs = self.api.send_request('api/v1/orgs', 'get',
+                                     param={'email': org_info.get('email'), 'limit': 100}).json().get('result')
+        if orgs:
+            for org in orgs:
+                if org_info.get('email') == org.get('email'):
+                    org_user = StarInterface(org_info.get('email'), org_info.get('password'), self.host)
+                    org_user.delete_device('all')
+                    self.api.send_request(f'api/v1/orgs/{org.get("_id")}', 'delete')
+                    logging.info(f'admin delete {org_info.get("email")} org delete success')
+                    break
+            else:
+                logging.info(f'the {org_info.get("email")} org not exist')
+
+    @__only_user
+    def bind_license(self, sn: list, licenses: dict):
+        """ 绑定license
+
+        :param sn
+        :param licenses: {'slug': 'star_pro'}
+        """
+        licenses_ = []
+        org_license = self.api.send_request('/api/v1/billing/licenses', 'get',
+                                            param={'expand': 'org,device,type', 'limit': 200, 'page': 0},
+                                            code=200).json().get('result')
+        if org_license:
+            for org in org_license:
+                if org['status'] != 'expired' and org.get('device') is None and org['type']['slug'] == licenses.get(
+                        'slug'):
+                    licenses_.append(org['_id'])
+        if len(licenses_) < len(sn):
+            logging.error(f'licenses not enough, please check the licenses')
+        else:
+            device_ids = [device.get('id') for device in self.device_state(sn)]
+            for license_, _id in zip(licenses_, device_ids):
+                self.api.send_request(f'/api/v1/billing/licenses/{license_}/device', 'put', body={'deviceId': _id},
+                                      code=200)
+            logging.info(f'bind license success')
+
     def device_state(self, sn: list) -> List[dict]:
         """根据sn 转换属性 属性值有：  online: 在线|离线   True|False
                                        iccid:
                                        imei:
                                        imsi:
                                        version: 固件版本
                                        licenseStatus: 'licensed'
                                        sn: 序列号
                                        address
                                        id: 设备id
                                        name: 设备名字
+                                       org:  {'_id': oid, 'name': 'org_name', 'email': 'org_email'}
         :param sn: 列表
         :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
         """
         result = []
         for sn_ in sn:
             response = self.api.send_request('/api/v1/devices', method='get',
                                              param={"expand": 'firmwareUpgradeStatus,compatibilities,org', "limit": 10,
@@ -721,19 +1031,19 @@
                     {'sn': sn_, 'online': res.get('online'),
                      'iccid': state.get('iccid') if state else None,
                      'imei': state.get('imei') if state else None,
                      'imsi': state.get('imsi') if state else None,
                      'version': res.get('firmware'),
                      'licenseStatus': res.get('licenseStatus'),
                      'address': res.get('address'),
-                     'id': res.get('_id'),
+                     'id': res.get('_id'), 'org': res.get('org'),
                      'name': res.get('name')})
             else:
                 result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None,
+                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'org': None,
                      'version': None, 'licenseStatus': None, 'address': None, 'id': None, 'name': None})
         return result
 
     def add_device(self, sn: str, mac_or_imei: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
@@ -795,23 +1105,124 @@
             else:
                 logging.exception(f"the {sn} state {state} check failed")
                 raise TimeOutError(f"the {sn} state {state} check failed")
 
     def delete_device(self, sn: str or list) -> None:
         """
 
-        :param sn: 设备序列号，一个或多个
+        :param sn: 设备序列号，一个或多个, sn='all' 时，删除所有设备
         :return:
         """
-        sn = [sn] if isinstance(sn, str) else sn
-        device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
-        if device:
-            for device_ in device:
-                self.api.send_request(f'api/devices/{device_.get("id")}', 'delete')
-                logging.info(f'the {device_.get("sn")} delete success')
+
+        def delete(ids: list):
+            if ids:
+                for _id in ids:
+                    self.api.send_request(f'api/v1/devices/{_id}', 'delete')
+                    logging.debug(f'{_id} device delete success')
+
+        if sn == 'all':
+            while True:
+                devices = self.api.send_request(f'api/v1/devices', 'get', {'limit': 100, 'page': 0}).json().get(
+                    'result')
+                if devices:
+                    delete([device.get('_id') for device in devices])
+                else:
+                    break
+                logging.info(f'{self.username} user delete all device success')
+        else:
+            sn = [sn] if isinstance(sn, str) else sn
+            devices = list(filter(lambda x: x.get('id'), self.device_state(sn)))
+            delete([device.get('id') for device in devices])
+            logging.info(f'{self.username} user delete {sn} device success')
+
+    def update_user(self, email: str, **kwargs):
+        """更新用户
+
+        :param email: 用户邮箱
+        :param kwargs:
+               password: 密码
+        :return:
+        """
+        users = self.api.send_request('api/v1/users', 'get',
+                                      param={'email': email, 'limit': 20, 'expand': 'roles,mfa,org'}).json().get(
+            'result')
+        if users:
+            if kwargs.get('password'):
+                for user in users:
+                    if email == user.get('email'):
+                        self.api.send_request(f'api/v1/users/{user.get("_id")}/password', 'put',
+                                              body={'password': kwargs.get('password')})
+                        logging.info(f'the {email} user update password success')
+                        self.api = InRequest(self.host, email, kwargs.get('password'), 'star')  # 重新登录
+                        break
+                else:
+                    logging.warning(f'the {email} user not exist')
+        else:
+            logging.warning(f'the {email} user not exist')
+
+    def assert_cellular_history(self, sn, state, delta_day=-1, data_interval=None):
+        """
+
+        :param sn:
+        :param state:
+        :param delta_day: 查询开始时间的起点， 默认晚一天时间
+        :param data_interval: 当查询的时间越长时，返回的数据会少，防止页面在渲染时卡顿，所以返回的数据间隔增大，可以对间隔做判断， 单位秒
+        :return:
+        """
+        time.sleep(2)
+
+        def time_reduction(time_list, delta):
+            """
+            校验数据点时间差
+            :param time_list: list of timestamp
+            :param delta: int
+            :return:
+            """
+            tmp = []
+            for each in time_list:
+                each = time.strptime(each, "%Y-%m-%dT%H:%M:%SZ")
+                tmp.append(int(time.mktime(each)))
+            t0 = tmp[0]
+            for i in tmp[1:]:
+                assert abs(t0 - i) == delta
+                t0 = i
+
+        payload = {
+            "after": get_time_stamp(delta=delta_day, delta_type='d', time_format='%Y-%m-%dT16:00:00.000Z'),
+            "before": get_time_stamp(time_format='%Y-%m-%dT16:00:00.000Z')
+        }
+        resp = self.api.send_request(f'/api/v1/devices/{self.device_state([sn])[0].get("id")}/signal', 'get',
+                                     param=payload, code=200).json().get('result').get('series')
+        fields = resp[0]['fields']
+        cellular_state = []
+        if state:
+            for each_type in resp:
+                for data in each_type["data"]:
+                    temp = {"name": "signal", "tags": {"type": each_type["type"]}, "fields": {}}
+                    if data[1]:
+                        temp["timestamp"] = data[0]
+                        for i in range(1, len(data)):
+                            if data[i] != 0:
+                                if data[i]:
+                                    if i == 5:
+                                        temp["fields"]["level"] = data[i] - 1
+                                    temp["fields"][fields[i]] = data[i]
+                            elif data[i] == 0:
+                                temp["fields"][fields[i]] = 0
+                        temp["fields"].pop("strength")
+                        cellular_state.append(temp)
+                        assert temp in state, '查询结果不对'
+            assert len(cellular_state) == len(state), '查询结果不对'
+        if data_interval is not None:
+            cellular_type = []
+            for each_type in resp:
+                cellular_type.append(each_type['type'])
+                timestamp_ls = [i[0] for i in each_type['data']]
+                time_reduction(timestamp_ls, delta=data_interval)
+            assert len(cellular_type) == len(set(cellular_type)), '蜂窝历史返回数据不对'
 
 
 class InRequest:
 
     def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443):
         """支持设备，平台登录及操作API, 自动识别地址
 
@@ -881,14 +1292,15 @@
             self.host = host_re
         elif self.type_ == 'device':
             username_password = '%s:%s' % (self.username, self.password)
             base_auth = base64.b64encode(username_password.encode()).decode()
             self.headers = {'Authorization': 'Basic %s' % base_auth}
             resp = self.send_request('v1/user/login', 'post').json()
             self.headers['Authorization'] = 'Bearer ' + resp['results']['web_session']
+        logging.info(f'{self.username} login success')
 
     def send_request(self, path, method, param=None, body=None, expect=None, file_path=None,
                      params_type='json', header=None, code=200, auth=True):
         """封装http请求，根据请求方式及参数类型自动判断使用哪些参数来发送请求
 
         :param path: 请求路径
         :param method: 请求方法
@@ -942,15 +1354,15 @@
             if params_type == 'JSON':
                 res = requests.put(url, json=body, params=param, headers=header, verify=False)
             else:
                 res = requests.put(url, data=param, headers=header, verify=False)
         else:
             logging.exception(f"requests method {method} not support")
             raise ParameterValueError(f"requests method {method} not support")
-        logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
+        # logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
         if res.status_code != 401:
             if self.type_ == 'device':
                 if res.status_code == 404:
                     logging.exception(f"not support API login")
                     raise Exception('not support API login')
                 if res.status_code == 200 and 'login' in path:
                     if 'error' in res.json().keys():
@@ -962,15 +1374,15 @@
             except Exception:
                 logging.warning(f'Requests Response json is None')
         else:
             # 当token过期时，统一重新登录后再次调API
             self.__login()
             res = self.send_request(path, method, param, body, expect, file_path, params_type, header, code)
         if code:
-            assert res.status_code == code, '返回状态不一致'
+            assert res.status_code == code, res.text
         if expect:
             if isinstance(expect, list):
                 if len(expect) > 0:
                     for i in expect:
                         if isinstance(i, str) or isinstance(i, int):
                             assert str(i) in res.text, f"Response text {res.text} Does not contain {i}"
                         elif isinstance(i, dict):
@@ -982,8 +1394,12 @@
             else:
                 logging.exception(f'expect param type error！')
                 raise ValueError('expect param type error！')
         return res
 
 
 if __name__ == "__main__":
-    pass
+    from inhandtest.log import enable_log
+
+    enable_log(console_level='info')
+    my = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
+    my.delete_org('test', None, )
```

### Comparing `inhandtest-0.0.56/inhandtest/inserial.py` & `inhandtest-0.0.57/inhandtest/inserial.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,26 +138,34 @@
         else:
             logging.exception(f'serial com {self.com} read log timeout')
             raise Exception('can not receive logs')
 
     def logout(self):
         self.send_cli({"exit": "[Y|N]", "y": "Press"})
 
-    def send_cli(self, command: dict):
+    def send_cli(self, command: dict, encoding='gbk'):
         """发送命令，支持多条，
 
         @param command: 支持发送多条命令，命令为key，期望返回为value, 先执行的命令写前面
         {"first_command": "first_flag", "second_command": "second_flag"}
+        @param encoding: 编码格式, 默认gbk, 支持 hex
         @return: 当发送一条命令时直接返回结果，发送多条时返回结果列表
         """
         flag_reacts = []
         if command:
             for com, flag in command.items():
-                self.serial.write(bytes((com + "\r\n").encode("gbk")))
-                flag_react = self.serial.read_until(flag.encode("gbk")).decode("gbk").strip()
+                if encoding == 'hex':
+                    self.serial.write(bytes.fromhex(com + "\r\n"))
+                else:
+                    self.serial.write(bytes((com + "\r\n").encode(encoding)))
+                if not flag:
+                    flag_react = None
+                    time.sleep(1)
+                else:
+                    flag_react = self.serial.read_until(flag.encode("gbk")).decode("gbk").strip()
                 logging.debug(flag_react)
                 flag_reacts.append(flag_react)
         if len(flag_reacts) == 1:
             return flag_reacts[0]
         else:
             return flag_reacts
```

### Comparing `inhandtest-0.0.56/inhandtest/insocket.py` & `inhandtest-0.0.57/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/inssh.py` & `inhandtest-0.0.57/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/ip.py` & `inhandtest-0.0.57/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/log.py` & `inhandtest-0.0.57/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/mail.py` & `inhandtest-0.0.57/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.57/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.57/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/pytest_email.html` & `inhandtest-0.0.57/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest/telnet.py` & `inhandtest-0.0.57/inhandtest/telnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,14 +317,15 @@
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
                interface_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在interface_replace 有值时生效，默认cli
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
+               read_until_timeout_no_raise: bool, 读取超时时是否抛出异常，默认False
 
         :return: 读取超时时返回Exception， 如果命令执行正确，返回最后一条命令输入后的结果
         """
         interface_replace_type = kwargs.get('interface_replace_type') if kwargs.get('interface_replace_type') else 'cli'
         key_replace_type = kwargs.get('key_replace_type') if kwargs.get('key_replace_type') else 'last_read'
         if kwargs.get('key_replace') and 'cli' in key_replace_type:  # 替换方法的关键字
             command = replace_str(command, kwargs.get('key_replace'))
@@ -375,16 +376,17 @@
                                 break
                     else:
                         # 如果没有readuntil 直接返回
                         break
                 else:
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     time.sleep(1)
-                    logging.exception(f"Device {self.host} send cli {command} ReadUntilTimeOutError")
-                    raise Exception('ReadUntilTimeOutError')
+                    if not kwargs.get('read_until_timeout_no_raise'):
+                        logging.exception(f"Device {self.host} send cli {command} ReadUntilTimeOutError")
+                        raise Exception('ReadUntilTimeOutError')
         if kwargs.get('key_replace') and 'last_read' in key_replace_type:
             result = replace_str(result, kwargs.get('key_replace'))
         if self.interface_replace and 'last_read' in interface_replace_type:  # 替换接口的关键字
             result = replace_str(result, self.interface_replace)
         return result
 
     @__auto_login
@@ -433,27 +435,27 @@
                 if expect:
                     if 'expect' in key_replace_type:
                         expect = replace_str(expect, key_replace)
                     if 'expect' in interface_replace_type:
                         expect = replace_str(expect, self.interface_replace)
                     logging.debug(f'start assert cli expect {expect}')
                     if isinstance(expect, str):
-                        if expect not in result:
+                        if not len(re.findall(expect, result)):
                             check_ = False
                     elif isinstance(expect, list):
-                        if [expect_ for expect_ in expect if expect_ not in result]:
+                        if [expect_ for expect_ in expect if not len(re.findall(expect_, result))]:
                             check_ = False
                     elif isinstance(expect, dict):
                         for k, v in expect.items():
                             if v:
-                                if k not in result:
+                                if not len(re.findall(k, result)):
                                     check_ = False
                                     break
                             else:
-                                if k in result:
+                                if len(re.findall(k, result)):
                                     check_ = False
                                     break
                     else:
                         logging.exception(f'parameter expect type error, expect {expect}')
                         raise Exception('parameter expect is error')
                 if check_:
                     break
@@ -515,42 +517,49 @@
         command = 'tcpdump'
         if kwargs:
             for k, v in kwargs.items():
                 for k_, v_ in flag.items():
                     if k == k_:
                         command = command + f' {v_} ' + f'{v}'
         for i in range(0, timeout, interval):
-            tag_not = False
+            result = True
+            not_expect_ = []
             if isinstance(expect, dict):
-                for k, v in expect.items():
-                    if not v:
-                        tag_not = True
-                        break
-                expect = [_ for _ in expect.keys()]
+                not_expect_ = [k for k, v in expect.items() if not v]
+                expect_ = [k for k, v in expect.items() if v]
+            elif isinstance(expect, str):
+                expect_ = [expect]
+            elif isinstance(expect, list) or isinstance(expect, tuple):
+                expect_ = expect
             else:
-                pass
-            if not tag_not:  # 判断需要抓到
+                logging.exception('parameter expect type error')
+                raise Exception('parameter expect type error')
+            if expect_:
                 try:
-                    self.send_cli(command, [expect], timeout=15, type_='super', key_replace=key_replace,
-                                  key_replace_type='cli')
+                    _result = self.send_cli(command, expect_, timeout=timeout, type_='super', key_replace=key_replace,
+                                            key_replace_type='cli')
                     logging.debug('find the exception in tcpdump result.')
                     self.tn.write(("\003" + "\r").encode("cp936"))
-                    break
+                    if not_expect_:
+                        if [not_expect for not_expect in not_expect_ if not_expect in _result]:
+                            result = False
                 except:
-                    time.sleep(interval)
-                    continue
-            else:  # 判断不需要抓到
-                try:
-                    self.send_cli(command, [expect], timeout=10, type_='super', key_replace=key_replace,
-                                  key_replace_type='cli')
-                    self.tn.write(("\003" + "\r").encode("cp936"))
-                    time.sleep(interval)
-                    continue
-                except:
-                    break
+                    result = False
+            else:
+                if not_expect_:
+                    _result = self.send_cli(command, '你还好', timeout=timeout, type_='super',
+                                            key_replace=key_replace,
+                                            key_replace_type='cli',
+                                            read_until_timeout_no_raise=True)
+                    if [not_expect for not_expect in not_expect_ if not_expect in _result]:
+                        result = False
+            if result:
+                break
+            else:
+                time.sleep(interval)
         else:
             logging.exception('TcpdumpTimeOutError')
             raise Exception('TcpdumpTimeOutError')
 
     @__auto_login
     @loop_inspector('Telnet regular match content')
     def re_match(self, command: str or list, regular: str or list, type_='super',
@@ -643,15 +652,16 @@
         """
         self.user_mode()
         self.send_cli(['reboot', 'y'])
         logging.info("【%s】Device is rebooting, wait for moment" % self.host)
         time.sleep(10)
         for i in range(0, 150, 5):
             try:
-                telnetlib.Telnet(self.host, self.port, timeout=5)
+                d = telnetlib.Telnet(self.host, self.port, timeout=5)
+                d.close()
                 break
             except:
                 pass
 
     @__auto_login
     def close(self) -> None:
         """关闭连接
@@ -660,11 +670,11 @@
         """
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
+
     enable_log('./log.log', 'DEBUG')
     a = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
-    a.reboot()
-    a.send_cli('ifconfig', type_='super')
+    a.assert_cli('ifconfig', 'fe80::67f:eff:fe01:92be/64')
```

### Comparing `inhandtest-0.0.56/inhandtest/tools.py` & `inhandtest-0.0.57/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.57/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.56
+Version: 0.0.57
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.56/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.57/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.56/setup.py` & `inhandtest-0.0.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.56',
+    version='0.0.57',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

