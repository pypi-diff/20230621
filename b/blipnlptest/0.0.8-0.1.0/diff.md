# Comparing `tmp/blipnlptest-0.0.8.tar.gz` & `tmp/blipnlptest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.0.8.tar", last modified: Wed Jun 21 13:27:48 2023, max compression
+gzip compressed data, was "blipnlptest-0.1.0.tar", max compression
```

## Comparing `blipnlptest-0.0.8.tar` & `blipnlptest-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.468092 blipnlptest-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 blipnlptest-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1821 2023-06-21 13:27:48.467094 blipnlptest-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1328 2023-06-21 13:26:10.000000 blipnlptest-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.454128 blipnlptest-0.0.8/blipnlptest/
--rw-rw-rw-   0        0        0       43 2023-06-20 21:12:16.000000 blipnlptest-0.0.8/blipnlptest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.465099 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-06-21 13:27:47.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1312 2023-06-21 13:26:15.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.py
--rw-rw-rw-   0        0        0       42 2023-06-21 13:27:48.469092 blipnlptest-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-06-21 13:26:33.000000 blipnlptest-0.0.8/setup.py
+-rw-r--r--   0        0        0       43 2023-06-20 21:12:16.233468 blipnlptest-0.1.0/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     1312 2023-06-21 13:26:15.520462 blipnlptest-0.1.0/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-06-20 19:54:30.133410 blipnlptest-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-06-21 14:51:09.647817 blipnlptest-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1328 2023-06-21 13:26:10.082330 blipnlptest-0.1.0/README.md
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 blipnlptest-0.1.0/PKG-INFO
```

### Comparing `blipnlptest-0.0.8/LICENSE.txt` & `blipnlptest-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.0.8/PKG-INFO` & `blipnlptest-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: blipnlptest
-Version: 0.0.8
-Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
-Author: Caio Souza
-Author-email: caios@take.net
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # BlipNlpTest
 
 Essa é uma classe que permite o teste de mensagens em provedores integrados na plataforma, com o retorno do conteúdo cadastrado no Assistente de Conteudo.
 
 ## Instalação
 
 Para instalar o pacote, basta executar o comando abaixo:
```

### Comparing `blipnlptest-0.0.8/blipnlptest/blipnlptest.py` & `blipnlptest-0.1.0/blipnlptest/blipnlptest.py`

 * *Files identical despite different names*

