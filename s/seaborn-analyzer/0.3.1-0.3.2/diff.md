# Comparing `tmp/seaborn-analyzer-0.3.1.tar.gz` & `tmp/seaborn-analyzer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.3.1.tar", last modified: Tue Jun 20 06:28:48 2023, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.2.tar", last modified: Wed Jun 21 06:34:36 2023, max compression
```

## Comparing `seaborn-analyzer-0.3.1.tar` & `seaborn-analyzer-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.334785 seaborn-analyzer-0.3.1/
--rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.1/LICENSE
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-20 06:28:48.334570 seaborn-analyzer-0.3.1/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-20 06:27:32.000000 seaborn-analyzer-0.3.1/README.rst
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.333405 seaborn-analyzer-0.3.1/seaborn_analyzer/
--rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-20 06:27:22.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/__init__.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53800 2023-06-20 05:32:06.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set_sklearn.py
--rw-r--r--   0 knakamura   (501) staff       (20)    82441 2023-06-19 07:44:36.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_hist_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_pair_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    97795 2022-04-23 10:03:42.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_reg_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     1635 2023-06-19 07:33:38.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/multiclass_fitparams.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.334360 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)      518 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/requires.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/top_level.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-20 06:28:48.334826 seaborn-analyzer-0.3.1/setup.cfg
--rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.1/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.784345 seaborn-analyzer-0.3.2/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.2/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-21 06:34:36.783991 seaborn-analyzer-0.3.2/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-21 06:25:30.000000 seaborn-analyzer-0.3.2/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.782839 seaborn-analyzer-0.3.2/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-21 06:25:22.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53230 2023-06-21 06:06:04.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set_old.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    82445 2023-06-21 06:21:22.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    97799 2023-06-21 06:18:38.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.783408 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      531 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-21 06:34:36.784394 seaborn-analyzer-0.3.2/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.2/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.783545 seaborn-analyzer-0.3.2/tests/
+-rw-r--r--   0 knakamura   (501) staff       (20)     3356 2023-06-21 06:33:42.000000 seaborn-analyzer-0.3.2/tests/test_cv.py
```

### Comparing `seaborn-analyzer-0.3.1/LICENSE` & `seaborn-analyzer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.1/PKG-INFO` & `seaborn-analyzer-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.1
+Version: 0.3.2
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.1 requires
+seaborn-analyzer 0.3.2 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.1/README.rst` & `seaborn-analyzer-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.1 requires
+seaborn-analyzer 0.3.2 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set_old.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set_sklearn.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,88 +2,78 @@
 import numpy as np
 import time
 import numbers
 from itertools import product
 from collections import defaultdict
 from sklearn import clone
 from sklearn.pipeline import Pipeline
-from sklearn.model_selection import check_cv, GridSearchCV, RandomizedSearchCV
+from sklearn.model_selection import check_cv, GridSearchCV, RandomizedSearchCV, train_test_split
 from sklearn.model_selection._validation import _fit_and_score, _insert_error_scores, _aggregate_score_dicts, _normalize_score_results, _translate_train_sizes, _incremental_fit_estimator
 from sklearn.utils.validation import indexable, check_random_state, _check_fit_params
 from sklearn.metrics import check_scoring
 from sklearn.metrics._scorer import _check_multimetric_scoring
 from sklearn.base import is_classifier
 from sklearn.utils.parallel import delayed, Parallel
 
