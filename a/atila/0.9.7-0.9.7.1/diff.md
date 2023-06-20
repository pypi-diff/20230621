# Comparing `tmp/atila-0.9.7-py3-none-any.whl.zip` & `tmp/atila-0.9.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 125698 bytes, number of entries: 36
+Zip file size: 125707 bytes, number of entries: 36
 -rw-rw-r--  2.0 unx     2172 b- defN 20-Oct-05 06:34 atila/named_session.py
 -rw-rw-r--  2.0 unx     3127 b- defN 20-Oct-05 06:34 atila/session.py
 -rw-rw-r--  2.0 unx    14125 b- defN 21-May-02 10:14 atila/was.py
 -rw-rw-r--  2.0 unx     2467 b- defN 20-Oct-05 06:34 atila/mbox.py
 -rw-rw-r--  2.0 unx    11685 b- defN 21-May-02 15:49 atila/Atila.py
 -rw-rw-r--  2.0 unx      947 b- defN 21-Apr-16 07:08 atila/pytest_hooks.py
 -rw-rw-r--  2.0 unx     4838 b- defN 20-Oct-05 06:34 atila/cookie.py
 -rw-rw-r--  2.0 unx     6675 b- defN 20-Oct-05 06:34 atila/secured_cookie_value.py
--rw-rw-r--  2.0 unx     2350 b- defN 21-May-02 23:00 atila/__init__.py
+-rw-rw-r--  2.0 unx     2352 b- defN 21-May-03 05:40 atila/__init__.py
 -rw-rw-r--  2.0 unx     3805 b- defN 20-Oct-05 06:34 atila/authorizer.py
 -rw-rw-r--  2.0 unx    12157 b- defN 20-Oct-05 06:34 atila/app/auth.py
 -rw-rw-r--  2.0 unx      953 b- defN 21-Apr-18 12:29 atila/app/testutils.py
 -rw-rw-r--  2.0 unx    18586 b- defN 21-May-02 15:16 atila/app/router.py
 -rw-rw-r--  2.0 unx     6056 b- defN 21-May-02 04:24 atila/app/template_engine.py
 -rw-rw-r--  2.0 unx     2853 b- defN 20-Oct-05 06:34 atila/app/events.py
 -rw-rw-r--  2.0 unx    23623 b- defN 21-May-02 14:23 atila/app/decorators.py
@@ -25,14 +25,14 @@
 -rw-rw-r--  2.0 unx       81 b- defN 20-Oct-05 06:34 atila/patches/skitaipatch.py
 -rw-rw-r--  2.0 unx     6281 b- defN 20-Oct-08 01:28 atila/patches/djangopatch.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Oct-05 06:34 atila/patches/__init__.py
 -rw-rw-r--  2.0 unx    12386 b- defN 21-Apr-05 04:39 atila/collectors/multipart_collector.py
 -rw-rw-r--  2.0 unx     2846 b- defN 20-Oct-13 11:10 atila/collectors/grpc_collector.py
 -rw-rw-r--  2.0 unx     1592 b- defN 20-Oct-13 11:40 atila/collectors/websocket_collector.py
 -rw-rw-r--  2.0 unx     3048 b- defN 20-Oct-13 14:15 atila/collectors/stream_collector.py
--rw-rw-r--  2.0 unx   117971 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx     1012 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/metadata.json
--rw-rw-r--  2.0 unx        6 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx   118828 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/METADATA
--rw-rw-r--  2.0 unx     2968 b- defN 21-May-02 23:14 atila-0.9.7.dist-info/RECORD
-36 files, 422852 bytes uncompressed, 121070 bytes compressed:  71.4%
+-rw-rw-r--  2.0 unx   117971 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx     1003 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        6 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx   118819 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2980 b- defN 21-May-03 05:40 atila-0.9.7.1.dist-info/RECORD
+36 files, 422848 bytes uncompressed, 121055 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -84,26 +84,26 @@
 
 Filename: atila/collectors/websocket_collector.py
 Comment: 
 
 Filename: atila/collectors/stream_collector.py
 Comment: 
 
-Filename: atila-0.9.7.dist-info/DESCRIPTION.rst
+Filename: atila-0.9.7.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: atila-0.9.7.dist-info/metadata.json
+Filename: atila-0.9.7.1.dist-info/metadata.json
 Comment: 
 
-Filename: atila-0.9.7.dist-info/top_level.txt
+Filename: atila-0.9.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: atila-0.9.7.dist-info/WHEEL
+Filename: atila-0.9.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: atila-0.9.7.dist-info/METADATA
+Filename: atila-0.9.7.1.dist-info/METADATA
 Comment: 
 
-Filename: atila-0.9.7.dist-info/RECORD
+Filename: atila-0.9.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atila/__init__.py

```diff
@@ -1,13 +1,13 @@
 """
 2015. 12. 10
 Hans Roh
 """
 
-__version__ = "0.9.7"
+__version__ = "0.9.7.1"
 
 version_info = tuple (map (lambda x: not x.isdigit () and x or int (x),  __version__.split (".")))
 assert len ([x for  x in version_info [:2] if isinstance (x, int)]) == 2, 'major and minor version should be integer'
 
 from .patches import skitaipatch
 from .Atila import Atila
 import os
```

## Comparing `atila-0.9.7.dist-info/DESCRIPTION.rst` & `atila-0.9.7.1.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `atila-0.9.7.dist-info/metadata.json` & `atila-0.9.7.1.dist-info/metadata.json`

 * *Files 17% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['skitai']}}", "'version'": "'0.9.7.1'"}*

