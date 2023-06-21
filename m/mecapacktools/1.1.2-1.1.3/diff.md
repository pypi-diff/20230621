# Comparing `tmp/mecapacktools-1.1.2.tar.gz` & `tmp/mecapacktools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.1.2.tar", max compression
+gzip compressed data, was "mecapacktools-1.1.3.tar", max compression
```

## Comparing `mecapacktools-1.1.2.tar` & `mecapacktools-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.1.2/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.1.2/mecapacktools/libCfg.py
--rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.1.2/mecapacktools/libFTP.py
--rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.1.2/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.1.2/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.1.2/mecapacktools/libSql.py
--rw-r--r--   0        0        0    16463 2023-06-15 10:07:47.700051 mecapacktools-1.1.2/mecapacktools/libTool.py
--rw-r--r--   0        0        0    20319 2023-06-07 08:51:38.798095 mecapacktools-1.1.2/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1161 2023-06-15 10:08:06.942286 mecapacktools-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.1.2/README.md
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mecapacktools-1.1.2/setup.py
--rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mecapacktools-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.1.3/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.1.3/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.1.3/mecapacktools/libFTP.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.1.3/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.1.3/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.1.3/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    16463 2023-06-15 10:07:47.700051 mecapacktools-1.1.3/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20375 2023-06-21 08:08:19.048994 mecapacktools-1.1.3/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1161 2023-06-21 08:08:25.054378 mecapacktools-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.1.3/README.md
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mecapacktools-1.1.3/setup.py
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mecapacktools-1.1.3/PKG-INFO
```

### Comparing `mecapacktools-1.1.2/LICENSE` & `mecapacktools-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libCfg.py` & `mecapacktools-1.1.3/mecapacktools/libCfg.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libFTP.py` & `mecapacktools-1.1.3/mecapacktools/libFTP.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libLog.py` & `mecapacktools-1.1.3/mecapacktools/libLog.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libMail.py` & `mecapacktools-1.1.3/mecapacktools/libMail.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libSql.py` & `mecapacktools-1.1.3/mecapacktools/libSql.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libTool.py` & `mecapacktools-1.1.3/mecapacktools/libTool.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/mecapacktools/libWebServices.py` & `mecapacktools-1.1.3/mecapacktools/libWebServices.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     #: Variables
     hshParam = {}
     hshParam["auth_cognito"] = {"address": "", "login": "", "pwd": ""}
     hshParam["auth"] = {"adress": "", "societe": ""}
     hshParam["request"] = {}
     hshParam["MaxRetryError"] = {"IterationMax": 2, "timeSleep": 120}
     __hshData = {}
+    retour_ligne = "<cr/>"
 
     @property
     def data(self):
         """
         return data
 
         Returns:
@@ -395,14 +396,15 @@
 
     #: Variables
     hshParam = {}
     hshParam["adress"] = ""
     hshParam = {"adress": "", "user": "", "password": ""}
     hshParam["request"] = [{"action": "", "param": ""}]
     __hshData = {}
+    retour_ligne = "&#10;"
 
     @property
     def data(self):
         """
         return data
 
         Returns:
```

### Comparing `mecapacktools-1.1.2/pyproject.toml` & `mecapacktools-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
```

### Comparing `mecapacktools-1.1.2/README.md` & `mecapacktools-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.2/setup.py` & `mecapacktools-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': '',
     'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n- FTP \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mecapacktools-1.1.2/PKG-INFO` & `mecapacktools-1.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

