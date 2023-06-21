# Comparing `tmp/xsarslc-2023.6.2.tar.gz` & `tmp/xsarslc-2023.6.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarslc-2023.6.2.tar", last modified: Fri Jun  2 08:40:32 2023, max compression
+gzip compressed data, was "xsarslc-2023.6.21.tar", last modified: Wed Jun 21 14:07:42 2023, max compression
```

## Comparing `xsarslc-2023.6.2.tar` & `xsarslc-2023.6.21.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.449012 xsarslc-2023.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.449012 xsarslc-2023.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-02 08:40:00.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VV.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.445012 xsarslc-2023.6.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/ATBD.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/ATBD_L1BSLC.tex
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.445012 xsarslc-2023.6.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/_static/css/xsarslc.css
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/crossspectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/cutoff.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.453012 xsarslc-2023.6.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/default_impulseResponse_files_IW.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/examples/xspec_WV_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_VH.png
--rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_vv.png
--rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_range_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/S1_range_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/figures/index
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/normalizedvariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/docs/sigma0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/get_config_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/get_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/HR_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/deramping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/impulseResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/interburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/intraburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    31595 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/processing/xspectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-06-02 08:40:01.000000 xsarslc-2023.6.2/xsarslc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:40:32.457012 xsarslc-2023.6.2/xsarslc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:40:32.000000 xsarslc-2023.6.2/xsarslc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.170193 xsarslc-2023.6.21/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.170193 xsarslc-2023.6.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.174193 xsarslc-2023.6.21/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/auxdata/S1B_IRs_IW3_VV.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.170193 xsarslc-2023.6.21/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.174193 xsarslc-2023.6.21/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.178193 xsarslc-2023.6.21/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/ATBD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/ATBD_L1BSLC.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.170193 xsarslc-2023.6.21/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.178193 xsarslc-2023.6.21/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/_static/css/xsarslc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/crossspectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/cutoff.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.178193 xsarslc-2023.6.21/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/L1B_Sentinel1_variables_explanation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/default_impulseResponse_files_IW.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/examples/xspec_WV_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.178193 xsarslc-2023.6.21/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/NIRAN_NRCS_VH.png
+-rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/NIRAN_NRCS_vv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/S1_azimuth_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/S1_azimuth_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/S1_range_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/S1_range_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/figures/index
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/normalizedvariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/product_description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/docs/sigma0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/xsarslc/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/get_config_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/get_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/xsarslc/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/HR_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/deramping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/impulseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/interburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32271 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/intraburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33793 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/processing/xspectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/xsarslc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-21 14:07:24.000000 xsarslc-2023.6.21/xsarslc/wallpaper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:07:42.182193 xsarslc-2023.6.21/xsarslc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 14:07:42.000000 xsarslc-2023.6.21/xsarslc.egg-info/top_level.txt
```

### Comparing `xsarslc-2023.6.2/.github/workflows/publish.yml` & `xsarslc-2023.6.21/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/.gitignore` & `xsarslc-2023.6.21/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/.pre-commit-config.yaml` & `xsarslc-2023.6.21/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/LICENSE` & `xsarslc-2023.6.21/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/PKG-INFO` & `xsarslc-2023.6.21/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.6.2
+Version: 2023.6.21
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 xsarslc
 
 
 Functions for Sentinel-1 SLC products 
+
+the main feature of this library is the SAR processor:
+
+
+```mermaid
+graph TD;
+    A[level-1 SLC] -->| SAR processor | B(level-1B XSP);
+```
+
+
 This is a Work In Progress Library.
+
 Disclaimer: no warranty on the quality of output product at this stage.
+
+
 # installation
 ```bash
-git clone https://github.com/umr-lops/xsar_slc
-cd xsar_slc
-pip install .
+pip install git+https://github.com/umr-lops/xsar_slc
 ```
 
 # usage
 ```python
 import xsarslc
 ```
```

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HH.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_HV.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VH.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW1_VV.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VH.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW2_VV.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HH.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_HV.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VH.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1A_IRs_IW3_VV.nc` & `xsarslc-2023.6.21/auxdata/S1A_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HH.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_HV.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VH.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW1_VV.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HH.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_HV.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VH.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW2_VV.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VH.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/auxdata/S1B_IRs_IW3_VV.nc` & `xsarslc-2023.6.21/auxdata/S1B_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/ATBD.rst` & `xsarslc-2023.6.21/docs/ATBD.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/ATBD_L1BSLC.tex` & `xsarslc-2023.6.21/docs/ATBD_L1BSLC.tex`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/Makefile` & `xsarslc-2023.6.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/basic_api.rst` & `xsarslc-2023.6.21/docs/basic_api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 .. automodule:: xsarslc.processing.intraburst
     :members: tile_burst_to_xspectra, compute_intraburst_xspectrum, compute_looks
 
 .. automodule:: xsarslc.processing.interburst
     :members: compute_interburst_xspectrum, tile_bursts_overlap_to_xspectra
 
 .. automodule:: xsarslc.burst
-    :members: burst_valid_indexes, crop_burst, deramp_burst
+    :members: burst_valid_indexes, crop_IW_burst, crop_WV, deramp_burst
 
 .. automodule:: xsarslc.processing.impulseResponse
     :members: compute_IWS_subswath_Impulse_Response, compute_WV_Impulse_Response
