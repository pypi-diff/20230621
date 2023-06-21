# Comparing `tmp/zapf-0.4.2.tar.gz` & `tmp/zapf-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zapf-0.4.2.tar", last modified: Thu May 12 11:51:02 2022, max compression
+gzip compressed data, was "zapf-0.4.6.tar", last modified: Wed Jun 21 09:02:38 2023, max compression
```

## Comparing `zapf-0.4.2.tar` & `zapf-0.4.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.837900 zapf-0.4.2/
--rw-r--r--   0 gbr       (1000) gbr       (1000)      107 2019-03-17 12:34:08.000000 zapf-0.4.2/.gitignore
--rw-r--r--   0 gbr       (1000) gbr       (1000)      177 2022-05-12 05:32:58.000000 zapf-0.4.2/.isort.cfg
--rw-r--r--   0 gbr       (1000) gbr       (1000)    18137 2021-10-07 06:25:33.000000 zapf-0.4.2/LICENSE
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1086 2021-04-21 16:31:20.000000 zapf-0.4.2/Makefile
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1697 2022-05-12 11:51:02.837900 zapf-0.4.2/PKG-INFO
--rw-r--r--   0 gbr       (1000) gbr       (1000)      907 2021-06-11 13:47:48.000000 zapf-0.4.2/README.rst
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.832899 zapf-0.4.2/debian/
--rw-r--r--   0 gbr       (1000) gbr       (1000)     7952 2022-05-12 11:50:48.000000 zapf-0.4.2/debian/changelog
--rw-r--r--   0 gbr       (1000) gbr       (1000)        3 2021-04-23 06:03:23.000000 zapf-0.4.2/debian/compat
--rw-r--r--   0 gbr       (1000) gbr       (1000)      502 2021-04-23 06:03:23.000000 zapf-0.4.2/debian/control
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1178 2021-04-23 06:03:23.000000 zapf-0.4.2/debian/copyright
--rwxr-xr-x   0 gbr       (1000) gbr       (1000)      502 2021-04-23 06:03:23.000000 zapf-0.4.2/debian/rules
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.832899 zapf-0.4.2/debian/source/
--rw-r--r--   0 gbr       (1000) gbr       (1000)       13 2021-04-23 06:03:23.000000 zapf-0.4.2/debian/source/format
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.833899 zapf-0.4.2/doc/
--rw-r--r--   0 gbr       (1000) gbr       (1000)      634 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/Makefile
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.833899 zapf-0.4.2/doc/_static/
--rw-r--r--   0 gbr       (1000) gbr       (1000)   168539 2021-06-11 13:58:36.000000 zapf-0.4.2/doc/_static/logo.png
--rw-r--r--   0 gbr       (1000) gbr       (1000)   427468 2021-06-11 13:58:33.000000 zapf-0.4.2/doc/_static/logo.xcf
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1273 2021-11-09 18:21:32.000000 zapf-0.4.2/doc/conf.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     4388 2021-10-19 12:35:46.000000 zapf-0.4.2/doc/device.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)      203 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/errors.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)      263 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/index.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)      987 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/intro.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)      407 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/proto.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)      316 2021-06-11 13:47:48.000000 zapf-0.4.2/doc/scanner.rst
--rw-r--r--   0 gbr       (1000) gbr       (1000)     7528 2021-10-07 09:14:03.000000 zapf-0.4.2/pylintrc
--rw-r--r--   0 gbr       (1000) gbr       (1000)      122 2022-05-12 11:46:04.000000 zapf-0.4.2/pyproject.toml
--rwxr-xr-x   0 gbr       (1000) gbr       (1000)       15 2021-06-11 13:47:48.000000 zapf-0.4.2/requirements.txt
--rw-r--r--   0 gbr       (1000) gbr       (1000)      376 2022-05-12 05:32:58.000000 zapf-0.4.2/scan.py
--rwxr-xr-x   0 gbr       (1000) gbr       (1000)      872 2022-05-12 11:51:02.837900 zapf-0.4.2/setup.cfg
--rw-r--r--   0 gbr       (1000) gbr       (1000)       57 2022-05-12 11:43:55.000000 zapf-0.4.2/setup.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.834899 zapf-0.4.2/test/
--rw-r--r--   0 gbr       (1000) gbr       (1000)        0 2021-04-21 16:09:01.000000 zapf-0.4.2/test/__init__.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     6771 2021-11-09 18:21:26.000000 zapf-0.4.2/test/conftest.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    12169 2022-05-12 05:32:58.000000 zapf-0.4.2/test/test_devices.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     3059 2021-11-09 18:21:32.000000 zapf-0.4.2/test/test_scan.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     3464 2021-11-09 18:21:32.000000 zapf-0.4.2/test/test_spec.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    25286 2021-11-09 18:21:26.000000 zapf-0.4.2/test/testplc_2015_02.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    48576 2021-11-09 18:29:11.000000 zapf-0.4.2/test/testplc_2021_09.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.834899 zapf-0.4.2/tools/
--rwxr-xr-x   0 gbr       (1000) gbr       (1000)     2524 2021-11-18 18:24:37.000000 zapf-0.4.2/tools/sim-standalone.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.835899 zapf-0.4.2/zapf/
--rw-r--r--   0 gbr       (1000) gbr       (1000)       18 2022-05-12 05:48:27.000000 zapf-0.4.2/zapf/RELEASE-VERSION
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1809 2021-11-09 18:21:33.000000 zapf-0.4.2/zapf/__init__.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    38908 2022-05-12 05:32:58.000000 zapf-0.4.2/zapf/device.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    10601 2021-11-09 18:21:32.000000 zapf-0.4.2/zapf/indexer.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    13799 2022-05-12 05:32:58.000000 zapf-0.4.2/zapf/io.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.836900 zapf-0.4.2/zapf/proto/
--rw-r--r--   0 gbr       (1000) gbr       (1000)     2560 2021-11-09 18:21:32.000000 zapf-0.4.2/zapf/proto/__init__.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    16488 2022-05-12 05:32:58.000000 zapf-0.4.2/zapf/proto/ads.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     6081 2021-11-15 07:09:32.000000 zapf-0.4.2/zapf/proto/modbus.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     4117 2021-11-13 08:21:15.000000 zapf-0.4.2/zapf/proto/sim.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     5178 2021-11-13 09:22:47.000000 zapf-0.4.2/zapf/proto/tango.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    14354 2021-11-09 18:21:32.000000 zapf-0.4.2/zapf/scan.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.836900 zapf-0.4.2/zapf/simulator/
--rw-r--r--   0 gbr       (1000) gbr       (1000)        0 2021-04-26 08:08:36.000000 zapf-0.4.2/zapf/simulator/__init__.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1355 2021-10-07 16:57:17.000000 zapf-0.4.2/zapf/simulator/funcs.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    14573 2021-11-13 08:21:15.000000 zapf-0.4.2/zapf/simulator/runtime.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     6742 2022-05-12 05:32:58.000000 zapf-0.4.2/zapf/simulator/server.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     5781 2021-10-21 11:11:26.000000 zapf-0.4.2/zapf/simulator/util.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.837900 zapf-0.4.2/zapf/spec/
--rw-r--r--   0 gbr       (1000) gbr       (1000)     4114 2021-10-27 12:24:16.000000 zapf-0.4.2/zapf/spec/__init__.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     6062 2021-11-18 18:24:37.000000 zapf-0.4.2/zapf/spec/v_2015_02.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)    33234 2021-11-09 18:21:33.000000 zapf-0.4.2/zapf/spec/v_2021_09.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     9820 2022-05-12 05:32:58.000000 zapf-0.4.2/zapf/table.py
--rw-r--r--   0 gbr       (1000) gbr       (1000)     3488 2021-11-09 18:21:26.000000 zapf-0.4.2/zapf/util.py
-drwxr-xr-x   0 gbr       (1000) gbr       (1000)        0 2022-05-12 11:51:02.835899 zapf-0.4.2/zapf.egg-info/
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1697 2022-05-12 11:51:02.000000 zapf-0.4.2/zapf.egg-info/PKG-INFO
--rw-r--r--   0 gbr       (1000) gbr       (1000)     1057 2022-05-12 11:51:02.000000 zapf-0.4.2/zapf.egg-info/SOURCES.txt
--rw-r--r--   0 gbr       (1000) gbr       (1000)        1 2022-05-12 11:51:02.000000 zapf-0.4.2/zapf.egg-info/dependency_links.txt
--rw-r--r--   0 gbr       (1000) gbr       (1000)        5 2022-05-12 11:51:02.000000 zapf-0.4.2/zapf.egg-info/top_level.txt
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.794714 zapf-0.4.6/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      107 2019-03-25 10:50:41.000000 zapf-0.4.6/.gitignore
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      177 2022-03-14 10:16:20.000000 zapf-0.4.6/.isort.cfg
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    18137 2019-03-25 10:50:41.000000 zapf-0.4.6/LICENSE
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1086 2021-04-22 08:48:58.000000 zapf-0.4.6/Makefile
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-06-21 09:02:38.794714 zapf-0.4.6/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      907 2021-06-11 14:35:30.000000 zapf-0.4.6/README.rst
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.788714 zapf-0.4.6/debian/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8596 2023-06-21 09:02:31.000000 zapf-0.4.6/debian/changelog
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        3 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/compat
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      527 2022-05-19 16:40:52.000000 zapf-0.4.6/debian/control
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1178 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/copyright
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)      502 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/rules
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.789714 zapf-0.4.6/debian/source/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       13 2021-04-23 11:05:09.000000 zapf-0.4.6/debian/source/format
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.789714 zapf-0.4.6/doc/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      634 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/Makefile
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.790714 zapf-0.4.6/doc/_static/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   168539 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/_static/logo.png
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)   427468 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/_static/logo.xcf
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1273 2021-11-12 08:23:59.000000 zapf-0.4.6/doc/conf.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4388 2021-10-21 04:57:33.000000 zapf-0.4.6/doc/device.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      203 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/errors.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      263 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/index.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      987 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/intro.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      407 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/proto.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      316 2021-06-11 14:35:30.000000 zapf-0.4.6/doc/scanner.rst
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     7528 2021-04-23 11:05:09.000000 zapf-0.4.6/pylintrc
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      122 2022-05-12 11:50:21.000000 zapf-0.4.6/pyproject.toml
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)       15 2021-06-11 14:35:30.000000 zapf-0.4.6/requirements.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      376 2022-03-14 10:16:16.000000 zapf-0.4.6/scan.py
+-rwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)      872 2023-06-21 09:02:38.794714 zapf-0.4.6/setup.cfg
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       57 2022-05-12 11:50:21.000000 zapf-0.4.6/setup.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.791714 zapf-0.4.6/test/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-22 08:48:58.000000 zapf-0.4.6/test/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6771 2021-11-08 08:47:11.000000 zapf-0.4.6/test/conftest.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    12169 2022-03-14 10:16:13.000000 zapf-0.4.6/test/test_devices.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3059 2021-11-08 08:47:11.000000 zapf-0.4.6/test/test_scan.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3464 2021-11-12 08:23:59.000000 zapf-0.4.6/test/test_spec.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    25286 2021-11-08 09:47:15.000000 zapf-0.4.6/test/testplc_2015_02.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    48576 2021-11-12 08:23:59.000000 zapf-0.4.6/test/testplc_2021_09.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.791714 zapf-0.4.6/tools/
+-rwxrwxr-x   0 gbrandl   (1000) gbrandl   (1000)     2524 2021-11-19 10:53:12.000000 zapf-0.4.6/tools/sim-standalone.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.792714 zapf-0.4.6/zapf/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        6 2022-05-11 17:22:16.000000 zapf-0.4.6/zapf/RELEASE-VERSION
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1809 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    39161 2023-05-18 05:30:50.000000 zapf-0.4.6/zapf/device.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10601 2022-10-26 05:57:09.000000 zapf-0.4.6/zapf/indexer.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13837 2023-06-21 07:33:05.000000 zapf-0.4.6/zapf/io.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/proto/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2560 2021-04-26 13:20:39.000000 zapf-0.4.6/zapf/proto/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    16488 2021-11-19 13:08:34.000000 zapf-0.4.6/zapf/proto/ads.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6081 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/modbus.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4117 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/sim.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5178 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/proto/tango.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    14575 2023-05-18 05:30:50.000000 zapf-0.4.6/zapf/scan.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/simulator/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2021-04-26 13:20:39.000000 zapf-0.4.6/zapf/simulator/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1355 2021-10-11 05:32:57.000000 zapf-0.4.6/zapf/simulator/funcs.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    14573 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/simulator/runtime.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6742 2022-03-14 10:16:16.000000 zapf-0.4.6/zapf/simulator/server.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5781 2021-11-08 08:44:16.000000 zapf-0.4.6/zapf/simulator/util.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.793714 zapf-0.4.6/zapf/spec/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4114 2021-11-08 08:47:11.000000 zapf-0.4.6/zapf/spec/__init__.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6062 2021-11-17 11:33:49.000000 zapf-0.4.6/zapf/spec/v_2015_02.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    33234 2021-11-17 15:35:39.000000 zapf-0.4.6/zapf/spec/v_2021_09.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9820 2022-03-14 10:16:16.000000 zapf-0.4.6/zapf/table.py
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3488 2021-11-08 09:47:15.000000 zapf-0.4.6/zapf/util.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2023-06-21 09:02:38.792714 zapf-0.4.6/zapf.egg-info/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1697 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1057 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        1 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        5 2023-06-21 09:02:38.000000 zapf-0.4.6/zapf.egg-info/top_level.txt
```

### Comparing `zapf-0.4.2/LICENSE` & `zapf-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/Makefile` & `zapf-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/PKG-INFO` & `zapf-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zapf
-Version: 0.4.2
+Version: 0.4.6
 Summary: Client library for the PILS specification
 Home-page: https://forge.frm2.tum.de/review/plugins/gitiles/mlz/pils/zapf
 Author: Georg Brandl
 Author-email: g.brandl@fz-juelich.de
 License: GPL-2.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zapf-0.4.2/README.rst` & `zapf-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/debian/changelog` & `zapf-0.4.6/debian/changelog`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+python-zapf (0.4.6) focal; urgency=medium
+
+  * io: fix missing locked access to proto
+
+ -- Georg Brandl <jenkins@frm2.tum.de>  Wed, 21 Jun 2023 09:34:30 +0200
+
+python-zapf (0.4.5) focal; urgency=medium
+
+  * adapt to minor spec clarification
+
+ -- Enrico Faulhaber <jenkins@frm2.tum.de>  Wed, 17 May 2023 16:25:01 +0200
+
+python-zapf (0.4.4) focal; urgency=medium
+
+  * fix up limits
+
+ -- Enrico Faulhaber <jenkins@frm2.tum.de>  Wed, 25 Jan 2023 08:57:55 +0100
+
+python-zapf (0.4.3) focal; urgency=medium
+
+  * debian: add missing dependency of setuptools_scm
+
+ -- Georg Brandl <jenkins@jenkins02.admin.frm2.tum.de>  Thu, 19 May 2022 18:41:00 +0200
+
 python-zapf (0.4.2) focal; urgency=medium
 
   * switch to pyproject.toml/setup.cfg based build
 
  -- Georg Brandl <jenkins@frm2.tum.de>  Thu, 12 May 2022 13:50:28 +0200
 
 python-zapf (0.4.1) focal; urgency=medium
```

