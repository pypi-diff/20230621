# Comparing `tmp/spark_llm-0.1.4.tar.gz` & `tmp/spark_llm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.4.tar", max compression
+gzip compressed data, was "spark_llm-0.1.5.tar", max compression
```

## Comparing `spark_llm-0.1.4.tar` & `spark_llm-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.4/LICENSE
--rw-r--r--   0        0        0     2328 2023-06-19 20:17:51.380866 spark_llm-0.1.4/README.md
--rw-r--r--   0        0        0      926 2023-06-19 20:19:09.082658 spark_llm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.4/spark_llm/__init__.py
--rw-r--r--   0        0        0     2668 2023-06-16 21:50:36.340803 spark_llm-0.1.4/spark_llm/cache.py
--rw-r--r--   0        0        0     1093 2023-06-16 21:50:36.341090 spark_llm-0.1.4/spark_llm/llm_chain_with_cache.py
--rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.4/spark_llm/llm_utils.py
--rw-r--r--   0        0        0     6900 2023-06-19 20:17:59.833736 spark_llm-0.1.4/spark_llm/prompt.py
--rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.4/spark_llm/search_tool_with_cache.py
--rw-r--r--   0        0        0    12623 2023-06-19 20:17:59.879989 spark_llm-0.1.4/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 spark_llm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2608 2023-06-20 22:40:46.469019 spark_llm-0.1.5/README.md
+-rw-r--r--   0        0        0      926 2023-06-20 22:56:10.563144 spark_llm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.5/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2650 2023-06-20 22:56:07.634484 spark_llm-0.1.5/spark_llm/cache.py
+-rw-r--r--   0        0        0     1093 2023-06-20 22:40:29.711290 spark_llm-0.1.5/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.5/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     6900 2023-06-19 20:17:59.833736 spark_llm-0.1.5/spark_llm/prompt.py
+-rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.5/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    12710 2023-06-20 22:56:07.635416 spark_llm-0.1.5/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 spark_llm-0.1.5/PKG-INFO
```

### Comparing `spark_llm-0.1.4/LICENSE` & `spark_llm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.4/README.md` & `spark_llm-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 ## Usage
 ### Initialization
 ```python
 from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
 llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
-assistant=SparkLLMAssistant(llm=llm)
+assistant = SparkLLMAssistant(llm=llm)
 assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
-auto_df=assistant.create_df("2022 USA national auto sales by brand")
+auto_df = assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
 ```
 | rank | brand     | us_sales_2022 | sales_change_vs_2021 |
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
@@ -62,12 +62,19 @@
 ### DataFrame Attribute Verification
 ```python
 auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
 ```
 
 > result: True
 
+### Cache
+The SparkLLMAssistant supports a simple in-memory and persistent cache system. It keeps an in-memory staging cache that can be persisted through the `commit()` method. Cache lookup is always performed on the persistent cache only.
+
+```python
+assistant.commit()
+```
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

### Comparing `spark_llm-0.1.4/pyproject.toml` & `spark_llm-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.4"
+version = "0.1.5"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `spark_llm-0.1.4/spark_llm/cache.py` & `spark_llm-0.1.5/spark_llm/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     lookup is always performed on the persistent cache only.
 
     Attributes:
         _staging_updates: A dictionary to keep track of the in-memory staging updates.
         _sqlite_cache: An SQLiteCache instance that acts as the persistent cache.
     """
 
-    def __init__(self, database_path: str = ".spark_llm.db"):
+    def __init__(self, database_path: str):
         """
         Initializes a new instance of the Cache class.
 
         Args:
             database_path (str, optional): The path to the database file for the SQLiteCache.
                 Defaults to ".spark_llm.db".
         """
```

### Comparing `spark_llm-0.1.4/spark_llm/llm_chain_with_cache.py` & `spark_llm-0.1.5/spark_llm/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.4/spark_llm/llm_utils.py` & `spark_llm-0.1.5/spark_llm/llm_utils.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.4/spark_llm/prompt.py` & `spark_llm-0.1.5/spark_llm/prompt.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.4/spark_llm/search_tool_with_cache.py` & `spark_llm-0.1.5/spark_llm/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.4/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.5/spark_llm/spark_llm_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
         enable_cache: bool = True,
+        cache_file_location: str = ".spark_llm.db",
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
         verbose: bool = False,
     ) -> None:
         """
         Initialize the SparkLLMAssistant object with the provided parameters.
 
@@ -55,15 +56,15 @@
         :param encoding: optional Encoding, cl100k_base will be used if not provided
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         if enable_cache:
-            self._cache = Cache()
+            self._cache = Cache(database_path = cache_file_location)
             self._web_search_tool = SearchToolWithCache(
                 self._web_search_tool, self._cache
             ).search
         else:
             self._cache = None
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
         self._max_tokens_of_web_content = max_tokens_of_web_content
```

### Comparing `spark_llm-0.1.4/PKG-INFO` & `spark_llm-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.4
+Version: 0.1.5
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -38,21 +38,21 @@
 ## Usage
 ### Initialization
 ```python
 from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
 llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
-assistant=SparkLLMAssistant(llm=llm)
+assistant = SparkLLMAssistant(llm=llm)
 assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
-auto_df=assistant.create_df("2022 USA national auto sales by brand")
+auto_df = assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
 ```
 | rank | brand     | us_sales_2022 | sales_change_vs_2021 |
 |------|-----------|---------------|----------------------|
 | 1    | Toyota    | 1849751       | -9                   |
 | 2    | Ford      | 1767439       | -2                   |
 | 3    | Chevrolet | 1502389       | 6                    |
@@ -91,13 +91,20 @@
 ### DataFrame Attribute Verification
 ```python
 auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
 ```
 
 > result: True
 
+### Cache
+The SparkLLMAssistant supports a simple in-memory and persistent cache system. It keeps an in-memory staging cache that can be persisted through the `commit()` method. Cache lookup is always performed on the persistent cache only.
+
+```python
+assistant.commit()
+```
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

