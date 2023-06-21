# Comparing `tmp/embedchain-0.0.5.tar.gz` & `tmp/embedchain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.5.tar", last modified: Wed Jun 21 07:10:20 2023, max compression
+gzip compressed data, was "embedchain-0.0.6.tar", last modified: Wed Jun 21 10:40:49 2023, max compression
```

## Comparing `embedchain-0.0.5.tar` & `embedchain-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 07:10:20.105926 embedchain-0.0.5/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.5/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     6142 2023-06-21 07:10:20.105808 embedchain-0.0.5/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     5647 2023-06-21 07:09:55.000000 embedchain-0.0.5/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 07:10:20.103325 embedchain-0.0.5/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 07:10:20.105092 embedchain-0.0.5/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.5/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     6657 2023-06-21 07:09:55.000000 embedchain-0.0.5/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 07:10:20.105636 embedchain-0.0.5/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.5/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.5/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 07:10:20.104125 embedchain-0.0.5/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     6142 2023-06-21 07:10:20.000000 embedchain-0.0.5/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-21 07:10:20.000000 embedchain-0.0.5/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-21 07:10:20.000000 embedchain-0.0.5/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-21 07:10:20.000000 embedchain-0.0.5/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-21 07:10:20.000000 embedchain-0.0.5/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-21 07:10:20.105957 embedchain-0.0.5/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      978 2023-06-21 07:09:55.000000 embedchain-0.0.5/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.550436 embedchain-0.0.6/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.6/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     6349 2023-06-21 10:40:49.550268 embedchain-0.0.6/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     5854 2023-06-21 10:39:51.000000 embedchain-0.0.6/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.547526 embedchain-0.0.6/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.549232 embedchain-0.0.6/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.6/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     6661 2023-06-21 10:39:51.000000 embedchain-0.0.6/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.550006 embedchain-0.0.6/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.6/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.548414 embedchain-0.0.6/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     6349 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-21 10:40:49.550475 embedchain-0.0.6/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-21 10:39:51.000000 embedchain-0.0.6/setup.py
```

### Comparing `embedchain-0.0.5/LICENSE` & `embedchain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/PKG-INFO` & `embedchain-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,30 +14,30 @@
 
 # embedchain
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.qna` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
@@ -78,18 +78,18 @@
 from embedchain import App as EmbedChainApp
 
 # or
 
 from embedchain import App as ECApp
 ```
 
-* Now your app is created. You can use `.qna` function to get the answer for any query.
+* Now your app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
@@ -115,14 +115,18 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### More Formats coming soon
+
+* If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
+
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
 
 * load the data
 * create meaningful chunks
 * create embeddigns for each chunk
@@ -142,15 +146,15 @@
 * Should I store meta data along with the embeddings?
 * How should I find similar documents for a query? Which ranking model should I use?
 
 These questions may be trivial for some but for a lot of us, it needs research, experimentation and time to find out the accurate answers.
 
 embedchain is a framework which takes care of all these nuances and provides a simple interface to create bots over any dataset.
 
-In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.qna` function to get the relevant answer.
+In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
 - [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
```

### Comparing `embedchain-0.0.5/README.md` & `embedchain-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # embedchain
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.qna` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
@@ -64,18 +64,18 @@
 from embedchain import App as EmbedChainApp
 
 # or
 
 from embedchain import App as ECApp
 ```
 
-* Now your app is created. You can use `.qna` function to get the answer for any query.
+* Now your app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
@@ -101,14 +101,18 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### More Formats coming soon
+
+* If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
+
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
 
 * load the data
 * create meaningful chunks
 * create embeddigns for each chunk
@@ -128,15 +132,15 @@
 * Should I store meta data along with the embeddings?
 * How should I find similar documents for a query? Which ranking model should I use?
 
 These questions may be trivial for some but for a lot of us, it needs research, experimentation and time to find out the accurate answers.
 
 embedchain is a framework which takes care of all these nuances and provides a simple interface to create bots over any dataset.
 
-In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.qna` function to get the relevant answer.
+In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
 - [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
```

### Comparing `embedchain-0.0.5/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.6/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/embedchain/embedchain.py` & `embedchain-0.0.6/embedchain/embedchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         {context}
         Query: {query}
         Helpful Answer:
         """
         answer = self.get_openai_answer(prompt)
         return answer
 
-    def qna(self, input_query):
+    def query(self, input_query):
         """
         Queries the vector database based on the given input query.
         Gets relevant doc based on the query and then passes it to an
         LLM as context to get the answer.
 
         :param input_query: The query to use.
         :return: The answer to the query.
@@ -190,10 +190,10 @@
 
 class App(EmbedChain):
     """
     The EmbedChain app.
     Has two functions: add and query.
 
     adds(data_type, url): adds the data from the given URL to the vector db.
-    qna(query): finds answer to the given query using vector database and LLM.
+    query(query): finds answer to the given query using vector database and LLM.
     """
     pass
```

### Comparing `embedchain-0.0.5/embedchain/loaders/pdf_file.py` & `embedchain-0.0.6/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/embedchain/loaders/web_page.py` & `embedchain-0.0.6/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/embedchain/loaders/youtube_video.py` & `embedchain-0.0.6/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.6/embedchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,30 +14,30 @@
 
 # embedchain
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.qna` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
@@ -78,18 +78,18 @@
 from embedchain import App as EmbedChainApp
 
 # or
 
 from embedchain import App as ECApp
 ```
 
-* Now your app is created. You can use `.qna` function to get the answer for any query.
+* Now your app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(naval_chat_bot.qna("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
@@ -115,14 +115,18 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### More Formats coming soon
+
+* If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
+
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
 
 * load the data
 * create meaningful chunks
 * create embeddigns for each chunk
@@ -142,15 +146,15 @@
 * Should I store meta data along with the embeddings?
 * How should I find similar documents for a query? Which ranking model should I use?
 
 These questions may be trivial for some but for a lot of us, it needs research, experimentation and time to find out the accurate answers.
 
 embedchain is a framework which takes care of all these nuances and provides a simple interface to create bots over any dataset.
 
-In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.qna` function to get the relevant answer.
+In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
 - [Langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
```

### Comparing `embedchain-0.0.5/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.6/embedchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.5/setup.py` & `embedchain-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.5",
+    version="0.0.6",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
     description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
@@ -26,8 +26,8 @@
         "openai",
         "chromadb>=0.3.26",
         "youtube-transcript-api",
         "beautifulsoup4",
         "pypdf",
         "pytube",
     ]
-)
+)
```

