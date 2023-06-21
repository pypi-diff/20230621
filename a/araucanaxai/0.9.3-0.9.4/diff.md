# Comparing `tmp/araucanaxai-0.9.3.tar.gz` & `tmp/araucanaxai-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "araucanaxai-0.9.3.tar", last modified: Fri Oct 21 13:35:43 2022, max compression
+gzip compressed data, was "E:\Business\Dottorato\Araucana XAI\AraucanaXAI repository\araucanaxai\dist\tmpi8o1xx_0\araucanaxai-0.9.4.tar", last modified: Wed Jun 21 08:19:10 2023, max compression
```

## Comparing `araucanaxai-0.9.3.tar` & `araucanaxai-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-10-21 13:35:43.387520 araucanaxai-0.9.3/
--rw-rw-rw-   0        0        0     1091 2021-10-27 10:49:42.000000 araucanaxai-0.9.3/LICENSE
--rw-rw-rw-   0        0        0       29 2021-10-27 10:51:11.000000 araucanaxai-0.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2000 2022-10-21 13:35:43.388516 araucanaxai-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     1397 2021-11-05 11:51:39.000000 araucanaxai-0.9.3/README.md
--rw-rw-rw-   0        0        0      108 2021-10-27 10:44:52.000000 araucanaxai-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0      858 2022-10-21 13:35:43.408460 araucanaxai-0.9.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-21 13:35:43.215008 araucanaxai-0.9.3/src/
-drwxrwxrwx   0        0        0        0 2022-10-21 13:35:43.335654 araucanaxai-0.9.3/src/araucanaxai/
--rw-rw-rw-   0        0        0       66 2021-11-05 09:52:47.000000 araucanaxai-0.9.3/src/araucanaxai/__init__.py
--rw-rw-rw-   0        0        0      191 2022-06-27 16:43:20.000000 araucanaxai-0.9.3/src/araucanaxai/constants.py
--rw-rw-rw-   0        0        0      414 2021-10-27 13:21:22.000000 araucanaxai-0.9.3/src/araucanaxai/init.py
--rw-rw-rw-   0        0        0    13386 2022-10-14 14:04:27.000000 araucanaxai-0.9.3/src/araucanaxai/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-21 13:35:43.379539 araucanaxai-0.9.3/src/araucanaxai.egg-info/
--rw-rw-rw-   0        0        0     2000 2022-10-21 13:35:42.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2022-10-21 13:35:42.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-21 13:35:42.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-04 12:14:55.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2022-10-21 13:35:42.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-10-21 13:35:42.000000 araucanaxai-0.9.3/src/araucanaxai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/
+-rw-rw-rw-   0        0        0     1091 2021-10-27 10:49:42.000000 araucanaxai-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0       29 2021-10-27 10:51:11.000000 araucanaxai-0.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2041 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-10-27 10:44:52.000000 araucanaxai-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1397 2021-11-05 11:51:39.000000 araucanaxai-0.9.4/README.md
+-rw-rw-rw-   0        0        0      863 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai/
+-rw-rw-rw-   0        0        0      191 2022-06-27 16:43:20.000000 araucanaxai-0.9.4/src/araucanaxai/constants.py
+-rw-rw-rw-   0        0        0      414 2021-10-27 13:21:22.000000 araucanaxai-0.9.4/src/araucanaxai/init.py
+-rw-rw-rw-   0        0        0    13386 2022-10-14 14:04:27.000000 araucanaxai-0.9.4/src/araucanaxai/utils.py
+-rw-rw-rw-   0        0        0       66 2021-11-05 09:52:47.000000 araucanaxai-0.9.4/src/araucanaxai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-04 12:14:55.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2041 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      392 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 08:19:10.000000 araucanaxai-0.9.4/src/araucanaxai.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `araucanaxai-0.9.3/LICENSE` & `araucanaxai-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `araucanaxai-0.9.3/PKG-INFO` & `araucanaxai-0.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: araucanaxai
-Version: 0.9.3
+Version: 0.9.4
 Summary: A novel approach for generating explanations of the predictions of a generic ML model
 Home-page: https://github.com/detsutut/AraucanaXAI
 Author: Tommaso Buonocore
 Author-email: buonocore.tms@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/detsutut/AraucanaXAI/issues
 Keywords: xai,ai
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -24,7 +26,9 @@
 Increasingly complex learning methods such as boosting, bagging and deep learning have made ML models more accurate, but harder to understand and interpret. A tradeoff between performance and intelligibility is often to be faced, especially in high-stakes applications like medicine. This project propose a novel methodological approach for generating explanations of the predictions of a generic ML model, given a specific instance for which the prediction has been made, that can tackle both classification and regression tasks. Advantages of the proposed XAI approach include improved fidelity to the original model, the ability to deal with non-linear decision boundaries, and native support to both classification and regression problems.
 
 **Keywords**: *explainable AI, explanations, local explanation, fidelity, interpretability, transparency, trustworthy AI, black-box, machine learning, feature importance, decision tree, CART, AIM*.
 
 ### Paper
 The araucanaxai package implements the pipeline described in <a href="https://arxiv.org/abs/2110.08272">*Tree-based local explanations of machine learning model predictions - Parimbelli et al., 2021*</a>.
 
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: araucanaxai Version: 0.9.3 Summary: A novel
+Metadata-Version: 2.1 Name: araucanaxai Version: 0.9.4 Summary: A novel
 approach for generating explanations of the predictions of a generic ML model
 Home-page: https://github.com/detsutut/AraucanaXAI Author: Tommaso Buonocore
