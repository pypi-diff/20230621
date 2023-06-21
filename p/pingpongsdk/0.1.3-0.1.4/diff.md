# Comparing `tmp/pingpongsdk-0.1.3.tar.gz` & `tmp/pingpongsdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingpongsdk-0.1.3.tar", max compression
+gzip compressed data, was "pingpongsdk-0.1.4.tar", max compression
```

## Comparing `pingpongsdk-0.1.3.tar` & `pingpongsdk-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,16 @@
--rw-r--r--   0        0        0      747 2023-03-09 11:45:56.465044 pingpongsdk-0.1.3/README.md
--rw-r--r--   0        0        0      510 2023-03-09 11:43:10.990049 pingpongsdk-0.1.3/pingpongsdk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 10:51:02.603747 pingpongsdk-0.1.3/pingpongsdk/deployments/__init__.py
--rw-r--r--   0        0        0      191 2023-03-09 08:29:57.155998 pingpongsdk-0.1.3/pingpongsdk/deployments/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2738 2023-03-09 09:58:37.797021 pingpongsdk-0.1.3/pingpongsdk/deployments/__pycache__/deployments.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-03-09 10:58:21.110673 pingpongsdk-0.1.3/pingpongsdk/deployments/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     3324 2023-03-09 10:57:16.857101 pingpongsdk-0.1.3/pingpongsdk/deployments/__pycache__/test_deployments.cpython-311-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1152 2023-03-09 09:58:32.608557 pingpongsdk-0.1.3/pingpongsdk/deployments/deployments.py
--rw-r--r--   0        0        0      472 2023-03-09 10:58:03.917210 pingpongsdk-0.1.3/pingpongsdk/deployments/model.py
--rw-r--r--   0        0        0      754 2023-03-09 09:37:50.806133 pingpongsdk-0.1.3/pingpongsdk/deployments/test_deployments.py
--rw-r--r--   0        0        0        0 2023-03-07 10:25:11.654435 pingpongsdk-0.1.3/pingpongsdk/models/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 10:29:01.122612 pingpongsdk-0.1.3/pingpongsdk/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      765 2023-03-09 08:29:57.253234 pingpongsdk-0.1.3/pingpongsdk/models/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     2494 2023-03-09 11:44:42.320106 pingpongsdk-0.1.3/pingpongsdk/models/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     3222 2023-03-09 08:29:57.251750 pingpongsdk-0.1.3/pingpongsdk/models/__pycache__/test_models.cpython-311-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      191 2023-03-09 08:13:16.365361 pingpongsdk-0.1.3/pingpongsdk/models/model.py
--rw-r--r--   0        0        0      894 2023-03-09 11:44:38.310879 pingpongsdk-0.1.3/pingpongsdk/models/models.py
--rw-r--r--   0        0        0      503 2023-03-07 10:50:52.527135 pingpongsdk-0.1.3/pingpongsdk/models/test_models.py
--rw-r--r--   0        0        0        0 2023-03-07 10:30:59.063001 pingpongsdk-0.1.3/pingpongsdk/shared/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 10:31:00.990567 pingpongsdk-0.1.3/pingpongsdk/shared/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-03-07 10:28:06.621784 pingpongsdk-0.1.3/pingpongsdk/shared/client/__init__.py
--rw-r--r--   0        0        0      193 2023-03-07 10:29:28.629410 pingpongsdk-0.1.3/pingpongsdk/shared/client/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2160 2023-03-09 10:57:16.815786 pingpongsdk-0.1.3/pingpongsdk/shared/client/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     1089 2023-03-09 10:56:37.514088 pingpongsdk-0.1.3/pingpongsdk/shared/client/client.py
--rw-r--r--   0        0        0     1006 2023-03-09 09:38:24.019817 pingpongsdk-0.1.3/pingpongsdk/shared/model/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-03-09 11:09:06.221521 pingpongsdk-0.1.3/pingpongsdk/tests/__init__.py
--rw-r--r--   0        0        0      280 2023-03-09 11:47:02.237396 pingpongsdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 pingpongsdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      430 2023-06-21 16:48:36.511402 pingpongsdk-0.1.4/README.md
+-rw-r--r--   0        0        0      510 2023-06-12 15:18:48.399004 pingpongsdk-0.1.4/pingpongsdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:51:02.603747 pingpongsdk-0.1.4/pingpongsdk/deployments/__init__.py
+-rw-r--r--   0        0        0     1120 2023-06-21 16:48:11.346070 pingpongsdk-0.1.4/pingpongsdk/deployments/deployments.py
+-rw-r--r--   0        0        0      472 2023-06-12 15:18:48.399442 pingpongsdk-0.1.4/pingpongsdk/deployments/model.py
+-rw-r--r--   0        0        0      754 2023-06-12 15:18:48.400649 pingpongsdk-0.1.4/pingpongsdk/deployments/test_deployments.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:25:11.654435 pingpongsdk-0.1.4/pingpongsdk/models/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-12 15:18:48.401347 pingpongsdk-0.1.4/pingpongsdk/models/model.py
+-rw-r--r--   0        0        0      894 2023-06-12 15:18:48.401588 pingpongsdk-0.1.4/pingpongsdk/models/models.py
+-rw-r--r--   0        0        0      503 2023-03-07 10:50:52.527135 pingpongsdk-0.1.4/pingpongsdk/models/test_models.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:30:59.063001 pingpongsdk-0.1.4/pingpongsdk/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:28:06.621784 pingpongsdk-0.1.4/pingpongsdk/shared/client/__init__.py
+-rw-r--r--   0        0        0     1089 2023-06-12 15:18:48.401850 pingpongsdk-0.1.4/pingpongsdk/shared/client/client.py
+-rw-r--r--   0        0        0        0 2023-03-09 11:09:06.221521 pingpongsdk-0.1.4/pingpongsdk/tests/__init__.py
+-rw-r--r--   0        0        0      279 2023-06-21 16:50:52.195999 pingpongsdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 pingpongsdk-0.1.4/PKG-INFO
```

### Comparing `pingpongsdk-0.1.3/pingpongsdk/deployments/deployments.py` & `pingpongsdk-0.1.4/pingpongsdk/deployments/deployments.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
     def create(self, deployment: CreateDeployment) -> Deployment:
         """
         create - create a new Deployment
         """
         try:
             deployment = super().post("/api/v1/deployments", asdict(deployment))
-            print(deployment)
-            # return dto(deployment)
+            return dto(deployment)
         except Exception as e:
             raise Exception('error creating deployment %s' % e)
 
 
     def list(self, start: int, to: int) -> list[Deployment]:
         """
         list - list all of your deployments
```

### Comparing `pingpongsdk-0.1.3/pingpongsdk/deployments/test_deployments.py` & `pingpongsdk-0.1.4/pingpongsdk/deployments/test_deployments.py`

 * *Files identical despite different names*

### Comparing `pingpongsdk-0.1.3/pingpongsdk/models/models.py` & `pingpongsdk-0.1.4/pingpongsdk/models/models.py`

 * *Files identical despite different names*

### Comparing `pingpongsdk-0.1.3/pingpongsdk/shared/client/client.py` & `pingpongsdk-0.1.4/pingpongsdk/shared/client/client.py`

 * *Files identical despite different names*

