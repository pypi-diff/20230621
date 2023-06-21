# Comparing `tmp/scikit-rmt-0.5.0.tar.gz` & `tmp/scikit-rmt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.5.0.tar", last modified: Sat May  6 16:07:34 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.6.0.tar", last modified: Wed Jun 21 15:28:57 2023, max compression
```

## Comparing `scikit-rmt-0.5.0.tar` & `scikit-rmt-0.6.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.811442 scikit-rmt-0.5.0/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.5.0/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.5.0/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.5.0/CITATION.cff
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.5.0/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.5.0/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.5.0/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    19527 2023-05-06 16:07:34.812171 scikit-rmt-0.5.0/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    15299 2023-05-06 14:59:09.000000 scikit-rmt-0.5.0/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.5.0/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.654809 scikit-rmt-0.5.0/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.5.0/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1274 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.689918 scikit-rmt-0.5.0/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.5.0/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2021-05-10 19:43:36.000000 scikit-rmt-0.5.0/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.5.0/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.5.0/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.5.0/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.5.0/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.5.0/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.5.0/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.5.0/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       22 2021-05-14 17:37:20.000000 scikit-rmt-0.5.0/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.697134 scikit-rmt-0.5.0/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    19527 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1727 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       23 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-05-06 16:07:34.814241 scikit-rmt-0.5.0/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.710031 scikit-rmt-0.5.0/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.5.0/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-05-06 15:21:13.000000 scikit-rmt-0.5.0/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.714296 scikit-rmt-0.5.0/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.5.0/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.5.0/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.5.0/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.726109 scikit-rmt-0.5.0/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.793978 scikit-rmt-0.5.0/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)     1256 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     9331 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    12876 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    14169 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    33491 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/law.py
--rw-r--r--   0 santorum   (501) staff       (20)    13192 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    21317 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/plot_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.807378 scikit-rmt-0.5.0/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     4937 2021-05-02 16:51:08.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    11902 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    18193 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     5040 2023-03-18 23:10:48.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    19622 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_plot_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14644 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    15746 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.810743 scikit-rmt-0.5.0/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.5.0/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2705 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/tutorial/plot_0_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)    10227 2023-05-06 13:37:21.000000 scikit-rmt-0.5.0/tutorial/plot_1_spectral_laws.py
--rw-r--r--   0 santorum   (501) staff       (20)     8822 2023-05-06 12:57:57.000000 scikit-rmt-0.5.0/tutorial/plot_2_plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.597631 scikit-rmt-0.6.0/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.6.0/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.6.0/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.6.0/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.6.0/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.6.0/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.6.0/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-06-21 15:28:57.598713 scikit-rmt-0.6.0/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.6.0/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.545699 scikit-rmt-0.6.0/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.6.0/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.6.0/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.558401 scikit-rmt-0.6.0/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.6.0/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2155 2021-05-10 19:43:36.000000 scikit-rmt-0.6.0/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.6.0/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.6.0/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.6.0/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.6.0/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.6.0/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.6.0/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.6.0/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       66 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.566671 scikit-rmt-0.6.0/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       67 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-06-21 15:28:57.000000 scikit-rmt-0.6.0/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-06-21 15:28:57.602252 scikit-rmt-0.6.0/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.569092 scikit-rmt-0.6.0/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.6.0/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.572410 scikit-rmt-0.6.0/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.6.0/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.6.0/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.6.0/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.574926 scikit-rmt-0.6.0/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.6.0/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.585824 scikit-rmt-0.6.0/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9337 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/_base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13146 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14462 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13462 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    57283 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/spectral_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.592524 scikit-rmt-0.6.0/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)      287 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_base_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    11926 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    42495 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_spectral_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14668 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.6.0/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    16015 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-06-21 15:28:57.596444 scikit-rmt-0.6.0/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.6.0/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2706 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.6.0/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9176 2023-06-21 15:09:01.000000 scikit-rmt-0.6.0/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.5.0/LICENSE` & `scikit-rmt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/Makefile` & `scikit-rmt-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/PKG-INFO` & `scikit-rmt-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.5.0
+Version: 0.6.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.5.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
@@ -65,25 +65,52 @@
         ```
         You may need to use `pip3`.
         ```bash
         pip3 install scikit-rmt
         ```
         
         ### Global installation
-        Just install it using `pip`or `pip3`.
+        Just install it using `pip` or `pip3`.
         ```bash
         pip install scikit-rmt
         ```
         
         ### Requirements
         *scikit-rmt* depends on the following packages:
         * [numpy](https://github.com/numpy/numpy) - The fundamental package for scientific computing with Python
         * [matplotlib](https://github.com/matplotlib/matplotlib) - Plotting with Python
         * [scipy](https://github.com/scipy/scipy) - Scientific computation in Python
         
+        Check the pinned versions in the [requirements.txt](requirements.txt) file.
+        
+        ----------------
+        ## Main features
+        *scikit-rmt* provides support to analyze, study and simulate Random Matrix Theory properties and results:
+        * **Sampling** of the following random matrix ensembles:
+           * Gaussian Ensemble (GOE, GUE and GSE; for beta=1, 2 and 4 respectively): class `GaussianEnsemble`.
+           * Wishart Ensemble (WRE, WCE and WQE; for beta=1, 2 and 4 respectively): class `WishartEnsemble`.
+           * Manova Ensemble (MRE, MCE and MQE; for beta=1, 2 and 4 respectively): class `ManovaEnsemble`.
+           * Circular Ensemble (COE, CUE, CSE; for beta=1, 2 and 4 respectively): class `CircularEnsemble`.
+        * **Eigenvalue computation** for the previous ensembles using the class method `eigvals`.
+        * Computation of the **joint eigenvalue probability density function** given the random matrix eigenvalues, using the class method `joint_eigval_pdf`.
+        * Computation of the **empirical spectral histogram** by executing the class method `eigval_hist`.
+        * **Plotting of the empirical spectral histogram** using the class method `plot_eigval_hist`.
+        * Computation and plotting of the following **spectral laws** (`spectral_law` sub-module), including the calculation and plotting of the corresponding probability density functions (PDFs) and cumulative distribution functions (CDFs):
+           * **Wigner Semicircle law**: describes the limiting distribution of the eigenvalues of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `WignerSemicircleDistribution`.
+           * **Tracy-Widom law**: describes the limiting distribution of the largest eigenvalue of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `TracyWidomDistribution`.
+           * **Marchenko-Pastur law**: describes the limiting distribution of the eigenvalues of Wishart matrices (random matrices from the Wishart Ensemble). Implemented by class `MarchenkoPasturDistribution`.
+           * **Manova Spectrum law**: introduced and proved by K. W. Wachter (1980), it describes the limiting distribution of the eigenvalues of Manova matrices (random matrices from the Manova Ensemble). Implemented by class `ManovaSpectrumDistribution`.
+        * **Covariance matrix estimation** using different matrix smoothing and estimation methods (`covariance` module).
+           * Estimation of sample covariance matrix using `sample_estimator` function.
+           * Finite-sample Optimal (FSOpt) estimator by `fsopt_estimator` function.
+           * Empirical Bayesian estimator by `empirical_bayesian_estimator` function. Haff in *"Estimation of a covariance matrix under Stein’s loss"* (1985).
+           * Minimax estimator by `minimax_estimator` function 
+           * Linear shrinkage estimator by `linear_shrinkage_estimator` function. Ledoit and Wolf in *"A well-conditioned estimator for large-dimensional covariance matrices"* (2004).
+           * Analytical shrinkage estimator by `analytical_shrinkage_estimator` function. Ledoit and Wolf in *"Analytical nonlinear shrinkage of large-dimensional covariance matrices"* (2020).
+        
         
         -----------------
         ## A brief tutorial
         
         First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
         **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
         a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
@@ -132,14 +159,20 @@
         we can speed up histogramming procedure. The following graphical simulation using GOE matrices
         tries to illustrate it.
         ![Speed up by tridigonal forms](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/gauss_tridiag_sim.png)
         <!---
         <img src="imgs/gauss_tridiag_sim.png" width=820 height=370 alt="Speed up by tridigonal forms">
         -->
         
+        On the other hand, for all the supported ensembles, the **joint eigenvalue probability density function** can be computed by using the class method `joint_eigval_pdf(eigvals=None)`. By default, the method computes the joint eigenvalue PDF of the eigenvalues of the sampled random matrix. However, the method can be called using a pre-computed array of eigenvalues, and the joint eigenvalue PDF of these eigenvalues is returned. AS an example, we can simulate sampling and histogramming many eigenvalues of GOE random matrices of size 2x2, as well as illustrating the joint eigenvalue PDF for GOE matrices 2x2. This simulation is shown in the figure below.
+        ![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
+        <!---
+        <img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
+        -->
+        
         In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
         Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
         by using the `limit_pdf` argument.
         
         Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
         ```python
         from skrmt.ensemble import wigner_semicircular_law
