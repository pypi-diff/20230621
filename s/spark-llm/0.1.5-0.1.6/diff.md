# Comparing `tmp/spark_llm-0.1.5.tar.gz` & `tmp/spark_llm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.5.tar", max compression
+gzip compressed data, was "spark_llm-0.1.6.tar", max compression
```

## Comparing `spark_llm-0.1.5.tar` & `spark_llm-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.5/LICENSE
--rw-r--r--   0        0        0     2608 2023-06-20 22:40:46.469019 spark_llm-0.1.5/README.md
--rw-r--r--   0        0        0      926 2023-06-20 22:56:10.563144 spark_llm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.5/spark_llm/__init__.py
--rw-r--r--   0        0        0     2650 2023-06-20 22:56:07.634484 spark_llm-0.1.5/spark_llm/cache.py
--rw-r--r--   0        0        0     1093 2023-06-20 22:40:29.711290 spark_llm-0.1.5/spark_llm/llm_chain_with_cache.py
--rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.5/spark_llm/llm_utils.py
--rw-r--r--   0        0        0     6900 2023-06-19 20:17:59.833736 spark_llm-0.1.5/spark_llm/prompt.py
--rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.5/spark_llm/search_tool_with_cache.py
--rw-r--r--   0        0        0    12710 2023-06-20 22:56:07.635416 spark_llm-0.1.5/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 spark_llm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.6/README.md
+-rw-r--r--   0        0        0      947 2023-06-21 20:02:07.581768 spark_llm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.6/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2650 2023-06-21 09:05:46.581124 spark_llm-0.1.6/spark_llm/cache.py
+-rw-r--r--   0        0        0     1946 2023-06-21 20:01:50.301401 spark_llm-0.1.6/spark_llm/code_logger.py
+-rw-r--r--   0        0        0     1093 2023-06-20 22:40:29.711290 spark_llm-0.1.6/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.6/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     8842 2023-06-21 20:01:50.301781 spark_llm-0.1.6/spark_llm/prompt.py
+-rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.6/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    13837 2023-06-21 20:01:50.302232 spark_llm-0.1.6/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.6/PKG-INFO
```

### Comparing `spark_llm-0.1.5/LICENSE` & `spark_llm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.5/README.md` & `spark_llm-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -53,28 +53,49 @@
 ### DataFrame Explanation
 ```python
 auto_top_growth_df.llm.explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
-Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
-
 ### DataFrame Attribute Verification
 ```python
 auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
 ```
 
 > result: True
 
+### UDF Generation
+```python
+@assistant.udf
+def previous_years_sales(brand: str, current_year_sale: int, sales_change_percentage: float) -> int:
+    """Calculate previous years sales from sales change percentage"""
+    ...
+    
+spark.udf.register("previous_years_sales", previous_years_sales)
+auto_df.createOrReplaceTempView("autoDF")
+
+spark.sql("select brand as brand, previous_years_sales(brand, us_sales, sales_change_percentage) as 2021_sales from autoDF").show()
+```
+
+| brand         |2021_sales|
+|---------------|-------------|
+| Toyota        |   2032693|
+| Ford          |   1803509|
+| Chevrolet     |   1417348|
+| Honda         |   1315225|
+| Hyundai       |    739045|
+
 ### Cache
 The SparkLLMAssistant supports a simple in-memory and persistent cache system. It keeps an in-memory staging cache that can be persisted through the `commit()` method. Cache lookup is always performed on the persistent cache only.
 
 ```python
 assistant.commit()
 ```
 
+Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

### Comparing `spark_llm-0.1.5/pyproject.toml` & `spark_llm-0.1.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.5"
+version = "0.1.6"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -25,11 +25,12 @@
 requests = "^2.31.0"
 tiktoken = "0.4.0"
 beautifulsoup4 = "^4.12.2"
 pyspark = "^3.4.0"
 openai = "^0.27.8"
 langchain = "^0.0.201"
 pandas = "^2.0.2"
+pygments = "^2.15.1"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `spark_llm-0.1.5/spark_llm/cache.py` & `spark_llm-0.1.6/spark_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.5/spark_llm/llm_chain_with_cache.py` & `spark_llm-0.1.6/spark_llm/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.5/spark_llm/llm_utils.py` & `spark_llm-0.1.6/spark_llm/llm_utils.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.5/spark_llm/prompt.py` & `spark_llm-0.1.6/spark_llm/prompt.py`

 * *Files 21% similar despite different names*