```

### Comparing `xsarslc-2023.6.2/docs/conf.py` & `xsarslc-2023.6.21/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,10 +101,12 @@
 .. _github: https://github.com/umr-lops/xsar_slc/tree/main/docs/{{ env.doc2path(env.docname, base=False) }}
 
 ----
 """
 
 today_fmt = '%b %d %Y at %H:%M'
 
+latex_engine='xelatex' #add agrouaze
+
 numfig = True
 # Make sure the target is unique
-autosectionlabel_prefix_document = True
+autosectionlabel_prefix_document = True
```

### Comparing `xsarslc-2023.6.2/docs/crossspectra.rst` & `xsarslc-2023.6.21/docs/crossspectra.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/cutoff.rst` & `xsarslc-2023.6.21/docs/cutoff.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/examples/default_impulseResponse_files_IW.ipynb` & `xsarslc-2023.6.21/docs/examples/default_impulseResponse_files_IW.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.21/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891369047619047%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(10, "#IRs_IW1_VH = '*

 * *            'generate_IWS_AUX_file_ImpulseReponse(subswathes, subswath_number , '*

 * *            'polarization=\'VH\')\\n"), (11, \'#IRs_IW1_VH\')], delete: [11, 10]}}, 6: '*

 * *            "{'source': {insert: [(2, "*

 * *            '"#IRs_IW1_VH[\'range_IR\'].plot(label=\'VH\',alpha=0.7)\\n"), (5, "plt.title(\'burst '*

 * *            '= %s subswath = %s\'%(IRs_IW1_VV.burst.values,IRs_IW1_VV.attrs[\'subswath\']))")], '*

 * *            "delete: [5, 2]}}, 8: {'sourc […]*

```diff
@@ -31,16 +31,16 @@
                 "# SENTINEL1_DS:/home/datawork-cersat-public/cache/project/mpc-sentinel1/data/esa/sentinel-1a/L1/WV/S1A\\_WV\\_SLC\\_\\_1S/2018/050/S1A\\_WV\\_SLC\\_\\_1SSV\\_20180219T221522\\_20180219T222851\\_020681\\_0236CE\\_8F55.SAFE:WV_051\n",
                 "subswathes = {'/home/datawork-cersat-public/cache/project/mpc-sentinel1/data/esa/sentinel-1a/L1/IW/S1A_IW_SLC__1S/2022/271/S1A_IW_SLC__1SDV_20220928T095555_20220928T095622_045203_056722_FB4F.SAFE/':[1],\n",
                 "             }\n",
                 "subswath_number = 1\n",
                 "\n",
                 "IRs_IW1_VV = generate_IWS_AUX_file_ImpulseReponse(subswathes, subswath_number , polarization='VV')\n",
                 "IRs_IW1_VV\n",
-                "IRs_IW1_VH = generate_IWS_AUX_file_ImpulseReponse(subswathes, subswath_number , polarization='VH')\n",
-                "IRs_IW1_VH"
+                "#IRs_IW1_VH = generate_IWS_AUX_file_ImpulseReponse(subswathes, subswath_number , polarization='VH')\n",
+                "#IRs_IW1_VH"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ece558c8-cf71-49c3-8cbe-15564e68300b",
             "metadata": {},
             "source": [
@@ -80,18 +80,18 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from matplotlib import pyplot as plt\n",
                 "IRs_IW1_VV['range_IR'].plot(label='VV')\n",
-                "IRs_IW1_VH['range_IR'].plot(label='VH',alpha=0.7)\n",
+                "#IRs_IW1_VH['range_IR'].plot(label='VH',alpha=0.7)\n",
                 "plt.legend()\n",
                 "plt.grid(True)\n",
-                "plt.title('burst = %s subswath = %s'%(IRs_IW1_VH.burst.values,IRs_IW1_VH.attrs['subswath']))"
+                "plt.title('burst = %s subswath = %s'%(IRs_IW1_VV.burst.values,IRs_IW1_VV.attrs['subswath']))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3db5ce08-40d0-4b4a-872b-6882b7ae76c3",
             "metadata": {},
             "source": [
@@ -105,18 +105,18 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from matplotlib import pyplot as plt\n",
                 "IRs_IW1_VV['azimuth_IR'].plot(label='VV')\n",
-                "IRs_IW1_VH['azimuth_IR'].plot(label='VH',alpha=0.7)\n",
+                "#IRs_IW1_VH['azimuth_IR'].plot(label='VH',alpha=0.7)\n",
                 "plt.legend()\n",
                 "plt.grid(True)\n",
-                "plt.title('burst = %s subswath = %s'%(IRs_IW1_VH.burst.values,IRs_IW1_VH.attrs['subswath']))"
+                "plt.title('burst = %s subswath = %s'%(IRs_IW1_VV.burst.values,IRs_IW1_VV.attrs['subswath']))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "206eaad3-8b01-4ee1-b2e7-2953d292edfe",
             "metadata": {},
             "source": [
@@ -165,43 +165,35 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import xsarslc.processing.xspectra\n",
                 "intra_xs_without_IR = xsarslc.processing.xspectra.compute_IW_subswath_intraburst_xspectra(dt, \n",
-                "                                         tile_width={'sample': 20.e3, 'line': 20.e3},\n",
-                "                                         tile_overlap={'sample': 10.e3, 'line': 10.e3},\n",
+                "                                         tile_width={'sample': 5.e3, 'line': 5.e3},\n",
+                "                                         tile_overlap={'sample': -10.e3, 'line': -10.e3},\n",
                 "                                         periodo_width = {'sample': 4000, 'line': 4000},\n",
                 "                                        periodo_overlap = {'sample': 2000, 'line': 2000},\n",
                 "                                        polarization='VV',dev=True)\n",
                 "intra_xs_without_IR"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4ed97aae-974c-42ba-ba47-7aaa33fd5f51",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "875058c6-55a4-4b83-88b1-bc197684407f",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "IR_path = out_file\n",
                 "intra_xs_with_IR = xsarslc.processing.xspectra.compute_IW_subswath_intraburst_xspectra(dt, \n",
-                "                                         tile_width={'sample': 20.e3, 'line': 20.e3},\n",
-                "                                         tile_overlap={'sample': 10.e3, 'line': 10.e3},\n",
+                "                                         tile_width={'sample': 5.e3, 'line': 5.e3},\n",
+                "                                         tile_overlap={'sample': -10.e3, 'line': -10.e3},\n",
                 "                                         periodo_width = {'sample': 4000, 'line': 4000},\n",
                 "                                        periodo_overlap = {'sample': 2000, 'line': 2000},\n",
                 "                                        polarization='VV',dev=True,IR_path=IR_path)\n",
                 "intra_xs_with_IR"
             ]
         },
         {
@@ -255,13 +247,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsarslc-2023.6.2/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.6.21/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994574238892421%*

 * *Differences: {"'cells'": "{14: {'source': {insert: [(4, '                                          "*

 * *            'polarization=\\\'VV\\\',periodo_width={"line":3000,"sample":3000},\\n\'), (5, '*

 * *            "'                                          "*

 * *            'periodo_overlap={"line":-3000,"sample":-3000})\\n\')], delete: [5, 4]}}, 16: '*

 * *            "{'source': {insert: [(6, '                                          "*

 * *            'polarization=\\\'VV\\\',periodo_width={"line":3000,"sample":3000},\\n\'), (7, '*

 * *      […]*

```diff
@@ -196,16 +196,16 @@
             },
             "outputs": [],
             "source": [
                 "from xsarslc.processing.xspectra import compute_WV_intraburst_xspectra\n",
                 "import time\n",
                 "t0 = time.time()\n",
                 "xs0 = compute_WV_intraburst_xspectra(dt=s1ds.datatree,\n",
-                "                                          polarization='VV',periodo_width={\"line\":2000,\"sample\":2000},\n",
-                "                                          periodo_overlap={\"line\":1000,\"sample\":1000})\n",
+                "                                          polarization='VV',periodo_width={\"line\":3000,\"sample\":3000},\n",
+                "                                          periodo_overlap={\"line\":-3000,\"sample\":-3000})\n",
                 "print('time to compute x-spectra on WV :%1.1f sec'%(time.time()-t0))\n",
                 "xs0"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7da47cba-37a0-4435-b59e-08a72c54d4b0",
@@ -225,16 +225,16 @@
             "source": [
                 "import time\n",
                 "import xsarslc.processing.xspectra\n",
                 "from importlib import reload\n",
                 "reload(xsarslc.processing.xspectra)\n",
                 "t0 = time.time()\n",
                 "xs1 = xsarslc.processing.xspectra.compute_WV_intraburst_xspectra(dt=s1ds.datatree,\n",
-                "                                          polarization='VV',periodo_width={\"line\":2000,\"sample\":2000},\n",
-                "                                          periodo_overlap={\"line\":1000,\"sample\":1000},IR_path=out_file)\n",
+                "                                          polarization='VV',periodo_width={\"line\":3000,\"sample\":3000},\n",
+                "                                          periodo_overlap={\"line\":-3000,\"sample\":-3000},IR_path=out_file)\n",
                 "print('time to compute x-spectra on WV :%1.1f sec'%(time.time()-t0))\n",
                 "xs1"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d8849e56-1bc3-4539-959c-94c9882c7cef",
@@ -251,24 +251,24 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from xsarslc.processing import xspectra\n",
                 "xs = xs0.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})\n",
-                "xs = xspectra.symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az')\n",
+                "xs = xspectra.symmetrize_xspectrum(xs['xspectra_2tau'], dim_range='k_rg', dim_azimuth='k_az')\n",
                 "\n",
                 "xs_ir = xs1.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})\n",
-                "xs_ir = xspectra.symmetrize_xspectrum(xs_ir, dim_range='k_rg', dim_azimuth='k_az')\n",
+                "xs_ir = xspectra.symmetrize_xspectrum(xs_ir['xspectra_2tau'], dim_range='k_rg', dim_azimuth='k_az')\n",
                 "\n",
                 "############################################ real part ############################\n",
-                "coS=np.abs(xs['xspectra_2tau'].mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
+                "coS=np.abs(xs.mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
                 "coS_reduced = coS.where(np.logical_and(np.abs(coS.k_rg)<=0.14, np.abs(coS.k_az)<=0.14), drop=True)\n",
                 "\n",
-                "coS_IRcor=np.abs(xs['xspectra_2tau'].mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
+                "coS_IRcor=np.abs(xs_ir.mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
                 "coS_reduced_IRcor = coS_IRcor.where(np.logical_and(np.abs(coS_IRcor.k_rg)<=0.14, np.abs(coS_IRcor.k_az)<=0.14), drop=True)\n",
                 "from matplotlib import pyplot as plt\n",
                 "%matplotlib inline\n",
                 "from matplotlib import colors as mcolors\n",
                 "cmap = mcolors.LinearSegmentedColormap.from_list(\"\", [\"white\",\"violet\",\"mediumpurple\",\"cyan\",\"springgreen\",\"yellow\",\"red\"])\n",
                 "PuOr = plt.get_cmap('PuOr')\n",
                 "plt.figure(figsize=(16,12))\n",
@@ -288,17 +288,17 @@
                 "\n",
                 "plt.grid()\n",
                 "plt.xticks(fontsize=20)\n",
                 "plt.yticks(fontsize=20)\n",
                 "plt.axis('scaled')\n",
                 "\n",
                 "############################################ imag.part ############################\n",
-                "ims = xs['xspectra_2tau'].mean(dim='2tau').imag.squeeze()\n",
+                "ims = xs.mean(dim='2tau').imag.squeeze()\n",
                 "xS_red = ims.where(np.logical_and(np.abs(ims.k_rg)<=0.14, np.abs(ims.k_az)<=0.14), drop=True)\n",
-                "ims_irCor = xs_ir['xspectra_2tau'].mean(dim='2tau').imag.squeeze()\n",
+                "ims_irCor = xs_ir.mean(dim='2tau').imag.squeeze()\n",
                 "xS_red_IRCor = ims_irCor.where(np.logical_and(np.abs(ims_irCor.k_rg)<=0.14, np.abs(ims_irCor.k_az)<=0.14), drop=True)\n",
                 "#xS_av=xS_red.rolling(k_rg=3, center=True).mean().rolling(k_az=3, center=True).mean()\n",
                 "\n",
                 "plt.figure(figsize=(16,12))\n",
                 "plt.subplot(1,2,1)\n",
                 "xS_red.plot(x='k_rg',cmap=PuOr)\n",
                 "plt.grid()\n",
@@ -330,24 +330,24 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from xsarslc.processing import xspectra\n",
                 "xs = xs0.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})\n",
-                "xs = xspectra.symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az')\n",
+                "xs = xspectra.symmetrize_xspectrum(xs['xspectra_2tau'], dim_range='k_rg', dim_azimuth='k_az')\n",
                 "\n",
                 "xs_ir = xs1.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})\n",
-                "xs_ir = xspectra.symmetrize_xspectrum(xs_ir, dim_range='k_rg', dim_azimuth='k_az')\n",
+                "xs_ir = xspectra.symmetrize_xspectrum(xs_ir['xspectra_2tau'], dim_range='k_rg', dim_azimuth='k_az')\n",
                 "\n",
                 "############################################ real part ############################\n",
-                "coS=np.abs(xs['xspectra_2tau'].mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
+                "coS=np.abs(xs.mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
                 "coS_reduced = coS.where(np.logical_and(np.abs(coS.k_rg)<=0.14, np.abs(coS.k_az)<=0.14), drop=True)\n",
                 "\n",
-                "coS_IRcor=np.abs(xs['xspectra_2tau'].mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
+                "coS_IRcor=np.abs(xs_ir.mean(dim='2tau').real) # co spectrum = real part of cross-spectrum\n",
                 "coS_reduced_IRcor = coS_IRcor.where(np.logical_and(np.abs(coS_IRcor.k_rg)<=0.14, np.abs(coS_IRcor.k_az)<=0.14), drop=True)\n",
                 "from matplotlib import pyplot as plt\n",
                 "%matplotlib inline\n",
                 "from matplotlib import colors as mcolors\n",
                 "cmap = mcolors.LinearSegmentedColormap.from_list(\"\", [\"white\",\"violet\",\"mediumpurple\",\"cyan\",\"springgreen\",\"yellow\",\"red\"])\n",
                 "PuOr = plt.get_cmap('PuOr')\n",
                 "plt.figure(figsize=(8,6))\n",
@@ -360,17 +360,17 @@
                 "plt.grid()\n",
                 "plt.xticks(fontsize=20)\n",
                 "plt.yticks(fontsize=20)\n",
                 "plt.axis('scaled')\n",
                 "\n",
                 "\n",
                 "############################################ imag.part ############################\n",
-                "ims = xs['xspectra_2tau'].mean(dim='2tau').imag.squeeze()\n",
+                "ims = xs.mean(dim='2tau').imag.squeeze()\n",
                 "xS_red = ims.where(np.logical_and(np.abs(ims.k_rg)<=0.14, np.abs(ims.k_az)<=0.14), drop=True)\n",
-                "ims_irCor = xs_ir['xspectra_2tau'].mean(dim='2tau').imag.squeeze()\n",
+                "ims_irCor = xs_ir.mean(dim='2tau').imag.squeeze()\n",
                 "xS_red_IRCor = ims_irCor.where(np.logical_and(np.abs(ims_irCor.k_rg)<=0.14, np.abs(ims_irCor.k_az)<=0.14), drop=True)\n",
                 "#xS_av=xS_red.rolling(k_rg=3, center=True).mean().rolling(k_az=3, center=True).mean()\n",
                 "\n",
                 "plt.figure(figsize=(8,6))\n",
                 "plt.subplot(1,1,1)\n",
                 "(xS_red-xS_red_IRCor).plot(x='k_rg',cmap=PuOr)\n",
                 "plt.grid()\n",
```

### Comparing `xsarslc-2023.6.2/docs/examples/xspec_IW_intra_and_inter_burst.ipynb` & `xsarslc-2023.6.21/docs/examples/xspec_IW_intra_and_inter_burst.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/examples/xspec_WV_example.ipynb` & `xsarslc-2023.6.21/docs/examples/xspec_WV_example.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976100288600289%*

 * *Differences: {"'cells'": '{10: {\'source\': {insert: [(3, "xs = '*

 * *            "xspectra.symmetrize_xspectrum(xs['xspectra_2tau'], dim_range='k_rg', "*

 * *            'dim_azimuth=\'k_az\')\\n"), (6, "coS=np.abs(xs.mean(dim=\'2tau\').real) \\n"), (23, '*

 * *            '"ims = xs.mean(dim=\'2tau\').imag.squeeze()\\n")], delete: [23, 6, 3]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -148,18 +148,18 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from xsarslc.processing import xspectra\n",
                 "xs = xs0.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})\n",
-                "xs = xspectra.symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az')\n",
+                "xs = xspectra.symmetrize_xspectrum(xs['xspectra_2tau'], dim_range='k_rg', dim_azimuth='k_az')\n",
                 "\n",
                 "############################################ real part ############################\n",
-                "coS=np.abs(xs['xspectra_2tau'].mean(dim='2tau').real) \n",
+                "coS=np.abs(xs.mean(dim='2tau').real) \n",
                 "coS_reduced = coS.where(np.logical_and(np.abs(coS.k_rg)<=0.14, np.abs(coS.k_az)<=0.14), drop=True)\n",
                 "from matplotlib import pyplot as plt\n",
                 "%matplotlib inline\n",
                 "from matplotlib import colors as mcolors\n",
                 "cmap = mcolors.LinearSegmentedColormap.from_list(\"\", [\"white\",\"violet\",\"mediumpurple\",\"cyan\",\"springgreen\",\"yellow\",\"red\"])\n",
                 "PuOr = plt.get_cmap('PuOr')\n",
                 "plt.figure(figsize=(8,6))\n",
@@ -168,15 +168,15 @@
                 "\n",
                 "plt.grid()\n",
                 "plt.xticks(fontsize=20)\n",
                 "plt.yticks(fontsize=20)\n",
                 "plt.axis('scaled')\n",
                 "\n",
                 "############################################ imag.part ############################\n",
-                "ims = xs['xspectra_2tau'].mean(dim='2tau').imag.squeeze()\n",
+                "ims = xs.mean(dim='2tau').imag.squeeze()\n",
                 "xS_red = ims.where(np.logical_and(np.abs(ims.k_rg)<=0.14, np.abs(ims.k_az)<=0.14), drop=True)\n",
                 "#xS_av=xS_red.rolling(k_rg=3, center=True).mean().rolling(k_az=3, center=True).mean()\n",
                 "\n",
                 "plt.figure(figsize=(8,6))\n",
                 "xS_red.plot(x='k_rg',cmap=PuOr)\n",
                 "plt.grid()\n",
                 "plt.xticks(fontsize=20)\n",
@@ -197,13 +197,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_VH.png` & `xsarslc-2023.6.21/docs/figures/NIRAN_NRCS_VH.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/figures/NIRAN_NRCS_vv.png` & `xsarslc-2023.6.21/docs/figures/NIRAN_NRCS_vv.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_IW_VV.png` & `xsarslc-2023.6.21/docs/figures/S1_azimuth_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/figures/S1_azimuth_IR_WV_VV.png` & `xsarslc-2023.6.21/docs/figures/S1_azimuth_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/figures/S1_range_IR_IW_VV.png` & `xsarslc-2023.6.21/docs/figures/S1_range_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/figures/S1_range_IR_WV_VV.png` & `xsarslc-2023.6.21/docs/figures/S1_range_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/index.rst` & `xsarslc-2023.6.21/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 .....................................
 
 .. note::
     The Algorithm Technical Baseline Document (ATBD) describes implemented processing steps from Sentinel-1 SLC product to cross spectra
 
 * :doc:`ATBD`
 
+Sentinel-1 Level-1B IFREMER Product Description
+...............................................
+
+.. note::
+    It describes the format, the files and the content of Level-1B SAR product.
+
+* :doc:`product_description`
+
 Examples
 ........
 
 .. note::
     here are some examples of usage
 
 * :doc:`examples/xspec_IW_intra_and_inter_burst`
@@ -96,14 +104,21 @@
 .. toctree::
    :maxdepth: 18
    :hidden:
    :caption: Algorithm description
 
    ATBD
 
+.. toctree::
+   :maxdepth: 1
+   :hidden:
+   :caption: Level-1B product description
+
+   product_description
+
 
 .. toctree::
    :maxdepth: 1
    :hidden:
    :caption: Examples
 
    examples/xspec_IW_intra_and_inter_burst
@@ -111,14 +126,21 @@
    examples/example_IW_compute_and_correct_from_impulse_response
    examples/example_WV_compute_and_correct_from_impulse_response
    examples/default_impulseResponse_files_IW
 
 .. toctree::
    :maxdepth: 1
    :hidden:
+   :caption: extra explanations
+
+    examples/L1B_Sentinel1_variables_explanation
+
+.. toctree::
+   :maxdepth: 1
+   :hidden:
    :caption: Reference
 
    basic_api
 
 .. _on github: https://github.com/umr-lops/xsar_slc
 .. _xsar: https://github.com/umr-lops/xsar
 .. _xarray: http://xarray.pydata.org
```

### Comparing `xsarslc-2023.6.2/docs/installing.rst` & `xsarslc-2023.6.21/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/normalizedvariance.rst` & `xsarslc-2023.6.21/docs/normalizedvariance.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/oceanspectrumSAR.png` & `xsarslc-2023.6.21/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/docs/sigma0.rst` & `xsarslc-2023.6.21/docs/sigma0.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/pyproject.toml` & `xsarslc-2023.6.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/burst.py` & `xsarslc-2023.6.21/xsarslc/burst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/config.yml` & `xsarslc-2023.6.21/xsarslc/config.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/get_config_infos.py` & `xsarslc-2023.6.21/xsarslc/get_config_infos.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/get_test_files.py` & `xsarslc-2023.6.21/xsarslc/get_test_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,16 +49,20 @@
     res_path = config['data_dir']
     base_url = 'https://cyclobs.ifremer.fr/static/sarwing_datarmor/xsardata'
     file_url = '%s/%s.zip' % (base_url, fname)
     if not os.path.exists(os.path.join(res_path, fname)):
         warnings.warn("Downloading %s" % file_url)
         local_file = url_get(file_url)
         warnings.warn("Unzipping %s" % os.path.join(res_path, fname))
-        with zipfile.ZipFile(local_file, 'r') as zip_ref:
-            zip_ref.extractall(res_path)
+        if os.path.splitext(local_file)[1]=='.nc':
+            with zipfile.ZipFile(local_file, 'r') as zip_ref:
+                zip_ref.extract(res_path)
+        else:
+            with zipfile.ZipFile(local_file, 'r') as zip_ref:
+                zip_ref.extractall(res_path)
     return os.path.join(res_path, fname)
 
 def url_get(url, cache_dir=os.path.join(config['data_dir'], 'fsspec_cache')):
     """
     Get fil from url, using caching.
 
     Parameters
