# Comparing `tmp/jiggybase-0.1.0.tar.gz` & `tmp/jiggybase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.1.0.tar", last modified: Wed Jun  7 00:12:23 2023, max compression
+gzip compressed data, was "jiggybase-0.1.2.tar", last modified: Wed Jun 21 05:32:34 2023, max compression
```

## Comparing `jiggybase-0.1.0.tar` & `jiggybase-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.197262 jiggybase-0.1.0/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.1.0/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-07 00:12:23.196848 jiggybase-0.1.0/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.1.0/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.180688 jiggybase-0.1.0/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.1.0/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.1.0/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     4356 2023-06-04 23:55:57.000000 jiggybase-0.1.0/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     9397 2023-06-05 00:10:11.000000 jiggybase-0.1.0/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.184847 jiggybase-0.1.0/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.1.0/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.1.0/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.1.0/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.1.0/jiggybase/examples/upload_email_example.py
--rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.1.0/jiggybase/ijiggy.py
--rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-28 04:35:07.000000 jiggybase-0.1.0/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.1.0/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.194126 jiggybase-0.1.0/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.1.0/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.1.0/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.1.0/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.1.0/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.1.0/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     1833 2023-06-04 00:49:56.000000 jiggybase-0.1.0/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.1.0/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.1.0/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 23:09:48.000000 jiggybase-0.1.0/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     4707 2023-06-03 23:40:06.000000 jiggybase-0.1.0/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3411 2023-06-03 23:48:09.000000 jiggybase-0.1.0/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.1.0/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.1.0/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.1.0/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4799 2023-06-05 00:03:48.000000 jiggybase-0.1.0/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.182710 jiggybase-0.1.0/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     1018 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)      109 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      794 2023-06-04 23:57:56.000000 jiggybase-0.1.0/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-07 00:12:23.197393 jiggybase-0.1.0/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.195960 jiggybase-0.1.0/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.1.0/test/test.py
--rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.1.0/test/test_extract_typed_completion.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.811447 jiggybase-0.1.2/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.1.2/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-21 05:32:34.810977 jiggybase-0.1.2/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.1.2/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.794914 jiggybase-0.1.2/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.1.2/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.1.2/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4385 2023-06-10 19:13:08.000000 jiggybase-0.1.2/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    10188 2023-06-19 05:34:38.000000 jiggybase-0.1.2/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.798816 jiggybase-0.1.2/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1416 2023-06-13 01:56:18.000000 jiggybase-0.1.2/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      310 2023-06-11 03:47:40.000000 jiggybase-0.1.2/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     6851 2023-06-21 04:30:38.000000 jiggybase-0.1.2/jiggybase/examples/confluence_sync.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.1.2/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1392 2023-06-08 03:25:05.000000 jiggybase-0.1.2/jiggybase/examples/qa_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.1.2/jiggybase/examples/upload_email_example.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.1.2/jiggybase/ijiggy.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5887 2023-06-10 18:20:45.000000 jiggybase-0.1.2/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.1.2/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.808858 jiggybase-0.1.2/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.1.2/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.1.2/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.1.2/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.1.2/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.1.2/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1833 2023-06-04 00:49:56.000000 jiggybase-0.1.2/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.1.2/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.1.2/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 23:09:48.000000 jiggybase-0.1.2/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4858 2023-06-19 05:14:08.000000 jiggybase-0.1.2/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3411 2023-06-03 23:48:09.000000 jiggybase-0.1.2/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.1.2/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.1.2/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.1.2/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4799 2023-06-05 00:03:48.000000 jiggybase-0.1.2/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.796646 jiggybase-0.1.2/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     1089 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      109 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-21 05:32:34.000000 jiggybase-0.1.2/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      794 2023-06-19 02:49:26.000000 jiggybase-0.1.2/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-21 05:32:34.811577 jiggybase-0.1.2/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-21 05:32:34.810324 jiggybase-0.1.2/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.1.2/test/test.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.1.2/test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.1.0/LICENSE` & `jiggybase-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/PKG-INFO` & `jiggybase-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.1.0
+Version: 0.1.2
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.1.0/README.md` & `jiggybase-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/chat_stream.py` & `jiggybase-0.1.2/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/client.py` & `jiggybase-0.1.2/jiggybase/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from .models.user import User, ApiKey
 from .jiggybase_session import JiggyBaseSession
 from .models.chat import Message, TypedCompletionRequest
 from pydantic import BaseModel    
 
 class JiggyBase():
 