-Author-email: buonocore.tms@gmail.com Project-URL: Bug Tracker, https://
-github.com/detsutut/AraucanaXAI/issues Keywords: xai,ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Auracana XAI
-Tree-based local explanations of machine learning model predictions.
-Implementation of the pipeline described in Parimbelli_et_al.,_2021 ## About
-The Project Increasingly complex learning methods such as boosting, bagging and
-deep learning have made ML models more accurate, but harder to understand and
-interpret. A tradeoff between performance and intelligibility is often to be
-faced, especially in high-stakes applications like medicine. This project
-propose a novel methodological approach for generating explanations of the
-predictions of a generic ML model, given a specific instance for which the
-prediction has been made, that can tackle both classification and regression
-tasks. Advantages of the proposed XAI approach include improved fidelity to the
-original model, the ability to deal with non-linear decision boundaries, and
-native support to both classification and regression problems. **Keywords**:
-*explainable AI, explanations, local explanation, fidelity, interpretability,
-transparency, trustworthy AI, black-box, machine learning, feature importance,
-decision tree, CART, AIM*. ### Paper The araucanaxai package implements the
-pipeline described in *Tree-based_local_explanations_of_machine_learning_model
-predictions_-_Parimbelli_et_al.,_2021*.
+Author-email: buonocore.tms@gmail.com License: UNKNOWN Project-URL: Bug
+Tracker, https://github.com/detsutut/AraucanaXAI/issues Keywords: xai,ai
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE # Auracana XAI Tree-based local explanations of machine
+learning model predictions. Implementation of the pipeline described in
+Parimbelli_et_al.,_2021 ## About The Project Increasingly complex learning
+methods such as boosting, bagging and deep learning have made ML models more
+accurate, but harder to understand and interpret. A tradeoff between
+performance and intelligibility is often to be faced, especially in high-stakes
+applications like medicine. This project propose a novel methodological
+approach for generating explanations of the predictions of a generic ML model,
+given a specific instance for which the prediction has been made, that can
+tackle both classification and regression tasks. Advantages of the proposed XAI
+approach include improved fidelity to the original model, the ability to deal
+with non-linear decision boundaries, and native support to both classification
+and regression problems. **Keywords**: *explainable AI, explanations, local
+explanation, fidelity, interpretability, transparency, trustworthy AI, black-
+box, machine learning, feature importance, decision tree, CART, AIM*. ### Paper
+The araucanaxai package implements the pipeline described in *Tree-based_local
+explanations_of_machine_learning_model_predictions_-_Parimbelli_et_al.,_2021*.
```

### Comparing `araucanaxai-0.9.3/README.md` & `araucanaxai-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `araucanaxai-0.9.3/setup.cfg` & `araucanaxai-0.9.4/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7261 7563 616e 6178 6169 0d0a   = araucanaxai..
-00000020: 7665 7273 696f 6e20 3d20 302e 392e 330d  version = 0.9.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 392e 340d  version = 0.9.4.
 00000030: 0a61 7574 686f 7220 3d20 546f 6d6d 6173  .author = Tommas
 00000040: 6f20 4275 6f6e 6f63 6f72 650d 0a61 7574  o Buonocore..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6275 6f6e  hor_email = buon
 00000060: 6f63 6f72 652e 746d 7340 676d 6169 6c2e  ocore.tms@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 206e 6f76 656c 2061 7070 726f   = A novel appro
 00000090: 6163 6820 666f 7220 6765 6e65 7261 7469  ach for generati
@@ -38,17 +38,17 @@
 00000250: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 00000260: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
 00000270: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 00000280: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
 00000290: 2e36 0d0a 696e 7374 616c 6c5f 7265 7175  .6..install_requ
 000002a0: 6972 6573 203d 200d 0a09 676f 7765 720d  ires = ...gower.
 000002b0: 0a09 7061 6e64 6173 0d0a 096e 756d 7079  ..pandas...numpy
-000002c0: 0d0a 0973 6b6c 6561 726e 0d0a 0969 6d62  ...sklearn...imb
-000002d0: 6c65 6172 6e0d 0a69 6e63 6c75 6465 5f70  learn..include_p
-000002e0: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-000002f0: 7565 0d0a 7a69 705f 7361 6665 203d 2046  ue..zip_safe = F
-00000300: 616c 7365 0d0a 0d0a 5b6f 7074 696f 6e73  alse....[options
-00000310: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000320: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000330: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000340: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000350: 7465 203d 2030 0d0a 0d0a                 te = 0....
+000002c0: 0d0a 0973 6369 6b69 742d 6c65 6172 6e0d  ...scikit-learn.
+000002d0: 0a09 696d 626c 6561 726e 0d0a 696e 636c  ..imblearn..incl
+000002e0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000002f0: 203d 2054 7275 650d 0a7a 6970 5f73 6166   = True..zip_saf
+00000300: 6520 3d20 4661 6c73 650d 0a0d 0a5b 6f70  e = False....[op
+00000310: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000320: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000330: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
+00000340: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000350: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `araucanaxai-0.9.3/src/araucanaxai/utils.py` & `araucanaxai-0.9.4/src/araucanaxai/utils.py`

 * *Files identical despite different names*

### Comparing `araucanaxai-0.9.3/src/araucanaxai.egg-info/PKG-INFO` & `araucanaxai-0.9.4/src/araucanaxai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: araucanaxai
-Version: 0.9.3
+Version: 0.9.4
 Summary: A novel approach for generating explanations of the predictions of a generic ML model
 Home-page: https://github.com/detsutut/AraucanaXAI
 Author: Tommaso Buonocore
 Author-email: buonocore.tms@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/detsutut/AraucanaXAI/issues
 Keywords: xai,ai
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -24,7 +26,9 @@
 Increasingly complex learning methods such as boosting, bagging and deep learning have made ML models more accurate, but harder to understand and interpret. A tradeoff between performance and intelligibility is often to be faced, especially in high-stakes applications like medicine. This project propose a novel methodological approach for generating explanations of the predictions of a generic ML model, given a specific instance for which the prediction has been made, that can tackle both classification and regression tasks. Advantages of the proposed XAI approach include improved fidelity to the original model, the ability to deal with non-linear decision boundaries, and native support to both classification and regression problems.
 
 **Keywords**: *explainable AI, explanations, local explanation, fidelity, interpretability, transparency, trustworthy AI, black-box, machine learning, feature importance, decision tree, CART, AIM*.
 
 ### Paper
 The araucanaxai package implements the pipeline described in <a href="https://arxiv.org/abs/2110.08272">*Tree-based local explanations of machine learning model predictions - Parimbelli et al., 2021*</a>.
 
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: araucanaxai Version: 0.9.3 Summary: A novel
+Metadata-Version: 2.1 Name: araucanaxai Version: 0.9.4 Summary: A novel
 approach for generating explanations of the predictions of a generic ML model
 Home-page: https://github.com/detsutut/AraucanaXAI Author: Tommaso Buonocore