```diff
@@ -48,35 +48,35 @@
 TRANSFORM_PROMPT = PromptTemplate(
     input_variables=["view_name", "columns", "desc"], template=TRANSFORM_TEMPLATE
 )
 
 EXPLAIN_PREFIX = """You are an Apache Spark SQL expert, who can summary what a dataframe retrieves. Given an analyzed 
 query plan of a dataframe, you will 
 1. convert the dataframe to SQL query. Note that an explain output contains plan 
-nodes separated by "\n". Each plan node has its own expressions and expression ids. 
+nodes separated by `\\n`. Each plan node has its own expressions and expression ids. 
 2. summary what the sql query retrieves. 
 """
 
 EXPLAIN_SUFFIX = "analyzed_plan: {input}\nexplain:"
 
 _plan1 = """
 GlobalLimit 100
     +- LocalLimit 100
-       +- Sort [d_year#778 ASC NULLS FIRST, sum_agg#743 DESC NULLS LAST, brand_id#741 ASC NULLS FIRST], true
-          +- Aggregate [d_year#778, i_brand#912, i_brand_id#911], [d_year#778, i_brand_id#911 AS brand_id#741, i_brand#912 AS brand#742, sum(ss_ext_sales_price#896) AS sum_agg#743]
-             +- Filter (((d_date_sk#772 = ss_sold_date_sk#881) AND (ss_item_sk#883 = i_item_sk#904)) AND ((i_manufact_id#917 = 128) AND (d_moy#780 = 11)))
+       +- Sort [d_year ASC NULLS FIRST, sum_agg DESC NULLS LAST, brand_id ASC NULLS FIRST], true
+          +- Aggregate [d_year, i_brand, i_brand_id], [d_year, i_brand_id AS brand_id, i_brand AS brand, sum(ss_ext_sales_price) AS sum_agg]
+             +- Filter (((d_date_sk = ss_sold_date_sk) AND (ss_item_sk = i_item_sk)) AND ((i_manufact_id = 128) AND (d_moy = 11)))
                 +- Join Inner
                    :- Join Inner
                    :  :- SubqueryAlias dt
-                   :  :  +- SubqueryAlias main.tpcds_sf1_delta.date_dim
-                   :  :     +- Relation main.tpcds_sf1_delta.date_dim[d_date_sk#772,d_date_id#773,d_date#774,d_month_seq#775,d_week_seq#776,d_quarter_seq#777,d_year#778,d_dow#779,d_moy#780,d_dom#781,d_qoy#782,d_fy_year#783,d_fy_quarter_seq#784,d_fy_week_seq#785,d_day_name#786,d_quarter_name#787,d_holiday#788,d_weekend#789,d_following_holiday#790,d_first_dom#791,d_last_dom#792,d_same_day_ly#793,d_same_day_lq#794,d_current_day#795,... 4 more fields] parquet
-                   :  +- SubqueryAlias main.tpcds_sf1_delta.store_sales
-                   :     +- Relation main.tpcds_sf1_delta.store_sales[ss_sold_date_sk#881,ss_sold_time_sk#882,ss_item_sk#883,ss_customer_sk#884,ss_cdemo_sk#885,ss_hdemo_sk#886,ss_addr_sk#887,ss_store_sk#888,ss_promo_sk#889,ss_ticket_number#890L,ss_quantity#891,ss_wholesale_cost#892,ss_list_price#893,ss_sales_price#894,ss_ext_discount_amt#895,ss_ext_sales_price#896,ss_ext_wholesale_cost#897,ss_ext_list_price#898,ss_ext_tax#899,ss_coupon_amt#900,ss_net_paid#901,ss_net_paid_inc_tax#902,ss_net_profit#903] parquet
-                   +- SubqueryAlias main.tpcds_sf1_delta.item
-                      +- Relation main.tpcds_sf1_delta.item[i_item_sk#904,i_item_id#905,i_rec_start_date#906,i_rec_end_date#907,i_item_desc#908,i_current_price#909,i_wholesale_cost#910,i_brand_id#911,i_brand#912,i_class_id#913,i_class#914,i_category_id#915,i_category#916,i_manufact_id#917,i_manufact#918,i_size#919,i_formulation#920,i_color#921,i_units#922,i_container#923,i_manager_id#924,i_product_name#925] parquet
+                   :  :  +- SubqueryAlias spark_catalog.tpcds_sf1_delta.date_dim
+                   :  :     +- Relation spark_catalog.tpcds_sf1_delta.date_dim[d_date_sk,d_date_id,d_date,d_month_seq,d_week_seq,d_quarter_seq,d_year,d_dow,d_moy,d_dom,d_qoy,d_fy_year,d_fy_quarter_seq,d_fy_week_seq,d_day_name,d_quarter_name,d_holiday,d_weekend,d_following_holiday,d_first_dom,d_last_dom,d_same_day_ly,d_same_day_lq,d_current_day,... 4 more fields] parquet
+                   :  +- SubqueryAlias spark_catalog.tpcds_sf1_delta.store_sales
+                   :     +- Relation spark_catalog.tpcds_sf1_delta.store_sales[ss_sold_date_sk,ss_sold_time_sk,ss_item_sk,ss_customer_sk,ss_cdemo_sk,ss_hdemo_sk,ss_addr_sk,ss_store_sk,ss_promo_sk,ss_ticket_numberL,ss_quantity,ss_wholesale_cost,ss_list_price,ss_sales_price,ss_ext_discount_amt,ss_ext_sales_price,ss_ext_wholesale_cost,ss_ext_list_price,ss_ext_tax,ss_coupon_amt,ss_net_paid,ss_net_paid_inc_tax,ss_net_profit] parquet
+                   +- SubqueryAlias spark_catalog.tpcds_sf1_delta.item
+                      +- Relation spark_catalog.tpcds_sf1_delta.item[i_item_sk,i_item_id,i_rec_start_date,i_rec_end_date,i_item_desc,i_current_price,i_wholesale_cost,i_brand_id,i_brand,i_class_id,i_class,i_category_id,i_category,i_manufact_id,i_manufact,i_size,i_formulation,i_color,i_units,i_container,i_manager_id,i_product_name] parquet
 """
 
 _explain1 = """
 The analyzed plan can be translated into the following SQL query:
 ```sql
 SELECT
   dt.d_year,
