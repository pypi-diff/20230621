# Comparing `tmp/pingpongsdk-0.1.4.tar.gz` & `tmp/pingpongsdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingpongsdk-0.1.4.tar", max compression
+gzip compressed data, was "pingpongsdk-0.1.5.tar", max compression
```

## Comparing `pingpongsdk-0.1.4.tar` & `pingpongsdk-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      430 2023-06-21 16:48:36.511402 pingpongsdk-0.1.4/README.md
--rw-r--r--   0        0        0      510 2023-06-12 15:18:48.399004 pingpongsdk-0.1.4/pingpongsdk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 10:51:02.603747 pingpongsdk-0.1.4/pingpongsdk/deployments/__init__.py
--rw-r--r--   0        0        0     1120 2023-06-21 16:48:11.346070 pingpongsdk-0.1.4/pingpongsdk/deployments/deployments.py
--rw-r--r--   0        0        0      472 2023-06-12 15:18:48.399442 pingpongsdk-0.1.4/pingpongsdk/deployments/model.py
--rw-r--r--   0        0        0      754 2023-06-12 15:18:48.400649 pingpongsdk-0.1.4/pingpongsdk/deployments/test_deployments.py
--rw-r--r--   0        0        0        0 2023-03-07 10:25:11.654435 pingpongsdk-0.1.4/pingpongsdk/models/__init__.py
--rw-r--r--   0        0        0      191 2023-06-12 15:18:48.401347 pingpongsdk-0.1.4/pingpongsdk/models/model.py
--rw-r--r--   0        0        0      894 2023-06-12 15:18:48.401588 pingpongsdk-0.1.4/pingpongsdk/models/models.py
--rw-r--r--   0        0        0      503 2023-03-07 10:50:52.527135 pingpongsdk-0.1.4/pingpongsdk/models/test_models.py
--rw-r--r--   0        0        0        0 2023-03-07 10:30:59.063001 pingpongsdk-0.1.4/pingpongsdk/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 10:28:06.621784 pingpongsdk-0.1.4/pingpongsdk/shared/client/__init__.py
--rw-r--r--   0        0        0     1089 2023-06-12 15:18:48.401850 pingpongsdk-0.1.4/pingpongsdk/shared/client/client.py
--rw-r--r--   0        0        0        0 2023-03-09 11:09:06.221521 pingpongsdk-0.1.4/pingpongsdk/tests/__init__.py
--rw-r--r--   0        0        0      279 2023-06-21 16:50:52.195999 pingpongsdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 pingpongsdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-06-21 16:57:59.764416 pingpongsdk-0.1.5/README.md
+-rw-r--r--   0        0        0      528 2023-06-21 16:57:59.765387 pingpongsdk-0.1.5/pingpongsdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:51:02.603747 pingpongsdk-0.1.5/pingpongsdk/deployments/__init__.py
+-rw-r--r--   0        0        0     1300 2023-06-21 16:57:59.765647 pingpongsdk-0.1.5/pingpongsdk/deployments/deployments.py
+-rw-r--r--   0        0        0      606 2023-06-21 16:57:59.765877 pingpongsdk-0.1.5/pingpongsdk/deployments/model.py
+-rw-r--r--   0        0        0      743 2023-06-21 16:57:59.766115 pingpongsdk-0.1.5/pingpongsdk/deployments/test_deployments.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:25:11.654435 pingpongsdk-0.1.5/pingpongsdk/models/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-21 16:57:59.766341 pingpongsdk-0.1.5/pingpongsdk/models/model.py
+-rw-r--r--   0        0        0     1308 2023-06-21 16:57:59.766811 pingpongsdk-0.1.5/pingpongsdk/models/models.py
+-rw-r--r--   0        0        0      503 2023-03-07 10:50:52.527135 pingpongsdk-0.1.5/pingpongsdk/models/test_models.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:30:59.063001 pingpongsdk-0.1.5/pingpongsdk/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:28:06.621784 pingpongsdk-0.1.5/pingpongsdk/shared/client/__init__.py
+-rw-r--r--   0        0        0     1124 2023-06-21 16:57:59.767079 pingpongsdk-0.1.5/pingpongsdk/shared/client/client.py
+-rw-r--r--   0        0        0        0 2023-03-09 11:09:06.221521 pingpongsdk-0.1.5/pingpongsdk/tests/__init__.py
+-rw-r--r--   0        0        0      279 2023-06-21 17:02:26.356449 pingpongsdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 pingpongsdk-0.1.5/PKG-INFO
```

### Comparing `pingpongsdk-0.1.4/pingpongsdk/deployments/deployments.py` & `pingpongsdk-0.1.5/pingpongsdk/deployments/deployments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from ..shared.client.client import Client
-from .model import Deployment, dto, CreateDeployment
+from .model import Deployment, dto, request_dto, CreateDeployment
 
 from dataclasses import asdict
 
 
 class Deployments(Client):
