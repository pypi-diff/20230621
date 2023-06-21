# Comparing `tmp/testery-1.6.9-py3-none-any.whl.zip` & `tmp/testery-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15863 bytes, number of entries: 11
--rw-r--r--  2.0 unx    50242 b- defN 23-Jun-13 18:37 testery.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:37 tests/__init__.py
--rw-r--r--  2.0 unx     2354 b- defN 23-Jun-13 18:37 tests/conftest.py
--rw-r--r--  2.0 unx     4857 b- defN 23-Jun-13 18:37 tests/test_integration.py
--rw-r--r--  2.0 unx     2797 b- defN 23-Jun-13 18:37 tests/test_unit.py
--rw-r--r--  2.0 unx     1055 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     1264 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      851 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/RECORD
-11 files, 63586 bytes uncompressed, 14433 bytes compressed:  77.3%
+Zip file size: 15923 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    50552 b- defN 23-Jun-21 21:37 testery.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 21:37 tests/__init__.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-Jun-21 21:37 tests/conftest.py
+-rw-r--r--  2.0 unx     4857 b- defN 23-Jun-21 21:37 tests/test_integration.py
+-rw-r--r--  2.0 unx     2797 b- defN 23-Jun-21 21:37 tests/test_unit.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      851 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/RECORD
+11 files, 63896 bytes uncompressed, 14493 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tests/test_integration.py
 Comment: 
 
 Filename: tests/test_unit.py
 Comment: 
 
-Filename: testery-1.6.9.dist-info/LICENSE
+Filename: testery-1.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: testery-1.6.9.dist-info/METADATA
+Filename: testery-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: testery-1.6.9.dist-info/WHEEL
+Filename: testery-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: testery-1.6.9.dist-info/entry_points.txt
+Filename: testery-1.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: testery-1.6.9.dist-info/top_level.txt
+Filename: testery-1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: testery-1.6.9.dist-info/RECORD
+Filename: testery-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testery.py

```diff
@@ -562,17 +562,18 @@
         request["variables"]=vars
 
 @click.command('update-environment')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
 @click.option('--token', required=True, help='Your Testery API token.')
 @click.option('--name', required=True, help='The display name for the environment.')
 @click.option('--key', required=True, help='An identifier for the environment. This is used when creating test runs to indicate where tests should run.')
+@click.option('--pipeline-stage', default=None, help='The name of a pipeline stage to associate this environment to.')
 @click.option('--variable', help='A variable to add to the environment. Specified as "KEY=VALUE". To encrypt value, pass in "secure:KEY=VALUE", Multiple variables can be provided.', multiple=True)
 @click.option('--create-if-not-exists', is_flag=True, default=False, help='If passed in, environment will be created if not present. Otherwise command will fail.')
-def update_environment(testery_dev, token, key, name, variable, create_if_not_exists):
+def update_environment(testery_dev, token, key, name, pipeline_stage, variable, create_if_not_exists):
     """
     Updates an environment where tests can be run.
     """
     environment_request = {"key": key, "name": name}
 
     headers['Authorization'] = "Bearer " + token
     api_url = get_api_url(testery_dev)
@@ -588,20 +589,26 @@
     if not environment and not create_if_not_exists:
         raise Exception("Environment not found by key and --create-if-not-exists flag was not set: " + key)
 
     headers['Authorization'] = "Bearer " + token
 
     if environment:
         environment["name"]=name
+
         handle_variables(variable, environment)
         print("Updating environment: " + key)
         print(environment)
         response = requests.patch(api_url + '/environments/' + str(environment['id']), headers=headers, json=environment)
     else:
         environment_request = {"key": key, "name": name}
+
+        if pipeline_stage:
+            stage = find_pipeline_stage_by_name(api_url, token, pipeline_stage)
+            environment_request['pipelineStageId'] = stage['id']
+
         handle_variables(variable, environment_request)
         print("Creating environment: " + key)
         response = requests.post(api_url + '/environments', headers=headers, json=environment_request)
 
     print(response)
 
 @click.command('upload-environment-file')
```

## Comparing `testery-1.6.9.dist-info/LICENSE` & `testery-1.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testery-1.6.9.dist-info/METADATA` & `testery-1.7.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testery
-Version: 1.6.9
+Version: 1.7.0
 Summary: Testery CLI
 Home-page: https://github.com/testery/testery-cli
 Author: Testery
 Author-email: chris.harbert@testery.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `testery-1.6.9.dist-info/RECORD` & `testery-1.7.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-testery.py,sha256=UDAKRktL-NWJRxlPe7NvwYBzXDOnCqvbVNdG-HDmV-A,50242
+testery.py,sha256=Rip01NC2Ln7d1pcvcJ9KYw_3ld5ooiZC-uZ-bRRZ7mI,50552
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=AfQWy8n3D0jiQx2zlUCPa4s8MtoL-_x4IA2PEB61N0s,2354
 tests/test_integration.py,sha256=OuTRk7nJz11ks6Z21GcMND5xEt-Q9hKWboiP-uR6hok,4857
 tests/test_unit.py,sha256=0W33Gq-L6JxjAfeIGcOvqrA4Enl4HTvMRgvW4FAGMpg,2797
-testery-1.6.9.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
-testery-1.6.9.dist-info/METADATA,sha256=Gq5j9enmw1UMZ2RvaUMTMBTRwcjZsLw0-hr6Dtk_Oaw,1264
-testery-1.6.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-testery-1.6.9.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
-testery-1.6.9.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
-testery-1.6.9.dist-info/RECORD,,
+testery-1.7.0.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
+testery-1.7.0.dist-info/METADATA,sha256=VyaRrz06qbFMAVCsnOEHy8tH3rsRvm9dXAFRdwV0eV8,1264
+testery-1.7.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+testery-1.7.0.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
+testery-1.7.0.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
+testery-1.7.0.dist-info/RECORD,,
```