```diff
@@ -35,14 +35,14 @@
     "license": "MIT",
     "metadata_version": "2.0",
     "name": "atila",
     "platform": "posix",
     "run_requires": [
         {
             "requires": [
-                "skitai (>=0.36.8)"
+                "skitai"
             ]
         }
     ],
     "summary": "Atila Framework",
-    "version": "0.9.7"
+    "version": "0.9.7.1"
 }
```

## Comparing `atila-0.9.7.dist-info/METADATA` & `atila-0.9.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: atila
-Version: 0.9.7
+Version: 0.9.7.1
 Summary: Atila Framework
 Home-page: https://gitlab.com/sitai/atila
 Author: Hans Roh
 Author-email: hansroh@gmail.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/atila
 Platform: posix
@@ -16,15 +16,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: skitai (>=0.36.8)
+Requires-Dist: skitai
 
 Atila
 ===========
 
 *Atila* is simple and minimal framework integrated with `Skitai App Engine`_.
 It is the easiest way to make backend API services.
```

## Comparing `atila-0.9.7.dist-info/RECORD` & `atila-0.9.7.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 atila/Atila.py,sha256=bDbYvZJty9I0fAGD0O749bvLCQpgp_cQFIjakbR2DRg,11685
-atila/__init__.py,sha256=p_k3xeNZCPrYrmHoCkLC5vy8J_wD_PkdR0cpmFQi19g,2350
+atila/__init__.py,sha256=eD2cIeSfk2c_9eI7DDFAquwZh7TBq2XycM7qyth2RBs,2352
 atila/authorizer.py,sha256=CnbYq9L2VPdAEvIAW7tPXFktLH_twRIK-V-hLUPlcUo,3805
 atila/cookie.py,sha256=g8w_z4mfWJW65hIL0OZ9L9HqDHR7kQFPNMzPgYQBv-0,4838
 atila/mbox.py,sha256=t4dgKHLgzol6AehN_9KfzsroUFaSHQJa3RmnXcT_ANI,2467
 atila/named_session.py,sha256=I2uBQl3vL7c-D6a8kK9Jn1YwHJd1CwgAnlBKV29lQNM,2172
 atila/pytest_hooks.py,sha256=aqQoarDRJUAnI0EWORHoPXSqGJfMiJqsNNi9h-9T89w,947
 atila/secured_cookie_value.py,sha256=asWdCXYcaoLiMdaefvNME08jMHQSoQ7yOde6deeA_pk,6675
 atila/session.py,sha256=JyycU0wU65sOBI_C3m1skzzisNxnAAILOkdrT7NBPV8,3127
@@ -24,13 +24,13 @@
 atila/executors/ws_executor.py,sha256=RmVl3vC-giymxu-m1IEvpp6TAj0hVcLZ1pXvy-JxRew,531
 atila/executors/wsgi_executor.py,sha256=DX-Q9PAhHOmzFj8phQfKUmUGdwwMIkv4nNrqP_JuNOs,11598
 atila/executors/xmlrpc_executor.py,sha256=vCo56CaDCow8Pss-9xKuth9eDo5wCnzLUk7e9i8nKY8,1931
 atila/patches/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atila/patches/djangopatch.py,sha256=RlW4SURJjSiA1HZ2qlfBihmJwrBC17N71k3_JntCPXw,6281
 atila/patches/jinjapatch.py,sha256=JFdfPVwTMd-2WY4fnV7-t4er_khL72DCXLETaHemyJw,2714
 atila/patches/skitaipatch.py,sha256=nPHRBfjTVBtVBW-4YH3wc1xk2l3WSfcEImqG5gbtZdw,81
-atila-0.9.7.dist-info/DESCRIPTION.rst,sha256=nxvIgS9ieBermYQv-fiirSdJs6vo4obybcmHjmc9gmk,117971
-atila-0.9.7.dist-info/METADATA,sha256=7lOcjxgyNfE0k7YPiQe1TVQEJnRKpJCpvcP1cTAugZc,118828
-atila-0.9.7.dist-info/RECORD,,
-atila-0.9.7.dist-info/WHEEL,sha256=rNo05PbNqwnXiIHFsYm0m22u4Zm6YJtugFG2THx4w3g,92
-atila-0.9.7.dist-info/metadata.json,sha256=kKwv1Mg4bMu6gVNyRvmCUGff9pP4kmu-bsw9Jv8df5w,1012
-atila-0.9.7.dist-info/top_level.txt,sha256=6yuCsTGtBh6xMJtmM4Kns8owdFj01IYT6yrXp4G3BCY,6
+atila-0.9.7.1.dist-info/DESCRIPTION.rst,sha256=nxvIgS9ieBermYQv-fiirSdJs6vo4obybcmHjmc9gmk,117971
+atila-0.9.7.1.dist-info/METADATA,sha256=UTVudnVpR7e0wc4Nk5XYlNmXneVekyokDkS33Lf-6LM,118819
+atila-0.9.7.1.dist-info/RECORD,,
+atila-0.9.7.1.dist-info/WHEEL,sha256=rNo05PbNqwnXiIHFsYm0m22u4Zm6YJtugFG2THx4w3g,92
+atila-0.9.7.1.dist-info/metadata.json,sha256=ozrY1lbRec2UfeJX5PLx6JYEF9MiVQOE3WBvki2u1wY,1003
+atila-0.9.7.1.dist-info/top_level.txt,sha256=6yuCsTGtBh6xMJtmM4Kns8owdFj01IYT6yrXp4G3BCY,6
```

