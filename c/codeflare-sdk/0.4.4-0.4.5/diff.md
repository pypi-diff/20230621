# Comparing `tmp/codeflare_sdk-0.4.4.tar.gz` & `tmp/codeflare_sdk-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.4.4.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.4.5.tar", max compression
```

## Comparing `codeflare_sdk-0.4.4.tar` & `codeflare_sdk-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-06 14:48:51.492503 codeflare_sdk-0.4.4/LICENSE
--rw-r--r--   0        0        0     3501 2023-06-08 11:59:02.916039 codeflare_sdk-0.4.4/README.md
--rw-r--r--   0        0        0      826 2023-06-08 12:24:02.233819 codeflare_sdk-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497258 codeflare_sdk-0.4.4/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497352 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4434 2023-04-10 20:47:55.250729 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0     3931 2023-06-07 19:18:08.800687 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/awload.py
--rw-r--r--   0        0        0    17847 2023-06-07 19:18:08.801280 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1706 2023-04-07 18:58:14.108111 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-04-06 14:48:51.497790 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497880 codeflare_sdk-0.4.4/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6618 2023-05-11 16:55:51.327687 codeflare_sdk-0.4.4/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    10292 2023-04-06 14:48:51.498140 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/aw-kuberay.yaml
--rw-r--r--   0        0        0     7782 2023-04-10 20:47:55.251043 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0    10080 2023-05-11 16:55:51.328009 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/new-template.yaml
--rw-r--r--   0        0        0        0 2023-04-06 14:48:51.498421 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/__init__.py
--rwxr-xr-x   0        0        0    10830 2023-04-06 14:48:51.498552 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-04-06 14:48:51.498650 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     4499 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3589 2023-06-20 18:50:42.508892 codeflare_sdk-0.4.5/README.md
+-rw-r--r--   0        0        0      835 2023-06-20 23:01:36.939282 codeflare_sdk-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.5/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     4434 2023-04-11 19:26:34.787878 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0     3931 2023-06-20 18:50:33.161832 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/awload.py
+-rw-r--r--   0        0        0    17847 2023-06-20 18:50:33.162832 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1707 2023-06-20 22:32:42.953379 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.5/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6618 2023-06-20 18:50:33.166832 codeflare_sdk-0.4.5/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    10069 2023-06-20 22:32:42.954379 codeflare_sdk-0.4.5/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.5/src/codeflare_sdk/utils/__init__.py
+-rwxr-xr-x   0        0        0    10884 2023-06-20 22:32:42.954379 codeflare_sdk-0.4.5/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.5/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.5/PKG-INFO
```

### Comparing `codeflare_sdk-0.4.4/LICENSE` & `codeflare_sdk-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/README.md` & `codeflare_sdk-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 ### Pre-commit
 
 We use pre-commit to make sure the code is consistently formatted. To make sure that pre-commit is run every time you commit changes, simply run `pre-commit install`
 
 ### Testing
 
+- To install codeflare-sdk in editable mode, run `pip install -e .` from the repo root.
 - To run the unit tests, run `pytest -v tests/unit_test.py`
 - Any new test functions/scripts can be added into the `tests` folder
 - NOTE: Functional tests coming soon, will live in `tests/func_test.py`
 
 #### Code Coverage
 
 - Run tests with the following command: `coverage run -m --source=src pytest tests/unit_test.py`
```

### Comparing `codeflare_sdk-0.4.4/pyproject.toml` & `codeflare_sdk-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.4.4"
+version = "0.4.5"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
@@ -20,15 +20,15 @@
 keywords = ['codeflare', 'python', 'sdk', 'client', 'batch', 'scale']
 
 [tool.poetry.dependencies]
 python = "^3.7"
 openshift-client = "1.0.18"
 rich = "^12.5"
 ray = {version = "2.1.0", extras = ["default"]}
-kubernetes = "26.1.0"
+kubernetes = ">= 25.3.0, < 27"
 codeflare-torchx = "0.6.0.dev0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 pdoc3 = "0.10.0"
```

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/auth.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/awload.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/awload.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     min_cpus: int = 1
     max_cpus: int = 1
     min_worker: int = 1
     max_worker: int = 1
     min_memory: int = 2
     max_memory: int = 2
     gpu: int = 0
-    template: str = f"{dir}/templates/new-template.yaml"
+    template: str = f"{dir}/templates/base-template.yaml"
     instascale: bool = False
     envs: dict = field(default_factory=dict)
     image: str = "ghcr.io/foundation-model-stack/base:ray2.1.0-py38-gpu-pytorch1.12.0cu116-20221213-193103"
```

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/cluster/model.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/job/jobs.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/templates/aw-kuberay.yaml` & `codeflare_sdk-0.4.5/src/codeflare_sdk/templates/base-template.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 apiVersion: mcad.ibm.com/v1beta1
 kind: AppWrapper
 metadata:
