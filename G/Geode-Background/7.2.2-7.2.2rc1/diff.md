# Comparing `tmp/Geode_Background-7.2.2-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Background-7.2.2rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 4637498 bytes, number of entries: 16
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-21 00:49 geode_background/__init__.py
--rw-r--r--  2.0 unx      191 b- defN 23-Jun-21 00:49 geode_background/brep.py
--rw-r--r--  2.0 unx      192 b- defN 23-Jun-21 00:49 geode_background/solid.py
--rw-r--r--  2.0 unx      196 b- defN 23-Jun-21 00:49 geode_background/surface.py
--rwxr-xr-x  2.0 unx   122232 b- defN 23-Jun-21 00:50 geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122232 b- defN 23-Jun-21 00:50 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122232 b- defN 23-Jun-21 00:50 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122232 b- defN 23-Jun-21 00:50 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx  3235248 b- defN 23-Jun-21 00:50 geode_background/lib64/libGeode-Background_brep.so
--rwxr-xr-x  2.0 unx   166552 b- defN 23-Jun-21 00:50 geode_background/lib64/libGeode-Background_common.so
--rwxr-xr-x  2.0 unx  3540560 b- defN 23-Jun-21 00:50 geode_background/lib64/libGeode-Background_solid.so
--rwxr-xr-x  2.0 unx  3260464 b- defN 23-Jun-21 00:50 geode_background/lib64/libGeode-Background_surface.so
--rw-r--r--  2.0 unx     1058 b- defN 23-Jun-21 00:50 Geode_Background-7.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-21 00:50 Geode_Background-7.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-21 00:50 Geode_Background-7.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1662 b- defN 23-Jun-21 00:50 Geode_Background-7.2.2.dist-info/RECORD
-16 files, 10695281 bytes uncompressed, 4634676 bytes compressed:  56.7%
+Zip file size: 3487177 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      216 b- defN 23-Jun-20 13:01 geode_background/__init__.py
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Jun-20 13:01 geode_background/brep.py
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Jun-20 13:01 geode_background/solid.py
+-rw-rw-rw-  2.0 fat      203 b- defN 23-Jun-20 13:01 geode_background/surface.py
+-rw-rw-rw-  2.0 fat  2133504 b- defN 23-Jun-20 13:03 geode_background/bin/Geode-Background_brep.dll
+-rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-20 13:03 geode_background/bin/Geode-Background_common.dll
+-rw-rw-rw-  2.0 fat  2378240 b- defN 23-Jun-20 13:03 geode_background/bin/Geode-Background_solid.dll
+-rw-rw-rw-  2.0 fat  2172928 b- defN 23-Jun-20 13:03 geode_background/bin/Geode-Background_surface.dll
+-rw-rw-rw-  2.0 fat   124928 b- defN 23-Jun-20 13:03 geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Jun-20 13:03 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   124928 b- defN 23-Jun-20 13:03 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Jun-20 13:03 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1108 b- defN 23-Jun-20 13:03 Geode_Background-7.2.2rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-20 13:03 Geode_Background-7.2.2rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-20 13:03 Geode_Background-7.2.2rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1601 b- defN 23-Jun-20 13:03 Geode_Background-7.2.2rc1.dist-info/RECORD
+16 files, 7254587 bytes uncompressed, 3484475 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -6,44 +6,44 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_brep.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_common.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_solid.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_surface.dll
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_brep.so
+Filename: geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_common.so
+Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_solid.so
+Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_surface.so
+Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Background-7.2.2.dist-info/METADATA
+Filename: Geode_Background-7.2.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.2.2.dist-info/WHEEL
+Filename: Geode_Background-7.2.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.2.2.dist-info/top_level.txt
+Filename: Geode_Background-7.2.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.2.2.dist-info/RECORD
+Filename: Geode_Background-7.2.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,5 +1,8 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .surface import *
-from .solid import *
-from .brep import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .surface import *
+from .solid import *
+from .brep import *
```

## geode_background/brep.py

```diff
@@ -1,10 +1,10 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_brep import *
-
-BackgroundBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_brep import *
+
+BackgroundBRepLibrary.initialize()
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.2.2.dist-info/RECORD` & `Geode_Background-7.2.2rc1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-geode_background/__init__.py,sha256=xN9xp7sD-rYx2_DVAlmXQ2DZCaivEH_fzxzx5rK54Q8,110
-geode_background/brep.py,sha256=dFe-2umFv9gMhRUkxD834QNl9oWw6PRLcHnkzhsWOhc,191
-geode_background/solid.py,sha256=kybi5kyMS2KSCgp8NgBJZisGT7hgYItke8hJV41nftA,192
-geode_background/surface.py,sha256=LVBOteZJ7wrE545OnayMOFuiN8mYCgdJclrMLM7b2TU,196
-geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=TvY89RGTvIrmJHjBSkb_19jKFS170n3r0goeSFYt4vA,122232
-geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so,sha256=0pLo5XsW7qM3RGyWWTenXi71cFgTorHVLxystNBucNY,122232
-geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so,sha256=fj9voR1_Vt9VNxKY1ztHzzzz1So0Pp0D7g920xbT2VI,122232
-geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so,sha256=utAsD6K-t-ADhnPLJPxrRprzMuha9923CTTnr7bZZp8,122232
-geode_background/lib64/libGeode-Background_brep.so,sha256=YyGDZClKruPih5KIDPWZK9ExxrWsYle7abVk78a2HPE,3235248
-geode_background/lib64/libGeode-Background_common.so,sha256=c2JbUhQ63wEwqm84IITGlj-FVR6FeAdYV0Dz3VQpQfE,166552
-geode_background/lib64/libGeode-Background_solid.so,sha256=MoOVMaVDtBonJUcFVBSlSyjYUnLTXwERMQJRnfAGhoQ,3540560
-geode_background/lib64/libGeode-Background_surface.so,sha256=Z6r__ICkCPKz7KOPof5eLJUvUmKq7AS9o-_uQPDq1Og,3260464
-Geode_Background-7.2.2.dist-info/METADATA,sha256=t14o6wVT4is6a7rg6_sdn9Tioh7dC4HBMM3LiSL1ytE,1058
-Geode_Background-7.2.2.dist-info/WHEEL,sha256=3s2LSuQQhT9U1Dyv6MxBd72puf_ocSkY6hn5h0Kjf-o,103
-Geode_Background-7.2.2.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
-Geode_Background-7.2.2.dist-info/RECORD,,
+geode_background/__init__.py,sha256=ZiWaNNKFnYl2kPUXNm9QVAx84vLbfgB7pldlbTSpUns,216
+geode_background/brep.py,sha256=M_Vf6-xgndueM-iPCMbFLnMVHqxHcPYkkf_Pdt0-40U,199
+geode_background/solid.py,sha256=DMeE_kcPihrhANbHWVJLkRmXJNV60SmALzozbU9AsXY,199
+geode_background/surface.py,sha256=KNExP1n53P95lYbgU7GJXKaZqKakt1kUzkCj3LDs4mw,203
+geode_background/bin/Geode-Background_brep.dll,sha256=IovDyN9C3rIFhBoOy4nRLN15a6jWngSAQm2CYKHCkO4,2133504
+geode_background/bin/Geode-Background_common.dll,sha256=vm52hO8Lt3FVMjas9xpRwpyiXt_4S742R0i6yxLW4tE,65536
+geode_background/bin/Geode-Background_solid.dll,sha256=Cj4vUMcXTwyJX6N0FaFyyTf6eoJvaYR-aAnJxQZ6bpg,2378240
+geode_background/bin/Geode-Background_surface.dll,sha256=ZGCtG4TwgAWLOchtANiXPRNesKGhl06KbfcUhfwH-bY,2172928
+geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd,sha256=YT0yhdLyO55lx28ZtN8HDivIrUTNjAkZHtZPy2DB6a8,124928
+geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd,sha256=MsbJqnXtwH24OP7QNuYsOlZZmnGmb1TpYCuF8IPLdZk,125440
+geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd,sha256=qsxs9jDZ595WV03xiVzT_pMPvsV8AZz6Q8vH7aURVi0,124928
+geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd,sha256=XL6JYFLVSlxD7jmChgAebnaUn5LhpYsaZsfVbA3KRbM,125440
+Geode_Background-7.2.2rc1.dist-info/METADATA,sha256=q8iyVRrUgtUOcmZwrzYsDJIpxGwbQjkok-eAHXQ-8B8,1108
+Geode_Background-7.2.2rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Background-7.2.2rc1.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
+Geode_Background-7.2.2rc1.dist-info/RECORD,,
```