@@ -119,16 +119,16 @@
 Given a pyspark dataframe `df`.
 The output columns of `df`:
 {columns}
 
 {explain}
 
 Now help me write python code to visualize the result of `df` using plotly:
-1. All the code MUST be in one code block.
-2. There is no need to install any package with pip.
+1. Do NOT use method 'append' of pandas DataFrame. 
+2. There is no need to install any package with pip. 
 3. Show the plot directly, instead of saving into a HTML.
 {instruction}
 """
 
 PLOT_PROMPT = PromptTemplate(
     input_variables=["columns", "explain", "instruction"], template=PLOT_PROMPT_TEMPLATE
 )
@@ -140,14 +140,20 @@
 You will call the function, passing in df as the parameter, and return the output (True/False).
 
 In total, your output must follow the format below, exactly (no explanation words):
 1. function definition f, in Python
 2. 1 blank new line
 3. Call f on df and assign the result to a variable, result: result = name_of_f(df)
 
+Include any necessary import statements INSIDE the function definition.
+For example:
+def gen_random():
+    import random
+    return random.randint(0, 10)
+
 For example:
 Input:
 df = DataFrame[name: string, age: int]
 desc = "expect 5 columns"
 
 Output:
 "def has_5_columns(df) -> bool:
@@ -163,7 +169,79 @@
 result = has_5_columns(df)"
 
 Here is your input df: {df}
 Here is your input description: {desc}
 """
 
 VERIFY_PROMPT = PromptTemplate(input_variables=["df", "desc"], template=VERIFY_TEMPLATE)
