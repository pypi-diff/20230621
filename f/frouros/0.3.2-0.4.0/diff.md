# Comparing `tmp/frouros-0.3.2.tar.gz` & `tmp/frouros-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.3.2.tar", last modified: Fri Jun  9 07:54:09 2023, max compression
+gzip compressed data, was "frouros-0.4.0.tar", last modified: Wed Jun 21 12:19:19 2023, max compression
```

## Comparing `frouros-0.3.2.tar` & `frouros-0.4.0.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-09 07:53:53.000000 frouros-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 07:53:53.000000 frouros-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    22236 2023-06-09 07:54:09.130316 frouros-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20615 2023-06-09 07:53:53.000000 frouros-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.114316 frouros-0.3.2/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5461 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5329 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    22236 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4703 2023-06-09 07:54:09.000000 frouros-0.3.2/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-09 07:54:09.000000 frouros-0.3.2/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-09 07:53:53.000000 frouros-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 07:54:09.130316 frouros-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-09 07:53:53.000000 frouros-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.294962 frouros-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-21 12:19:04.000000 frouros-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-21 12:19:04.000000 frouros-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    23091 2023-06-21 12:19:19.294962 frouros-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21470 2023-06-21 12:19:04.000000 frouros-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14974 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.294962 frouros-0.4.0/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    23091 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-21 12:19:04.000000 frouros-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 12:19:19.294962 frouros-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-21 12:19:04.000000 frouros-0.4.0/setup.py
```

### Comparing `frouros-0.3.2/LICENSE` & `frouros-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/PKG-INFO` & `frouros-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.2
-Summary: An open source Python library for drift detection in machine learning systems
+Version: 0.4.0
+Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
@@ -51,15 +51,15 @@
   </a>
   <!-- Documentation -->
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
-    <img src="https://static.pepy.tech/badge/frouros/month" alt="downloads"/>
+    <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
@@ -239,20 +239,26 @@
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Numerical (N) / Categorical (C)</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Method</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Reference</th>
     </tr>
   </thead>
   <tbody>
   <tr>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
-    <td rowspan="3" style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
+    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Change detection</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">BOCD</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.48550/arXiv.0710.3742">Adams and MacKay (2007)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUSUM</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2333009">Page (1954)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Geometric moving average</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/1266443">Roberts (1959)</a></td>
@@ -316,16 +322,16 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
     <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
@@ -367,15 +373,15 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">PSI</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1057/jors.2008.144">Wu and Olson (2010)</a></td>
   </tr>
   <tr>
-    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
+    <td rowspan="5" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">C</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Chi-square test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1080/14786440009463897">Pearson (1900)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
@@ -388,15 +394,21 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2280095">Massey Jr (1951)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's T-Test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Mann-Whitney U test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1214/aoms/1177730491">Mann and Whitney (1947)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's t-test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2332510">Welch (1947)</a></td>
   </tr>
   <tr>
     <td rowspan="2" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">M</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.2 Summary: An open source
+Metadata-Version: 2.1 Name: frouros Version: 0.4.0 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -78,24 +78,25 @@
 Installation Frouros can be installed via pip: ```bash pip install frouros ```
 ## ðµð»ââï¸ï¸ Drift detection methods The currently implemented
 detectors are listed in the following table.
                                Univariate   Numerical
 Drift    Type      Family      (U) /        (N) /       Method              Reference
 detector                       Multivariate Categorical
                                (M)          (C)
-                               U            N           CUMSUM              Page_(1954)
-                   CUMSUM      U            N           Geometric moving    Roberts_(1959)
+                               U            N           BOCD                Adams_and_MacKay_(2007)
+                   Change      U            N           CUSUM               Page_(1954)
+                   detection   U            N           Geometric moving    Roberts_(1959)
                                                         average
                                U            N           Page Hinkley        Page_(1954)
                                U            N           DDM                 Gama_et_al._(2004)
                                U            N           ECDD-WT             Ross_et_al._(2012)
                                U            N           EDDM                Baena-GarcÄ±a_et_al._
