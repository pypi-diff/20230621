# Comparing `tmp/hypos-0.0.2.tar.gz` & `tmp/hypos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypos-0.0.2.tar", last modified: Wed Jun 21 10:43:37 2023, max compression
+gzip compressed data, was "hypos-0.0.3.tar", last modified: Wed Jun 21 10:50:24 2023, max compression
```

## Comparing `hypos-0.0.2.tar` & `hypos-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 10:43:37.940349 hypos-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-06-21 06:54:40.000000 hypos-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     5711 2023-06-21 10:43:37.939416 hypos-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5297 2023-06-20 16:35:33.000000 hypos-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 10:43:37.938455 hypos-0.0.2/hypos.egg-info/
--rw-rw-rw-   0        0        0     5711 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 10:43:37.000000 hypos-0.0.2/hypos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4493 2023-06-20 16:31:44.000000 hypos-0.0.2/hypos.py
--rw-rw-rw-   0        0        0       42 2023-06-21 10:43:37.940349 hypos-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      723 2023-06-21 10:43:22.000000 hypos-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:50:24.828046 hypos-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-21 06:54:40.000000 hypos-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     5709 2023-06-21 10:50:24.827088 hypos-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5295 2023-06-21 10:50:17.000000 hypos-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 10:50:24.827088 hypos-0.0.3/hypos.egg-info/
+-rw-rw-rw-   0        0        0     5709 2023-06-21 10:50:24.000000 hypos-0.0.3/hypos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-21 10:50:24.000000 hypos-0.0.3/hypos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 10:50:24.000000 hypos-0.0.3/hypos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 10:50:24.000000 hypos-0.0.3/hypos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 10:50:24.000000 hypos-0.0.3/hypos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4493 2023-06-20 16:31:44.000000 hypos-0.0.3/hypos.py
+-rw-rw-rw-   0        0        0       42 2023-06-21 10:50:24.828046 hypos-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      723 2023-06-21 10:50:14.000000 hypos-0.0.3/setup.py
```

### Comparing `hypos-0.0.2/LICENSE.md` & `hypos-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hypos-0.0.2/PKG-INFO` & `hypos-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypos
-Version: 0.0.2
+Version: 0.0.3
 Summary: PrABpY
 Home-page: https://github.com/PrABpY/ML-Hypothesis.git
 Author: prabdalip
 Author-email: anasterstudio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 ----- | ----- | ----- | ----- | ----- | ----- | ----- |
 1 | Some | Small | No | Affordable | One | No |
 2 | Many | Big | No | Expensive | Many | Yes |
 3 | Many | Medium | No | Expensive | Few | Yes |
 4 | Many | Small | No | Affordable | Many | Yes |
 
 	# Find-S
-	Hypo = Hyposis.Hypo()
+	Hypo = hypos.Hypo()
 	data = Hypo.Format("Sample.csv")
 	find_s = Hypo.FindS(data,CorrectP = "Yes",CorrectN = "No")
 	
 	# find_s -> [['Many', '?', 'No', '?', '?']]
 
 	#-------------------------------------------------------
```

### Comparing `hypos-0.0.2/README.md` & `hypos-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ----- | ----- | ----- | ----- | ----- | ----- | ----- |
 1 | Some | Small | No | Affordable | One | No |
 2 | Many | Big | No | Expensive | Many | Yes |
 3 | Many | Medium | No | Expensive | Few | Yes |
 4 | Many | Small | No | Affordable | Many | Yes |
 
 	# Find-S
-	Hypo = Hyposis.Hypo()
+	Hypo = hypos.Hypo()
 	data = Hypo.Format("Sample.csv")
 	find_s = Hypo.FindS(data,CorrectP = "Yes",CorrectN = "No")
 	
 	# find_s -> [['Many', '?', 'No', '?', '?']]
 
 	#-------------------------------------------------------
```

### Comparing `hypos-0.0.2/hypos.egg-info/PKG-INFO` & `hypos-0.0.3/hypos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypos
-Version: 0.0.2
+Version: 0.0.3
 Summary: PrABpY
 Home-page: https://github.com/PrABpY/ML-Hypothesis.git
 Author: prabdalip
 Author-email: anasterstudio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 ----- | ----- | ----- | ----- | ----- | ----- | ----- |
 1 | Some | Small | No | Affordable | One | No |
 2 | Many | Big | No | Expensive | Many | Yes |
 3 | Many | Medium | No | Expensive | Few | Yes |
 4 | Many | Small | No | Affordable | Many | Yes |
 
 	# Find-S
-	Hypo = Hyposis.Hypo()
+	Hypo = hypos.Hypo()
 	data = Hypo.Format("Sample.csv")
 	find_s = Hypo.FindS(data,CorrectP = "Yes",CorrectN = "No")
 	
 	# find_s -> [['Many', '?', 'No', '?', '?']]
 
 	#-------------------------------------------------------
```

### Comparing `hypos-0.0.2/hypos.py` & `hypos-0.0.3/hypos.py`

 * *Files identical despite different names*

### Comparing `hypos-0.0.2/setup.py` & `hypos-0.0.3/setup.py`

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
-00000090: 3d22 302e 302e 3222 2c0d 0a20 2020 2061  ="0.0.2",..    a
+00000090: 3d22 302e 302e 3322 2c0d 0a20 2020 2061  ="0.0.3",..    a
 000000a0: 7574 686f 723d 2270 7261 6264 616c 6970  uthor="prabdalip
 000000b0: 222c 0d0a 2020 2020 6175 7468 6f72 5f65  ",..    author_e
 000000c0: 6d61 696c 3d22 616e 6173 7465 7273 7475  mail="anasterstu
 000000d0: 6469 6f40 676d 6169 6c2e 636f 6d22 2c0d  dio@gmail.com",.
 000000e0: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
 000000f0: 3d22 5072 4142 7059 222c 0d0a 2020 2020  ="PrABpY",..    
 00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

