# Comparing `tmp/TB2J-0.7.6.1.tar.gz` & `tmp/TB2J-0.7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.7.6.1.tar", last modified: Thu May 11 08:31:23 2023, max compression
+gzip compressed data, was "TB2J-0.7.6.2.tar", last modified: Wed Jun 21 12:31:45 2023, max compression
```

## Comparing `TB2J-0.7.6.1.tar` & `TB2J-0.7.6.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.724813 TB2J-0.7.6.1/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1327 2020-07-08 14:12:19.000000 TB2J-0.7.6.1/LICENSE
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1256 2023-05-11 08:31:23.724813 TB2J-0.7.6.1/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1902 2023-01-10 13:52:13.000000 TB2J-0.7.6.1/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.716813 TB2J-0.7.6.1/TB2J/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7121 2022-10-28 09:32:56.000000 TB2J-0.7.6.1/TB2J/Jdownfolder.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1771 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/Jtensor.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3994 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/Oiju.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7423 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/Oiju_epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       24 2023-05-11 10:16:37.000000 TB2J-0.7.6.1/TB2J/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2884 2022-02-27 23:27:25.000000 TB2J-0.7.6.1/TB2J/citation.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2489 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/contour.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3518 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    29406 2023-05-11 10:11:51.000000 TB2J-0.7.6.1/TB2J/exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    11701 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/exchangeCL2.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     8372 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/exchange_pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9017 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/exchange_qspace.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.720813 TB2J-0.7.6.1/TB2J/external/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      137 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/external/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5943 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/external/p_tqdm.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6630 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/gpaw_wrapper.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12286 2023-04-13 10:00:17.000000 TB2J-0.7.6.1/TB2J/green.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1571 2022-10-07 20:57:03.000000 TB2J-0.7.6.1/TB2J/greentest.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.720813 TB2J-0.7.6.1/TB2J/io_exchange/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       32 2020-07-08 14:12:19.000000 TB2J-0.7.6.1/TB2J/io_exchange/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    16870 2022-10-28 09:32:56.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6720 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_multibinit.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4024 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_tomsasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10198 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_txt.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3190 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_uppasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5639 2022-10-28 09:32:56.000000 TB2J-0.7.6.1/TB2J/io_exchange/io_vampire.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6921 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/io_merge.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      533 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/kpoints.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    18356 2023-03-08 08:29:40.000000 TB2J-0.7.6.1/TB2J/manager.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    17974 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/myTB.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4756 2022-08-08 19:50:55.000000 TB2J-0.7.6.1/TB2J/orbmap.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4092 2022-02-27 23:27:25.000000 TB2J-0.7.6.1/TB2J/pauli.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1223 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1435 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/plot.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1126 2021-05-27 13:46:56.000000 TB2J-0.7.6.1/TB2J/rotate_atoms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    11639 2023-04-13 10:00:17.000000 TB2J-0.7.6.1/TB2J/sisl_wrapper.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.720813 TB2J-0.7.6.1/TB2J/spinham/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-08 14:12:19.000000 TB2J-0.7.6.1/TB2J/spinham/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2234 2021-09-17 19:59:43.000000 TB2J-0.7.6.1/TB2J/spinham/base_parser.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      741 2020-07-08 14:12:19.000000 TB2J-0.7.6.1/TB2J/spinham/constants.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    16545 2023-05-11 10:12:24.000000 TB2J-0.7.6.1/TB2J/spinham/hamiltonian.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9870 2021-11-24 10:31:21.000000 TB2J-0.7.6.1/TB2J/spinham/hamiltonian_terms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7011 2022-04-19 19:03:09.000000 TB2J-0.7.6.1/TB2J/spinham/plot.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2215 2022-08-04 12:47:35.000000 TB2J-0.7.6.1/TB2J/spinham/qsolver.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2238 2021-02-01 11:14:39.000000 TB2J-0.7.6.1/TB2J/spinham/spin_api.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10923 2022-04-19 19:03:17.000000 TB2J-0.7.6.1/TB2J/spinham/spin_xml.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.6.1/TB2J/spinham/supercell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3896 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/utest.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9358 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/utils.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      276 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/TB2J/versioninfo.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.720813 TB2J-0.7.6.1/TB2J/wannier/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       70 2021-10-04 10:59:57.000000 TB2J-0.7.6.1/TB2J/wannier/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4092 2023-01-10 13:52:13.000000 TB2J-0.7.6.1/TB2J/wannier/w90_parser.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.720813 TB2J-0.7.6.1/TB2J.egg-info/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1256 2023-05-11 08:31:23.000000 TB2J-0.7.6.1/TB2J.egg-info/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1367 2023-05-11 08:31:23.000000 TB2J-0.7.6.1/TB2J.egg-info/SOURCES.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2023-05-11 08:31:23.000000 TB2J-0.7.6.1/TB2J.egg-info/dependency_links.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       68 2023-05-11 08:31:23.000000 TB2J-0.7.6.1/TB2J.egg-info/requires.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        5 2023-05-11 08:31:23.000000 TB2J-0.7.6.1/TB2J.egg-info/top_level.txt
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-05-11 08:31:23.724813 TB2J-0.7.6.1/scripts/
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     2160 2022-10-28 09:32:56.000000 TB2J-0.7.6.1/scripts/TB2J_downfold.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1186 2022-08-04 12:29:36.000000 TB2J-0.7.6.1/scripts/TB2J_eigen.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     3415 2023-05-11 10:11:51.000000 TB2J-0.7.6.1/scripts/TB2J_magnon.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1475 2022-10-28 09:34:11.000000 TB2J-0.7.6.1/scripts/TB2J_merge.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)      715 2021-11-24 10:31:21.000000 TB2J-0.7.6.1/scripts/TB2J_rotate.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     5083 2022-12-13 21:35:26.000000 TB2J-0.7.6.1/scripts/siesta2J.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     7092 2022-09-04 19:02:49.000000 TB2J-0.7.6.1/scripts/wann2J.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2023-05-11 08:31:23.724813 TB2J-0.7.6.1/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1787 2023-05-11 10:13:02.000000 TB2J-0.7.6.1/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1327 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1902 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.042108 TB2J-0.7.6.2/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7121 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1771 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3994 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7423 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       24 2023-06-21 12:30:10.000000 TB2J-0.7.6.2/TB2J/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2884 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2489 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3518 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29406 2023-06-21 12:28:48.000000 TB2J-0.7.6.2/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11701 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8372 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9017 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.042108 TB2J-0.7.6.2/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5943 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6630 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12286 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1571 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16870 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6720 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4024 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10198 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3190 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5639 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6921 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      533 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    18356 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17974 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4756 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1223 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1435 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     2144 2023-06-21 12:30:10.000000 TB2J-0.7.6.2/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11639 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.7.6.2/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2234 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/spinham/base_parser.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)      741 2020-07-08 14:12:19.000000 TB2J-0.7.6.2/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16545 2023-05-26 14:16:44.000000 TB2J-0.7.6.2/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9870 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7011 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2215 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2238 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10923 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/spinham/spin_xml.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.6.2/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3896 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9358 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      276 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       70 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/TB2J/wannier/w90_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.042108 TB2J-0.7.6.2/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2023-06-21 12:31:45.000000 TB2J-0.7.6.2/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1367 2023-06-21 12:31:45.000000 TB2J-0.7.6.2/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2023-06-21 12:31:45.000000 TB2J-0.7.6.2/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       68 2023-06-21 12:31:45.000000 TB2J-0.7.6.2/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2023-06-21 12:31:45.000000 TB2J-0.7.6.2/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     2160 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1186 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3415 2023-05-10 13:02:58.000000 TB2J-0.7.6.2/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1475 2023-05-09 15:15:38.000000 TB2J-0.7.6.2/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      715 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/scripts/TB2J_rotate.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     5083 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     7092 2023-05-09 15:15:14.000000 TB2J-0.7.6.2/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2023-06-21 12:31:45.046108 TB2J-0.7.6.2/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1787 2023-06-21 12:30:10.000000 TB2J-0.7.6.2/setup.py
```

### Comparing `TB2J-0.7.6.1/LICENSE` & `TB2J-0.7.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/PKG-INFO` & `TB2J-0.7.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.6.1
+Version: 0.7.6.2
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.6.1/README.md` & `TB2J-0.7.6.2/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/Jdownfolder.py` & `TB2J-0.7.6.2/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/Jtensor.py` & `TB2J-0.7.6.2/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/Oiju.py` & `TB2J-0.7.6.2/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/Oiju_epc.py` & `TB2J-0.7.6.2/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/citation.py` & `TB2J-0.7.6.2/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/contour.py` & `TB2J-0.7.6.2/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/epc.py` & `TB2J-0.7.6.2/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/exchange.py` & `TB2J-0.7.6.2/TB2J/exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/exchangeCL2.py` & `TB2J-0.7.6.2/TB2J/exchangeCL2.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/exchange_pert.py` & `TB2J-0.7.6.2/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/exchange_qspace.py` & `TB2J-0.7.6.2/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/external/p_tqdm.py` & `TB2J-0.7.6.2/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/gpaw_wrapper.py` & `TB2J-0.7.6.2/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/green.py` & `TB2J-0.7.6.2/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/greentest.py` & `TB2J-0.7.6.2/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_exchange.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_txt.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_exchange/io_vampire.py` & `TB2J-0.7.6.2/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/io_merge.py` & `TB2J-0.7.6.2/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/kpoints.py` & `TB2J-0.7.6.2/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/manager.py` & `TB2J-0.7.6.2/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/myTB.py` & `TB2J-0.7.6.2/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/orbmap.py` & `TB2J-0.7.6.2/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/pauli.py` & `TB2J-0.7.6.2/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/pert.py` & `TB2J-0.7.6.2/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/plot.py` & `TB2J-0.7.6.2/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/rotate_atoms.py` & `TB2J-0.7.6.2/TB2J/rotate_atoms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 import copy
 from ase.io import read, write
