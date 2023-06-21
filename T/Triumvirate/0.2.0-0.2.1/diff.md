# Comparing `tmp/Triumvirate-0.2.0.tar.gz` & `tmp/Triumvirate-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Triumvirate-0.2.0.tar", last modified: Thu Jun  1 12:27:56 2023, max compression
+gzip compressed data, was "Triumvirate-0.2.1.tar", last modified: Mon Jun 19 15:13:48 2023, max compression
```

## Comparing `Triumvirate-0.2.0.tar` & `Triumvirate-0.2.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    24555 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/src/Triumvirate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 12:27:56.000000 Triumvirate-0.2.0/src/Triumvirate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_bihankel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_fftlog.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_particles.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_particles.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_threept.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_twopt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_valid_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/_winconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28099 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/dataobjs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/dataobjs.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/arrayops.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/dataobjs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/fftlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/field.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/maths.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/monitor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/parameters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/particles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/threept.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/include/twopt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/parameters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/parameters.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.191980 Triumvirate-0.2.0/src/triumvirate/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/resources/params_template.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/resources/params_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/src/triumvirate/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/arrayops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/dataobjs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/fftlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74090 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/field.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/maths.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/monitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27800 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/particles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74244 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/threept.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28450 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/src/twopt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/threept.py
--rw-r--r--   0 runner    (1001) docker     (123)    47337 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/src/triumvirate/twopt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/test_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_build/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_dataobjs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.187980 Triumvirate-0.2.0/tests/test_input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.195980 Triumvirate-0.2.0/tests/test_input/ctlgs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.fits
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.h5
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/test_data_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/ctlgs/test_rand_catalogue.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.199980 Triumvirate-0.2.0/tests/test_input/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/test_params.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/test_params.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/params/tmpl_params.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:27:56.203981 Triumvirate-0.2.0/tests/test_input/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/pk2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xi2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xiw0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/xiw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw000_bin0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw000_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_input/stats/zetaw202_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_threept.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-01 12:27:35.000000 Triumvirate-0.2.0/tests/test_twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24555 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.926374 Triumvirate-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.930374 Triumvirate-0.2.1/src/Triumvirate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.934374 Triumvirate-0.2.1/src/triumvirate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_bihankel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_fftlog.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_particles.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_particles.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_threept.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_twopt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_valid_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_winconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28099 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/dataobjs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/dataobjs.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.938374 Triumvirate-0.2.1/src/triumvirate/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/arrayops.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/dataobjs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/fftlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/field.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/maths.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/monitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/parameters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/particles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/threept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/twopt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/parameters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/parameters.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.938374 Triumvirate-0.2.1/src/triumvirate/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/resources/params_template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/resources/params_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.942374 Triumvirate-0.2.1/src/triumvirate/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/arrayops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/dataobjs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/fftlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74104 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/maths.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/monitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27800 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/particles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74281 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/threept.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28450 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/twopt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47337 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/test_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_build/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_dataobjs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.926374 Triumvirate-0.2.1/tests/test_input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/test_input/ctlgs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/test_data_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/test_rand_catalogue.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.954374 Triumvirate-0.2.1/tests/test_input/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/test_params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/test_params.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/tmpl_params.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/tests/test_input/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk2_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi0_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi0_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi2_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi2_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xiw0.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xiw2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw000_bin0.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw000_diag.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw202_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_twopt.py
```

### Comparing `Triumvirate-0.2.0/CHANGELOG.md` & `Triumvirate-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/LICENCE` & `Triumvirate-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/MANIFEST.in` & `Triumvirate-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/Makefile` & `Triumvirate-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/PKG-INFO` & `Triumvirate-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `Triumvirate-0.2.0/README.md` & `Triumvirate-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/README.rst` & `Triumvirate-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/pyproject.toml` & `Triumvirate-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/setup.cfg` & `Triumvirate-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/setup.py` & `Triumvirate-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/Triumvirate.egg-info/PKG-INFO` & `Triumvirate-0.2.1/src/Triumvirate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `Triumvirate-0.2.0/src/Triumvirate.egg-info/SOURCES.txt` & `Triumvirate-0.2.1/src/Triumvirate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/__init__.py` & `Triumvirate-0.2.1/src/triumvirate/__init__.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_bihankel.py` & `Triumvirate-0.2.1/src/triumvirate/_bihankel.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_fftlog.pyx` & `Triumvirate-0.2.1/src/triumvirate/_fftlog.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_particles.pxd` & `Triumvirate-0.2.1/src/triumvirate/_particles.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_particles.pyx` & `Triumvirate-0.2.1/src/triumvirate/_particles.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_threept.pyx` & `Triumvirate-0.2.1/src/triumvirate/_threept.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_twopt.pyx` & `Triumvirate-0.2.1/src/triumvirate/_twopt.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_valid_install.py` & `Triumvirate-0.2.1/src/triumvirate/_valid_install.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/_winconv.py` & `Triumvirate-0.2.1/src/triumvirate/_winconv.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/catalogue.py` & `Triumvirate-0.2.1/src/triumvirate/catalogue.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/dataobjs.pxd` & `Triumvirate-0.2.1/src/triumvirate/dataobjs.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/dataobjs.pyx` & `Triumvirate-0.2.1/src/triumvirate/dataobjs.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/arrayops.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/arrayops.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/dataobjs.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/dataobjs.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/fftlog.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/fftlog.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
  * @param[in] a Pre-transform sample values.
  * @param[out] k Post-transform sample points.
  * @param[out] b Post-trasform sample values.
  * @param[out] u FFTLog transform kernel coefficients.
  */
 void hankel_transform(
   double mu, double q, double kr_c, int N, bool lowring,
-  double* r, const std::complex<double>* a,
+  double* r, std::complex<double>* a,
   double* k, std::complex<double>* b,
   std::complex<double>* u
 );
 
 /**
  * @brief Perform the (forward) spherical Fourier--Bessel transform.
  *
```

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/field.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/field.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/io.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/io.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/maths.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/maths.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/monitor.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/monitor.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/parameters.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/parameters.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/particles.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/particles.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/threept.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/threept.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/include/twopt.hpp` & `Triumvirate-0.2.1/src/triumvirate/include/twopt.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/logger.py` & `Triumvirate-0.2.1/src/triumvirate/logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/parameters.pxd` & `Triumvirate-0.2.1/src/triumvirate/parameters.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/parameters.pyx` & `Triumvirate-0.2.1/src/triumvirate/parameters.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/resources/params_template.ini` & `Triumvirate-0.2.1/src/triumvirate/resources/params_template.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/resources/params_template.yml` & `Triumvirate-0.2.1/src/triumvirate/resources/params_template.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/arrayops.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/arrayops.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/dataobjs.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/dataobjs.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/fftlog.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/fftlog.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
   if (N % 2 == 0) {
     u[N/2] = u[N/2].real() + trvm::M_I * 0.;  // make real by log-periodicity
   }
 }
 
 void hankel_transform(
   double mu, double q, double kr_c, int N, bool lowring,
-  double* r, const std::complex<double>* a,
+  double* r, std::complex<double>* a,
   double* k, std::complex<double>* b,
   std::complex<double>* u
 ) {
   // Calculate the logarithmic interval.
   double L = N * std::log(r[N - 1] / r[0]) / (N - 1.);
 
   // Compute the forward transform kernel.
```

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/field.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/field.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1221,15 +1221,15 @@
 
         double kv[3];
         this->get_grid_wavevector(i, j, k, kv);
 
         double k_ = trvm::get_vec3d_magnitude(kv);
 
         // Determine the grid cell contribution to the band.
-        if (k_lower < k_ && k_ <= k_upper) {
+        if (k_lower <= k_ && k_ < k_upper) {
           std::complex<double> fk(
             field_fourier[idx_grid][0], field_fourier[idx_grid][1]
           );
 
           // Apply assignment compensation.
           double win = this->calc_assignment_window_in_fourier(i, j, k);
           fk /= win;
@@ -1606,15 +1606,15 @@
 
   // Perform binning.
   for (int ibin = 0; ibin < kbinning.num_bins; ibin++) {
     double k_lower = kbinning.bin_edges[ibin];
     double k_upper = kbinning.bin_edges[ibin + 1];
     for (int i = 0; i < n_sample; i++) {
       double k_ = i * dk_sample;
-      if (k_lower < k_ && k_ <= k_upper) {
+      if (k_lower <= k_ && k_ < k_upper) {
         this->nmodes[ibin] += nmodes_sample[i];
         this->k[ibin] += k_sample[i];
         this->pk[ibin] += pk_sample[i];
         this->sn[ibin] += sn_sample[i];
       }
     }
 
@@ -1824,15 +1824,15 @@
         this->xi[ibin] += xi_sample[i];
       }
     }
 
     if (this->npairs[ibin] != 0) {
       this->r[ibin] /= double(this->npairs[ibin]);
       this->xi[ibin] /= double(this->npairs[ibin]);
-      this->npairs[ibin] /= 2;  // reality condition
+      // this->npairs[ibin] /= 2;  // reality condition
     } else {
       this->r[ibin] = rbinning.bin_centres[ibin];
       this->xi[ibin] = 0.;
     }
   }
 
   fftw_free(twopt_3d); twopt_3d = nullptr;
@@ -2028,28 +2028,28 @@
         this->xi[ibin] += xi_sample[i];
       }
     }
 
     if (this->npairs[ibin] != 0) {
       this->r[ibin] /= double(this->npairs[ibin]);
       this->xi[ibin] /= double(this->npairs[ibin]);
-      this->npairs[ibin] /= 2;  // reality condition
     } else {
       this->r[ibin] = rbinning.bin_centres[ibin];
       this->xi[ibin] = 0.;
     }
   }
 
   // Apply normalisation factors.
   double norm_factors = 1 / this->vol_cell
     * std::pow(-1, this->params.ell1 + this->params.ell2);
 
   for (int ibin = 0; ibin < rbinning.num_bins; ibin++) {
     if (this->npairs[ibin] != 0) {
-      this->xi[ibin] *= norm_factors / this->npairs[ibin];
+      this->xi[ibin] *= norm_factors / double(this->npairs[ibin]);
+      // this->npairs[ibin] /= 2;  // reality condition
     }
   }
 
   fftw_free(twopt_3d); twopt_3d = nullptr;
 
   trvs::gbytesMem -= trvs::size_in_gb<fftw_complex>(this->params.nmesh);
```

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/io.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/io.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/maths.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/maths.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/monitor.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/monitor.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/parameters.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/parameters.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/particles.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/particles.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/threept.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/threept.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 
       // Initialise reduced-spherical-harmonic weights on mesh grids.
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_fourier_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_k_a
         );
       trvm::SphericalHarmonicCalculator::
@@ -487,15 +487,15 @@
             "Bispectrum term at orders (m1, m2, M) = (%d, %d, %d) computed.",
             m1_, m2_, M_
           );
         }
       }
 
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   dn_00.finalise_density_field();  // ~dn_00 (likely redundant but safe)
   N_00.finalise_density_field();  // ~N_00 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
@@ -556,15 +556,15 @@
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
   double alpha = catalogue_data.wstotal / catalogue_rand.wstotal;
 
-  double parity = std::pow(-1, params.ell1 + params.ell2);
+  std::complex<double> parity = std::pow(trvm::M_I, params.ell1 + params.ell2);
 
   // Set up output.
   int* npairs_save = new int[rbinning.num_bins];
   double* r1_save = new double[rbinning.num_bins];
   double* r2_save = new double[rbinning.num_bins];
   std::complex<double>* zeta_save =
     new std::complex<double>[rbinning.num_bins];
@@ -623,15 +623,15 @@
 
       // Initialise reduced-spherical-harmonic weights on mesh grids.
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_config_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_r_a
         );
       trvm::SphericalHarmonicCalculator::
@@ -764,15 +764,15 @@
             "(m1, m2, M) = (%d, %d, %d) computed.",
             m1_, m2_, M_
           );
         }
       }
 
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   dn_00.finalise_density_field();  // ~dn_00 (likely redundant but safe)
   N_00.finalise_density_field();  // ~N_00 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
@@ -895,15 +895,15 @@
 
       // Initialise/reset spherical harmonic mesh grids.
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_fourier_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_k_a
         );
       trvm::SphericalHarmonicCalculator
@@ -1052,15 +1052,15 @@
         trvs::logger.stat(
           "Bispectrum term at orders (m1, m2, M) = (%d, %d, 0) computed.",
           m1_, m2_
         );
       }
 
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   dn_00.finalise_density_field();  // ~dn_00 (likely redundant but safe)
   N_L0.finalise_density_field();  // ~N_L0 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
@@ -1120,15 +1120,15 @@
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
-  double parity = std::pow(-1, params.ell1 + params.ell2);
+  std::complex<double> parity = std::pow(trvm::M_I, params.ell1 + params.ell2);
 
   // Set up output.
   int* npairs_save = new int[rbinning.num_bins];
   double* r1_save = new double[rbinning.num_bins];
   double* r2_save = new double[rbinning.num_bins];
   std::complex<double>* zeta_save =
     new std::complex<double>[rbinning.num_bins];
@@ -1181,15 +1181,15 @@
 
       // Initialise/reset spherical harmonic mesh grids.
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_config_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_r_a
         );
       trvm::SphericalHarmonicCalculator::
@@ -1221,15 +1221,15 @@
       );
 
       for (int ibin = 0; ibin < rbinning.num_bins; ibin++) {
         if (params.form == "diag") {
           sn_save[ibin] += coupling * stats_sn.xi[ibin];
         } else
         if (params.form == "full") {
-            // Enforce the Kronecker delta in eq. (51) in the Paper.
+          // Enforce the Kronecker delta in eq. (51) in the Paper.
           if (ibin == params.idx_bin) {
             sn_save[ibin] += coupling * stats_sn.xi[ibin];
           }
           // else {
           //   sn_save[ibin] += 0.;
           // }
         }
@@ -1304,15 +1304,15 @@
           "Three-point correlation function term at orders "
           "(m1, m2, M) = (%d, %d, 0) computed.",
           m1_, m2_
         );
       }
 
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   dn_00.finalise_density_field();  // ~dn_00 (likely redundant but safe)
   N_00.finalise_density_field();  // ~N_00 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
@@ -1375,15 +1375,15 @@
   // ---------------------------------------------------------------------
   // Set-up
   // ---------------------------------------------------------------------
 
   // Set up/check input.
   validate_multipole_coupling(params);
 
-  double parity = std::pow(-1, params.ell1 + params.ell2);
+  std::complex<double> parity = std::pow(trvm::M_I, params.ell1 + params.ell2);
 
   // Set up output.
   int* npairs_save = new int[rbinning.num_bins];
   double* r1_save = new double[rbinning.num_bins];
   double* r2_save = new double[rbinning.num_bins];
   std::complex<double>* zeta_save =
     new std::complex<double>[rbinning.num_bins];
@@ -1438,15 +1438,15 @@
 
       // Initialise reduced-spherical-harmonic weights on mesh grids.
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_config_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_r_a
         );
       trvm::SphericalHarmonicCalculator::
@@ -1580,15 +1580,15 @@
             "(m1, m2, M) = (%d, %d, %d) computed.",
             m1_, m2_, M_
           );
         }
       }
 
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   n_00.finalise_density_field();  // ~n_00 (likely redundant but safe)
   N_00.finalise_density_field();  // ~N_00 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
@@ -1717,15 +1717,15 @@
 
       // Initialise reduced-spherical-harmonic weights on mesh grids.
       std::vector< std::complex<double> > ylm_k_a(params.nmesh);
       std::vector< std::complex<double> > ylm_k_b(params.nmesh);
       std::vector< std::complex<double> > ylm_r_a(params.nmesh);
       std::vector< std::complex<double> > ylm_r_b(params.nmesh);
       trvs::gbytesMem +=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
       trvs::update_maxmem();
 
       trvm::SphericalHarmonicCalculator::
         store_reduced_spherical_harmonic_in_fourier_space(
           params.ell1, m1_, params.boxsize, params.ngrid, ylm_k_a
         );
       trvm::SphericalHarmonicCalculator::
@@ -1986,15 +1986,15 @@
       }
 
       delete[] ylm_k_a; ylm_k_a = nullptr;
       delete[] ylm_k_b; ylm_k_b = nullptr;
       delete[] ylm_r_a; ylm_r_a = nullptr;
       delete[] ylm_r_b; ylm_r_b = nullptr;
       trvs::gbytesMem -=
-        trvs::size_in_gb< std::complex<double> >(4 * params.nmesh);
+        trvs::size_in_gb< std::complex<double> >(4*params.nmesh);
     }
   }
 
   dn_00.finalise_density_field();  // ~dn_00 (likely redundant but safe)
   N_00.finalise_density_field();  // ~N_00 (likely redundant but safe)
 
 #if defined(TRV_USE_OMP) && defined(TRV_USE_FFTWOMP)
```

### Comparing `Triumvirate-0.2.0/src/triumvirate/src/twopt.cpp` & `Triumvirate-0.2.1/src/triumvirate/src/twopt.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/threept.py` & `Triumvirate-0.2.1/src/triumvirate/threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/src/triumvirate/twopt.py` & `Triumvirate-0.2.1/src/triumvirate/twopt.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/conftest.py` & `Triumvirate-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_catalogue.py` & `Triumvirate-0.2.1/tests/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_dataobjs.py` & `Triumvirate-0.2.1/tests/test_dataobjs.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.fits` & `Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.fits`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/ctlgs/sample_catalogue.h5` & `Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.h5`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/ctlgs/test_rand_catalogue.txt` & `Triumvirate-0.2.1/tests/test_input/ctlgs/test_rand_catalogue.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/params/test_params.ini` & `Triumvirate-0.2.1/tests/test_input/params/test_params.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/params/test_params.yml` & `Triumvirate-0.2.1/tests/test_input/params/test_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/params/tmpl_params.yml` & `Triumvirate-0.2.1/tests/test_input/params/tmpl_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_gpp.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 8.142524244e+07 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 8.142524244e+07 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.130521010e+17	 0.000000000e+00	 2.861146360e+17	 2.481069172e-18
-1.750000000e-02	2.258782336e-02	4.250000000e-02	4.488283313e-02	      2340	 1.245150156e+17	 0.000000000e+00	 1.334039644e+17	-1.225690582e-18
-1.750000000e-02	2.258782336e-02	6.750000000e-02	6.912253858e-02	      5908	 2.098911542e+17	 0.000000000e+00	 2.075665390e+17	 5.697472148e-18
-1.750000000e-02	2.258782336e-02	9.250000000e-02	9.369454264e-02	     10840	 1.926191628e+17	 0.000000000e+00	 1.923215410e+17	 2.379079834e-17
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.130521010e+17	 0.000000000e+00	 2.861146360e+17	 7.939421349e-18
+1.750000000e-02	2.258782336e-02	4.250000000e-02	4.488283313e-02	      2340	 1.245150156e+17	 0.000000000e+00	 1.334039644e+17	 8.115428820e-18
+1.750000000e-02	2.258782336e-02	6.750000000e-02	6.912253858e-02	      5908	 2.098911542e+17	 0.000000000e+00	 2.075665390e+17	 6.277424167e-19
+1.750000000e-02	2.258782336e-02	9.250000000e-02	9.369454264e-02	     10840	 1.926191628e+17	 0.000000000e+00	 1.923215410e+17	 2.832744705e-17
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk000_bin0_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_lpp.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.129296339e+17	 0.000000000e+00	 2.860393289e+17	 1.120866014e-02
-1.750000000e-02	2.258782336e-02	4.250000000e-02	4.488283313e-02	      2340	 1.244926134e+17	 0.000000000e+00	 1.333700973e+17	 7.223211401e-03
-1.750000000e-02	2.258782336e-02	6.750000000e-02	6.912253858e-02	      5908	 2.098960240e+17	 0.000000000e+00	 2.075891723e+17	 4.951665049e-03
-1.750000000e-02	2.258782336e-02	9.250000000e-02	9.369454264e-02	     10840	 1.929396325e+17	 0.000000000e+00	 1.926016786e+17	 7.426521708e-03
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.129296339e+17	 0.000000000e+00	 2.860393289e+17	-3.037861160e-03
+4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 4.930747041e+16	 0.000000000e+00	 4.721358074e+16	 7.128054406e-04
+6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 1.410887484e+17	 0.000000000e+00	 1.424394978e+17	-1.824596775e-03
+9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.225673312e+17	 0.000000000e+00	 1.287321375e+17	 1.568811057e-03
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_gpp.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 8.142524244e+07 (mesh-based, alternative)
-# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.130521010e+17	 0.000000000e+00	 2.861146360e+17	 7.939421349e-18
-4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 4.930737735e+16	 0.000000000e+00	 4.719929695e+16	 4.292037610e-18
-6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 1.410970587e+17	 0.000000000e+00	 1.422978439e+17	-1.110769797e-17
-9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.217545947e+17	 0.000000000e+00	 1.277625663e+17	 1.899345426e-17
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 8.142524244e+07 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
+# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk202_raw}, [6] Im{bk202_raw}, [7] Re{bk202_shot}, [8] Im{bk202_shot}
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 2.034323739e+17	 0.000000000e+00	 1.656109877e+17	-3.225389923e-17
+4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 7.275271099e+16	 0.000000000e+00	 8.298921775e+16	 6.133224198e-17
+6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	-6.279010232e+16	 0.000000000e+00	-6.059337933e+16	-5.483822192e-17
+9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.736677108e+16	 0.000000000e+00	 1.947973945e+16	 3.074328516e-17
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk000_diag_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/pk0_gpp.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
-# Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
-# Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
-# Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
+# Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
-# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.129296339e+17	 0.000000000e+00	 2.860393289e+17	 1.316406503e-02
-4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 4.930747041e+16	 0.000000000e+00	 4.721358074e+16	-1.635827352e-03
-6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 1.410887484e+17	 0.000000000e+00	 1.424394978e+17	 2.264202605e-03
-9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.225673312e+17	 0.000000000e+00	 1.287321375e+17	-2.883315433e-03
+# Normalisation factor: 1.111111111e+08 (particle)
+# Normalisation factor alternatives: 1.111111111e+08 (particle), 6.663249584e+03 (mesh), 0.000000000e+00 (mesh-mixed)
+# [0] k_cen, [1] k_eff, [2] nmodes, [3] Re{pk0_raw}, [4] Im{pk0_raw}, [5] Re{pk0_shot}, [6] Im{pk0_shot}
+1.750000000e-02	2.258782336e-02	       460	 5.605891524e+08	 0.000000000e+00	 3.333333333e+08	 0.000000000e+00
+4.250000000e-02	4.488283313e-02	      2340	 2.220321045e+08	 0.000000000e+00	 3.333333333e+08	 0.000000000e+00
+6.750000000e-02	6.912253858e-02	      5908	 3.741577638e+08	 0.000000000e+00	 3.333333333e+08	 0.000000000e+00
+9.250000000e-02	9.369454264e-02	     10840	 3.431795046e+08	 0.000000000e+00	 3.333333333e+08	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_gpp.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 8.142524244e+07 (mesh-based, alternative)
-# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk202_raw}, [6] Im{bk202_raw}, [7] Re{bk202_shot}, [8] Im{bk202_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 2.034323739e+17	 0.000000000e+00	 1.656109877e+17	-2.481069172e-18
-4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 7.275271099e+16	 0.000000000e+00	 8.298921775e+16	 2.267951691e-17
-6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	-6.279010232e+16	 0.000000000e+00	-6.059337933e+16	 7.310428340e-17
-9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.736677108e+16	 0.000000000e+00	 1.947973945e+16	 2.220531159e-17
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 8.142524244e+07 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
+# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.130521010e+17	 0.000000000e+00	 2.861146360e+17	 7.939421349e-18
+4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	 4.930737735e+16	 0.000000000e+00	 4.719929695e+16	 3.014180958e-17
+6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 1.410970587e+17	 0.000000000e+00	 1.422978439e+17	 2.456250081e-17
+9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	 1.217545947e+17	 0.000000000e+00	 1.277625663e+17	-5.090540539e-17
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/bk202_diag_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_lpp.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk202_raw}, [6] Im{bk202_raw}, [7] Re{bk202_shot}, [8] Im{bk202_shot}
-1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	-2.585274899e+17	-7.067391939e+00	-2.175937633e+17	-1.500816896e-01
-4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	-9.125399262e+16	 3.232528699e-01	-1.062954937e+17	-9.541983009e-01
-6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 7.758101605e+16	-2.489147488e+00	 7.441153620e+16	-3.818110810e+00
-9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	-1.993021128e+16	-2.828964557e+00	-2.328348174e+16	-1.416741033e+00
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	-2.585274899e+17	-7.982940440e+00	-2.175937633e+17	 7.611500807e+00
+4.250000000e-02	4.488283313e-02	4.250000000e-02	4.488283313e-02	      2340	-9.125399262e+16	 8.924590105e-01	-1.062954937e+17	-2.220104726e+00
+6.750000000e-02	6.912253858e-02	6.750000000e-02	6.912253858e-02	      5908	 7.758101605e+16	-3.055090983e+00	 7.441153620e+16	-1.507091214e+00
+9.250000000e-02	9.369454264e-02	9.250000000e-02	9.369454264e-02	     10840	-1.993021128e+16	-3.425275752e+00	-2.328348174e+16	-1.553772141e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/pk0_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/pk0_lpp.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 1.111111111e+08 (particle-based, used), 4.538831600e+07 (mesh-based, alternative)
+# Normalisation factor: 1.111111111e+08 (particle)
+# Normalisation factor alternatives: 1.111111111e+08 (particle), 4.538831600e+07 (mesh), 8.158928783e+07 (mesh-mixed)
 # [0] k_cen, [1] k_eff, [2] nmodes, [3] Re{pk0_raw}, [4] Im{pk0_raw}, [5] Re{pk0_shot}, [6] Im{pk0_shot}
-1.750000000e-02	2.258782336e-02	       460	 5.605170801e+08	 6.698886763e-27	 3.333666667e+08	 0.000000000e+00
-4.250000000e-02	4.488283313e-02	      2340	 2.220594005e+08	 2.368546323e-27	 3.333666667e+08	 0.000000000e+00
-6.750000000e-02	6.912253858e-02	      5908	 3.741576428e+08	 1.645780521e-26	 3.333666667e+08	 0.000000000e+00
-9.250000000e-02	9.369454264e-02	     10840	 3.436435992e+08	-1.368049868e-27	 3.333666667e+08	 0.000000000e+00
+1.750000000e-02	2.258782336e-02	       460	 5.605170801e+08	-1.256041268e-26	 3.333666667e+08	 0.000000000e+00
+4.250000000e-02	4.488283313e-02	      2340	 2.220594005e+08	 3.017838944e-28	 3.333666667e+08	 0.000000000e+00
+6.750000000e-02	6.912253858e-02	      5908	 3.741576428e+08	-2.570949136e-26	 3.333666667e+08	 0.000000000e+00
+9.250000000e-02	9.369454264e-02	     10840	 3.436435992e+08	-6.961162840e-27	 3.333666667e+08	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/pk2_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/xi0_lpp.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-# Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
-# Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
+# Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
+# Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
+# Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 1.111111111e+08 (particle-based, used), 6.663249584e+03 (mesh-based, alternative)
-# [0] k_cen, [1] k_eff, [2] nmodes, [3] Re{pk2_raw}, [4] Im{pk2_raw}, [5] Re{pk2_shot}, [6] Im{pk2_shot}
-1.750000000e-02	2.258782336e-02	       460	 3.642045289e+08	 0.000000000e+00	-2.963276430e-08	 0.000000000e+00
-4.250000000e-02	4.488283313e-02	      2340	 3.271845226e+08	 0.000000000e+00	 6.642359976e-09	 0.000000000e+00
-6.750000000e-02	6.912253858e-02	      5908	-1.678964677e+08	 0.000000000e+00	 2.469563459e-08	 0.000000000e+00
-9.250000000e-02	9.369454264e-02	     10840	 3.782552178e+07	 0.000000000e+00	 1.875407487e-08	 0.000000000e+00
+# Normalisation factor: 1.111111111e+08 (particle)
+# Normalisation factor alternatives: 1.111111111e+08 (particle), 4.538831600e+07 (mesh), 8.158928783e+07 (mesh-mixed)
+# [0] r_cen, [1] r_eff, [2] npairs, [3] Re{xi0}, [4] Im{xi0}
+6.250000000e+01	6.431962465e+01	       314	 3.982979617e+01	 5.048087177e-16
+8.750000000e+01	8.777591768e+01	       584	 9.310073255e+01	-1.718456185e-15
+1.125000000e+02	1.122315212e+02	      1058	 9.290046987e+01	-2.341478839e-16
+1.375000000e+02	1.381486607e+02	      1640	 5.697589689e+00	 2.086077607e-16
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/xi0_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/xiw2.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
-# Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
+# Catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
+# Catalogue particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 1.111111111e+08 (particle-based, used), 6.663249584e+03 (mesh-based, alternative)
-# [0] r_cen, [1] r_eff, [2] npairs, [3] Re{xi0}, [4] Im{xi0}
-6.250000000e+01	6.431962465e+01	       157	 3.783114933e+01	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	       292	 8.367608860e+01	 0.000000000e+00
-1.125000000e+02	1.122315212e+02	       529	 9.879249232e+01	 0.000000000e+00
-1.375000000e+02	1.381486607e+02	       820	 5.990741734e+00	 0.000000000e+00
+# Normalisation factor: 1.111111111e+04 (particle)
+# Normalisation factor alternatives: 1.111111111e+04 (particle), 4.538831600e-01 (mesh), 0.000000000e+00 (mesh-mixed)
+# [0] r_cen, [1] r_eff, [2] npairs, [3] Re{xi2}, [4] Im{xi2}
+6.250000000e+01	6.431962465e+01	       314	 3.936047096e+01	 8.342491228e-15
+8.750000000e+01	8.777591768e+01	       584	 2.474456669e+01	-4.347439422e-15
+1.125000000e+02	1.122315212e+02	      1058	 1.661148343e+01	-1.371103236e-16
+1.375000000e+02	1.381486607e+02	      1640	 4.181385435e+01	-4.159897813e-15
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/xi0_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/pk2_gpp.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
-# Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
-# Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
-# Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
+# Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 1.111111111e+08 (particle-based, used), 4.538831600e+07 (mesh-based, alternative)
-# [0] r_cen, [1] r_eff, [2] npairs, [3] Re{xi0}, [4] Im{xi0}
-6.250000000e+01	6.431962465e+01	       157	 3.982979617e+01	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	       292	 9.310073255e+01	 0.000000000e+00
-1.125000000e+02	1.122315212e+02	       529	 9.290046987e+01	 0.000000000e+00
-1.375000000e+02	1.381486607e+02	       820	 5.697589689e+00	 0.000000000e+00
+# Normalisation factor: 1.111111111e+08 (particle)
+# Normalisation factor alternatives: 1.111111111e+08 (particle), 6.663249584e+03 (mesh), 0.000000000e+00 (mesh-mixed)
+# [0] k_cen, [1] k_eff, [2] nmodes, [3] Re{pk2_raw}, [4] Im{pk2_raw}, [5] Re{pk2_shot}, [6] Im{pk2_shot}
+1.750000000e-02	2.258782336e-02	       460	 3.642045289e+08	 0.000000000e+00	-2.856008505e-08	 0.000000000e+00
+4.250000000e-02	4.488283313e-02	      2340	 3.271845226e+08	 0.000000000e+00	 1.128146853e-08	 0.000000000e+00
+6.750000000e-02	6.912253858e-02	      5908	-1.678964677e+08	 0.000000000e+00	 2.672619934e-08	 0.000000000e+00
+9.250000000e-02	9.369454264e-02	     10840	 3.782552178e+07	 0.000000000e+00	 1.795179194e-08	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/xi2_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/xi2_lpp.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 1.111111111e+08 (particle-based, used), 4.538831600e+07 (mesh-based, alternative)
+# Normalisation factor: 1.111111111e+08 (particle)
+# Normalisation factor alternatives: 1.111111111e+08 (particle), 4.538831600e+07 (mesh), 8.158928783e+07 (mesh-mixed)
 # [0] r_cen, [1] r_eff, [2] npairs, [3] Re{xi2}, [4] Im{xi2}
-6.250000000e+01	6.431962465e+01	       157	 6.184653430e+01	-3.010018340e-15
-8.750000000e+01	8.777591768e+01	       292	 2.981831540e+02	-1.422291109e-14
-1.125000000e+02	1.122315212e+02	       529	 3.004480760e+02	 2.831944736e-15
-1.375000000e+02	1.381486607e+02	       820	 1.370759622e+01	 8.903680205e-16
+6.250000000e+01	6.431962465e+01	       314	 6.184653430e+01	-3.665585986e-15
+8.750000000e+01	8.777591768e+01	       584	 2.981831540e+02	-1.396938273e-15
+1.125000000e+02	1.122315212e+02	      1058	 3.004480760e+02	-9.083213088e-15
+1.375000000e+02	1.381486607e+02	      1640	 1.370759622e+01	 2.076378970e-15
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zetaw000_bin0.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
-# Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
+# Catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
+# Catalogue particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 8.142524244e+07 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+12 (particle)
+# Normalisation factor alternatives: 3.703703704e+12 (particle), 4.417104020e+03 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta000_raw}, [6] Im{zeta000_raw}, [7] Re{zeta000_shot}, [8] Im{zeta000_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 3.945082572e+04	 0.000000000e+00	 2.105564503e+04	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	8.750000000e+01	8.777591768e+01	       292	 1.237361281e+02	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	1.125000000e+02	1.122315212e+02	       529	-1.016546758e+04	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	1.375000000e+02	1.381486607e+02	       820	-1.811605867e+03	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	 1.068000923e+08	 6.901219445e-11	 2.779789991e+06	 6.376218938e-13
+6.250000000e+01	6.431962465e+01	8.750000000e+01	8.777591768e+01	       584	 9.890579500e+07	 2.605428804e-11	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.125000000e+02	1.122315212e+02	      1058	 9.970071289e+07	 2.329642099e-12	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.375000000e+02	1.381486607e+02	      1640	 1.006337717e+08	-7.738299012e-12	 0.000000000e+00	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zeta000_bin0_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_lpp.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta000_raw}, [6] Im{zeta000_raw}, [7] Re{zeta000_shot}, [8] Im{zeta000_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 3.984712201e+04	 0.000000000e+00	 2.216320643e+04	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	8.750000000e+01	8.777591768e+01	       292	-9.032833334e+02	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	1.125000000e+02	1.122315212e+02	       529	-1.167972323e+04	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
-6.250000000e+01	6.431962465e+01	1.375000000e+02	1.381486607e+02	       820	-1.287951495e+03	 0.000000000e+00	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	 3.984712201e+04	-3.359470921e-12	 1.108160322e+04	 5.640862872e-13
+6.250000000e+01	6.431962465e+01	8.750000000e+01	8.777591768e+01	       584	-9.032833334e+02	-2.001685603e-13	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.125000000e+02	1.122315212e+02	      1058	-1.167972323e+04	-1.365943336e-12	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.375000000e+02	1.381486607e+02	      1640	-1.287951495e+03	-4.918041022e-13	 0.000000000e+00	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_gpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_gpp.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Catalogue size: 3 particles of total sample weight 3.000
+# Catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Catalogue particle extents: ([450.000, 550.000], [456.699, 543.301], [500.000, 500.000])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 8.142524244e+07 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 8.142524244e+07 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta000_raw}, [6] Im{zeta000_raw}, [7] Re{zeta000_shot}, [8] Im{zeta000_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 3.945082572e+04	 0.000000000e+00	 2.105564503e+04	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       292	 1.508921453e+04	 0.000000000e+00	 2.504016503e+04	 0.000000000e+00
-1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	       529	-1.802677540e+04	 0.000000000e+00	 1.631875180e+04	 0.000000000e+00
-1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	       820	 3.211464934e+03	 0.000000000e+00	 6.383890248e+02	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	 3.945082572e+04	 6.950580231e-13	 1.052782252e+04	 2.760054093e-13
+6.250000000e+01	6.431962465e+01	8.750000000e+01	8.777591768e+01	       584	 1.237361281e+02	 9.778382360e-13	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.125000000e+02	1.122315212e+02	      1058	-1.016546758e+04	 3.162548194e-13	 0.000000000e+00	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	1.375000000e+02	1.381486607e+02	      1640	-1.811605867e+03	-1.659818691e-13	 0.000000000e+00	 0.000000000e+00
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zeta000_diag_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_lpp.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta000_raw}, [6] Im{zeta000_raw}, [7] Re{zeta000_shot}, [8] Im{zeta000_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 3.984712201e+04	 0.000000000e+00	 2.216320643e+04	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       292	 1.298808584e+04	 0.000000000e+00	 2.785966115e+04	 0.000000000e+00
-1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	       529	-1.337497363e+04	 0.000000000e+00	 1.534744686e+04	 0.000000000e+00
-1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	       820	 3.569578550e+03	 0.000000000e+00	 6.105297474e+02	 0.000000000e+00
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	 3.984712201e+04	-1.386977727e-12	 1.108160322e+04	 2.638504637e-13
+8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       584	 1.298808584e+04	 1.487970569e-12	 1.392983057e+04	 3.920232217e-13
+1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	      1058	-1.337497363e+04	 6.774963609e-13	 7.673723429e+03	-6.724440994e-14
+1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	      1640	 3.569578550e+03	 2.059235767e-13	 3.052648737e+02	-5.554559920e-14
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zeta202_diag_lpp.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_lpp.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
-# Data catalogue size: 3 particles of total sample weight 3.000
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
 # Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
 # Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Random catalogue size: 30000 particles of total sample weight 30000.000
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+16 (particle-based, used), 4.417104020e+15 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta202_raw}, [6] Im{zeta202_raw}, [7] Re{zeta202_shot}, [8] Im{zeta202_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 3.150294433e+04	 8.623696294e+02	 3.436193163e+04	 1.353572097e-13
-8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       292	-1.576434791e+03	-6.080253566e+02	 8.918398668e+04	 1.515635535e-12
-1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	       529	-1.120966787e+04	 4.076174762e+02	 4.965661784e+04	-1.217986629e-12
-1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	       820	 3.688257823e+02	 4.803109669e+02	 1.478206285e+03	 1.967587096e-13
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	-3.150294433e+04	-8.623696294e+02	 1.718096582e+04	 2.054957722e-12
+8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       584	 1.576434791e+03	 6.080253566e+02	 4.459199334e+04	-1.811923091e-12
+1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	      1058	 1.120966787e+04	-4.076174762e+02	 2.482830892e+04	-6.208523708e-14
+1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	      1640	-3.688257823e+02	-4.803109669e+02	 7.391031427e+02	-1.276923971e-13
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zetaw000_diag.txt` & `Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_lpp.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-# Catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Catalogue size: 30000 particles of total sample weight 30000.000
-# Catalogue particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Data catalogue source: extfile:tests/test_input/ctlgs/test_data_catalogue.txt
+# Data catalogue size: ntotal = 3, wtotal = 3.000, wstotal = 3.000
+# Data-source particle extents: ([450.002, 550.002], [471.122, 557.724], [500.017, 500.017])
+# Random catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
+# Random catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
+# Random-source particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+12 (particle-based, used), 4.417104020e+03 (mesh-based, alternative)
-# [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta000_raw}, [6] Im{zeta000_raw}, [7] Re{zeta000_shot}, [8] Im{zeta000_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 1.068000923e+08	 0.000000000e+00	 5.559579982e+06	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       292	 9.972766937e+07	 0.000000000e+00	 2.987769085e+06	 0.000000000e+00
-1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	       529	 1.001141931e+08	 0.000000000e+00	 1.650921567e+06	 0.000000000e+00
-1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	       820	 1.011786651e+08	 0.000000000e+00	 1.064927669e+06	 0.000000000e+00
+# Normalisation factor: 3.703703704e+16 (particle)
+# Normalisation factor alternatives: 3.703703704e+16 (particle), 4.417104020e+15 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
+# [0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, [5] Re{bk000_raw}, [6] Im{bk000_raw}, [7] Re{bk000_shot}, [8] Im{bk000_shot}
+1.750000000e-02	2.258782336e-02	1.750000000e-02	2.258782336e-02	       460	 3.129296339e+17	 0.000000000e+00	 2.860393289e+17	 1.204669081e-02
+1.750000000e-02	2.258782336e-02	4.250000000e-02	4.488283313e-02	      2340	 1.244926134e+17	 0.000000000e+00	 1.333700973e+17	 4.347106872e-03
+1.750000000e-02	2.258782336e-02	6.750000000e-02	6.912253858e-02	      5908	 2.098960240e+17	 0.000000000e+00	 2.075891723e+17	 7.844226065e-03
+1.750000000e-02	2.258782336e-02	9.250000000e-02	9.369454264e-02	     10840	 1.929396325e+17	 0.000000000e+00	 1.926016786e+17	 6.344097645e-03
```

### Comparing `Triumvirate-0.2.0/tests/test_input/stats/zetaw202_diag.txt` & `Triumvirate-0.2.1/tests/test_input/stats/zetaw202_diag.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Catalogue source: extfile:tests/test_input/ctlgs/test_rand_catalogue.txt
-# Catalogue size: 30000 particles of total sample weight 30000.000
+# Catalogue size: ntotal = 30000, wtotal = 30000.000, wstotal = 30000.000
 # Catalogue particle extents: ([0.015, 999.985], [0.017, 999.983], [0.031, 999.969])
-# Box size: (1000.000, 1000.000, 1000.000)
+# Box size: [1000.000, 1000.000, 1000.000]
 # Box alignment: centre
-# Mesh number: (64, 64, 64)
+# Mesh number: [64, 64, 64]
 # Mesh assignment and interlacing: tsc, False
-# Normalisation factor: 3.703703704e+12 (particle-based, used), 4.417104020e+03 (mesh-based, alternative)
+# Normalisation factor: 3.703703704e+12 (particle)
+# Normalisation factor alternatives: 3.703703704e+12 (particle), 4.417104020e+03 (mesh), 0.000000000e+00 (mesh-mixed; n/a)
 # [0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, [5] Re{zeta202_raw}, [6] Im{zeta202_raw}, [7] Re{zeta202_shot}, [8] Im{zeta202_shot}
-6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       157	 7.435066520e+04	 3.966588958e+05	 2.190681805e+04	 0.000000000e+00
-8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       292	-3.484985079e+05	 7.448528021e+04	 7.404839828e+03	-5.744309809e-13
-1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	       529	-1.541766206e+05	 9.198698266e+04	 2.743919794e+03	 8.616464714e-13
-1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	       820	-2.161243758e+05	 9.939665590e+04	 4.455793103e+03	 8.616464714e-13
+6.250000000e+01	6.431962465e+01	6.250000000e+01	6.431962465e+01	       314	-7.435066520e+04	-3.966588958e+05	 1.095340902e+04	-5.499558323e-13
+8.750000000e+01	8.777591768e+01	8.750000000e+01	8.777591768e+01	       584	 3.484985079e+05	-7.448528021e+04	 3.702419914e+03	 1.416244534e-12
+1.125000000e+02	1.122315212e+02	1.125000000e+02	1.122315212e+02	      1058	 1.541766206e+05	-9.198698266e+04	 1.371959897e+03	 3.837194074e-13
+1.375000000e+02	1.381486607e+02	1.375000000e+02	1.381486607e+02	      1640	 2.161243758e+05	-9.939665590e+04	 2.227896552e+03	 4.036107001e-13
```

### Comparing `Triumvirate-0.2.0/tests/test_logger.py` & `Triumvirate-0.2.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_parameters.py` & `Triumvirate-0.2.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_threept.py` & `Triumvirate-0.2.1/tests/test_threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.0/tests/test_twopt.py` & `Triumvirate-0.2.1/tests/test_twopt.py`

 * *Files identical despite different names*