```

### Comparing `xsarslc-2023.6.2/xsarslc/interface.py` & `xsarslc-2023.6.21/xsarslc/interface.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/processing/HR_tiles.py` & `xsarslc-2023.6.21/xsarslc/processing/HR_tiles.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/processing/deramping.py` & `xsarslc-2023.6.21/xsarslc/processing/deramping.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/processing/impulseResponse.py` & `xsarslc-2023.6.21/xsarslc/processing/impulseResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,37 @@
         IRs.append(myIRs)
 
     IRs = xr.concat(IRs, dim='tile', combine_attrs='drop_conflicts')
     IRs = IRs.swap_dims({'freq_line':'k_az', 'freq_sample':'k_srg'})
     IRs.attrs.update({'subswath':'IW'+str(subswath_number)})
     return IRs.mean(dim='tile', keep_attrs=True)
 
+def generate_EWS_AUX_file_ImpulseReponse(subswathes, subswath_number,polarization):
+    """
+    Compute IR for each file listed in subswathes. Average over all files, bursts, tiles and returm mean range and azimuth Impulse Response.
+    All listed subswath/burst should be on homogeneous zone
+
+    Args:
+        subswathes (dict): keys are SAFE file path (str), and values are list of burst number. Ex {'/home/my_directory/my_file.SAFE', [0,2,6]}
+        subswath_number (int): subswath number to process. In [1,2,3,4,5]
+        polarization (str) : VV or VH or HV or HH
+    """
+    import xsar
+    IRs = list()
+    for SAFE_path, burst_list in subswathes.items():
+        slc_ew_path = 'SENTINEL1_DS:'+SAFE_path+':EW'+str(subswath_number)
+        dt = xsar.open_datatree(slc_ew_path)
+        myIRs = compute_IWS_subswath_Impulse_Response(dt, burst_list = burst_list , polarization=polarization)
+        IRs.append(myIRs)
+
+    IRs = xr.concat(IRs, dim='tile', combine_attrs='drop_conflicts')
+    IRs = IRs.swap_dims({'freq_line':'k_az', 'freq_sample':'k_srg'})
+    IRs.attrs.update({'subswath':'EW'+str(subswath_number)})
+    return IRs.mean(dim='tile', keep_attrs=True)
+
 def generate_WV_AUX_file_ImpulseReponse(subswathes):
     """
     Compute IR for each file listed in subswathes. Average over all files, bursts, tiles and returm mean range and azimuth Impulse Response.
     All listed subswath/burst should be on homogeneous zone
 
     Args:
         subswathes (dict): keys are SAFE file path (str), and values are list of burst number. Ex {'/home/my_directory/my_file.SAFE', [0,2,6]}
```

### Comparing `xsarslc-2023.6.2/xsarslc/processing/interburst.py` & `xsarslc-2023.6.21/xsarslc/processing/interburst.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,52 +4,49 @@
 """
 import numpy as np
 import xarray as xr
 import logging
 from scipy.constants import c as celerity
 from xsarslc.tools import xtiling, xndindex
 import warnings