-  name: aw-kuberay-glue
+  name: aw-kuberay
   namespace: default
+  #new addition
+  labels:
+    orderedinstance: "m4.xlarge_g4dn.xlarge"
 spec:
   priority: 9
   resources:
     Items: []
     GenericItems:
     - replicas: 1
+      #new addition
       custompodresources:
-      - replicas: 4
+      - replicas: 1
+        requests:
+          cpu: 2
+          memory: 8G
+          nvidia.com/gpu: 0
+        limits:
+          cpu: 2
+          memory: 8G
+          nvidia.com/gpu: 0
+      - replicas: 3
         requests:
           cpu: 2
           memory: 12G
           nvidia.com/gpu: 1
         limits:
           cpu: 2
           memory: 12G
@@ -24,23 +37,23 @@
         # The resource requests and limits in this config are too small for production!
         # For an example with more realistic resource configuration, see
         # ray-cluster.autoscaler.large.yaml.
         apiVersion: ray.io/v1alpha1
         kind: RayCluster
         metadata:
           labels:
-            appwrapper.mcad.ibm.com: "aw-kuberay-glue"
+            appwrapper.mcad.ibm.com: "aw-kuberay"
             controller-tools.k8s.io: "1.0"
             # A unique identifier for the head node and workers of this cluster.
-          name: glue-cluster
+          name: kuberay-cluster
           # finalizers:
           # - kubernetes
         spec:
           # The version of Ray you are using. Make sure all Ray containers are running this version of Ray.
-          rayVersion: '1.12.0'
+          rayVersion: '2.1.0'
           # If enableInTreeAutoscaling is true, the autoscaler sidecar will be added to the Ray head pod.
           # Ray autoscaler integration is supported only for Ray versions >= 1.11.0
           # Ray autoscaler integration is Beta with KubeRay >= 0.3.0 and Ray >= 2.0.0.
           enableInTreeAutoscaling: false
           # autoscalerOptions is an OPTIONAL field specifying configuration overrides for the Ray autoscaler.
           # The example configuration shown below below represents the DEFAULT values.
           # (You may delete autoscalerOptions if the defaults are suitable.)
@@ -85,64 +98,54 @@
               # The value of `resources` is a string-integer mapping.
               # Currently, `resources` must be provided in the specific format demonstrated below:
               # resources: '"{\"Custom1\": 1, \"Custom2\": 5}"'
               num-gpus: '0'
             #pod template
             template:
               spec:
+                #new addition
                 affinity:
                   nodeAffinity:
                     requiredDuringSchedulingIgnoredDuringExecution:
                       nodeSelectorTerms:
                       - matchExpressions:
-                        - key: aw-kuberay-glue #--> key changed to AW name
+                        - key: aw-kuberay
                           operator: In
                           values:
-                          - "aw-kuberay-glue"
+                          - "aw-kuberay"
                 containers:
                 # The Ray head pod
-                - name: ray-head
-                  image: asm582/codeflare-tl-aws:latest
-                  env:
-                  - name: AWS_ACCESS_KEY_ID
+                - env:
+                  - name: MY_POD_IP
                     valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: AWS_ACCESS_KEY_ID
-                  - name: AWS_SECRET_ACCESS_KEY
-                    valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: AWS_SECRET_ACCESS_KEY
-                  - name: ENDPOINT_URL
-                    valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: ENDPOINT_URL
+                      fieldRef:
+                        fieldPath: status.podIP
+                  name: ray-head
+                  image: rayproject/ray:latest
                   imagePullPolicy: Always
                   ports:
                   - containerPort: 6379
                     name: gcs
                   - containerPort: 8265
                     name: dashboard
                   - containerPort: 10001
                     name: client
                   lifecycle:
                     preStop:
                       exec:
                         command: ["/bin/sh","-c","ray stop"]
                   resources:
                     limits:
-                      cpu: "2"
-                      memory: "12G"
-                      nvidia.com/gpu: "0"
+                      cpu: 2
+                      memory: "8G"
+                      nvidia.com/gpu: 0
                     requests:
-                      cpu: "2"
-                      memory: "12G"
-                      nvidia.com/gpu: "0"
+                      cpu: 2
+                      memory: "8G"
+                      nvidia.com/gpu: 0
           workerGroupSpecs:
           # the pod replicas in this group typed worker
           - replicas: 3
             minReplicas: 3
             maxReplicas: 3
             # logical group name, for this called small-group, also can be functional
             groupName: small-group
@@ -154,15 +157,15 @@
             #  workersToDelete:
             #  - raycluster-complete-worker-small-group-bdtwh
             #  - raycluster-complete-worker-small-group-hv457
             #  - raycluster-complete-worker-small-group-k8tj7
             # the following params are used to complete the ray start: ray start --block ...
             rayStartParams:
               block: 'true'