```

### Comparing `scikit-rmt-0.5.0/README.md` & `scikit-rmt-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -56,25 +56,52 @@
 ```
 You may need to use `pip3`.
 ```bash
 pip3 install scikit-rmt
 ```
 
 ### Global installation
-Just install it using `pip`or `pip3`.
+Just install it using `pip` or `pip3`.
 ```bash
 pip install scikit-rmt
 ```
 
 ### Requirements
 *scikit-rmt* depends on the following packages:
 * [numpy](https://github.com/numpy/numpy) - The fundamental package for scientific computing with Python
 * [matplotlib](https://github.com/matplotlib/matplotlib) - Plotting with Python
 * [scipy](https://github.com/scipy/scipy) - Scientific computation in Python
 
+Check the pinned versions in the [requirements.txt](requirements.txt) file.
+
+----------------
+## Main features
+*scikit-rmt* provides support to analyze, study and simulate Random Matrix Theory properties and results:
+* **Sampling** of the following random matrix ensembles:
+   * Gaussian Ensemble (GOE, GUE and GSE; for beta=1, 2 and 4 respectively): class `GaussianEnsemble`.
+   * Wishart Ensemble (WRE, WCE and WQE; for beta=1, 2 and 4 respectively): class `WishartEnsemble`.
+   * Manova Ensemble (MRE, MCE and MQE; for beta=1, 2 and 4 respectively): class `ManovaEnsemble`.
+   * Circular Ensemble (COE, CUE, CSE; for beta=1, 2 and 4 respectively): class `CircularEnsemble`.
+* **Eigenvalue computation** for the previous ensembles using the class method `eigvals`.
+* Computation of the **joint eigenvalue probability density function** given the random matrix eigenvalues, using the class method `joint_eigval_pdf`.
+* Computation of the **empirical spectral histogram** by executing the class method `eigval_hist`.
+* **Plotting of the empirical spectral histogram** using the class method `plot_eigval_hist`.
+* Computation and plotting of the following **spectral laws** (`spectral_law` sub-module), including the calculation and plotting of the corresponding probability density functions (PDFs) and cumulative distribution functions (CDFs):
+   * **Wigner Semicircle law**: describes the limiting distribution of the eigenvalues of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `WignerSemicircleDistribution`.
+   * **Tracy-Widom law**: describes the limiting distribution of the largest eigenvalue of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `TracyWidomDistribution`.
+   * **Marchenko-Pastur law**: describes the limiting distribution of the eigenvalues of Wishart matrices (random matrices from the Wishart Ensemble). Implemented by class `MarchenkoPasturDistribution`.
+   * **Manova Spectrum law**: introduced and proved by K. W. Wachter (1980), it describes the limiting distribution of the eigenvalues of Manova matrices (random matrices from the Manova Ensemble). Implemented by class `ManovaSpectrumDistribution`.
+* **Covariance matrix estimation** using different matrix smoothing and estimation methods (`covariance` module).
+   * Estimation of sample covariance matrix using `sample_estimator` function.
+   * Finite-sample Optimal (FSOpt) estimator by `fsopt_estimator` function.
+   * Empirical Bayesian estimator by `empirical_bayesian_estimator` function. Haff in *"Estimation of a covariance matrix under Stein’s loss"* (1985).
+   * Minimax estimator by `minimax_estimator` function 
+   * Linear shrinkage estimator by `linear_shrinkage_estimator` function. Ledoit and Wolf in *"A well-conditioned estimator for large-dimensional covariance matrices"* (2004).
+   * Analytical shrinkage estimator by `analytical_shrinkage_estimator` function. Ledoit and Wolf in *"Analytical nonlinear shrinkage of large-dimensional covariance matrices"* (2020).
+
 
 -----------------
 ## A brief tutorial
 
 First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
 **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
 a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
@@ -123,14 +150,20 @@
 we can speed up histogramming procedure. The following graphical simulation using GOE matrices
 tries to illustrate it.
 ![Speed up by tridigonal forms](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/gauss_tridiag_sim.png)
 <!---
 <img src="imgs/gauss_tridiag_sim.png" width=820 height=370 alt="Speed up by tridigonal forms">
 -->
 
+On the other hand, for all the supported ensembles, the **joint eigenvalue probability density function** can be computed by using the class method `joint_eigval_pdf(eigvals=None)`. By default, the method computes the joint eigenvalue PDF of the eigenvalues of the sampled random matrix. However, the method can be called using a pre-computed array of eigenvalues, and the joint eigenvalue PDF of these eigenvalues is returned. AS an example, we can simulate sampling and histogramming many eigenvalues of GOE random matrices of size 2x2, as well as illustrating the joint eigenvalue PDF for GOE matrices 2x2. This simulation is shown in the figure below.
+![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
+<!---
+<img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
+-->
+
 In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
 Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
 by using the `limit_pdf` argument.
 
 Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
 ```python
 from skrmt.ensemble import wigner_semicircular_law
```

### Comparing `scikit-rmt-0.5.0/conf.py` & `scikit-rmt-0.6.0/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/docs/skrmt.covariance.rst` & `scikit-rmt-0.6.0/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/docs/skrmt.ensemble.rst` & `scikit-rmt-0.6.0/docs/skrmt.ensemble.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 skrmt.ensemble package
 ======================
 
 Submodules
 ----------
 
-skrmt.ensemble.circular\_ensemble module
+skrmt.ensemble.gaussian\_ensemble module
 ----------------------------------------
 
-.. automodule:: skrmt.ensemble.circular_ensemble
+.. automodule:: skrmt.ensemble.gaussian_ensemble
    :members:
    :undoc-members:
    :show-inheritance:
 
-skrmt.ensemble.gaussian\_ensemble module
-----------------------------------------
+skrmt.ensemble.wishart\_ensemble module
+---------------------------------------
 
-.. automodule:: skrmt.ensemble.gaussian_ensemble
+.. automodule:: skrmt.ensemble.wishart_ensemble
    :members:
    :undoc-members:
    :show-inheritance:
 
 skrmt.ensemble.manova\_ensemble module
 --------------------------------------
 
 .. automodule:: skrmt.ensemble.manova_ensemble
    :members:
    :undoc-members:
    :show-inheritance:
 
-skrmt.ensemble.plot\_law module
--------------------------------
+skrmt.ensemble.circular\_ensemble module
+----------------------------------------
 
-.. automodule:: skrmt.ensemble.plot_law
+.. automodule:: skrmt.ensemble.circular_ensemble
    :members:
    :undoc-members:
    :show-inheritance:
 
 skrmt.ensemble.tridiagonal\_utils module
 ----------------------------------------
 
 .. automodule:: skrmt.ensemble.tridiagonal_utils
    :members:
    :undoc-members:
    :show-inheritance:
 
