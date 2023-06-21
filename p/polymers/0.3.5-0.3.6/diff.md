# Comparing `tmp/polymers-0.3.5-cp39-none-win_amd64.whl.zip` & `tmp/polymers-0.3.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1479291 bytes, number of entries: 6
--rw-r--r--  4.6 unx     3523 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/WHEEL
--rw-r--r--  4.6 unx     1569 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-May-08 23:32 polymers/__init__.py
--rwxr-xr-x  4.6 unx  6302208 b- defN 23-May-08 23:32 polymers/polymers.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      484 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/RECORD
-6 files, 6307994 bytes uncompressed, 1478421 bytes compressed:  76.6%
+Zip file size: 1507625 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     3530 b- defN 23-Jun-21 16:54 polymers-0.3.6.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-21 16:54 polymers-0.3.6.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1569 b- defN 23-Jun-21 16:54 polymers-0.3.6.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-Jun-21 16:54 polymers/__init__.py
+-rwxr-xr-x  4.6 unx  6398464 b- defN 23-Jun-21 16:54 polymers/polymers.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      484 b- defN 23-Jun-21 16:54 polymers-0.3.6.dist-info/RECORD
+6 files, 6404256 bytes uncompressed, 1506755 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polymers-0.3.5.dist-info/METADATA
+Filename: polymers-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: polymers-0.3.5.dist-info/WHEEL
+Filename: polymers-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: polymers-0.3.5.dist-info/license_files/LICENSE
+Filename: polymers-0.3.6.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: polymers/__init__.py
 Comment: 
 
 Filename: polymers/polymers.cp39-win_amd64.pyd
 Comment: 
 
-Filename: polymers-0.3.5.dist-info/RECORD
+Filename: polymers-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `polymers-0.3.5.dist-info/METADATA` & `polymers-0.3.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymers
-Version: 0.3.5
+Version: 0.3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: cffi
@@ -12,15 +12,15 @@
 Requires-Dist: numpy
 License-File: LICENSE
 Summary: Polymers Modeling Library
 Keywords: julia,polymers,python,rust
 Author: Michael R. Buche
 Author-email: mrbuche@sandia.gov
 License: BSD-3-Clause
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Documentation, https://polymers.readthedocs.io
 Project-URL: Homepage, https://sandialabs.github.io/Polymers
 Project-URL: Repository, https://github.com/sandialabs/polymers
 
 # Polymers Modeling Library
```

## Comparing `polymers-0.3.5.dist-info/license_files/LICENSE` & `polymers-0.3.6.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