-def init_eval_set(src_eval_set_selection, src_fit_params, X, y):
-        """
-        fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理
-        
-        Parameters
-        ----------
-        src_eval_set_selection : {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            eval_setに渡すデータの決め方 ('all': X, 'test': X[test], 'train': X[train], 'original': 入力そのまま, 'original_transformed': 入力そのまま＆パイプラインの時は最終学習器以外の変換実行)
-
-        src_fit_params : Dict
-            処理前の学習時パラメータ
-        """
-
-        fit_params = copy.deepcopy(src_fit_params)
-        eval_set_selection = src_eval_set_selection
-        # fit_paramsにeval_metricが設定されているときのみ以下の処理を実施
-        if 'eval_metric' in src_fit_params and src_fit_params['eval_metric'] is not None:
-            # fit_paramsにeval_setが存在しないとき、入力データをそのまま追加
-            if 'eval_set' not in src_fit_params:
-                print('There is no "eval_set" in fit_params, so "eval_set" is set to (self.X, self.y)')
-                fit_params['eval_set'] = [(X, y)]
-                if src_eval_set_selection is None:  # eval_set_selection未指定時、eval_setが入力されていなければeval_set_selection='test'とする
-                    eval_set_selection = 'test'
-                if eval_set_selection not in ['all', 'train', 'test']:  # eval_set_selectionの指定が間違っていたらエラーを出す
-                    raise ValueError('The `eval_set_selection` argument should be "all", "train", or "test" when `eval_set` is not in `fit_params`')
-            # src_fit_paramsにeval_setが存在するとき、eval_set_selection未指定ならばeval_set_selection='original_transformed'とする
-            else:
-                if src_eval_set_selection is None:
-                    eval_set_selection = 'original_transformed'
-
-        return fit_params, eval_set_selection
-
 def _transform_except_last_estimator(transformer, X_src, X_train):
     """パイプラインのとき、最終学習器以外のtransformを適用"""
     if transformer is not None:
         transformer.fit(X_train)
         X_dst = transformer.transform(X_src)
         return X_dst
     else:
         return X_src
 
-def _eval_set_selection(eval_set_selection, transformer, X, y,
-                        fit_params, train, test):
+def _eval_set_selection(validation_fraction, 
+                        transformer, 
+                        X, 
+                        y,
+                        fit_params, 
+                        train, 
+                        test, 
+                        random_state,
+                        stratify
+                        ):
     """eval_setの中から学習データ or テストデータのみを抽出"""
     fit_params_modified = copy.deepcopy(fit_params)
     # eval_setが存在しない or Noneなら、そのままfit_paramsを返す
     eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
     if len(eval_sets) == 0 or fit_params[eval_sets[0]] is None:
         return fit_params_modified
     # eval_setの列名(pipelineでは列名が変わるため)
     eval_set_name = eval_sets[0]
     # 元のeval_setからX, yを取得
     X_fit = fit_params[eval_set_name][0][0]
     y_fit = fit_params[eval_set_name][0][1]
-    # eval_setにテストデータを使用する場合
-    if eval_set_selection == 'test':
+    # Training dataの一部をeval_setとして使用する場合
+    if isinstance(validation_fraction, float):
+        # Select training data from source training data
+        rng = np.random.default_rng(seed=random_state)
+        size = int(train.shape[0]*validation_fraction)
+        train_divided = rng.choice(train, size=size, replace=False)
+        train_divided.sort()
+        # Select validation data from difference set of the selected training data and the source training data
+        val_divided = np.setdiff1d(train, train_divided)
+        fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X[val_divided], X[train_divided])\
+                                              , y[val_divided])]
+    # Cross validationのテストデータをeval_setとして使用する場合
+    elif validation_fraction == 'cv':
         fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X[test], X[train])\
                                               , y[test])]
-    # eval_setをそのまま使用する場合
+        train_divided = train
+    # eval_setをそのまま使用、またはPipelineのみ適用して使用する場合
     else:
         fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X_fit, X[train])\
                                               , y_fit)]
-    return fit_params_modified
+        train_divided = train
+
+    return fit_params_modified, train_divided
 
 def _fit_and_score_eval_set(
-    eval_set_selection,
+    validation_fraction,
     transformer,
     estimator,
     X, 
     y, 
     scorer,
     train,
     test,
@@ -95,42 +85,52 @@
     return_n_test_samples=False,
     return_times=False,
     return_estimator=False,
     split_progress=None,
     candidate_progress=None,
     error_score=np.nan,
     ):
-
     """Fit estimator and compute scores for a given dataset split."""
-    # eval_setの中から必要データのみを抽出
-    fit_params_modified = _eval_set_selection(eval_set_selection, transformer, X, y,
-                                              fit_params, train, test)
+    
+    # fit_params内のデータをvalidation_fractionに合わせて整形 (validation_fraction='')
+    stratify = y if is_classifier(estimator) else None
+    fit_params_modified, train_divided = _eval_set_selection(
+        validation_fraction, 
+        transformer, 
+        X, 
+        y,
+        fit_params, 
+        train, 
+        test,
+        estimator.random_state,
+        stratify
+        )
 
     # 学習してスコア計算
