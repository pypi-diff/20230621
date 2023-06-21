# Comparing `tmp/stam-0.2.0.tar.gz` & `tmp/stam-0.2.1.tar.gz`

## Comparing `stam-0.2.0.tar` & `stam-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 stam-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123    35147 2023-06-07 11:51:01.000000 stam-0.2.0/LICENSE
--rw-r--r--   0     1001      123     6669 2023-06-07 11:51:01.000000 stam-0.2.0/README.md
--rw-r--r--   0     1001      123      154 2023-06-07 11:51:01.000000 stam-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123    16125 2023-06-07 11:51:01.000000 stam-0.2.0/src/annotation.rs
--rw-r--r--   0     1001      123    19159 2023-06-07 11:51:01.000000 stam-0.2.0/src/annotationdata.rs
--rw-r--r--   0     1001      123    13137 2023-06-07 11:51:01.000000 stam-0.2.0/src/annotationdataset.rs
--rw-r--r--   0     1001      123    29679 2023-06-07 11:51:01.000000 stam-0.2.0/src/annotationstore.rs
--rw-r--r--   0     1001      123     1840 2023-06-07 11:51:01.000000 stam-0.2.0/src/config.rs
--rw-r--r--   0     1001      123       98 2023-06-07 11:51:01.000000 stam-0.2.0/src/error.rs
--rw-r--r--   0     1001      123     1218 2023-06-07 11:51:01.000000 stam-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123    24828 2023-06-07 11:51:01.000000 stam-0.2.0/src/resources.rs
--rw-r--r--   0     1001      123    13953 2023-06-07 11:51:01.000000 stam-0.2.0/src/selector.rs
--rw-r--r--   0     1001      123    28540 2023-06-07 11:51:01.000000 stam-0.2.0/src/textselection.rs
--rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 stam-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 stam-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123    35147 2023-06-21 13:30:52.000000 stam-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     6669 2023-06-21 13:30:52.000000 stam-0.2.1/README.md
+-rw-r--r--   0     1001      123      149 2023-06-21 13:30:52.000000 stam-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123    15434 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotation.rs
+-rw-r--r--   0     1001      123    19159 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationdata.rs
+-rw-r--r--   0     1001      123    13137 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationdataset.rs
+-rw-r--r--   0     1001      123    29680 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationstore.rs
+-rw-r--r--   0     1001      123     1840 2023-06-21 13:30:52.000000 stam-0.2.1/src/config.rs
+-rw-r--r--   0     1001      123       98 2023-06-21 13:30:52.000000 stam-0.2.1/src/error.rs
+-rw-r--r--   0     1001      123     1218 2023-06-21 13:30:52.000000 stam-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123    24828 2023-06-21 13:30:52.000000 stam-0.2.1/src/resources.rs
+-rw-r--r--   0     1001      123    13953 2023-06-21 13:30:52.000000 stam-0.2.1/src/selector.rs
+-rw-r--r--   0     1001      123    28540 2023-06-21 13:30:52.000000 stam-0.2.1/src/textselection.rs
+-rw-r--r--   0     1001      123    18049 2023-06-21 13:31:00.000000 stam-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     7243 1970-01-01 00:00:00.000000 stam-0.2.1/PKG-INFO
```

### Comparing `stam-0.2.0/Cargo.toml` & `stam-0.2.1/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "stam-python"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 authors = ["Maarten van Gompel <proycon@anaproy.nl>"]
 description = "STAM is a library for dealing with standoff annotations on text"
 documentation = "https://docs.rs/stam"
 homepage = "https://github.com/annotation/stam"
 include = ["pyproject.toml", "src/**/*","tests/**/*", "LICENSE", "README.md"]
 license = "GPL-3.0-only"
```

### Comparing `stam-0.2.0/LICENSE` & `stam-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/README.md` & `stam-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/annotation.rs` & `stam-0.2.1/src/annotation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -434,25 +434,8 @@
             f(annotation).map_err(|err| PyStamError::new_err(format!("{}", err)))
         } else {
             Err(PyRuntimeError::new_err(
                 "Unable to obtain store (should never happen)",
             ))
         }
     }
-
-    /// Map function to act on the actual underlying store, helps reduce boilerplate
-    fn map_mut<T, F>(&self, f: F) -> Result<T, PyErr>
-    where
-        F: FnOnce(&mut Annotation) -> Result<T, StamError>,
-    {
-        if let Ok(mut store) = self.store.write() {
-            let annotation: &mut Annotation = store
-                .get_mut(&self.handle.into())
-                .map_err(|_| PyRuntimeError::new_err("Failed to resolve textresource"))?;
-            f(annotation).map_err(|err| PyStamError::new_err(format!("{}", err)))
-        } else {
-            Err(PyRuntimeError::new_err(
-                "Unable to obtain store (should never happen)",
-            ))
-        }
-    }
 }
```

### Comparing `stam-0.2.0/src/annotationdata.rs` & `stam-0.2.1/src/annotationdata.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/annotationdataset.rs` & `stam-0.2.1/src/annotationdataset.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/annotationstore.rs` & `stam-0.2.1/src/annotationstore.rs`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     /// Returns the public ID (by value, aka a copy)
     fn id(&self) -> PyResult<Option<String>> {
         self.map(|store| Ok(store.id().map(|x| x.to_owned())))
     }
 
     /// Saves the annotation store to file
     fn to_file(&mut self, filename: &str) -> PyResult<()> {
-        self.set_filename(filename);
+        self.set_filename(filename)?;
         self.save()
     }
 
     /// Saves the annotation store to file
     fn save(&self) -> PyResult<()> {
         self.map(|store| store.save())
     }
```

### Comparing `stam-0.2.0/src/config.rs` & `stam-0.2.1/src/config.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/lib.rs` & `stam-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/resources.rs` & `stam-0.2.1/src/resources.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/selector.rs` & `stam-0.2.1/src/selector.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/src/textselection.rs` & `stam-0.2.1/src/textselection.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.0/PKG-INFO` & `stam-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: stam
-Version: 0.2.0
-Requires-Dist: pytest; extra == 'test'
+Version: 0.2.1
+Requires-Dist: pytest ; extra == 'test'
 Provides-Extra: test
+License-File: LICENSE
 Summary: STAM is a library for dealing with standoff annotations on text
 Keywords: text-processing,annotation,linguistics,standoff,nlp
 Home-Page: https://github.com/annotation/stam
 Author: Maarten van Gompel <proycon@anaproy.nl>
 Author-email: Maarten van Gompel <proycon@anaproy.nl>
 License: GPL-3.0-only
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

