# Comparing `tmp/embedbase-1.2.7.tar.gz` & `tmp/embedbase-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.7.tar", max compression
+gzip compressed data, was "embedbase-1.2.8.tar", max compression
```

## Comparing `embedbase-1.2.7.tar` & `embedbase-1.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-06-09 23:39:27.632114 embedbase-1.2.7/LICENSE
--rw-r--r--   0        0        0     4931 2023-06-09 23:39:27.632114 embedbase-1.2.7/README.md
--rw-r--r--   0        0        0      121 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/__main__.py
--rw-r--r--   0        0        0      416 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/api.py
--rw-r--r--   0        0        0    19516 2023-06-09 23:39:27.776115 embedbase-1.2.7/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3920 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/base.py
--rw-r--r--   0        0        0     6962 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    11071 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     9332 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1459 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/models.py
--rw-r--r--   0        0        0     1245 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-06-09 23:39:27.780115 embedbase-1.2.7/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-06-09 23:39:27.784115 embedbase-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 09:49:08.910008 embedbase-1.2.8/LICENSE
+-rw-r--r--   0        0        0     4931 2023-05-30 12:00:19.910827 embedbase-1.2.8/README.md
+-rw-r--r--   0        0        0      121 2023-04-17 09:49:08.965565 embedbase-1.2.8/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-15 09:13:00.923384 embedbase-1.2.8/embedbase/__main__.py
+-rw-r--r--   0        0        0      416 2023-05-30 12:00:19.923995 embedbase-1.2.8/embedbase/api.py
+-rw-r--r--   0        0        0    19516 2023-06-21 19:07:41.219754 embedbase-1.2.8/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-17 09:49:08.965863 embedbase-1.2.8/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3920 2023-05-30 12:00:23.900738 embedbase-1.2.8/embedbase/database/base.py
+-rw-r--r--   0        0        0     6962 2023-05-30 12:00:23.900994 embedbase-1.2.8/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    11071 2023-05-30 12:00:23.901154 embedbase-1.2.8/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     9642 2023-06-21 18:45:26.099291 embedbase-1.2.8/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-04-17 09:49:08.966416 embedbase-1.2.8/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-19 14:33:24.295852 embedbase-1.2.8/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-19 14:34:20.779193 embedbase-1.2.8/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-20 13:55:18.629954 embedbase-1.2.8/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-17 09:49:08.966647 embedbase-1.2.8/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-04-23 15:48:21.932644 embedbase-1.2.8/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1459 2023-06-05 21:35:48.358259 embedbase-1.2.8/embedbase/models.py
+-rw-r--r--   0        0        0     1245 2023-05-30 12:00:19.927410 embedbase-1.2.8/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-17 09:49:08.966943 embedbase-1.2.8/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-17 09:49:08.967015 embedbase-1.2.8/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-01 11:26:55.164806 embedbase-1.2.8/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-06-21 19:08:18.938528 embedbase-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.8/PKG-INFO
```

### Comparing `embedbase-1.2.7/LICENSE` & `embedbase-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/README.md` & `embedbase-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/__main__.py` & `embedbase-1.2.8/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/app.py` & `embedbase-1.2.8/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/database/base.py` & `embedbase-1.2.8/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/database/memory_db.py` & `embedbase-1.2.8/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/database/postgres_db.py` & `embedbase-1.2.8/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/database/supabase_db.py` & `embedbase-1.2.8/embedbase/database/supabase_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,35 +109,46 @@
         store_data: bool = True,
     ):
         df_batcher = BatchGenerator(batch_size)
         batches = [batch_df for batch_df in df_batcher(df)]
 
         # create dataset in datasets table if not exist
 
-        q = self.supabase.table("datasets").select("*").eq("name", dataset_id)
+        q = self.supabase.table("datasets").select("id").eq("name", dataset_id)
         if user_id:
             q = q.eq("owner", user_id)
+        dataset_final_id = ""
         data = q.execute().data
         if not data:
-            self.supabase.table("datasets").insert(
-                {
-                    "name": dataset_id,
-                    "owner": user_id,
-                }
-            ).execute()
+            data = (
+                self.supabase.table("datasets")
+                .insert(
+                    {
+                        "name": dataset_id,
+                        "owner": user_id,
+                    }
+                )
+                .execute()
+                .data
+            )
+
+        dataset_final_id = data[0]["id"]
 
-        async def _insert(batch_df: DataFrame):
+        async def _insert(
+            batch_df: DataFrame, dataset_final_id: str = dataset_final_id
+        ):
             def _d(row: Series):
                 data = {
                     "id": row.id,
                     "embedding": row.embedding,
                     "hash": row.hash,
                     "dataset_id": dataset_id,
                     "user_id": user_id,
                     "metadata": row.metadata,
+                    "dataset_final_id": dataset_final_id,
                 }
                 # {'code': '22P05', 'details': '\\u0000 cannot be converted to text.', 'hint': None, 'message': 'unsupported Unicode escape sequence'}
                 row.data = row.data.replace("\x00", "")
                 if store_data:
                     data["data"] = row.data
                 return data
```

### Comparing `embedbase-1.2.7/embedbase/embedding/base.py` & `embedbase-1.2.8/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/embedding/cohere.py` & `embedbase-1.2.8/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/embedding/openai.py` & `embedbase-1.2.8/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/firebase_auth.py` & `embedbase-1.2.8/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/logging_utils.py` & `embedbase-1.2.8/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/models.py` & `embedbase-1.2.8/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/settings.py` & `embedbase-1.2.8/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/strings.py` & `embedbase-1.2.8/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/embedbase/utils.py` & `embedbase-1.2.8/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.7/pyproject.toml` & `embedbase-1.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.7"
+version = "1.2.8"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.7/PKG-INFO` & `embedbase-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.7
+Version: 1.2.8
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

