# Comparing `tmp/chanpackage-0.2.tar.gz` & `tmp/chanpackage-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanpackage-0.2.tar", last modified: Mon Jun 19 06:20:27 2023, max compression
+gzip compressed data, was "chanpackage-0.3.tar", last modified: Wed Jun 21 08:34:04 2023, max compression
```

## Comparing `chanpackage-0.2.tar` & `chanpackage-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.442341 chanpackage-0.2/
--rw-rw-rw-   0        0        0      188 2023-06-19 06:20:27.441340 chanpackage-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.435342 chanpackage-0.2/chanpackage.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 06:20:27.443339 chanpackage-0.2/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-19 06:20:02.000000 chanpackage-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.439340 chanpackage-0.2/zabbix/
--rw-rw-rw-   0        0        0        0 2023-06-19 06:16:27.000000 chanpackage-0.2/zabbix/__init__.py
--rw-rw-rw-   0        0        0    10362 2023-06-19 05:03:14.000000 chanpackage-0.2/zabbix/get_Availability_report.py
--rw-rw-rw-   0        0        0     1773 2023-06-19 06:19:30.000000 chanpackage-0.2/zabbix/login_zabbix.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:34:04.376671 chanpackage-0.3/
+-rw-rw-rw-   0        0        0      189 2023-06-21 08:34:04.375669 chanpackage-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 08:34:04.369666 chanpackage-0.3/chanpackage.egg-info/
+-rw-rw-rw-   0        0        0      189 2023-06-21 08:34:04.000000 chanpackage-0.3/chanpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-21 08:34:04.000000 chanpackage-0.3/chanpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:34:04.000000 chanpackage-0.3/chanpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 08:33:24.000000 chanpackage-0.3/chanpackage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-06-21 08:34:04.000000 chanpackage-0.3/chanpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 08:34:04.000000 chanpackage-0.3/chanpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 08:34:04.377669 chanpackage-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      411 2023-06-21 08:33:51.000000 chanpackage-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:34:04.373669 chanpackage-0.3/zabbix/
+-rw-rw-rw-   0        0        0        0 2023-06-19 08:38:34.000000 chanpackage-0.3/zabbix/__init__.py
+-rw-rw-rw-   0        0        0    10362 2023-06-19 05:03:14.000000 chanpackage-0.3/zabbix/get_Availability_report.py
+-rw-rw-rw-   0        0        0     1773 2023-06-19 06:19:30.000000 chanpackage-0.3/zabbix/login_zabbix.py
```

### Comparing `chanpackage-0.2/zabbix/get_Availability_report.py` & `chanpackage-0.3/zabbix/get_Availability_report.py`

 * *Files identical despite different names*

### Comparing `chanpackage-0.2/zabbix/login_zabbix.py` & `chanpackage-0.3/zabbix/login_zabbix.py`

 * *Files identical despite different names*

