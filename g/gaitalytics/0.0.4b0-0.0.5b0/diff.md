# Comparing `tmp/gaitalytics-0.0.4b0.tar.gz` & `tmp/gaitalytics-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.0.4b0.tar", last modified: Wed Jun 21 08:13:38 2023, max compression
+gzip compressed data, was "gaitalytics-0.0.5b0.tar", last modified: Wed Jun 21 08:19:59 2023, max compression
```

## Comparing `gaitalytics-0.0.4b0.tar` & `gaitalytics-0.0.5b0.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:13:38.333640 gaitalytics-0.0.4b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.4b0/LICENSE
--rw-rw-rw-   0        0        0     1405 2023-06-21 08:13:38.333640 gaitalytics-0.0.4b0/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.4b0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 08:13:38.332640 gaitalytics-0.0.4b0/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     1405 2023-06-21 08:13:38.000000 gaitalytics-0.0.4b0/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-21 08:13:38.000000 gaitalytics-0.0.4b0/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:13:38.000000 gaitalytics-0.0.4b0/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-21 08:13:38.000000 gaitalytics-0.0.4b0/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:13:38.000000 gaitalytics-0.0.4b0/gaitalytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.0.4b0/pyproject.toml
--rw-rw-rw-   0        0        0      667 2023-06-21 08:13:38.335642 gaitalytics-0.0.4b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:59.424991 gaitalytics-0.0.5b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.5b0/LICENSE
+-rw-rw-rw-   0        0        0     1405 2023-06-21 08:19:59.424991 gaitalytics-0.0.5b0/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.5b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.0.5b0/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-06-21 08:19:59.427603 gaitalytics-0.0.5b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:59.395809 gaitalytics-0.0.5b0/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:59.415404 gaitalytics-0.0.5b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:54:38.000000 gaitalytics-0.0.5b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    19482 2023-06-20 16:36:53.000000 gaitalytics-0.0.5b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    10450 2023-06-21 06:41:27.000000 gaitalytics-0.0.5b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     4160 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    18703 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15087 2023-06-20 18:48:37.000000 gaitalytics-0.0.5b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     9354 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6051 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0     1505 2023-06-20 15:51:04.000000 gaitalytics-0.0.5b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:59.424487 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     1405 2023-06-21 08:19:59.000000 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-21 08:19:59.000000 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:19:59.000000 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-21 08:19:59.000000 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 08:19:59.000000 gaitalytics-0.0.5b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.0.4b0/LICENSE` & `gaitalytics-0.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.4b0/PKG-INFO` & `gaitalytics-0.0.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gait_analysis
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaitalytics-0.0.4b0/README.md` & `gaitalytics-0.0.5b0/README.md`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.4b0/gaitalytics.egg-info/PKG-INFO` & `gaitalytics-0.0.5b0/src/gaitalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gait_analysis
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaitalytics-0.0.4b0/setup.cfg` & `gaitalytics-0.0.5b0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 3462  version = 0.0.4b
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 3562  version = 0.0.5b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
@@ -28,15 +28,19 @@
 000001b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
 000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
 000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
 000001e0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
 000001f0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 00000200: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 00000210: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000220: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
-00000230: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000240: 0970 616e 6461 730d 0a09 7079 7961 6d6c  .pandas...pyyaml
-00000250: 0d0a 096d 6174 706c 6f74 6c69 620d 0a09  ...matplotlib...
-00000260: 6e75 6d70 790d 0a09 7363 6970 790d 0a0d  numpy...scipy...
-00000270: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000280: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000290: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000220: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
+00000230: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000240: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000250: 6573 203d 200d 0a09 7061 6e64 6173 0d0a  es = ...pandas..
+00000260: 0970 7979 616d 6c0d 0a09 6d61 7470 6c6f  .pyyaml...matplo
+00000270: 746c 6962 0d0a 096e 756d 7079 0d0a 0973  tlib...numpy...s
+00000280: 6369 7079 0d0a 0d0a 5b6f 7074 696f 6e73  cipy....[options
+00000290: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000002a0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+000002b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000002c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

