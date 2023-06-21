# Comparing `tmp/atlantis-2022.9.7.1.tar.gz` & `tmp/atlantis-2023.6.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantis-2022.9.7.1.tar", last modified: Wed Sep  7 18:06:35 2022, max compression
+gzip compressed data, was "atlantis-2023.6.21.tar", last modified: Wed Jun 21 16:28:13 2023, max compression
```

## Comparing `atlantis-2022.9.7.1.tar` & `atlantis-2023.6.21.tar`

### file list

```diff
@@ -1,274 +1,294 @@
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.510216 atlantis-2022.9.7.1/
--rw-r--r--   0 idin       (503) wheel        (0)     3922 2022-09-07 18:06:35.509773 atlantis-2022.9.7.1/PKG-INFO
--rw-r--r--   0 idin       (503) wheel        (0)     2838 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/README.md
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.386440 atlantis-2022.9.7.1/atlantis/
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.390128 atlantis-2022.9.7.1/atlantis/auto/
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/auto/DataScientist.py
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/auto/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.398391 atlantis-2022.9.7.1/atlantis/collections/
--rw-r--r--   0 idin       (503) wheel        (0)     1304 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/Counter.py
--rw-r--r--   0 idin       (503) wheel        (0)     1990 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/List.py
--rw-r--r--   0 idin       (503) wheel        (0)     1771 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/OrderedSet.py
--rw-r--r--   0 idin       (503) wheel        (0)     2248 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/Series.py
--rw-r--r--   0 idin       (503) wheel        (0)     2652 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_JupyterContainer.py
--rw-r--r--   0 idin       (503) wheel        (0)      635 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      931 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_create_grid.py
--rw-r--r--   0 idin       (503) wheel        (0)      457 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_cross_lists.py
--rw-r--r--   0 idin       (503) wheel        (0)      709 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_duplicates.py
--rw-r--r--   0 idin       (503) wheel        (0)      225 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_flatten.py
--rw-r--r--   0 idin       (503) wheel        (0)      300 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_get_powerset.py
--rw-r--r--   0 idin       (503) wheel        (0)      482 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_make_hashable.py
--rw-r--r--   0 idin       (503) wheel        (0)      682 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/_product.py
--rw-r--r--   0 idin       (503) wheel        (0)      148 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/cumsum.py
--rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/collections/get_intersection.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.401906 atlantis-2022.9.7.1/atlantis/colour/
--rw-r--r--   0 idin       (503) wheel        (0)    17843 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/Colour.py
--rw-r--r--   0 idin       (503) wheel        (0)      831 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/Gradient.py
--rw-r--r--   0 idin       (503) wheel        (0)     6007 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/Scheme.py
--rw-r--r--   0 idin       (503) wheel        (0)      165 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1123 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/_colour_schemes.py
--rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/_colour_text.py
--rw-r--r--   0 idin       (503) wheel        (0)     1023 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/_colourize.py
--rw-r--r--   0 idin       (503) wheel        (0)      699 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/colour/_convert_rgb_to_hsl.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.403245 atlantis-2022.9.7.1/atlantis/data_files/
--rw-r--r--   0 idin       (503) wheel        (0)    20341 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/data_files/colour_schemes.pickle
--rw-r--r--   0 idin       (503) wheel        (0)     3044 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/data_files/svg_colours.pickle
--rw-r--r--   0 idin       (503) wheel        (0)    11016 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/data_files/x11_colours.pickle
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.403640 atlantis-2022.9.7.1/atlantis/ds/
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.404418 atlantis-2022.9.7.1/atlantis/ds/algebra/
--rw-r--r--   0 idin       (503) wheel        (0)     2460 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/algebra/Matrix.py
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/algebra/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.405215 atlantis-2022.9.7.1/atlantis/ds/auto/
--rw-r--r--   0 idin       (503) wheel        (0)     3403 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/auto/_AutoML.py
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/auto/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.405848 atlantis-2022.9.7.1/atlantis/ds/classification/
--rw-r--r--   0 idin       (503) wheel        (0)     5718 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/classification/ProbabilityClassifier.py
--rw-r--r--   0 idin       (503) wheel        (0)       57 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/classification/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.406954 atlantis-2022.9.7.1/atlantis/ds/clustering/
--rw-r--r--   0 idin       (503) wheel        (0)     5643 2022-09-07 18:06:26.000000 atlantis-2022.9.7.1/atlantis/ds/clustering/ClusteringOptimizer.py
--rw-r--r--   0 idin       (503) wheel        (0)    10186 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/clustering/KMeans.py
--rw-r--r--   0 idin       (503) wheel        (0)       80 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/clustering/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.408151 atlantis-2022.9.7.1/atlantis/ds/ensemble/
--rw-r--r--   0 idin       (503) wheel        (0)     2647 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/ensemble/Ensemble.py
--rw-r--r--   0 idin       (503) wheel        (0)     1019 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/ensemble/PrincipalComponentModelFactory.py
--rw-r--r--   0 idin       (503) wheel        (0)      131 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/ensemble/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.408926 atlantis-2022.9.7.1/atlantis/ds/entropy/
--rw-r--r--   0 idin       (503) wheel        (0)      104 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/entropy/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1003 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/entropy/_get_entropy.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.411278 atlantis-2022.9.7.1/atlantis/ds/evaluation/
--rw-r--r--   0 idin       (503) wheel        (0)      262 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/evaluation/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     2887 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_classification.py
--rw-r--r--   0 idin       (503) wheel        (0)     1676 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_mutliclass_classification.py
--rw-r--r--   0 idin       (503) wheel        (0)     2651 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_regression.py
--rw-r--r--   0 idin       (503) wheel        (0)     1078 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/evaluation/_get_confusion_matrix_df.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.413329 atlantis-2022.9.7.1/atlantis/ds/feature_importance/
--rw-r--r--   0 idin       (503) wheel        (0)     7079 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/feature_importance/InfluenceSimulator.py
--rw-r--r--   0 idin       (503) wheel        (0)      214 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/feature_importance/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      885 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_coefficients.py
--rw-r--r--   0 idin       (503) wheel        (0)      719 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_feature_importances.py
--rw-r--r--   0 idin       (503) wheel        (0)     4348 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_model_influence.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.414993 atlantis-2022.9.7.1/atlantis/ds/imputation/
--rw-r--r--   0 idin       (503) wheel        (0)     5060 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation/Imputer.py
--rw-r--r--   0 idin       (503) wheel        (0)     2674 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation/SingleColumnImputer.py
--rw-r--r--   0 idin       (503) wheel        (0)      163 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1844 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation/_find_good_columns.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.415503 atlantis-2022.9.7.1/atlantis/ds/imputation/exceptions/
--rw-r--r--   0 idin       (503) wheel        (0)      418 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation/exceptions/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.418039 atlantis-2022.9.7.1/atlantis/ds/imputation2/
--rw-r--r--   0 idin       (503) wheel        (0)     5205 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation2/DataImputer.py
--rw-r--r--   0 idin       (503) wheel        (0)     3054 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation2/Imputer.py
--rw-r--r--   0 idin       (503) wheel        (0)     3985 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation2/_ColumnImputer.py
--rw-r--r--   0 idin       (503) wheel        (0)       79 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation2/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     2053 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/imputation2/_fill_na_and_flag.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.420908 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/
--rw-r--r--   0 idin       (503) wheel        (0)      990 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_DataSlice.py
--rw-r--r--   0 idin       (503) wheel        (0)    12982 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Processor.py
--rw-r--r--   0 idin       (503) wheel        (0)     5643 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Project.py
--rw-r--r--   0 idin       (503) wheel        (0)     2641 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Task.py
--rw-r--r--   0 idin       (503) wheel        (0)      696 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_TimeEstimate.py
--rw-r--r--   0 idin       (503) wheel        (0)       87 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      766 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_get_data_from_namespace.py
--rw-r--r--   0 idin       (503) wheel        (0)     1096 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_worker.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.422767 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/
--rw-r--r--   0 idin       (503) wheel        (0)     4598 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_CrossValidationProject.py
--rw-r--r--   0 idin       (503) wheel        (0)    13867 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_LearningProject.py
--rw-r--r--   0 idin       (503) wheel        (0)     6194 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_LearningTask.py
--rw-r--r--   0 idin       (503) wheel        (0)      146 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1067 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_example_1.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.423445 atlantis-2022.9.7.1/atlantis/ds/prediction/
--rw-r--r--   0 idin       (503) wheel        (0)     2471 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/prediction/PredictorBase.py
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/prediction/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.426136 atlantis-2022.9.7.1/atlantis/ds/preprocessing/
--rw-r--r--   0 idin       (503) wheel        (0)     2976 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/Normalizer.py
--rw-r--r--   0 idin       (503) wheel        (0)     5700 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/OneHotEncoder.py
--rw-r--r--   0 idin       (503) wheel        (0)     3326 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/PCA.py
--rw-r--r--   0 idin       (503) wheel        (0)     1666 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/Polynomial.py
--rw-r--r--   0 idin       (503) wheel        (0)     2422 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/Scaler.py
--rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1502 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/preprocessing/disassemble.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.426484 atlantis-2022.9.7.1/atlantis/ds/regression/
--rw-r--r--   0 idin       (503) wheel        (0)      155 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/regression/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.427879 atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/
--rw-r--r--   0 idin       (503) wheel        (0)     1157 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/RegularizedLeastSquares.py
--rw-r--r--   0 idin       (503) wheel        (0)     3422 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForNumpy.py
--rw-r--r--   0 idin       (503) wheel        (0)     2228 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForPandas.py
--rw-r--r--   0 idin       (503) wheel        (0)       61 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.430481 atlantis-2022.9.7.1/atlantis/ds/sampling/
--rw-r--r--   0 idin       (503) wheel        (0)      287 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/Sampler.py
--rw-r--r--   0 idin       (503) wheel        (0)     2139 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/UpSampler.py
--rw-r--r--   0 idin       (503) wheel        (0)      223 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      981 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/_balance_sample.py
--rw-r--r--   0 idin       (503) wheel        (0)     2871 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/_sample_by_id.py
--rw-r--r--   0 idin       (503) wheel        (0)     1788 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/_sample_per_group.py
--rw-r--r--   0 idin       (503) wheel        (0)      618 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/sampling/_split_data.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.432113 atlantis-2022.9.7.1/atlantis/ds/slicing/
--rw-r--r--   0 idin       (503) wheel        (0)     2135 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/slicing/DataSlice.py
--rw-r--r--   0 idin       (503) wheel        (0)      821 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/slicing/SliceTemplate.py
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/slicing/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      290 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/slicing/_get_rows.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.433357 atlantis-2022.9.7.1/atlantis/ds/synthetic_data/
--rw-r--r--   0 idin       (503) wheel        (0)       38 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/synthetic_data/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      504 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/synthetic_data/_create_data.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.435089 atlantis-2022.9.7.1/atlantis/ds/testing/
--rw-r--r--   0 idin       (503) wheel        (0)      116 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/testing/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      472 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/testing/assert_columns_are_unique.py
--rw-r--r--   0 idin       (503) wheel        (0)      751 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/testing/assert_has_columns.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.436060 atlantis-2022.9.7.1/atlantis/ds/tuning/
--rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/tuning/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      151 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/tuning/_tune.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.444853 atlantis-2022.9.7.1/atlantis/ds/validation/
--rw-r--r--   0 idin       (503) wheel        (0)     4728 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_CrossValidation.py
--rw-r--r--   0 idin       (503) wheel        (0)      785 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_DataContainer.py
--rw-r--r--   0 idin       (503) wheel        (0)     1591 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_EstimatorRace.py
--rw-r--r--   0 idin       (503) wheel        (0)     4045 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_EstimatorRepository.py
--rw-r--r--   0 idin       (503) wheel        (0)     4478 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_Evaluation.py
--rw-r--r--   0 idin       (503) wheel        (0)     1680 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_Result.py
--rw-r--r--   0 idin       (503) wheel        (0)     8053 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_Scoreboard.py
--rw-r--r--   0 idin       (503) wheel        (0)     5365 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_TrainingTestContainer.py
--rw-r--r--   0 idin       (503) wheel        (0)     6870 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_ValidationContainer.py
--rw-r--r--   0 idin       (503) wheel        (0)      444 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     6974 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_get_cross_validation.py
--rw-r--r--   0 idin       (503) wheel        (0)     1162 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_get_training_test.py
--rw-r--r--   0 idin       (503) wheel        (0)     1037 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_split_data.py
--rw-r--r--   0 idin       (503) wheel        (0)     2188 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/validation/_train_and_test.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.466242 atlantis-2022.9.7.1/atlantis/ds/wrangling/
--rw-r--r--   0 idin       (503) wheel        (0)     6477 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/NearestFinder.py
--rw-r--r--   0 idin       (503) wheel        (0)     2167 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/NullReplacer.py
--rw-r--r--   0 idin       (503) wheel        (0)     1454 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     3436 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_apply_function.py
--rw-r--r--   0 idin       (503) wheel        (0)      238 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_as_numeric.py
--rw-r--r--   0 idin       (503) wheel        (0)       85 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_as_string.py
--rw-r--r--   0 idin       (503) wheel        (0)     1054 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_bring_to_front.py
--rw-r--r--   0 idin       (503) wheel        (0)      120 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_columns_are_unique.py
--rw-r--r--   0 idin       (503) wheel        (0)      342 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_count_rows_with_missing.py
--rw-r--r--   0 idin       (503) wheel        (0)      403 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_create_data_from_combinations.py
--rw-r--r--   0 idin       (503) wheel        (0)     4122 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_drop_bad_columns.py
--rw-r--r--   0 idin       (503) wheel        (0)      510 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_fast_merge.py
--rw-r--r--   0 idin       (503) wheel        (0)      607 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_fill_na.py
--rw-r--r--   0 idin       (503) wheel        (0)      190 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_find_duplicated_columns.py
--rw-r--r--   0 idin       (503) wheel        (0)     3073 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_find_values.py
--rw-r--r--   0 idin       (503) wheel        (0)      550 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_get_string_columns.py
--rw-r--r--   0 idin       (503) wheel        (0)     1579 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_imputate_with_regression.py
--rw-r--r--   0 idin       (503) wheel        (0)      556 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_join_and_preserve_types.py
--rw-r--r--   0 idin       (503) wheel        (0)     2019 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_join_wisely.py
--rw-r--r--   0 idin       (503) wheel        (0)      543 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_long_to_wide.py
--rw-r--r--   0 idin       (503) wheel        (0)      669 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_min_max.py
--rw-r--r--   0 idin       (503) wheel        (0)     3686 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_read_excel.py
--rw-r--r--   0 idin       (503) wheel        (0)       69 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_reset_column_index.py
--rw-r--r--   0 idin       (503) wheel        (0)      237 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_select_columns.py
--rw-r--r--   0 idin       (503) wheel        (0)      850 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_select_extreme.py
--rw-r--r--   0 idin       (503) wheel        (0)      262 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_set_value_where.py
--rw-r--r--   0 idin       (503) wheel        (0)      914 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_split_rows.py
--rw-r--r--   0 idin       (503) wheel        (0)     1937 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/_standardize_columns.py
--rw-r--r--   0 idin       (503) wheel        (0)     2844 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/get_modified_zscore.py
--rw-r--r--   0 idin       (503) wheel        (0)      580 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/melt.py
--rw-r--r--   0 idin       (503) wheel        (0)     4155 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/ds/wrangling/union.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.468208 atlantis-2022.9.7.1/atlantis/exceptions/
--rw-r--r--   0 idin       (503) wheel        (0)       74 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/exceptions/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      657 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/exceptions/_datascience_exceptions.py
--rw-r--r--   0 idin       (503) wheel        (0)      447 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/exceptions/_general_exceptions.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.470065 atlantis-2022.9.7.1/atlantis/functions/
--rw-r--r--   0 idin       (503) wheel        (0)      138 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/functions/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      744 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/functions/_exit_after.py
--rw-r--r--   0 idin       (503) wheel        (0)      222 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/functions/_get_function_arguments.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.470694 atlantis-2022.9.7.1/atlantis/hash/
--rw-r--r--   0 idin       (503) wheel        (0)     1083 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/hash/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.476127 atlantis-2022.9.7.1/atlantis/multiprocessing/
--rw-r--r--   0 idin       (503) wheel        (0)     4571 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/BaseController.py
--rw-r--r--   0 idin       (503) wheel        (0)     1029 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/Controller.py
--rw-r--r--   0 idin       (503) wheel        (0)     1281 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/JobController.py
--rw-r--r--   0 idin       (503) wheel        (0)     6879 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/ProcessController.py
--rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/SimpleController.py
--rw-r--r--   0 idin       (503) wheel        (0)      110 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/_DEFAULT_VALUES.py
--rw-r--r--   0 idin       (503) wheel        (0)     3323 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/_Task.py
--rw-r--r--   0 idin       (503) wheel        (0)     1134 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/_WorkerReport.py
--rw-r--r--   0 idin       (503) wheel        (0)      172 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     2070 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/_do_task.py
--rw-r--r--   0 idin       (503) wheel        (0)     2770 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/_supervise.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.477702 atlantis-2022.9.7.1/atlantis/multiprocessing/validation/
--rw-r--r--   0 idin       (503) wheel        (0)     1071 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/validation/ValidationController.py
--rw-r--r--   0 idin       (503) wheel        (0)       55 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/validation/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     2270 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/multiprocessing/validation/_validate.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.482173 atlantis-2022.9.7.1/atlantis/text/
--rw-r--r--   0 idin       (503) wheel        (0)      440 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      184 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_align.py
--rw-r--r--   0 idin       (503) wheel        (0)      740 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_convert_camel_to_snake.py
--rw-r--r--   0 idin       (503) wheel        (0)      425 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_count_sentences.py
--rw-r--r--   0 idin       (503) wheel        (0)      291 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_get_domain_and_tld.py
--rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_is_word.py
--rw-r--r--   0 idin       (503) wheel        (0)      467 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_remove_non_alphanumeric.py
--rw-r--r--   0 idin       (503) wheel        (0)      205 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_split_and_strip.py
--rw-r--r--   0 idin       (503) wheel        (0)      587 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/text/_wrap.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.482782 atlantis-2022.9.7.1/atlantis/time/
--rw-r--r--   0 idin       (503) wheel        (0)      760 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.492013 atlantis-2022.9.7.1/atlantis/time/date/
--rw-r--r--   0 idin       (503) wheel        (0)     2726 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/YearMonth.py
--rw-r--r--   0 idin       (503) wheel        (0)     1980 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/YearQuarter.py
--rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     2135 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/add_time.py
--rw-r--r--   0 idin       (503) wheel        (0)      236 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/convert_string_to_date.py
--rw-r--r--   0 idin       (503) wheel        (0)      491 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_date_mean.py
--rw-r--r--   0 idin       (503) wheel        (0)     2506 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_date_part.py
--rw-r--r--   0 idin       (503) wheel        (0)      695 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_first_day_of_month.py
--rw-r--r--   0 idin       (503) wheel        (0)      621 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_month.py
--rw-r--r--   0 idin       (503) wheel        (0)      493 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_number_of_days.py
--rw-r--r--   0 idin       (503) wheel        (0)      116 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_quarter.py
--rw-r--r--   0 idin       (503) wheel        (0)      341 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_today.py
--rw-r--r--   0 idin       (503) wheel        (0)      186 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/get_week_number.py
--rw-r--r--   0 idin       (503) wheel        (0)     1160 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/parse_date.py
--rw-r--r--   0 idin       (503) wheel        (0)      247 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/date/remove_non_alphanumeric.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.495310 atlantis-2022.9.7.1/atlantis/time/estimate/
--rw-r--r--   0 idin       (503) wheel        (0)    16371 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/estimate/Estimator.py
--rw-r--r--   0 idin       (503) wheel        (0)     1648 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/estimate/Measurement.py
--rw-r--r--   0 idin       (503) wheel        (0)       33 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/estimate/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      895 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/estimate/create_arguments.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.497542 atlantis-2022.9.7.1/atlantis/time/numbers/
--rw-r--r--   0 idin       (503) wheel        (0)     3995 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/numbers/FlexibleNumber.py
--rw-r--r--   0 idin       (503) wheel        (0)     3246 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/numbers/NumberPart.py
--rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/numbers/__init__.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.500372 atlantis-2022.9.7.1/atlantis/time/progress/
--rw-r--r--   0 idin       (503) wheel        (0)     1549 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/progress/Iterable.py
--rw-r--r--   0 idin       (503) wheel        (0)    14487 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/progress/ProgressBar.py
--rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/progress/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)     1805 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/progress/_map.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.508937 atlantis-2022.9.7.1/atlantis/time/time/
--rw-r--r--   0 idin       (503) wheel        (0)     4520 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/MeasurementSet.py
--rw-r--r--   0 idin       (503) wheel        (0)      821 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/TimeMeasurement.py
--rw-r--r--   0 idin       (503) wheel        (0)     1755 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/Timer.py
--rw-r--r--   0 idin       (503) wheel        (0)      838 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/_Job.py
--rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/__init__.py
--rw-r--r--   0 idin       (503) wheel        (0)      978 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/convert.py
--rw-r--r--   0 idin       (503) wheel        (0)     1926 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/get_elapsed.py
--rw-r--r--   0 idin       (503) wheel        (0)      184 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/get_time.py
--rw-r--r--   0 idin       (503) wheel        (0)      563 2022-09-06 18:08:35.000000 atlantis-2022.9.7.1/atlantis/time/time/measure.py
-drwxr-xr-x   0 idin       (503) wheel        (0)        0 2022-09-07 18:06:35.389170 atlantis-2022.9.7.1/atlantis.egg-info/
--rw-r--r--   0 idin       (503) wheel        (0)     3922 2022-09-07 18:06:35.000000 atlantis-2022.9.7.1/atlantis.egg-info/PKG-INFO
--rw-r--r--   0 idin       (503) wheel        (0)     8934 2022-09-07 18:06:35.000000 atlantis-2022.9.7.1/atlantis.egg-info/SOURCES.txt
--rw-r--r--   0 idin       (503) wheel        (0)        1 2022-09-07 18:06:35.000000 atlantis-2022.9.7.1/atlantis.egg-info/dependency_links.txt
--rw-r--r--   0 idin       (503) wheel        (0)        1 2022-09-07 17:46:57.000000 atlantis-2022.9.7.1/atlantis.egg-info/not-zip-safe
--rw-r--r--   0 idin       (503) wheel        (0)      104 2022-09-07 18:06:35.000000 atlantis-2022.9.7.1/atlantis.egg-info/requires.txt
--rw-r--r--   0 idin       (503) wheel        (0)        9 2022-09-07 18:06:35.000000 atlantis-2022.9.7.1/atlantis.egg-info/top_level.txt
--rw-r--r--   0 idin       (503) wheel        (0)       38 2022-09-07 18:06:35.510371 atlantis-2022.9.7.1/setup.cfg
--rw-r--r--   0 idin       (503) wheel        (0)      738 2022-09-07 18:06:34.000000 atlantis-2022.9.7.1/setup.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.619337 atlantis-2023.6.21/
+-rw-r--r--   0 idin       (503) wheel        (0)     3107 2023-06-21 16:28:13.618858 atlantis-2023.6.21/PKG-INFO
+-rw-r--r--   0 idin       (503) wheel        (0)     2838 2022-09-06 18:08:35.000000 atlantis-2023.6.21/README.md
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.414428 atlantis-2023.6.21/atlantis/
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.418295 atlantis-2023.6.21/atlantis/auto/
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/auto/DataScientist.py
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/auto/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.429747 atlantis-2023.6.21/atlantis/collections/
+-rw-r--r--   0 idin       (503) wheel        (0)     1304 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/Counter.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1990 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/List.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1771 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/OrderedSet.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2248 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/Series.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2652 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_JupyterContainer.py
+-rw-r--r--   0 idin       (503) wheel        (0)      635 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      931 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_create_grid.py
+-rw-r--r--   0 idin       (503) wheel        (0)      457 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_cross_lists.py
+-rw-r--r--   0 idin       (503) wheel        (0)      709 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_duplicates.py
+-rw-r--r--   0 idin       (503) wheel        (0)      225 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_flatten.py
+-rw-r--r--   0 idin       (503) wheel        (0)      300 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_get_powerset.py
+-rw-r--r--   0 idin       (503) wheel        (0)      482 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_make_hashable.py
+-rw-r--r--   0 idin       (503) wheel        (0)      682 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/_product.py
+-rw-r--r--   0 idin       (503) wheel        (0)      148 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/cumsum.py
+-rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/collections/get_intersection.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.436588 atlantis-2023.6.21/atlantis/colour/
+-rw-r--r--   0 idin       (503) wheel        (0)    17843 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/Colour.py
+-rw-r--r--   0 idin       (503) wheel        (0)      831 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/Gradient.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6007 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/Scheme.py
+-rw-r--r--   0 idin       (503) wheel        (0)      165 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1123 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/_colour_schemes.py
+-rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/_colour_text.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1023 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/_colourize.py
+-rw-r--r--   0 idin       (503) wheel        (0)      699 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/colour/_convert_rgb_to_hsl.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.438855 atlantis-2023.6.21/atlantis/data_files/
+-rw-r--r--   0 idin       (503) wheel        (0)    20341 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/data_files/colour_schemes.pickle
+-rw-r--r--   0 idin       (503) wheel        (0)     3044 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/data_files/svg_colours.pickle
+-rw-r--r--   0 idin       (503) wheel        (0)    11016 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/data_files/x11_colours.pickle
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.439579 atlantis-2023.6.21/atlantis/ds/
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.441097 atlantis-2023.6.21/atlantis/ds/algebra/
+-rw-r--r--   0 idin       (503) wheel        (0)     2460 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/algebra/Matrix.py
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/algebra/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.442579 atlantis-2023.6.21/atlantis/ds/auto/
+-rw-r--r--   0 idin       (503) wheel        (0)     3411 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/auto/_AutoML.py
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/auto/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.447848 atlantis-2023.6.21/atlantis/ds/classification/
+-rw-r--r--   0 idin       (503) wheel        (0)    11647 2023-06-19 22:51:27.000000 atlantis-2023.6.21/atlantis/ds/classification/Classifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6691 2023-06-05 17:09:00.000000 atlantis-2023.6.21/atlantis/ds/classification/Encoder.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4054 2023-06-19 22:51:27.000000 atlantis-2023.6.21/atlantis/ds/classification/EnsembleClassifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)      124 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/classification/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2833 2022-10-26 00:11:41.000000 atlantis-2023.6.21/atlantis/ds/classification/measure_performance.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.450922 atlantis-2023.6.21/atlantis/ds/clustering/
+-rw-r--r--   0 idin       (503) wheel        (0)     5643 2022-09-07 18:06:26.000000 atlantis-2023.6.21/atlantis/ds/clustering/ClusteringOptimizer.py
+-rw-r--r--   0 idin       (503) wheel        (0)    11289 2022-12-16 22:09:43.000000 atlantis-2023.6.21/atlantis/ds/clustering/KMeans.py
+-rw-r--r--   0 idin       (503) wheel        (0)       80 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/clustering/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.454190 atlantis-2023.6.21/atlantis/ds/ensemble/
+-rw-r--r--   0 idin       (503) wheel        (0)     2647 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/ensemble/Ensemble.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1019 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/ensemble/PrincipalComponentModelFactory.py
+-rw-r--r--   0 idin       (503) wheel        (0)      131 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/ensemble/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.455720 atlantis-2023.6.21/atlantis/ds/entropy/
+-rw-r--r--   0 idin       (503) wheel        (0)      104 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/entropy/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1003 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/entropy/_get_entropy.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.459950 atlantis-2023.6.21/atlantis/ds/evaluation/
+-rw-r--r--   0 idin       (503) wheel        (0)      262 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/evaluation/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2887 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_classification.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1676 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_mutliclass_classification.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2651 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_regression.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1078 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/evaluation/_get_confusion_matrix_df.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.464379 atlantis-2023.6.21/atlantis/ds/feature_importance/
+-rw-r--r--   0 idin       (503) wheel        (0)     7079 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/feature_importance/InfluenceSimulator.py
+-rw-r--r--   0 idin       (503) wheel        (0)      214 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/feature_importance/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      885 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/feature_importance/_get_coefficients.py
+-rw-r--r--   0 idin       (503) wheel        (0)      719 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/feature_importance/_get_feature_importances.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4348 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/feature_importance/_get_model_influence.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.468085 atlantis-2023.6.21/atlantis/ds/imputation/
+-rw-r--r--   0 idin       (503) wheel        (0)     5060 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation/Imputer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2674 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation/SingleColumnImputer.py
+-rw-r--r--   0 idin       (503) wheel        (0)      163 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1844 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation/_find_good_columns.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.469008 atlantis-2023.6.21/atlantis/ds/imputation/exceptions/
+-rw-r--r--   0 idin       (503) wheel        (0)      418 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation/exceptions/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.473948 atlantis-2023.6.21/atlantis/ds/imputation2/
+-rw-r--r--   0 idin       (503) wheel        (0)     5205 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation2/DataImputer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3054 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation2/Imputer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3989 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/imputation2/_ColumnImputer.py
+-rw-r--r--   0 idin       (503) wheel        (0)       79 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation2/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2053 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/imputation2/_fill_na_and_flag.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.480346 atlantis-2023.6.21/atlantis/ds/old_classification/
+-rw-r--r--   0 idin       (503) wheel        (0)     5718 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_classification/ProbabilityClassifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)      829 2022-09-09 23:55:46.000000 atlantis-2023.6.21/atlantis/ds/old_classification/RandomForestClassifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)       57 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_classification/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1700 2022-09-10 00:22:14.000000 atlantis-2023.6.21/atlantis/ds/old_classification/oldClassifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6006 2022-09-07 23:03:10.000000 atlantis-2023.6.21/atlantis/ds/old_classification/pyspark_classifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6442 2022-09-08 17:56:57.000000 atlantis-2023.6.21/atlantis/ds/old_classification/test delete.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.491510 atlantis-2023.6.21/atlantis/ds/old_validation/
+-rw-r--r--   0 idin       (503) wheel        (0)     4728 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_CrossValidation.py
+-rw-r--r--   0 idin       (503) wheel        (0)      785 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_DataContainer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1591 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_EstimatorRace.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4045 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_EstimatorRepository.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4478 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_Evaluation.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1680 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_Result.py
+-rw-r--r--   0 idin       (503) wheel        (0)     8053 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_Scoreboard.py
+-rw-r--r--   0 idin       (503) wheel        (0)     5365 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_TrainingTestContainer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6870 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_ValidationContainer.py
+-rw-r--r--   0 idin       (503) wheel        (0)      444 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6974 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_get_cross_validation.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1162 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_get_training_test.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1037 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_split_data.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2188 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/old_validation/_train_and_test.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.499046 atlantis-2023.6.21/atlantis/ds/parallel_computing/
+-rw-r--r--   0 idin       (503) wheel        (0)      990 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_DataSlice.py
+-rw-r--r--   0 idin       (503) wheel        (0)    12982 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_Processor.py
+-rw-r--r--   0 idin       (503) wheel        (0)     5643 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_Project.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2641 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_Task.py
+-rw-r--r--   0 idin       (503) wheel        (0)      696 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_TimeEstimate.py
+-rw-r--r--   0 idin       (503) wheel        (0)       87 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      766 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_get_data_from_namespace.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1096 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/_worker.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.507717 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/
+-rw-r--r--   0 idin       (503) wheel        (0)     4602 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_CrossValidationProject.py
+-rw-r--r--   0 idin       (503) wheel        (0)    13871 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_LearningProject.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6194 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_LearningTask.py
+-rw-r--r--   0 idin       (503) wheel        (0)      146 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1075 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_example_1.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.509818 atlantis-2023.6.21/atlantis/ds/prediction/
+-rw-r--r--   0 idin       (503) wheel        (0)     2471 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/prediction/PredictorBase.py
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/prediction/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.519861 atlantis-2023.6.21/atlantis/ds/preprocessing/
+-rw-r--r--   0 idin       (503) wheel        (0)     2976 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/Normalizer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     5700 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/OneHotEncoder.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3470 2022-12-19 19:40:48.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/PCA.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1666 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/Polynomial.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2574 2022-12-19 19:37:08.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/Scaler.py
+-rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1502 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/preprocessing/disassemble.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.520615 atlantis-2023.6.21/atlantis/ds/regression/
+-rw-r--r--   0 idin       (503) wheel        (0)      155 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/regression/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.524528 atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/
+-rw-r--r--   0 idin       (503) wheel        (0)     1157 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/RegularizedLeastSquares.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3422 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForNumpy.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2228 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForPandas.py
+-rw-r--r--   0 idin       (503) wheel        (0)       61 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.532150 atlantis-2023.6.21/atlantis/ds/sampling/
+-rw-r--r--   0 idin       (503) wheel        (0)      287 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/Sampler.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2139 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/UpSampler.py
+-rw-r--r--   0 idin       (503) wheel        (0)      223 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      981 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/_balance_sample.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2871 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/_sample_by_id.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1788 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/_sample_per_group.py
+-rw-r--r--   0 idin       (503) wheel        (0)      618 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/sampling/_split_data.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.537482 atlantis-2023.6.21/atlantis/ds/slicing/
+-rw-r--r--   0 idin       (503) wheel        (0)      153 2023-06-19 20:16:14.000000 atlantis-2023.6.21/atlantis/ds/slicing/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      934 2023-06-19 20:11:25.000000 atlantis-2023.6.21/atlantis/ds/slicing/_get_random_split_without_hashing.py
+-rw-r--r--   0 idin       (503) wheel        (0)      454 2023-06-19 20:10:15.000000 atlantis-2023.6.21/atlantis/ds/slicing/get_random_by_object.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1064 2023-06-19 20:14:13.000000 atlantis-2023.6.21/atlantis/ds/slicing/get_random_split.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2352 2023-06-19 20:10:15.000000 atlantis-2023.6.21/atlantis/ds/slicing/label_random_split.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.541801 atlantis-2023.6.21/atlantis/ds/supervised_learning/
+-rw-r--r--   0 idin       (503) wheel        (0)      960 2022-09-09 18:54:20.000000 atlantis-2023.6.21/atlantis/ds/supervised_learning/PySparkRandomForestClassifier.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2634 2022-09-09 18:45:35.000000 atlantis-2023.6.21/atlantis/ds/supervised_learning/_BaseSupervisedModel.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2753 2022-09-09 18:29:26.000000 atlantis-2023.6.21/atlantis/ds/supervised_learning/_PySparkModel.py
+-rw-r--r--   0 idin       (503) wheel        (0)      127 2022-09-09 23:27:15.000000 atlantis-2023.6.21/atlantis/ds/supervised_learning/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.543409 atlantis-2023.6.21/atlantis/ds/synthetic_data/
+-rw-r--r--   0 idin       (503) wheel        (0)       38 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/synthetic_data/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      504 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/synthetic_data/_create_data.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.545481 atlantis-2023.6.21/atlantis/ds/testing/
+-rw-r--r--   0 idin       (503) wheel        (0)      116 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/testing/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      472 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/testing/assert_columns_are_unique.py
+-rw-r--r--   0 idin       (503) wheel        (0)      751 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/testing/assert_has_columns.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.546585 atlantis-2023.6.21/atlantis/ds/tuning/
+-rw-r--r--   0 idin       (503) wheel        (0)        0 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/tuning/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      151 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/tuning/_tune.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.548927 atlantis-2023.6.21/atlantis/ds/validation/
+-rw-r--r--   0 idin       (503) wheel        (0)     9229 2023-06-20 21:38:38.000000 atlantis-2023.6.21/atlantis/ds/validation/CrossValidation.py
+-rw-r--r--   0 idin       (503) wheel        (0)       45 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/ds/validation/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2655 2023-06-16 17:14:27.000000 atlantis-2023.6.21/atlantis/ds/validation/validate_classifier.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.571110 atlantis-2023.6.21/atlantis/ds/wrangling/
+-rw-r--r--   0 idin       (503) wheel        (0)     6477 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/NearestFinder.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2167 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/NullReplacer.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1454 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3436 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_apply_function.py
+-rw-r--r--   0 idin       (503) wheel        (0)      238 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_as_numeric.py
+-rw-r--r--   0 idin       (503) wheel        (0)       85 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_as_string.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1054 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_bring_to_front.py
+-rw-r--r--   0 idin       (503) wheel        (0)      120 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_columns_are_unique.py
+-rw-r--r--   0 idin       (503) wheel        (0)      342 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_count_rows_with_missing.py
+-rw-r--r--   0 idin       (503) wheel        (0)      403 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_create_data_from_combinations.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4122 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_drop_bad_columns.py
+-rw-r--r--   0 idin       (503) wheel        (0)      510 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_fast_merge.py
+-rw-r--r--   0 idin       (503) wheel        (0)      607 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_fill_na.py
+-rw-r--r--   0 idin       (503) wheel        (0)      190 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_find_duplicated_columns.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3073 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_find_values.py
+-rw-r--r--   0 idin       (503) wheel        (0)      550 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_get_string_columns.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1579 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_imputate_with_regression.py
+-rw-r--r--   0 idin       (503) wheel        (0)      556 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_join_and_preserve_types.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2019 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_join_wisely.py
+-rw-r--r--   0 idin       (503) wheel        (0)      543 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_long_to_wide.py
+-rw-r--r--   0 idin       (503) wheel        (0)      669 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_min_max.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3686 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_read_excel.py
+-rw-r--r--   0 idin       (503) wheel        (0)       69 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_reset_column_index.py
+-rw-r--r--   0 idin       (503) wheel        (0)      237 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_select_columns.py
+-rw-r--r--   0 idin       (503) wheel        (0)      850 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_select_extreme.py
+-rw-r--r--   0 idin       (503) wheel        (0)      262 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_set_value_where.py
+-rw-r--r--   0 idin       (503) wheel        (0)      914 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_split_rows.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1937 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/_standardize_columns.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2844 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/get_modified_zscore.py
+-rw-r--r--   0 idin       (503) wheel        (0)      580 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/melt.py
+-rw-r--r--   0 idin       (503) wheel        (0)     4155 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/ds/wrangling/union.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.573092 atlantis-2023.6.21/atlantis/exceptions/
+-rw-r--r--   0 idin       (503) wheel        (0)       74 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/exceptions/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      657 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/exceptions/_datascience_exceptions.py
+-rw-r--r--   0 idin       (503) wheel        (0)      447 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/exceptions/_general_exceptions.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.574984 atlantis-2023.6.21/atlantis/functions/
+-rw-r--r--   0 idin       (503) wheel        (0)      138 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/functions/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      744 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/functions/_exit_after.py
+-rw-r--r--   0 idin       (503) wheel        (0)      222 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/functions/_get_function_arguments.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.575512 atlantis-2023.6.21/atlantis/hash/
+-rw-r--r--   0 idin       (503) wheel        (0)     1083 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/hash/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.583167 atlantis-2023.6.21/atlantis/multiprocessing/
+-rw-r--r--   0 idin       (503) wheel        (0)     4571 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/BaseController.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1029 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/Controller.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1281 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/JobController.py
+-rw-r--r--   0 idin       (503) wheel        (0)     6879 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/ProcessController.py
+-rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/SimpleController.py
+-rw-r--r--   0 idin       (503) wheel        (0)      110 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/_DEFAULT_VALUES.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3323 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/_Task.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1134 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/_WorkerReport.py
+-rw-r--r--   0 idin       (503) wheel        (0)      172 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2070 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/_do_task.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2770 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/_supervise.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.585280 atlantis-2023.6.21/atlantis/multiprocessing/validation/
+-rw-r--r--   0 idin       (503) wheel        (0)     1071 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/validation/ValidationController.py
+-rw-r--r--   0 idin       (503) wheel        (0)       55 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/multiprocessing/validation/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2278 2023-06-20 21:38:30.000000 atlantis-2023.6.21/atlantis/multiprocessing/validation/_validate.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.591609 atlantis-2023.6.21/atlantis/text/
+-rw-r--r--   0 idin       (503) wheel        (0)      440 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      184 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_align.py
+-rw-r--r--   0 idin       (503) wheel        (0)      740 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_convert_camel_to_snake.py
+-rw-r--r--   0 idin       (503) wheel        (0)      425 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_count_sentences.py
+-rw-r--r--   0 idin       (503) wheel        (0)      291 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_get_domain_and_tld.py
+-rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_is_word.py
+-rw-r--r--   0 idin       (503) wheel        (0)      467 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_remove_non_alphanumeric.py
+-rw-r--r--   0 idin       (503) wheel        (0)      205 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_split_and_strip.py
+-rw-r--r--   0 idin       (503) wheel        (0)      587 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/text/_wrap.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.592261 atlantis-2023.6.21/atlantis/time/
+-rw-r--r--   0 idin       (503) wheel        (0)      760 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.602368 atlantis-2023.6.21/atlantis/time/date/
+-rw-r--r--   0 idin       (503) wheel        (0)     2726 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/YearMonth.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1980 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/YearQuarter.py
+-rw-r--r--   0 idin       (503) wheel        (0)      782 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2135 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/add_time.py
+-rw-r--r--   0 idin       (503) wheel        (0)      236 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/convert_string_to_date.py
+-rw-r--r--   0 idin       (503) wheel        (0)      491 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_date_mean.py
+-rw-r--r--   0 idin       (503) wheel        (0)     2506 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_date_part.py
+-rw-r--r--   0 idin       (503) wheel        (0)      695 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_first_day_of_month.py
+-rw-r--r--   0 idin       (503) wheel        (0)      621 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_month.py
+-rw-r--r--   0 idin       (503) wheel        (0)      493 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_number_of_days.py
+-rw-r--r--   0 idin       (503) wheel        (0)      116 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_quarter.py
+-rw-r--r--   0 idin       (503) wheel        (0)      341 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_today.py
+-rw-r--r--   0 idin       (503) wheel        (0)      186 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/get_week_number.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1160 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/parse_date.py
+-rw-r--r--   0 idin       (503) wheel        (0)      247 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/date/remove_non_alphanumeric.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.606783 atlantis-2023.6.21/atlantis/time/estimate/
+-rw-r--r--   0 idin       (503) wheel        (0)    16371 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/estimate/Estimator.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1648 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/estimate/Measurement.py
+-rw-r--r--   0 idin       (503) wheel        (0)       33 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/estimate/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      895 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/estimate/create_arguments.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.608898 atlantis-2023.6.21/atlantis/time/numbers/
+-rw-r--r--   0 idin       (503) wheel        (0)     3995 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/numbers/FlexibleNumber.py
+-rw-r--r--   0 idin       (503) wheel        (0)     3246 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/numbers/NumberPart.py
+-rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/numbers/__init__.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.611560 atlantis-2023.6.21/atlantis/time/progress/
+-rw-r--r--   0 idin       (503) wheel        (0)     1549 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/progress/Iterable.py
+-rw-r--r--   0 idin       (503) wheel        (0)    14487 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/progress/ProgressBar.py
+-rw-r--r--   0 idin       (503) wheel        (0)       77 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/progress/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1805 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/progress/_map.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.618057 atlantis-2023.6.21/atlantis/time/time/
+-rw-r--r--   0 idin       (503) wheel        (0)     4520 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/MeasurementSet.py
+-rw-r--r--   0 idin       (503) wheel        (0)      821 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/TimeMeasurement.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1755 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/Timer.py
+-rw-r--r--   0 idin       (503) wheel        (0)      838 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/_Job.py
+-rw-r--r--   0 idin       (503) wheel        (0)      309 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/__init__.py
+-rw-r--r--   0 idin       (503) wheel        (0)      978 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/convert.py
+-rw-r--r--   0 idin       (503) wheel        (0)     1926 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/get_elapsed.py
+-rw-r--r--   0 idin       (503) wheel        (0)      184 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/get_time.py
+-rw-r--r--   0 idin       (503) wheel        (0)      563 2022-09-06 18:08:35.000000 atlantis-2023.6.21/atlantis/time/time/measure.py
+drwxr-xr-x   0 idin       (503) wheel        (0)        0 2023-06-21 16:28:13.417181 atlantis-2023.6.21/atlantis.egg-info/
+-rw-r--r--   0 idin       (503) wheel        (0)     3107 2023-06-21 16:28:13.000000 atlantis-2023.6.21/atlantis.egg-info/PKG-INFO
+-rw-r--r--   0 idin       (503) wheel        (0)     9836 2023-06-21 16:28:13.000000 atlantis-2023.6.21/atlantis.egg-info/SOURCES.txt
+-rw-r--r--   0 idin       (503) wheel        (0)        1 2023-06-21 16:28:13.000000 atlantis-2023.6.21/atlantis.egg-info/dependency_links.txt
+-rw-r--r--   0 idin       (503) wheel        (0)        1 2022-09-07 17:46:57.000000 atlantis-2023.6.21/atlantis.egg-info/not-zip-safe
+-rw-r--r--   0 idin       (503) wheel        (0)      114 2023-06-21 16:28:13.000000 atlantis-2023.6.21/atlantis.egg-info/requires.txt
+-rw-r--r--   0 idin       (503) wheel        (0)        9 2023-06-21 16:28:13.000000 atlantis-2023.6.21/atlantis.egg-info/top_level.txt
+-rw-r--r--   0 idin       (503) wheel        (0)       38 2023-06-21 16:28:13.619881 atlantis-2023.6.21/setup.cfg
+-rw-r--r--   0 idin       (503) wheel        (0)      750 2023-06-21 16:28:12.000000 atlantis-2023.6.21/setup.py
```

### Comparing `atlantis-2022.9.7.1/PKG-INFO` & `atlantis-2023.6.21/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,110 @@
 Metadata-Version: 2.1
 Name: atlantis
