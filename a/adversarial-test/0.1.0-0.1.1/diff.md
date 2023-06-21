# Comparing `tmp/adversarial-test-0.1.0.tar.gz` & `tmp/adversarial-test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adversarial-test-0.1.0.tar", last modified: Mon Jun 19 03:16:36 2023, max compression
+gzip compressed data, was "adversarial-test-0.1.1.tar", last modified: Wed Jun 21 02:44:28 2023, max compression
```

## Comparing `adversarial-test-0.1.0.tar` & `adversarial-test-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-19 03:16:36.835475 adversarial-test-0.1.0/
--rw-r--r--   0 lap14814   (501) staff       (20)      116 2023-06-19 03:16:36.835346 adversarial-test-0.1.0/PKG-INFO
--rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-18 13:12:08.000000 adversarial-test-0.1.0/README.md
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-19 03:16:36.834334 adversarial-test-0.1.0/adversarial/
--rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-19 03:09:54.000000 adversarial-test-0.1.0/adversarial/__init__.py
--rw-r--r--   0 lap14814   (501) staff       (20)     1976 2023-06-19 03:09:59.000000 adversarial-test-0.1.0/adversarial/adversarial_test.py
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-19 03:16:36.834896 adversarial-test-0.1.0/adversarial_test.egg-info/
--rw-r--r--   0 lap14814   (501) staff       (20)      116 2023-06-19 03:16:36.000000 adversarial-test-0.1.0/adversarial_test.egg-info/PKG-INFO
--rw-r--r--   0 lap14814   (501) staff       (20)      322 2023-06-19 03:16:36.000000 adversarial-test-0.1.0/adversarial_test.egg-info/SOURCES.txt
--rw-r--r--   0 lap14814   (501) staff       (20)        1 2023-06-19 03:16:36.000000 adversarial-test-0.1.0/adversarial_test.egg-info/dependency_links.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       21 2023-06-19 03:16:36.000000 adversarial-test-0.1.0/adversarial_test.egg-info/requires.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       18 2023-06-19 03:16:36.000000 adversarial-test-0.1.0/adversarial_test.egg-info/top_level.txt
--rw-r--r--   0 lap14814   (501) staff       (20)       38 2023-06-19 03:16:36.835512 adversarial-test-0.1.0/setup.cfg
--rw-r--r--   0 lap14814   (501) staff       (20)      374 2023-06-19 03:08:31.000000 adversarial-test-0.1.0/setup.py
-drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-19 03:16:36.835145 adversarial-test-0.1.0/tests/
--rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-19 03:09:38.000000 adversarial-test-0.1.0/tests/__init__.py
--rw-r--r--   0 lap14814   (501) staff       (20)      832 2023-06-19 03:11:24.000000 adversarial-test-0.1.0/tests/test_adversarial_test.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 02:44:28.333989 adversarial-test-0.1.1/
+-rw-r--r--   0 lap14814   (501) staff       (20)      116 2023-06-21 02:44:28.333709 adversarial-test-0.1.1/PKG-INFO
+-rw-r--r--   0 lap14814   (501) staff       (20)      697 2023-06-20 01:13:11.000000 adversarial-test-0.1.1/README.md
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 02:44:28.332172 adversarial-test-0.1.1/adversarial/
+-rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-19 03:09:54.000000 adversarial-test-0.1.1/adversarial/__init__.py
+-rw-r--r--   0 lap14814   (501) staff       (20)     2665 2023-06-20 08:11:15.000000 adversarial-test-0.1.1/adversarial/adversarial_test.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 02:44:28.333068 adversarial-test-0.1.1/adversarial_test.egg-info/
+-rw-r--r--   0 lap14814   (501) staff       (20)      116 2023-06-21 02:44:28.000000 adversarial-test-0.1.1/adversarial_test.egg-info/PKG-INFO
+-rw-r--r--   0 lap14814   (501) staff       (20)      322 2023-06-21 02:44:28.000000 adversarial-test-0.1.1/adversarial_test.egg-info/SOURCES.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)        1 2023-06-21 02:44:28.000000 adversarial-test-0.1.1/adversarial_test.egg-info/dependency_links.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       35 2023-06-21 02:44:28.000000 adversarial-test-0.1.1/adversarial_test.egg-info/requires.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       18 2023-06-21 02:44:28.000000 adversarial-test-0.1.1/adversarial_test.egg-info/top_level.txt
+-rw-r--r--   0 lap14814   (501) staff       (20)       38 2023-06-21 02:44:28.334035 adversarial-test-0.1.1/setup.cfg
+-rw-r--r--   0 lap14814   (501) staff       (20)      380 2023-06-21 02:40:14.000000 adversarial-test-0.1.1/setup.py
+drwxr-xr-x   0 lap14814   (501) staff       (20)        0 2023-06-21 02:44:28.333289 adversarial-test-0.1.1/tests/
+-rw-r--r--   0 lap14814   (501) staff       (20)        0 2023-06-19 03:09:38.000000 adversarial-test-0.1.1/tests/__init__.py
+-rw-r--r--   0 lap14814   (501) staff       (20)     3404 2023-06-20 01:14:48.000000 adversarial-test-0.1.1/tests/test_adversarial_test.py
```

### Comparing `adversarial-test-0.1.0/adversarial/adversarial_test.py` & `adversarial-test-0.1.1/adversarial/adversarial_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import StratifiedGroupKFold, StratifiedKFold
 from sklearn.metrics import roc_auc_score, fbeta_score
