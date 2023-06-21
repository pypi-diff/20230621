# Comparing `tmp/python-oauth-token-manager-0.2.6.tar.gz` & `tmp/python-oauth-token-manager-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.2.6.tar", last modified: Thu Jun 15 15:31:36 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.7.tar", last modified: Wed Jun 21 15:33:01 2023, max compression
```

## Comparing `python-oauth-token-manager-0.2.6.tar` & `python-oauth-token-manager-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.6/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.6/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.2.6/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2023-06-15 15:30:01.000000 python-oauth-token-manager-0.2.6/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5770 2023-06-15 15:29:48.000000 python-oauth-token-manager-0.2.6/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.6/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.6/auth/credentials_helpers_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/auth/datastore/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.6/auth/datastore/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.2.6/auth/datastore/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.2.6/auth/datastore/local_file.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.6/auth/datastore/local_file_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6001 2023-06-15 15:27:21.000000 python-oauth-token-manager-0.2.6/auth/datastore/secret_manager.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.6/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.6/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.6/auth/exceptions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-15 15:29:36.000000 python-oauth-token-manager-0.2.6/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:33:00.998300 python-oauth-token-manager-0.2.7/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.7/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-21 15:33:00.994300 python-oauth-token-manager-0.2.7/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.7/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:33:00.994300 python-oauth-token-manager-0.2.7/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.2.7/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2023-06-15 15:30:01.000000 python-oauth-token-manager-0.2.7/auth/abstract_datastore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5770 2023-06-15 15:52:54.000000 python-oauth-token-manager-0.2.7/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.7/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.7/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:33:00.994300 python-oauth-token-manager-0.2.7/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.7/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.2.7/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.7/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.2.7/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.2.7/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.7/auth/datastore/local_file_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6754 2023-06-21 14:44:05.000000 python-oauth-token-manager-0.2.7/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.7/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.7/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      947 2023-06-21 13:37:58.000000 python-oauth-token-manager-0.2.7/auth/exceptions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-21 13:32:45.000000 python-oauth-token-manager-0.2.7/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:33:00.994300 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-21 15:33:00.000000 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-21 15:33:00.000000 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-21 15:33:00.000000 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-21 15:33:00.000000 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-21 15:33:00.000000 python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-21 15:33:00.998300 python-oauth-token-manager-0.2.7/setup.cfg
```

### Comparing `python-oauth-token-manager-0.2.6/LICENSE` & `python-oauth-token-manager-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/PKG-INFO` & `python-oauth-token-manager-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.6
+Version: 0.2.7
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.6/README.md` & `python-oauth-token-manager-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/__init__.py` & `python-oauth-token-manager-0.2.7/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.7/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/credentials.py` & `python-oauth-token-manager-0.2.7/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.7/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.7/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/__init__.py` & `python-oauth-token-manager-0.2.7/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage.py` & `python-oauth-token-manager-0.2.7/auth/datastore/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage_test.py` & `python-oauth-token-manager-0.2.7/auth/datastore/cloud_storage_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/firestore.py` & `python-oauth-token-manager-0.2.7/auth/datastore/firestore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/local_file.py` & `python-oauth-token-manager-0.2.7/auth/datastore/local_file.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/local_file_test.py` & `python-oauth-token-manager-0.2.7/auth/datastore/local_file_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/datastore/secret_manager.py` & `python-oauth-token-manager-0.2.7/auth/datastore/secret_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -89,32 +89,55 @@
     As this is a specific 'update' request, remove any other enabled versions.
 
     Args:
         id (str): the id of the document.
         new_data (Dict[str, Any]): the document content.
         type (Optional[Type]): Unused.
     """
-    new_version = self.store_document(id=id, type=type, document=new_data)
+    new_version: resources.SecretVersion = self.store_document(
+        id=id, type=type, document=new_data)
+
+    latest = self._get_latest(id)
 
     # Destroy other versions
     request = secretmanager_v1.ListSecretVersionsRequest(
         parent=self.client.secret_path(project=self._project, secret=id),
-        filter='state:enabled'
+        filter=f'state:enabled AND name!="{latest.name}"'
     )
     version_list = self.client.list_secret_versions(request=request)
     for page in version_list.pages:
       for version in page.versions:
         if version == new_version:
           continue
         else:
           self.client.destroy_secret_version(
               secretmanager_v1.DestroySecretVersionRequest(
                   name=version.name
               ))
 
+  def _get_latest(self, id: str) -> resources.SecretVersion:
+    """Fetches the latest secret version.
+
+    Arguments:
+        id (str): document id.
+
+    Returns:
+        SecretVersion: the latest version of the stored secret.
+    """
+    secret = self.client.secret_version_path(project=self._project,
+                                             secret=id,
+                                             secret_version='latest')
+    try:
+      request = secretmanager_v1.GetSecretVersionRequest(name=secret)
+      response = self.client.get_secret_version(request=request)
+      return response
+    except Exception as e:
+      print(e)
+      return None
+
   def get_document(self, id: str, type: Optional[Type] = None,
                    key: Optional[str] = None) -> Mapping[str, Any]:
     """Fetches a document (could be anything).
 
     Fetch a document
 
     Arguments:
```

### Comparing `python-oauth-token-manager-0.2.6/auth/decorators.py` & `python-oauth-token-manager-0.2.7/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/decorators_test.py` & `python-oauth-token-manager-0.2.7/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.6/auth/exceptions.py` & `python-oauth-token-manager-0.2.7/auth/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,10 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 
 class OAuthException(Exception): ...
 
-class CredentialsError(OAuthException): ...
-class KeyEncodingError(OAuthException): ...
+class CredentialsError(OAuthException):
+  def __init__(self, *args: object, message: str | None = ..., email: str | None) -> None: ...
+  message: str | None
+
+class KeyEncodingError(OAuthException):
+  def __init__(self, *args: object, message: str | None = ...) -> None: ...
+  message: str | None
```

### Comparing `python-oauth-token-manager-0.2.6/pyproject.toml` & `python-oauth-token-manager-0.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-oauth-token-manager"
-version = "0.2.6"
+version = "0.2.7"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "API for managing stored OAuth credentials."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
```

### Comparing `python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/PKG-INFO` & `python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.6
+Version: 0.2.7
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.7/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