-skrmt.ensemble.wishart\_ensemble module
----------------------------------------
-
-.. automodule:: skrmt.ensemble.wishart_ensemble
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 Module contents
 ---------------
 
 .. automodule:: skrmt.ensemble
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit-rmt-0.5.0/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.6.0/examples/plot_boosting_density_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/examples/plot_circular_ensemble.py` & `scikit-rmt-0.6.0/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/examples/plot_complex_histograms.py` & `scikit-rmt-0.6.0/examples/plot_complex_histograms.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.6.0/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/examples/plot_manova_ensemble.py` & `scikit-rmt-0.6.0/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.6.0/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/index.rst` & `scikit-rmt-0.6.0/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.6.0/scikit_rmt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.5.0
+Version: 0.6.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.5.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
@@ -65,25 +65,52 @@
         ```
         You may need to use `pip3`.
         ```bash
         pip3 install scikit-rmt
         ```
         
         ### Global installation
-        Just install it using `pip`or `pip3`.
+        Just install it using `pip` or `pip3`.
         ```bash
         pip install scikit-rmt
         ```
         
         ### Requirements
         *scikit-rmt* depends on the following packages:
         * [numpy](https://github.com/numpy/numpy) - The fundamental package for scientific computing with Python
         * [matplotlib](https://github.com/matplotlib/matplotlib) - Plotting with Python
         * [scipy](https://github.com/scipy/scipy) - Scientific computation in Python
         
+        Check the pinned versions in the [requirements.txt](requirements.txt) file.
+        
+        ----------------
+        ## Main features
+        *scikit-rmt* provides support to analyze, study and simulate Random Matrix Theory properties and results:
+        * **Sampling** of the following random matrix ensembles:
+           * Gaussian Ensemble (GOE, GUE and GSE; for beta=1, 2 and 4 respectively): class `GaussianEnsemble`.
+           * Wishart Ensemble (WRE, WCE and WQE; for beta=1, 2 and 4 respectively): class `WishartEnsemble`.
+           * Manova Ensemble (MRE, MCE and MQE; for beta=1, 2 and 4 respectively): class `ManovaEnsemble`.
+           * Circular Ensemble (COE, CUE, CSE; for beta=1, 2 and 4 respectively): class `CircularEnsemble`.
+        * **Eigenvalue computation** for the previous ensembles using the class method `eigvals`.
+        * Computation of the **joint eigenvalue probability density function** given the random matrix eigenvalues, using the class method `joint_eigval_pdf`.
+        * Computation of the **empirical spectral histogram** by executing the class method `eigval_hist`.
+        * **Plotting of the empirical spectral histogram** using the class method `plot_eigval_hist`.
+        * Computation and plotting of the following **spectral laws** (`spectral_law` sub-module), including the calculation and plotting of the corresponding probability density functions (PDFs) and cumulative distribution functions (CDFs):
+           * **Wigner Semicircle law**: describes the limiting distribution of the eigenvalues of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `WignerSemicircleDistribution`.
+           * **Tracy-Widom law**: describes the limiting distribution of the largest eigenvalue of Wigner matrices (in particular, random matrices from the Gaussian Ensemble). Implemented by class `TracyWidomDistribution`.
+           * **Marchenko-Pastur law**: describes the limiting distribution of the eigenvalues of Wishart matrices (random matrices from the Wishart Ensemble). Implemented by class `MarchenkoPasturDistribution`.
+           * **Manova Spectrum law**: introduced and proved by K. W. Wachter (1980), it describes the limiting distribution of the eigenvalues of Manova matrices (random matrices from the Manova Ensemble). Implemented by class `ManovaSpectrumDistribution`.
+        * **Covariance matrix estimation** using different matrix smoothing and estimation methods (`covariance` module).
+           * Estimation of sample covariance matrix using `sample_estimator` function.
+           * Finite-sample Optimal (FSOpt) estimator by `fsopt_estimator` function.
+           * Empirical Bayesian estimator by `empirical_bayesian_estimator` function. Haff in *"Estimation of a covariance matrix under Stein’s loss"* (1985).
+           * Minimax estimator by `minimax_estimator` function 
+           * Linear shrinkage estimator by `linear_shrinkage_estimator` function. Ledoit and Wolf in *"A well-conditioned estimator for large-dimensional covariance matrices"* (2004).
+           * Analytical shrinkage estimator by `analytical_shrinkage_estimator` function. Ledoit and Wolf in *"Analytical nonlinear shrinkage of large-dimensional covariance matrices"* (2020).
+        
         
         -----------------
         ## A brief tutorial
         
         First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
         **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
         a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
@@ -132,14 +159,20 @@
         we can speed up histogramming procedure. The following graphical simulation using GOE matrices
         tries to illustrate it.
         ![Speed up by tridigonal forms](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/gauss_tridiag_sim.png)
         <!---
         <img src="imgs/gauss_tridiag_sim.png" width=820 height=370 alt="Speed up by tridigonal forms">
         -->
         
+        On the other hand, for all the supported ensembles, the **joint eigenvalue probability density function** can be computed by using the class method `joint_eigval_pdf(eigvals=None)`. By default, the method computes the joint eigenvalue PDF of the eigenvalues of the sampled random matrix. However, the method can be called using a pre-computed array of eigenvalues, and the joint eigenvalue PDF of these eigenvalues is returned. AS an example, we can simulate sampling and histogramming many eigenvalues of GOE random matrices of size 2x2, as well as illustrating the joint eigenvalue PDF for GOE matrices 2x2. This simulation is shown in the figure below.
+        ![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
+        <!---
+        <img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
+        -->
+        
         In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
         Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
         by using the `limit_pdf` argument.
         
         Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
         ```python
         from skrmt.ensemble import wigner_semicircular_law
```

### Comparing `scikit-rmt-0.5.0/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.6.0/scikit_rmt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -36,26 +36,25 @@
 skrmt/covariance/tests/__init__.py
 skrmt/covariance/tests/test_estimator.py
 skrmt/covariance/tests/test_metrics.py
 skrmt/ensemble/__init__.py
 skrmt/ensemble/_base_ensemble.py
 skrmt/ensemble/circular_ensemble.py
 skrmt/ensemble/gaussian_ensemble.py
-skrmt/ensemble/law.py
 skrmt/ensemble/manova_ensemble.py
-skrmt/ensemble/plot_law.py
+skrmt/ensemble/spectral_law.py
 skrmt/ensemble/tracy_widom_approximator.py
 skrmt/ensemble/tridiagonal_utils.py
 skrmt/ensemble/wishart_ensemble.py
 skrmt/ensemble/tests/__init__.py
+skrmt/ensemble/tests/test_base_ens.py
 skrmt/ensemble/tests/test_circular_ens.py
 skrmt/ensemble/tests/test_gaussian_ens.py
-skrmt/ensemble/tests/test_law.py
 skrmt/ensemble/tests/test_manova_ens.py
-skrmt/ensemble/tests/test_plot_law.py
+skrmt/ensemble/tests/test_spectral_law.py
 skrmt/ensemble/tests/test_tracy_widom_approx.py
 skrmt/ensemble/tests/test_tridiagonalization.py
 skrmt/ensemble/tests/test_wishart_ens.py
 tutorial/README.txt
 tutorial/plot_0_introduction.py
 tutorial/plot_1_spectral_laws.py
 tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.5.0/setup.py` & `scikit-rmt-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/covariance/__init__.py` & `scikit-rmt-0.6.0/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/covariance/estimator.py` & `scikit-rmt-0.6.0/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/covariance/metrics.py` & `scikit-rmt-0.6.0/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.6.0/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.6.0/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/__init__.py` & `scikit-rmt-0.6.0/skrmt/ensemble/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,36 +4,27 @@
 """
 
 from .gaussian_ensemble import GaussianEnsemble
 from .wishart_ensemble import WishartEnsemble
 from .manova_ensemble import ManovaEnsemble
 from .circular_ensemble import CircularEnsemble
 
-from .law import WignerSemicircleDistribution
-from .law import MarchenkoPasturDistribution
-from .law import TracyWidomDistribution
-from .law import ManovaSpectrumDistribution
-
-from .plot_law import wigner_semicircle
-from .plot_law import marchenko_pastur
-from .plot_law import tracy_widom
-from .plot_law import manova_spectrum
+from .spectral_law import WignerSemicircleDistribution
+from .spectral_law import MarchenkoPasturDistribution
+from .spectral_law import TracyWidomDistribution
+from .spectral_law import ManovaSpectrumDistribution
 
 from .tridiagonal_utils import tridiag_eigval_neg
 from .tridiagonal_utils import tridiag_eigval_hist
 from .tridiagonal_utils import householder_reduction
 
 
 __all__ = ["GaussianEnsemble", "WishartEnsemble",
            "ManovaEnsemble", "CircularEnsemble",
            "WignerSemicircleDistribution",
            "MarchenkoPasturDistribution",
            "TracyWidomDistribution",
            "ManovaSpectrumDistribution",
-           "wigner_semicircle",
-           "marchenko_pastur",
-           "tracy_widom",
-           "manova_spectrum",
            "tridiag_eigval_neg",
            "tridiag_eigval_hist",
            "householder_reduction"
         ]
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.6.0/skrmt/ensemble/_base_ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def eigvals(self):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
     @abstractmethod
-    def eigval_pdf(self):
+    def joint_eigval_pdf(self):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
     def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
         """Calculates the histogram of the matrix eigenvalues.
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.6.0/skrmt/ensemble/circular_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,39 +288,47 @@
         # Saving plot or showing it
         if fig_path:
             plt.savefig(fig_path, dpi=600)
         else:
             plt.show()
 
 
-    def eigval_pdf(self):
+    def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
-        Calculates joint eigenvalue probability density function given the
-            current random matrix (so its eigenvalues). This function depends
-            on beta, i.e., in the sub-Circular ensemble.
+        Calculates joint eigenvalue probability density function given an array of
+        eigenvalues. If the array of eigenvalues is not provided, the current random
+        matrix sample (so its eigenvalues) is used. This function depends on beta,
+        i.e., in the sub-Circular ensemble.
+
+        Args:
+            eigvals (np.ndarray, default=None): numpy array with the values (eigenvalues)
+                to evaluate the joint pdf in.
 
         Returns:
-            real number. Value of the joint pdf of the current eigenvalues.
+            real number. Value of the joint pdf of the eigenvalues.
 
         References:
             - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
             - "Circular ensemble". Wikipedia.
                 en.wikipedia.org/wiki/Circular_ensemble
 
         '''
+        if eigvals is None:
+            # calculating eigenvalues
+            eigvals = self.eigvals()
+        n_eigvals = len(eigvals)
+
         # calculating Circular eigval pdf constant depeding on beta
         const_beta = (2*np.pi)**self.n * \
                      special.gamma(1 + self.n*self.beta/2)/(special.gamma(1 + self.beta/2)**self.n)
-        # calculating eigenvalues
-        eigvals = np.linalg.eigvals(self.matrix)
-        n_eigvals = len(eigvals)
+
         # calculating prod
         pdf = 1
         for k in range(n_eigvals):
             for i in range(k):
                 complex_num = complex(0, np.exp(eigvals[i])) - complex(0,np.exp(eigvals[k]))
                 pdf *= np.abs(complex_num)**self.beta
         # calculating Circular eigval pdf
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.6.0/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -284,37 +284,44 @@
         else:
             # pylint: disable=too-many-arguments
             if norm_const is None:
                 norm_const = 1/np.sqrt(self.n)
             super().plot_eigval_hist(bins, interval=interval, density=density,
                                      norm_const=norm_const, fig_path=fig_path)
 
-    def eigval_pdf(self):
+    def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
-        Calculates joint eigenvalue probability density function given the current
-        random matrix (so its eigenvalues). This function depends on beta, i.e.,
-        in the sub-Gaussian ensemble.
+        Calculates joint eigenvalue probability density function given an array of
+        eigenvalues. If the array of eigenvalues is not provided, the current random
+        matrix sample (so its eigenvalues) is used. This function depends on beta,
+        i.e., in the sub-Gaussian ensemble.
+
+        Args:
+            eigvals (np.ndarray, default=None): numpy array with the values (eigenvalues)
+                to evaluate the joint pdf in.
 
         Returns:
-            real number. Value of the joint pdf of the current eigenvalues.
+            real number. Value of the joint pdf of the eigenvalues.
 
         References:
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
+        if eigvals is None:
+            # calculating eigenvalues
+            eigvals = self.eigvals()
+        n_eigvals = len(eigvals)
+
         # calculating Hermite eigval pdf constant depeding on beta
         const_beta = (2*np.pi)**(-self.n/2)
         for j in range(self.n):
             const_beta *= special.gamma(1 + self.beta/2)/special.gamma(1 + self.beta*j/2)
-        # calculating eigenvalues
-        eigvals = self.eigvals()
-        n_eigvals = len(eigvals)
         # calculating prod
         pdf = 1
         for j in range(n_eigvals):
             for i in range(j):
                 pdf *= np.abs(eigvals[i] - eigvals[j])**self.beta
         # calculating exponential term
         exp_val = np.exp(-np.sum((eigvals**2)/2))
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/law.py` & `scikit-rmt-0.6.0/skrmt/ensemble/spectral_law.py`

 * *Files 27% similar despite different names*

```diff
@@ -111,14 +111,35 @@
 
     if savefig_path:
         plt.savefig(savefig_path, dpi=800)
     else:
         plt.show()
 
 
+def _get_bins_centers_and_contour(bins):
+    """Calculates the centers and contour of the given bins.
+
+    Computes the centers of the given bins. Also, the smallest and the largest bin
+    delimitiers are included to define the countour of the representation interval.
+
+    Args:
+        bins (list): list of numbers (floats) that specify each bin delimiter.
+
+    Returns:
+        list of numbers (floats) consisting in the list of bin centers and contour.
+    
+    """
+    centers = [bins[0]] # Adding initial contour
+    l = len(bins)
+    for i in range(l-1):
+        centers.append((bins[i]+bins[i+1])/2) # Adding centers
+    centers.append(bins[-1]) # Adding final contour
+    return centers
+
+
 class WignerSemicircleDistribution:
     """Wigner Semicircle Distribution class.
 
     The Wigner Semicircle Law describes the spectrum of the Wigner random matrices.
     In particular, random matrices of the Gaussian Ensemble are Wigner matrices,
     and therefore the spectrum of the random matrices of this ensemble converge
     to the Wigner Semicircle Law when the matrix size goes to infinity. This
@@ -162,15 +183,15 @@
         """
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
 
         self.beta = beta
         self.center = center
         self.sigma = sigma
-        self.radius = 2.0 * np.sqrt(self.beta) * sigma
+        self.radius = 2.0 * np.sqrt(self.beta) * self.sigma
         self._gaussian_ens = None
     
     def rvs(self, size):
         """Samples ranfom variates following this distribution.
 
         Args:
             size (int): sample size.
@@ -256,14 +277,101 @@
         if interval is None:
             interval = (self.center - self.radius - 0.1, self.center + self.radius + 0.1)
         
         _plot_func(
             interval, func=self.cdf, bins=bins, 
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
+    
+
+    def plot_empirical_pdf(self, n_size=1000, bins=100, interval=None, density=False,
+                           plot_law_pdf=False, savefig_path=None):
+        """Computes and plots Wigner's semicircle empirical law using Gaussian Ensemble.
+
+        Calculates and plots Wigner's semicircle empirical law using Gaussian Ensemble
+        random matrices. Gaussian (Hermite) ensemble has improved routines (using
+        tridiagonal forms and Sturm sequences) to avoid calculating the eigenvalues,
+        so the histogram is built using certain techniques to boost efficiency.
+
+        Args:
+            n_size (int, default=1000): random matrix size n times n. This is the sample size.
+            bins (int or sequence, default=100): If bins is an integer, it defines the number
+                of equal-width bins in the range. If bins is a sequence, it defines the
+                bin edges, including the left edge of the first bin and the right
+                edge of the last bin; in this case, bins may be unequally spaced.
+            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
+                The lower and upper range of the bins. Lower and upper outliers are ignored.
+            density (bool, default=False): If True, draw and return a probability
+                density: each bin will display the bin's raw count divided by the total
+                number of counts and the bin width, so that the area under the histogram
+                integrates to 1. If set to False, the absolute frequencies of the eigenvalues
+                are returned.
+            plot_law_pdf (bool, default=False): If True, the theoretical law is plotted.
+                If set to False, just the empirical histogram is shown. This parameter is only
+                considered when the argument 'density' is set also to True.
+            savefig_path (string, default=None): path to save the created figure. If it is not
+                provided, the plot is shown are the end of the routine.
+
+        References:
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
+                "Sturm sequences and random eigenvalue distributions".
+                Foundations of Computational Mathematics. 9.4 (2008): 461-483.
+            - Dumitriu, I. and Edelman, A.
+                "Matrix Models for Beta Ensembles".
+                Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
+
+        """
+        # pylint: disable=too-many-arguments
+        if n_size<1:
+            raise ValueError("matrix size must be positive")
+
+        if self.center != 0.0:
+            print(f"Warning: The given center is not 0.0 (center = {self.center}).\n"
+                  "\t It is only available the centered empirical Wigner's semicircle law.")
+        
+        use_tridiag = (self.sigma == 1.0)
+        if not use_tridiag:
+            print(f"Warning: The given scale is not the standard (sigma = {self.sigma}).\n"
+                "\t Tridiagonal histogramming is deactivated.\n"
+                "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
+
+        ens = GaussianEnsemble(beta=self.beta, n=n_size, sigma=self.sigma, use_tridiagonal=use_tridiag)
+
+        # default plotting interval in case it's not provided
+        if interval is None:
+            interval = (-self.radius, self.radius)
+
+        # Wigner eigenvalue normalization constant
+        if use_tridiag:
+            norm_const = 1/np.sqrt(n_size) if self.beta==4 else 1/np.sqrt(n_size/2)
+        else:
+            norm_const = 1/np.sqrt(n_size)
+
+        observed, bins = ens.eigval_hist(bins=bins, interval=interval,
+                                        density=density, norm_const=norm_const)
+        width = bins[1]-bins[0]
+        plt.bar(bins[:-1], observed, width=width, align='edge')
+
+        # Plotting Wigner Semicircle Law pdf
+        if plot_law_pdf and density:
+            centers = np.asarray(_get_bins_centers_and_contour(bins))
+            pdf = self.pdf(centers)
+            plt.plot(centers, pdf, color='red', linewidth=2)
+        elif plot_law_pdf and not density:
+            print("Warning: Wigner's Semicircle Law PDF is only plotted when density is True.")
+
+        plt.title("Wigner Semicircle Law - Empirical density histogram", fontweight="bold")
+        plt.xlabel("x")
+        plt.ylabel("probability density")
+
+        # Saving plot or showing it
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=1200)
+        else:
+            plt.show()
 
 
 
 class MarchenkoPasturDistribution:
     """Marchenko-Pastur Distribution class.
 
     The Marchenko-Pastur Law describes the spectrum of the Wishart random matrices.
@@ -297,21 +405,21 @@
 
     def __init__(self, ratio, beta=1, sigma=1.0):
         """Constructor for MarchenkoPasturDistribution class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
-            ratio (float): random matrix size ratio. This is the ratio between the
-                number of degrees of freedom 'p' and the sample size 'n'. The value
-                of ratio = p/n.
-            beta (int, default=1): descriptive integer of the Wishart ensemble type.
+            ratio (float): random matrix size ratio (:math:`\lambda`). This is the ratio
+                between the number of degrees of freedom :math:`p` and the sample size :math:`n`.
+                The value of ratio is computed as :math:`\lambda = p/n`.
+            beta (int, default=1): descriptive integer of the Wishart ensemble type (:math:`\beta`).
                 For WRE beta=1, for WCE beta=2, for WQE beta=4.
-            sigma (float, default=1.0): scale of the distribution. This value also corresponds
-                to the standard deviation of the random entries of the sampled matrix.
+            sigma (float, default=1.0): scale of the distribution (:math:`\sigma`). This value also
+                corresponds to the standard deviation of the random entries of the sampled matrix.
         
         """
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
         if ratio <= 0:
             raise ValueError(f"Error: invalid ratio. It has to be positive. Provided ratio = {ratio}.")
 
@@ -323,15 +431,15 @@
         self._var = self.beta * self.sigma**2
         self._wishart_ens = None
     
     def rvs(self, size):
         """Samples ranfom variates following this distribution.
 
         Args:
-            size (int): sample size.
+            size (int): sample size :math:`n`.
         
         Returns:
             numpy array with the generated samples.
         """
         if size <= 0:
             raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
         
@@ -442,14 +550,140 @@
             interval = (self.lambda_minus, self.lambda_plus)
         
         _plot_func(
             interval, func=self.cdf, bins=bins, 
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
+    def plot_empirical_pdf(self, n_size=3000, p_size=None, bins=100, interval=None,
+                           density=False, plot_law_pdf=False, savefig_path=None):
+        """Computes and plots Marchenko-Pastur empirical law using Wishart Ensemble random matrices.
+
+        Calculates and plots Marchenko-Pastur empirical law using Wishart Ensemble random matrices.
+        The size of the sampled matrix will depend on the `n_size` (:math:`n`) parameter and on the
+        ratio :math:`\lambda` given when instantiating this class, unless the parameter `p_size` (:math:`p`)
+        is also given. In this last case, the ratio :math:`\lambda` for the empirical pdf plotting is
+        computed as :math:`\lambda = p/n`. If only the sample size :math:`n` is provided, the number
+        of degrees of freedom :math:`p` is computed as :math:`[\lambda * n]`.
+        Wishart (Laguerre) ensemble has improved routines (using tridiagonal forms and Sturm
+        sequences) to avoid calculating the eigenvalues, so the histogram is built using certain
+        techniques to boost efficiency. This optimization is only used when the ratio p_size/n_size
+        is less or equal than 1.
+
+        Args:
+            n_size (int, default=3000): number of columns of the guassian matrix that generates
+                the matrix of the corresponding ensemble. This is the sample size. The number of
+                degrees of freedom is computed depending on this argument and on the given ratio,
+                unless the argument `p_size` is also provided, which in this case the ratio is
+                re-computed as ratio=p_size/n_size.
+            p_size (int, default=None): number of rows of the guassian matrix that generates
+                the matrix of the corresponding ensemble. If provided, the current ratio is ignored
+                (but not replaced) and the new ratio=p_size/n_size is used instead.
+            bins (int or sequence, default=100): If bins is an integer, it defines the number
+                of equal-width bins in the range. If bins is a sequence, it defines the
+                bin edges, including the left edge of the first bin and the right
+                edge of the last bin; in this case, bins may be unequally spaced.
+            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
+                The lower and upper range of the bins. Lower and upper outliers are ignored.
+            density (bool, default=False): If True, draw and return a probability
+                density: each bin will display the bin's raw count divided by the total
+                number of counts and the bin width, so that the area under the histogram
+                integrates to 1. If set to False, the absolute frequencies of the eigenvalues
+                are returned.
+            plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+                If set to False, just the empirical histogram is shown. This parameter is only
+                considered when the argument 'density' is set also to True.
+            savefig_path (string, default=None): path to save the created figure. If it is not
+                provided, the plot is shown are the end of the routine.
+
+        References:
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
+                "Sturm sequences and random eigenvalue distributions".
+                Foundations of Computational Mathematics. 9.4 (2008): 461-483.
+            - Dumitriu, I. and Edelman, A.
+                "Matrix Models for Beta Ensembles".
+                Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
+
+        """
+        # pylint: disable=too-many-arguments
+        if n_size<1 or (p_size is not None and p_size<1):
+            raise ValueError("matrix size must be positive")
+        
+        if interval and interval[0] == 0:
+            print("Warning: setting the beginning of the interval to zero may generate numerical errors.")
+            print(f"Setting interval to (-0.01, {interval[1]})")
+            interval = (-0.01, interval[1])
+
+        # calculating constants depending on matrix sizes
+        if p_size is None:
+            p_size = round(self.ratio * n_size)
+
+        # computing an approximated ratio since p_size is rounded to the closest integer        
+        approx_ratio = p_size/n_size
+        lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(approx_ratio))**2
+        lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(approx_ratio))**2
+        use_tridiag_ratio = (approx_ratio <= 1)
+        if not use_tridiag_ratio:
+            print("Warning: Cannot use tridiagonal histogramming if 'p' (degrees of freedom) is "
+                " greater than 'n' (sample size).\n"
+                f"\t Provided n={n_size} and p={p_size}. Tridiagonal histogramming is therefore deactivated.\n"
+                "\t It is adviced to increase sample size (`n`) to optimize and boost histogramming.")
+
+        # computing interval according to the matrix size ratio and support
+        if interval is None:
+            if approx_ratio <= 1:
+                interval = (lambda_minus, lambda_plus)
+            else:
+                interval = (min(-0.05, lambda_minus), lambda_plus)
+        
+        use_tridiag_sigma = (self.sigma == 1.0)
+        if not use_tridiag_sigma:
+            print(f"Warning: The given scale is not the standard (sigma = {self.sigma}).\n"
+                "\t Tridiagonal histogramming is deactivated.\n"
+                "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
+
+        ens = WishartEnsemble(beta=self.beta, p=p_size, n=n_size, sigma=self.sigma,
+                            use_tridiagonal=(use_tridiag_ratio and use_tridiag_sigma))
+
+        # Wigner eigenvalue normalization constant
+        norm_const = 1/n_size 
+
+        observed, bins = ens.eigval_hist(bins=bins, interval=interval,
+                                         density=density, norm_const=norm_const)
+        width = bins[1]-bins[0]
+        plt.bar(bins[:-1], observed, width=width, align='edge')
+
+        # Plotting theoretical graphic
+        if plot_law_pdf and density:
+            centers = np.array(_get_bins_centers_and_contour(bins))
+            # creating new instance with the approximated ratio depending on the given matrix sizes
+            mpd = MarchenkoPasturDistribution(beta=self.beta, ratio=approx_ratio, sigma=self.sigma)
+            pdf = mpd.pdf(centers)
+            plt.plot(centers, pdf, color='red', linewidth=2)
+
+        plt.title("Marchenko-Pastur Law - Empirical density histogram", fontweight="bold")
+        plt.xlabel("x")
+        plt.ylabel("probability density")
+        if approx_ratio > 1:
+            if plot_law_pdf and density:
+                ylim_vals = pdf
+            else:
+                ylim_vals = observed
+            try:
+                plt.ylim(0, np.max(ylim_vals)+0.25*np.max(ylim_vals))
+            except ValueError:
+                second_highest_val = np.partition(ylim_vals.flatten(), -2)[-2]
+                plt.ylim(0, second_highest_val+0.25*second_highest_val)
+
+        # Saving plot or showing it
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=1200)
+        else:
+            plt.show()
+
 
 
 class TracyWidomDistribution:
     """Tracy-Widom Distribution class.
 
     The Tracy-Widom Law describes the behaviour of the largest eigenvalue of the
     Wigner random matrices. In particular, random matrices of the Gaussian Ensemble
@@ -597,14 +831,100 @@
             interval = (-5, 4-self.beta)
         
         _plot_func(
             interval, func=self.cdf, bins=bins, 
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
+    def plot_empirical_pdf(self, n_size=100, times=1000, bins=100, interval=None,
+                           density=False, plot_law_pdf=False, savefig_path=None):
+        """Computes and plots Tracy-Widom empirical law using Gaussian Ensemble.
+
+        Calculates and plots Tracy-Widom empirical law using Gaussian Ensemble random matrices.
+        Because we need to obtain the largest eigenvalue of each sampled random matrix,
+        we need to sample a certain amount them. For each random matrix sammpled, its
+        largest eigenvalue is calcualted in order to simulate its density.
+
+        Args:
+            n_size (int, default=100): random matrix size n times n. This is the sample size.
+            times (int, default=1000): number of times to sample a random matrix.
+            bins (int or sequence, default=100): If bins is an integer, it defines the number
+                of equal-width bins in the range. If bins is a sequence, it defines the
+                bin edges, including the left edge of the first bin and the right
+                edge of the last bin; in this case, bins may be unequally spaced.
+            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
+                The lower and upper range of the bins. Lower and upper outliers are ignored.
+            density (bool, default=False): If True, draw and return a probability
+                density: each bin will display the bin's raw count divided by the total
+                number of counts and the bin width, so that the area under the histogram
+                integrates to 1. If set to False, the absolute frequencies of the eigenvalues
+                are returned.
+            plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+                If set to False, just the empirical histogram is shown. This parameter is only
+                considered when the argument 'density' is set also to True.
+            savefig_path (string, default=None): path to save the created figure. If it is not
+                provided, the plot is shown are the end of the routine.
+
+        References:
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
+                "Sturm sequences and random eigenvalue distributions".
+                Foundations of Computational Mathematics. 9.4 (2008): 461-483.
+            - Dumitriu, I. and Edelman, A.
+                "Matrix Models for Beta Ensembles".
+                Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
+
+        """
+        # pylint: disable=too-many-arguments
+        if n_size<1 or times<1:
+            raise ValueError("matrix size or number of repetitions must be positive")
+
+        ens = GaussianEnsemble(beta=self.beta, n=n_size, use_tridiagonal=False)
+
+        eigvals = []
+        for _ in range(times):
+            eigvals.append(ens.eigvals().max())
+            ens.sample()
+        eigvals = np.asarray(eigvals)
+
+        # Tracy-Widom eigenvalue distr. normalization constants
+        eigval_scale = 1.0
+        size_scale = 1.0
+        if self.beta == 2:
+            eigval_scale = 1/np.sqrt(2)
+        elif self.beta == 4:
+            eigval_scale = size_scale = 1/np.sqrt(2)
+            n_size *= 2
+        eigvals = size_scale*(n_size**(1/6))*(eigval_scale*eigvals - (2.0*np.sqrt(n_size)))
+
+        if interval is None:
+            xmin=eigvals.min()
+            xmax=eigvals.max()
+            interval=(xmin, xmax)
+
+        # using numpy to obtain histogram in the given interval and no. of bins
+        observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
+        width = bins[1]-bins[0]
+        plt.bar(bins[:-1], observed, width=width, align='edge')
+
+        # Plotting theoretical graphic
+        if plot_law_pdf and density:
+            centers = _get_bins_centers_and_contour(bins)
+            pdf = self.pdf(centers)
+            plt.plot(centers, pdf, color='red', linewidth=2)
+
+        plt.title("Tracy-Widom Law - Empirical density histogram", fontweight="bold")
+        plt.xlabel("x")
+        plt.ylabel("probability density")
+
+        # Saving plot or showing it
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=1200)
+        else:
+            plt.show()
+
 
 
 class ManovaSpectrumDistribution:
     """Manova Spectrum Distribution class.
 
     The spectrum of the random matrices of the Manova Ensemble converge to a
     well-defined function implemented in this class. The class provides methods
@@ -777,7 +1097,127 @@
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
 
         _plot_func(
             interval, func=self.cdf, bins=bins, 
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
+
+    def plot_empirical_pdf(self, m_size=1000, n1_size=None, n2_size=None, bins=100, interval=None,
+                           density=False, plot_law_pdf=False, savefig_path=None):
+        """Computes and plots Manova spectrum empirical pdf and analytical distribution.
+
+        Calculates and plots Manova spectrum empirical pdf using Manova Ensemble random matrices.
+        The size of the sampeld matrices will depend on the `m_size` (:math:`m`) parameter (no. of
+        degrees of freedom) and on the ratios :math:`a` and :math:`b` given when instantiating this
+        class, unless the parameters `n1_size` (:math:`n_1`) and/or `n2_size` (:math:`n_2`) are also
+        given. In this last case, the new ratio :math:`a` for the empirical pdf plotting is computed
+        as :math:`a = n_1/m`, and the new ratio :math:`b` is calculated as :math:`b = n_2/m`. If only
+        the number of degrees of freedom :math:`m` is provided, the sample sizes :math:`n_1` and :math:`n_2`
+        are computed as :math:`n_1 = [a * m]` and :math:`n_2 = [b * m]` respectively.
+
+        Args:
+            m_size (int, default=1000): number of rows of the two Wishart Ensemble matrices that
+                generates the matrix of the corresponding ensemble. This is the number of degrees
+                of freedom (:math:`m`). The sample sizes (:math:`n_1` and :math:`n_2`) of the two
+                matrices are computed from this value and the ratios :math:`a` and :math:`b` given
+                to instantiate this class.
+            n1_size (int, default=None): number of columns of the first Wishart Ensemble matrix
+                that generates the matrix of the corresponding ensemble (:math:`n_1`). If provided,
+                the ratio :math:`a` is ignored (but not replaced) and the new ratio :math:`a = n_1/m`
+                is used instead to plot the empirical pdf.
+            n2_size (int, default=None): number of columns of the second Wishart Ensemble matrix
+                that generates the matrix of the corresponding ensemble (:math:`n_2`). If provided,
+                the ratio :math:`b` is ignored (but not replaced) and the new ratio :math:`b = n_2/m`
+                is used instead to plot the empirical pdf.
+            bins (int or sequence, default=100): If bins is an integer, it defines the number
+                of equal-width bins in the range. If bins is a sequence, it defines the
+                bin edges, including the left edge of the first bin and the right
+                edge of the last bin; in this case, bins may be unequally spaced.
+            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
+                The lower and upper range of the bins. Lower and upper outliers are ignored.
+            density (bool, default=False): If True, draw and return a probability
+                density: each bin will display the bin's raw count divided by the total
+                number of counts and the bin width, so that the area under the histogram
+                integrates to 1. If set to False, the absolute frequencies of the eigenvalues
+                are returned.
+            plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+                If set to False, just the empirical histogram is shown. This parameter is only
+                considered when the argument 'density' is set also to True.
+            savefig_path (string, default=None): path to save the created figure. If it is not
+                provided, the plot is shown are the end of the routine.
+
+        References:
+            - Laszlo, L. and Farrel, B.
+                "Local Eigenvalue Density for General MANOVA Matrices".
+                Journal of Statistical Physics. 152.6 (2013): 1003-1032.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
+                "Sturm sequences and random eigenvalue distributions".
+                Foundations of Computational Mathematics. 9.4 (2008): 461-483.
+            - Dumitriu, I. and Edelman, A.
+                "Matrix Models for Beta Ensembles".
+                Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
+
+        """
+        if m_size<1 or (n1_size is not None and n1_size<1) or (n2_size is not None and n2_size<1):
+            raise ValueError("matrix size must be positive")
+
+        if n1_size is None:
+            n1_size = round(self.a * m_size)
+        
+        if n2_size is None:
+            n2_size = round(self.b * m_size)
+
+        ens = ManovaEnsemble(beta=self.beta, m=m_size, n1=n1_size, n2=n2_size)
+
+        # computing approximated ratios since the n1_size and n2_size parameters
+        # could have been rounded previously
+        approx_a = n1_size/m_size
+        approx_b = n2_size/m_size
+        if approx_a <= 1 or approx_b <= 1:
+            print("Warning: sample size ('n1_size' or 'n2_size') too small compared "
+                  "to degrees of freedom ('m_size'). It may cause numerical instability.")
+        lambda_term1 = np.sqrt((approx_a/(approx_a+approx_b)) * (1 - (1/(approx_a+approx_b))))
+        lambda_term2 = np.sqrt((1/(approx_a+approx_b)) * (1 - (approx_a/(approx_a+approx_b))))
+        lambda_minus = (lambda_term1 - lambda_term2)**2
+        lambda_plus = (lambda_term1 + lambda_term2)**2
+
+        if interval is None:
+            interval = [lambda_minus, lambda_plus]
+            if approx_a <= 1:
+                interval[0] = min(-0.05, lambda_minus)
+            if approx_b <= 1:
+                interval[1] = max(lambda_plus, 1.05)
+            interval = tuple(interval)
+
+        observed, bins = ens.eigval_hist(bins=bins, interval=interval, density=density, avoid_img=True)
+
+        width = bins[1]-bins[0]
+        plt.bar(bins[:-1], observed, width=width, align='edge')
+
+        # Plotting theoretical graphic
+        if plot_law_pdf and density:
+            centers = np.array(_get_bins_centers_and_contour(bins))
+            # creating new instance with the approximated ratios depending on the given matrix sizes
+            msd = ManovaSpectrumDistribution(beta=self.beta, a=approx_a, b=approx_b)
+            pdf = msd.pdf(centers)
+            plt.plot(centers, pdf, color='red', linewidth=2)
+
+        plt.title("Manova Spectrum - Empirical density histogram", fontweight="bold")
+        plt.xlabel("x")
+        plt.ylabel("probability density")
+        if approx_a <= 1 or approx_b <= 1:
+            if plot_law_pdf and density:
+                ylim_vals = pdf
+            else:
+                ylim_vals = observed
+            try:
+                plt.ylim(0, np.max(ylim_vals) + 0.25*np.max(ylim_vals))
+            except ValueError:
+                second_highest_val = np.partition(ylim_vals.flatten(), -2)[-2]
+                plt.ylim(0, second_highest_val + 0.25*second_highest_val)
+
+        # Saving plot or showing it
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=1200)
+        else:
+            plt.show()
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.6.0/skrmt/ensemble/manova_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,45 +245,53 @@
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         return super().plot_eigval_hist(bins, interval, density,
                                         norm_const=norm_const, avoid_img=True, fig_path=fig_path)
 
-    def eigval_pdf(self):
+    def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
-        Calculates joint eigenvalue probability density function given the current
-            random matrix (so its eigenvalues). This function depends on beta, i.e.,
-            in the sub-Manova ensemble.
+        Calculates joint eigenvalue probability density function given an array of
+        eigenvalues. If the array of eigenvalues is not provided, the current random
+        matrix sample (so its eigenvalues) is used. This function depends on beta,
+        i.e., in the sub-Manova ensemble.
+
+        Args:
+            eigvals (np.ndarray, default=None): numpy array with the values (eigenvalues)
+                to evaluate the joint pdf in.
 
         Returns:
-            real number. Value of the joint pdf of the current eigenvalues.
+            real number. Value of the joint pdf of the eigenvalues.
 
         References:
             - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
         # pylint: disable=invalid-name
         a1 = self.beta*self.n1/2
         a2 = self.beta*self.n2/2
         p = 1 + self.beta/2*(self.m - 1)
 
+        if eigvals is None:
+            # calculating eigenvalues
+            eigvals = self.eigvals()
+        n_eigvals = len(eigvals)
+
         # calculating Jacobi eigval pdf constant depeding on beta
         const_beta = 1
         for j in range(self.m):
             const_beta *= (special.gamma(1 + self.beta/2) * \
                             special.gamma(a1 + a2 -self.beta/2*(self.m - j)))/ \
                           (special.gamma(1 + self.beta*j/2) * \
                             special.gamma(a1 - self.beta/2*(self.m - j)) * \
                               special.gamma(a2 - self.beta/2*(self.m - j)))
-        # calculating eigenvalues
-        eigvals = np.linalg.eigvals(self.matrix)
-        n_eigvals = len(eigvals)
+
         # calculating first prod
         prod1 = 1
         for j in range(n_eigvals):
             for i in range(j):
                 prod1 *= np.abs(eigvals[i] - eigvals[j])**self.beta
         # calculating second prod
         prod2 = 1
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,29 +68,28 @@
     coe = CircularEnsemble(beta=1, n=n_size)
 
     vals = coe.eigvals()
 
     assert_array_equal(vals.imag, 0.0)
 
 
-
-def test_beta1_eigval_pdf():
+def test_beta1_joint_eigval_pdf():
     '''Testing joint eigenvalue pdf
     '''
     n_size = 3
     coe = CircularEnsemble(beta=1, n=n_size)
 
     coe.matrix = np.zeros((n_size,n_size))
-    assert coe.eigval_pdf() == 0.0
+    assert coe.joint_eigval_pdf() == 0.0
 
     coe.matrix = np.eye(n_size)
-    assert coe.eigval_pdf() == 0.0
+    assert coe.joint_eigval_pdf() == 0.0
 
     coe.matrix = 10*np.eye(n_size)
-    assert coe.eigval_pdf() == 0.0
+    assert coe.joint_eigval_pdf() == 0.0
 
 
 ##########################################
 ### Circular Unitary Ensemble = CUE
 
 def test_cue_init():
     '''Testing CUE init
