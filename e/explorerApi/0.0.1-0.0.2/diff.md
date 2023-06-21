# Comparing `tmp/explorerApi-0.0.1.tar.gz` & `tmp/explorerApi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explorerApi-0.0.1.tar", last modified: Sat Jun 17 10:17:26 2023, max compression
+gzip compressed data, was "explorerApi-0.0.2.tar", last modified: Wed Jun 21 08:44:55 2023, max compression
```

## Comparing `explorerApi-0.0.1.tar` & `explorerApi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:17:26.391385 explorerApi-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-06-17 08:10:12.000000 explorerApi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      525 2023-06-17 10:17:26.391385 explorerApi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-17 08:09:11.000000 explorerApi-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-17 08:12:46.000000 explorerApi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      666 2023-06-17 10:17:26.393386 explorerApi-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-17 10:17:26.351386 explorerApi-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 10:17:26.366386 explorerApi-0.0.1/src/explorerApi/
--rw-rw-rw-   0        0        0        0 2023-06-17 08:09:56.000000 explorerApi-0.0.1/src/explorerApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:17:26.390386 explorerApi-0.0.1/src/explorerApi.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-17 10:17:26.000000 explorerApi-0.0.1/src/explorerApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-17 10:17:26.000000 explorerApi-0.0.1/src/explorerApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:17:26.000000 explorerApi-0.0.1/src/explorerApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-17 10:17:26.000000 explorerApi-0.0.1/src/explorerApi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 08:44:55.734947 explorerApi-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-06-17 08:10:12.000000 explorerApi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-06-21 08:44:55.735945 explorerApi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-21 08:41:52.000000 explorerApi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 08:44:55.730947 explorerApi-0.0.2/explorerApi.egg-info/
+-rw-rw-rw-   0        0        0      540 2023-06-21 08:44:55.000000 explorerApi-0.0.2/explorerApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-21 08:44:55.000000 explorerApi-0.0.2/explorerApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:44:55.000000 explorerApi-0.0.2/explorerApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-21 08:44:55.000000 explorerApi-0.0.2/explorerApi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 08:44:55.733946 explorerApi-0.0.2/explorers-api/
+-rw-rw-rw-   0        0        0       32 2023-06-21 08:12:54.000000 explorerApi-0.0.2/explorers-api/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-06-21 08:05:31.000000 explorerApi-0.0.2/explorers-api/coin.py
+-rw-rw-rw-   0        0        0      108 2023-06-17 08:12:46.000000 explorerApi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      610 2023-06-21 08:44:55.737945 explorerApi-0.0.2/setup.cfg
```

### Comparing `explorerApi-0.0.1/PKG-INFO` & `explorerApi-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: explorerApi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connect multiple crypto explorers API
 Home-page: https://github.com/pypa/sampleproject
 Author: Sau1707
 Author-email: leonardo.saurwein@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+py -m build
```

### Comparing `explorerApi-0.0.1/setup.cfg` & `explorerApi-0.0.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7870 6c6f 7265 7241 7069 0d0a   = explorerApi..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 310d  version = 0.0.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 320d  version = 0.0.2.
 00000030: 0a61 7574 686f 7220 3d20 5361 7531 3730  .author = Sau170
 00000040: 370d 0a61 7574 686f 725f 656d 6169 6c20  7..author_email 
 00000050: 3d20 6c65 6f6e 6172 646f 2e73 6175 7277  = leonardo.saurw
 00000060: 6569 6e40 676d 6169 6c2e 636f 6d0d 0a64  ein@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2043 6f6e  escription = Con
 00000080: 6e65 6374 206d 756c 7469 706c 6520 6372  nect multiple cr
 00000090: 7970 746f 2065 7870 6c6f 7265 7273 2041  ypto explorers A
@@ -26,17 +26,14 @@
 00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000001a0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
 000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
 000001c0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 000001f0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000200: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000210: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000220: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000230: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000240: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
-00000250: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000260: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000270: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000280: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000290: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000200: 5d0d 0a70 6163 6b61 6765 7320 3d20 6578  ]..packages = ex
+00000210: 706c 6f72 6572 732d 6170 690d 0a70 7974  plorers-api..pyt
+00000220: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000230: 3d33 2e36 0d0a 0d0a 5b65 6767 5f69 6e66  =3.6....[egg_inf
+00000240: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000250: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000260: 0d0a                                     ..
```

### Comparing `explorerApi-0.0.1/src/explorerApi.egg-info/PKG-INFO` & `explorerApi-0.0.2/explorerApi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: explorerApi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connect multiple crypto explorers API
 Home-page: https://github.com/pypa/sampleproject
 Author: Sau1707
 Author-email: leonardo.saurwein@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+py -m build
```

