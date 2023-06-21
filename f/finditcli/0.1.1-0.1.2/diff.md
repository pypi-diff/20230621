# Comparing `tmp/finditcli-0.1.1.tar.gz` & `tmp/finditcli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finditcli-0.1.1.tar", max compression
+gzip compressed data, was "finditcli-0.1.2.tar", max compression
```

## Comparing `finditcli-0.1.1.tar` & `finditcli-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     2836 2023-06-20 22:57:59.883709 finditcli-0.1.1/README.md
--rw-r--r--   0        0        0      257 2023-06-20 20:58:19.603692 finditcli-0.1.1/file_finder/cli.py
--rw-r--r--   0        0        0      319 2023-06-20 20:47:27.383710 finditcli-0.1.1/file_finder/constants.py
--rw-r--r--   0        0        0      363 2023-06-20 19:22:11.453803 finditcli-0.1.1/file_finder/exceptions.py
--rw-r--r--   0        0        0     5973 2023-06-20 20:48:25.593711 finditcli-0.1.1/file_finder/finder.py
--rw-r--r--   0        0        0      150 2023-06-20 20:49:32.043677 finditcli-0.1.1/file_finder/teste.py
--rw-r--r--   0        0        0     3638 2023-06-20 22:55:42.513693 finditcli-0.1.1/file_finder/utils.py
--rw-r--r--   0        0        0      457 2023-06-20 22:57:07.273707 finditcli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 finditcli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2765 2023-06-21 01:57:01.526555 finditcli-0.1.2/README.md
+-rw-r--r--   0        0        0      253 2023-06-21 02:08:41.986567 finditcli-0.1.2/finditcli/cli.py
+-rw-r--r--   0        0        0      313 2023-06-21 02:06:13.066551 finditcli-0.1.2/finditcli/constants.py
+-rw-r--r--   0        0        0      363 2023-06-21 00:48:56.336550 finditcli-0.1.2/finditcli/exceptions.py
+-rw-r--r--   0        0        0     5985 2023-06-21 02:06:10.866552 finditcli-0.1.2/finditcli/finder.py
+-rw-r--r--   0        0        0     3637 2023-06-21 02:05:05.436564 finditcli-0.1.2/finditcli/utils.py
+-rw-r--r--   0        0        0      451 2023-06-21 02:20:13.566558 finditcli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 finditcli-0.1.2/PKG-INFO
```

### Comparing `finditcli-0.1.1/README.md` & `finditcli-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-**FindItCLI**
+**FinditCLI**
 
-O FindItCLI é um programa em Python que permite pesquisar e gerenciar arquivos em um diretório especificado. Ele oferece opções para buscar arquivos por nome, extensão ou data de modificação e fornece recursos adicionais, como salvar os resultados em um arquivo de relatório e copiar os arquivos encontrados para um diretório específico.
+O FinditCLI é um programa em Python que permite pesquisar e gerenciar arquivos em um diretório especificado. Ele oferece opções para buscar arquivos por nome, extensão ou data de modificação e fornece recursos adicionais, como salvar os resultados em um arquivo de relatório e copiar os arquivos encontrados para um diretório específico.
 
 ## Instalação
 
-Para executar o FindItCLI, você precisa ter o Python instalado em seu sistema. Além disso, você precisa instalar as dependências do programa. Para fazer isso, siga as etapas abaixo:
+Para executar o FinditCLI, você precisa ter o Python instalado em seu sistema. Além disso, você precisa instalar as dependências do programa. Para fazer isso, siga as etapas abaixo:
 
-1. Clone o repositório do FindItCLI:
+1. Clone o repositório do FinditCLI:
 
 ```
-git clone https://github.com/seu-usuario/file-finder.git
+git clone https://github.com/seu-usuario/pathFinder.git
 ```
 
 2. Acesse o diretório do projeto:
 
 ```
 cd file-finder
 ```
@@ -32,19 +32,14 @@
 ```
 
 - Linux/Mac:
 ```
 source venv/bin/activate
 ```
 
-5. Instale as dependências:
-
-```
-pip install -r requirements.txt
-```
 
 ## Uso
 
 Após concluir a instalação, você pode executar o programa usando o seguinte comando:
 
 ```
 python file_finder.py [diretório] -k [chave] -v [valor] [-r] [-s] [-c [diretório_destino]]
```

### Comparing `finditcli-0.1.1/file_finder/finder.py` & `finditcli-0.1.2/finditcli/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import click
 import shutil
 from tabulate import tabulate
 from pathlib import Path
 from datetime import datetime