-Version: 2022.9.7.1
+Version: 2023.6.21
 Summary: Python library for simplifying data science
 Home-page: https://github.com/idin/atlantis
 Author: Idin
 Author-email: py@idin.ca
 License: MIT
-Description: # ***Atlantis***
-        ***Atlantis*** is a Python library for simplifying programming with Python for data science.
-        
-        # Installation
-        You can just use pip to install Atlantis:
-        
-        `pip install atlantis`
-        
-        # Modules
-        
-        - [***collections***](#collections) helps with working with collections.
-        - [***colour***](about_colour.md) simplifies using colours.
-        - [***ds (datascience)***](#ds-data-science) provides tools for:
-          - data wrangling, 
-          - validation, 
-          - tuning,
-          - sampling, 
-          - evaluation,
-          - clustering, and 
-          - parallel processing of machine learning models.
-        - [***functions***](about_functions.md) manages higher order functions.
-        - [***hash***](about_hash.md) simplifies and standardizes hashing.
-        - [***text***](about_text.md) makes working with texts and strings easy.
-        - [***time***](about_time.md) 
-          - provides methods for interacting with time and date as well as 
-          - progress bars
-          
-        ## *collections*
-        This module of the package [***atlantis***](README.md) helps with working with collections.
-        
-        ### *`flatten`*
-        ```python
-        from atlantis.collections import flatten
-        flatten([1, 2, [3, 4, [5, 6], 7], 8])
-        ```
-        returns: `[1, 2, 3, 4, 5, 6, 7, 8]`
-        
-        ### *`List`*
-        This class inherits from Python's list class but implements a few 
-        additional functionalities.
-        
-        ```python
-        from atlantis.collections import List
-        l = List(1, 2, 3, 4, 2, [1, 2], [1, 2])
-        ```
-        
-        Flattening: 
-        ```python
-        l.flatten()
-        >>> List: [1, 2, 3, 4, 2, 1, 2, 1, 2]
-        ```
-        
-        Finding duplicates:
-        ```python
-        l.get_duplicates()
-        >>> List: [2, List: [1, 2]]
-        ```
-        **Note:** the ***list*** elements of a ***List*** automatically get converted to ***Lists***, recursively.
-        
-        ## *ds* (Data Science)
-        This module provides data science tools for:
-        - data wrangling, 
-        - validation, 
-        - tuning,
-        - sampling, 
-        - evaluation,
-        - clustering, and 
-        - parallel processing of machine learning models.
-        
-        ### *KMeans* Clustering
-        I have used the `KMeans` class from both *sklearn* and that of *pyspark* and was frustrated 
-        by two problems: (a) even though the two classes do exactly the same thing their interfaces
-        are vastly different and (b) some of the simplest operations are very hard to do with 
-        both classes. I solved this problem by creating my own `KMeans` class that is a wrapper 
-        aroung both of those classes and uses the appropriate one automatically without 
-        complicating it for the data scientist programmer. 
-        
-        #### Usage
-        
-        ```python
-        from atlantis.ds.clustering import KMeans
-        
-        kmeans = KMeans(n_clusters=3, n_jobs=10)
-        kmeans.fit(X=X)
-        
-        predictions = kmeans.predict(X=X)
-        transformed_x = kmeans.transform(X=X)
-        ```
-        
-        ### Clustering Optimization
-        
-        #### Usage
-        ```python
-        from atlantis.ds.clustering import ClusteringOptimizer
-        
-        clustering_optimizer = ClusteringOptimizer(min_k=2, max_k=16, n_jobs=10)
-        clustering_optimizer.fit(X=X)
-        print(f'best number of clusters: {clustering_optimizer.optimal_number_of_clusters}')
-        ```
-Platform: UNKNOWN
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+
+# ***Atlantis***
+***Atlantis*** is a Python library for simplifying programming with Python for data science.
+
+# Installation
+You can just use pip to install Atlantis:
+
+`pip install atlantis`
+
+# Modules
+
+- [***collections***](#collections) helps with working with collections.
+- [***colour***](about_colour.md) simplifies using colours.
+- [***ds (datascience)***](#ds-data-science) provides tools for:
+  - data wrangling, 
+  - validation, 
+  - tuning,
+  - sampling, 
+  - evaluation,
+  - clustering, and 
+  - parallel processing of machine learning models.
+- [***functions***](about_functions.md) manages higher order functions.
+- [***hash***](about_hash.md) simplifies and standardizes hashing.
+- [***text***](about_text.md) makes working with texts and strings easy.
+- [***time***](about_time.md) 
+  - provides methods for interacting with time and date as well as 
+  - progress bars
+  
+## *collections*
+This module of the package [***atlantis***](README.md) helps with working with collections.
+
+### *`flatten`*
+```python
+from atlantis.collections import flatten
+flatten([1, 2, [3, 4, [5, 6], 7], 8])
+```
+returns: `[1, 2, 3, 4, 5, 6, 7, 8]`
+
+### *`List`*
+This class inherits from Python's list class but implements a few 
+additional functionalities.
+
+```python
+from atlantis.collections import List
+l = List(1, 2, 3, 4, 2, [1, 2], [1, 2])
+```
+
+Flattening: 
+```python
+l.flatten()
+>>> List: [1, 2, 3, 4, 2, 1, 2, 1, 2]
+```
+
+Finding duplicates:
+```python
+l.get_duplicates()
+>>> List: [2, List: [1, 2]]
+```
+**Note:** the ***list*** elements of a ***List*** automatically get converted to ***Lists***, recursively.
+
+## *ds* (Data Science)
+This module provides data science tools for:
+- data wrangling, 
+- validation, 
+- tuning,
+- sampling, 
+- evaluation,
+- clustering, and 
+- parallel processing of machine learning models.
+
+### *KMeans* Clustering
+I have used the `KMeans` class from both *sklearn* and that of *pyspark* and was frustrated 
+by two problems: (a) even though the two classes do exactly the same thing their interfaces
+are vastly different and (b) some of the simplest operations are very hard to do with 
+both classes. I solved this problem by creating my own `KMeans` class that is a wrapper 
+aroung both of those classes and uses the appropriate one automatically without 
+complicating it for the data scientist programmer. 
+
+#### Usage
+
+```python
+from atlantis.ds.clustering import KMeans
+
+kmeans = KMeans(n_clusters=3, n_jobs=10)
+kmeans.fit(X=X)
+
+predictions = kmeans.predict(X=X)
+transformed_x = kmeans.transform(X=X)
+```
+
+### Clustering Optimization
+
+#### Usage
+```python
+from atlantis.ds.clustering import ClusteringOptimizer
+
+clustering_optimizer = ClusteringOptimizer(min_k=2, max_k=16, n_jobs=10)
+clustering_optimizer.fit(X=X)
+print(f'best number of clusters: {clustering_optimizer.optimal_number_of_clusters}')
+```
```

### Comparing `atlantis-2022.9.7.1/README.md` & `atlantis-2023.6.21/README.md`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/Counter.py` & `atlantis-2023.6.21/atlantis/collections/Counter.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/List.py` & `atlantis-2023.6.21/atlantis/collections/List.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/OrderedSet.py` & `atlantis-2023.6.21/atlantis/collections/OrderedSet.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/Series.py` & `atlantis-2023.6.21/atlantis/collections/Series.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/_JupyterContainer.py` & `atlantis-2023.6.21/atlantis/collections/_JupyterContainer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/__init__.py` & `atlantis-2023.6.21/atlantis/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/_create_grid.py` & `atlantis-2023.6.21/atlantis/collections/_create_grid.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/_duplicates.py` & `atlantis-2023.6.21/atlantis/collections/_duplicates.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/collections/_product.py` & `atlantis-2023.6.21/atlantis/collections/_product.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/Colour.py` & `atlantis-2023.6.21/atlantis/colour/Colour.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/Gradient.py` & `atlantis-2023.6.21/atlantis/colour/Gradient.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/Scheme.py` & `atlantis-2023.6.21/atlantis/colour/Scheme.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/_colour_schemes.py` & `atlantis-2023.6.21/atlantis/colour/_colour_schemes.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/_colour_text.py` & `atlantis-2023.6.21/atlantis/colour/_colour_text.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/_colourize.py` & `atlantis-2023.6.21/atlantis/colour/_colourize.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/colour/_convert_rgb_to_hsl.py` & `atlantis-2023.6.21/atlantis/colour/_convert_rgb_to_hsl.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/data_files/colour_schemes.pickle` & `atlantis-2023.6.21/atlantis/data_files/colour_schemes.pickle`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/data_files/svg_colours.pickle` & `atlantis-2023.6.21/atlantis/data_files/svg_colours.pickle`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/data_files/x11_colours.pickle` & `atlantis-2023.6.21/atlantis/data_files/x11_colours.pickle`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/algebra/Matrix.py` & `atlantis-2023.6.21/atlantis/ds/algebra/Matrix.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/auto/_AutoML.py` & `atlantis-2023.6.21/atlantis/ds/auto/_AutoML.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..parallel_computing import Processor
 from ..parallel_computing import CrossValidationProject
-from ..validation import CrossValidation, TimeSeriesValidation, Scoreboard
-from ..validation import EstimatorRepository
+from ..old_validation import CrossValidation, TimeSeriesValidation, Scoreboard
+from ..old_validation import EstimatorRepository
 import multiprocess
 from pandas import DataFrame
 
 
 class AutoML:
 	def __init__(self):
 		"""
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/classification/ProbabilityClassifier.py` & `atlantis-2023.6.21/atlantis/ds/old_classification/ProbabilityClassifier.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/clustering/ClusteringOptimizer.py` & `atlantis-2023.6.21/atlantis/ds/clustering/ClusteringOptimizer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/clustering/KMeans.py` & `atlantis-2023.6.21/atlantis/ds/clustering/KMeans.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pandas import DataFrame as PandasDF, Series as PandasSeries, concat
 from sklearn.cluster import KMeans as SklearnKMeans
 from sklearn.metrics import silhouette_score
 
 from pyspark.sql import functions as f
 from pyspark.sql.types import DoubleType, StringType
 from pyspark.sql import DataFrame as SparkDF, Column as SparkColumn
-from pyspark.sql.window import Window
 from pyspark.ml.clustering import KMeans as SparkKMeans
 from pyspark.ml.feature import VectorAssembler
 from pyspark.ml.evaluation import ClusteringEvaluator
 from pyspark.ml.linalg import Vectors
 
 from scipy.spatial.distance import cdist
 import numpy as np
@@ -219,70 +218,100 @@
 	@property
 	def _spark_cluster_centers(self):
 		"""
 		:rtype: list[np_array]
 		"""
 		return self._spark_model.clusterCenters()
 
-	def _transform_spark(self, X, prefix='distance_', keep_columns=False):
-		"""
-		:type X: SparkDF
-		:type prefix: str
-		:rtype: SparkDF
-		"""
+	@staticmethod
+	def _get_keep_columns(X, keep_columns):
+		if isinstance(keep_columns, str):
+			keep_columns = [keep_columns]
+		elif isinstance(keep_columns, list):
+			pass
+		elif keep_columns == True:
+			keep_columns = list(X.columns)
+		elif keep_columns == False or keep_columns is None:
+			keep_columns = []
+		else:
+			raise TypeError(f'keep_columns of type {type(keep_columns)} is not supported!')
+		return keep_columns
+
+	def _transform_and_predict_spark(self, X, add_distances, keep_prediction, distance_prefix, cluster_prefix, keep_columns):
 		assembled = self._spark_assembler.transform(X)
-		centers = self.cluster_centers
+		transformed = self._spark_model.transform(assembled)
 
-		@f.udf(DoubleType())
-		def _get_distance(features, cluster):
-			"""
-			:type features: np_array
-			:rtype: SparkColumn
-			"""
-			center = centers[cluster]
-			return float(Vectors.squared_distance(features, center) ** 0.5)
+		keep_columns = self._get_keep_columns(X=X, keep_columns=keep_columns)
+		transformed = transformed.select(*[
+			col for col in transformed.columns
+			if (col in transformed.columns and col not in X.columns) or col in keep_columns
+		])
 
-		if isinstance(keep_columns, (list, str)):
-			if isinstance(keep_columns, str):
-				keep_columns = [keep_columns]
-		elif keep_columns:
-			keep_columns = [col for col in X.columns if col != 'features']
+		if add_distances:
+			centers = self.cluster_centers
+
+			@f.udf(DoubleType())
+			def _get_distance(features, cluster):
+				"""
+				:type features: np_array
+				:rtype: SparkColumn
+				"""
+				center = centers[cluster]
+				return float(Vectors.squared_distance(features, center) ** 0.5)
+
+			transformed = (
+				transformed
+				.select(*transformed.columns, *[
+					_get_distance('features', f.lit(cluster)).alias(f'{distance_prefix}{cluster + 1}')
+					for cluster in range(len(centers))
+				])
+			)
+
+		transformed = transformed.drop('features')
+
+		if not keep_prediction:
+			transformed = transformed.drop('prediction')
 		else:
-			keep_columns = []
+			@f.udf(StringType())
+			def _convert_prediction_to_string(x):
+				return f'{cluster_prefix}{x + 1}'
+
+			transformed = transformed.withColumn('prediction', _convert_prediction_to_string('prediction'))
 
-		transformed = assembled.select(*keep_columns, *[
-			_get_distance('features', f.lit(cluster)).alias(f'{prefix}{cluster + 1}')
-			for cluster in range(len(centers))
-		])
 		return transformed
 
-	def _predict_spark(self, X, prefix='cluster_', keep_columns=False):
+	def _predict_spark(self, X, prefix='cluster_', keep_columns=False, add_distance=False, distance_prefix='distance_'):
 		"""
 		:type X: SparkDF
+		:type prefix: str
+		:type keep_columns: bool or NoneType or list[str] or str
+		:type add_distance: bool
+		:type distance_prefix: str
 		:rtype: SparkDF
 		"""
-		assembled = self._spark_assembler.transform(X)
-		result = self._spark_model.transform(assembled)
-
-		@f.udf(StringType())
-		def _convert_prediction_to_string(x):
-			return f'{prefix}{x + 1}'
-		result = result.withColumn('prediction', _convert_prediction_to_string('prediction'))
-
-		if keep_columns:
-			if isinstance(keep_columns, str):
-				keep_columns = [keep_columns]
+		return self._transform_and_predict_spark(
+			X=X, cluster_prefix=prefix, keep_columns=keep_columns, keep_prediction=True,
+			add_distances=add_distance, distance_prefix=distance_prefix
+		)
 
-			if isinstance(keep_columns, list):
-				columns = keep_columns + ['prediction']
-				return result.select(*columns)
-			else:
-				return result.drop('features')
-		else:
-			return result.select('prediction')
+	def _transform_spark(
+			self, X, prefix='distance_', keep_columns=False, add_prediction=False, cluster_prefix='cluster_'
+	):
+		"""
+		:type X: SparkDF
+		:type prefix: str
+		:type keep_columns: bool or NoneType or list[str] or str
+		:type add_prediction: bool
+		:type cluster_prefix: str
+		:rtype: SparkDF
+		"""
+		return self._transform_and_predict_spark(
+			X=X, distance_prefix=prefix, keep_columns=keep_columns, add_distances=True,
+			keep_prediction=add_prediction, cluster_prefix=cluster_prefix
+		)
 
 	# GENERAL METHODS #
 
 	def fit(self, X):
 		"""
 		:type X: SparkDF or PandasDF
 		"""
@@ -314,15 +343,15 @@
 			return self._spark_cluster_centers
 		else:
 			return self._python_cluster_centers
 
 	def transform(self, X, keep_columns=False):
 		"""
 		:type X: SparkDF or PandasDF
-		:type keep_columns: bool
+		:type keep_columns: bool or list[str] or str
 		"""
 		if self._env == 'spark':
 			return self._transform_spark(X=X, keep_columns=keep_columns)
 
 		elif self._env == 'python':
 			return self._transform_python(X=X, keep_columns=keep_columns)
 
@@ -362,30 +391,26 @@
 
 	def transform_and_predict(self, X, keep_columns=False):
 		"""
 		:type X: PandasDF or SparkDF
 		:type keep_columns: bool or str or list[str]
 		:rtype: PandasDF
 		"""
-		transformed = self.transform(X=X, keep_columns=keep_columns)
-		predictions = self.predict(X=X, return_dataframe=False, keep_columns=False)
-
-		if self._env == 'python':
-			transformed['prediction'] = predictions
 
-		elif self._env == 'spark':
-			w = Window.orderBy(f.monotonically_increasing_id())
-			transformed = transformed.withColumn('_index', f.row_number().over(w))
-			predictions = predictions.withColumn('_index', f.row_number().over(w))
-			transformed = transformed.join(predictions, on='_index', how='inner').drop('_index')
+		if isinstance(X, SparkDF):
+			return self._transform_and_predict_spark(
+				X=X, add_distances=True, keep_prediction=True, distance_prefix='distance_', cluster_prefix='cluster_',
+				keep_columns=keep_columns
+			)
 
 		else:
-			raise RuntimeError(f'unknown environment {self._env}')
-
-		return transformed
+			transformed = self._transform_python(X=X, keep_columns=True, prefix='distance_')
+			keep_columns = self._get_keep_columns(X=X, keep_columns=keep_columns)
+			keep_columns = keep_columns + [col for col in transformed.columns if col not in X.columns]
+			return self._predict_python(X=transformed, return_dataframe=True, keep_columns=keep_columns)
 
 	@property
 	def n_clusters(self):
 		"""
 		:rtype: int
 		"""
 		return self._n_clusters
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/ensemble/Ensemble.py` & `atlantis-2023.6.21/atlantis/ds/ensemble/Ensemble.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/ensemble/PrincipalComponentModelFactory.py` & `atlantis-2023.6.21/atlantis/ds/ensemble/PrincipalComponentModelFactory.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/entropy/_get_entropy.py` & `atlantis-2023.6.21/atlantis/ds/entropy/_get_entropy.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_classification.py` & `atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_classification.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_mutliclass_classification.py` & `atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_mutliclass_classification.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/evaluation/_evaluate_regression.py` & `atlantis-2023.6.21/atlantis/ds/evaluation/_evaluate_regression.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/evaluation/_get_confusion_matrix_df.py` & `atlantis-2023.6.21/atlantis/ds/evaluation/_get_confusion_matrix_df.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/feature_importance/InfluenceSimulator.py` & `atlantis-2023.6.21/atlantis/ds/feature_importance/InfluenceSimulator.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_coefficients.py` & `atlantis-2023.6.21/atlantis/ds/feature_importance/_get_coefficients.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_feature_importances.py` & `atlantis-2023.6.21/atlantis/ds/feature_importance/_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/feature_importance/_get_model_influence.py` & `atlantis-2023.6.21/atlantis/ds/feature_importance/_get_model_influence.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation/Imputer.py` & `atlantis-2023.6.21/atlantis/ds/imputation/Imputer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation/SingleColumnImputer.py` & `atlantis-2023.6.21/atlantis/ds/imputation/SingleColumnImputer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation/_find_good_columns.py` & `atlantis-2023.6.21/atlantis/ds/imputation/_find_good_columns.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation2/DataImputer.py` & `atlantis-2023.6.21/atlantis/ds/imputation2/DataImputer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation2/Imputer.py` & `atlantis-2023.6.21/atlantis/ds/imputation2/Imputer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation2/_ColumnImputer.py` & `atlantis-2023.6.21/atlantis/ds/imputation2/_ColumnImputer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.linear_model import LinearRegression
 from sklearn.tree import DecisionTreeClassifier
 from pandas import concat
-from ..validation import CrossValidation
+from ..old_validation import CrossValidation
 from ._fill_na_and_flag import NaFillerFlagger
 ROW_NUM_COLUMN = '_imputer_row_number_'
 
 
 class ColumnImputer:
 	def __init__(
 			self, column, estimators, helper_columns=None, cross_validation=None,
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/imputation2/_fill_na_and_flag.py` & `atlantis-2023.6.21/atlantis/ds/imputation2/_fill_na_and_flag.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_DataSlice.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_DataSlice.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Processor.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_Processor.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Project.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_Project.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_Task.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_Task.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_TimeEstimate.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_TimeEstimate.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_get_data_from_namespace.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_get_data_from_namespace.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/_worker.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/_worker.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_CrossValidationProject.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_CrossValidationProject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from ...validation import Validation
+from ...old_validation import Validation
 from .._DataSlice import TrainingTestSlice
 from ._LearningProject import LearningProject
 from ._LearningTask import LearningTask
 from pandas import DataFrame
 
 
 class CrossValidationProject(LearningProject):
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_LearningProject.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_LearningProject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pandas import concat, DataFrame
 from numpy import random
 
 from .._Project import Project
 from ...evaluation import evaluate_regression, evaluate_classification
 from .._DataSlice import TrainingTestSlice
-from ...validation import Scoreboard, TrainingTestContainer
+from ...old_validation import Scoreboard, TrainingTestContainer
 from ._LearningTask import LearningTask
 from ....collections.OrderedSet import OrderedSet
 
 
 class LearningProject(Project):
 	def __init__(
 			self, name, y_column, problem_type, x_columns=None,
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_LearningTask.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_LearningTask.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/parallel_computing/learning/_example_1.py` & `atlantis-2023.6.21/atlantis/ds/parallel_computing/learning/_example_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from atlantis.ds.synthetic_data import create_data
-from atlantis.ds.validation import CrossValidation
-from atlantis.ds.validation import EstimatorRepository
+from atlantis.ds.old_validation import CrossValidation
+from atlantis.ds.old_validation import EstimatorRepository
 from atlantis.ds.parallel_computing import Processor
 
 from sklearn.linear_model import LinearRegression, Lasso
 from sklearn.ensemble import RandomForestRegressor
 
 repository = EstimatorRepository()
 repository.append(RandomForestRegressor, {'n_estimators': 100, 'n_jobs': 1, 'max_depth': [6, 12, 24]})
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/prediction/PredictorBase.py` & `atlantis-2023.6.21/atlantis/ds/prediction/PredictorBase.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/Normalizer.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/Normalizer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/OneHotEncoder.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/PCA.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/PCA.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,32 +63,35 @@
 			self._assembler = VectorAssembler(inputCols=self._columns, outputCol='features')
 			assembled = self._assembler.transform(X).select('features')
 			self._pca = SparkPCA(k=self._k, inputCol='features', outputCol='pca_features').fit(assembled)
 
 		self._fitted = True
 		return self
 
-	def transform(self, X, return_vector=False):
+	def transform(self, X, return_vector=False, keep_columns=False):
 		"""
 		:type X: DataFrame
 		:type return_vector: bool
 		:param return_vector: True: the vector column will be returned. False: the vector column will be disassembled.
 		:rtype: DataFrame
 		"""
 		if not self._fitted:
 			self.fit(X=X)
 
 		assert_has_columns(X, self._columns)
 
 		if self._scale:
-			scaled = self._scaler.transform(X=X, return_vector=True)
+			scaled = self._scaler.transform(X=X, return_vector=True, keep_columns=keep_columns)
 		else:
-			scaled = self._assembler.transform(X).select(
-				'features', *[col for col in X.columns if col not in self._columns]
-			)
+			if keep_columns:
+				columns_to_keep = list(X.columns)
+			else:
+				columns_to_keep = [col for col in X.columns if col not in self._columns]
+
+			scaled = self._assembler.transform(X).select('features', *columns_to_keep)
 
 		transformed = self._pca.transform(scaled).drop('features', 'scaled_features')
 		if return_vector:
 			return transformed
 
 		else:
 			self._pca_columns = [f'pca_{i}' for i in range(1, self._k + 1)]
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/Polynomial.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/Polynomial.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/Scaler.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/Scaler.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,29 +46,34 @@
         self._scaler = StandardScaler(
             inputCol='features', outputCol='scaled_features',
             withMean=self._with_mean, withStd=self._with_sd
         ).fit(assembled)
         self._fitted = True
         return self
 
-    def transform(self, X, return_vector=False):
+    def transform(self, X, return_vector=False, keep_columns=False):
         """
         :type X: DataFrame
         :type return_vector: bool
         :param return_vector: if True, the vector column will be returned
                             if False, the vector column will be disassembled
         :rtype: DataFrame
         """
         if not self._fitted:
             self.fit(X)
 
         assert_has_columns(X, columns=self._columns)
 
+        if keep_columns:
+            columns_to_keep = list(X.columns)
+        else:
+            columns_to_keep = [col for col in X.columns if col not in self._columns]
+
         assembled = self._assembler.transform(X).select(
-            'features', *[col for col in X.columns if col not in self._columns]
+            'features', *columns_to_keep
         )
         df_scaled = self._scaler.transform(assembled).drop('features')
         if return_vector:
             return df_scaled
         else:
             names = [f'{col}_scaled' for col in self._columns]
             return disassemble(df_scaled, column='scaled_features', names=names, drop=True)
```

### Comparing `atlantis-2022.9.7.1/atlantis/ds/preprocessing/disassemble.py` & `atlantis-2023.6.21/atlantis/ds/preprocessing/disassemble.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/RegularizedLeastSquares.py` & `atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/RegularizedLeastSquares.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForNumpy.py` & `atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForNumpy.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForPandas.py` & `atlantis-2023.6.21/atlantis/ds/regression/regularized_least_squares_regression/_RegularizedLeastSquaresForPandas.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/sampling/UpSampler.py` & `atlantis-2023.6.21/atlantis/ds/sampling/UpSampler.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/sampling/_balance_sample.py` & `atlantis-2023.6.21/atlantis/ds/sampling/_balance_sample.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/sampling/_sample_by_id.py` & `atlantis-2023.6.21/atlantis/ds/sampling/_sample_by_id.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/sampling/_sample_per_group.py` & `atlantis-2023.6.21/atlantis/ds/sampling/_sample_per_group.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/sampling/_split_data.py` & `atlantis-2023.6.21/atlantis/ds/sampling/_split_data.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/testing/assert_has_columns.py` & `atlantis-2023.6.21/atlantis/ds/testing/assert_has_columns.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_CrossValidation.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_CrossValidation.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_DataContainer.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_DataContainer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_EstimatorRace.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_EstimatorRace.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_EstimatorRepository.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_EstimatorRepository.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_Evaluation.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_Evaluation.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_Result.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_Result.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_Scoreboard.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_Scoreboard.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_TrainingTestContainer.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_TrainingTestContainer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_ValidationContainer.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_ValidationContainer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_get_cross_validation.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_get_cross_validation.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_get_training_test.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_get_training_test.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_split_data.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_split_data.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/validation/_train_and_test.py` & `atlantis-2023.6.21/atlantis/ds/old_validation/_train_and_test.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/NearestFinder.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/NearestFinder.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/NullReplacer.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/NullReplacer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/__init__.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_apply_function.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_apply_function.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_bring_to_front.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_bring_to_front.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_drop_bad_columns.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_drop_bad_columns.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_fill_na.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_fill_na.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_find_values.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_find_values.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_get_string_columns.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_get_string_columns.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_imputate_with_regression.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_imputate_with_regression.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_join_and_preserve_types.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_join_and_preserve_types.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_join_wisely.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_join_wisely.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_long_to_wide.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_long_to_wide.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_min_max.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_min_max.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_read_excel.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_read_excel.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_select_extreme.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_select_extreme.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_split_rows.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_split_rows.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/_standardize_columns.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/_standardize_columns.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/get_modified_zscore.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/get_modified_zscore.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/melt.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/melt.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/ds/wrangling/union.py` & `atlantis-2023.6.21/atlantis/ds/wrangling/union.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/exceptions/_datascience_exceptions.py` & `atlantis-2023.6.21/atlantis/exceptions/_datascience_exceptions.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/functions/_exit_after.py` & `atlantis-2023.6.21/atlantis/functions/_exit_after.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/hash/__init__.py` & `atlantis-2023.6.21/atlantis/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/BaseController.py` & `atlantis-2023.6.21/atlantis/multiprocessing/BaseController.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/Controller.py` & `atlantis-2023.6.21/atlantis/multiprocessing/Controller.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/JobController.py` & `atlantis-2023.6.21/atlantis/multiprocessing/JobController.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/ProcessController.py` & `atlantis-2023.6.21/atlantis/multiprocessing/ProcessController.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/SimpleController.py` & `atlantis-2023.6.21/atlantis/multiprocessing/SimpleController.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/_Task.py` & `atlantis-2023.6.21/atlantis/multiprocessing/_Task.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/_WorkerReport.py` & `atlantis-2023.6.21/atlantis/multiprocessing/_WorkerReport.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/_do_task.py` & `atlantis-2023.6.21/atlantis/multiprocessing/_do_task.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/_supervise.py` & `atlantis-2023.6.21/atlantis/multiprocessing/_supervise.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/validation/ValidationController.py` & `atlantis-2023.6.21/atlantis/multiprocessing/validation/ValidationController.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/multiprocessing/validation/_validate.py` & `atlantis-2023.6.21/atlantis/multiprocessing/validation/_validate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pandas import DataFrame
 
-from ...ds.validation import ValidationContainer
-from ...ds.validation._train_and_test import train_and_test
+from ...ds.old_validation import ValidationContainer
+from ...ds.old_validation._train_and_test import train_and_test
 from .. import ProcessController
 from ...time.progress import ProgressBar
 
 from time import sleep
 
 
 def validate(
```

### Comparing `atlantis-2022.9.7.1/atlantis/text/_convert_camel_to_snake.py` & `atlantis-2023.6.21/atlantis/text/_convert_camel_to_snake.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/text/_wrap.py` & `atlantis-2023.6.21/atlantis/text/_wrap.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/__init__.py` & `atlantis-2023.6.21/atlantis/time/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/YearMonth.py` & `atlantis-2023.6.21/atlantis/time/date/YearMonth.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/YearQuarter.py` & `atlantis-2023.6.21/atlantis/time/date/YearQuarter.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/__init__.py` & `atlantis-2023.6.21/atlantis/time/date/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/add_time.py` & `atlantis-2023.6.21/atlantis/time/date/add_time.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/get_date_part.py` & `atlantis-2023.6.21/atlantis/time/date/get_date_part.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/get_first_day_of_month.py` & `atlantis-2023.6.21/atlantis/time/date/get_first_day_of_month.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/get_month.py` & `atlantis-2023.6.21/atlantis/time/date/get_month.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/date/parse_date.py` & `atlantis-2023.6.21/atlantis/time/date/parse_date.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/estimate/Estimator.py` & `atlantis-2023.6.21/atlantis/time/estimate/Estimator.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/estimate/Measurement.py` & `atlantis-2023.6.21/atlantis/time/estimate/Measurement.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/estimate/create_arguments.py` & `atlantis-2023.6.21/atlantis/time/estimate/create_arguments.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/numbers/FlexibleNumber.py` & `atlantis-2023.6.21/atlantis/time/numbers/FlexibleNumber.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/numbers/NumberPart.py` & `atlantis-2023.6.21/atlantis/time/numbers/NumberPart.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/progress/Iterable.py` & `atlantis-2023.6.21/atlantis/time/progress/Iterable.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/progress/ProgressBar.py` & `atlantis-2023.6.21/atlantis/time/progress/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/progress/_map.py` & `atlantis-2023.6.21/atlantis/time/progress/_map.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/MeasurementSet.py` & `atlantis-2023.6.21/atlantis/time/time/MeasurementSet.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/TimeMeasurement.py` & `atlantis-2023.6.21/atlantis/time/time/TimeMeasurement.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/Timer.py` & `atlantis-2023.6.21/atlantis/time/time/Timer.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/_Job.py` & `atlantis-2023.6.21/atlantis/time/time/_Job.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/convert.py` & `atlantis-2023.6.21/atlantis/time/time/convert.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/get_elapsed.py` & `atlantis-2023.6.21/atlantis/time/time/get_elapsed.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis/time/time/measure.py` & `atlantis-2023.6.21/atlantis/time/time/measure.py`

 * *Files identical despite different names*

### Comparing `atlantis-2022.9.7.1/atlantis.egg-info/PKG-INFO` & `atlantis-2023.6.21/atlantis.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,110 @@
 Metadata-Version: 2.1
 Name: atlantis
-Version: 2022.9.7.1
+Version: 2023.6.21
 Summary: Python library for simplifying data science
 Home-page: https://github.com/idin/atlantis
 Author: Idin
 Author-email: py@idin.ca
 License: MIT
-Description: # ***Atlantis***
-        ***Atlantis*** is a Python library for simplifying programming with Python for data science.
-        
-        # Installation
-        You can just use pip to install Atlantis:
-        
-        `pip install atlantis`
-        
-        # Modules
-        
-        - [***collections***](#collections) helps with working with collections.
-        - [***colour***](about_colour.md) simplifies using colours.
-        - [***ds (datascience)***](#ds-data-science) provides tools for:
-          - data wrangling, 
-          - validation, 
-          - tuning,
-          - sampling, 
-          - evaluation,
-          - clustering, and 
-          - parallel processing of machine learning models.
-        - [***functions***](about_functions.md) manages higher order functions.
-        - [***hash***](about_hash.md) simplifies and standardizes hashing.
-        - [***text***](about_text.md) makes working with texts and strings easy.
-        - [***time***](about_time.md) 
-          - provides methods for interacting with time and date as well as 
-          - progress bars
-          
-        ## *collections*
-        This module of the package [***atlantis***](README.md) helps with working with collections.
-        
-        ### *`flatten`*
-        ```python
-        from atlantis.collections import flatten
-        flatten([1, 2, [3, 4, [5, 6], 7], 8])
-        ```
-        returns: `[1, 2, 3, 4, 5, 6, 7, 8]`
-        
-        ### *`List`*
-        This class inherits from Python's list class but implements a few 
-        additional functionalities.
-        
-        ```python
-        from atlantis.collections import List
-        l = List(1, 2, 3, 4, 2, [1, 2], [1, 2])
-        ```
-        
-        Flattening: 
-        ```python
-        l.flatten()
-        >>> List: [1, 2, 3, 4, 2, 1, 2, 1, 2]
-        ```
-        
-        Finding duplicates:
-        ```python
-        l.get_duplicates()
-        >>> List: [2, List: [1, 2]]
-        ```
-        **Note:** the ***list*** elements of a ***List*** automatically get converted to ***Lists***, recursively.
-        
-        ## *ds* (Data Science)
-        This module provides data science tools for:
-        - data wrangling, 
-        - validation, 
-        - tuning,
-        - sampling, 
-        - evaluation,
-        - clustering, and 
-        - parallel processing of machine learning models.
-        
-        ### *KMeans* Clustering
-        I have used the `KMeans` class from both *sklearn* and that of *pyspark* and was frustrated 
-        by two problems: (a) even though the two classes do exactly the same thing their interfaces
-        are vastly different and (b) some of the simplest operations are very hard to do with 
-        both classes. I solved this problem by creating my own `KMeans` class that is a wrapper 
-        aroung both of those classes and uses the appropriate one automatically without 
-        complicating it for the data scientist programmer. 
-        
-        #### Usage
-        
-        ```python
-        from atlantis.ds.clustering import KMeans
-        
-        kmeans = KMeans(n_clusters=3, n_jobs=10)
-        kmeans.fit(X=X)
-        
-        predictions = kmeans.predict(X=X)
-        transformed_x = kmeans.transform(X=X)
-        ```
-        
-        ### Clustering Optimization
-        
-        #### Usage
-        ```python
-        from atlantis.ds.clustering import ClusteringOptimizer
-        
-        clustering_optimizer = ClusteringOptimizer(min_k=2, max_k=16, n_jobs=10)
-        clustering_optimizer.fit(X=X)
-        print(f'best number of clusters: {clustering_optimizer.optimal_number_of_clusters}')
-        ```
-Platform: UNKNOWN
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+
+# ***Atlantis***
+***Atlantis*** is a Python library for simplifying programming with Python for data science.
+
+# Installation
+You can just use pip to install Atlantis:
+
+`pip install atlantis`
+
+# Modules
+
+- [***collections***](#collections) helps with working with collections.
+- [***colour***](about_colour.md) simplifies using colours.
+- [***ds (datascience)***](#ds-data-science) provides tools for:
+  - data wrangling, 
+  - validation, 
+  - tuning,
+  - sampling, 
+  - evaluation,
+  - clustering, and 
+  - parallel processing of machine learning models.
+- [***functions***](about_functions.md) manages higher order functions.
+- [***hash***](about_hash.md) simplifies and standardizes hashing.
+- [***text***](about_text.md) makes working with texts and strings easy.
+- [***time***](about_time.md) 
+  - provides methods for interacting with time and date as well as 
+  - progress bars
+  
+## *collections*
+This module of the package [***atlantis***](README.md) helps with working with collections.
+
+### *`flatten`*
+```python
+from atlantis.collections import flatten
+flatten([1, 2, [3, 4, [5, 6], 7], 8])
+```
+returns: `[1, 2, 3, 4, 5, 6, 7, 8]`
+
+### *`List`*
+This class inherits from Python's list class but implements a few 
+additional functionalities.
+
+```python
+from atlantis.collections import List
+l = List(1, 2, 3, 4, 2, [1, 2], [1, 2])
+```
+
+Flattening: 
+```python
+l.flatten()
+>>> List: [1, 2, 3, 4, 2, 1, 2, 1, 2]
+```
+
+Finding duplicates:
+```python
+l.get_duplicates()
+>>> List: [2, List: [1, 2]]
+```
+**Note:** the ***list*** elements of a ***List*** automatically get converted to ***Lists***, recursively.
+
+## *ds* (Data Science)
+This module provides data science tools for:
+- data wrangling, 
+- validation, 
+- tuning,
+- sampling, 
+- evaluation,
+- clustering, and 
+- parallel processing of machine learning models.
+
+### *KMeans* Clustering
+I have used the `KMeans` class from both *sklearn* and that of *pyspark* and was frustrated 
+by two problems: (a) even though the two classes do exactly the same thing their interfaces
+are vastly different and (b) some of the simplest operations are very hard to do with 
+both classes. I solved this problem by creating my own `KMeans` class that is a wrapper 
+aroung both of those classes and uses the appropriate one automatically without 
+complicating it for the data scientist programmer. 
+
+#### Usage
+
+```python
+from atlantis.ds.clustering import KMeans
+
+kmeans = KMeans(n_clusters=3, n_jobs=10)
+kmeans.fit(X=X)
+
+predictions = kmeans.predict(X=X)
+transformed_x = kmeans.transform(X=X)
+```
+
+### Clustering Optimization
+
+#### Usage
+```python
+from atlantis.ds.clustering import ClusteringOptimizer
+
+clustering_optimizer = ClusteringOptimizer(min_k=2, max_k=16, n_jobs=10)
+clustering_optimizer.fit(X=X)
+print(f'best number of clusters: {clustering_optimizer.optimal_number_of_clusters}')
+```
```

### Comparing `atlantis-2022.9.7.1/atlantis.egg-info/SOURCES.txt` & `atlantis-2023.6.21/atlantis.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,19 @@
 atlantis/data_files/svg_colours.pickle
 atlantis/data_files/x11_colours.pickle
 atlantis/ds/__init__.py
 atlantis/ds/algebra/Matrix.py
 atlantis/ds/algebra/__init__.py
 atlantis/ds/auto/_AutoML.py
 atlantis/ds/auto/__init__.py
-atlantis/ds/classification/ProbabilityClassifier.py
+atlantis/ds/classification/Classifier.py
+atlantis/ds/classification/Encoder.py
+atlantis/ds/classification/EnsembleClassifier.py
 atlantis/ds/classification/__init__.py
+atlantis/ds/classification/measure_performance.py
 atlantis/ds/clustering/ClusteringOptimizer.py
 atlantis/ds/clustering/KMeans.py
 atlantis/ds/clustering/__init__.py
 atlantis/ds/ensemble/Ensemble.py
 atlantis/ds/ensemble/PrincipalComponentModelFactory.py
 atlantis/ds/ensemble/__init__.py
 atlantis/ds/entropy/__init__.py
@@ -66,14 +69,34 @@
 atlantis/ds/imputation/_find_good_columns.py
 atlantis/ds/imputation/exceptions/__init__.py
 atlantis/ds/imputation2/DataImputer.py
 atlantis/ds/imputation2/Imputer.py
 atlantis/ds/imputation2/_ColumnImputer.py
 atlantis/ds/imputation2/__init__.py
 atlantis/ds/imputation2/_fill_na_and_flag.py
+atlantis/ds/old_classification/ProbabilityClassifier.py
+atlantis/ds/old_classification/RandomForestClassifier.py
+atlantis/ds/old_classification/__init__.py
+atlantis/ds/old_classification/oldClassifier.py
+atlantis/ds/old_classification/pyspark_classifier.py
+atlantis/ds/old_classification/test delete.py
+atlantis/ds/old_validation/_CrossValidation.py
+atlantis/ds/old_validation/_DataContainer.py
+atlantis/ds/old_validation/_EstimatorRace.py
+atlantis/ds/old_validation/_EstimatorRepository.py
+atlantis/ds/old_validation/_Evaluation.py
+atlantis/ds/old_validation/_Result.py
+atlantis/ds/old_validation/_Scoreboard.py
+atlantis/ds/old_validation/_TrainingTestContainer.py
+atlantis/ds/old_validation/_ValidationContainer.py
+atlantis/ds/old_validation/__init__.py
+atlantis/ds/old_validation/_get_cross_validation.py
+atlantis/ds/old_validation/_get_training_test.py
+atlantis/ds/old_validation/_split_data.py
+atlantis/ds/old_validation/_train_and_test.py
 atlantis/ds/parallel_computing/_DataSlice.py
 atlantis/ds/parallel_computing/_Processor.py
 atlantis/ds/parallel_computing/_Project.py
 atlantis/ds/parallel_computing/_Task.py
 atlantis/ds/parallel_computing/_TimeEstimate.py
 atlantis/ds/parallel_computing/__init__.py
 atlantis/ds/parallel_computing/_get_data_from_namespace.py
@@ -100,39 +123,33 @@
 atlantis/ds/sampling/Sampler.py
 atlantis/ds/sampling/UpSampler.py
 atlantis/ds/sampling/__init__.py
 atlantis/ds/sampling/_balance_sample.py
 atlantis/ds/sampling/_sample_by_id.py
 atlantis/ds/sampling/_sample_per_group.py
 atlantis/ds/sampling/_split_data.py
-atlantis/ds/slicing/DataSlice.py
-atlantis/ds/slicing/SliceTemplate.py
 atlantis/ds/slicing/__init__.py
-atlantis/ds/slicing/_get_rows.py
+atlantis/ds/slicing/_get_random_split_without_hashing.py
+atlantis/ds/slicing/get_random_by_object.py
+atlantis/ds/slicing/get_random_split.py
+atlantis/ds/slicing/label_random_split.py
+atlantis/ds/supervised_learning/PySparkRandomForestClassifier.py
+atlantis/ds/supervised_learning/_BaseSupervisedModel.py
+atlantis/ds/supervised_learning/_PySparkModel.py
+atlantis/ds/supervised_learning/__init__.py
 atlantis/ds/synthetic_data/__init__.py
 atlantis/ds/synthetic_data/_create_data.py
 atlantis/ds/testing/__init__.py
 atlantis/ds/testing/assert_columns_are_unique.py
 atlantis/ds/testing/assert_has_columns.py
 atlantis/ds/tuning/__init__.py
 atlantis/ds/tuning/_tune.py
-atlantis/ds/validation/_CrossValidation.py
-atlantis/ds/validation/_DataContainer.py
-atlantis/ds/validation/_EstimatorRace.py
-atlantis/ds/validation/_EstimatorRepository.py
-atlantis/ds/validation/_Evaluation.py
-atlantis/ds/validation/_Result.py
-atlantis/ds/validation/_Scoreboard.py
-atlantis/ds/validation/_TrainingTestContainer.py
-atlantis/ds/validation/_ValidationContainer.py
+atlantis/ds/validation/CrossValidation.py
 atlantis/ds/validation/__init__.py
-atlantis/ds/validation/_get_cross_validation.py
-atlantis/ds/validation/_get_training_test.py
-atlantis/ds/validation/_split_data.py
-atlantis/ds/validation/_train_and_test.py
+atlantis/ds/validation/validate_classifier.py
 atlantis/ds/wrangling/NearestFinder.py
 atlantis/ds/wrangling/NullReplacer.py
 atlantis/ds/wrangling/__init__.py
 atlantis/ds/wrangling/_apply_function.py
 atlantis/ds/wrangling/_as_numeric.py
 atlantis/ds/wrangling/_as_string.py
 atlantis/ds/wrangling/_bring_to_front.py
```

### Comparing `atlantis-2022.9.7.1/setup.py` & `atlantis-2023.6.21/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 def readme():
 	with open('./README.md') as f:
 		return f.read()
 
 
 setup(
 	name='atlantis',
-	version='2022.9.7.1',
+	version='2023.6.21',
 	description='Python library for simplifying data science',
 	long_description=readme(),
 	long_description_content_type='text/markdown',
 	url='https://github.com/idin/atlantis',
 	author='Idin',
 	author_email='py@idin.ca',
 	license='MIT',
 	packages=find_packages(exclude=("jupyter", ".idea", ".git", "data_files")),
 	install_requires=[
 		'base32hex', 'geopy', 'pandas', 'joblib', 'numpy', 'sklearn', 'multiprocess', 'pyspark', 'matplotlib',
-		'scipy', 'tldextract', 'validators'
+		'scipy', 'tldextract', 'validators', 'amazonian'
 	],
 	package_data={'atlantis': ['data_files/*.pickle']},
 	python_requires='~=3.6',
 	zip_safe=False
 )
```