+from catboost import CatBoostClassifier
 
-class AdversarialModel():
-    def __init__(
-        self,
-        model
-    ) -> None:
+class AdversarialModel:
+    def __init__(self, model=CatBoostClassifier(iterations=400, verbose=False)) -> None:
         self.model = model
-    
+
     def fit(
         self,
         df1: pd.DataFrame,
         df2: pd.DataFrame,
-        groups=None,
+        groups_col=None,
         features=None,
         cat_features=None,
-        metrics=[(roc_auc_score,), (fbeta_score, {"beta": 0.5})]
+        metrics=[(roc_auc_score,), (fbeta_score, {"beta": 0.5})],
     ):
-        data_adversarial = pd.concat([
-            df1.assign(label=0),
-            df2.assign(label=1),
-        ], ignore_index=True)
-        # print(data_adversarial)
-        # print(data_adversarial["label"].value_counts())
+        data_adversarial = pd.concat(
+            [
+                df1.assign(label=0),
+                df2.assign(label=1),
+            ],
+            ignore_index=True,
+        )
         if features == None:
             features = df1.columns
 
         # stratified_group split 80/20
-        if groups != None:
+        if groups_col != None:
             sgkf = StratifiedGroupKFold(n_splits=5)
+            groups = data_adversarial[groups_col]
         else:
             sgkf = StratifiedKFold(n_splits=5)
-        for fold_ind, (dev_ind, val_ind) in enumerate(sgkf.split(data_adversarial, data_adversarial["label"], groups)):
+            groups = None
+        for fold_ind, (dev_ind, val_ind) in enumerate(
+            sgkf.split(data_adversarial, data_adversarial["label"], groups)
+        ):
             train_idx = dev_ind
             val_idx = val_ind
             break
         # Create train/dev data
         X_train = data_adversarial.iloc[train_idx][features]
         y_train = data_adversarial.iloc[train_idx]["label"]
         X_val = data_adversarial.iloc[val_idx][features]
         y_val = data_adversarial.iloc[val_idx]["label"]
 
         # Train adversarial model
-        self.model.set_params(cat_features = cat_features)
+        self.model.set_params(cat_features=cat_features)
         self.model.fit(X_train, y_train)
-        # for metric, param in metrics:
-        #     print(metric(y_val, self.model.predict(X_val), **param))
         self.auc_score = roc_auc_score(y_val, self.model.predict(X_val))
 
     def get_features_importance(
         self,
     ):
         pass
 
-    def evaluate(self, threshold=0.7):
-        if self.auc_score <= 0.7:
-            return "pass"
+    def evaluate(self, threshold=0.6, metadata=True, n_features=5):
+        if self.auc_score <= threshold:
+            message = f"""Test passed: roc_auc score {self.auc_score:02f}
+            Top {n_features} important feature(s):
+            {self.model.get_feature_importance(prettified=True).head(n_features)}
+            """
+            if metadata:
+                return message
+            else:
+                return "pass"
         else:
-            return "fail"
+            self.get_features_importance
+            message = f"""Test failed: roc_auc score {self.auc_score:02f}
+            Top {n_features} important feature(s):
+            {self.model.get_feature_importance(prettified=True).head(n_features)}
+            """
+            if metadata:
+                return message
+            else:
+                return "fail"
```