-                   Statistical                                              (2006)
-Concept  Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
-drift              control                                                  (2014)
+Concept            Statistical                                              (2006)
+drift    Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
+                   control                                                  (2014)
                                U            N           HDDM-W              Frias-Blanco_et_al._
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
@@ -116,15 +117,16 @@
 drift                          M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
-                               U            N           Welch's T-Test      Welch_(1947)
+                               U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
+                               U            N           Welch's t-test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
 ## â What is and what is not Frouros? Unlike other libraries that in addition
 to provide drift detection algorithms, include other functionalities such as
```

### Comparing `frouros-0.3.2/README.md` & `frouros-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   </a>
   <!-- Documentation -->
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
-    <img src="https://static.pepy.tech/badge/frouros/month" alt="downloads"/>
+    <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
@@ -203,20 +203,26 @@
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Numerical (N) / Categorical (C)</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Method</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Reference</th>
     </tr>
   </thead>
   <tbody>
   <tr>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
-    <td rowspan="3" style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
+    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Change detection</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">BOCD</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.48550/arXiv.0710.3742">Adams and MacKay (2007)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUSUM</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2333009">Page (1954)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Geometric moving average</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/1266443">Roberts (1959)</a></td>
@@ -280,16 +286,16 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
     <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
@@ -331,15 +337,15 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">PSI</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1057/jors.2008.144">Wu and Olson (2010)</a></td>
   </tr>
   <tr>
-    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
+    <td rowspan="5" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">C</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Chi-square test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1080/14786440009463897">Pearson (1900)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
@@ -352,15 +358,21 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2280095">Massey Jr (1951)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's T-Test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Mann-Whitney U test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1214/aoms/1177730491">Mann and Whitney (1947)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's t-test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2332510">Welch (1947)</a></td>
   </tr>
   <tr>
     <td rowspan="2" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">M</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
```

#### html2text {}

```diff
@@ -56,24 +56,25 @@
 Installation Frouros can be installed via pip: ```bash pip install frouros ```
 ## ðµð»ââï¸ï¸ Drift detection methods The currently implemented
 detectors are listed in the following table.
                                Univariate   Numerical
 Drift    Type      Family      (U) /        (N) /       Method              Reference
 detector                       Multivariate Categorical
                                (M)          (C)
-                               U            N           CUMSUM              Page_(1954)
-                   CUMSUM      U            N           Geometric moving    Roberts_(1959)
+                               U            N           BOCD                Adams_and_MacKay_(2007)
+                   Change      U            N           CUSUM               Page_(1954)
+                   detection   U            N           Geometric moving    Roberts_(1959)
                                                         average
                                U            N           Page Hinkley        Page_(1954)
                                U            N           DDM                 Gama_et_al._(2004)
                                U            N           ECDD-WT             Ross_et_al._(2012)
                                U            N           EDDM                Baena-GarcÄ±a_et_al._
-                   Statistical                                              (2006)
-Concept  Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
-drift              control                                                  (2014)
+Concept            Statistical                                              (2006)
+drift    Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
+                   control                                                  (2014)
                                U            N           HDDM-W              Frias-Blanco_et_al._
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
@@ -94,15 +95,16 @@
 drift                          M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
-                               U            N           Welch's T-Test      Welch_(1947)
+                               U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
+                               U            N           Welch's t-test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
 ## â What is and what is not Frouros? Unlike other libraries that in addition
 to provide drift detection algorithms, include other functionalities such as