-    def __init__(self):
-        self.session = JiggyBaseSession()     
+    def __init__(self, api_key=None):
+        self.session = JiggyBaseSession(api_key=api_key)     
         
     def orgs(self) -> List[Org]:
         """
         return all Orgs that the user is a member of
         """
         resp = self.session.get('/orgs')
         return [Org(self.session, **i) for i in resp.json()]
```

### Comparing `jiggybase-0.1.0/jiggybase/collection.py` & `jiggybase-0.1.2/jiggybase/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 from typing import Optional, List, Iterator
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
 from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
-from .models import Message, CompletionRequest, ChatCompletion, ChatUsage
+from .models import Message, CompletionRequest, ChatCompletion 
 from .chat_stream import extract_content_from_sse_bytes
 from .models import ExtractMetadataConfig
 from .models import CollectionPatchRequest, PluginAuthConfigOAuth, PatchPluginOAuthConfigRequest
-
+from .models import DocumentMetadata
 from typing import Union, List
 
 
         
 class Collection(collection.Collection):
     """
     derived from models.collection.Collection data model for purposes of adding management methods
     """
     class Config(BaseConfig):
         extra = "allow"
 
     def __init__(self, session, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.session = session
-        self.plugin_session = JiggyBaseSession(host=f'https://{kwargs["fqdn"]}', api='')
-        self.chat_session = JiggyBaseSession(host=session.host, api='v1')
+        self.session = session        
+        api_key = self.session.api_key
+        self.plugin_session = JiggyBaseSession(host=f'https://{kwargs["fqdn"]}', api='', api_key=api_key)
+        self.chat_session = JiggyBaseSession(host=session.host, api='v1', api_key=api_key)
         
     def set_description(self, description:str) -> "Collection":
         """
         Update an existing collection using its ID and the provided description.
         """
         patch_request = CollectionPatchRequest(description=description)
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}", model=patch_request)
@@ -72,24 +73,33 @@
         """
         Update the chat configuration for this collection.
         """
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}/chat_config/{model}", model=PatchCollectionChatConfig(prompt_task_id=prompt_task_id))
         return CollectionChatConfig(**rsp.json())
 
  
-    def upsert_file(self, file_path: str, mimetype: str = None) -> UpsertResponse:
+    def upsert_file(self, file_path: str, mimetype: str = None, id: str = None, metadata : DocumentMetadata = None) -> UpsertResponse:
         """
         Add a file to the collection.
+        Mimetype can be specified, otherwise it will be inferred from the file extension.
+        The doc id can be specified, otherwise it will be generated.
+        Metadata can be specified, otherwise some metadata will be inferred from the file.
         """
         if not os.path.exists(file_path):
             raise ValueError("File not found")
-             
         with open(file_path, "rb") as file:
             files = {"file": (os.path.basename(file_path), file, mimetype)}
-            rsp = self.plugin_session.post("/upsert-file", files=files)
+            params = {'id': id} if id else {}
+            if metadata:
+                rsp = self.plugin_session.post("/upsert-file", 
+                                               files=files, 
+                                               params=params,
+                                               data={'metadata': metadata.json(exclude_unset=True)})
+            else:
+                rsp = self.plugin_session.post("/upsert-file", params=params, files=files)
         return UpsertResponse.parse_obj(rsp.json())
 
     def upsert(self, documents: List[Document]) -> UpsertResponse:
         """
         Add a list of Document objects to the collection.
         """
         upsert_request = UpsertRequest(documents=documents)
```

### Comparing `jiggybase-0.1.0/jiggybase/examples/chat_completion.py` & `jiggybase-0.1.2/jiggybase/examples/chat_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jiggybase
 
 collection = jiggybase.JiggyBase().collection('hackernews-summary')   # replace with your collection name
 
 messages = [{'role':'user',  'content': 'articles about python 3.11'}]
 
