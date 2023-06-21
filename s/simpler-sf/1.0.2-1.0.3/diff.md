# Comparing `tmp/simpler_sf-1.0.2.tar.gz` & `tmp/simpler_sf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/simpler-sf/simpler-sf/dist/.tmp-olk08g_3/simpler_sf-1.0.2.tar", last modified: Fri May 19 15:42:55 2023, max compression
+gzip compressed data, was "/home/runner/work/simpler-sf/simpler-sf/dist/.tmp-9efgxqey/simpler_sf-1.0.3.tar", last modified: Wed Jun 21 14:36:13 2023, max compression
```

## Comparing `simpler_sf-1.0.2.tar` & `simpler_sf-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/simpler_sf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-19 15:42:44.000000 simpler_sf-1.0.2/simpler_sf/_simpler_sf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 15:42:55.000000 simpler_sf-1.0.2/simpler_sf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/simpler_sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-21 14:36:04.000000 simpler_sf-1.0.3/simpler_sf/_simpler_sf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 14:36:13.000000 simpler_sf-1.0.3/simpler_sf.egg-info/top_level.txt
```

### Comparing `simpler_sf-1.0.2/LICENSE` & `simpler_sf-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simpler_sf-1.0.2/PKG-INFO` & `simpler_sf-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpler_sf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extending Simple Salesforce to support Pandas exports and more.
 Home-page: https://github.com/benvigano/simpler-sf
 Author: benvigano
 Author-email: beniamino.vigano@protonmail.com
 License: MIT
 Keywords: Salesforce,Simple Salesforce,Pandas,Dataframe,Unpack Salesforce
 Description-Content-Type: text/markdown
@@ -18,33 +18,32 @@
 `pip install simpler-sf`
 
 ### Import
 ```python
 import simpler_sf
 simpler_sf.simple_salesforce()
 import simple_salesforce
-# That's it!
 ```
 ### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
 - Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
 - The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
 #### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Contact.Account.Name, Campaign.Name FROM CampaignMember')
 print(df)
 ```
 Output:
 ```
-            Contact.Id   Contact.FirstName   Account.Name           Campaign
-0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
-1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
-2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
-3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
+            Contact.Id   Contact.FirstName   Contact.Account.Name      Campaign.Name
+0   0032400000QZbmtAAD               Emily                 Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine                 Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng              Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena                 Google   CampaignC_2023Q1
 ```
```

### Comparing `simpler_sf-1.0.2/README.md` & `simpler_sf-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 `pip install simpler-sf`
 
 ### Import
 ```python
 import simpler_sf
 simpler_sf.simple_salesforce()
 import simple_salesforce
-# That's it!
 ```
 ### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
 - Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
 - The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
 #### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Contact.Account.Name, Campaign.Name FROM CampaignMember')
 print(df)
 ```
 Output:
 ```
-            Contact.Id   Contact.FirstName   Account.Name           Campaign
-0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
-1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
-2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
-3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
+            Contact.Id   Contact.FirstName   Contact.Account.Name      Campaign.Name
+0   0032400000QZbmtAAD               Emily                 Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine                 Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng              Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena                 Google   CampaignC_2023Q1
 ```
```

### Comparing `simpler_sf-1.0.2/setup.py` & `simpler_sf-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `simpler_sf-1.0.2/simpler_sf/_simpler_sf.py` & `simpler_sf-1.0.3/simpler_sf/_simpler_sf.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def _determine_fields(query):
     '''Parse a query to determine the fields'''
     
     before_from = re.split(" from ", query, flags=re.IGNORECASE)[0]
     after_select = re.split("select ", before_from, flags=re.IGNORECASE)[1]
-    fields = after_select.replace(" ", "").split(",")
+    fields = set(after_select.replace(" ", "").split(","))
     
     return fields
 
 
 def _generate_sub_queries(query, filter_field, filter_values, not_in):
     '''
     Split the input query in multiple sub-queries that respect Salesforce 10,000 character limit.
@@ -145,14 +145,17 @@
     
     # Make the query inline to ease parsing
     query = " ".join(line.strip() for line in query.splitlines())
     
     # Determine the Salesforce object by parsing the query
     object = getattr(self.bulk, _determine_object(query))
 
+    # Determine the fields by parsing the query
+    fields = _determine_fields(query)
+
     if filter_field is not None and filter_values is not None:
         sub_queries = _generate_sub_queries(query, filter_field, filter_values, not_in)
     else:
         sub_queries = [query]
                  
     dfs = []
     for sub_query in tqdm(sub_queries):
@@ -160,18 +163,23 @@
         partial_df = pd.DataFrame(results)
         dfs.append(partial_df)
         
     output_df = pd.concat(dfs)
         
     # If the query didn't output any records, add the columns for output consistency
     if output_df.shape[0] == 0:
-        # Determine the columns from the query
-        output_df = pd.DataFrame(columns=_determine_fields(query))
+        output_df = pd.DataFrame(columns=list(fields))
     else:
         pass
+
+    # Remove any unrequested columns that were returned
+    #   This can happen for example in the query "SELECT Account.Id FROM Contact", infact
+    #   if contacts that are not linked to an account are present, the additional column "Account" is returned.
+    unrequested_columns = [c for c in output_df.columns if c not in fields]
+    output_df.drop(columns=unrequested_columns, inplace=True)
                     
     return output_df
 
 
 def simple_salesforce():
     import simple_salesforce
     simple_salesforce.Salesforce.smart_query = _smart_query
```

### Comparing `simpler_sf-1.0.2/simpler_sf.egg-info/PKG-INFO` & `simpler_sf-1.0.3/simpler_sf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpler-sf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extending Simple Salesforce to support Pandas exports and more.
 Home-page: https://github.com/benvigano/simpler-sf
 Author: benvigano
 Author-email: beniamino.vigano@protonmail.com
 License: MIT
 Keywords: Salesforce,Simple Salesforce,Pandas,Dataframe,Unpack Salesforce
 Description-Content-Type: text/markdown
@@ -18,33 +18,32 @@
 `pip install simpler-sf`
 
 ### Import
 ```python
 import simpler_sf
 simpler_sf.simple_salesforce()
 import simple_salesforce
-# That's it!
 ```
 ### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
 - Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
 - The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
 #### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Contact.Account.Name, Campaign.Name FROM CampaignMember')
 print(df)
 ```
 Output:
 ```
-            Contact.Id   Contact.FirstName   Account.Name           Campaign
-0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
-1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
-2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
-3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
+            Contact.Id   Contact.FirstName   Contact.Account.Name      Campaign.Name
+0   0032400000QZbmtAAD               Emily                 Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine                 Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng              Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena                 Google   CampaignC_2023Q1
 ```
```