```

### Comparing `frouros-0.3.2/frouros/callbacks/base.py` & `frouros-0.4.0/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/batch/base.py` & `frouros-0.4.0/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/batch/permutation_test.py` & `frouros-0.4.0/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/batch/reset.py` & `frouros-0.4.0/frouros/callbacks/batch/reset.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/streaming/base.py` & `frouros-0.4.0/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/streaming/history.py` & `frouros-0.4.0/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/streaming/msprt.py` & `frouros-0.4.0/frouros/callbacks/streaming/msprt.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.4.0/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/datasets/base.py` & `frouros-0.4.0/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/datasets/real.py` & `frouros-0.4.0/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/datasets/synthetic.py` & `frouros-0.4.0/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/base.py` & `frouros-0.4.0/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/__init__.py` & `frouros-0.4.0/frouros/detectors/concept_drift/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Concept drift detection methods init."""
 
 from .streaming import (
     ADWIN,
     ADWINConfig,
+    BOCD,
+    BOCDConfig,
     CUSUM,
     CUSUMConfig,
     DDM,
     DDMConfig,
     ECDDWT,
     ECDDWTConfig,
     EDDM,
@@ -26,14 +28,16 @@
     STEPD,
     STEPDConfig,
 )
 
 __all__ = [
     "ADWIN",
     "ADWINConfig",
+    "BOCD",
+    "BOCDConfig",
     "CUSUM",
     "CUSUMConfig",
     "DDM",
     "DDMConfig",
     "ECDDWT",
     "ECDDWTConfig",
     "EDDM",
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/base.py` & `frouros-0.4.0/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Concept drift streaming detection methods init."""
 # FIXME: Remove pylint disable if batch methods are added
 # pylint: skip-file