-
+import pdb
 def tile_bursts_overlap_to_xspectra(burst0, burst1, geolocation_annotation, calibration, noise_range, noise_azimuth, tile_width, tile_overlap,
                                     lowpass_width={'sample': 4750., 'line': 4750.},
                                     periodo_width={'sample': 2000., 'line': 1200.}, #2000 1200 en 20km# 1800 1200 en 2km
                                     periodo_overlap={'sample': 1000., 'line': 600.},
                                     landmask=None, IR_path=None, **kwargs):
     """
     Divide bursts overlaps in tiles and compute inter-burst cross-spectra using compute_interburst_xspectrum() function.
 
     Args:
         burst0 (xarray.Dataset): first burst (in time) dataset (No need of deramped digital number variable)
         burst1 (xarray.Dataset): second burst (in time) dataset (No need of deramped digital number variable)
         geolocation_annotation (xarray.Dataset): dataset of geolocation annotation
         tile_width (dict): approximative sizes of tiles in meters. Dict of shape {dim_name (str): width of tile [m](float)}
         tile_overlap (dict): approximative sizes of tiles overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)}
-        azimuth_steering_rate (float) : antenna azimuth steering rate [deg/s]
-        azimuth_time_interval (float) : azimuth time spacing [s]
         lowpass_width (dict): width for low pass filtering [m]. Dict of form {dim_name (str): width (float)}
-        landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
+        landmask (optional) : If provided, land mask passed to is_ocean(). None -> xspectra are calculated by default. True -> no xspectra computed.
         IR_path (str, optional) : a path to the Impulse Response file
     Keyword Args:
         kwargs: keyword arguments passed to compute_interburst_xspectrum()
     """
     from xsarslc.tools import get_tiles, get_corner_tile, get_middle_tile, is_ocean, FullResolutionInterpolation, haversine
-    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest
+    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest, get_bright_target_mask
 
     # ------------------ preprocessing --------------
     azitime_interval = burst0.attrs['azimuth_time_interval']
     azimuth_spacing = float(burst0['lineSpacing'])
 
     # -------- find overlapping burst portion -----------
 
     az0 = burst0['time'].load()
     az1 = burst1['time'][{'line': 0}].load()
 
     # az0 = burst0[{'sample':0}].azimuth_time.load()
     # az1 = burst1.isel(sample=0).azimuth_time[{'line':0}].load()
-
     frl = np.argwhere(az0.data >= az1.data)[0].item()  # first overlapping line of first burst
     # Lines below ensures we choose the closest index since azimuth_time are not exactly the same
     t0 = burst0[{'sample': 0, 'line': frl}].time
     t1 = burst1[{'sample': 0, 'line': 0}].time
     aziTimeDiff = np.abs(t0 - t1)
 
     if np.abs(burst0[{'sample': 0, 'line': frl - 1}].time - t1) < aziTimeDiff:
@@ -125,15 +122,15 @@
     iends = np.searchsorted(cumulative_len,ends, side='left') # index of ending of tiles
     tile_sample = {'sample':xr.DataArray([slice(s,min(e+1,burst.sizes['sample'])) for s,e in zip(istarts,iends)], dims='tile_sample')}#, coords={'tile_sample':[(e+s)//2 for s,e in zip(istarts,iends)]})} # This is custom tile indexing along sample dimension to preserve constant tile width
     tile_sample_coords = get_middle_tile(tile_sample)
     tile_sample['sample'] = tile_sample['sample'].assign_coords({'tile_sample':burst['sample'][tile_sample_coords]})
 
 
     # ------------- defining regular line indexing --------
-    tile_line = xtiling(burst['line'], nperseg=nperseg_tile, noverlap=noverlap_tile) # homogeneous tiling along line dimension can be done using xtiling()
+    tile_line = xtiling(burst['line'], nperseg=nperseg_tile, noverlap=noverlap_tile,centering=True) # homogeneous tiling along line dimension can be done using xtiling()
 
     # ------------- customized indexes --------
     tiles_index = tile_sample.copy()
     tiles_index.update(tile_line)
 
     # ----- getting all tiles ------
     all_tiles_0 = get_tiles(burst0, tiles_index)