+import numpy as np 
 
 def rotate_atom_xyz(atoms):
     """
     given a atoms, return:
     - 'z'->'x'
     - 'z'->'y'
     - 'z'->'z'
@@ -12,14 +13,54 @@
     atoms_x = copy.deepcopy(atoms)
     atoms_x.rotate(90, 'y', rotate_cell=True)
     atoms_y = copy.deepcopy(atoms)
     atoms_y.rotate(90, 'x', rotate_cell=True)
     atoms_z = atoms
     return atoms_x, atoms_y, atoms_z
 
+def rotate_atom_spin(atoms):
+    """
+    given a atoms, return the atoms with rotated spin:
+    - 'z'->'x'
+    - 'z'->'y'
+    - 'z'->'z'
+    """
+    magmoms=np.array(atoms.get_initial_magnetic_moments())
+    if len(magmoms.shape)==1:
+        m=np.zeros((len(magmoms), 3), dtype=float)
+        m[:,2]=magmoms
+    else:
+        m=magmoms
+    atoms_copy=copy.deepcopy(atoms)
+    atoms.set_initial_magnetic_moments(None)
+
+    m_x = copy.deepcopy(m)
+    m_x[:,0] = m[:,2] 
+    m_x[:,1] = m[:,1]
+    m_x[:,2] = m[:,0]
+    atoms_x = copy.deepcopy(atoms_copy)
+    atoms_x.set_initial_magnetic_moments(m_x)
+
+    m_y = copy.deepcopy(m)
+    m_y[:,0] = m[:,0]
+    m_y[:,1] = m[:,2]
+    m_y[:,2] = m[:,1]
+    atoms_y = copy.deepcopy(atoms_copy)
+    atoms_y.set_initial_magnetic_moments(m_y)
+
+    m_z = copy.deepcopy(m)
+    m_z[:,0] = m[:,0]
+    m_z[:,1] = m[:,1]
+    m_z[:,2] = m[:,2]
+    atoms_z = copy.deepcopy(atoms_copy)
+    atoms_z.set_initial_magnetic_moments(m_z)
+
+    return atoms_x, atoms_y, atoms_z
+
+
 
 def check_ftype(ftype):
     if ftype in ['cif']:
         print("="*40)
         print("WARNING!!!!!")
         print(f'{ftype} type does not contains the cell matrix explicitly. Therefore the outputted files does not give the rotation properly. Please use another format.')
         print("="*40)
```

### Comparing `TB2J-0.7.6.1/TB2J/sisl_wrapper.py` & `TB2J-0.7.6.2/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/base_parser.py` & `TB2J-0.7.6.2/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/constants.py` & `TB2J-0.7.6.2/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/hamiltonian.py` & `TB2J-0.7.6.2/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.7.6.2/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/plot.py` & `TB2J-0.7.6.2/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/qsolver.py` & `TB2J-0.7.6.2/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/spin_api.py` & `TB2J-0.7.6.2/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/spin_xml.py` & `TB2J-0.7.6.2/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/spinham/supercell.py` & `TB2J-0.7.6.2/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/utest.py` & `TB2J-0.7.6.2/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/utils.py` & `TB2J-0.7.6.2/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J/wannier/w90_parser.py` & `TB2J-0.7.6.2/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/TB2J.egg-info/PKG-INFO` & `TB2J-0.7.6.2/TB2J.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.6.1
+Version: 0.7.6.2
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.6.1/TB2J.egg-info/SOURCES.txt` & `TB2J-0.7.6.2/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/TB2J_downfold.py` & `TB2J-0.7.6.2/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/TB2J_eigen.py` & `TB2J-0.7.6.2/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/TB2J_magnon.py` & `TB2J-0.7.6.2/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/TB2J_merge.py` & `TB2J-0.7.6.2/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/TB2J_rotate.py` & `TB2J-0.7.6.2/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/siesta2J.py` & `TB2J-0.7.6.2/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/scripts/wann2J.py` & `TB2J-0.7.6.2/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.6.1/setup.py` & `TB2J-0.7.6.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.7.6.1"
+__version__ = "0.7.6.2"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name='TB2J',
     version=__version__,
     description='TB2J: First principle to Heisenberg exchange J using tight-binding Green function method',
```