@@ -136,14 +135,30 @@
 
     vals = cue.eigvals()
 
     mods = np.absolute(vals)
     assert_almost_equal(mods, 1.0, decimal=12)
 
 
+def test_beta2_joint_eigval_pdf():
+    '''Testing joint eigenvalue pdf
+    '''
+    n_size = 3
+    cue = CircularEnsemble(beta=2, n=n_size)
+
+    cue.matrix = np.zeros((n_size,n_size))
+    assert cue.joint_eigval_pdf() == 0.0
+
+    cue.matrix = np.eye(n_size)
+    assert cue.joint_eigval_pdf() == 0.0
+
+    cue.matrix = 10*np.eye(n_size)
+    assert cue.joint_eigval_pdf() == 0.0
+
+
 ##########################################
 ### Circular Symplectic Ensemble = CSE
 
 def test_cse_init():
     '''Testing CSE init
     '''
     n_size = 2
@@ -177,7 +192,23 @@
     cse.set_size(n2_size, resample_mtx=False)
     assert cse.n == n2_size
     assert cse.matrix.shape == (2*n1_size,2*n1_size)
 
     cse.set_size(n2_size, resample_mtx=True)
     assert cse.n == n2_size
     assert cse.matrix.shape == (2*n2_size,2*n2_size)