-              num-gpus: '1'
+              num-gpus: 1
             #pod template
             template:
               metadata:
                 labels:
                   key: value
                 # annotations for pod
                 annotations:
@@ -171,42 +174,31 @@
                 # - kubernetes
               spec:
                 affinity:
                   nodeAffinity:
                     requiredDuringSchedulingIgnoredDuringExecution:
                       nodeSelectorTerms:
                       - matchExpressions:
-                        - key: aw-kuberay-glue #--> key changed to AW name
+                        - key: aw-kuberay
                           operator: In
                           values:
-                          - "aw-kuberay-glue"
+                          - "aw-kuberay"
                 initContainers:
                 # the env var $RAY_IP is set by the operator if missing, with the value of the head service name
                 - name: init-myservice
                   image: busybox:1.28
                   command: ['sh', '-c', "until nslookup $RAY_IP.$(cat /var/run/secrets/kubernetes.io/serviceaccount/namespace).svc.cluster.local; do echo waiting for myservice; sleep 2; done"]
                 containers:
                 - name: machine-learning # must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character (e.g. 'my-name',  or '123-abc'
-                  image: asm582/codeflare-tl-aws:latest
+                  image: rayproject/ray:latest
                   env:
-                  - name: AWS_ACCESS_KEY_ID
-                    valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: AWS_ACCESS_KEY_ID
-                  - name: AWS_SECRET_ACCESS_KEY
-                    valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: AWS_SECRET_ACCESS_KEY
-                  - name: ENDPOINT_URL
+                  - name: MY_POD_IP
                     valueFrom:
-                      secretKeyRef:
-                        name: glue-s3-creds
-                        key: ENDPOINT_URL
+                      fieldRef:
+                        fieldPath: status.podIP
                   # environment variables to set in the container.Optional.
                   # Refer to https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/
                   lifecycle:
                     preStop:
                       exec:
                         command: ["/bin/sh","-c","ray stop"]
                   resources:
@@ -214,7 +206,23 @@
                       cpu: "2"
                       memory: "12G"
                       nvidia.com/gpu: "1"
                     requests:
                       cpu: "2"
                       memory: "12G"
                       nvidia.com/gpu: "1"
+    - replica: 1
+      generictemplate:
+        kind: Route
+        apiVersion: route.openshift.io/v1
+        metadata:
+          name: ray-dashboard-deployment-name
+          namespace: default
+          labels:
+            # allows me to return name of service that Ray operator creates
+            odh-ray-cluster-service: deployment-name-head-svc
+        spec:
+          to:
+            kind: Service
+            name: deployment-name-head-svc
+          port:
+            targetPort: dashboard
```

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,16 @@
 
         for comp in [head, worker]:
             spec = comp.get("template").get("spec")
             update_affinity(spec, appwrapper_name, instascale)
             update_image(spec, image)
             update_env(spec, env)
             if comp == head:
-                update_resources(spec, 2, 2, 8, 8, 0)
+                # TODO: Eventually add head node configuration outside of template
+                continue
             else:
                 update_resources(spec, min_cpu, max_cpu, min_memory, max_memory, gpu)
 
 
 def write_user_appwrapper(user_yaml, output_file_name):
     with open(output_file_name, "w") as outfile:
         yaml.dump(user_yaml, outfile, default_flow_style=False)
```

### Comparing `codeflare_sdk-0.4.4/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.4.5/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.4/PKG-INFO` & `codeflare_sdk-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.7,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: codeflare-torchx (==0.6.0.dev0)
-Requires-Dist: kubernetes (==26.1.0)
+Requires-Dist: kubernetes (>=25.3.0,<27)
 Requires-Dist: openshift-client (==1.0.18)
 Requires-Dist: ray[default] (==2.1.0)
 Requires-Dist: rich (>=12.5,<13.0)
 Project-URL: Repository, https://github.com/project-codeflare/codeflare-sdk
 Description-Content-Type: text/markdown
 
 # Codeflare-SDK
@@ -50,14 +50,15 @@
 
 ### Pre-commit
 
 We use pre-commit to make sure the code is consistently formatted. To make sure that pre-commit is run every time you commit changes, simply run `pre-commit install`
 
 ### Testing
 
+- To install codeflare-sdk in editable mode, run `pip install -e .` from the repo root.
 - To run the unit tests, run `pytest -v tests/unit_test.py`
 - Any new test functions/scripts can be added into the `tests` folder
 - NOTE: Functional tests coming soon, will live in `tests/func_test.py`
 
 #### Code Coverage
 
 - Run tests with the following command: `coverage run -m --source=src pytest tests/unit_test.py`
```