-rsp = collection._chat_completion(messages)   # note _ as this is preliminary low-level interface
+rsp = collection._chat_completion(messages, temperature=0, model="gpt-3.5-turbo")   # note _ as this is preliminary low-level interface
 
 print(rsp)
 
 """
 Here are some articles about Python 3.11:
 
 1. Python 3.11.1, 3.10.9, 3.9.16, 3.8.16, 3.7.16, and 3.12.0 alpha 3 now available - This is a blog post from the official Python Software Foundation blog. The post is announcing the release of Python 3.11.1, 3.10.9, 3.9.16, 3.8.16, 3.7.16, and 3.12.0 alpha 3. The post goes over some of the security content in the new releases.
```

### Comparing `jiggybase-0.1.0/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.1.2/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/examples/upload_email_example.py` & `jiggybase-0.1.2/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/ijiggy.py` & `jiggybase-0.1.2/jiggybase/ijiggy.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/jiggybase_session.py` & `jiggybase-0.1.2/jiggybase/jiggybase_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class ServerError(Exception):
     """
     API returned 5xx Server error
     """
 
     
 class JiggyBaseSession(requests.Session):
-    def __init__(self, host=JIGGYBASE_HOST, api='gpt-gateway-v1', bearer_token=None, *args, **kwargs):
+    def __init__(self, host=JIGGYBASE_HOST, api='gpt-gateway-v1', bearer_token=None, api_key=None, *args, **kwargs):
         """
         Extend requests.Session with common GPTG authentication, retry, and exceptions.
 
         host: The url host prefix of the form "https:/api.gpt-gateway.com"
               if host arg is not set, will use 
                     JIGGYBASE_HOST environment variable or "api.gpt-gateway.com" as final default.
 
@@ -50,16 +50,23 @@
         if not host.startswith('http'):
             host = f"https://{host}" if not host.startswith('localhost') else f'http://{host}'
         self.host = host
         if api:
             self.prefix_url = f"{host}/{api}"
         else:
             self.prefix_url = host          
+
+        self.bearer_token = None            
+        self.api_key = None
+        if api_key:
+            self.api_key = api_key
+            self._getjwt(api_key)
+        elif bearer_token:
+            self._set_bearer(bearer_token)
             
-        self.bearer_token = bearer_token
         super(JiggyBaseSession, self).mount('https://',
                                             HTTPAdapter(max_retries=Retry(connect=5,
                                                                           read=5,
                                                                           status=5,
                                                                           redirect=2,
                                                                           backoff_factor=.001,
                                                                           status_forcelist=None)))
```

### Comparing `jiggybase-0.1.0/jiggybase/login.py` & `jiggybase-0.1.2/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/auth.py` & `jiggybase-0.1.2/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/chat.py` & `jiggybase-0.1.2/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/chunk.py` & `jiggybase-0.1.2/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/collection.py` & `jiggybase-0.1.2/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/metadata.py` & `jiggybase-0.1.2/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/org.py` & `jiggybase-0.1.2/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/plugin.py` & `jiggybase-0.1.2/jiggybase/models/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 
 class Source(str, Enum):
     email = "email"
     file = "file"
     chat = "chat"
     web  = "web"
 
+
 class DocumentMetadata(BaseModel):
     source: Optional[Source] = None
     source_id: Optional[str] = None
     url: Optional[str] = None
     created_at: Optional[str] = None
-    author: Union[str, list[str]] = None
+    author: Union[str, List[str]] = None
     title: Optional[str] = None
     description: Optional[str] = None
-    
+    language: Optional[str] = Field(description="The 2 character ISO 639-1 language code of the primary language of the content.")
+    version: str = None
 
 class DocumentChunkMetadata(DocumentMetadata):
     document_id: Optional[str] = None
 
 
 class DocumentChunk(BaseModel):
     id: Optional[str] = None
```

### Comparing `jiggybase-0.1.0/jiggybase/models/plugin_config.py` & `jiggybase-0.1.2/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/prompt.py` & `jiggybase-0.1.2/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/providers.py` & `jiggybase-0.1.2/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/models/user.py` & `jiggybase-0.1.2/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase/org.py` & `jiggybase-0.1.2/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.1.2/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.1.0
+Version: 0.1.2
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.1.0/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.1.2/jiggybase.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 jiggybase.egg-info/SOURCES.txt
 jiggybase.egg-info/dependency_links.txt
 jiggybase.egg-info/entry_points.txt
 jiggybase.egg-info/requires.txt
 jiggybase.egg-info/top_level.txt
 jiggybase/examples/chat_completion.py
 jiggybase/examples/chat_completion_stream.py
+jiggybase/examples/confluence_sync.py
 jiggybase/examples/jiggybase_upload.py
+jiggybase/examples/qa_example.py
 jiggybase/examples/upload_email_example.py
 jiggybase/models/__init__.py
 jiggybase/models/auth.py
 jiggybase/models/chat.py
 jiggybase/models/chatmodel.py
 jiggybase/models/chunk.py
 jiggybase/models/collection.py
```

### Comparing `jiggybase-0.1.0/pyproject.toml` & `jiggybase-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.1.0/test/test.py` & `jiggybase-0.1.2/test/test.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.1.0/test/test_extract_typed_completion.py` & `jiggybase-0.1.2/test/test_extract_typed_completion.py`

 * *Files identical despite different names*

