# Comparing `tmp/genopyc-1.0.2-py3-none-any.whl.zip` & `tmp/genopyc-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 20542 bytes, number of entries: 7
+Zip file size: 20541 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx      917 b- defN 23-Jun-21 11:24 genopyc/__init__.py
 -rwxrwxrwx  2.0 unx    32935 b- defN 23-Jun-21 11:26 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-21 11:31 genopyc-1.0.2.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-21 11:31 genopyc-1.0.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-21 11:31 genopyc-1.0.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-21 11:31 genopyc-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-Jun-21 11:31 genopyc-1.0.2.dist-info/RECORD
-7 files, 69611 bytes uncompressed, 19588 bytes compressed:  71.9%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-21 11:35 genopyc-1.0.4.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-21 11:35 genopyc-1.0.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-21 11:35 genopyc-1.0.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-21 11:35 genopyc-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-Jun-21 11:35 genopyc-1.0.4.dist-info/RECORD
+7 files, 69611 bytes uncompressed, 19587 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-1.0.2.dist-info/LICENSE.txt
+Filename: genopyc-1.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.0.2.dist-info/METADATA
+Filename: genopyc-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.0.2.dist-info/WHEEL
+Filename: genopyc-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.0.2.dist-info/top_level.txt
+Filename: genopyc-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.0.2.dist-info/RECORD
+Filename: genopyc-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `genopyc-1.0.2.dist-info/LICENSE.txt` & `genopyc-1.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.0.2.dist-info/METADATA` & `genopyc-1.0.4.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.0.2
+Version: 1.0.4
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

## Comparing `genopyc-1.0.2.dist-info/RECORD` & `genopyc-1.0.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 genopyc/__init__.py,sha256=Evc18XwNN4kPqHdq62q_qSYtBIQmYeKZQORuF99rXz8,917
 genopyc/genopyc.py,sha256=Ya3MU2VpfhSIV86wRjkTNDlBdkrTV8RQ8AkE67_dWc8,32935
-genopyc-1.0.2.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-1.0.2.dist-info/METADATA,sha256=OfIz53VC_O2gv0WQjbS7XnSniSLufIVWk528kt9H6gQ,596
-genopyc-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-1.0.2.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-1.0.2.dist-info/RECORD,,
+genopyc-1.0.4.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-1.0.4.dist-info/METADATA,sha256=D61U4N-lff_fSLZy0kNfpOdLSZEkwc-ZgLBJfwhrNw4,596
+genopyc-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-1.0.4.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-1.0.4.dist-info/RECORD,,
```