@@ -185,15 +182,15 @@
 
         # ------ checking if we are over water only ------
         if landmask:
             tile_lons = [float(corner_lons.sel(mytile)[{'c_line': j, 'c_sample': k}]) for j, k in
                          [(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]]
             tile_lats = [float(corner_lats.sel(mytile)[{'c_line': j, 'c_sample': k}]) for j, k in
                          [(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]]
-            water_only = is_ocean((tile_lons, tile_lats), landmask)
+            water_only = False if landmask is True else is_ocean((tile_lons, tile_lats), landmask)
             landflag.append(xr.DataArray(not water_only, coords=mytile, name='land_flag'))
         else:
             water_only = True
             # landflag.append(xr.DataArray(np.nan, coords=mytile, name='land_flag'))
     
         # ------------------------------------------------
         sub = sub0
@@ -201,57 +198,79 @@
         mean_incidence = float(corner_incs.sel(mytile).mean())
         mean_slant_range = float(corner_slantTimes.sel(mytile).mean()) * celerity / 2.
         slant_spacing = float(sub['sampleSpacing'])
         ground_spacing = slant_spacing / np.sin(np.radians(mean_incidence))
         azimuth_spacing = float(sub['lineSpacing'])
 
 
-        mod0 = compute_modulation(np.abs(sub0['digital_number']), lowpass_width=lowpass_width,
+        DN0 = sub0['digital_number']
+        DN1 = sub1['digital_number']
+        # ------------- Bright target processing -----------------------
+        if water_only: # Bright target mask is applied only on water 
+            bright_target_mask0, hist_bright0 = get_bright_target_mask(np.abs(DN0), targetsize={'line':5,'sample':5}, guardsize={'line':350,'sample':350}, cluttersize={'line':1000,'sample':1000}, spacing={'line':azimuth_spacing, 'sample':ground_spacing}, nstddev=10,itermax=10, nstddev_neigh=5)
+            bright_target_mask1, hist_bright1 = get_bright_target_mask(np.abs(DN1), targetsize={'line':5,'sample':5}, guardsize={'line':350,'sample':350}, cluttersize={'line':1000,'sample':1000}, spacing={'line':azimuth_spacing, 'sample':ground_spacing}, nstddev=10,itermax=10, nstddev_neigh=5)
+            mean_DN0 = DN0.where(~bright_target_mask0, 1j*np.nan).mean(skipna=True)
+            mean_DN1 = DN1.where(~bright_target_mask1, 1j*np.nan).mean(skipna=True)
+            DN0 = DN0.where(~bright_target_mask0, mean_DN0)
+            DN1 = DN1.where(~bright_target_mask1, mean_DN1)
+            variables_list+=[hist_bright0.to_dataset()]
+
+
+        mod0 = compute_modulation(np.abs(DN0), lowpass_width=lowpass_width,
                                   spacing={'sample': ground_spacing, 'line': azimuth_spacing})
         # ------------- nv ------------
         nv = compute_normalized_variance(mod0)
         # ------------- mean sigma0 and nesz ------------
-        sigma0, nesz = compute_mean_sigma0_interp(sub0['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
-        sigma0_overlap, _ = compute_mean_sigma0_interp(sub1['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        sigma0, nesz = compute_mean_sigma0_interp(DN0, calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        sigma0_overlap, _ = compute_mean_sigma0_interp(DN1, calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         sigma0_overlap = sigma0_overlap.rename(sigma0_overlap.name+'_overlap').drop('burst')
         sigma0_overlap.attrs.update({'long_name':sigma0_overlap.attrs['long_name']+' (latest burst overlap)'})
         if not np.isfinite(sigma0): # should only append in IW mode. Case when line are badly indexed in noise-range LUT
-            sigma0, nesz = compute_mean_sigma0_closest(sub0['digital_number'], burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+            sigma0, nesz = compute_mean_sigma0_closest(DN0, burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         # ------------- mean incidence ------------
         mean_incidence = xr.DataArray(mean_incidence, name='incidence', attrs={'long_name':'incidence at tile middle', 'units':'degree'})
         # ------------- heading ------------
         _,heading = haversine(float(corner_lons.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lons.sel(mytile)[{'c_line': 1, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 1, 'c_sample': 0}]))
         ground_heading = xr.DataArray(float(heading), name='ground_heading', attrs={'long_name':'ground heading', 'units':'degree', 'convention':'from North clockwise'})
 
+        # ------------- sensing time of the tile (first burst)------------
+        antenna_velocity = np.radians(sub.attrs['azimuth_steering_rate']) * mean_slant_range
+        ground_velocity = azimuth_spacing / sub.attrs['azimuth_time_interval']
+        scan_velocity = (ground_velocity + antenna_velocity).item()
+        dist = (sub[{'line': sub.sizes['line'] // 2}]['line'] - sub['linesPerBurst'] * sub['burst']) * azimuth_spacing  # distance from begining of the burst
+        t_tile = (sub['sensingTime'])+ np.timedelta64(int(1.e3*dist.data / scan_velocity), 'ms')
+        t_tile = xr.DataArray(t_tile, name='sensing_time', attrs={'long_name': 'tile first sensing time'})
+
+
         # ---------------- part of the variables to be added to the final dataset ----------------------
-        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), sigma0_overlap.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
+        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), sigma0_overlap.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset(), t_tile.to_dataset()]
 
         if water_only:
 
             periodo_spacing = {'sample': ground_spacing, 'line': azimuth_spacing}
             nperseg_periodo = {d: int(np.rint(periodo_width[d] / periodo_spacing[d])) for d in tile_width.keys()}
             noverlap_periodo = {d: int(np.rint(periodo_overlap[d] / periodo_spacing[d])) for d in tile_width.keys()}
 
             if np.any([sub0.sizes[d] < nperseg_periodo[d] for d in ['line', 'sample']]):
                 raise ValueError(
                     'periodo_width ({}) is too large compared to available data (line : {} m, sample : {} m).'.format(
                         periodo_width, sub0.sizes['line'] * azimuth_spacing, sub0.sizes['sample'] * ground_spacing))
 
 
-            mod1 = compute_modulation(np.abs(sub1['digital_number']), lowpass_width=lowpass_width,
+            mod1 = compute_modulation(np.abs(DN1), lowpass_width=lowpass_width,
                                       spacing={'sample': ground_spacing, 'line': azimuth_spacing})
 
             xspecs = compute_interburst_xspectrum(mod0 ** 2, mod1 ** 2, float(mean_incidence), slant_spacing, azimuth_spacing,
                                                   nperseg=nperseg_periodo, noverlap=noverlap_periodo, **kwargs)
             xspecs_m = xspecs.mean(dim=['periodo_line', 'periodo_sample'],
                                    keep_attrs=True)  # averaging all the periodograms in each tile
             # ------------- tau ------------------
-            antenna_velocity = np.radians(sub.attrs['azimuth_steering_rate']) * mean_slant_range
-            ground_velocity = azimuth_spacing / sub.attrs['azimuth_time_interval']
-            scan_velocity = (ground_velocity + antenna_velocity).item()
+            # antenna_velocity = np.radians(sub.attrs['azimuth_steering_rate']) * mean_slant_range
+            # ground_velocity = azimuth_spacing / sub.attrs['azimuth_time_interval']
+            # scan_velocity = (ground_velocity + antenna_velocity).item()
             dist0 = (sub0[{'line': sub0.sizes['line'] // 2}]['line'] - sub0['linesPerBurst'] * sub0[
                 'burst']) * azimuth_spacing  # distance from begining of the burst
             dist1 = (sub1[{'line': sub1.sizes['line'] // 2}]['line'] - sub1['linesPerBurst'] * sub1[
                 'burst']) * azimuth_spacing  # distance from begining of the burst
             tau = (sub1['sensingTime'] - sub0['sensingTime']) / np.timedelta64(1, 's') + (
                         dist1 - dist0) / scan_velocity  # The division by timedelta64(1,s) is to convert in seconds
             tau = xr.DataArray(float(tau), name='tau', attrs={'long_name': 'delay between two successive acquisitions', 'units': 's'})
```

### Comparing `xsarslc-2023.6.2/xsarslc/processing/intraburst.py` & `xsarslc-2023.6.21/xsarslc/processing/intraburst.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 # coding=utf-8
 """
 """
+import pdb
+
 import numpy as np
 import xarray as xr
 import logging
 from scipy.constants import c as celerity
 from xsarslc.tools import xtiling, xndindex
 import warnings
 from tqdm import tqdm
@@ -31,15 +33,15 @@
         landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
         IR_path (str, optional) : a path to the Impulse Response file
     Keyword Args:
         landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
         kwargs: keyword arguments passed to compute_intraburst_xspectrum()
     """
     from xsarslc.tools import get_tiles, get_corner_tile, get_middle_tile, is_ocean, FullResolutionInterpolation, haversine
-    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest
+    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest, get_bright_target_mask
 
 
 
     # burst.load()
 
     # ------------------ preprocessing --------------
     azitime_interval = burst.attrs['azimuth_time_interval']
@@ -97,15 +99,15 @@
     istarts = np.searchsorted(cumulative_len,starts, side='right') # index of begining of tiles
     iends = np.searchsorted(cumulative_len,ends, side='left') # index of ending of tiles
     tile_sample = {'sample':xr.DataArray([slice(s,min(e+1,burst.sizes['sample'])) for s,e in zip(istarts,iends)], dims='tile_sample')}#, coords={'tile_sample':[(e+s)//2 for s,e in zip(istarts,iends)]})} # This is custom tile indexing along sample dimension to preserve constant tile width
     tile_sample_coords = get_middle_tile(tile_sample)
     tile_sample['sample'] = tile_sample['sample'].assign_coords({'tile_sample':burst['sample'][tile_sample_coords]})
 
     # ------------- defining regular line indexing --------
-    tile_line = xtiling(burst['line'], nperseg=nperseg_tile, noverlap=noverlap_tile) # homogeneous tiling along line dimension can be done using xtiling()
+    tile_line = xtiling(burst['line'], nperseg=nperseg_tile, noverlap=noverlap_tile,centering=True) # homogeneous tiling along line dimension can be done using xtiling()
 
     # ------------- customized indexes --------
     tiles_index = tile_sample.copy()
     tiles_index.update(tile_line)
 
     # ----- getting all tiles ------
     all_tiles = get_tiles(burst, tiles_index)
@@ -165,47 +167,71 @@
 
         # ------ checking if we are over water only ------
         if landmask:
             tile_lons = [float(corner_lons.sel(mytile)[{'c_line': j, 'c_sample': k}]) for j, k in
                          [(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]]
             tile_lats = [float(corner_lats.sel(mytile)[{'c_line': j, 'c_sample': k}]) for j, k in
                          [(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)]]
-            water_only = is_ocean((tile_lons, tile_lats), landmask)
+            water_only = False if landmask is True else is_ocean((tile_lons, tile_lats), landmask)
             landflag.append(xr.DataArray(not water_only, coords=mytile, name='land_flag'))
         else:
             water_only = True
             # landflag.append(xr.DataArray(np.nan, coords=mytile, name='land_flag'))
         # ------------------------------------------------
         
         mean_incidence = float(corner_incs.sel(mytile).mean())
         mean_slant_range = float(corner_slantTimes.sel(mytile).mean()) * celerity / 2.
         mean_velocity = float(corner_velos.sel({'tile_line':sub['tile_line']}).mean())
 
         slant_spacing = float(sub['sampleSpacing'])
         ground_spacing = slant_spacing / np.sin(np.radians(mean_incidence))
 
         DN = sub['digital_number'] if sub.swath=='WV' else sub['deramped_digital_number']
+
+        # ------------- Bright target processing -----------------------
+        if water_only: # Bright target mask is applied only on water 
+            bright_target_mask, hist_bright = get_bright_target_mask(np.abs(DN), targetsize={'line':5,'sample':5}, guardsize={'line':350,'sample':350}, cluttersize={'line':1000,'sample':1000}, spacing={'line':azimuth_spacing, 'sample':ground_spacing}, nstddev=10,itermax=10, nstddev_neigh=5)
+            mean_DN = DN.where(~bright_target_mask, 1j*np.nan).mean(skipna=True)
+            DN = DN.where(~bright_target_mask, mean_DN)
+            variables_list+=[hist_bright.to_dataset()]
+
+
         mod = compute_modulation(DN, lowpass_width=lowpass_width,
                                  spacing={'sample': ground_spacing, 'line': azimuth_spacing})
             
         # ------------- nv ------------
         nv = compute_normalized_variance(mod)
         # ------------- mean sigma0 and nesz ------------
         sigma0, nesz = compute_mean_sigma0_interp(DN, calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         if not np.isfinite(sigma0): # should only append in IW mode. Case when line are badly indexed in noise-range LUT
             sigma0, nesz = compute_mean_sigma0_closest(DN, burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        
         # ------------- mean incidence ------------
         mean_incidence = xr.DataArray(mean_incidence, name='incidence', attrs={'long_name':'incidence at tile middle', 'units':'degree'})
+        
         # ------------- heading ------------
         # heding below is computed on one border of the tile. It should be evaluated at the middle of the tile (maybe)    
         _,heading = haversine(float(corner_lons.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lons.sel(mytile)[{'c_line': 1, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 1, 'c_sample': 0}]))
         ground_heading = xr.DataArray(float(heading), name='ground_heading', attrs={'long_name':'ground heading', 'units':'degree', 'convention':'from North clockwise'})
+
+        # ------------- sensing time of the tile ------------
+        if sub.swath=='WV':
+            # print(sub[{'line': sub.sizes['line'] // 2}]['time'])
+            t_tile = sub[{'line': sub.sizes['line'] // 2}]['time'].drop('line').rename('sensing_time')
+            t_tile.attrs.update({'long_name': 'tile sensing time'})
+        else:
+            dist = (sub[{'line': sub.sizes['line'] // 2}]['line'] - sub['linesPerBurst'] * sub['burst']) * azimuth_spacing  # distance from begining of the burst
+            antenna_velocity = np.radians(sub.attrs['azimuth_steering_rate']) * mean_slant_range
+            ground_velocity = azimuth_spacing / sub.attrs['azimuth_time_interval']
+            scan_velocity = (ground_velocity + antenna_velocity).item()    
+            t_tile = (sub['sensingTime'])+ np.timedelta64(int(1.e3*dist.data / scan_velocity), 'ms')
+            t_tile = xr.DataArray(t_tile, name='sensing_time', attrs={'long_name': 'tile sensing time'})
         
         # ---------------- part of the variables to be added to the final dataset ----------------------
-        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
+        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset(), t_tile.to_dataset()]
 
         if water_only:
             periodo_spacing = {'sample': ground_spacing, 'line': azimuth_spacing}
             nperseg_periodo = {d: int(np.rint(periodo_width[d] / periodo_spacing[d])) for d in tile_width.keys()}
             noverlap_periodo = {d: int(np.rint(periodo_overlap[d] / periodo_spacing[d])) for d in tile_width.keys()}
 
             if np.any([sub.sizes[d] < nperseg_periodo[d] for d in ['line', 'sample']]):
```

### Comparing `xsarslc-2023.6.2/xsarslc/processing/xspectra.py` & `xsarslc-2023.6.21/xsarslc/processing/xspectra.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from xsarslc.tools import xtiling, xndindex
 import warnings
 from tqdm import tqdm
 
 def compute_subswath_xspectra(dt, polarization, tile_width_intra, tile_width_inter, tile_overlap_intra,
                               tile_overlap_inter,
                               periodo_width_intra, periodo_width_inter, periodo_overlap_intra, periodo_overlap_inter,
-                              decimation=None,
                               **kwargs):
     """
     Main function to compute IW inter and intra burst spectra. It has to be modified to be able to change Xspectra options
 
     Args:
         dt (xarray.Datatree): datatree contraining subswath information
         tile_width_intra (dict, optional): approximate sizes of tiles in meters. Dict of shape {dim_name (str): width of tile [m](float)} for intra burst.
@@ -27,15 +26,14 @@
         tile_overlap_intra (dict, optional): approximate sizes of tiles overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for intra burst.
         tile_overlap_inter (dict, optional): approximate sizes of tiles overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for inter burst.
         periodo_width_intra (dict): approximate sizes of periodogram in meters. Dict of shape {dim_name (str): width of tile [m](float)} for intra burst.
         periodo_width_inter (dict): approximate sizes of periodogram in meters. Dict of shape {dim_name (str): width of tile [m](float)} for inter burst.
         periodo_overlap_intra (dict): approximate sizes of periodogram overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for intra burst.
         periodo_overlap_inter (dict): approximate sizes of periodogram overlapping in meters. Dict of shape {dim_name (str): overlap [m](float)} for inter burst.
         polarization (str, optional): polarization to be selected for xspectra computation
-        decimation (int): decimation will be used to decimate xspectra along tile_sample,tile_line dimension, only few specific tiles are saved to netCDF (to save space on disk) [optional, default is None -> no decimation]
 
     Keyword Args:
         kwargs (dict): keyword arguments passed to called functions. landmask, IR_path ...
     """
     import datatree
     from xsarslc.tools import netcdf_compliant
     intra_xs = compute_IW_subswath_intraburst_xspectra(dt, polarization=polarization, tile_width=tile_width_intra,
@@ -66,50 +64,14 @@
             inter_xs.attrs.update({'multidataset': str(inter_xs.multidataset)})
             # inter_xs.attrs.update({'start_date': str(inter_xs.start_date)})
             # inter_xs.attrs.update({'stop_date': str(inter_xs.stop_date)})
         if 'footprint' in inter_xs.attrs:
             inter_xs.attrs.update({'footprint': str(inter_xs.footprint)})
         # inter_xs.attrs.pop('pixel_line_m')
         # inter_xs.attrs.pop('pixel_sample_m')
-    if decimation:
-        logging.info('decimation of intra burst and inter burst dataset to save only few tiles')
-        logging.info('one out of %s xspectra will be kept along tile_sample/line axis',decimation)
-        decimation_selection = {'intra':
-                                    {'tile_sample':
-                                        {'iw1': intra_xs.tile_sample.values[::decimation],
-                                         'iw2': intra_xs.tile_sample.values[::decimation],
-                                         'iw3': intra_xs.tile_sample.values[::decimation]
-                                         }
-                                     ,
-                                    'tile_line':
-                                         {
-                                         'iw1': intra_xs.tile_line.values[::decimation],
-                                         'iw2': intra_xs.tile_line.values[::decimation],
-                                         'iw3': intra_xs.tile_line.values[::decimation]
-                                         }
-                                    }
-                                ,
-                                'inter':{
-                                    'tile_sample':
-                                        {'iw1': inter_xs.tile_sample.values[::decimation],
-                                         'iw2': inter_xs.tile_sample.values[::decimation],
-                                         'iw3': inter_xs.tile_sample.values[::decimation]
-                                         },
-                                    'tile_line':
-                                         {
-                                             'iw1': inter_xs.tile_line.values[::decimation],
-                                             'iw2': inter_xs.tile_line.values[::decimation],
-                                             'iw3': inter_xs.tile_line.values[::decimation],
-                                         }
-                                     }
-                                     }
-        subswa = dt.attrs['name'].split(':')[2].lower()
-        inter_xs = inter_xs.isel({'tile_sample':decimation_selection['inter']['tile_sample'][subswa]})
-        intra_xs = intra_xs.isel({'tile_sample':decimation_selection['intra']['tile_sample'][subswa],
-                                  'tile_line':decimation_selection['intra']['tile_line'][subswa]})
 
     if not inter_xs and not intra_xs:
         dt = None
     else:
         dt_dict = {}
         if inter_xs:
             dt_dict.update({'interburst': netcdf_compliant(inter_xs)})
@@ -195,15 +157,16 @@
 
     if not IR_path:
         warnings.warn('Impulse Reponse not found in keyword argument. No IR correction will be applied.')
 
     if not landmask:
         warnings.warn('Landmask not found in keyword argument. X-spectra will be evaluated everywhere.')
 
-    commons = {'radar_frequency': float(dt['image']['radarFrequency']),
+    commons = {'azimuth_steering_rate': dt['image']['azimuthSteeringRate'].item(),
+               'radar_frequency': float(dt['image']['radarFrequency']),
                'azimuth_time_interval': float(dt['image']['azimuthTimeInterval']),
                'swath': dt.attrs['swath']}
     xspectra = list()
 
     burst_list = kwargs.pop('burst_list', dt['bursts'].ds['burst'].data) # this is a list of burst number (not burst index)
 
     if kwargs.pop('dev', False):
@@ -563,7 +526,74 @@
         except:
             centroid = np.nan
         
     else:
         raise ValueError('Unknown method : {}'.format(method))
 
     return centroid
+
+def get_bright_target_mask(nrcs, targetsize, guardsize, cluttersize, spacing, nstddev=10,itermax=10,nstddev_neigh=5):
+    """
+    Compute Brigh Target mask based on cell-averaging Constant False Alarm Rate (CFAR) algorithm
+    
+    Args:
+        nrcs (xarray.DataArray): 2D map of nrcs values
+        guardsize (dict): size of guard zone in [meter]. Dict of form {'name_of_dimension':size_of_guard}
+        cluttersize (dict): size of clutter zone in [meter]. Dict of form {'name_of_dimension':size_of_clutter}
+        spacing (dict): ground spacing of the image in [meter]. Dict of form {'name_of_dimension'(str): ground_spacing [float] }
+        nstddev (float, optional): treshold for bright detection
+        itermax (int, optional): maximum number of iteration to maximize number of detection
+        nstsdev_neigh (int, optional): treshold for neighborhood detection
+        
+    Return:
+        xarray.DataArray: same dimension as nrcs with integer datatype
+    """
+    from scipy.ndimage import uniform_filter, binary_dilation
+    from scipy.signal import fftconvolve
+    
+    ntarget = {'line':2*int(0.5*targetsize['line'] / spacing['line'])+1, 'sample':2*int(0.5*targetsize['sample'] / spacing['sample'])+1} # number of pixel to define what is a target
+    if np.all([s==1 for s in ntarget.values()]):
+        tmean = nrcs
+    else:
+        tmean = xr.apply_ufunc(uniform_filter, nrcs, input_core_dims=[ntarget.keys()], output_core_dims=[ntarget.keys()], kwargs={'size':ntarget.values(),'mode':'constant', 'cval':0}, vectorize=True)
+        tnorm = xr.apply_ufunc(uniform_filter, xr.ones_like(nrcs), input_core_dims=[ntarget.keys()], output_core_dims=[ntarget.keys()], kwargs={'size':ntarget.values(),'mode':'constant', 'cval':0}, vectorize=True)
+        tmean = tmean/tnorm
+    
+    # Defining clutter kernel
+    nclutter = {'line':2*int(0.5*cluttersize['line'] / spacing['line'])+1, 'sample':2*int(0.5*cluttersize['sample'] / spacing['sample'])+1} # number of pixel to define the clutter
+    cker = xr.DataArray(np.ones([nclutter[d]for d in ['line','sample']]), coords = {'_'+d:np.arange(-(nclutter[d]-1)//2,nclutter[d]//2+1)*spacing[d] for d in ['line','sample']})
+    cker = cker.where(np.logical_and((cker['_line']/guardsize['line'])**2+(cker['_sample']/guardsize['sample'])**2>0.25, (cker['_line']/cluttersize['line'])**2+(cker['_sample']/cluttersize['sample'])**2<0.25),0.)
+    
+    # Find bright targets
+    values = nrcs.copy()
+    brightmask = xr.zeros_like(nrcs, dtype='bool')
+    for _iter in range(itermax):
+        cnorm = xr.apply_ufunc(fftconvolve, 1.-brightmask, cker, input_core_dims=[['line','sample'], ['_line','_sample']], output_core_dims=[['line','sample']], vectorize=True, kwargs={'mode':'same'})
+        cmean = xr.apply_ufunc(fftconvolve, values, cker, input_core_dims=[['line','sample'], ['_line','_sample']], output_core_dims=[['line','sample']], vectorize=True, kwargs={'mode':'same'})
+        cmean = cmean/cnorm
+        cvar = xr.apply_ufunc(fftconvolve, values**2, cker, input_core_dims=[['line','sample'], ['_line','_sample']], output_core_dims=[['line','sample']], vectorize=True, kwargs={'mode':'same'})
+        cvar = cvar/cnorm-cmean**2
+        cvar = cvar.where(cvar>0., np.inf)
+        devratio = (tmean - cmean) / np.sqrt(cvar)
+        bright_points = devratio > nstddev
+        iter_nbright = np.count_nonzero(np.logical_and(~brightmask, bright_points)) # number of found NEW bright targets compared to previous iteration
+        brightmask = brightmask.where(~bright_points, True)
+        values = values.where(~bright_points, 0.)
+        
+        # Looking to possible bright neighbor
+        iter_nneigh = 0
+        if nstddev_neigh is not None and nstddev_neigh < nstddev:
+            neighmask = binary_dilation(brightmask, structure=np.ones((3, 3)), iterations=0, mask=devratio > nstddev_neigh)
+            iter_nneigh = np.count_nonzero(neighmask) - np.count_nonzero(brightmask)
+            if iter_nneigh != 0:
+                brightmask = brightmask.where(~neighmask, True)
+                values = values.where(~neighmask, 0.) # cancel pixels for next clutter stats
+        # print(iter_nbright, iter_nneigh)
+        if iter_nbright == 0 and iter_nneigh == 0:
+            break
+    # computing histogram of Bright Target
+    dev = devratio.where(brightmask).data.ravel()
+    dev = dev[np.isfinite(dev)]
+    hist_bright = np.histogram(np.clip(dev,a_min=0.,a_max=249.), bins=[5,50,100,150,200,250])
+    hist_bright = xr.DataArray(hist_bright[0], coords={'bt_thresh':hist_bright[1][:-1]}, attrs={'long_name':'bright targets histogram'}, name='bright_targets_histogram')
+    hist_bright['bt_thresh'].attrs.update({'long_name':'lower edge of bright target to background amplitude ratio'})
+    return brightmask, hist_bright
```

### Comparing `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py` & `xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py` & `xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,24 +36,23 @@
         import psutil
         memory_used_go = psutil.virtual_memory().used / 1000 / 1000 / 1000.
     str_mem = 'RAM usage: %1.1f Go' % memory_used_go
     return str_mem
 
 
 def generate_IW_L1Bxspec_product(slc_iw_path, output_filename, xspeconfigname, polarization=None, dev=False,
-                                 landmask=None,decimation=False):
+                                 landmask=None):
     """
 
     :param tiff: str full path
     :param output_filename : str full path
     :param xspeconfigname : str (eg 'tiles20km')
     :param polarization : str : VV VH HH HV [optional]
     :param dev: bool: allow to shorten the processing
-    :param landmask : landmask obj (eg : cartopy.feature.NaturalEarthFeature() )
-    :param decimation: bool True -> select few tiles to saved on disk [default=False]
+    :param landmask : landmask obj (eg : cartopy.feature.NaturalEarthFeature() ) True -> will skip all the processing of cross spectrum
     :return:
     """
     safe = os.path.dirname(os.path.dirname(slc_iw_path))
     logging.info('start loading the datatree %s', get_memory_usage())
     tiff_number = os.path.basename(slc_iw_path).split('-')[1].replace('iw', '')
     str_gdal = 'SENTINEL1_DS:%s:IW%s' % (safe, tiff_number)
     bu = xsar.Sentinel1Meta(str_gdal)._bursts
@@ -84,37 +83,36 @@
                                                                    tile_overlap_intra=tile_overlap_intra,
                                                                    periodo_width_intra=periodo_width_intra,
                                                                    periodo_overlap_intra=periodo_overlap_intra,
                                                                    tile_width_inter=tile_width_inter,
                                                                    tile_overlap_inter=tile_overlap_inter,
                                                                    periodo_width_inter=periodo_width_inter,
                                                                    periodo_overlap_inter=periodo_overlap_inter
-                                                                   , IR_path=IR_path,landmask=landmask,decimation=decimation)
+                                                                   , IR_path=IR_path,landmask=landmask)
     else:
         one_subswath_xspectrum_dt = proc.compute_subswath_xspectra(dt, polarization=polarization.upper(),
                                                                    dev=dev, compute_intra_xspec=True,
                                                                    compute_inter_xspec=True,
                                                                    tile_width_intra=tile_width_intra,
                                                                    tile_overlap_intra=tile_overlap_intra,
                                                                    periodo_width_intra=periodo_width_intra,
                                                                    periodo_overlap_intra=periodo_overlap_intra,
                                                                    tile_width_inter=tile_width_inter,
                                                                    tile_overlap_inter=tile_overlap_inter,
                                                                    periodo_width_inter=periodo_width_inter,
                                                                    periodo_overlap_inter=periodo_overlap_inter,
-                                                                   landmask=landmask,decimation=decimation
+                                                                   landmask=landmask
                                                                    )
     if one_subswath_xspectrum_dt:
         logging.info('xspec intra and inter ready for %s', slc_iw_path)
         logging.debug('one_subswath_xspectrum = %s', one_subswath_xspectrum_dt)
         one_subswath_xspectrum_dt.attrs['version_xsar'] = xsar.__version__
         one_subswath_xspectrum_dt.attrs['version_xsarslc'] = xsarslc.__version__
         one_subswath_xspectrum_dt.attrs['processor'] = __file__
         one_subswath_xspectrum_dt.attrs['generation_date'] = datetime.datetime.today().strftime('%Y-%b-%d')
-        one_subswath_xspectrum_dt.attrs['decimation'] = str(decimation)
         if not os.path.exists(os.path.dirname(output_filename)):
             os.makedirs(os.path.dirname(output_filename), 0o0775)
             logging.info('makedir %s', os.path.dirname(output_filename))
         one_subswath_xspectrum_dt.to_netcdf(output_filename)
         logging.info('successfuly written %s', output_filename)
     else:
         logging.info('no inter nor intra xspectra available in this subswath')
@@ -129,16 +127,14 @@
     parser.add_argument('--tiff', required=True, help='tiff file full path IW SLC')
     parser.add_argument('--outputdir', required=False, help='directory where to store output netCDF files',
                         default=get_default_outputdir(mode='iw'))
     parser.add_argument('--version',
                         help='set the output product version (e.g. 1.4) default version will be read from config.yml',
                         required=False, default=PRODUCT_VERSION)
     parser.add_argument('--dev', action='store_true', default=False, help='dev mode stops the computation early')
-    parser.add_argument('--decimation', action='store',type=int, default=None, help='decimation of intra and inter burst '
-                            'tiles before saving, value N implies to keep 1  xspectra out of N in tile_line/sample axis')
     parser.add_argument('--landmask', required=False, default=get_default_landmask_dir(),
                         help='landmask files (such as cartopy /.local/share/cartopy ) to have a landmask information '
                              'without web connexion , default value cromes from config.yml')
     parser.add_argument('--xspeconfigname', required=False, default='tiles20km',
                         help='name of the cross-spectra (tiles/periodogram) in config.yml e.g. "tiles20km" ')
     args = parser.parse_args()
     fmt = '%(asctime)s %(levelname)s %(filename)s(%(lineno)d) %(message)s'
@@ -155,29 +151,32 @@
     slc_iw_path = args.tiff
     if 'cartopy' in args.landmask:
         logging.info('landmask is a cartopy feature')
         import cartopy
 
         cartopy.config['pre_existing_data_dir'] = args.landmask
         landmask = cartopy.feature.NaturalEarthFeature('physical', 'land', '10m')
+    elif args.landmask=='True':
+        landmask = True
+        logging.info('all the tiles will be considered on land -> no xspectra expected in L1B output file')
     else:
         landmask = None
     polarization_from_file = os.path.basename(slc_iw_path).split('-')[3]
     safe_basename = os.path.basename(os.path.dirname(os.path.dirname(slc_iw_path)))
     safe_basename = safe_basename.replace('SLC', 'XSP')
     output_filename = os.path.join(args.outputdir, args.version, safe_basename, os.path.basename(
         slc_iw_path).replace('.tiff', '') + '_L1B_xspec_IFR_' + args.version + '.nc')
     logging.info('mode dev is %s', args.dev)
     logging.info('output filename would be: %s', output_filename)
     if os.path.exists(output_filename) and args.overwrite is False:
         logging.info('%s already exists', output_filename)
     else:
         generate_IW_L1Bxspec_product(slc_iw_path=slc_iw_path, output_filename=output_filename,
                                      xspeconfigname=args.xspeconfigname, dev=args.dev,
-                                     polarization=polarization_from_file, landmask=landmask,decimation=args.decimation)
+                                     polarization=polarization_from_file, landmask=landmask)
     logging.info('peak memory usage: %s Mbytes', get_memory_usage())
     logging.info('done in %1.3f min', (time.time() - t0) / 60.)
 
 
 if __name__ == '__main__':
     root = logging.getLogger()
     if root.handlers:
```

### Comparing `xsarslc-2023.6.2/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py` & `xsarslc-2023.6.21/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc/tools.py` & `xsarslc-2023.6.21/xsarslc/tools.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.6.2/xsarslc.egg-info/PKG-INFO` & `xsarslc-2023.6.21/xsarslc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.6.2
+Version: 2023.6.21
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 xsarslc
 
 
 Functions for Sentinel-1 SLC products 
+
+the main feature of this library is the SAR processor:
+
+
+```mermaid
+graph TD;
+    A[level-1 SLC] -->| SAR processor | B(level-1B XSP);
+```
+
+
 This is a Work In Progress Library.
+
 Disclaimer: no warranty on the quality of output product at this stage.
+
+
 # installation
 ```bash
-git clone https://github.com/umr-lops/xsar_slc
-cd xsar_slc
-pip install .
+pip install git+https://github.com/umr-lops/xsar_slc
 ```
 
 # usage
 ```python
 import xsarslc
 ```
```

### Comparing `xsarslc-2023.6.2/xsarslc.egg-info/SOURCES.txt` & `xsarslc-2023.6.21/xsarslc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -39,16 +39,18 @@
 docs/conf.py
 docs/crossspectra.rst
 docs/cutoff.rst
 docs/index.rst
 docs/installing.rst
 docs/normalizedvariance.rst
 docs/oceanspectrumSAR.png
+docs/product_description.rst
 docs/sigma0.rst
 docs/_static/css/xsarslc.css
+docs/examples/L1B_Sentinel1_variables_explanation.ipynb
 docs/examples/default_impulseResponse_files_IW.ipynb
 docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
 docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
 docs/examples/intro.py
 docs/examples/xspec_IW_intra_and_inter_burst.ipynb
 docs/examples/xspec_WV_example.ipynb
 docs/figures/NIRAN_NRCS_VH.png
@@ -61,14 +63,15 @@
 xsarslc/__init__.py
 xsarslc/burst.py
 xsarslc/config.yml
 xsarslc/get_config_infos.py
 xsarslc/get_test_files.py
 xsarslc/interface.py
 xsarslc/tools.py
+xsarslc/wallpaper.py
 xsarslc.egg-info/PKG-INFO
 xsarslc.egg-info/SOURCES.txt
 xsarslc.egg-info/dependency_links.txt
 xsarslc.egg-info/entry_points.txt
 xsarslc.egg-info/requires.txt
 xsarslc.egg-info/top_level.txt
 xsarslc/processing/HR_tiles.py
```

