# Comparing `tmp/blipnlptest-0.0.7.tar.gz` & `tmp/blipnlptest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.0.7.tar", last modified: Tue Jun 20 21:12:39 2023, max compression
+gzip compressed data, was "blipnlptest-0.0.8.tar", last modified: Wed Jun 21 13:27:48 2023, max compression
```

## Comparing `blipnlptest-0.0.7.tar` & `blipnlptest-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.102443 blipnlptest-0.0.7/
--rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 blipnlptest-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1796 2023-06-20 21:12:39.100452 blipnlptest-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1303 2023-06-20 19:54:30.000000 blipnlptest-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.077991 blipnlptest-0.0.7/blipnlptest/
-drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.096457 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/
--rw-rw-rw-   0        0        0     1796 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-20 21:12:39.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-06-20 21:12:16.000000 blipnlptest-0.0.7/blipnlptest/__init__.py
--rw-rw-rw-   0        0        0     1312 2023-06-20 21:11:33.000000 blipnlptest-0.0.7/blipnlptest/blipnlptest.py
--rw-rw-rw-   0        0        0       42 2023-06-20 21:12:39.102443 blipnlptest-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-06-20 21:12:32.000000 blipnlptest-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.468092 blipnlptest-0.0.8/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 blipnlptest-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1821 2023-06-21 13:27:48.467094 blipnlptest-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1328 2023-06-21 13:26:10.000000 blipnlptest-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.454128 blipnlptest-0.0.8/blipnlptest/
+-rw-rw-rw-   0        0        0       43 2023-06-20 21:12:16.000000 blipnlptest-0.0.8/blipnlptest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:27:48.465099 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-06-21 13:27:47.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-21 13:27:48.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1312 2023-06-21 13:26:15.000000 blipnlptest-0.0.8/blipnlptest/blipnlptest.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:27:48.469092 blipnlptest-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-06-21 13:26:33.000000 blipnlptest-0.0.8/setup.py
```

### Comparing `blipnlptest-0.0.7/LICENSE.txt` & `blipnlptest-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.0.7/PKG-INFO` & `blipnlptest-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.0.7
+Version: 0.0.8
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -24,26 +24,31 @@
 
 ## Uso
 
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
-data : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
-key  : chave do bot
-organization : nome do cliente
+df : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
+key  : chave do bot.
 
-Com os parâmetros previamente atribuídos, rodando o código abaixo você terá como saída a exibição do resultado.
+
+Exemplo do código:
 
 <pre><code>
-bnt = BlipNlpTest(data, key)
-result = bnt.test()
+
+import blipnlptest as bnt
+
+
+cc = bnt.contentchecker(df, key)
+result = cc.test()
 display(result)
 </code></pre>
 
+Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado.
 
 A saída contém:
 
 - A mensagem de entrada;
 - Resposta entregue pelo Assistente de Conteudo;
 - Entidades reconhecidas;
 - N intenções, onde N representa o número de colunas/intenções exibidas (onde a primeira é a que obteve maior confiança).
```

### Comparing `blipnlptest-0.0.7/README.md` & `blipnlptest-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,31 @@
 
 ## Uso
 
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
-data : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
-key  : chave do bot
-organization : nome do cliente
+df : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
+key  : chave do bot.
 
-Com os parâmetros previamente atribuídos, rodando o código abaixo você terá como saída a exibição do resultado.
+
+Exemplo do código:
 
 <pre><code>
-bnt = BlipNlpTest(data, key)
-result = bnt.test()
+
+import blipnlptest as bnt
+
+
+cc = bnt.contentchecker(df, key)
+result = cc.test()
 display(result)
 </code></pre>
 
+Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado.
 
 A saída contém:
 
 - A mensagem de entrada;
 - Resposta entregue pelo Assistente de Conteudo;
 - Entidades reconhecidas;
 - N intenções, onde N representa o número de colunas/intenções exibidas (onde a primeira é a que obteve maior confiança).
```

### Comparing `blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/PKG-INFO` & `blipnlptest-0.0.8/blipnlptest/blipnlptest.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.0.7
+Version: 0.0.8
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -24,26 +24,31 @@
 
 ## Uso
 
 Após a instalação do pacote, você terá acesso a classe que permitirá a execução do teste.
 
 Os parâmetros necessários são:
 
-data : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
-key  : chave do bot
-organization : nome do cliente
+df : dataframe de entrada, onde o cabeçalho com as mensagens devem ter como título "Text";
+key  : chave do bot.
 
-Com os parâmetros previamente atribuídos, rodando o código abaixo você terá como saída a exibição do resultado.
+
+Exemplo do código:
 
 <pre><code>
-bnt = BlipNlpTest(data, key)
-result = bnt.test()
+
+import blipnlptest as bnt
+
+
+cc = bnt.contentchecker(df, key)
+result = cc.test()
 display(result)
 </code></pre>
 
+Com os parâmetros previamente atribuídos, rodando o código acima você terá como saída a exibição do resultado.
 
 A saída contém:
 
 - A mensagem de entrada;
 - Resposta entregue pelo Assistente de Conteudo;
 - Entidades reconhecidas;
 - N intenções, onde N representa o número de colunas/intenções exibidas (onde a primeira é a que obteve maior confiança).
```

### Comparing `blipnlptest-0.0.7/blipnlptest/blipnlptest.py` & `blipnlptest-0.0.8/blipnlptest/blipnlptest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 import pandas as pd
 
-class ContentChecker:
+class contentchecker:
 
   def __init__(self, data, key):
       self.data = data
       self.key = key
 
       if isinstance(data, pd.DataFrame) == False:
         print(f'Ao invés de "{data}", favor inserir um DataFrame. A coluna com o texto deve ter o cabeçalho com o nome "Text".')
```

### Comparing `blipnlptest-0.0.7/setup.py` & `blipnlptest-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r", encoding="utf-8") as fh:
 	long_description = fh.read()
 	
 setuptools.setup(
   name = "blipnlptest",
-  version = "0.0.7",
+  version = "0.0.8",
   author = "Caio Souza",
   author_email = "caios@take.net",
   description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.",
   long_description = long_description,
   long_description_content_type="text/markdown",
   keywords = [],
   install_requires=[
```

