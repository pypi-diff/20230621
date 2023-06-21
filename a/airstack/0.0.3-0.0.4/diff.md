# Comparing `tmp/airstack-0.0.3.tar.gz` & `tmp/airstack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airstack-0.0.3.tar", last modified: Mon Jun 19 07:46:44 2023, max compression
+gzip compressed data, was "airstack-0.0.4.tar", last modified: Wed Jun 21 06:18:15 2023, max compression
```

## Comparing `airstack-0.0.3.tar` & `airstack-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.267694 airstack-0.0.3/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-19 07:46:44.267760 airstack-0.0.3/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2785 2023-06-19 07:46:20.000000 airstack-0.0.3/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 airstack-0.0.3/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      704 2023-06-19 07:46:44.268016 airstack-0.0.3/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.265411 airstack-0.0.3/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.266708 airstack-0.0.3/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     8401 2023-06-19 07:46:20.000000 airstack-0.0.3/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     8894 2023-06-19 07:46:20.000000 airstack-0.0.3/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 airstack-0.0.3/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-19 07:46:44.267540 airstack-0.0.3/src/airstack.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      346 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/requires.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-19 07:46:44.000000 airstack-0.0.3/src/airstack.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 06:18:15.176385 airstack-0.0.4/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-21 06:18:15.176475 airstack-0.0.4/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2785 2023-06-19 07:46:20.000000 airstack-0.0.4/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 airstack-0.0.4/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      704 2023-06-21 06:18:15.176747 airstack-0.0.4/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 06:18:15.172841 airstack-0.0.4/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 06:18:15.175175 airstack-0.0.4/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 airstack-0.0.4/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 airstack-0.0.4/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     9033 2023-06-21 06:14:44.000000 airstack-0.0.4/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8944 2023-06-21 06:14:44.000000 airstack-0.0.4/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)    25580 2023-06-21 06:14:44.000000 airstack-0.0.4/src/airstack/popular_queries.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 airstack-0.0.4/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 06:18:15.176245 airstack-0.0.4/src/airstack.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-21 06:18:15.000000 airstack-0.0.4/src/airstack.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      378 2023-06-21 06:18:15.000000 airstack-0.0.4/src/airstack.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-21 06:18:15.000000 airstack-0.0.4/src/airstack.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-21 06:18:15.000000 airstack-0.0.4/src/airstack.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-21 06:18:15.000000 airstack-0.0.4/src/airstack.egg-info/top_level.txt
```

### Comparing `airstack-0.0.3/PKG-INFO` & `airstack-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `airstack-0.0.3/README.md` & `airstack-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `airstack-0.0.3/setup.cfg` & `airstack-0.0.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airstack
-version = 0.0.3
+version = 0.0.4
 author = Airstack
 author_email = support@airstack.xyz
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `airstack-0.0.3/src/airstack/execute_query.py` & `airstack-0.0.4/src/airstack/execute_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 import json
 import warnings
 import re
 from graphql import parse, print_ast, visit
 from airstack.send_request import SendRequest
-from graphql.language.ast import OperationDefinition
 from airstack.generic import (
     find_page_info,
     add_cursor_to_input_field,
     replace_cursor_value,
     has_cursor,
     RemoveQueryByStartingName,
     add_page_info_to_queries,
@@ -62,20 +61,40 @@
         """
         self.url = AirstackConstants.API_ENDPOINT_PROD if url is None else url
         if api_key is None:
             raise ValueError("API key must be provided.")
 
         self.timeout = AirstackConstants.API_TIMEOUT
         self.api_key = api_key
-    
+
     def create_execute_query_object(self, query=None, variables=None):
-        # Create a new object using the caller's `self` variables
-        execute_query = ExecuteQuery(query=query, variables=variables, url=self.url, api_key=self.api_key, timeout=self.timeout)
+        """Create execute query object for every query
+
+        Args:
+            query (str, optional): query. Defaults to None.
+            variables (dict, optional): variables for the query. Defaults to None.
+
+        Returns:
+            object: execute query obiect
+        """
+        execute_query = ExecuteQuery(query=query, variables=variables, url=self.url,
+        api_key=self.api_key, timeout=self.timeout)
         return execute_query
 
+    def create_popular_queries_object(self):
+        """Create popular query object for popular queries
+
+        Returns:
+            object: execute popular query obiect
+        """
+        from airstack.popular_queries import ExecutePopularQueries
+        execute_popular_query = ExecutePopularQueries(url=self.url,api_key=self.api_key,
+        timeout=self.timeout)
+        return execute_popular_query
+
 class ExecuteQuery:
     """Class to execute query functions
 
     Returns:
         object: object of execute query
     """
     def __init__(self, query=None, variables=None, url=None, api_key=None, timeout=None):
@@ -96,15 +115,15 @@
 
         Returns:
             Tuple: GraphQL response data or None, GraphQL response status code,
             error message or None
         """
         if query is None:
             query = self.query
-            
+
         headers = {
             'Content-Type': 'application/json',
             'Authorization': self.api_key
         }
         payload = {
             'query': query,
             'variables': self.variables
@@ -133,15 +152,16 @@
         regex = re.compile(r'pageInfo')
         has_page_info = regex.search(query)
         if has_page_info is None:
             query = add_page_info_to_queries(query)
 
         query_response = await self.execute_query(query=query)
         if query_response.error is not None:
-            return QueryResponse(None, query_response.status_code, query_response.error, None, None, None, None)
+            return QueryResponse(None, query_response.status_code, query_response.error,
+            None, None, None, None)
 
         page_info = {}
         for _key, value in query_response.data.items():
             page_info[_key] = find_page_info(query_response.data[_key])
 
         has_next_page = any(page_info['nextCursor'] != '' for page_info in page_info.values())
         has_prev_page = any(page_info['prevCursor'] != '' for page_info in page_info.values())
@@ -171,22 +191,25 @@
         for _page_info_key, _page_info_value in page_info.items():
             document_ast = parse(next_query)
             if _page_info_value['nextCursor'] == "":
                 self.deleted_queries.append(next_query)
                 stored = True
                 visitor = RemoveQueryByStartingName(query_start=_page_info_key)
                 document_ast = visit(document_ast, visitor)
-                next_query = remove_unused_variables(document_ast=document_ast, query=print_ast(document_ast))
+                next_query = remove_unused_variables(document_ast=document_ast,
+                query=print_ast(document_ast))
             else:
                 if not stored:
                     self.deleted_queries.append(None)
                 if has_cursor(document_ast, _page_info_key):
-                    replace_cursor_value(document_ast, _page_info_key, _page_info_value['nextCursor'])
+                    replace_cursor_value(document_ast, _page_info_key,
+                    _page_info_value['nextCursor'])
                 else:
-                    add_cursor_to_input_field(document_ast, _page_info_key, _page_info_value['nextCursor'])
+                    add_cursor_to_input_field(document_ast, _page_info_key,
+                    _page_info_value['nextCursor'])
                 next_query = print_ast(document_ast)
         return await self.execute_paginated_query(next_query, variables)
 
     async def get_prev_page(self, query, variables, page_info):
         """Async function to get the previous page data.
 
         Args:
```