+
+UDF_PREFIX = """
+This is the documentation for a PySpark user-defined function (udf): pyspark.sql.functions.udf
+
+A udf creates a deterministic, reusable function in Spark. It can take any data type as a parameter, 
+and by default returns a String (although it can return any data type). 
+The point is to reuse a function on several dataframes and SQL functions.
+
+Given 1) input arguments, 2) a description of the udf functionality,
+3) the udf return type, and 4) the udf function name, 
+generate and return a callable udf.
+        
+Return ONLY the callable resulting udf function (no explanation words). 
+Include any necessary import statements INSIDE the function definition.
+For example:
+def gen_random():
+    import random
+    return random.randint(0, 10)
+"""
+
+UDF_SUFFIX = """
+input_args_types: {input_args_types}
+input_desc: {desc}
+return_type: {return_type}
+udf_name: {udf_name}
+output:\n
+"""
+
+_udf_output1 = """
+def to_upper(s) -> str:
+    if s is not None:
+        return s.upper()
+"""
+
+_udf_output2 = """
+def add_one(x) -> int:
+    if x is not None:
+        return x + 1
+"""
+
+_udf_examples = [{"input_args_types": "(s: str)", 
+                  "desc": "Convert string s to uppercase", 
+                  "return_type": "str", 
+                  "udf_name": "to_upper", 
+                  "output": _udf_output1},
+                {"input_args_types": "(x: int)", 
+                  "desc": "Add 1", 
+                  "return_type": "int", 
+                  "udf_name": "add_one", 
+                  "output": _udf_output2}]
+
+_udf_formatter = """
+input_args_types: {input_args_types}
+desc: {desc}
+return_type: {return_type}
+udf_name: {udf_name}
+output: {output}
+"""
+
+_udf_prompt = PromptTemplate(
+    input_variables=["input_args_types", "desc", "return_type", "udf_name", "output"], template=_udf_formatter
+)
+
+UDF_PROMPT = FewShotPromptTemplate(
+    examples=_udf_examples,
+    example_prompt=_udf_prompt,
+    prefix=UDF_PREFIX,
+    suffix=UDF_SUFFIX,
+    input_variables=["input_args_types", "desc", "return_type", "udf_name"],
+    example_separator="\n\n",
+)
+
```

### Comparing `spark_llm-0.1.5/spark_llm/search_tool_with_cache.py` & `spark_llm-0.1.6/spark_llm/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.5/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.6/spark_llm/spark_llm_assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 from bs4 import BeautifulSoup
 from langchain import LLMChain, GoogleSearchAPIWrapper, BasePromptTemplate
 from langchain.base_language import BaseLanguageModel
 from pyspark.sql import SparkSession, DataFrame
 from tiktoken import Encoding
 
 from spark_llm.cache import Cache