+
+
+def test_beta4_joint_eigval_pdf():
+    '''Testing joint eigenvalue pdf
+    '''
+    n_size = 3
+    cse = CircularEnsemble(beta=4, n=n_size)
+
+    cse.matrix = np.zeros((n_size,n_size))
+    assert cse.joint_eigval_pdf() == 0.0
+
+    cse.matrix = np.eye(n_size)
+    assert cse.joint_eigval_pdf() == 0.0
+
+    cse.matrix = 10*np.eye(n_size)
+    assert cse.joint_eigval_pdf() == 0.0
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,28 +89,28 @@
     for i in range(n_size):
         assert normals[i] == goe.matrix[i][i]
     for i in range(n_size-1):
         assert chisqs[i] == goe.matrix[i][i+1]
         assert chisqs[i] == goe.matrix[i+1][i]
 
 
-def test_beta1_eigval_pdf():
+def test_beta1_joint_eigval_pdf():
     '''Testing joint eigenvalue pdf
     '''
     n_size = 3
     goe = GaussianEnsemble(beta=1, n=n_size)
 
     goe.matrix = np.zeros((n_size,n_size))
-    assert goe.eigval_pdf() == 0.0
+    assert goe.joint_eigval_pdf() == 0.0
 
     goe.matrix = np.eye(n_size)
