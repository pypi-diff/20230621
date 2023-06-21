# Comparing `tmp/hypos-0.0.1.tar.gz` & `tmp/hypos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypos-0.0.1.tar", last modified: Wed Jun 21 10:36:38 2023, max compression
+gzip compressed data, was "hypos-0.0.2.tar", last modified: Wed Jun 21 10:43:37 2023, max compression
```

## Comparing `hypos-0.0.1.tar` & `hypos-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 10:36:38.801468 hypos-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-06-21 06:54:40.000000 hypos-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     5711 2023-06-21 10:36:38.799986 hypos-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5297 2023-06-20 16:35:33.000000 hypos-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 10:36:38.799986 hypos-0.0.1/hypos.egg-info/
--rw-rw-rw-   0        0        0     5711 2023-06-21 10:36:38.000000 hypos-0.0.1/hypos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-21 10:36:38.000000 hypos-0.0.1/hypos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 10:36:38.000000 hypos-0.0.1/hypos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-21 10:36:38.000000 hypos-0.0.1/hypos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 10:36:38.000000 hypos-0.0.1/hypos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4493 2023-06-20 16:31:44.000000 hypos-0.0.1/hypos.py
--rw-rw-rw-   0        0        0       42 2023-06-21 10:36:38.801468 hypos-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-06-21 10:35:47.000000 hypos-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:43:37.940349 hypos-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-21 06:54:40.000000 hypos-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     5711 2023-06-21 10:43:37.939416 hypos-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5297 2023-06-20 16:35:33.000000 hypos-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 10:43:37.938455 hypos-0.0.2/hypos.egg-info/
+-rw-rw-rw-   0        0        0     5711 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4493 2023-06-20 16:31:44.000000 hypos-0.0.2/hypos.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 10:43:37.940349 hypos-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      723 2023-06-21 10:43:22.000000 hypos-0.0.2/setup.py
```

### Comparing `hypos-0.0.1/LICENSE.md` & `hypos-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hypos-0.0.1/PKG-INFO` & `hypos-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypos
-Version: 0.0.1
+Version: 0.0.2
 Summary: PrABpY
 Home-page: https://github.com/PrABpY/ML-Hypothesis.git
 Author: prabdalip
 Author-email: anasterstudio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypos-0.0.1/README.md` & `hypos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hypos-0.0.1/hypos.egg-info/PKG-INFO` & `hypos-0.0.2/hypos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypos
-Version: 0.0.1
+Version: 0.0.2
 Summary: PrABpY
 Home-page: https://github.com/PrABpY/ML-Hypothesis.git
 Author: prabdalip
 Author-email: anasterstudio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypos-0.0.1/hypos.py` & `hypos-0.0.2/hypos.py`

 * *Files identical despite different names*

### Comparing `hypos-0.0.1/setup.py` & `hypos-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 0d0a 7769 7468 206f 7065 6e28 2252 4541  ..with open("REA
 00000030: 444d 452e 6d64 222c 2022 7222 2920 6173  DME.md", "r") as
 00000040: 2066 683a 0d0a 2020 2020 6c6f 6e67 5f64   fh:..    long_d
 00000050: 6573 6372 6970 7469 6f6e 203d 2066 682e  escription = fh.
 00000060: 7265 6164 2829 0d0a 0d0a 7365 7475 7028  read()....setup(
 00000070: 0d0a 2020 2020 6e61 6d65 3d22 6879 706f  ..    name="hypo
 00000080: 7322 2c0d 0a20 2020 2076 6572 7369 6f6e  s",..    version
-00000090: 3d22 302e 302e 3122 2c0d 0a20 2020 2061  ="0.0.1",..    a
+00000090: 3d22 302e 302e 3222 2c0d 0a20 2020 2061  ="0.0.2",..    a
 000000a0: 7574 686f 723d 2270 7261 6264 616c 6970  uthor="prabdalip
 000000b0: 222c 0d0a 2020 2020 6175 7468 6f72 5f65  ",..    author_e
 000000c0: 6d61 696c 3d22 616e 6173 7465 7273 7475  mail="anasterstu
 000000d0: 6469 6f40 676d 6169 6c2e 636f 6d22 2c0d  dio@gmail.com",.
 000000e0: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
 000000f0: 3d22 5072 4142 7059 222c 0d0a 2020 2020  ="PrABpY",..    
 00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
@@ -22,26 +22,25 @@
 00000150: 646f 776e 222c 0d0a 2020 2020 7572 6c3d  down",..    url=
 00000160: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
 00000170: 636f 6d2f 5072 4142 7059 2f4d 4c2d 4879  com/PrABpY/ML-Hy
 00000180: 706f 7468 6573 6973 2e67 6974 222c 0d0a  pothesis.git",..
 00000190: 2020 2020 6c69 6365 6e73 653d 224d 4954      license="MIT
 000001a0: 222c 0d0a 2020 2020 696e 7374 616c 6c5f  ",..    install_
 000001b0: 7265 7175 6972 6573 3d5b 0d0a 2020 2020  requires=[..    
-000001c0: 2020 2020 276e 756d 7079 272c 0d0a 2020      'numpy',..  
-000001d0: 2020 2020 2020 2769 7465 7274 6f6f 6c73        'itertools
-000001e0: 270d 0a20 2020 205d 2c0d 0a20 2020 2074  '..    ],..    t
-000001f0: 6573 7473 5f72 6571 7569 7265 3d5b 0d0a  ests_require=[..
-00000200: 2020 2020 2020 2020 2763 6f76 6572 6167          'coverag
-00000210: 6527 2c20 2777 6865 656c 272c 2027 7079  e', 'wheel', 'py
-00000220: 7465 7374 272c 2027 7265 7175 6573 7473  test', 'requests
-00000230: 5f6d 6f63 6b27 0d0a 2020 2020 5d2c 0d0a  _mock'..    ],..
-00000240: 2020 2020 636c 6173 7369 6669 6572 733d      classifiers=
-00000250: 5b0d 0a20 2020 2020 2020 2022 5072 6f67  [..        "Prog
-00000260: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000270: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
-00000280: 2c0d 0a20 2020 2020 2020 2022 4c69 6365  ,..        "Lice
-00000290: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000002a0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-000002b0: 7365 222c 0d0a 2020 2020 2020 2020 2244  se",..        "D
-000002c0: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-000002d0: 7320 3a3a 2033 202d 2041 6c70 6861 220d  s :: 3 - Alpha".
-000002e0: 0a20 2020 205d 0d0a 29                   .    ]..)
+000001c0: 2020 2020 276e 756d 7079 270d 0a20 2020      'numpy'..   
+000001d0: 205d 2c0d 0a20 2020 2074 6573 7473 5f72   ],..    tests_r
+000001e0: 6571 7569 7265 3d5b 0d0a 2020 2020 2020  equire=[..      
+000001f0: 2020 2763 6f76 6572 6167 6527 2c20 2777    'coverage', 'w
+00000200: 6865 656c 272c 2027 7079 7465 7374 272c  heel', 'pytest',
+00000210: 2027 7265 7175 6573 7473 5f6d 6f63 6b27   'requests_mock'
+00000220: 0d0a 2020 2020 5d2c 0d0a 2020 2020 636c  ..    ],..    cl
+00000230: 6173 7369 6669 6572 733d 5b0d 0a20 2020  assifiers=[..   
+00000240: 2020 2020 2022 5072 6f67 7261 6d6d 696e       "Programmin
+00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000260: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
+00000270: 2020 2020 2022 4c69 6365 6e73 6520 3a3a       "License ::
+00000280: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000290: 204d 4954 204c 6963 656e 7365 222c 0d0a   MIT License",..
+000002a0: 2020 2020 2020 2020 2244 6576 656c 6f70          "Develop
+000002b0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
+000002c0: 202d 2041 6c70 6861 220d 0a20 2020 205d   - Alpha"..    ]
+000002d0: 0d0a 29                                  ..)
```

