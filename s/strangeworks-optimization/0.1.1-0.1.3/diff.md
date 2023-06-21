# Comparing `tmp/strangeworks_optimization-0.1.1.tar.gz` & `tmp/strangeworks_optimization-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.1.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.3.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.1.tar` & `strangeworks_optimization-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/README.md
--rw-r--r--   0        0        0      919 2023-06-15 13:10:45.083640 strangeworks_optimization-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      174 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     1968 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/README.md
+-rw-r--r--   0        0        0      993 2023-06-21 09:22:25.630510 strangeworks_optimization-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     2283 2023-06-21 09:22:09.749642 strangeworks_optimization-0.1.3/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.3/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.1/strangeworks_optimization/optimization.py` & `strangeworks_optimization-0.1.3/strangeworks_optimization/optimization.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 path = "qubo"
 
 
 class OptimizationJob:
     def __init__(
         self,
-        bqm: BinaryQuadraticModel | Dict,
+        model: BinaryQuadraticModel | Dict,
         var_type: str,
         lagrange_multiplier: float,
         solver: dict,
     ) -> None:
         self.var_type = var_type
         self.lagrange_multiplier = lagrange_multiplier
         self.solver = solver
-        self.model = json.dumps(bqm.to_serializable())
+        self.model = json.dumps(model.to_serializable())
 
 
 class StrangeworksOptimization:
     """Strangeworks client object."""
 
     def __init__(self, resource_slug: Optional[str] = " ") -> None:
         if resource_slug != " " and resource_slug != "":
@@ -62,9 +62,18 @@
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
         else:
             job_slug = sw_job.slug
 
         return sw.jobs(slug=job_slug)[0].status
 
-    # def get_backends(self):
-    # todo: implement this
+    def backends(self):
+        """
+        To-Do: Add cross check as to which backends the current user actually has
+          access to.
+                Currently, this just lists all backends that could work with the qaoa
+                  service.
+        """
+
+        self.backends = sw.backends(backend_type_slugs=["optimization"])
+
+        return self.backends
```