-from .cusum_based import (
+from .change_detection import (
+    BOCD,
+    BOCDConfig,
     CUSUM,
     CUSUMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
     PageHinkley,
     PageHinkleyConfig,
 )
@@ -31,14 +33,16 @@
     STEPD,
     STEPDConfig,
 )
 
 __all__ = [
     "ADWIN",
     "ADWINConfig",
+    "BOCD",
+    "BOCDConfig",
     "CUSUM",
     "CUSUMConfig",
     "DDM",
     "DDMConfig",
     "ECDDWT",
     "ECDDWTConfig",
     "EDDM",
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,35 @@
-"""Base concept drift CUSUM based module."""
+"""Base concept drift ChangeDetection based module."""
 
 import abc
 from typing import List, Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.base import (
     BaseConceptDriftStreaming,
     BaseConceptDriftStreamingConfig,
 )
 from frouros.utils.stats import Mean
 
 
-class BaseCUSUMConfig(BaseConceptDriftStreamingConfig):
+class BaseChangeDetectionConfig(BaseConceptDriftStreamingConfig):
+    """Class representing a ChangeDetection based configuration class."""
+
+
+class BaseChangeDetection(BaseConceptDriftStreaming):
+    """ChangeDetection based algorithm class."""
+
+    config_type = BaseChangeDetectionConfig
+
+    @abc.abstractmethod
+    def _update(self, value: Union[int, float], **kwargs) -> None:
+        pass
+
+
+class BaseCUSUMConfig(BaseChangeDetectionConfig):
     """Class representing a CUSUM based configuration class."""
 
     def __init__(
         self,
         lambda_: float = 50.0,
         min_num_instances: int = 30,
     ) -> None:
@@ -120,15 +134,15 @@
         :raises ValueError: Value error exception
         """
         if not 0.0 <= value <= 1.0:
             raise ValueError("alpha must be in the range [0, 1].")
         self._alpha = value
 
 
-class BaseCUSUM(BaseConceptDriftStreaming):
+class BaseCUSUM(BaseChangeDetection):
     """CUSUM based algorithm class."""
 
     config_type = BaseCUSUMConfig
 
     def __init__(
         self,
         config: Optional[BaseCUSUMConfig] = None,
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-"""CUSUM module."""
+"""Page Hinkley module."""
 
-import numpy as np  # type: ignore
-
-from frouros.detectors.concept_drift.streaming.cusum_based.base import (
+from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseCUSUM,
     BaseCUSUMConfig,
     DeltaConfig,
+    AlphaConfig,
 )
 
 
-class CUSUMConfig(BaseCUSUMConfig, DeltaConfig):
-    """CUSUM [page1954continuous]_ configuration.
+class PageHinkleyConfig(BaseCUSUMConfig, DeltaConfig, AlphaConfig):
+    """Page Hinkley [page1954continuous]_ configuration.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
     """
 
     def __init__(
         self,
         delta: float = 0.005,
         lambda_: float = 50.0,
         min_num_instances: int = 30,
+        alpha: float = 0.9999,
     ) -> None:
         """Init method.
 
         :param delta: delta value
         :type delta: float
-        :param lambda_: delta value
+        :param lambda_: lambda value
         :type lambda_: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
+        :param alpha: forgetting factor value
+        :type alpha: float
         """
         BaseCUSUMConfig.__init__(
-            self, lambda_=lambda_, min_num_instances=min_num_instances
+            self, min_num_instances=min_num_instances, lambda_=lambda_
         )
         DeltaConfig.__init__(self, delta=delta)
+        AlphaConfig.__init__(self, alpha=alpha)
 
 
-class CUSUM(BaseCUSUM):
-    """CUSUM [page1954continuous]_ detector.
+class PageHinkley(BaseCUSUM):
+    """Page Hinkley [page1954continuous]_ detector.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
     """
 
-    config_type = CUSUMConfig  # type: ignore
+    config_type = PageHinkleyConfig  # type: ignore
 
     def _update_sum(self, error_rate: float) -> None:
-        self.sum_ = np.maximum(
-            0,
-            self.sum_
-            + error_rate
-            - self.mean_error_rate.mean
-            - self.config.delta,  # type: ignore
+        self.sum_ = self.config.alpha * self.sum_ + (  # type: ignore
+            error_rate - self.mean_error_rate.mean - self.config.delta  # type: ignore
         )
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Geometric Moving Average module."""
 
-from frouros.detectors.concept_drift.streaming.cusum_based.base import (
+from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseCUSUM,
     BaseCUSUMConfig,
     AlphaConfig,
 )
 
 
 class GeometricMovingAverageConfig(BaseCUSUMConfig, AlphaConfig):
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-"""Page Hinkley module."""
+"""CUSUM module."""
 
-from frouros.detectors.concept_drift.streaming.cusum_based.base import (
+import numpy as np  # type: ignore
+
+from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseCUSUM,
     BaseCUSUMConfig,
     DeltaConfig,
-    AlphaConfig,
 )
 
 
-class PageHinkleyConfig(BaseCUSUMConfig, DeltaConfig, AlphaConfig):
-    """Page Hinkley [page1954continuous]_ configuration.
+class CUSUMConfig(BaseCUSUMConfig, DeltaConfig):
+    """CUSUM [page1954continuous]_ configuration.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
     """
 
     def __init__(
         self,
         delta: float = 0.005,
         lambda_: float = 50.0,
         min_num_instances: int = 30,
-        alpha: float = 0.9999,
     ) -> None:
         """Init method.
 
         :param delta: delta value
         :type delta: float
-        :param lambda_: lambda value
+        :param lambda_: delta value
         :type lambda_: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
-        :param alpha: forgetting factor value
-        :type alpha: float
         """
         BaseCUSUMConfig.__init__(
-            self, min_num_instances=min_num_instances, lambda_=lambda_
+            self, lambda_=lambda_, min_num_instances=min_num_instances
         )
         DeltaConfig.__init__(self, delta=delta)
-        AlphaConfig.__init__(self, alpha=alpha)
 
 
-class PageHinkley(BaseCUSUM):
-    """Page Hinkley [page1954continuous]_ detector.
+class CUSUM(BaseCUSUM):
+    """CUSUM [page1954continuous]_ detector.
 
     :References:
 
     .. [page1954continuous] Page, Ewan S.
         "Continuous inspection schemes."
         Biometrika 41.1/2 (1954): 100-115.
     """
 
-    config_type = PageHinkleyConfig  # type: ignore
+    config_type = CUSUMConfig  # type: ignore
 
     def _update_sum(self, error_rate: float) -> None:
-        self.sum_ = self.config.alpha * self.sum_ + (  # type: ignore
-            error_rate - self.mean_error_rate.mean - self.config.delta  # type: ignore
+        self.sum_ = np.maximum(
+            0,
+            self.sum_
+            + error_rate
+            - self.mean_error_rate.mean
+            - self.config.delta,  # type: ignore
         )
```

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/__init__.py` & `frouros-0.4.0/frouros/detectors/data_drift/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
     KL,
     KSTest,
     PSI,
+    MannWhitneyUTest,
     MMD,
     WelchTTest,
 )
 
 from .streaming import IncrementalKSTest, MMD as MMDStreaming  # noqa: N811
 
 __all__ = [
@@ -25,10 +26,11 @@
     "HellingerDistance",
     "HINormalizedComplement",
     "IncrementalKSTest",
     "JS",
     "KL",
     "KSTest",
     "PSI",
+    "MannWhitneyUTest",
     "MMDStreaming",
     "WelchTTest",
 ]
```

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,26 @@
     PSI,
     MMD,
 )
 from .statistical_test import (
     ChiSquareTest,
     CVMTest,
     KSTest,
+    MannWhitneyUTest,
     WelchTTest,
 )
 
 __all__ = [
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
     "HINormalizedComplement",
     "JS",
     "KL",
     "KSTest",
     "PSI",
+    "MannWhitneyUTest",
     "MMD",
     "WelchTTest",
 ]
```

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Welch's T-test module."""
+"""Welch's t-test module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ttest_ind  # type: ignore
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
@@ -10,15 +10,15 @@
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 
 
 class WelchTTest(BaseStatisticalTest):
-    """Welch's T-test [welch1947generalization]_ detector.
+    """Welch's t-test [welch1947generalization]_ detector.
 
     :References:
 
     .. [welch1947generalization] Welch, Bernard L.
         "The generalization of ‘STUDENT'S’problem when several different population
         varlances are involved."
         Biometrika 34.1-2 (1947): 28-35.
@@ -36,14 +36,24 @@
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
 
     def _statistical_test(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> StatisticalResult:
         test = ttest_ind(
-            a=X_ref, b=X, equal_var=False, alternative="two-sided", **kwargs
+            a=X_ref,
+            b=X,
+            equal_var=False,
+            alternative="two-sided",
+            **kwargs,
+        )
+        test = StatisticalResult(
+            statistic=test.statistic,
+            p_value=test.pvalue,
         )
-        test = StatisticalResult(statistic=test.statistic, p_value=test.pvalue)
         return test
```

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/metrics/base.py` & `frouros-0.4.0/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/metrics/prequential_error.py` & `frouros-0.4.0/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/tests/conftest.py` & `frouros-0.4.0/frouros/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,42 @@
     :return: SEA dataset generator
     :rtype: SEA
     """
     generator = SEA()
     return generator
 
 
+@pytest.fixture(scope="function")
+def stream_drift() -> np.ndarray:
+    """Stream with drift.
+
+    :return: stream with drift
+    :rtype: np.ndarray
+    """
+    np.random.seed(seed=31)
+
+    dist_normal = np.random.normal(
+        loc=0.0,
+        scale=0.5,
+        size=100,
+    )
+    dist_drift_1 = np.random.normal(
+        loc=4.0,
+        scale=0.2,
+        size=100,
+    )
+    dist_drift_2 = np.random.normal(
+        loc=6.0,
+        scale=0.5,
+        size=100,
+    )
+
+    return np.concatenate((dist_normal, dist_drift_1, dist_drift_2))
+
+
 @pytest.fixture(scope="module", name="clf_dataset")
 def classification_dataset() -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """Classification dataset using SEA generator.
 
     :return: classification dataset
     :rtype: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
     """
```

### Comparing `frouros-0.3.2/frouros/tests/integration/test_callback.py` & `frouros-0.4.0/frouros/tests/integration/test_callback.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/tests/integration/test_concept_drift.py` & `frouros-0.4.0/frouros/tests/integration/test_concept_drift.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Test concept drift detectors."""
 
-from typing import Callable, Tuple
+from typing import Callable, List, Tuple
 
 import numpy as np  # type: ignore
 import pytest  # type: ignore
 
 from frouros.detectors.concept_drift import ADWIN, ADWINConfig, KSWIN, KSWINConfig
 from frouros.detectors.concept_drift import (
+    BOCD,
+    BOCDConfig,
     CUSUM,
     CUSUMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
     PageHinkley,
     PageHinkleyConfig,
 )
@@ -27,20 +29,40 @@
     HDDMWConfig,
     RDDM,
     RDDMConfig,
     STEPD,
     STEPDConfig,
 )
 from frouros.detectors.concept_drift.base import BaseConceptDrift