-Author-email: buonocore.tms@gmail.com Project-URL: Bug Tracker, https://
-github.com/detsutut/AraucanaXAI/issues Keywords: xai,ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Auracana XAI
-Tree-based local explanations of machine learning model predictions.
-Implementation of the pipeline described in Parimbelli_et_al.,_2021 ## About
-The Project Increasingly complex learning methods such as boosting, bagging and
-deep learning have made ML models more accurate, but harder to understand and
-interpret. A tradeoff between performance and intelligibility is often to be
-faced, especially in high-stakes applications like medicine. This project
-propose a novel methodological approach for generating explanations of the
-predictions of a generic ML model, given a specific instance for which the
-prediction has been made, that can tackle both classification and regression
-tasks. Advantages of the proposed XAI approach include improved fidelity to the
-original model, the ability to deal with non-linear decision boundaries, and
-native support to both classification and regression problems. **Keywords**:
-*explainable AI, explanations, local explanation, fidelity, interpretability,
-transparency, trustworthy AI, black-box, machine learning, feature importance,
-decision tree, CART, AIM*. ### Paper The araucanaxai package implements the
-pipeline described in *Tree-based_local_explanations_of_machine_learning_model
-predictions_-_Parimbelli_et_al.,_2021*.
+Author-email: buonocore.tms@gmail.com License: UNKNOWN Project-URL: Bug
+Tracker, https://github.com/detsutut/AraucanaXAI/issues Keywords: xai,ai
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE # Auracana XAI Tree-based local explanations of machine
+learning model predictions. Implementation of the pipeline described in
+Parimbelli_et_al.,_2021 ## About The Project Increasingly complex learning
+methods such as boosting, bagging and deep learning have made ML models more
+accurate, but harder to understand and interpret. A tradeoff between
+performance and intelligibility is often to be faced, especially in high-stakes
+applications like medicine. This project propose a novel methodological
+approach for generating explanations of the predictions of a generic ML model,
+given a specific instance for which the prediction has been made, that can
+tackle both classification and regression tasks. Advantages of the proposed XAI
+approach include improved fidelity to the original model, the ability to deal
+with non-linear decision boundaries, and native support to both classification
+and regression problems. **Keywords**: *explainable AI, explanations, local
+explanation, fidelity, interpretability, transparency, trustworthy AI, black-
+box, machine learning, feature importance, decision tree, CART, AIM*. ### Paper
+The araucanaxai package implements the pipeline described in *Tree-based_local
+explanations_of_machine_learning_model_predictions_-_Parimbelli_et_al.,_2021*.
```

