# Comparing `tmp/embedchain-0.0.3.tar.gz` & `tmp/embedchain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.3.tar", last modified: Tue Jun 20 15:38:46 2023, max compression
+gzip compressed data, was "embedchain-0.0.4.tar", last modified: Tue Jun 20 16:18:19 2023, max compression
```

## Comparing `embedchain-0.0.3.tar` & `embedchain-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.807260 embedchain-0.0.3/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.3/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 15:38:46.807106 embedchain-0.0.3/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     5668 2023-06-20 15:38:37.000000 embedchain-0.0.3/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.799258 embedchain-0.0.3/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.806274 embedchain-0.0.3/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.3/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     4451 2023-06-20 15:38:37.000000 embedchain-0.0.3/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.806888 embedchain-0.0.3/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.3/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.800103 embedchain-0.0.3/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-20 15:38:46.807297 embedchain-0.0.3/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      966 2023-06-20 15:38:37.000000 embedchain-0.0.3/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 16:18:19.640077 embedchain-0.0.4/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.4/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 16:18:19.639936 embedchain-0.0.4/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     5656 2023-06-20 15:49:54.000000 embedchain-0.0.4/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 16:18:19.637619 embedchain-0.0.4/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 16:18:19.639168 embedchain-0.0.4/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.4/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     6661 2023-06-20 16:10:45.000000 embedchain-0.0.4/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 16:18:19.639715 embedchain-0.0.4/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.4/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.4/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 16:18:19.638365 embedchain-0.0.4/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 16:18:19.000000 embedchain-0.0.4/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-20 16:18:19.000000 embedchain-0.0.4/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-20 16:18:19.000000 embedchain-0.0.4/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-20 16:18:19.000000 embedchain-0.0.4/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-20 16:18:19.000000 embedchain-0.0.4/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-20 16:18:19.640113 embedchain-0.0.4/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      978 2023-06-20 16:10:45.000000 embedchain-0.0.4/setup.py
```

### Comparing `embedchain-0.0.3/LICENSE` & `embedchain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/PKG-INFO` & `embedchain-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.3
-Summary: embedchain is a framework to easily create bots over any dataset
+Version: 0.0.4
+Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -16,15 +16,15 @@
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
-* If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
@@ -105,15 +105,15 @@
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
-Note that we do not support password protected pdfs as of now.
+Note that we do not support password protected pdfs.
 
 ### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
@@ -148,15 +148,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
+- [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.3/README.md` & `embedchain-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
-* If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
@@ -91,15 +91,15 @@
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
-Note that we do not support password protected pdfs as of now.
+Note that we do not support password protected pdfs.
 
 ### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
@@ -134,15 +134,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
+- [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.3/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.4/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/embedchain/loaders/pdf_file.py` & `embedchain-0.0.4/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/embedchain/loaders/web_page.py` & `embedchain-0.0.4/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/embedchain/loaders/youtube_video.py` & `embedchain-0.0.4/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.4/embedchain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.3
-Summary: embedchain is a framework to easily create bots over any dataset
+Version: 0.0.4
+Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -16,15 +16,15 @@
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
-* If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
@@ -105,15 +105,15 @@
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
-Note that we do not support password protected pdfs as of now.
+Note that we do not support password protected pdfs.
 
 ### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
@@ -148,15 +148,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
+- [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.3/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.4/embedchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.3/setup.py` & `embedchain-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.3",
+    version="0.0.4",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
-    description="embedchain is a framework to easily create bots over any dataset",
+    description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