+from spark_llm.code_logger import CodeLogger
 from spark_llm.llm_chain_with_cache import LLMChainWithCache
 from spark_llm.prompt import (
     SEARCH_PROMPT,
     SQL_PROMPT,
     EXPLAIN_DF_PROMPT,
     TRANSFORM_PROMPT,
     PLOT_PROMPT,
     VERIFY_PROMPT,
+    UDF_PROMPT
 )
 from spark_llm.search_tool_with_cache import SearchToolWithCache
 from spark_llm.llm_utils import LLMUtils
 
 
 class SparkLLMAssistant:
     _HTTP_HEADER = {
@@ -70,15 +72,18 @@
         self._max_tokens_of_web_content = max_tokens_of_web_content
         self._search_llm_chain = self._create_llm_chain(prompt=SEARCH_PROMPT)
         self._sql_llm_chain = self._create_llm_chain(prompt=SQL_PROMPT)
         self._explain_chain = self._create_llm_chain(prompt=EXPLAIN_DF_PROMPT)
         self._transform_chain = self._create_llm_chain(prompt=TRANSFORM_PROMPT)
         self._plot_chain = self._create_llm_chain(prompt=PLOT_PROMPT)
         self._verify_chain = self._create_llm_chain(prompt=VERIFY_PROMPT)
+        self._udf_chain = self._create_llm_chain(prompt=UDF_PROMPT)
         self._verbose = verbose
+        if verbose:
+            self._logger = CodeLogger("spark_llm_assistant")
 
     def _create_llm_chain(self, prompt: BasePromptTemplate):
         if self._cache is None:
             return LLMChain(llm=self._llm, prompt=prompt)
 
         return LLMChainWithCache(llm=self._llm, prompt=prompt, cache=self._cache)
 
@@ -143,15 +148,19 @@
             return extracted_blocks
         else:
             # If there are no code blocks, treat the whole text as a single block of code.
             return [text]
 
     def log(self, message: str) -> None:
         if self._verbose:
-            print(message)
+            self._logger.log(message)
+
+    def log_code(self, code: str, language: str) -> None:
+        if self._verbose:
+            self._logger.log_code(code, language)
 
     def _trim_text_from_end(self, text: str, max_tokens: int) -> str:
         """
         Trim text from the end based on the maximum number of tokens allowed.
 
         :param text: text to trim
         :param max_tokens: maximum tokens allowed
@@ -181,15 +190,16 @@
         sql_columns_hint = self._generate_sql_prompt(columns)
 
         # Run the LLM chain to get an ingestion SQL query
         llm_result = self._sql_llm_chain.run(
             query=desc, web_content=web_content, columns=sql_columns_hint
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        self.log(f"SQL query for the ingestion:\n {sql_query}\n")
+        self.log(f"SQL query for the ingestion:\n")
+        self.log_code(sql_query, "sql")
 
         view_name = self._extract_view_name(sql_query)
         self.log(f"Storing data into temp view: {view_name}\n")
         self._spark.sql(sql_query)
         return self._spark.table(view_name)
 
     def _get_df_schema(self, df: DataFrame) -> str:
@@ -253,15 +263,16 @@
         temp_view_name = "temp_view_for_transform"
         df.createOrReplaceTempView(temp_view_name)
         schema_str = self._get_df_schema(df)
         llm_result = self._transform_chain.run(
             view_name=temp_view_name, columns=schema_str, desc=desc
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        self.log(f"SQL query for the transform:\n{sql_query}")
+        self.log(f"SQL query for the transform:")
+        self.log_code(sql_query, "sql")
         return self._spark.sql(sql_query)
 
     def explain_df(self, df: DataFrame) -> str:
         """
         This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
 
         :param df: The Spark DataFrame to be explained.
@@ -293,21 +304,46 @@
         This method creates and runs test cases for the provided PySpark dataframe transformation function.
 
         :param df: The Spark DataFrame to be verified
         :param desc: A description of the expectation to be verified
         """
         llm_output = self._verify_chain.run(df=df, desc=desc)
 
-        self.log(f"Generated code:\n{llm_output}")
+        self.log(f"Generated code:")
+        self.log_code(llm_output, "python")
 
         locals_ = {}
         exec(llm_output, {"df": df}, locals_)
 
         self.log(f"\nResult: {locals_['result']}")
 
+    def udf(self, func: Callable) -> Callable:
+        from inspect import signature
+
+        desc = func.__doc__
+        func_signature = str(signature(func))
+        input_args_types = func_signature.split("->")[0].strip()
+        return_type = func_signature.split("->")[1].strip()
+        udf_name = func.__name__
+
+        code = self._udf_chain.run(
+            input_args_types=input_args_types,
+            desc=desc,
+            return_type=return_type,
+            udf_name=udf_name
+        )
+
+        self.log(f"Creating following Python UDF:")
+        self.log_code(code, "python")
+
+        locals_ = {}
+        exec(code, globals(), locals_)
+
+        return locals_[udf_name]
+
     def activate(self):
         """
         Activates LLM utility functions for Spark DataFrame.
         """
         DataFrame.llm = LLMUtils(self)
 
     def commit(self):
```

### Comparing `spark_llm-0.1.5/PKG-INFO` & `spark_llm-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.5
+Version: 0.1.6
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: langchain (>=0.0.201,<0.0.202)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (==0.4.0)
 Description-Content-Type: text/markdown
 
 # LLM Assistant for Apache Spark
 
@@ -82,29 +83,50 @@
 ### DataFrame Explanation
 ```python
 auto_top_growth_df.llm.explain()
 ```
 
 > In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
-Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
-
 ### DataFrame Attribute Verification
 ```python
 auto_top_growth_df.llm.verify("expect sales change percentage to be between -100 to 100")
 ```
 
 > result: True
 
+### UDF Generation
+```python
+@assistant.udf
+def previous_years_sales(brand: str, current_year_sale: int, sales_change_percentage: float) -> int:
+    """Calculate previous years sales from sales change percentage"""
+    ...
+    
+spark.udf.register("previous_years_sales", previous_years_sales)
+auto_df.createOrReplaceTempView("autoDF")
+
+spark.sql("select brand as brand, previous_years_sales(brand, us_sales, sales_change_percentage) as 2021_sales from autoDF").show()
+```
+
+| brand         |2021_sales|
+|---------------|-------------|
+| Toyota        |   2032693|
+| Ford          |   1803509|
+| Chevrolet     |   1417348|
+| Honda         |   1315225|
+| Hyundai       |    739045|
+
 ### Cache
 The SparkLLMAssistant supports a simple in-memory and persistent cache system. It keeps an in-memory staging cache that can be persisted through the `commit()` method. Cache lookup is always performed on the persistent cache only.
 
 ```python
 assistant.commit()
 ```
 
+Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Licensed under the Apache License 2.0.
```

