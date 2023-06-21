# Comparing `tmp/openborders-0.1.1.post3.tar.gz` & `tmp/openborders-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openborders-0.1.1.post3.tar", max compression
+gzip compressed data, was "openborders-0.1.2.tar", max compression
```

## Comparing `openborders-0.1.1.post3.tar` & `openborders-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1735 2023-06-20 22:08:25.003241 openborders-0.1.1.post3/data/gdim.columns.json
--rw-r--r--   0        0        0      851 2023-06-20 19:26:13.994401 openborders-0.1.1.post3/data/isocodes.csv
--rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.1.post3/openborders/__init__.py
--rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.1.post3/openborders/cli.py
--rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.1.post3/openborders/data.py
--rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.1.post3/openborders/indices.py
--rw-r--r--   0        0        0      499 2023-06-21 14:04:54.128527 openborders-0.1.1.post3/openborders/utils.py
--rw-r--r--   0        0        0     1206 2023-06-21 14:07:20.813970 openborders-0.1.1.post3/pyproject.toml
--rw-r--r--   0        0        0      895 2023-06-21 12:18:59.512183 openborders-0.1.1.post3/README.md
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 openborders-0.1.1.post3/PKG-INFO
+-rw-r--r--   0        0        0     1735 2023-06-20 22:08:25.003241 openborders-0.1.2/data/gdim.columns.json
+-rw-r--r--   0        0        0      851 2023-06-20 19:26:13.994401 openborders-0.1.2/data/isocodes.csv
+-rw-r--r--   0        0        0      202 2023-06-21 05:01:43.184465 openborders-0.1.2/openborders/__init__.py
+-rw-r--r--   0        0        0     5511 2023-06-21 12:12:49.976324 openborders-0.1.2/openborders/cli.py
+-rw-r--r--   0        0        0    12956 2023-06-21 08:17:56.339418 openborders-0.1.2/openborders/data.py
+-rw-r--r--   0        0        0    10585 2023-06-21 12:14:22.711631 openborders-0.1.2/openborders/indices.py
+-rw-r--r--   0        0        0      499 2023-06-21 14:04:54.128527 openborders-0.1.2/openborders/utils.py
+-rw-r--r--   0        0        0     1200 2023-06-21 15:29:01.734930 openborders-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1030 2023-06-21 14:44:29.062188 openborders-0.1.2/README.md
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 openborders-0.1.2/PKG-INFO
```

### Comparing `openborders-0.1.1.post3/data/gdim.columns.json` & `openborders-0.1.2/data/gdim.columns.json`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post3/data/isocodes.csv` & `openborders-0.1.2/data/isocodes.csv`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post3/openborders/cli.py` & `openborders-0.1.2/openborders/cli.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post3/openborders/data.py` & `openborders-0.1.2/openborders/data.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post3/openborders/indices.py` & `openborders-0.1.2/openborders/indices.py`

 * *Files identical despite different names*

### Comparing `openborders-0.1.1.post3/pyproject.toml` & `openborders-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openborders"
-version = "0.1.1-post3"
+version = "0.1.2"
 description = ""
 authors = ["arnos-stuff <mail@arnov.dev>"]
 readme = "README.md"
 homepage = "https://arnos-stuff.github.io/open-borders-index"
 
 include = [
     "data/gdim.columns.json",
```

### Comparing `openborders-0.1.1.post3/README.md` & `openborders-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 * `-o` means output to file, extension is detected (`.csv`|`.xlsx`|`.json`)
 
 
 ## Example result
 
 A sample CSV file can be found [here](tests/open-borders-index.csv)
 
+## Vote for your metrics, propose yours !
+
+See the poll [available on the strawpoll website](https://strawpoll.com/polls/X3nk4ReRzgE)
+
 ## Credits
 
 This toolbox heavily relies on the work from the folks at [wbdata](https://github.com/OliverSherouse/wbdata) and overall APIs of
 international organisations:
 
 - [World Bank API](https://data.worldbank.org/)
 - [World Bank's GDIM][1] which is the Global Database on Intergenerational Mobility
```

### Comparing `openborders-0.1.1.post3/PKG-INFO` & `openborders-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openborders
-Version: 0.1.1.post3
+Version: 0.1.2
 Summary: 
 Home-page: https://arnos-stuff.github.io/open-borders-index
 Author: arnos-stuff
 Author-email: mail@arnov.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -40,14 +40,18 @@
 * `-o` means output to file, extension is detected (`.csv`|`.xlsx`|`.json`)
 
 
 ## Example result
 
 A sample CSV file can be found [here](tests/open-borders-index.csv)
 
+## Vote for your metrics, propose yours !
+
+See the poll [available on the strawpoll website](https://strawpoll.com/polls/X3nk4ReRzgE)
+
 ## Credits
 
 This toolbox heavily relies on the work from the folks at [wbdata](https://github.com/OliverSherouse/wbdata) and overall APIs of
 international organisations:
 
 - [World Bank API](https://data.worldbank.org/)
 - [World Bank's GDIM][1] which is the Global Database on Intergenerational Mobility
```