-    def __init__(self, api_key: str) -> None:
+
+    def __init__(self, api_key: str, models) -> None:
+        self.models = models
         super().__init__(api_key)
 
 
     def get_by_id(self, id: str) -> Deployment:
         """
         get_by_id - get a deployment by its ID
         """
@@ -18,15 +20,19 @@
     
 
     def create(self, deployment: CreateDeployment) -> Deployment:
         """
         create - create a new Deployment
         """
         try:
-            deployment = super().post("/api/v1/deployments", asdict(deployment))
+            model = self.models.get_by_alias(deployment.model)
+            id = model.id
+            request = request_dto(id, deployment)
+
+            deployment = super().post("/api/v1/deployments", request)
             return dto(deployment)
         except Exception as e:
             raise Exception('error creating deployment %s' % e)
 
 
     def list(self, start: int, to: int) -> list[Deployment]:
         """
```

### Comparing `pingpongsdk-0.1.4/pingpongsdk/deployments/test_deployments.py` & `pingpongsdk-0.1.5/pingpongsdk/deployments/test_deployments.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 _API_KEY = os.getenv("X_MEDIAMAGIC_KEY")
 
 
 def test_can_create_deployment():
     deployment_client = Deployments(api_key=_API_KEY)
     deployment = deployment_client.create(deployment=CreateDeployment(
         name="test-deployment",
-        model_id="4954c9fd-7fc2-4d4c-a036-f23f7605fa69",
+        model="pingponai/background-removal",
         args={
             'input_image_file': 'https://cdn.mediamagic.dev/media/eb341446-be53-11ed-b4a8-66139910f724.jpg',
         },
     ))
     assert deployment.job.credits_used > 0
     assert deployment.job.id is not None
```

### Comparing `pingpongsdk-0.1.4/pingpongsdk/shared/client/client.py` & `pingpongsdk-0.1.5/pingpongsdk/shared/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,12 @@
     def post(self, path: str, body: dict):
         try:
             response = requests.post(_BASE_URL + path, json=body, headers={
                 'Content-Type': 'application/json',
                 'x-mediamagic-key': self._api_key,
                 'Accept': 'application/json',
             })
+            print(response.json())
             response.raise_for_status()
             return response.json()
         except requests.exceptions.HTTPError as e:
             return "A HTTP error occured: %s" % e
```

### Comparing `pingpongsdk-0.1.4/PKG-INFO` & `pingpongsdk-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingpongsdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Ewan Valentine
 Author-email: ewan.valentine89@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 
 from pingpongsdk import PingPong
 from pingpongsdk.deployments.model import CreateDeployment
 
 pingpong = PingPong()
 deployment = pingpong.deployments.create(deployment=CreateDeployment(
     name="example-deployment",
-    model='pingpongai/<model-name>',
+    model='pingpongai/ai-image-scan',
     args={
         'input_image_file': 'https://cdn.mediamagic.dev/media/eb341446-be53-11ed-b4a8-66139910f724.jpg',
     }
 ))
 
 ```
```