-from file_finder.utils import get_folders
-from file_finder.utils import get_files_details
-from file_finder.constants import SEARCH_MAPPING
-from file_finder.constants import TABLE_HEADERS
-from file_finder.exceptions import FileFinderError
-from file_finder.exceptions import InvalidInputError
-from file_finder.exceptions import ZeroFilesFoundError
+from finditcli.utils import get_folders
+from finditcli.utils import get_files_details
+from finditcli.constants import SEARCH_MAPPING
+from finditcli.constants import TABLE_HEADERS
+from finditcli.exceptions import FileFinderError
+from finditcli.exceptions import InvalidInputError
+from finditcli.exceptions import ZeroFilesFoundError
 
 
 def process_search(path, key, value, recursive):
     """Detém toda lógica necessária para realizar a pesquisa
     conforme os inputs do usuário
 
     Args:
@@ -38,15 +38,15 @@
 
 def process_results(files, key, value):
     """Processa os resultados da pesquisa, exibindo-os na tela em formato
     de tabela.
 
     Args:
         files (_type_): Uma lista de objetos Path(), cada um representando um
-     arquivo encontrado pela pesquisa
+    arquivo encontrado pela pesquisa
         key (_type_): str que representa a chave de pesquisa.
         value (_type_): str que representa o nome que os arquivos podem ter.
 
     Returns:
         _type_: A string que representa os resultados tabulados.
     """
     if not files:
@@ -108,16 +108,16 @@
 
 @click.command()
 @click.argument("path", default="")
 @click.option(
     "-k",
     "--key",
     required=True,
-    type=click.Choice(SEARCH_MAPPING.keys()),
-    help="Define a cave de pesquisa. Pode ser 'name', 'ext' ou qualquer outra string para pesquisar por data de modificação.",
+    type=click.Choice(list(SEARCH_MAPPING.keys())),
+    help="Define a chave da pesquisa. Pode ser 'name', 'ext' ou 'mod' para pesquisar por nome, extensão ou data de modificação, respectivamente.",
 )
 @click.option(
     "-v", "--value", required=True, help="Define o valor da chave de pesquisa."
 )
 @click.option(
     "-r",
     "--recursive",
```

### Comparing `finditcli-0.1.1/file_finder/utils.py` & `finditcli-0.1.2/finditcli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
+from finditcli.exceptions import InvalidInputError
 import platform
-from file_finder.exceptions import InvalidInputError
 
 
 def get_folders(path):
     """Obtém os subdiretórios no diretório pesquisado.
 
     Args:
         path (str): um objeto Path() que representa o diretório.
@@ -107,8 +107,9 @@
         files_details.append(details)
     return files_details
 
 
 def get_created_timestamp(stat):
     if platform.system() == "Darwin":
         return stat.st_birthtime
+
     return stat.st_ctime
```

### Comparing `finditcli-0.1.1/PKG-INFO` & `finditcli-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: finditcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: dgeison
 Author-email: dgeison.peixoto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datetime (>=5.1,<6.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-**FindItCLI**
+**FinditCLI**
 
-O FindItCLI é um programa em Python que permite pesquisar e gerenciar arquivos em um diretório especificado. Ele oferece opções para buscar arquivos por nome, extensão ou data de modificação e fornece recursos adicionais, como salvar os resultados em um arquivo de relatório e copiar os arquivos encontrados para um diretório específico.
+O FinditCLI é um programa em Python que permite pesquisar e gerenciar arquivos em um diretório especificado. Ele oferece opções para buscar arquivos por nome, extensão ou data de modificação e fornece recursos adicionais, como salvar os resultados em um arquivo de relatório e copiar os arquivos encontrados para um diretório específico.
 
 ## Instalação
 
-Para executar o FindItCLI, você precisa ter o Python instalado em seu sistema. Além disso, você precisa instalar as dependências do programa. Para fazer isso, siga as etapas abaixo:
+Para executar o FinditCLI, você precisa ter o Python instalado em seu sistema. Além disso, você precisa instalar as dependências do programa. Para fazer isso, siga as etapas abaixo:
 
-1. Clone o repositório do FindItCLI:
+1. Clone o repositório do FinditCLI:
 
 ```
-git clone https://github.com/seu-usuario/file-finder.git
+git clone https://github.com/seu-usuario/pathFinder.git
 ```
 
 2. Acesse o diretório do projeto:
 
 ```
 cd file-finder
 ```
@@ -49,19 +49,14 @@
 ```
 
 - Linux/Mac:
 ```
 source venv/bin/activate
 ```
 
-5. Instale as dependências:
-
-```
-pip install -r requirements.txt
-```
 
 ## Uso
 
 Após concluir a instalação, você pode executar o programa usando o seguinte comando:
 
 ```
 python file_finder.py [diretório] -k [chave] -v [valor] [-r] [-s] [-c [diretório_destino]]
```