-    result = _fit_and_score(estimator, X, y, scorer, train, test, verbose, parameters,
+    result = _fit_and_score(estimator, X, y, scorer, train_divided, test, verbose, parameters,
                             fit_params_modified,
                             return_train_score=return_train_score,
                             return_parameters=return_parameters, return_n_test_samples=return_n_test_samples,
                             return_times=return_times, return_estimator=return_estimator,
                             split_progress=split_progress, candidate_progress=candidate_progress,
                             error_score=error_score)
     return result
 
-def _make_transformer(eval_set_selection, estimator):
+def _make_transformer(validation_fraction, estimator):
     """estimatorがパイプラインのとき、最終学習器以外の変換器(前処理クラスのリスト)を作成"""
-    if isinstance(estimator, Pipeline) and eval_set_selection is not None:
+    if isinstance(estimator, Pipeline) and validation_fraction is not None:
         transformer = Pipeline([step for i, step in enumerate(estimator.steps) if i < len(estimator) - 1])
         return transformer
     else:
         return None
 
 def cross_validate_eval_set(estimator,
     X,
     y=None,
-    eval_set_selection='test',
+    validation_fraction='cv',
     *,
     groups=None,
     scoring=None,
     cv=None,
     n_jobs=None,
     verbose=0,
     fit_params=None,
@@ -152,18 +152,20 @@
     X : array-like of shape (n_samples, n_features)
         The data to fit. Can be for example a list, or an array.
 
     y : array-like of shape (n_samples,) or (n_samples, n_outputs), default=None
         The target variable to try to predict in the case of
         supervised learning.
 
-    eval_set_selection : {'test', 'transformed', or None}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "test", select test data from `X` and `y` using cv.split().
+    validation_fraction : {float, 'cv', 'transformed', or None}
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+        If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+        
+        If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
         If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
         If None, use raw `eval_set`.
 
     groups : array-like of shape (n_samples,), default=None
         Group labels for the samples used while splitting the dataset into
@@ -304,23 +306,23 @@
         scorers = scoring
     elif scoring is None or isinstance(scoring, str):
         scorers = check_scoring(estimator, scoring)
     else:
         scorers = _check_multimetric_scoring(estimator, scoring)
 
     # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
+    transformer = _make_transformer(validation_fraction, estimator)
 
     # We clone the estimator to make sure that all the folds are
     # independent, and that it is pickle-able.
     parallel = Parallel(n_jobs=n_jobs, verbose=verbose,
                         pre_dispatch=pre_dispatch)
     results = parallel(
         delayed(_fit_and_score_eval_set)(
-            eval_set_selection, transformer,
+            validation_fraction, transformer,
             clone(estimator), X, y, scorers, train, test, verbose, None,
             fit_params, return_train_score=return_train_score,
             return_times=True, return_estimator=return_estimator,
             error_score=error_score)
         for train, test in cv.split(X, y, groups))
 
     # For callabe scoring, the return type is only know after calling. If the
@@ -350,15 +352,15 @@
 
     return ret
 
 def cross_val_score_eval_set(
     estimator,
     X,
     y=None,
-    eval_set_selection='test',
+    validation_fraction='cv',
     *,
     groups=None,
     scoring=None,
     cv=None,
     n_jobs=None,
     verbose=0,
     fit_params=None,
@@ -379,18 +381,20 @@
         The data to fit. Can be for example a list, or an array.
 
     y : array-like of shape (n_samples,) or (n_samples, n_outputs), \
             default=None
         The target variable to try to predict in the case of
         supervised learning.
     
-    eval_set_selection : {'test', 'transformed', or None}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "test", select test data from `X` and `y` using cv.split().
+    validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+        If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+        
+        If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
         If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
         If None, use raw `eval_set`.
 
     groups : array-like of shape (n_samples,), default=None
         Group labels for the samples used while splitting the dataset into
@@ -469,59 +473,46 @@
     -------
     scores : ndarray of float of shape=(len(list(cv)),)
         Array of scores of the estimator for each run of the cross validation.
     """
     # To ensure multimetric format is not supported
     scorer = check_scoring(estimator, scoring=scoring)
 
-    cv_results = cross_validate_eval_set(estimator=estimator, X=X, y=y, eval_set_selection=eval_set_selection,
+    cv_results = cross_validate_eval_set(estimator=estimator, X=X, y=y, validation_fraction=validation_fraction,
                                          groups=groups,
                                          scoring={'score': scorer}, cv=cv,
                                          n_jobs=n_jobs, verbose=verbose,
                                          fit_params=fit_params,
                                          pre_dispatch=pre_dispatch,
                                          error_score=error_score)
     return cv_results['test_score']
 
 def validation_curve_eval_set(
-    eval_set_selection,
     estimator,
     X, 
     y,
     *,
     param_name, 
     param_range, 
+    validation_fraction='cv',
     groups=None,
     cv=None, 
     scoring=None, 
     n_jobs=None, 
     pre_dispatch="all",
     verbose=0, 
     error_score=np.nan, 
     fit_params=None
 ):
     """Validation curve.
 
     Determine training and test scores for varying parameter values with `eval_set` argument in `fit_params`
 
     Parameters
-    ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-    
+    ----------    
     estimator : object type that implements the "fit" and "predict" methods
         An object of that type which is cloned for each validation.
 
     X : array-like of shape (n_samples, n_features)
         Training vector, where n_samples is the number of samples and
         n_features is the number of features.
 
@@ -531,14 +522,25 @@
 
     param_name : str
         Name of the parameter that will be varied.
 
     param_range : array-like of shape (n_values,)
         The values of the parameter that will be evaluated.
 
+    validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+        If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+        
+        If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
+
+        If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
+
+        If None, use raw `eval_set`.
+
     groups : array-like of shape (n_samples,), default=None
         Group labels for the samples used while splitting the dataset into
         train/test set. Only used in conjunction with a "Group" :term:`cv`
         instance (e.g., :class:`GroupKFold`).
 
     cv : int, cross-validation generator or an iterable, default=None
         Determines the cross-validation splitting strategy.
@@ -603,20 +605,20 @@
     """
     X, y, groups = indexable(X, y, groups)
 
     cv = check_cv(cv, y, classifier=is_classifier(estimator))
     scorer = check_scoring(estimator, scoring=scoring)
 
     # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
+    transformer = _make_transformer(validation_fraction, estimator)
 
     parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch, verbose=verbose)
     results = parallel(
         delayed(_fit_and_score_eval_set)(
-            eval_set_selection,
+            validation_fraction,
             transformer,
             clone(estimator), 
             X, 
             y, 
             scorer, 
             train, 
             test, 
@@ -635,19 +637,19 @@
     results = _aggregate_score_dicts(results)
     train_scores = results["train_scores"].reshape(-1, n_params).T
     test_scores = results["test_scores"].reshape(-1, n_params).T
 
     return train_scores, test_scores
 
 def learning_curve_eval_set(
-    eval_set_selection,
     estimator,
     X, 
     y,
     *,
+    validation_fraction='cv',
     groups=None,
     train_sizes=np.linspace(0.1, 1.0, 5), 
     cv=None,
     scoring=None, 
     exploit_incremental_learning=False,
     n_jobs=None, 
     pre_dispatch="all",
@@ -660,38 +662,36 @@
 ):
     """Learning curve.
 
     Determines cross-validated training and test scores for different training set sizes with `eval_set` argument in `fit_params`
 
     Parameters
     ----------
-    eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-        If "all", use all data in `X` and `y`.
-
-        If "train", select train data from `X` and `y` using cv.split().
-
-        If "test", select test data from `X` and `y` using cv.split().
-
-        If "original", use raw `eval_set`.
-
-        If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
-    
     estimator : object type that implements the "fit" and "predict" methods
         An object of that type which is cloned for each validation.
 
     X : array-like of shape (n_samples, n_features)
         Training vector, where n_samples is the number of samples and
         n_features is the number of features.
 
     y : array-like of shape (n_samples,) or (n_samples, n_outputs)
         Target relative to X for classification or regression;
         None for unsupervised learning.
 
+    validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+        Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+        If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+        
+        If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
+
+        If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
+
+        If None, use raw `eval_set`.
+
     groups : array-like of  shape (n_samples,), default=None
         Group labels for the samples used while splitting the dataset into
         train/test set. Only used in conjunction with a "Group" :term:`cv`
         instance (e.g., :class:`GroupKFold`).
 
     train_sizes : array-like of shape (n_ticks,), \
             default=np.linspace(0.1, 1.0, 5)
@@ -809,15 +809,15 @@
     # use the first 'n_max_training_samples' samples.
     train_sizes_abs = _translate_train_sizes(train_sizes, n_max_training_samples)
     n_unique_ticks = train_sizes_abs.shape[0]
     if verbose > 0:
         print("[learning_curve] Training set sizes: " + str(train_sizes_abs))
 
     # 最終学習器以外の前処理変換器作成
-    transformer = _make_transformer(eval_set_selection, estimator)
+    transformer = _make_transformer(validation_fraction, estimator)
 
     parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch, verbose=verbose)
 
     if shuffle:
         rng = check_random_state(random_state)
         cv_iter = ((rng.permutation(train), test) for train, test in cv_iter)
 
@@ -845,15 +845,15 @@
         train_test_proportions = []
         for train, test in cv_iter:
             for n_train_samples in train_sizes_abs:
                 train_test_proportions.append((train[:n_train_samples], test))
 
         results = parallel(
             delayed(_fit_and_score_eval_set)(
-                eval_set_selection, 
+                validation_fraction, 
                 transformer,
                 clone(estimator), 
                 X, 
                 y, 
                 scorer, 
                 train, 
                 test, 
@@ -883,49 +883,62 @@
 
     return ret
 
 class GridSearchCVEvalSet(GridSearchCV):
     """
     Exhaustive search over specified parameter values for an estimator with `eval_set` argument in `fit_params`.
     """
-    def fit(self, eval_set_selection,
-            X, y=None, groups=None, **fit_params):
+    def fit(self,
+            X, 
+            y=None, 
+            groups=None,
+            validation_fraction='cv',
+            **fit_params):
         """Run fit with all sets of parameters.
 
         Parameters
         ----------
-        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-                
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
 
         X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
+            Training vector, where `n_samples` is the number of samples and
+            `n_features` is the number of features.
 
         y : array-like of shape (n_samples, n_output) \
             or (n_samples,), default=None
             Target relative to X for classification or regression;
             None for unsupervised learning.
 
         groups : array-like of shape (n_samples,), default=None
             Group labels for the samples used while splitting the dataset into
             train/test set. Only used in conjunction with a "Group" :term:`cv`
             instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
 
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
+
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
+
+            If None, use raw `eval_set`.
+
         **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
+            Parameters passed to the `fit` method of the estimator.
+
+            If a fit parameter is an array-like whose length is equal to
+            `num_samples` then it will be split across CV groups along with `X`
+            and `y`. For example, the :term:`sample_weight` parameter is split
+            because `len(sample_weights) = len(X)`.
+
+        Returns
+        -------
+        self : object
+            Instance of fitted estimator.
         """
         estimator = self.estimator
         refit_metric = "score"
 
         if callable(self.scoring):
             scorers = self.scoring
         elif self.scoring is None or isinstance(self.scoring, str):
@@ -940,90 +953,97 @@
 
         cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
         n_splits = cv_orig.get_n_splits(X, y, groups)
 
         base_estimator = clone(self.estimator)
 
         # 最終学習器以外の前処理変換器作成
-        transformer = _make_transformer(eval_set_selection, estimator)
+        transformer = _make_transformer(validation_fraction, estimator)
 
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
+        parallel = Parallel(n_jobs=self.n_jobs, pre_dispatch=self.pre_dispatch)
 
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
+        fit_and_score_kwargs = dict(
+            scorer=scorers,
+            fit_params=fit_params,
+            return_train_score=self.return_train_score,
+            return_n_test_samples=True,
+            return_times=True,
+            return_parameters=False,
+            error_score=self.error_score,
+            verbose=self.verbose,
+        )
         results = {}
         with parallel:
             all_candidate_params = []
             all_out = []
             all_more_results = defaultdict(list)
 
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
+            def evaluate_candidates(candidate_params, cv=None, more_results=None):
                 cv = cv or cv_orig
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
+                    print(
+                        "Fitting {0} folds for each of {1} candidates,"
                           " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
+                              n_splits, n_candidates, n_candidates * n_splits
+                        )
+                    )
+
+                out = parallel(
+                    delayed(_fit_and_score_eval_set)(
+                        validation_fraction, 
+                        transformer,
+                        clone(base_estimator),
+                        X, 
+                        y,
+                        train=train, 
+                        test=test,
+                        parameters=parameters,
+                        split_progress=(split_idx, n_splits),
+                        candidate_progress=(cand_idx, n_candidates),
+                        **fit_and_score_kwargs,
+                    )
+                    for (cand_idx, parameters), (split_idx, (train, test)) in product(
+                        enumerate(candidate_params),enumerate(cv.split(X, y, groups))
+                    )
+                )
 
                 if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
+                    raise ValueError(
+                        "No fits were performed. "
+                        "Was the CV iterator empty? "
+                        "Were there no candidates?"
+                    )
                 elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
+                    raise ValueError(
+                        "cv.split and cv.get_n_splits returned "
+                        "inconsistent results. Expected {} "
+                        "splits, got {}".format(n_splits, len(out) // n_candidates)
+                    )
 
                 # For callable self.scoring, the return type is only know after
                 # calling. If the return type is a dictionary, the error scores
                 # can now be inserted with the correct key. The type checking
                 # of out will be done in `_insert_error_scores`.
                 if callable(self.scoring):
                     _insert_error_scores(out, self.error_score)
+
                 all_candidate_params.extend(candidate_params)
                 all_out.extend(out)
+
                 if more_results is not None:
                     for key, value in more_results.items():
                         all_more_results[key].extend(value)
 
                 nonlocal results
                 results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
+                    all_candidate_params, n_splits, all_out, all_more_results
+                )
 
                 return results
 
             self._run_search(evaluate_candidates)
 
             # multimetric is determined here because in the case of a callable
             # self.scoring the return type is only known after calling
@@ -1035,90 +1055,102 @@
                 self._check_refit_for_multimetric(first_test_score)
                 refit_metric = self.refit
 
         # For multi-metric evaluation, store the best_index_, best_params_ and
         # best_score_ iff refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
         if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
+            self.best_index_ = self._select_best_index(
+                self.refit, refit_metric, results
+            )
+            if not callable(self.refit):
+                # With a non-custom callable, we can select the best score
+                # based on the best index
+                self.best_score_ = results[f"mean_test_{refit_metric}"][
+                    self.best_index_
+                ]
             self.best_params_ = results["params"][self.best_index_]
 
         if self.refit:
             # we clone again after setting params in case some
             # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
+            self.best_estimator_ = clone(
+                clone(base_estimator).set_params(**self.best_params_)
+            )
             refit_start_time = time.time()
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
             else:
                 self.best_estimator_.fit(X, **fit_params)
             refit_end_time = time.time()
             self.refit_time_ = refit_end_time - refit_start_time
 
+            if hasattr(self.best_estimator_, "feature_names_in_"):
+                self.feature_names_in_ = self.best_estimator_.feature_names_in_
+
         # Store the only scorer not as a dict for single metric evaluation
         self.scorer_ = scorers
 
         self.cv_results_ = results
         self.n_splits_ = n_splits
 
         return self
 
 class RandomizedSearchCVEvalSet(RandomizedSearchCV):
     """
     Randomized search on hyper parameters with `eval_set` argument in `fit_params`.
     """
-    def fit(self, eval_set_selection,
-            X, y=None, groups=None, **fit_params):
+    def fit(self,
+            X, 
+            y=None, 
+            groups=None,
+            validation_fraction='cv',
+            **fit_params):
         """Run fit with all sets of parameters.
 
         Parameters
         ----------
-        eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-                
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
-
-            If "original", use raw `eval_set`.
-
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
 
         X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
+            Training vector, where `n_samples` is the number of samples and
+            `n_features` is the number of features.
 
         y : array-like of shape (n_samples, n_output) \
             or (n_samples,), default=None
             Target relative to X for classification or regression;
             None for unsupervised learning.
 
         groups : array-like of shape (n_samples,), default=None
             Group labels for the samples used while splitting the dataset into
             train/test set. Only used in conjunction with a "Group" :term:`cv`
             instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
 
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
+
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
+
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
+
+            If None, use raw `eval_set`.
+
         **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
+            Parameters passed to the `fit` method of the estimator.
+
+            If a fit parameter is an array-like whose length is equal to
+            `num_samples` then it will be split across CV groups along with `X`
+            and `y`. For example, the :term:`sample_weight` parameter is split
+            because `len(sample_weights) = len(X)`.
+
+        Returns
+        -------
+        self : object
+            Instance of fitted estimator.
         """
         estimator = self.estimator
         refit_metric = "score"
 
         if callable(self.scoring):
             scorers = self.scoring
         elif self.scoring is None or isinstance(self.scoring, str):
@@ -1133,90 +1165,97 @@
 
         cv_orig = check_cv(self.cv, y, classifier=is_classifier(estimator))
         n_splits = cv_orig.get_n_splits(X, y, groups)
 
         base_estimator = clone(self.estimator)
 
         # 最終学習器以外の前処理変換器作成
-        transformer = _make_transformer(eval_set_selection, estimator)
+        transformer = _make_transformer(validation_fraction, estimator)
 
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
+        parallel = Parallel(n_jobs=self.n_jobs, pre_dispatch=self.pre_dispatch)
 
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
+        fit_and_score_kwargs = dict(
+            scorer=scorers,
+            fit_params=fit_params,
+            return_train_score=self.return_train_score,
+            return_n_test_samples=True,
+            return_times=True,
+            return_parameters=False,
+            error_score=self.error_score,
+            verbose=self.verbose,
+        )
         results = {}
         with parallel:
             all_candidate_params = []
             all_out = []
             all_more_results = defaultdict(list)
 
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
+            def evaluate_candidates(candidate_params, cv=None, more_results=None):
                 cv = cv or cv_orig
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
+                    print(
+                        "Fitting {0} folds for each of {1} candidates,"
                           " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
+                              n_splits, n_candidates, n_candidates * n_splits
+                        )
+                    )
+
+                out = parallel(
+                    delayed(_fit_and_score_eval_set)(
+                        validation_fraction, 
+                        transformer,
+                        clone(base_estimator),
+                        X, 
+                        y,
+                        train=train, 
+                        test=test,
+                        parameters=parameters,
+                        split_progress=(split_idx, n_splits),
+                        candidate_progress=(cand_idx, n_candidates),
+                        **fit_and_score_kwargs,
+                    )
+                    for (cand_idx, parameters), (split_idx, (train, test)) in product(
+                        enumerate(candidate_params),enumerate(cv.split(X, y, groups))
+                    )
+                )
 
                 if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
+                    raise ValueError(
+                        "No fits were performed. "
+                        "Was the CV iterator empty? "
+                        "Were there no candidates?"
+                    )
                 elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
+                    raise ValueError(
+                        "cv.split and cv.get_n_splits returned "
+                        "inconsistent results. Expected {} "
+                        "splits, got {}".format(n_splits, len(out) // n_candidates)
+                    )
 
                 # For callable self.scoring, the return type is only know after
                 # calling. If the return type is a dictionary, the error scores
                 # can now be inserted with the correct key. The type checking
                 # of out will be done in `_insert_error_scores`.
                 if callable(self.scoring):
                     _insert_error_scores(out, self.error_score)
+
                 all_candidate_params.extend(candidate_params)
                 all_out.extend(out)
+
                 if more_results is not None:
                     for key, value in more_results.items():
                         all_more_results[key].extend(value)
 
                 nonlocal results
                 results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
+                    all_candidate_params, n_splits, all_out, all_more_results
+                )
 
                 return results
 
             self._run_search(evaluate_candidates)
 
             # multimetric is determined here because in the case of a callable
             # self.scoring the return type is only known after calling
@@ -1228,43 +1267,42 @@
                 self._check_refit_for_multimetric(first_test_score)
                 refit_metric = self.refit
 
         # For multi-metric evaluation, store the best_index_, best_params_ and
         # best_score_ iff refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
         if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
+            self.best_index_ = self._select_best_index(
+                self.refit, refit_metric, results
+            )
+            if not callable(self.refit):
+                # With a non-custom callable, we can select the best score
+                # based on the best index
+                self.best_score_ = results[f"mean_test_{refit_metric}"][
+                    self.best_index_
+                ]
             self.best_params_ = results["params"][self.best_index_]
 
         if self.refit:
             # we clone again after setting params in case some
             # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
+            self.best_estimator_ = clone(
+                clone(base_estimator).set_params(**self.best_params_)
+            )
             refit_start_time = time.time()
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
             else:
                 self.best_estimator_.fit(X, **fit_params)
             refit_end_time = time.time()
             self.refit_time_ = refit_end_time - refit_start_time
 
+            if hasattr(self.best_estimator_, "feature_names_in_"):
+                self.feature_names_in_ = self.best_estimator_.feature_names_in_
+
         # Store the only scorer not as a dict for single metric evaluation
         self.scorer_ = scorers
 
         self.cv_results_ = results
         self.n_splits_ = n_splits
 
         return self
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_class_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
 from sklearn.preprocessing import label_binarize
 from matplotlib import colors
 import copy
 import decimal
 
 from .multiclass_fitparams import OneVsRestClassifierPatched
-from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection
+from ._cv_eval_set_old import init_eval_set, _make_transformer, _eval_set_selection
 
 class classplot():
     # 散布図カラーリスト
     _SCATTER_COLORS = ['green', 'red', 'mediumblue', 'brown', 'darkmagenta', 'darkorange', 'gold', 'grey']
     # クラス確率図カラーマップ
     _PROB_CMAP = ['Greens', 'Reds', 'Blues', 'YlOrBr', 'Purples', 'OrRd', 'Wistia', 'Greys']
     # デフォルトでの決定境界図の透明度(alpha)
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_hist_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_pair_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_reg_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from scipy import stats
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, mean_squared_log_error, mean_absolute_percentage_error
 from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
 import decimal
 
-from ._cv_eval_set import init_eval_set, _make_transformer, _eval_set_selection, cross_val_score_eval_set
+from ._cv_eval_set_old import init_eval_set, _make_transformer, _eval_set_selection, cross_val_score_eval_set
 
 class regplot():
     # regression_heat_plotメソッド (回帰モデルヒートマップ表示)における、散布図カラーマップ
     _HEAT_SCATTER_HUECOLORS = ['red', 'mediumblue', 'darkorange', 'darkmagenta', 'cyan',  'pink', 'brown', 'gold', 'grey']
 
     def _round_digits(src: float, rounddigit: int = None, method='decimal'):
         """
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.2/seaborn_analyzer/multiclass_fitparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 import numpy as np
 from sklearn import clone
 from sklearn.multiclass import OneVsRestClassifier, _ConstantPredictor
 from sklearn.preprocessing import LabelBinarizer
-from sklearn.utils.fixes import delayed
-from joblib import Parallel
+from sklearn.utils.parallel import delayed, Parallel
 
 def _fit_binary(estimator, X, y, classes=None, **kwargs):
     """Fit a single binary estimator with kwargs."""
     unique_y = np.unique(y)
     if len(unique_y) == 1:
         if classes is not None:
             if y[0] == -1:
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/PKG-INFO` & `seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.1
+Version: 0.3.2
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.1 requires
+seaborn-analyzer 0.3.2 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/SOURCES.txt` & `seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE
 README.rst
 setup.py
 seaborn_analyzer/__init__.py
 seaborn_analyzer/_cv_eval_set.py
-seaborn_analyzer/_cv_eval_set_sklearn.py
+seaborn_analyzer/_cv_eval_set_old.py
 seaborn_analyzer/custom_class_plot.py
 seaborn_analyzer/custom_hist_plot.py
 seaborn_analyzer/custom_pair_plot.py
 seaborn_analyzer/custom_reg_plot.py
 seaborn_analyzer/multiclass_fitparams.py
 seaborn_analyzer.egg-info/PKG-INFO
 seaborn_analyzer.egg-info/SOURCES.txt
 seaborn_analyzer.egg-info/dependency_links.txt
 seaborn_analyzer.egg-info/requires.txt
-seaborn_analyzer.egg-info/top_level.txt
+seaborn_analyzer.egg-info/top_level.txt
+tests/test_cv.py
```

### Comparing `seaborn-analyzer-0.3.1/setup.py` & `seaborn-analyzer-0.3.2/setup.py`

 * *Files identical despite different names*

