# Comparing `tmp/pytheus_backend_rs-0.0.3.tar.gz` & `tmp/pytheus_backend_rs-0.0.4.tar.gz`

## Comparing `pytheus_backend_rs-0.0.3.tar` & `pytheus_backend_rs-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.3/Cargo.toml
--rw-r--r--   0     1001      123     2792 2023-06-20 23:47:31.000000 pytheus_backend_rs-0.0.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-20 23:47:31.000000 pytheus_backend_rs-0.0.3/.gitignore
--rw-r--r--   0     1001      123      620 2023-06-20 23:47:31.000000 pytheus_backend_rs-0.0.3/pyproject.toml
--rw-r--r--   0     1001      123    10016 2023-06-20 23:47:31.000000 pytheus_backend_rs-0.0.3/src/lib.rs
--rw-r--r--   0     1001      123    11135 2023-06-20 23:47:31.000000 pytheus_backend_rs-0.0.3/Cargo.lock
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      123     2792 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/.gitignore
+-rw-r--r--   0     1001      123      620 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      123    10149 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      123    11135 2023-06-21 00:37:25.000000 pytheus_backend_rs-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.4/PKG-INFO
```

### Comparing `pytheus_backend_rs-0.0.3/.github/workflows/CI.yml` & `pytheus_backend_rs-0.0.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.3/.gitignore` & `pytheus_backend_rs-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.3/pyproject.toml` & `pytheus_backend_rs-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.3/src/lib.rs` & `pytheus_backend_rs-0.0.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,23 @@
         let redis_job_tx_mutex = REDIS_JOB_TX.get().unwrap();
         let redis_job_tx = redis_job_tx_mutex.lock().unwrap();
         let cloned_tx = redis_job_tx.clone();
 
         let py = metric.py();
         let collector = metric.getattr(intern!(metric.py(), "_collector"))?;
 
-        let key_name: String = metric
+        let mut key_name: String = metric
             .getattr(intern!(py, "_collector"))?
             .getattr(intern!(py, "name"))?
             .extract()?;
 
+        if let Some(bucket_id) = histogram_bucket.clone() {
+            key_name = format!("{key_name}:{bucket_id}");
+        }
+
         let mut default_labels: Option<HashMap<&str, &str>> = None;
         let mut metric_labels: Option<HashMap<&str, &str>> = None;
 
         let py_metric_labels = metric.getattr(intern!(py, "_labels"))?;
         if py_metric_labels.is_true()? {
             let labels: HashMap<&str, &str> = py_metric_labels.extract()?;
             metric_labels = Some(labels);
```

### Comparing `pytheus_backend_rs-0.0.3/Cargo.lock` & `pytheus_backend_rs-0.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytheus-backend-rs"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "itertools",
  "pyo3",
  "redis",
 ]
 
 [[package]]
```