### Comparing `zapf-0.4.2/debian/copyright` & `zapf-0.4.6/debian/copyright`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/Makefile` & `zapf-0.4.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/_static/logo.png` & `zapf-0.4.6/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/_static/logo.xcf` & `zapf-0.4.6/doc/_static/logo.xcf`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/conf.py` & `zapf-0.4.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/device.rst` & `zapf-0.4.6/doc/device.rst`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/doc/intro.rst` & `zapf-0.4.6/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/pylintrc` & `zapf-0.4.6/pylintrc`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/setup.cfg` & `zapf-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/conftest.py` & `zapf-0.4.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/test_devices.py` & `zapf-0.4.6/test/test_devices.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/test_scan.py` & `zapf-0.4.6/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/test_spec.py` & `zapf-0.4.6/test/test_spec.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/testplc_2015_02.py` & `zapf-0.4.6/test/testplc_2015_02.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/test/testplc_2021_09.py` & `zapf-0.4.6/test/testplc_2021_09.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/tools/sim-standalone.py` & `zapf-0.4.6/tools/sim-standalone.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/__init__.py` & `zapf-0.4.6/zapf/__init__.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/device.py` & `zapf-0.4.6/zapf/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,14 @@
         This is normally equivalent to `change_status(..., RESET)` with all
         error or unknown states as the initial states.  However, special
         devices like MessageIO can have a different reset strategy.
         """
         error_stati = set(range(16)) - {
             DevStatus.RESET,
             DevStatus.IDLE,
-            DevStatus.DISABLED,
             DevStatus.WARN,
             DevStatus.START,
             DevStatus.BUSY,
             DevStatus.STOP,
             DevStatus.DIAGNOSTIC_ERROR,
         }
         return self.change_status(error_stati, DevStatus.RESET)
@@ -1021,7 +1020,18 @@
     elif typecode == 0x1E03:
         name += ' (16 bit, legacy)'
     elif (typecode) >> 8 == 5:
         name += f' ({valuesize} bytes)'
     else:
         name += f' ({valuesize*8} bit)'
     return name
+
+FMT_LIMITS = {
+    'h' : (-(2**15), 2**15-1),
+    'H' : (0, 2**16-1),
+    'i' : (-(2**31), 2**31-1),
+    'I' : (0, 2**32-1),
+    'q' : (-(2**63), 2**63-1),
+    'Q' : (0, 2**64-1),
+    'f' : (-3.403823e38, 3.403823e38),
+    'd' : (-1.7976931348623157e+308, 1.7976931348623157e+308),
+}
```

### Comparing `zapf-0.4.2/zapf/indexer.py` & `zapf-0.4.6/zapf/indexer.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/io.py` & `zapf-0.4.6/zapf/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,16 @@
         else:
             fmt_ = self.byteorder + 'H'
         size = calcsize(fmt_)
         assert size in (2, 6, 10)
         if cached:
             data = self.cache.get(addr, size)
         else:
-            data = self.proto.read(addr, size)
+            with self.cache.lock:
+                data = self.proto.read(addr, size)
         if fmt == 'f':
             # honor floatconv, if required
             data = data[:2] + self.floatconv(data[2:])
         return (*unpack(fmt_, data), None)[:2]
 
     # Note: floatconv is not used for 64-bit floats, since the PLCs that would
     # need floatconv don't support them.
```

### Comparing `zapf-0.4.2/zapf/proto/__init__.py` & `zapf-0.4.6/zapf/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/proto/ads.py` & `zapf-0.4.6/zapf/proto/ads.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/proto/modbus.py` & `zapf-0.4.6/zapf/proto/modbus.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/proto/sim.py` & `zapf-0.4.6/zapf/proto/sim.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/proto/tango.py` & `zapf-0.4.6/zapf/proto/tango.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/scan.py` & `zapf-0.4.6/zapf/scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # *****************************************************************************
 
 """Support for scanning the indexer and creating devices."""
 
 from collections import namedtuple
 
 from zapf import SpecError, spec
-from zapf.device import TYPECODE_MAP, Device
+from zapf.device import TYPECODE_MAP, Device, FMT_LIMITS
 from zapf.io import PlcIO
 from zapf.spec import FMT_TO_BASETYPE, v_2015_02
 from zapf.spec.v_2021_09 import fix_unit
 
 DeviceInfo = namedtuple('DeviceInfo', 'name addr typecode info')
 
 
@@ -286,14 +286,20 @@
                         params[par.pop('name')] = par
 
             basetype, width = FMT_TO_BASETYPE.get(tce.value_fmt, (None, 0))
             # Keyword/RealValue are special
             access = 'rw' if (tce.has_target or typecode >> 8 in (0x14, 0x15)) \
                 else 'ro'
 
+            # fixup limits, if needed
+            limits = FMT_LIMITS.get(tce.value_fmt)
+            if limits:
+                absmin = max(absmin, limits[0])
+                absmax = min(absmax, limits[1])
+
             info = dict(unit=unit,
                         absmin=absmin, absmax=absmax,
                         params=params, funcs=funcs,
                         aux=aux, tables={}, flags=flags,
                         errid=[(0, 16, 'errid', {})],
                         description='',
                         access=access,
```

### Comparing `zapf-0.4.2/zapf/simulator/funcs.py` & `zapf-0.4.6/zapf/simulator/funcs.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/simulator/runtime.py` & `zapf-0.4.6/zapf/simulator/runtime.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/simulator/server.py` & `zapf-0.4.6/zapf/simulator/server.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/simulator/util.py` & `zapf-0.4.6/zapf/simulator/util.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/spec/__init__.py` & `zapf-0.4.6/zapf/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/spec/v_2015_02.py` & `zapf-0.4.6/zapf/spec/v_2015_02.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/spec/v_2021_09.py` & `zapf-0.4.6/zapf/spec/v_2021_09.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/table.py` & `zapf-0.4.6/zapf/table.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf/util.py` & `zapf-0.4.6/zapf/util.py`

 * *Files identical despite different names*

### Comparing `zapf-0.4.2/zapf.egg-info/PKG-INFO` & `zapf-0.4.6/zapf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zapf
-Version: 0.4.2
+Version: 0.4.6
 Summary: Client library for the PILS specification
 Home-page: https://forge.frm2.tum.de/review/plugins/gitiles/mlz/pils/zapf
 Author: Georg Brandl
 Author-email: g.brandl@fz-juelich.de
 License: GPL-2.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zapf-0.4.2/zapf.egg-info/SOURCES.txt` & `zapf-0.4.6/zapf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

