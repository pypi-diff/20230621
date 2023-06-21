# Comparing `tmp/blipnlptest-0.1.0.tar.gz` & `tmp/blipnlptest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.1.0.tar", max compression
+gzip compressed data, was "blipnlptest-0.1.1.tar", max compression
```

## Comparing `blipnlptest-0.1.0.tar` & `blipnlptest-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-06-20 21:12:16.233468 blipnlptest-0.1.0/blipnlptest/__init__.py
--rw-r--r--   0        0        0     1312 2023-06-21 13:26:15.520462 blipnlptest-0.1.0/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-06-20 19:54:30.133410 blipnlptest-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-06-21 14:51:09.647817 blipnlptest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1328 2023-06-21 13:26:10.082330 blipnlptest-0.1.0/README.md
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 blipnlptest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-21 14:54:05.694918 blipnlptest-0.1.1/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     1312 2023-06-21 13:26:15.520462 blipnlptest-0.1.1/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-06-20 19:54:30.133410 blipnlptest-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-06-21 14:53:37.056593 blipnlptest-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1328 2023-06-21 13:26:10.082330 blipnlptest-0.1.1/README.md
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 blipnlptest-0.1.1/PKG-INFO
```

### Comparing `blipnlptest-0.1.0/blipnlptest/blipnlptest.py` & `blipnlptest-0.1.1/blipnlptest/blipnlptest.py`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.0/LICENSE.txt` & `blipnlptest-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.0/pyproject.toml` & `blipnlptest-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.1.0/README.md` & `blipnlptest-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.0/PKG-INFO` & `blipnlptest-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

