# Comparing `tmp/FlowAnalyzer-0.1.4.tar.gz` & `tmp/FlowAnalyzer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.1.4.tar", last modified: Wed Jun 21 04:39:06 2023, max compression
+gzip compressed data, was "FlowAnalyzer-0.1.5.tar", last modified: Wed Jun 21 14:12:42 2023, max compression
```

## Comparing `FlowAnalyzer-0.1.4.tar` & `FlowAnalyzer-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 04:39:06.269724 FlowAnalyzer-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-21 04:39:06.266723 FlowAnalyzer-0.1.4/FlowAnalyzer/
--rw-rw-rw-   0        0        0     7317 2023-06-21 04:37:18.000000 FlowAnalyzer-0.1.4/FlowAnalyzer/FlowAnalyzer.py
--rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.4/FlowAnalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 04:39:06.268722 FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     6271 2023-06-21 04:39:06.000000 FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-21 04:39:06.000000 FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 04:39:06.000000 FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 04:39:06.000000 FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6271 2023-06-21 04:39:06.268722 FlowAnalyzer-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 04:39:06.269724 FlowAnalyzer-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-21 04:38:59.000000 FlowAnalyzer-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.193653 FlowAnalyzer-0.1.5/FlowAnalyzer/
+-rw-rw-rw-   0        0        0     9264 2023-06-21 14:08:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer/FlowAnalyzer.py
+-rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.5/FlowAnalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.195544 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     6271 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6271 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-21 14:10:34.000000 FlowAnalyzer-0.1.5/setup.py
```

### Comparing `FlowAnalyzer-0.1.4/FlowAnalyzer.egg-info/PKG-INFO` & `FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.4
+Version: 0.1.5
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.4/LICENSE` & `FlowAnalyzer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.4/PKG-INFO` & `FlowAnalyzer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.4
+Version: 0.1.5
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.4/README.md` & `FlowAnalyzer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.4/setup.py` & `FlowAnalyzer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="FlowAnalyzer",
-    version="0.1.4",
+    version="0.1.5",
     description="FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件",
     author="Byxs20",
     author_email="97766819@qq.com",
     packages=find_packages(exclude=["tests", "*.egg-info"]),
     package_data={
         '': ['LICENSE', 'README.md', 'setup.py'],
     },
```