-    assert goe.eigval_pdf() == 0.0
+    assert goe.joint_eigval_pdf() == 0.0
 
     goe.matrix = 10*np.eye(n_size)
-    assert goe.eigval_pdf() == 0.0
+    assert goe.joint_eigval_pdf() == 0.0
 
 
 def test_goe_tridiag_hist():
     '''Testing tridiagonal histogram of GOE
     '''
     n_size = 50
     goe1 = GaussianEnsemble(beta=1, n=n_size, use_tridiagonal=False)
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,25 +53,25 @@
     mre.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True)
     assert mre.m == m2_size
     assert mre.n1 == n21_size
     assert mre.n2 == n22_size
     assert mre.matrix.shape == (m2_size,m2_size)
 
 
-def test_beta1_eigval_pdf():
+def test_beta1_joint_eigval_pdf():
     '''Testing joint eigenvalue pdf
     '''
     m_size, n1_size, n2_size = 4, 6, 8
     mre = ManovaEnsemble(beta=1, m=m_size, n1=n1_size, n2=n2_size)
 
     mre.matrix = np.zeros((m_size,m_size))
-    assert mre.eigval_pdf() == 0.0
+    assert mre.joint_eigval_pdf() == 0.0
 
     mre.matrix = np.eye(m_size)
-    assert mre.eigval_pdf() == 0.0
+    assert mre.joint_eigval_pdf() == 0.0
 
 
 ##########################################
 ### Manova Complex Ensemble = MCE
 
 def test_manova_complex_init():
     '''Testing MCE init
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,28 +111,28 @@
     for i in range(p_size-1):
         assert offdiag[i] == wre.matrix[i][i+1]
         assert offdiag[i] == wre.matrix[i+1][i]
 
     assert_almost_equal(wre.matrix, np.dot(mtx, mtx.transpose()), decimal=7)
 
 
-def test_beta1_eigval_pdf():
+def test_beta1_joint_eigval_pdf():
     '''Testing joint eigenvalue pdf
     '''
     p_size, n_size = 3, 5
     wre = WishartEnsemble(beta=1, p=p_size, n=n_size)
 
     wre.matrix = np.zeros((p_size,p_size))
-    assert wre.eigval_pdf() == 0.0
+    assert wre.joint_eigval_pdf() == 0.0
 
     wre.matrix = np.eye(p_size)
-    assert wre.eigval_pdf() == 0.0
+    assert wre.joint_eigval_pdf() == 0.0
 
     wre.matrix = 10*np.eye(p_size)
-    assert wre.eigval_pdf() == 0.0
+    assert wre.joint_eigval_pdf() == 0.0
 
 
 def test_wre_tridiag_hist():
     '''Testing tridiagonal histogram of WRE
     '''
     p_size, n_size = 50, 100
     wre1 = WishartEnsemble(beta=1, p=p_size, n=n_size, use_tridiagonal=False)
```

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.6.0/skrmt/ensemble/tridiagonal_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.5.0/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.6.0/skrmt/ensemble/wishart_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,40 +306,47 @@
                 plt.savefig(fig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
             super().plot_eigval_hist(bins, interval, density, norm_const, fig_path)
 
-    def eigval_pdf(self):
+    def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
-        Calculates joint eigenvalue probability density function given the current
-            random matrix (so its eigenvalues). This function depends on beta, i.e.,
-            in the sub-Wishart ensemble.
+        Calculates joint eigenvalue probability density function given an array of
+        eigenvalues. If the array of eigenvalues is not provided, the current random
+        matrix sample (so its eigenvalues) is used. This function depends on beta,
+        i.e., in the sub-Wishart ensemble.
+
+        Args:
+            eigvals (np.ndarray, default=None): numpy array with the values (eigenvalues)
+                to evaluate the joint pdf in.
 
         Returns:
-            real number. Value of the joint pdf of the current eigenvalues.
+            real number. Value of the joint pdf of the eigenvalues.
 
         References:
             - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
+        if eigvals is None:
+            # calculating eigenvalues
+            eigvals = self.eigvals()
+        n_eigvals = len(eigvals)
+
         a_val = self.beta*self.n/2
         p_aux = 1 + self.beta/2*(self.p - 1)
         # calculating Laguerre eigval pdf constant depeding on beta
         const_beta = 2**(-self.p*a_val)
         for j in range(self.p):
             const_beta *= special.gamma(1 + self.beta/2)/ \
                           (special.gamma(1 + self.beta*j/2)*\
                             special.gamma(a_val - self.beta/2*(self.p - j)))
-        # calculating eigenvalues
-        eigvals = np.linalg.eigvals(self.matrix)
-        n_eigvals = len(eigvals)
         # calculating first prod
         prod1 = 1
         for j in range(n_eigvals):
             for i in range(j):
                 prod1 *= np.abs(eigvals[i] - eigvals[j])**self.beta
         # calculating second prod
         prod2 = np.prod(eigvals**(a_val - p_aux))
```

### Comparing `scikit-rmt-0.5.0/tutorial/plot_0_introduction.py` & `scikit-rmt-0.6.0/tutorial/plot_0_introduction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 ##############################################################################
 # To study its eigenvalue spectrum, its size should be a little bit larger.
 
 from skrmt.ensemble import GaussianEnsemble
 
 goe = GaussianEnsemble(beta=1, n=1000)
-goe.plot_eigval_hist(bins=60, interval=(-2,2))
+goe.plot_eigval_hist(bins=60, interval=(-2,2))
```

### Comparing `scikit-rmt-0.5.0/tutorial/plot_1_spectral_laws.py` & `scikit-rmt-0.6.0/tutorial/plot_1_spectral_laws.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 #
 # The *probability density function* (PDF) of the Wigner's Semicircle Law can
 # be studied and plotted using **scikit-rmt** with the
 # **WignerSemicircleDistribution** class.
 
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import WignerSemicircleDistribution
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
 
 x1 = np.linspace(-5, 5, num=1000)
 x2 = np.linspace(-10, 10, num=2000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
@@ -95,15 +95,15 @@
 plt.show()
 
 # Similarly, the *cumulative distribution function* (CDF) of the Wigner's Semicircle
 # Law can also be analyzed and plotted using **WignerSemicircleDistribution** class.
 
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import WignerSemicircleDistribution
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
 
 x1 = np.linspace(-5, 5, num=2000)
 x2 = np.linspace(-10, 10, num=4000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
@@ -146,15 +146,15 @@
 #
 # The probability density function (PDF) and cumulative distribution function (CDF)
 # of the Tracy-Widom Law can be computed and graphically represented using the
 # **TracyWidomDistribution** class from **scikit-rmt**.
 
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import TracyWidomDistribution
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
 
 x = np.linspace(-5, 2, num=1000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
 for beta in [1,2,4]:
@@ -205,15 +205,15 @@
 # size :math:`1 - \frac{1}{\lambda}`.
 #
 # Below we show how we can use the class **MarchenkoPasturDistribution** from **scikit-rmt**
 # to compute, study and illustrate the PDF of the Marchenko-Pastur Law.
 
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import MarchenkoPasturDistribution
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
 
 x1 = np.linspace(0, 4, num=1000)
 x2 = np.linspace(0, 5, num=2000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
@@ -256,15 +256,15 @@
 # The support of :math:`f_M` is the compact interval :math:`(0,1)`.
 #
 # The class ManovaSpectrumDistribution can be used to analyze the PDF and CDF of the
 # spectrum of the Manova random matrices, as exemplified below.
 
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import ManovaSpectrumDistribution
+from skrmt.ensemble.spectral_law import ManovaSpectrumDistribution
 
 plt.rcParams['figure.dpi'] = 100
 
 x1 = np.linspace(0, 1, num=1000)
 x2 = np.linspace(0, 1, num=1000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
```

### Comparing `scikit-rmt-0.5.0/tutorial/plot_2_plot_spectral_laws.py` & `scikit-rmt-0.6.0/tutorial/plot_2_plot_spectral_laws.py`

 * *Files 11% similar despite different names*

```diff
@@ -127,31 +127,34 @@
 ##############################################################################
 # Anyone can forget about the specific plotting details and directly study
 # those laws by using the functions provided in scikit-rmt.
 
 ##############################################################################
 # We can easily analyze **Wigner's Semicircle Law** as follows.
 
-from skrmt.ensemble import wigner_semicircle
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
-wigner_semicircle(ensemble='goe', n_size=2000, bins=80)
+wsd = WignerSemicircleDistribution(beta=1)
+wsd.plot_empirical_pdf(n_size=2000, bins=80)
 
 ##############################################################################
 # We can also study **Marchenko-Pastur Law** as by:
 
-from skrmt.ensemble import marchenko_pastur
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-marchenko_pastur(ensemble='wre', p_size=2000, n_size=6000, bins=80)
+mpd = MarchenkoPasturDistribution(ratio=1/3, beta=1)
+mpd.plot_empirical_pdf(n_size=6000, bins=80)
 
 ##############################################################################
 # Finally, **Tracy-Widom Law** can be represented using:
 
-from skrmt.ensemble import tracy_widom
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
-tracy_widom(ensemble='goe', n_size=100, times=10000, bins=80)
+twd = TracyWidomDistribution(beta=1)
+twd.plot_empirical_pdf(n_size=100, times=10000, bins=80)
 
 ##############################################################################
 # Spectral laws analytical expression
 # -----------------------------------
 # 
 # The spectral laws described so far have been proven to converge to certain
 # analytical functions that defines the limiting behaviour of the eigenvalue
@@ -160,46 +163,49 @@
 # theoretical eigenvalue pdf.
 
 ##############################################################################
 # The analytical probability function for the Gaussian Ensemble, known as
 # Wigner Semicircle Law, supported on :math:`[-R, R]` and centered at :math:`(0,0)`
 # is :math:`f(x) = \frac{2}{\pi R^2} \sqrt{R^2 - x^2}`.
 
-from skrmt.ensemble import wigner_semicircle
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
-wigner_semicircle(ensemble='goe', n_size=2000, bins=80, density=True, plot_law_pdf=True)
+wsd = WignerSemicircleDistribution(beta=1)
+wsd.plot_empirical_pdf(n_size=2000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # The analytical probability function for the Wishart Ensemble known as
 # Marchenko-Pastur Law with parameter :math:`\lambda = p/n \in (0,1]` is
 # :math:`f_{\lambda}(x) = \frac{1}{2\pi \sigma^2}\frac{\sqrt{(\lambda_+ - x)(x - \lambda_-)}}{\lambda x}`,
 # where :math:`\lambda_{\pm} = \sigma^2 (1 \pm \sqrt{\lambda})^2`. 
 # If :math:`\lambda > 1` then the limiting distribution has an additional
 # mass probability point in the origin of size :math:`1 - \frac{1}{\lambda}`.
 
-from skrmt.ensemble import marchenko_pastur
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-marchenko_pastur(ensemble='wre', p_size=2000, n_size=6000, bins=80, density=True, plot_law_pdf=True)
+mpd = MarchenkoPasturDistribution(ratio=1/3, beta=1)
+mpd.plot_empirical_pdf(n_size=6000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # In the other hand, the Tracy-Widom Law has a complex analytical expression,
 # that is the solution of a particular non-linear differential equation, described
 # in detail in:
 # S. Bauman. "The Tracy-Widom Distribution and its Application to Statistical Physics".
 # MIT Department of Physics. 2017.
 # The package scikit-rmt represents a precise
 # approximation of the theoretical Tracy-Widom pdf.
 
-from skrmt.ensemble import tracy_widom
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
-tracy_widom(ensemble='goe', n_size=10, times=5000, bins=80, density=True, plot_law_pdf=True)
+twd = TracyWidomDistribution(beta=1)
+twd.plot_empirical_pdf(n_size=10, times=5000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # Finally, the limiting distribution of the Manova Ensemble is not described
 # by any famous Law, but its expression has been determined. This library
 # provides functionality to show it on top of the empirical histogram of the
 # eigenvalue spectrum.
 
-from skrmt.ensemble import manova_spectrum
+from skrmt.ensemble.spectral_law import ManovaSpectrumDistribution
 
-manova_spectrum(ensemble='mre', m_size=1000, n1_size=3000, n2_size=3000,
-                bins=80, density=True, plot_law_pdf=True)
+msd = ManovaSpectrumDistribution(a=3, b=3, beta=1)
+msd.plot_empirical_pdf(m_size=1000, bins=80, density=True, plot_law_pdf=True)
```