+from frouros.detectors.concept_drift.streaming.change_detection.base import (
+    BaseChangeDetection,
+)
+from frouros.detectors.concept_drift.streaming.change_detection.bocd import (
+    GaussianUnknownMean,
+)
 
 MIN_NUM_INSTANCES = 30
+BOCD_ARGS = {
+    "model": GaussianUnknownMean(
+        prior_mean=0,
+        prior_var=1,
+        data_var=0.5,
+    ),
+    "hazard": 0.01,
+}
 CUMSUM_ARGS = {
     "delta": 0.005,
     "lambda_": 50,
 }
+GEOMETRIC_MOVING_AVERAGE_ARGS = {
+    "alpha": 0.99,
+}
+PAGE_HINKLEY_ARGS = {
+    "alpha": 0.9999,
+}
 HDDM_ARGS = {
     "alpha_w": 0.005,
     "alpha_d": 0.001,
 }
 HDDMW_ARGS = {
     **HDDM_ARGS,
     "lambda_": 0.05,
@@ -50,36 +72,45 @@
 def error_scorer(y_true, y_pred):
     """Error scorer function."""
     return int(1 - y_true == y_pred)
 
 
 detectors = [
     (
+        BOCD(
+            config=BOCDConfig(
+                min_num_instances=MIN_NUM_INSTANCES,
+                **BOCD_ARGS,  # type: ignore
+            ),
+        ),
+        error_scorer,
+    ),
+    (
         CUSUM(
             config=CUSUMConfig(
                 min_num_instances=MIN_NUM_INSTANCES,
                 **CUMSUM_ARGS,
             ),
         ),
         error_scorer,
     ),
     (
         GeometricMovingAverage(
             config=GeometricMovingAverageConfig(
                 min_num_instances=MIN_NUM_INSTANCES,
-                alpha=0.99,
+                **GEOMETRIC_MOVING_AVERAGE_ARGS,
             ),
         ),
         error_scorer,
     ),
     (
         PageHinkley(
             config=PageHinkleyConfig(
                 min_num_instances=MIN_NUM_INSTANCES,
-                alpha=0.9999,
+                **PAGE_HINKLEY_ARGS,
             ),
         ),
         error_scorer,
     ),
     (
         ADWIN(
             config=ADWINConfig(
@@ -218,7 +249,71 @@
     _, _, _, y_test = clf_dataset
     y_pred = train_prediction_normal  # noqa: N806
     detector, value_func = detector_info
 
     for y_sample_pred, y_sample in zip(y_pred, y_test):  # noqa: N806
         value_score = value_func(y_true=y_sample, y_pred=y_sample_pred)
         detector.update(value=value_score)
+
+
+CHANGE_DETECTION_MIN_NUM_INSTANCES = 1
+change_detection_detectors = [
+    (
+        BOCD(
+            config=BOCDConfig(
+                min_num_instances=CHANGE_DETECTION_MIN_NUM_INSTANCES,
+                **BOCD_ARGS,  # type: ignore
+            ),
+        ),
+        [100, 203],
+    ),
+    (
+        CUSUM(
+            config=CUSUMConfig(
+                min_num_instances=CHANGE_DETECTION_MIN_NUM_INSTANCES,
+                **CUMSUM_ARGS,
+            ),
+        ),
+        [113, 226],
+    ),
+    (
+        GeometricMovingAverage(
+            config=GeometricMovingAverageConfig(
+                min_num_instances=CHANGE_DETECTION_MIN_NUM_INSTANCES,
+                **GEOMETRIC_MOVING_AVERAGE_ARGS,
+            ),
+        ),
+        [134],
+    ),
+    (
+        PageHinkley(
+            config=PageHinkleyConfig(
+                min_num_instances=CHANGE_DETECTION_MIN_NUM_INSTANCES,
+                **PAGE_HINKLEY_ARGS,
+            ),
+        ),
+        [113, 227],
+    ),
+]
+
+
+@pytest.mark.parametrize("detector_info", change_detection_detectors)
+def test_streaming_change_detection_detector(
+    stream_drift: np.ndarray,
+    detector_info: Tuple[BaseChangeDetection, List[int]],
+) -> None:
+    """Test streaming change detection detector.
+
+    :param stream_drift: stream with drift
+    :type stream_drift: numpy.ndarray
+    :param detector_info: change detection detector and list of expected drift indices
+    :type detector_info: Tuple[BaseChangeDetection, List[int]]
+    """
+    detector, idx_drifts = detector_info
+    idx_detected_drifts = []
+    for i, val in enumerate(stream_drift):
+        detector.update(value=val)
+        if detector.status["drift"]:
+            detector.reset()
+            idx_detected_drifts.append(i)
+
+    assert idx_detected_drifts == idx_drifts
```

### Comparing `frouros-0.3.2/frouros/tests/integration/test_data_drift.py` & `frouros-0.4.0/frouros/tests/integration/test_data_drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     KL,
     MMD,
 )
 from frouros.detectors.data_drift.batch import (
     ChiSquareTest,
     CVMTest,
     KSTest,
+    MannWhitneyUTest,
     WelchTTest,
 )
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 from frouros.detectors.data_drift.streaming import (  # noqa: N811
     IncrementalKSTest,
     MMD as MMDStreaming,
 )
@@ -157,14 +158,15 @@
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [
         (CVMTest(), 3776.09848103, 5.38105056e-07),
         (KSTest(), 0.99576271, 0.0),
+        (MannWhitneyUTest(), 6912.0, 0.0),
         (WelchTTest(), -287.92032554, 0.0),
     ],
 )
 def test_batch_statistical_univariate(
     elec2_dataset: Tuple[np.ndarray, np.ndarray, np.ndarray],
     detector: BaseDataDriftBatch,
     expected_statistic: float,
```

### Comparing `frouros-0.3.2/frouros/tests/integration/test_real.py` & `frouros-0.4.0/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/tests/integration/test_synthetic.py` & `frouros-0.4.0/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.4.0/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/utils/checks.py` & `frouros-0.4.0/frouros/utils/checks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/utils/data_structures.py` & `frouros-0.4.0/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros/utils/stats.py` & `frouros-0.4.0/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.2/frouros.egg-info/PKG-INFO` & `frouros-0.4.0/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.2
-Summary: An open source Python library for drift detection in machine learning systems
+Version: 0.4.0
+Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
@@ -51,15 +51,15 @@
   </a>
   <!-- Documentation -->
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
-    <img src="https://static.pepy.tech/badge/frouros/month" alt="downloads"/>
+    <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
@@ -239,20 +239,26 @@
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Numerical (N) / Categorical (C)</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Method</th>
     <th style="text-align: center; border: 1px solid grey; padding: 4px;">Reference</th>
     </tr>
   </thead>
   <tbody>
   <tr>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
-    <td rowspan="3" style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Concept drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
+    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Change detection</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUMSUM</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">BOCD</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.48550/arXiv.0710.3742">Adams and MacKay (2007)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">CUSUM</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2333009">Page (1954)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Geometric moving average</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/1266443">Roberts (1959)</a></td>
@@ -316,16 +322,16 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="12" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
     <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
@@ -367,15 +373,15 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">PSI</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1057/jors.2008.144">Wu and Olson (2010)</a></td>
   </tr>
   <tr>
-    <td rowspan="4" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
+    <td rowspan="5" style="text-align: center; border: 1px solid grey; padding: 8px;">Statistical test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">C</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Chi-square test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1080/14786440009463897">Pearson (1900)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
@@ -388,15 +394,21 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2280095">Massey Jr (1951)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
-    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's T-Test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Mann-Whitney U test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1214/aoms/1177730491">Mann and Whitney (1947)</a></td>
+  </tr>
+  <tr>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Welch's t-test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2332510">Welch (1947)</a></td>
   </tr>
   <tr>
     <td rowspan="2" style="text-align: center; border: 1px solid grey; padding: 8px;">Streaming</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">M</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.2 Summary: An open source
+Metadata-Version: 2.1 Name: frouros Version: 0.4.0 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -78,24 +78,25 @@
 Installation Frouros can be installed via pip: ```bash pip install frouros ```
 ## ðµð»ââï¸ï¸ Drift detection methods The currently implemented
 detectors are listed in the following table.
                                Univariate   Numerical
 Drift    Type      Family      (U) /        (N) /       Method              Reference
 detector                       Multivariate Categorical
                                (M)          (C)
-                               U            N           CUMSUM              Page_(1954)
-                   CUMSUM      U            N           Geometric moving    Roberts_(1959)
+                               U            N           BOCD                Adams_and_MacKay_(2007)
+                   Change      U            N           CUSUM               Page_(1954)
+                   detection   U            N           Geometric moving    Roberts_(1959)
                                                         average
                                U            N           Page Hinkley        Page_(1954)
                                U            N           DDM                 Gama_et_al._(2004)
                                U            N           ECDD-WT             Ross_et_al._(2012)
                                U            N           EDDM                Baena-GarcÄ±a_et_al._
-                   Statistical                                              (2006)
-Concept  Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
-drift              control                                                  (2014)
+Concept            Statistical                                              (2006)
+drift    Streaming process     U            N           HDDM-A              Frias-Blanco_et_al._
+                   control                                                  (2014)
                                U            N           HDDM-W              Frias-Blanco_et_al._
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
@@ -116,15 +117,16 @@
 drift                          M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
-                               U            N           Welch's T-Test      Welch_(1947)
+                               U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
+                               U            N           Welch's t-test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
 ## â What is and what is not Frouros? Unlike other libraries that in addition
 to provide drift detection algorithms, include other functionalities such as
```

### Comparing `frouros-0.3.2/frouros.egg-info/SOURCES.txt` & `frouros-0.4.0/frouros.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 frouros/detectors/__init__.py
 frouros/detectors/base.py
 frouros/detectors/concept_drift/__init__.py
 frouros/detectors/concept_drift/base.py
 frouros/detectors/concept_drift/exceptions.py
 frouros/detectors/concept_drift/streaming/__init__.py
 frouros/detectors/concept_drift/streaming/base.py
-frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
-frouros/detectors/concept_drift/streaming/cusum_based/base.py
-frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
-frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
-frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+frouros/detectors/concept_drift/streaming/change_detection/base.py
+frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
 frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
@@ -68,14 +69,15 @@
 frouros/detectors/data_drift/batch/distance_based/mmd.py
 frouros/detectors/data_drift/batch/distance_based/psi.py
 frouros/detectors/data_drift/batch/statistical_test/__init__.py
 frouros/detectors/data_drift/batch/statistical_test/base.py
 frouros/detectors/data_drift/batch/statistical_test/chisquare.py
 frouros/detectors/data_drift/batch/statistical_test/cvm.py
 frouros/detectors/data_drift/batch/statistical_test/ks.py
+frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
 frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
 frouros/detectors/data_drift/streaming/__init__.py
 frouros/detectors/data_drift/streaming/base.py
 frouros/detectors/data_drift/streaming/distance_based/__init__.py
 frouros/detectors/data_drift/streaming/distance_based/base.py
 frouros/detectors/data_drift/streaming/distance_based/mmd.py
 frouros/detectors/data_drift/streaming/statistical_test/__init__.py
```

### Comparing `frouros-0.3.2/pyproject.toml` & `frouros-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "frouros"
-version = "0.3.2"
-description = "An open source Python library for drift detection in machine learning systems"
+version = "0.4.0"
+description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 readme = "README.md"
```

### Comparing `frouros-0.3.2/setup.py` & `frouros-0.4.0/setup.py`

 * *Files identical despite different names*

