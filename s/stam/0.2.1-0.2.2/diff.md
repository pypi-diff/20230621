# Comparing `tmp/stam-0.2.1.tar.gz` & `tmp/stam-0.2.2.tar.gz`

## Comparing `stam-0.2.1.tar` & `stam-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 stam-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123    35147 2023-06-21 13:30:52.000000 stam-0.2.1/LICENSE
--rw-r--r--   0     1001      123     6669 2023-06-21 13:30:52.000000 stam-0.2.1/README.md
--rw-r--r--   0     1001      123      149 2023-06-21 13:30:52.000000 stam-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123    15434 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotation.rs
--rw-r--r--   0     1001      123    19159 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationdata.rs
--rw-r--r--   0     1001      123    13137 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationdataset.rs
--rw-r--r--   0     1001      123    29680 2023-06-21 13:30:52.000000 stam-0.2.1/src/annotationstore.rs
--rw-r--r--   0     1001      123     1840 2023-06-21 13:30:52.000000 stam-0.2.1/src/config.rs
--rw-r--r--   0     1001      123       98 2023-06-21 13:30:52.000000 stam-0.2.1/src/error.rs
--rw-r--r--   0     1001      123     1218 2023-06-21 13:30:52.000000 stam-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123    24828 2023-06-21 13:30:52.000000 stam-0.2.1/src/resources.rs
--rw-r--r--   0     1001      123    13953 2023-06-21 13:30:52.000000 stam-0.2.1/src/selector.rs
--rw-r--r--   0     1001      123    28540 2023-06-21 13:30:52.000000 stam-0.2.1/src/textselection.rs
--rw-r--r--   0     1001      123    18049 2023-06-21 13:31:00.000000 stam-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     7243 1970-01-01 00:00:00.000000 stam-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 stam-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123    35147 2023-06-21 13:48:48.000000 stam-0.2.2/LICENSE
+-rw-r--r--   0     1001      123     6669 2023-06-21 13:48:48.000000 stam-0.2.2/README.md
+-rw-r--r--   0     1001      123      149 2023-06-21 13:48:48.000000 stam-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123    15434 2023-06-21 13:48:48.000000 stam-0.2.2/src/annotation.rs
+-rw-r--r--   0     1001      123    19159 2023-06-21 13:48:48.000000 stam-0.2.2/src/annotationdata.rs
+-rw-r--r--   0     1001      123    13137 2023-06-21 13:48:48.000000 stam-0.2.2/src/annotationdataset.rs
+-rw-r--r--   0     1001      123    29680 2023-06-21 13:48:48.000000 stam-0.2.2/src/annotationstore.rs
+-rw-r--r--   0     1001      123     1840 2023-06-21 13:48:48.000000 stam-0.2.2/src/config.rs
+-rw-r--r--   0     1001      123       98 2023-06-21 13:48:48.000000 stam-0.2.2/src/error.rs
+-rw-r--r--   0     1001      123     1218 2023-06-21 13:48:48.000000 stam-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123    24828 2023-06-21 13:48:48.000000 stam-0.2.2/src/resources.rs
+-rw-r--r--   0     1001      123    13953 2023-06-21 13:48:48.000000 stam-0.2.2/src/selector.rs
+-rw-r--r--   0     1001      123    28540 2023-06-21 13:48:48.000000 stam-0.2.2/src/textselection.rs
+-rw-r--r--   0     1001      123    18049 2023-06-21 13:49:01.000000 stam-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     7243 1970-01-01 00:00:00.000000 stam-0.2.2/PKG-INFO
```

### Comparing `stam-0.2.1/Cargo.toml` & `stam-0.2.2/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "stam-python"
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 authors = ["Maarten van Gompel <proycon@anaproy.nl>"]
 description = "STAM is a library for dealing with standoff annotations on text"
 documentation = "https://docs.rs/stam"
 homepage = "https://github.com/annotation/stam"
 include = ["pyproject.toml", "src/**/*","tests/**/*", "LICENSE", "README.md"]
 license = "GPL-3.0-only"
@@ -14,15 +14,15 @@
 
 [lib]
 name = "stam"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = "0.19.0"
-stam = "0.7.0"
+stam = "0.7.2"
 
 [features]
 default = ["pyo3/extension-module"]
 
 [target.x86_64-apple-darwin]
 rustflags = [
   "-C", "link-arg=-undefined",
```

### Comparing `stam-0.2.1/LICENSE` & `stam-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/README.md` & `stam-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/annotation.rs` & `stam-0.2.2/src/annotation.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/annotationdata.rs` & `stam-0.2.2/src/annotationdata.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/annotationdataset.rs` & `stam-0.2.2/src/annotationdataset.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/annotationstore.rs` & `stam-0.2.2/src/annotationstore.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/config.rs` & `stam-0.2.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/lib.rs` & `stam-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/resources.rs` & `stam-0.2.2/src/resources.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/selector.rs` & `stam-0.2.2/src/selector.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/src/textselection.rs` & `stam-0.2.2/src/textselection.rs`

 * *Files identical despite different names*

### Comparing `stam-0.2.1/Cargo.lock` & `stam-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -451,32 +451,32 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "stam"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ad91f39d4dbad0081198652b205af880ebe4f50ff69cb9e271c8c3439404200"
+checksum = "6dcf187e3fee4fbaefedfac5e0f71361c019a4d35bf47c8c1b05a49a96dc56b1"
 dependencies = [
  "chrono",
  "csv",
  "nanoid",
  "regex",
  "sealed",
  "serde",
  "serde_json",
  "serde_path_to_error",
  "smallvec",
 ]
 
 [[package]]
 name = "stam-python"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "pyo3",
  "stam",
 ]
 
 [[package]]
 name = "syn"
```

### Comparing `stam-0.2.1/PKG-INFO` & `stam-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stam
-Version: 0.2.1
+Version: 0.2.2
 Requires-Dist: pytest ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: STAM is a library for dealing with standoff annotations on text
 Keywords: text-processing,annotation,linguistics,standoff,nlp
 Home-Page: https://github.com/annotation/stam
 Author: Maarten van Gompel <proycon@anaproy.nl>
```