### Comparing `airstack-0.0.3/src/airstack/generic.py` & `airstack-0.0.4/src/airstack/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+"""
+Module: generic.py
+Description: This module contains the generic methods required by this product.
+"""
+
 import re
-from graphql.language.ast import Field, ObjectField, ObjectValue, StringValue, Name, Argument, FragmentSpread, InlineFragment, SelectionSet, Document, OperationDefinition, VariableDefinition
+from graphql.language.ast import Field, ObjectField, ObjectValue, StringValue, Name, Argument, FragmentSpread, InlineFragment, SelectionSet, Document
 from graphql.language.visitor import Visitor
-from graphql.language import ast
 from graphql import parse, print_ast
 
 
 def find_page_info(json_data):
     """Func to find the pageInfo from json response
 
     Args:
@@ -183,27 +187,29 @@
     """
     parsed_document = parse(graphql_document)
     modified_document = _add_page_info_to_queries(parsed_document)
     return print_ast(modified_document)
 
 def _add_page_info_to_queries(node):
     if isinstance(node, Document):
-        node.definitions = [_add_page_info_to_queries(definition) for definition in node.definitions]
+        node.definitions = [_add_page_info_to_queries(definition) for
+        definition in node.definitions]
     elif isinstance(node, Field):
         if node.selection_set is None:
             node.selection_set = SelectionSet(selections=[])
         node.selection_set.selections.append(Field(
             name=Name(value="pageInfo"),
             selection_set=SelectionSet(selections=[
                 Field(name=Name(value="nextCursor")),
                 Field(name=Name(value="prevCursor"))
             ])
         ))
     elif hasattr(node, "selection_set"):
-        node.selection_set.selections = [_add_page_info_to_queries(selection) for selection in node.selection_set.selections]
+        node.selection_set.selections = [_add_page_info_to_queries(selection) for
+        selection in node.selection_set.selections]
     return node
 
 def remove_unused_variables(document_ast, query):
     """Func to remove unused variables from the query
 
     Args:
         document_ast (ast): parsed query
```

### Comparing `airstack-0.0.3/src/airstack/send_request.py` & `airstack-0.0.4/src/airstack/send_request.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.3/src/airstack.egg-info/PKG-INFO` & `airstack-0.0.4/src/airstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

