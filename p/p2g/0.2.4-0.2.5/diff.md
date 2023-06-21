# Comparing `tmp/p2g-0.2.4.tar.gz` & `tmp/p2g-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2g-0.2.4.tar", max compression
+gzip compressed data, was "p2g-0.2.5.tar", max compression
```

## Comparing `p2g-0.2.4.tar` & `p2g-0.2.5.tar`

### file list

```diff
@@ -1,89 +1,85 @@
--rwxr-xr-x   0        0        0    41960 2023-06-13 04:28:58.639884 p2g-0.2.4/README.rst
--rwxr-xr-x   0        0        0     1078 2023-06-13 03:58:16.432322 p2g-0.2.4/p2g/__init__.py
--rwxr-xr-x   0        0        0       24 2023-06-13 03:37:27.633461 p2g-0.2.4/p2g/__main__.py
--rwxr-xr-x   0        0        0      688 2023-06-08 02:10:38.312650 p2g-0.2.4/p2g/axis.py
--rwxr-xr-x   0        0        0     1215 2023-06-13 03:37:27.589460 p2g-0.2.4/p2g/builtin.py
--rwxr-xr-x   0        0        0     3357 2023-06-13 04:18:14.162025 p2g-0.2.4/p2g/coords.py
--rw-r--r--   0        0        0     3963 2023-06-13 03:37:28.537481 p2g-0.2.4/p2g/debug.py
--rwxr-xr-x   0        0        0       16 2023-06-05 01:20:09.252416 p2g-0.2.4/p2g/doc/authors.org
--rwxr-xr-x   0        0        0       47 2023-06-05 01:20:09.252416 p2g-0.2.4/p2g/doc/authors.rst
--rw-r--r--   0        0        0     9227 2023-06-13 04:28:57.267854 p2g-0.2.4/p2g/doc/haas.md
--rwxr-xr-x   0        0        0     6302 2023-06-13 04:28:57.231854 p2g-0.2.4/p2g/doc/haas.org
--rwxr-xr-x   0        0        0    16404 2023-06-13 04:28:58.159874 p2g-0.2.4/p2g/doc/haas.txt
--rwxr-xr-x   0        0        0    29769 2023-06-10 05:20:54.073592 p2g-0.2.4/p2g/doc/readme.org
--rwxr-xr-x   0        0        0    41960 2023-06-13 04:28:57.663863 p2g-0.2.4/p2g/doc/readme.rst
--rwxr-xr-x   0        0        0     2441 2023-06-11 01:42:10.740032 p2g-0.2.4/p2g/err.py
--rwxr-xr-x   0        0        0     2835 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/examples/csearch.py
--rwxr-xr-x   0        0        0     2647 2023-06-10 05:25:02.918724 p2g-0.2.4/p2g/examples/defs.py
--rwxr-xr-x   0        0        0     1818 2023-06-10 05:25:06.598800 p2g-0.2.4/p2g/examples/probecalibrate.nc
--rwxr-xr-x   0        0        0     1216 2023-06-10 05:23:24.444693 p2g-0.2.4/p2g/examples/probecalibrate.py
--rwxr-xr-x   0        0        0    10188 2023-06-13 03:37:37.101665 p2g-0.2.4/p2g/examples/vicecenter.nc
--rwxr-xr-x   0        0        0     3891 2023-06-13 03:37:27.689463 p2g-0.2.4/p2g/examples/vicecenter.py
--rwxr-xr-x   0        0        0     1191 2023-06-13 03:38:18.678560 p2g-0.2.4/p2g/gbl.py
--rwxr-xr-x   0        0        0     4120 2023-06-11 03:01:33.696699 p2g-0.2.4/p2g/goto.py
--rw-r--r--   0        0        0     6953 2023-06-13 04:28:58.619884 p2g-0.2.4/p2g/haas.py
--rwxr-xr-x   0        0        0     3014 2023-06-13 03:38:50.239240 p2g-0.2.4/p2g/lib.py
--rwxr-xr-x   0        0        0     6095 2023-06-13 03:38:37.190959 p2g-0.2.4/p2g/main.py
--rw-r--r--   0        0        0    16970 2023-06-13 03:52:58.621503 p2g-0.2.4/p2g/makestdvars.md
--rwxr-xr-x   0        0        0    15803 2023-06-13 04:00:30.279193 p2g-0.2.4/p2g/makestdvars.py
--rwxr-xr-x   0        0        0    21488 2023-06-04 23:59:54.699683 p2g-0.2.4/p2g/mvarsorig
--rwxr-xr-x   0        0        0     1306 2023-06-11 09:26:10.489507 p2g-0.2.4/p2g/nd.py
--rwxr-xr-x   0        0        0    13402 2023-06-13 04:18:13.418009 p2g-0.2.4/p2g/op.py
--rwxr-xr-x   0        0        0      594 2023-06-13 03:58:16.432322 p2g-0.2.4/p2g/opinfo.py
--rwxr-xr-x   0        0        0     7076 2023-06-13 04:04:35.060445 p2g-0.2.4/p2g/ptest.py
--rwxr-xr-x   0        0        0     3111 2023-06-13 03:47:37.522590 p2g-0.2.4/p2g/scalar.py
--rwxr-xr-x   0        0        0     6838 2023-06-11 09:51:31.324668 p2g-0.2.4/p2g/stat.py
--rwxr-xr-x   0        0        0     2749 2023-06-13 03:37:27.593461 p2g-0.2.4/p2g/symbol.py
--rwxr-xr-x   0        0        0      194 2023-06-11 08:10:56.218160 p2g-0.2.4/p2g/tests/conftest.py
--rwxr-xr-x   0        0        0       24 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/dummy.py
--rw-r--r--   0        0        0     1569 2023-06-13 03:08:44.076383 p2g-0.2.4/p2g/tests/golden/probecalibrate.gold
--rw-r--r--   0        0        0     1569 2023-06-13 03:19:05.773743 p2g-0.2.4/p2g/tests/golden/probecalibrate.nc
--rw-r--r--   0        0        0     1569 2023-06-11 07:56:49.609064 p2g-0.2.4/p2g/tests/golden/probecalibrate_probecalibrate.nc
--rw-r--r--   0        0        0      161 2023-06-13 04:21:46.010573 p2g-0.2.4/p2g/tests/golden/test_forcefail.decorator
--rw-r--r--   0        0        0      162 2023-06-13 03:34:51.586102 p2g-0.2.4/p2g/tests/golden/test_forcefail0.decorator
--rw-r--r--   0        0        0       65 2023-06-13 03:19:05.713742 p2g-0.2.4/p2g/tests/golden/test_forcefail0.nc
--rw-r--r--   0        0        0     8926 2023-06-13 03:08:44.072383 p2g-0.2.4/p2g/tests/golden/vicecenter.gold
--rw-r--r--   0        0        0     8926 2023-06-13 03:19:05.769744 p2g-0.2.4/p2g/tests/golden/vicecenter.nc
--rw-r--r--   0        0        0     8926 2023-06-11 07:55:26.775391 p2g-0.2.4/p2g/tests/golden/vicecenter_vicecenter.nc
--rwxr-xr-x   0        0        0      277 2023-06-11 08:04:20.418171 p2g-0.2.4/p2g/tests/not_pytest_nonlocal0.py
--rw-r--r--   0        0        0       83 2023-06-11 08:03:18.916929 p2g-0.2.4/p2g/tests/not_pytest_nonlocal1.py
--rwxr-xr-x   0        0        0      277 2023-06-11 08:06:00.940202 p2g-0.2.4/p2g/tests/not_pytest_nonlocal2.py
--rw-r--r--   0        0        0      126 2023-06-11 08:01:52.419181 p2g-0.2.4/p2g/tests/not_pytest_return.py
--rwxr-xr-x   0        0        0     2456 2023-06-07 08:07:43.325712 p2g-0.2.4/p2g/tests/test_axes.py
--rwxr-xr-x   0        0        0      535 2023-06-08 00:39:20.635661 p2g-0.2.4/p2g/tests/test_basic.py
--rwxr-xr-x   0        0        0     6290 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_builtins.py
--rwxr-xr-x   0        0        0      331 2023-06-05 23:45:53.213891 p2g-0.2.4/p2g/tests/test_comment.py
--rwxr-xr-x   0        0        0     4071 2023-06-11 02:39:41.033010 p2g-0.2.4/p2g/tests/test_coords.py
--rw-r--r--   0        0        0       82 2023-06-13 02:47:29.877021 p2g-0.2.4/p2g/tests/test_debug.py
--rwxr-xr-x   0        0        0      419 2023-06-07 07:49:26.319342 p2g-0.2.4/p2g/tests/test_edge.py
--rwxr-xr-x   0        0        0     3045 2023-06-13 03:35:49.179342 p2g-0.2.4/p2g/tests/test_error.py
--rw-r--r--   0        0        0      548 2023-06-11 08:15:36.207808 p2g-0.2.4/p2g/tests/test_example.py
--rwxr-xr-x   0        0        0      769 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_expr.py
--rwxr-xr-x   0        0        0     2264 2023-06-11 03:11:56.361765 p2g-0.2.4/p2g/tests/test_for.py
--rwxr-xr-x   0        0        0     4754 2023-06-11 02:38:28.743482 p2g-0.2.4/p2g/tests/test_func.py
--rwxr-xr-x   0        0        0     1830 2023-06-11 02:38:49.195914 p2g-0.2.4/p2g/tests/test_goto.py
--rwxr-xr-x   0        0        0       48 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_gvar.py
--rwxr-xr-x   0        0        0     6413 2023-06-11 02:42:12.864218 p2g-0.2.4/p2g/tests/test_interp.py
--rwxr-xr-x   0        0        0      534 2023-06-11 02:40:28.086004 p2g-0.2.4/p2g/tests/test_linenos.py
--rwxr-xr-x   0        0        0     3569 2023-06-13 03:30:38.956664 p2g-0.2.4/p2g/tests/test_main.py
--rwxr-xr-x   0        0        0      556 2023-06-13 03:58:16.456322 p2g-0.2.4/p2g/tests/test_makestdvars.py
--rwxr-xr-x   0        0        0     2231 2023-06-13 03:37:27.653462 p2g-0.2.4/p2g/tests/test_meta.py
--rwxr-xr-x   0        0        0     1289 2023-06-07 08:17:30.717304 p2g-0.2.4/p2g/tests/test_nt1.py
--rwxr-xr-x   0        0        0     6315 2023-06-08 02:07:07.816139 p2g-0.2.4/p2g/tests/test_op.py
--rwxr-xr-x   0        0        0     8609 2023-06-12 19:54:53.504132 p2g-0.2.4/p2g/tests/test_smoke.py
--rwxr-xr-x   0        0        0     1014 2023-06-08 04:07:45.087005 p2g-0.2.4/p2g/tests/test_str.py
--rw-r--r--   0        0        0     1686 2023-06-08 04:13:46.258640 p2g-0.2.4/p2g/tests/test_symtab.py
--rwxr-xr-x   0        0        0     1206 2023-06-11 01:45:23.472112 p2g-0.2.4/p2g/tests/test_tuple.py
--rwxr-xr-x   0        0        0     4230 2023-06-13 03:37:27.641462 p2g-0.2.4/p2g/tests/test_vars.py
--rwxr-xr-x   0        0        0     9120 2023-06-11 01:45:49.500663 p2g-0.2.4/p2g/tests/test_vector.py
--rwxr-xr-x   0        0        0     1310 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/thanksto
--rwxr-xr-x   0        0        0     6461 2023-06-13 04:12:42.282901 p2g-0.2.4/p2g/vector.py
--rwxr-xr-x   0        0        0       23 2023-06-13 04:22:41.803771 p2g-0.2.4/p2g/version.py
--rwxr-xr-x   0        0        0      783 2023-06-13 04:18:11.833975 p2g-0.2.4/p2g/visible.py
--rwxr-xr-x   0        0        0    11821 2023-06-13 04:19:27.959609 p2g-0.2.4/p2g/walk.py
--rwxr-xr-x   0        0        0     3034 2023-06-13 03:20:45.459889 p2g-0.2.4/p2g/walkbase.py
--rwxr-xr-x   0        0        0     4687 2023-06-13 01:26:50.508840 p2g-0.2.4/p2g/walkexpr.py
--rwxr-xr-x   0        0        0     6378 2023-06-13 03:20:45.367887 p2g-0.2.4/p2g/walkfunc.py
--rwxr-xr-x   0        0        0     3401 2023-06-13 04:21:31.062252 p2g-0.2.4/p2g/walkns.py
--rwxr-xr-x   0        0        0     3665 2023-06-13 04:22:41.539765 p2g-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    42930 1970-01-01 00:00:00.000000 p2g-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0    42500 2023-06-21 02:42:18.121336 p2g-0.2.5/README.rst
+-rwxr-xr-x   0        0        0     1102 2023-06-21 10:05:40.530052 p2g-0.2.5/p2g/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-06-21 08:48:22.577390 p2g-0.2.5/p2g/__main__.py
+-rwxr-xr-x   0        0        0      688 2023-06-19 00:17:28.273631 p2g-0.2.5/p2g/axis.py
+-rwxr-xr-x   0        0        0     1215 2023-06-18 04:43:38.122521 p2g-0.2.5/p2g/builtin.py
+-rwxr-xr-x   0        0        0     3357 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/coords.py
+-rw-r--r--   0        0        0     4090 2023-06-19 00:15:06.786854 p2g-0.2.5/p2g/debug.py
+-rwxr-xr-x   0        0        0       16 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/doc/authors.org
+-rw-r--r--   0        0        0      211 2023-06-21 09:53:44.939805 p2g-0.2.5/p2g/doc/buildreadme.el
+-rwxr-xr-x   0        0        0    12081 2023-06-21 10:21:12.452589 p2g-0.2.5/p2g/doc/haas.org
+-rwxr-xr-x   0        0        0    16060 2023-06-21 10:21:14.096622 p2g-0.2.5/p2g/doc/haas.txt
+-rw-r--r--   0        0        0     1075 2023-06-21 02:43:31.506820 p2g-0.2.5/p2g/doc/license.org
+-rw-r--r--   0        0        0    33656 2023-06-21 10:21:13.628613 p2g-0.2.5/p2g/doc/readme.md
+-rw-r--r--   0        0        0    33656 2023-06-21 10:21:13.648613 p2g-0.2.5/p2g/doc/readme.md.tmp
+-rw-r--r--   0        0        0    33894 2023-06-21 10:16:16.954707 p2g-0.2.5/p2g/doc/readme.md~
+-rwxr-xr-x   0        0        0    35449 2023-06-21 10:16:15.150672 p2g-0.2.5/p2g/doc/readme.org
+-rwxr-xr-x   0        0        0     2550 2023-06-18 23:16:44.374437 p2g-0.2.5/p2g/err.py
+-rwxr-xr-x   0        0        0     2732 2023-06-18 01:57:11.841792 p2g-0.2.5/p2g/examples/csearch.py
+-rwxr-xr-x   0        0        0     2764 2023-06-18 03:11:37.467828 p2g-0.2.5/p2g/examples/defs.py
+-rw-r--r--   0        0        0     1883 2023-06-18 04:54:07.607190 p2g-0.2.5/p2g/examples/probecalibrate.nc
+-rwxr-xr-x   0        0        0     1174 2023-06-18 04:06:55.402328 p2g-0.2.5/p2g/examples/probecalibrate.py
+-rw-r--r--   0        0        0    10558 2023-06-18 22:45:07.561957 p2g-0.2.5/p2g/examples/vicecenter.nc
+-rwxr-xr-x   0        0        0     3942 2023-06-18 04:14:26.923355 p2g-0.2.5/p2g/examples/vicecenter.py
+-rwxr-xr-x   0        0        0     1191 2023-06-18 04:16:04.897315 p2g-0.2.5/p2g/gbl.py
+-rwxr-xr-x   0        0        0     5339 2023-06-18 04:17:41.923256 p2g-0.2.5/p2g/goto.py
+-rw-r--r--   0        0        0     6907 2023-06-21 10:21:14.492630 p2g-0.2.5/p2g/haas.py
+-rwxr-xr-x   0        0        0     3464 2023-06-21 10:05:40.530052 p2g-0.2.5/p2g/lib.py
+-rwxr-xr-x   0        0        0     5598 2023-06-21 10:05:26.129765 p2g-0.2.5/p2g/main.py
+-rwxr-xr-x   0        0        0    15809 2023-06-21 10:04:57.421194 p2g-0.2.5/p2g/makestdvars.py
+-rwxr-xr-x   0        0        0    21488 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/mvarsorig
+-rwxr-xr-x   0        0        0     1768 2023-06-18 04:50:09.654391 p2g-0.2.5/p2g/nd.py
+-rwxr-xr-x   0        0        0    13462 2023-06-18 04:18:48.592590 p2g-0.2.5/p2g/op.py
+-rwxr-xr-x   0        0        0      593 2023-06-21 10:05:40.562052 p2g-0.2.5/p2g/opinfo.py
+-rwxr-xr-x   0        0        0     6991 2023-06-19 00:15:06.766853 p2g-0.2.5/p2g/ptest.py
+-rwxr-xr-x   0        0        0     3056 2023-06-18 04:43:09.973955 p2g-0.2.5/p2g/scalar.py
+-rwxr-xr-x   0        0        0     7085 2023-06-19 00:15:06.754853 p2g-0.2.5/p2g/stat.py
+-rwxr-xr-x   0        0        0     2749 2023-06-18 04:14:26.855354 p2g-0.2.5/p2g/symbol.py
+-rwxr-xr-x   0        0        0      194 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/conftest.py
+-rwxr-xr-x   0        0        0       24 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/dummy.py
+-rw-r--r--   0        0        0     1628 2023-06-18 04:10:24.966517 p2g-0.2.5/p2g/tests/golden/probecalibrate_probecalibrate.nc
+-rw-r--r--   0        0        0      161 2023-06-21 10:03:44.567744 p2g-0.2.5/p2g/tests/golden/test_error_test_forcefail.decorator
+-rw-r--r--   0        0        0        0 2023-06-21 10:03:45.071754 p2g-0.2.5/p2g/tests/golden/test_meta_test_native_gold_compare_fail.got
+-rw-r--r--   0        0        0     9366 2023-06-18 04:07:32.343066 p2g-0.2.5/p2g/tests/golden/vicecenter_vicecenter.nc
+-rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/not_pytest_nonlocal0.py
+-rw-r--r--   0        0        0       83 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/not_pytest_nonlocal1.py
+-rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.131593 p2g-0.2.5/p2g/tests/not_pytest_nonlocal2.py
+-rw-r--r--   0        0        0      126 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/not_pytest_return.py
+-rwxr-xr-x   0        0        0     2456 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/test_axes.py
+-rwxr-xr-x   0        0        0      535 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_basic.py
+-rwxr-xr-x   0        0        0     6290 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_builtins.py
+-rwxr-xr-x   0        0        0      331 2023-06-18 01:55:22.163594 p2g-0.2.5/p2g/tests/test_comment.py
+-rwxr-xr-x   0        0        0     4071 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_coords.py
+-rw-r--r--   0        0        0       73 2023-06-18 23:49:09.560268 p2g-0.2.5/p2g/tests/test_debug.py
+-rwxr-xr-x   0        0        0      419 2023-06-18 01:55:22.163594 p2g-0.2.5/p2g/tests/test_edge.py
+-rwxr-xr-x   0        0        0     2866 2023-06-18 03:38:38.920293 p2g-0.2.5/p2g/tests/test_error.py
+-rw-r--r--   0        0        0      550 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/test_example.py
+-rwxr-xr-x   0        0        0      769 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_expr.py
+-rwxr-xr-x   0        0        0     2264 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_for.py
+-rwxr-xr-x   0        0        0     4754 2023-06-18 01:55:22.131593 p2g-0.2.5/p2g/tests/test_func.py
+-rwxr-xr-x   0        0        0     3402 2023-06-18 03:03:46.166348 p2g-0.2.5/p2g/tests/test_goto.py
+-rwxr-xr-x   0        0        0       48 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_gvar.py
+-rwxr-xr-x   0        0        0     6728 2023-06-18 04:13:07.893775 p2g-0.2.5/p2g/tests/test_interp.py
+-rwxr-xr-x   0        0        0      534 2023-06-18 01:55:22.139593 p2g-0.2.5/p2g/tests/test_linenos.py
+-rwxr-xr-x   0        0        0     3690 2023-06-19 00:39:08.547261 p2g-0.2.5/p2g/tests/test_main.py
+-rwxr-xr-x   0        0        0      556 2023-06-18 04:50:12.862456 p2g-0.2.5/p2g/tests/test_makestdvars.py
+-rwxr-xr-x   0        0        0     2562 2023-06-18 03:40:10.694133 p2g-0.2.5/p2g/tests/test_meta.py
+-rwxr-xr-x   0        0        0     1289 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_nt1.py
+-rwxr-xr-x   0        0        0     6315 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_op.py
+-rwxr-xr-x   0        0        0     8609 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/test_smoke.py
+-rwxr-xr-x   0        0        0     1014 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_str.py
+-rw-r--r--   0        0        0     1686 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_symtab.py
+-rwxr-xr-x   0        0        0     1206 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/test_tuple.py
+-rwxr-xr-x   0        0        0     4230 2023-06-18 22:48:54.014313 p2g-0.2.5/p2g/tests/test_vars.py
+-rwxr-xr-x   0        0        0     9120 2023-06-18 02:46:24.501230 p2g-0.2.5/p2g/tests/test_vector.py
+-rwxr-xr-x   0        0        0     1310 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/thanksto
+-rwxr-xr-x   0        0        0     6466 2023-06-18 04:36:41.638150 p2g-0.2.5/p2g/vector.py
+-rwxr-xr-x   0        0        0       22 2023-06-21 10:22:06.489669 p2g-0.2.5/p2g/version.py
+-rwxr-xr-x   0        0        0      787 2023-06-18 04:18:25.980138 p2g-0.2.5/p2g/visible.py
+-rwxr-xr-x   0        0        0    11859 2023-06-21 10:05:40.554052 p2g-0.2.5/p2g/walk.py
+-rwxr-xr-x   0        0        0     3034 2023-06-18 01:57:12.521805 p2g-0.2.5/p2g/walkbase.py
+-rwxr-xr-x   0        0        0     4687 2023-06-18 04:03:52.582675 p2g-0.2.5/p2g/walkexpr.py
+-rwxr-xr-x   0        0        0     6373 2023-06-19 00:36:16.907866 p2g-0.2.5/p2g/walkfunc.py
+-rwxr-xr-x   0        0        0     3427 2023-06-18 04:29:57.618030 p2g-0.2.5/p2g/walkns.py
+-rwxr-xr-x   0        0        0     3898 2023-06-21 10:22:06.229664 p2g-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    43392 1970-01-01 00:00:00.000000 p2g-0.2.5/PKG-INFO
```

### Comparing `p2g-0.2.4/README.rst` & `p2g-0.2.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+=======================
+p2g - Python to G-Code.
+=======================
+
     :Author: sac
 
 .. contents::
 
+`https://travis-ci.org/kaushalmodi/ox-hugo.svg?branch=master <https://travis-ci.org/kaushalmodi/ox-hugo>`_ .. image:: file:https://melpa.org/packages/ox-hugo-badge.svg
+    :target: https://melpa.org/#/ox-hugo .. image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+    :target: https://www.gnu.org/licenses/gpl-3.0
+
 1 p2g - Python 2 G-code
 -----------------------
 
 Many styli died to bring us this information.
 
 This is a Python to G-code transplier
 
@@ -48,20 +56,20 @@
 yields 
 
 ::
 
       O0001                           ( TST                           )
       #100= 9.                        (   x = Var[9]                  )
       #102= 0.                        (   for y in range[10]:         )
-    L2000
+    N2000
       IF [#102 GE 10.] GOTO 2002
       #100= #100 + #102               ( x += y                        )
       #102= #102 + 1.
       GOTO 2000
-    L2002
+    N2002
       M30
 
 3 A taste.
 ----------
 
 .. code:: python
     :name: demo1
@@ -94,59 +102,60 @@
             # point, then done.
             if SKIP_POS.z < sch.search_depth + sch.iota:
                 break
             # otherwise move to next point
             cursor.xy += sch.delta
             its -= 1
         else:
-            message(ALARM.var, f"too far {sch.name}.", code=101)
+            message(ALARM, f"too far {sch.name}.")
 
     def demo1():
         cursor = Var[3](2, 3, 4)
         # searching right, look down 0.4", move
         # 1.5" right if nothing hit.
         sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
         search(cursor, sch1)
 
 
 ⇨ ``p2g gen demo1.py`` ⇨
 
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( demo1                         )
       #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
       #101= 3.
       #102= 4.
       #103= 10.                       ( its = Var[sch.its]            )
-    L1000                             ( while its > 0:                )
-      IF [#103 LE 0.] GOTO 1002
+    N2000                             ( while its > 0:                )
+      IF [#103 LE 0.] GOTO 2002
       G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
       G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
-      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
+      IF [#5063 LT -0.5] GOTO 2001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
       #100= #100 + 1.5                (     cursor.xy += sch.delta    )
       #103= #103 - 1.                 (     its -= 1                  )
-      GOTO 1000
-    L1002
-      #3000= 101.                     ( too far right.                )
-    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
+      GOTO 2000
+    N2002
+      (# 3000) = 101 (too far right.)
+    N2001                             (     message[ALARM, f"too far {sch.name}."])
       M30
 
 4 Coordinates
 -------------
 
 Describe position, with axis by location, in sequence or by name.
 
 .. code:: python
     :name: co1
 
     from p2g import *       # this is the common header
     from p2g.haas import *  # to all the examples
 
     def co1():
+        axis.NAMES="xyza*c"
         com ("Coords by order.")
         p1 = Fixed[3](1, 2, 3, addr=100)
 
         com ("Coords by axis name.")
         p2 = Fixed[3](z=333, y=222, x=111, addr=200)
         p2.x = 17
 
@@ -162,15 +171,15 @@
         p4.a = 180
         p4.c = asin (0.5)
 
 ⇨ ``p2g gen co1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( co1                           )
     ( Coords by order. )
       #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
       #101= 2.
       #102= 3.
     ( Coords by axis name. )
       #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
       #201= 222.
@@ -210,15 +219,15 @@
 .. code:: python
     :name: var1
 
 
     from p2g import *   # this is the common header
     from p2g.haas import *
 
-    def ex2():
+    def var1():
         # On my machine, Renishaw skip positions are
         # in 5061, 5062, 5063.  Look in p2g.haas.py
         # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
         skip0 = SKIP_POS
 
         # can be done manualy too.
         skip1 = Fixed[3](addr=5061)
@@ -227,32 +236,32 @@
         workpos = WORK_POS
 
 
         tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
 
 
         com("Define a constant ")
-        above_tdc = Const (111,222,333)
+        above_tdc = Const (111,222,1333)
 
         com("Use it ")
         tmp0 += above_tdc
 
 ⇨ ``p2g gen var1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( var1                          )
       #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
       #101= #5062 * 2. + #5042 + #5062
       #102= #5063 * 2. + #5043 + #5063
     ( Define a constant  )
     ( Use it  )
       #100= #100 + 111.               ( tmp0 += above_tdc             )
       #101= #101 + 222.
-      #102= #102 + 333.
+      #102= #102 + 1333.
       M30
 
 6 Expressions
 -------------
 
 Python expressions turn into G-Code as you may expect, save that
 native Python uses radians for trig, and G-Code uses degrees, so
@@ -261,15 +270,15 @@
 
 .. code:: python
     :name: exp1
 
     from p2g import *       # this is the common header
     from p2g.haas import *  # to all the examples
 
-    def exp11():
+    def exp1():
         com ("Variables go into macro variables.")
         theta = Var(0.3)
         angle = Var(sin(theta))
 
         com ("Constants don't exist in G-code.")
         thetak = Const(0.3)
         anglek = Var(sin(thetak))
@@ -292,15 +301,15 @@
         tlhc.xy = ((a - b + 3) / sin(x),
                    (a + b + 3) / cos(x))
 
 ⇨ ``p2g gen exp1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( exp1                          )
     ( Variables go into macro variables. )
       #100= 0.3                       ( theta = Var[0.3]              )
       #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
     ( Constants don't exist in G-code. )
       #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
     ( Lots of things are folded. )
       #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
@@ -365,33 +374,39 @@
        a5()
        a3()   
 
 ⇨ ``p2g gen axes.py`` ⇨
 
 ::
 
-    O0001                           ( -                             )
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #5244= 0.
-    #5245= 0.
-    #5246= 0.
-    #5242= #5242 + 3.               (    G55.var += tmp1            )
-    #5243= #5243 + 9.
-    #5246= #5246 + 30.
-    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
-    #5246= #5246 * 2.
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
-    #101= #5242 * 34.
-    #102= #5243 * 34.
-    M30
+      O0001                           ( axes                          )
+    ( rhs of vector ops get expanded as needed )
+      #5241= 0.                       (    G55.var = [0,1]            )
+      #5242= 1.
+      #5243= 0.
+      #5244= 1.
+      #5245= 0.
+      #5246= 1.
+    ( fill yz and c with some stuff )
+    ( Unmentioned axes values are assumed    )
+    ( to be 0, so adding them makes no code. )
+      #5242= #5242 + 3.               (    G55.var += tmp1            )
+      #5243= #5243 + 9.
+      #5246= #5246 + 30.
+
+      #5244= #5244 * 2.               (    G55.ac *= 2.0              )
+      #5246= #5246 * 2.
+    ( Filling to number of axes. )
+      #5241= 0.                       (    G55.var = [0]              )
+      #5242= 0.
+      #5243= 0.
+      #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
+      #101= #5242 * 34.
+      #102= #5243 * 34.
+      M30
 
 8 Printing
 ----------
 
 Turns Python f string prints into G-code DPRNT.  Make sure
 that your print string does not have any characters in it that
 your machine considers to be illegal in a DPRNT string.
@@ -410,42 +425,39 @@
       for q in range(10):
         dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
 
 ⇨ ``p2g gen exprnt.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( exprnt                        )
       #100= 2.                        (   x = Var[2]                  )
       #101= 27.                       (   y = Var[27]                 )
       #103= 0.                        (   for q in range[10]:         )
-    L1000
-      IF [#103 GE 10.] GOTO 1002
-    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+    N2000
+      IF [#103 GE 10.] GOTO 2002
     DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
-      #103= #103 + 1.
-      GOTO 1000
-    L1002
+      #103= #103 + 1.                 ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+      GOTO 2000
+    N2002
       M30
 
 9 Symbol Tables.
 ----------------
 
 Set the global ``p2g.symbol.Table.print`` to get a symbol
 table in the output file.
 
 .. code:: python
     :name: stest
 
     import p2g
 
-
     x1 = -7
 
-
     MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
     MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
     MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
     RAW_ANALOG = p2g.Fixed[10](addr=1080)
     fish = 10
     not_used = 12
 
@@ -460,15 +472,15 @@
 ::
 
     ( RAW_ANALOG                              : #1080[10]               )
     ( v1                                      :  #106.x                 )
     ( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
     ( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
     ( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
-      O0001                           ( -                             )
+      O0001                           ( stest                         )
 
     ( Only used symbols are in output table. )
       #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
       #101= 8.
       #102= 9.
       #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
       #104= 180.
@@ -486,22 +498,25 @@
 
 modifier :
 
 - ``r9810``
   Use Renishaw macro 9810 to do a protected positioning cycle.
 
 - ``work``
-  Use current work coordinate system. - G90
+  Use current work coordinate system. - whatever set with set\ :sub:`wcs`\
 
 - ``machine``
-  Use the machine coordinate system - G90 G53
+  Use the machine coordinate system - G53
 
 - ``relative``
   Use relative coordinate system - G91
 
+- ``absolute``
+  Use absolute coordinate system - G90
+
 - ``z_then_xy``
   move Z axis first.
 
 - ``xy_then_z``
   move the other axes before the Z.
 
 - ``probe``
@@ -568,52 +583,52 @@
 ::
 
     ( v1        :  #100.x  #101.y  #102.z )
     ( absslow   : 10 machine xyz          )
     ( g1        : 20 work xyz             )
     ( p1        : 100 machine xyz         )
     ( p2        : 100 machine xyz probe   )
-    ( p3        : 100 relative xyz probe  )
     ( safe_goto : 20 r9810 xyz            )
-      O0001                           ( -                             )
+      O0001                           ( goto1                         )
 
     ( in work cosys, goto x=1, y=2, z=3 at 20ips )
       G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
 
     ( make a variable, 2,3,4 )
       #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
       #101= 3.
       #102= 4.
 
     ( In the machine cosys, move to v1.z then v1.xy, slowly )
-      G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
-      G01 G90 G53 F10. x#100 y#101
+      G01 G53 G90 F10. z#102          ( absslow.z_then_xy[v1]         )
+      G01 G53 G90 F10. x#100 y#101
 
     ( p1 is whatever absslow was, with feed adjusted to 100. )
-      G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
-      G01 G90 G53 F100. z#102
+      G01 G53 G90 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+      G01 G53 G90 F100. z#102
 
     ( p2 is whatever p1 was, with changed to a probe. )
     ( p2.xy_then_z[v1]              )
-      G01 G90 G53 G31 F100. x#100 y#101
-      G01 G90 G53 G31 F100. z#102
+      G01 G53 G90 G31 F100. x#100 y#101
+      G01 G53 G90 G31 F100. z#102
 
     ( p3 is whatever p1 was, with a probe and relative, )
     ( using only the x and y axes                       )
-      G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+    ( p3.xy_then_z[v1.xy]           )
+      G01 G53 G91 G31 F100. x#100 y#101
 
     ( move a and c axes  )
       G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
 
     ( probe with a hass MUST_SKIP mcode. )
       G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
 
     ( Define shortcut for safe_goto and use. )
-      G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
-      G01 G65 R9810 F20. x1. y2.
+      G65 R9810 F20. z3.              ( safe_goto.z_then_xy[1,2,3]    )
+      G65 R9810 F20. x1. y2.
       M30
 
 11 Notes.
 ---------
 
 The entire thing is brittle; I've only used it to make code
 for my own limited purposes. 
@@ -640,15 +655,15 @@
           p = X(12,34)
 
           p.adjust(TOOL_OFFSET)
           tmp = Var(p.a, p.b)
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( cool                          )
     ( You can do surprising things. )
       #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
       #101= #5082 + 34.
       M30
 
 
 
@@ -680,69 +695,66 @@
 
         G56.var = [1, 1, 1]
         G56.xyz = [2, 2, 2]
         G56[:] = [3, 3, 3]
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( beware                        )
     ( Names on the left hand side of an assignment need to be )
     ( treated with care.  A simple.                           )
     ( Will not do what you want - this will overwrite the definition )
     ( of G55 above - so no code will be generated.                   )
     ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
       #5261= 1.                       ( G56.var = [1, 1, 1]           )
       #5262= 1.
       #5263= 1.
       #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
       #5262= 2.
       #5263= 2.
       #5261= 3.                       ( G56[:] = [3, 3, 3]            )
       #5262= 3.
       #5263= 3.
+      M30
 
 .. code:: python
 
     from p2g import *
     from p2g.haas import *
     def beware1():
        com ("It's easy to forget that only macro variables will get into",
-          "the output code. Generated ifs with a constant are a give away:")
+          "the output code. Other code will go away.")
        x = 123
-       y = Var()
+       y = Var(7)
        if x==23 :  # look here
          y = 9
 
        com ("Should look like:")
        x = Var(123)
        y = Var()
        if x==23 :  # look here
          y = 9
        else:
          y = 99
 
 ::
 
-      O0001                           ( -                             )
-    ( It's easy to forget that only macro variables will get into     )
-    ( the output code. Generated ifs with a constant are a give away: )
-      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1001
-    L1000
-    L1001
+      O0001                           ( beware1                       )
+    ( It's easy to forget that only macro variables will get into )
+    ( the output code. Other code will go away.                   )
+      #100= 7.                        (    y = Var[7]                 )
     ( Should look like: )
       #101= 123.                      (    x = Var[123]               )
       #100= #102                      (    y = Var[]                  )
-      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
+      IF [#101 NE 23.] GOTO 2002      (    if x==23 :  # look here    )
       #100= 9.                        (  y = 9                        )
-      GOTO 1003
-    L1002
+      GOTO 2003
+    N2002
       #100= 99.                       (  y = 99                       )
-    L1003
+    N2003
       M30
 
 12 HAAS macro var definitions
 -----------------------------
 
 Names predefined in p2g.haas:
 
@@ -1047,10 +1059,7 @@
 -------
 
 Waiting for a replacement stylus **and** tool setter to arrive, I
 wondered if were possible to replace the hundreds of inscrutible lines
 of Hass WIPS Renishaw G-code with just a few lines of Python?
 
 Maybe.
-
-
->>
```

### Comparing `p2g-0.2.4/p2g/__init__.py` & `p2g-0.2.5/p2g/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 from .main import main
 from .ptest import check_golden
 from .ptest import check_golden_nodec
 from .ptest import must_be
 from .ptest import must_be_cc
 from .scalar import Scalar
 from .stat import code
+from .stat import codenl
 from .stat import com
 from .stat import comment
 from .stat import dprint
 from .symbol import Table
 from .vector import RValueVec
 from .vector import Vec
-
 # ruff: noqa: F401
 # noqa: F401
 from .version import __version__
 from .visible import address
 from .visible import alias
 from .visible import as_address
 from .visible import base_addr
```

### Comparing `p2g-0.2.4/p2g/axis.py` & `p2g-0.2.5/p2g/axis.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/builtin.py` & `p2g-0.2.5/p2g/builtin.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/coords.py` & `p2g-0.2.5/p2g/coords.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/debug.py` & `p2g-0.2.5/p2g/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #! /usr/bin/env python
 import contextlib
 import pathlib
 import sys
 import tempfile
 import typing
 
-from loguru import logger
-
 from p2g import err
 from p2g import gbl
 from p2g import lib
 from p2g import stat
 from p2g import walk
 
 
@@ -22,15 +20,15 @@
     return (pathlib.Path(__file__).parent / "tests" / module_name).with_suffix(".py")
 
 
 # testing can start app recursivly, clean up sys.argv
 def run_one_test(module_name, fname, args):
     prev_argv = sys.argv
     sys.argv = []
-    logger.info(f"starting test {fname}")
+    lib.log(f"starting test {fname}")
     if "native" in fname:
         inside = __import__(f"p2g.tests.{module_name}")
         fndef = getattr(getattr(inside.tests, module_name), fname)
         res = fndef(*args)
     else:
         res = walk.compile2g(
             func_name_arg=fname,
@@ -68,30 +66,37 @@
         return
     with tempfile.TemporaryDirectory() as tdir:
         dirpath = pathlib.Path(tdir)
         test_callee_arg.append(dirpath)
         yield
 
 
+@contextlib.contextmanager
+def savebp(catch_bp_early):
+    prev = gbl.config.bp_on_error
+    gbl.config.bp_on_error = catch_bp_early
+    yield
+    gbl.config.bp_on_error = prev
+
+
 def wrap_one_test(module_name, fname):
+    goingtofail = "forcefail" in fname or "cerror" in fname
+
     try:
         args: list[typing.Any] = []
         with capwrap(fname, args):
             with tmpwrap(fname, args):
-                run_one_test(module_name, fname, args)
+                with savebp(not goingtofail):
+                    run_one_test(module_name, fname, args)
 
     except (AssertionError, TypeError):
         return "cerror" in fname
 
     except err.CompilerError as ass:  # no cover
-        if "forcefail" in fname:
-            return True
-
-        # if all goes well, then this is never reached.
-        if "cerror" in fname:
+        if goingtofail:
             return True
         print(ass.report_error())
         return False
 
     return True
 
 
@@ -104,28 +109,29 @@
             yield func_name
 
 
 def run_all_test_(module_name):
     with stat.Nest():
         funcs = find_all_tests(module_name)
         for key in funcs:
-            lib.qprint("run", module_name, key)
+            lib.log("run", module_name, key)
+
             if not wrap_one_test(module_name, key):  # for debug
-                if gbl.opts["--break-on-error"]:
-                    breakpoint()
+                breakpoint()
+                wrap_one_test(module_name, key)
 
 
 def runthem():
     tnames = [
-        #        "test_meta", cant
+        "test_vars",
+        #        "test_meta",
         "not_pytest_nonlocal0",
         "not_pytest_nonlocal1",
         "not_pytest_nonlocal2",
         "not_pytest_return",
-        "test_vars",
         "test_tuple",
         "test_vector",
         "test_for",
         "test_makestdvars",
         "test_main",  # contains capfd stuff
         "test_op",
         "test_func",
```

### Comparing `p2g-0.2.4/p2g/doc/haas.txt` & `p2g-0.2.5/p2g/doc/haas.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,19 @@
 │  # 4001 … # 4021 │    21 │  V │  Float  │ LAST_BLOCK_G              │
 │  # 4022 … # 4100 │    79 │  _ │         │ -                         │
 │  # 4101 … # 4126 │    26 │  V │  Float  │ LAST_BLOCK_ADDRESS        │
 │  # 4127 … # 5000 │   874 │  _ │         │ -                         │
 │          # 5001… │ NAXES │  m │  Float  │ LAST_TARGET_POS           │
 │          # 5021… │ NAXES │  m │  Float  │ MACHINE_POS               │
 │          # 5021… │ NAXES │  A │         │  also MACHINE             │
-│          # 5021… │ NAXES │  A │         │  also MACHINE             │
-│          # 5021… │ NAXES │  A │         │  also G53                 │
 │          # 5021… │ NAXES │  A │         │  also G53                 │
 │          # 5041… │ NAXES │  m │  Float  │ WORK_POS                  │
 │          # 5041… │ NAXES │  A │         │  also WORK                │
-│          # 5041… │ NAXES │  A │         │  also WORK                │
 │          # 5061… │ NAXES │  m │  Float  │ SKIP_POS                  │
 │          # 5061… │ NAXES │  A │         │  also PROBE               │
-│          # 5061… │ NAXES │  A │         │  also PROBE               │
 │  # 5081 … # 5100 │    20 │  V │  Float  │ TOOL_OFFSET               │
 │  # 5101 … # 5200 │   100 │  _ │         │ -                         │
 │          # 5201… │ NAXES │  W │  Float  │ G52                       │
 │          # 5221… │ NAXES │  W │  Float  │ G54                       │
 │          # 5241… │ NAXES │  W │  Float  │ G55                       │
 │          # 5261… │ NAXES │  W │  Float  │ G56                       │
 │          # 5281… │ NAXES │  W │  Float  │ G57                       │
```

### Comparing `p2g-0.2.4/p2g/doc/readme.rst` & `p2g-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,44 @@
+Metadata-Version: 2.1
+Name: p2g
+Version: 0.2.5
+Summary: Transpile python into cnc gcode.
+Home-page: https://github.com/0x5ac/p2g
+License: MIT
+Keywords: cnc,gcode,mill,haas
+Author: sac
+Author-email: sac@0x5ac.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Compilers
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: typeguard (>=3.0.2,<4.0.0)
+Project-URL: Repository, https://github.com/0x5ac/p2g
+Description-Content-Type: text/x-rst
+
+=======================
+p2g - Python to G-Code.
+=======================
+
     :Author: sac
 
 .. contents::
 
+`https://travis-ci.org/kaushalmodi/ox-hugo.svg?branch=master <https://travis-ci.org/kaushalmodi/ox-hugo>`_ .. image:: file:https://melpa.org/packages/ox-hugo-badge.svg
+    :target: https://melpa.org/#/ox-hugo .. image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+    :target: https://www.gnu.org/licenses/gpl-3.0
+
 1 p2g - Python 2 G-code
 -----------------------
 
 Many styli died to bring us this information.
 
 This is a Python to G-code transplier
 
@@ -48,20 +81,20 @@
 yields 
 
 ::
 
       O0001                           ( TST                           )
       #100= 9.                        (   x = Var[9]                  )
       #102= 0.                        (   for y in range[10]:         )
-    L2000
+    N2000
       IF [#102 GE 10.] GOTO 2002
       #100= #100 + #102               ( x += y                        )
       #102= #102 + 1.
       GOTO 2000
-    L2002
+    N2002
       M30
 
 3 A taste.
 ----------
 
 .. code:: python
     :name: demo1
@@ -94,59 +127,60 @@
             # point, then done.
             if SKIP_POS.z < sch.search_depth + sch.iota:
                 break
             # otherwise move to next point
             cursor.xy += sch.delta
             its -= 1
         else:
-            message(ALARM.var, f"too far {sch.name}.", code=101)
+            message(ALARM, f"too far {sch.name}.")
 
     def demo1():
         cursor = Var[3](2, 3, 4)
         # searching right, look down 0.4", move
         # 1.5" right if nothing hit.
         sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
         search(cursor, sch1)
 
 
 ⇨ ``p2g gen demo1.py`` ⇨
 
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( demo1                         )
       #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
       #101= 3.
       #102= 4.
       #103= 10.                       ( its = Var[sch.its]            )
-    L1000                             ( while its > 0:                )
-      IF [#103 LE 0.] GOTO 1002
+    N2000                             ( while its > 0:                )
+      IF [#103 LE 0.] GOTO 2002
       G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
       G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
-      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
+      IF [#5063 LT -0.5] GOTO 2001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
       #100= #100 + 1.5                (     cursor.xy += sch.delta    )
       #103= #103 - 1.                 (     its -= 1                  )
-      GOTO 1000
-    L1002
-      #3000= 101.                     ( too far right.                )
-    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
+      GOTO 2000
+    N2002
+      (# 3000) = 101 (too far right.)
+    N2001                             (     message[ALARM, f"too far {sch.name}."])
       M30
 
 4 Coordinates
 -------------
 
 Describe position, with axis by location, in sequence or by name.
 
 .. code:: python
     :name: co1
 
     from p2g import *       # this is the common header
     from p2g.haas import *  # to all the examples
 
     def co1():
+        axis.NAMES="xyza*c"
         com ("Coords by order.")
         p1 = Fixed[3](1, 2, 3, addr=100)
 
         com ("Coords by axis name.")
         p2 = Fixed[3](z=333, y=222, x=111, addr=200)
         p2.x = 17
 
@@ -162,15 +196,15 @@
         p4.a = 180
         p4.c = asin (0.5)
 
 ⇨ ``p2g gen co1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( co1                           )
     ( Coords by order. )
       #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
       #101= 2.
       #102= 3.
     ( Coords by axis name. )
       #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
       #201= 222.
@@ -210,15 +244,15 @@
 .. code:: python
     :name: var1
 
 
     from p2g import *   # this is the common header
     from p2g.haas import *
 
-    def ex2():
+    def var1():
         # On my machine, Renishaw skip positions are
         # in 5061, 5062, 5063.  Look in p2g.haas.py
         # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
         skip0 = SKIP_POS
 
         # can be done manualy too.
         skip1 = Fixed[3](addr=5061)
@@ -227,32 +261,32 @@
         workpos = WORK_POS
 
 
         tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
 
 
         com("Define a constant ")
-        above_tdc = Const (111,222,333)
+        above_tdc = Const (111,222,1333)
 
         com("Use it ")
         tmp0 += above_tdc
 
 ⇨ ``p2g gen var1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( var1                          )
       #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
       #101= #5062 * 2. + #5042 + #5062
       #102= #5063 * 2. + #5043 + #5063
     ( Define a constant  )
     ( Use it  )
       #100= #100 + 111.               ( tmp0 += above_tdc             )
       #101= #101 + 222.
-      #102= #102 + 333.
+      #102= #102 + 1333.
       M30
 
 6 Expressions
 -------------
 
 Python expressions turn into G-Code as you may expect, save that
 native Python uses radians for trig, and G-Code uses degrees, so
@@ -261,15 +295,15 @@
 
 .. code:: python
     :name: exp1
 
     from p2g import *       # this is the common header
     from p2g.haas import *  # to all the examples
 
-    def exp11():
+    def exp1():
         com ("Variables go into macro variables.")
         theta = Var(0.3)
         angle = Var(sin(theta))
 
         com ("Constants don't exist in G-code.")
         thetak = Const(0.3)
         anglek = Var(sin(thetak))
@@ -292,15 +326,15 @@
         tlhc.xy = ((a - b + 3) / sin(x),
                    (a + b + 3) / cos(x))
 
 ⇨ ``p2g gen exp1.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( exp1                          )
     ( Variables go into macro variables. )
       #100= 0.3                       ( theta = Var[0.3]              )
       #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
     ( Constants don't exist in G-code. )
       #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
     ( Lots of things are folded. )
       #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
@@ -365,33 +399,39 @@
        a5()
        a3()   
 
 ⇨ ``p2g gen axes.py`` ⇨
 
 ::
 
-    O0001                           ( -                             )
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #5244= 0.
-    #5245= 0.
-    #5246= 0.
-    #5242= #5242 + 3.               (    G55.var += tmp1            )
-    #5243= #5243 + 9.
-    #5246= #5246 + 30.
-    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
-    #5246= #5246 * 2.
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
-    #101= #5242 * 34.
-    #102= #5243 * 34.
-    M30
+      O0001                           ( axes                          )
+    ( rhs of vector ops get expanded as needed )
+      #5241= 0.                       (    G55.var = [0,1]            )
+      #5242= 1.
+      #5243= 0.
+      #5244= 1.
+      #5245= 0.
+      #5246= 1.
+    ( fill yz and c with some stuff )
+    ( Unmentioned axes values are assumed    )
+    ( to be 0, so adding them makes no code. )
+      #5242= #5242 + 3.               (    G55.var += tmp1            )
+      #5243= #5243 + 9.
+      #5246= #5246 + 30.
+
+      #5244= #5244 * 2.               (    G55.ac *= 2.0              )
+      #5246= #5246 * 2.
+    ( Filling to number of axes. )
+      #5241= 0.                       (    G55.var = [0]              )
+      #5242= 0.
+      #5243= 0.
+      #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
+      #101= #5242 * 34.
+      #102= #5243 * 34.
+      M30
 
 8 Printing
 ----------
 
 Turns Python f string prints into G-code DPRNT.  Make sure
 that your print string does not have any characters in it that
 your machine considers to be illegal in a DPRNT string.
@@ -410,42 +450,39 @@
       for q in range(10):
         dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
 
 ⇨ ``p2g gen exprnt.py`` ⇨
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( exprnt                        )
       #100= 2.                        (   x = Var[2]                  )
       #101= 27.                       (   y = Var[27]                 )
       #103= 0.                        (   for q in range[10]:         )
-    L1000
-      IF [#103 GE 10.] GOTO 1002
-    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+    N2000
+      IF [#103 GE 10.] GOTO 2002
     DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
-      #103= #103 + 1.
-      GOTO 1000
-    L1002
+      #103= #103 + 1.                 ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+      GOTO 2000
+    N2002
       M30
 
 9 Symbol Tables.
 ----------------
 
 Set the global ``p2g.symbol.Table.print`` to get a symbol
 table in the output file.
 
 .. code:: python
     :name: stest
 
     import p2g
 
-
     x1 = -7
 
-
     MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
     MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
     MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
     RAW_ANALOG = p2g.Fixed[10](addr=1080)
     fish = 10
     not_used = 12
 
@@ -460,15 +497,15 @@
 ::
 
     ( RAW_ANALOG                              : #1080[10]               )
     ( v1                                      :  #106.x                 )
     ( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
     ( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
     ( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
-      O0001                           ( -                             )
+      O0001                           ( stest                         )
 
     ( Only used symbols are in output table. )
       #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
       #101= 8.
       #102= 9.
       #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
       #104= 180.
@@ -486,22 +523,25 @@
 
 modifier :
 
 - ``r9810``
   Use Renishaw macro 9810 to do a protected positioning cycle.
 
 - ``work``
-  Use current work coordinate system. - G90
+  Use current work coordinate system. - whatever set with set\ :sub:`wcs`\
 
 - ``machine``
-  Use the machine coordinate system - G90 G53
+  Use the machine coordinate system - G53
 
 - ``relative``
   Use relative coordinate system - G91
 
+- ``absolute``
+  Use absolute coordinate system - G90
+
 - ``z_then_xy``
   move Z axis first.
 
 - ``xy_then_z``
   move the other axes before the Z.
 
 - ``probe``
@@ -568,52 +608,52 @@
 ::
 
     ( v1        :  #100.x  #101.y  #102.z )
     ( absslow   : 10 machine xyz          )
     ( g1        : 20 work xyz             )
     ( p1        : 100 machine xyz         )
     ( p2        : 100 machine xyz probe   )
-    ( p3        : 100 relative xyz probe  )
     ( safe_goto : 20 r9810 xyz            )
-      O0001                           ( -                             )
+      O0001                           ( goto1                         )
 
     ( in work cosys, goto x=1, y=2, z=3 at 20ips )
       G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
 
     ( make a variable, 2,3,4 )
       #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
       #101= 3.
       #102= 4.
 
     ( In the machine cosys, move to v1.z then v1.xy, slowly )
-      G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
-      G01 G90 G53 F10. x#100 y#101
+      G01 G53 G90 F10. z#102          ( absslow.z_then_xy[v1]         )
+      G01 G53 G90 F10. x#100 y#101
 
     ( p1 is whatever absslow was, with feed adjusted to 100. )
-      G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
-      G01 G90 G53 F100. z#102
+      G01 G53 G90 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+      G01 G53 G90 F100. z#102
 
     ( p2 is whatever p1 was, with changed to a probe. )
     ( p2.xy_then_z[v1]              )
-      G01 G90 G53 G31 F100. x#100 y#101
-      G01 G90 G53 G31 F100. z#102
+      G01 G53 G90 G31 F100. x#100 y#101
+      G01 G53 G90 G31 F100. z#102
 
     ( p3 is whatever p1 was, with a probe and relative, )
     ( using only the x and y axes                       )
-      G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+    ( p3.xy_then_z[v1.xy]           )
+      G01 G53 G91 G31 F100. x#100 y#101
 
     ( move a and c axes  )
       G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
 
     ( probe with a hass MUST_SKIP mcode. )
       G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
 
     ( Define shortcut for safe_goto and use. )
-      G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
-      G01 G65 R9810 F20. x1. y2.
+      G65 R9810 F20. z3.              ( safe_goto.z_then_xy[1,2,3]    )
+      G65 R9810 F20. x1. y2.
       M30
 
 11 Notes.
 ---------
 
 The entire thing is brittle; I've only used it to make code
 for my own limited purposes. 
@@ -640,15 +680,15 @@
           p = X(12,34)
 
           p.adjust(TOOL_OFFSET)
           tmp = Var(p.a, p.b)
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( cool                          )
     ( You can do surprising things. )
       #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
       #101= #5082 + 34.
       M30
 
 
 
@@ -680,69 +720,66 @@
 
         G56.var = [1, 1, 1]
         G56.xyz = [2, 2, 2]
         G56[:] = [3, 3, 3]
 
 ::
 
-      O0001                           ( -                             )
+      O0001                           ( beware                        )
     ( Names on the left hand side of an assignment need to be )
     ( treated with care.  A simple.                           )
     ( Will not do what you want - this will overwrite the definition )
     ( of G55 above - so no code will be generated.                   )
     ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
       #5261= 1.                       ( G56.var = [1, 1, 1]           )
       #5262= 1.
       #5263= 1.
       #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
       #5262= 2.
       #5263= 2.
       #5261= 3.                       ( G56[:] = [3, 3, 3]            )
       #5262= 3.
       #5263= 3.
+      M30
 
 .. code:: python
 
     from p2g import *
     from p2g.haas import *
     def beware1():
        com ("It's easy to forget that only macro variables will get into",
-          "the output code. Generated ifs with a constant are a give away:")
+          "the output code. Other code will go away.")
        x = 123
-       y = Var()
+       y = Var(7)
        if x==23 :  # look here
          y = 9
 
        com ("Should look like:")
        x = Var(123)
        y = Var()
        if x==23 :  # look here
          y = 9
        else:
          y = 99
 
 ::
 
-      O0001                           ( -                             )
-    ( It's easy to forget that only macro variables will get into     )
-    ( the output code. Generated ifs with a constant are a give away: )
-      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1001
-    L1000
-    L1001
+      O0001                           ( beware1                       )
+    ( It's easy to forget that only macro variables will get into )
+    ( the output code. Other code will go away.                   )
+      #100= 7.                        (    y = Var[7]                 )
     ( Should look like: )
       #101= 123.                      (    x = Var[123]               )
       #100= #102                      (    y = Var[]                  )
-      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
+      IF [#101 NE 23.] GOTO 2002      (    if x==23 :  # look here    )
       #100= 9.                        (  y = 9                        )
-      GOTO 1003
-    L1002
+      GOTO 2003
+    N2002
       #100= 99.                       (  y = 99                       )
-    L1003
+    N2003
       M30
 
 12 HAAS macro var definitions
 -----------------------------
 
 Names predefined in p2g.haas:
 
@@ -1048,9 +1085,7 @@
 
 Waiting for a replacement stylus **and** tool setter to arrive, I
 wondered if were possible to replace the hundreds of inscrutible lines
 of Hass WIPS Renishaw G-code with just a few lines of Python?
 
 Maybe.
 
-
->>
```

### Comparing `p2g-0.2.4/p2g/err.py` & `p2g-0.2.5/p2g/err.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,21 @@
 
 
 def mark_pos(last_pos):
     state.last_pos = last_pos
 
 
 def src_code_from_line_near(pos, lineno):
-    with lib.openr(pos.filename) as inf:
-        src = inf.read()
-        lines = lib.splitnl(src)
-        return lines[lineno - 1]
+    try:
+        with lib.openr(pos.filename) as inf:
+            src = lib.logread(inf)
+            lines = lib.splitnl(src)
+            return lines[lineno - 1]
+    except FileNotFoundError:
+        return "not found"
 
 
 def src_code_from_node_place(pos):
     return src_code_from_line_near(pos, pos.lineno)
 
 
 def note_from_node_place(pos, absolute_lines, topfn=None):
@@ -93,11 +96,12 @@
         for line in self.error_lines(absolute_lines, topfn):
             print(line, file=outf)
 
 
 def compiler(message, exc=None, err_pos=None) -> typing.NoReturn:
     if gbl.config.bp_on_error:  # for debug
         breakpoint()
+        breakpoint()
 
     if not err_pos:
         err_pos = state.last_pos
     raise CompilerError(err_pos, str(message)) from exc
```

### Comparing `p2g-0.2.4/p2g/examples/csearch.py` & `p2g-0.2.5/p2g/examples/csearch.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from typing import Optional
-
-import p2g as pg
-
-
-class SearchConstraint:
-    # position roughly center above start of search.
-    above: pg.Vec
-    # min size of thing to look for.
-
-    amin: pg.Vec
-    # max size to search in one dimension for the thing
-    # to probe.  pg.RVALnstains max size of things measured.
-    amax: pg.Vec
-
-    # when measuring z, how far to
-    # move from an xy edge inwards to work it out.
-    indent: pg.Vec
-
-    # steps between probes
-
-    delta: pg.Vec
-    # safe distance above probed z surface to move
-    skim_distance: pg.Vec
-
-    # how far to backoff before probing slowly
-    backoff: pg.Vec
-
-    # how far to look down for a surface once we've
-    # already located the rough z0
-    search_depth: pg.Vec
-    # how far to look down and not found is a not there
-    #
-    found_if_below: pg.Vec
-
-    # to work out when there's a probe hit,
-    # say probe from z down to 0,   then any stop < iota
-    # is taken as a miss.
-    iota: pg.Vec
-
-    def __init__(
-        self,
-        amin: pg.Vec,
-        amax: pg.Vec,
-        above: pg.Vec,
-        delta: pg.Vec,
-        skim_distance=None,
-        indent: Optional[pg.Vec] = None,
-        backoff: Optional[pg.Vec] = None,
-        search_depth=None,
-        found_if_below=None,
-        iota=None,
-    ):
-        super().__init__()
-
-        if search_depth is None:
-            search_depth = pg.Const(-0.1)
-
-        if found_if_below is None:
-            found_if_below = search_depth * 0.5
-
-        if backoff is None:
-            backoff = pg.Const(x=0.1, y=0.1, z=0.1)
-
-        if indent is None:
-            indent = round(amax * 0.1, 1)
-
-        if skim_distance is None:
-            skim_distance = pg.Const(0.3)
-
-        if iota is None:
-            iota = pg.Const(x=0.025, y=0.025, z=0.025)
-
-        self.iota = iota
-        self.delta = delta
-
-        self.amin = amin
-        self.indent = indent
-        self.amax = amax
-
-        self.above = above
-        self.skim_distance = skim_distance
-        self.backoff = backoff
-        self.search_depth = search_depth
-        self.found_if_below = found_if_below
-
-    @property
-    def comment(self):
-        return [
-            "Search Constraints:",
-            "start:",
-            f"  {self.above}",
-            "boundary:",
-            f"  x= (-{(self.amax[0] * 0.5)}..-{(self.amin[0] * 0.5)})"
-            f"..({(self.amin[0] * 0.5)}..{(self.amax[0] * 0.5)})",
-            f"  y= (-{(self.amax[1] * 0.5)}..-{(self.amin[1] * 0.5)})"
-            f"..({(self.amin[1] * 0.5)}..{(self.amax[1] * 0.5)})",
-            f"  z= ({(-self.amax[2])}..{(-self.amin[2])})",
-            "indent:",
-            f"  {self.indent}",
-            "delta:",
-            f"  {self.delta}",
-        ]
+from typing import Optional
+
+import p2g as pg
+
+
+class SearchConstraint:
+    # position roughly center above start of search.
+    above: pg.Vec
+    # min size of thing to look for.
+
+    amin: pg.Vec
+    # max size to search in one dimension for the thing
+    # to probe.  pg.RVALnstains max size of things measured.
+    amax: pg.Vec
+
+    # when measuring z, how far to
+    # move from an xy edge inwards to work it out.
+    indent: pg.Vec
+
+    # steps between probes
+
+    delta: pg.Vec
+    # safe distance above probed z surface to move
+    skim_distance: pg.Vec
+
+    # how far to backoff before probing slowly
+    backoff: pg.Vec
+
+    # how far to look down for a surface once we've
+    # already located the rough z0
+    search_depth: pg.Vec
+    # how far to look down and not found is a not there
+    #
+    found_if_below: pg.Vec
+
+    # to work out when there's a probe hit,
+    # say probe from z down to 0,   then any stop < iota
+    # is taken as a miss.
+    iota: pg.Vec
+
+    def __init__(
+        self,
+        amin: pg.Vec,
+        amax: pg.Vec,
+        above: pg.Vec,
+        delta: pg.Vec,
+        skim_distance=None,
+        indent: Optional[pg.Vec] = None,
+        backoff: Optional[pg.Vec] = None,
+        search_depth=None,
+        found_if_below=None,
+        iota=None,
+    ):
+        super().__init__()
+
+        if search_depth is None:
+            search_depth = pg.Const(-0.1)
+
+        if found_if_below is None:
+            found_if_below = search_depth * 0.5
+
+        if backoff is None:
+            backoff = pg.Const(x=0.1, y=0.1, z=0.1)
+
+        if indent is None:
+            indent = round(amax * 0.1, 1)
+
+        if skim_distance is None:
+            skim_distance = pg.Const(0.3)
+
+        if iota is None:
+            iota = pg.Const(x=0.025, y=0.025, z=0.025)
+
+        self.iota = iota
+        self.delta = delta
+
+        self.amin = amin
+        self.indent = indent
+        self.amax = amax
+
+        self.above = above
+        self.skim_distance = skim_distance
+        self.backoff = backoff
+        self.search_depth = search_depth
+        self.found_if_below = found_if_below
+
+    @property
+    def comment(self):
+        return [
+            "Search Constraints:",
+            "start:",
+            f"  {self.above}",
+            "boundary:",
+            f"  x= (-{(self.amax[0] * 0.5)}..-{(self.amin[0] * 0.5)})"
+            f"..({(self.amin[0] * 0.5)}..{(self.amax[0] * 0.5)})",
+            f"  y= (-{(self.amax[1] * 0.5)}..-{(self.amin[1] * 0.5)})"
+            f"..({(self.amin[1] * 0.5)}..{(self.amax[1] * 0.5)})",
+            f"  z= ({(-self.amax[2])}..{(-self.amin[2])})",
+            "indent:",
+            f"  {self.indent}",
+            "delta:",
+            f"  {self.delta}",
+        ]
```

### Comparing `p2g-0.2.4/p2g/examples/defs.py` & `p2g-0.2.5/p2g/examples/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 
 class Tool(enum.IntEnum):
     PROBE = 1
     KNOWN_LENGTH = 2
 
 
 # pylint: disable=too-many-instance-attributes
-class JobDefs(Table):
+class JobDefs:
     def __init__(self):
         super().__init__()
-        self.MACHINE_ABS_ABOVE_OTS = Const(x=-1.16, y=-7.5, z=-7.2)
-        # difference in length between fixed length probe and spindle probe.
-        self.MACHINE_ABS_ABOVE_OTS_FOR_PROBE = self.MACHINE_ABS_ABOVE_OTS + (
-            0,
-            0,
-            1,
-        )
-        self.MACHINE_ABS_ABOVE_RING = Const(x=-16.46, y=-3.5, z=-22.7)
+        self.MACHINE_ABS_ABOVE_OTS = Const(x=-1.16, y=-7.5, z=-7.5)
+
+        # ots tool and probe are different lengths.
+        self.MACHINE_ABS_PROBE_ABOVE_OTS = Const(x=-1.16, y=-7.5, z=-7.5)
+
+        self.MACHINE_ABS_PROBE_ABOVE_RING = Const(x=-16.46, y=-3.5, z=-22.7)
         self.MACHINE_ABS_ABOVE_ROTARY = Const(x=-12.5214, y=-12.9896, z=-7.0)
         self.MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = Const(x=-15.5, y=-17.50, z=-14.0)
         self.MACHINE_ABS_ABOVE_VICE = Const(x=-28.0, y=-10.0, z=-16.00)
-
+        self.MACHINE_ABS_CLOSE_ABOVE_OTS = Const(x=-1.16, y=-7.5, z=-7.6)
         self.MACHINE_ABS_CLOSE_ABOVE_TOOL_TOUCH = Const(
             x=-1.16,
             y=-7.5,
             z=-7.6,
         )
         self.MACHINE_ABS_HOME2 = Const(x=-15.0, y=-15.0, z=-2.0)
         self.MACHINE_ABS_ROTARY_HOME = Const(x=-12, y=0.0, z=-3.0)
@@ -53,43 +51,44 @@
         self.FAST_FEED = 65.0
         self.SLOW_PROBE_FEED = 10.0
         self.FAST_PROBE_FEED = 10.0
 
         probe = goto.probe.mcode(MUST_SKIP).work
         self.slow_probe = probe.feed(self.SLOW_PROBE_FEED)
 
-        self.fast_probe = probe.feed(self.FAST_PROBE_FEED)
+        self.fast_mabs_probe = probe.machine.absolute.feed(self.FAST_PROBE_FEED)
+        self.slow_mabs_probe = probe.machine.absolute.feed(self.SLOW_PROBE_FEED)
         self.goto = goto.work.feed(self.FAST_FEED)
 
     def load_tool(self, tool):
-        code(f"T{tool:02} M06")
+        codenl(f"T{tool:02} M06")
 
     def setup_probing(self):
         self.load_tool(Tool.PROBE)
 
-        code(PROBE_ON)
-        code(NO_LOOKAHEAD)
+        codenl(PROBE_ON)
+        codenl(NO_LOOKAHEAD)
 
     def pause(self, txt: str):
-        comment()
+        comment("")
         message(MESSAGE, txt)
-        comment()
+        comment("")
 
     def alarm(self, txt: str):
-        comment()
+        comment("")
         message(ALARM, txt)
-        comment()
+        comment("")
 
     def ots_on(self):
-        code(OTS_ON)
+        codenl(OTS_ON)
 
     def spindle_probe_on(self):
-        code(SPINDLE_PROBE_ON)
+        codenl(SPINDLE_PROBE_ON)
 
     def ots_calibrate(self):
-        code("G65 P9023 A20. K5. S0.5 D-2.")
+        codenl("G65 P9023 A20. K5. S0.5 D-2.")
 
     def spindle_probe_find_height(self):
-        code("G65 P9023 A21. T1.")
+        codenl("G65 P9023 A21. T1.")
 
     def spindle_probe_find_radius(self):
-        code("G65 P9023 A10.0 D0.7")
+        codenl("G65 P9023 A10.0 D0.7")
```

### Comparing `p2g-0.2.4/p2g/examples/probecalibrate.nc` & `p2g-0.2.5/p2g/tests/golden/probecalibrate_probecalibrate.nc`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,63 @@
-( MACHINE_ABS_ABOVE_OTS  :  -1.160, -7.500, -7.200 )
-( MACHINE_ABS_ABOVE_RING : -16.460, -3.500,-22.700 )
-  O0001                           ( PROBECALIBRATE                )
-
-( Calibrate from known length tool,       )
-( first macke sure OTS working, move tool )
-( to above setter, and runs calibrate     )
-( macro.                                  )
-  T02 M06                         ( st.load_tool[defs.Tool.KNOWN_LENGTH])
-  G65 P9855                       ( st.ots_on[]                   )
-  G103 P1
-  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
-
-  (# 3006) = 101 ( touch OTS, must beep )
-
-  G01 G90 G53 F65. x-1.16 y-7.5   ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS])
-  G01 G90 G53 F65. z-7.2
-  G65 P9023 A20. K5. S0.5 D-2.    ( st.ots_calibrate[]            )
-
-( Calibrate the spindle probe.            )
-( load spindle probe, makes sure the      )
-( battery isn't flat, checks it over the  )
-( tool setter, and then in the fixed ring )
-  T01 M06                         ( st.load_tool[defs.Tool.PROBE] )
-  G65                             ( st.spindle_probe_on[]         )
-  P9832
-
-  (# 3006) = 101 ( touch probe, must beep )
-
-
-( test spindle probe with OTS )
-  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
-  G01 G90 G53 F65. x-1.16 y-7.5   ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS_FOR_PROBE])
-  G01 G90 G53 F65. z-6.2
-  G65 P9023 A21. T1.              ( st.spindle_probe_find_height[])
+( MACHINE_ABS_ABOVE_OTS        :  -1.160, -7.500, -7.500 )
+( MACHINE_ABS_CLOSE_ABOVE_OTS  :  -1.160, -7.500, -7.600 )
+( MACHINE_ABS_PROBE_ABOVE_OTS  :  -1.160, -7.500, -7.500 )
+( MACHINE_ABS_PROBE_ABOVE_RING : -16.460, -3.500,-22.700 )
+
+( Start with fixed height probe,   )
+( make sure probe stickout <2.25in )
+(     st.load_tool[defs.Tool.KNOWN_LENGTH])
+  T02 M06
+(     st.ots_on[]               )
+  M59 P2
+  G04 P1.0
+  M59 P3
+(     st.goto.machine[z=0]      )
+  G01 G53 G90 F65. z0.
+
+
+  (# 3006) = 101 (touch OTS, must beep)
+
+
+(     st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS])
+  G01 G53 G90 F65. x-1.16 y-7.5
+  G01 G53 G90 F65. z-7.5
+
+
+  (# 3006) = 101 (Make sure tool position looks safe.)
+
+
+(     st.goto.machine[z=st.MACHINE_ABS_CLOSE_ABOVE_OTS.z])
+  G01 G53 G90 F65. z-7.6
+(     st.ots_calibrate[]        )
+  G65 P9023 A20. K5. S0.5 D-2.
+
+( Calibrate spindle probe. )
+(     st.load_tool[defs.Tool.PROBE])
+  T01 M06
+(     st.spindle_probe_on[]     )
+  G65 P9832
+
+
+  (# 3006) = 101 (touch probe, must beep)
+
+
+
+( test spindle probe with OTS. )
+(     st.goto.machine[z=0]      )
+  G01 G53 G90 F65. z0.
+(     st.goto.machine.xy_then_z[st.MACHINE_ABS_PROBE_ABOVE_OTS])
+  G01 G53 G90 F65. x-1.16 y-7.5
+  G01 G53 G90 F65. z-7.5
+(     st.spindle_probe_find_height[])
+  G65 P9023 A21. T1.
 
 ( test spindle probe with ring. )
-  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
-  G01 G90 G53 F65. x-16.46 y-3.5  ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_RING])
-  G01 G90 G53 F65. z-22.7
-  G65 P9023 A10.0 D0.7            ( st.spindle_probe_find_radius[])
-  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
-  M30
+(     st.goto.machine[z=0]      )
+  G01 G53 G90 F65. z0.
+(     st.goto.machine.xy_then_z[st.MACHINE_ABS_PROBE_ABOVE_RING])
+  G01 G53 G90 F65. x-16.46 y-3.5
+  G01 G53 G90 F65. z-22.7
+(     st.spindle_probe_find_radius[])
+  G65 P9023 A10.0 D0.7
+(     st.goto.machine[z=0]      )
+  G01 G53 G90 F65. z0.
```

### Comparing `p2g-0.2.4/p2g/examples/probecalibrate.py` & `p2g-0.2.5/p2g/examples/probecalibrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,53 +2,44 @@
 import sys
 
 import defs
 
 from p2g import *
 
 
-symbol.Table.print = 1
-
-
 def probecalibrate():
-    symbol.Table.print = 1
     st = defs.JobDefs()
-
-    comment(
-        "Calibrate from known length tool,",
-        "first macke sure OTS working, move tool",
-        "to above setter, and runs calibrate",
-        "macro.",
-    )
-
-    st.load_tool(defs.Tool.KNOWN_LENGTH)
-    st.ots_on()
-    st.goto.machine(z=0)
-    st.pause("touch OTS, must beep")
-
-    st.goto.machine.xy_then_z(st.MACHINE_ABS_ABOVE_OTS)
-    st.ots_calibrate()
-
-    comment(
-        "Calibrate the spindle probe.",
-        "load spindle probe, makes sure the",
-        "battery isn't flat, checks it over the ",
-        "tool setter, and then in the fixed ring",
-    )
-
-    st.load_tool(defs.Tool.PROBE)
-    st.spindle_probe_on()
-
-    st.pause("touch probe, must beep")
-
-    comment("test spindle probe with OTS")
-    st.goto.machine(z=0)
-
-    st.goto.machine.xy_then_z(st.MACHINE_ABS_ABOVE_OTS_FOR_PROBE)
-
-    st.spindle_probe_find_height()
-
-    comment("test spindle probe with ring.")
-    st.goto.machine(z=0)
-    st.goto.machine.xy_then_z(st.MACHINE_ABS_ABOVE_RING)
-    st.spindle_probe_find_radius()
-    st.goto.machine(z=0)
+    if 1:
+        comment(
+            "Start with fixed height probe,",
+            "make sure probe stickout <2.25in",
+        )
+
+        Table.print = 1
+        st.load_tool(defs.Tool.KNOWN_LENGTH)
+        st.ots_on()
+        st.goto.machine(z=0)
+        st.pause("touch OTS, must beep")
+        st.goto.machine.xy_then_z(st.MACHINE_ABS_ABOVE_OTS)
+
+        st.pause("Make sure tool position looks safe.")
+        st.goto.machine(z=st.MACHINE_ABS_CLOSE_ABOVE_OTS.z)
+        st.ots_calibrate()
+    if 1:
+        comment("Calibrate spindle probe.")
+
+        st.load_tool(defs.Tool.PROBE)
+        st.spindle_probe_on()
+
+        st.pause("touch probe, must beep")
+
+        comment("test spindle probe with OTS.")
+        st.goto.machine(z=0)
+        st.goto.machine.xy_then_z(st.MACHINE_ABS_PROBE_ABOVE_OTS)
+
+        st.spindle_probe_find_height()
+
+        comment("test spindle probe with ring.")
+        st.goto.machine(z=0)
+        st.goto.machine.xy_then_z(st.MACHINE_ABS_PROBE_ABOVE_RING)
+        st.spindle_probe_find_radius()
+        st.goto.machine(z=0)
```

### Comparing `p2g-0.2.4/p2g/examples/vicecenter.nc` & `p2g-0.2.5/p2g/examples/vicecenter.nc`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-( brc                    :  #102.x  #103.y          )
-( cursor                 :  #104.x  #105.y          )
-( error                  :  #106.x  #107.y          )
-( G55                    : #5241.x #5242.y #5243.z  )
-( its                    :  #106.x                  )
-( MACHINE_POS            : #5021.x #5022.y #5023.z  )
-( output                 :  #102.x  #103.y          )
-( output                 :  #100.x  #101.y          )
-( PROBE_R                :  #556.x  #557.y          )
-( SKIP_POS               : #5061.x #5062.y #5063.z  )
-( tlc                    :  #100.x  #101.y          )
-( WCS                    : #5241.x #5242.y #5243.z  )
-( amax                   :  14.000,  8.000,  3.000  )
-( amin                   :   7.000,  4.000, -5.000  )
-( backoff                :   0.100,  0.100,  0.100  )
-( delta                  :   0.750,  0.400          )
-( iota                   :   0.025,  0.025,  0.025  )
-( MACHINE_ABS_ABOVE_VICE : -28.000,-10.000,-16.000  )
-( start_search           :   3.500,  0.000          )
-( start_search           :   0.000, -2.000          )
-( start_search           :   0.000,  2.000          )
-( start_search           :  -3.500,  0.000          )
-( stop_search            :   0.000,  4.000          )
-( stop_search            :   7.000,  0.000          )
-( stop_search            :  -7.000,  0.000          )
-( stop_search            :   0.000, -4.000          )
-( fast_probe             : 10.0 M79 work xyz probe  )
+( brc                    :  #102.x  #103.y             )
+( cursor                 :  #104.x  #105.y             )
+( error                  :  #106.x  #107.y             )
+( G55                    : #5241.x #5242.y #5243.z     )
+( its                    :  #106.x                     )
+( MACHINE_POS            : #5021.x #5022.y #5023.z     )
+( output                 :  #100.x  #101.y             )
+( output                 :  #102.x  #103.y             )
+( PROBE_R                :  #556.x  #557.y             )
+( SKIP_POS               : #5061.x #5062.y #5063.z     )
+( tlc                    :  #100.x  #101.y             )
+( WCS                    : #5241.x #5242.y #5243.z     )
+( amax                   :  14.000,  8.000,  3.000     )
+( amin                   :   7.000,  4.000, -5.000     )
+( backoff                :   0.100,  0.100,  0.100     )
+( delta                  :   0.750,  0.400             )
+( iota                   :   0.025,  0.025,  0.025     )
+( MACHINE_ABS_ABOVE_VICE : -28.000,-10.000,-16.000     )
+( start_search           :  -3.500,  0.000             )
+( start_search           :   0.000,  2.000             )
+( start_search           :   3.500,  0.000             )
+( start_search           :   0.000, -2.000             )
+( stop_search            :  -7.000,  0.000             )
+( stop_search            :   7.000,  0.000             )
+( stop_search            :   0.000, -4.000             )
+( stop_search            :   0.000,  4.000             )
+( fast_mabs_probe        : 10.0 M79 machine xyz probe  )
+( slow_probe             : 10.0 M79 work xyz probe     )
   O0001                           ( VICECENTER                    )
 
 ( Find center of plate in vice, )
 (  result in [#5241]            )
 ( Search Constraints:           )
 ( start:                        )
 (   -28.0, -13.0, -16.0         )
@@ -43,154 +44,168 @@
   T01 M06                         ( st.setup_probing[]            )
   G65 P9832
   G103 P1
   G04 P1
   G04 P1
   G04 P1
   G55                             ( set_wcs[st.WCS]               )
-  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
-  G01 G90 G53 F65. x-28. y-13.    ( st.goto.machine.xy_then_z[sch.above])
-  G01 G90 G53 F65. z-16.
+  G01 G53 G90 F65. z0.            ( st.goto.machine[z=0]          )
+  G01 G53 G90 F65. x-28. y-13.    ( st.goto.machine.xy_then_z[sch.above])
+  G01 G53 G90 F65. z-16.
 
 ( find top z roughly set [#5241].z. )
   #5241= #5021                    ( st.WCS.xyz = MACHINE_POS.xyz  )
   #5242= #5022
   #5243= #5023
-  G01 G90 G31 M79 F10. z-5.       ( st.fast_probe[z=sch.amin.z]   )
+  G01 G53 G90 G31 M79 F10. z-5.   ( st.fast_mabs_probe[z=sch.amin.z])
   #5243= #5023                    ( st.WCS.z = MACHINE_POS.z      )
 
-  (# 3006) = 101 ( check g55 )
+
+  (# 3006) = 101 (check g55)
+
 
 
 ( now work.z should be 0 at surface )
 ( and work.xy roughly middle        )
   G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= 0.                        ( st.cursor = Var[2][0, 0]      )
   #105= 0.
 
 
 ( quickly move probe to find left edge )
   #106= 5.6667                    (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #104= -3.5                      ( cursor[di.cur_axis] = start_search[di.cur_axis])
-L2000                             ( while its > 0:                )
+  G01 G90 F65. x#104 y#105        ( st.goto.xy_then_z[cursor]     )
+N2000                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2002
-  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
-  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto.z_then_xy[cursor] )
+  G01 G53 G90 G31 M79 F10. z-0.1  (     st.fast_mabs_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2001  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #104= #104 - 0.75               (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2000
-L2002
+N2002
+
 
-  (# 3000) = 101 ( search for left failed )
+  (# 3000) = 101 (search for left failed)
 
-L2001                             (     st.alarm[f"search for {di.name} failed"])
+
+N2001                             (     st.alarm[f"search for {di.name} failed"])
 
 ( back off a bit to the left, then slowly probe  )
 ( rightwards for precise measurement.            )
   #104= #104 - 0.1                ( cursor.xy += sch.backoff * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
-  G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
+  G01 G53 G90 G31 M79 F10. x0. y0.( st.slow_mabs_probe[[0, 0]]    )
   #100= #5061 - #556              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
 
 ( reposition above surface skim height, )
 ( just inside left edge                 )
   G01 G91 F65. x-0.1 y0.          ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= #104 + 1.4                ( cursor.xy += -sch.indent.xy * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
 
 
 ( quickly move probe to find near edge )
   #106= 6.                        (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #105= -2.                       ( cursor[di.cur_axis] = start_search[di.cur_axis])
-L2003                             ( while its > 0:                )
+  G01 G90 F65. x#104 y#105        ( st.goto.xy_then_z[cursor]     )
+N2003                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2005
-  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
-  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto.z_then_xy[cursor] )
+  G01 G53 G90 G31 M79 F10. z-0.1  (     st.fast_mabs_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2004  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #105= #105 - 0.4                (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2003
-L2005
+N2005
+
+
+  (# 3000) = 101 (search for near failed)
 
-  (# 3000) = 101 ( search for near failed )
 
-L2004                             (     st.alarm[f"search for {di.name} failed"])
+N2004                             (     st.alarm[f"search for {di.name} failed"])
 
 ( back off a bit to the near, then slowly probe  )
 ( farwards for precise measurement.              )
   #105= #105 - 0.1                ( cursor.xy += sch.backoff * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
-  G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
+  G01 G53 G90 G31 M79 F10. x0. y0.( st.slow_mabs_probe[[0, 0]]    )
   #103= #5062 - #557              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
 
 ( reposition above surface skim height, )
 ( just inside near edge                 )
   G01 G91 F65. x0. y-0.1          ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #105= #105 + 0.8                ( cursor.xy += -sch.indent.xy * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
 
 
 ( quickly move probe to find far edge )
   #106= 6.                        (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #105= 2.                        ( cursor[di.cur_axis] = start_search[di.cur_axis])
-L2006                             ( while its > 0:                )
+  G01 G90 F65. x#104 y#105        ( st.goto.xy_then_z[cursor]     )
+N2006                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2008
-  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
-  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto.z_then_xy[cursor] )
+  G01 G53 G90 G31 M79 F10. z-0.1  (     st.fast_mabs_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2007  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #105= #105 + 0.4                (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2006
-L2008
+N2008
 
-  (# 3000) = 101 ( search for far failed )
 
-L2007                             (     st.alarm[f"search for {di.name} failed"])
+  (# 3000) = 101 (search for far failed)
+
+
+N2007                             (     st.alarm[f"search for {di.name} failed"])
 
 ( back off a bit to the far, then slowly probe  )
 ( nearwards for precise measurement.            )
   #105= #105 + 0.1                ( cursor.xy += sch.backoff * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
-  G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
+  G01 G53 G90 G31 M79 F10. x0. y0.( st.slow_mabs_probe[[0, 0]]    )
   #101= #5062 + #557              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
 
 ( reposition above surface skim height, )
 ( just inside far edge                  )
   G01 G91 F65. x0. y0.1           ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #105= #105 - 0.8                ( cursor.xy += -sch.indent.xy * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
   G01 G90 F65. x0. y0.            ( st.goto[0, 0]                 )
 
 
 ( quickly move probe to find right edge )
   #106= 5.6667                    (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #104= 3.5                       ( cursor[di.cur_axis] = start_search[di.cur_axis])
-L2009                             ( while its > 0:                )
+  G01 G90 F65. x#104 y#105        ( st.goto.xy_then_z[cursor]     )
+N2009                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2011
-  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
-  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto.z_then_xy[cursor] )
+  G01 G53 G90 G31 M79 F10. z-0.1  (     st.fast_mabs_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2010  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #104= #104 + 0.75               (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2009
-L2011
+N2011
+
 
-  (# 3000) = 101 ( search for right failed )
+  (# 3000) = 101 (search for right failed)
 
-L2010                             (     st.alarm[f"search for {di.name} failed"])
+
+N2010                             (     st.alarm[f"search for {di.name} failed"])
 
 ( back off a bit to the right, then slowly probe  )
 ( leftwards for precise measurement.              )
   #104= #104 + 0.1                ( cursor.xy += sch.backoff * di.dxdy)
   G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
-  G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
+  G01 G53 G90 G31 M79 F10. x0. y0.( st.slow_mabs_probe[[0, 0]]    )
   #102= #5061 + #556              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
 
 ( reposition above surface skim height, )
 ( just inside right edge                )
   G01 G91 F65. x0.1 y0.           ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= #104 - 1.4                ( cursor.xy += -sch.indent.xy * di.dxdy)
@@ -204,12 +219,14 @@
   #5241= #5241 + #106             ( st.WCS.xy += st.error.xy      )
   #5242= #5242 + #107
   G01 G90 F65. x0. y0.            ( st.goto[0, 0]                 )
 
 (  final slow probe to find the surface z )
   G01 G90 G31 M79 F10. z-0.1      ( st.slow_probe[z=sch.search_depth])
   #5243= #5063                    ( st.WCS.z = SKIP_POS.z         )
-  G01 G90 G53 F65. z-16.          ( st.goto.machine[z=sch.above.z])
+  G01 G53 G90 F65. z-16.          ( st.goto.machine[z=sch.above.z])
+
+
+  (# 3000) = 101 ( what changed)
 
-  (# 3000) = 101 (  what changed )
 
-  M30                             ( st.alarm[" what changed"]     )
+  M30
```

### Comparing `p2g-0.2.4/p2g/examples/vicecenter.py` & `p2g-0.2.5/p2g/examples/vicecenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,32 +44,33 @@
 
     its = p2g.Var(
         (abs(stop_search - start_search) / sch.delta)[di.cur_axis] + 1,
     )
     cursor = st.cursor
 
     cursor[di.cur_axis] = start_search[di.cur_axis]
-
+    st.goto.xy_then_z(cursor)
     while its > 0:
-        st.goto(cursor)
-        st.fast_probe(z=sch.search_depth)
+        st.goto.z_then_xy(cursor)
+        st.fast_mabs_probe(z=sch.search_depth)
         if SKIP_POS.z < sch.search_depth + sch.iota:
             break
+
         cursor.xy += delta
         its -= 1
     else:
         st.alarm(f"search for {di.name} failed")
 
     p2g.comment(
         f"back off a bit to the {di.name}, then slowly probe ",
         f"{di.opposite}wards for precise measurement.",
     )
     cursor.xy += sch.backoff * di.dxdy
     st.goto(cursor.xy)
-    st.slow_probe([0, 0])
+    st.slow_mabs_probe([0, 0])
 
     # sets part of tlc or brc
     output[di.cur_axis] = (SKIP_POS + PROBE_R * di.dxdy)[di.cur_axis]
 
     p2g.comment(
         "reposition above surface skim height,",
         f"just inside {di.name} edge",
@@ -89,15 +90,15 @@
 
     st.goto.machine.xy_then_z(sch.above)
 
     p2g.comment(f"find top z roughly set {st.WCS}.z.")
 
     st.WCS.xyz = MACHINE_POS.xyz
     # fast find move down to min search distance
-    st.fast_probe(z=sch.amin.z)
+    st.fast_mabs_probe(z=sch.amin.z)
 
     # make work offset z make rough top 0.
     st.WCS.z = MACHINE_POS.z
     st.pause("check g55")
 
     p2g.comment(
         "now work.z should be 0 at surface",
@@ -146,17 +147,16 @@
 
     st.setup_probing()
 
     find_surface_before(st, sch)
 
 
 def vicecenter():
-    p2g.symbol.Table.print = True
     st = defs.JobDefs()
-
+    p2g.symbol.Table.print = 1
     sch = csearch.SearchConstraint(
         # minimum size expected
         amin=p2g.Const(x=7.0, y=4.0, z=-5.0),
         # maximum size expected
         amax=p2g.Const(x=14.0, y=8.0, z=3.0),
         delta=p2g.Const(x=0.75, y=0.4),
         above=st.MACHINE_ABS_ABOVE_VICE + p2g.Const(x=0.0, z=0.0, y=-3.0),
```

### Comparing `p2g-0.2.4/p2g/gbl.py` & `p2g-0.2.5/p2g/gbl.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/goto.py` & `p2g-0.2.5/p2g/goto.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,91 +13,116 @@
 # kwargs could contain x,y,z,feed ec
 # as could extras
 
 
 class MovementSpace(enum.IntEnum):
     WORK = enum.auto()
     MACHINE = enum.auto()
-    RELATIVE = enum.auto()
     R9810 = enum.auto()
 
 
+class MovementRelOrAbs(enum.IntEnum):
+    RELATIVE = enum.auto()
+    ABSOLUTE = enum.auto()
+
+
 class MovementOrder(enum.IntEnum):
     XYZ = enum.auto()
     XY_THEN_Z = enum.auto()
     Z_THEN_XY = enum.auto()
 
 
 def do_goto_worker(self, fter, args, kwargs):
     # split out arguments we understand from
     # ones for coordinates.
 
-    values = coords.unpack(args, kwargs)
-
-    res = ["G01"]
-
-    match self.space_:
-        case MovementSpace.MACHINE:
-            res.append("G90")
-            res.append("G53")
-        case MovementSpace.RELATIVE:
-            res.append("G91")
-        case MovementSpace.WORK:
-            res.append("G90")
-        case MovementSpace.R9810:
-            res.append("G65 R9810")
-
-    if self.probe_:
-        res.append("G31")
-    if self.mcode_:
-        res.append(self.mcode_)
-
-    if self.feed_ == 0.0:
-        err.compiler("Need feed rate.")
-
-    res.append(f"F{nd.to_gcode(self.feed_)}")
-
-    cos = []
-    for aname, value in zip(axis.low_names_v(), values):
-        if fter and aname not in fter:
-            continue
-
-        if value.is_none_constant:
-            continue
-        cos.append(f"{aname}{value.to_gcode(nd.NodeModifier.EMPTY)}")
+    def accumulate_relorabs():
+        match self.relorabs_:
+            case MovementRelOrAbs.ABSOLUTE:
+                yield "G90"
+
+            case MovementRelOrAbs.RELATIVE:
+                yield "G91"
+
+    def accumulate_probe():
+        if self.probe_:
+            yield "G31"
+
+    def accumulate_mcode():
+        if self.mcode_:
+            yield self.mcode_
+
+    def accumulate_feed():
+        if self.feed_ == 0.0:
+            err.compiler("Need feed rate.")
+
+        yield f"F{nd.to_gcode(self.feed_)}"
+
+    def accumulate_parts():
+        match self.space_:
+            case MovementSpace.MACHINE:
+                yield "G01"
+                yield "G53"
+                yield from accumulate_relorabs()
+                yield from accumulate_probe()
+                yield from accumulate_mcode()
+            case MovementSpace.WORK:
+                yield "G01"
+                yield from accumulate_relorabs()
+                yield from accumulate_probe()
+                yield from accumulate_mcode()
+            case MovementSpace.R9810:
+                yield "G65 R9810"
+                if self.relorabs_ & MovementRelOrAbs.RELATIVE:
+                    err.compiler("Relative with 9810 move is illegal.")
+
+                if self.probe_:
+                    err.compiler("Probe with 9810 move is illegal.")
+
+                if self.mcode_:
+                    err.compiler("MCODE with 9810 move is illegal.")
+
+        yield from accumulate_feed()
+
+    def get_coords():
+        values = coords.unpack(args, kwargs)
+        for aname, value in zip(axis.low_names_v(), values):
+            # skip non important coords
+            if fter and aname not in fter:
+                continue
+            # skip non mentioned coords
+            if value.is_none_constant:
+                continue
+            yield aname, value
+
+    def accumulate_coords(cos):
+        for aname, value in cos:
+            yield f"{aname}{value.to_gcode(nd.NodeModifier.EMPTY)}"
 
+    cos = list(get_coords())
     if not cos:
         return
 
-    rtxt = " ".join(res + cos)
-
-    stat.code(rtxt)
+    stat.code(
+        accumulate_parts(),
+        accumulate_coords(cos),
+    )
 
 
 @dataclasses.dataclass(eq=True, frozen=True)
 class GotoWorker:
     user_defined = True
     want_bp_: bool
     space_: MovementSpace
-    feed_: float
     order_: MovementOrder
+    relorabs_: MovementRelOrAbs
+    feed_: float
     probe_: bool
     mcode_: str
 
-    # def __eq__(self, x):
-    #     breakpoint()
-
-    # def __lt__(self, x):
-    #     breakpoint()
-
-    # def __hash__(self):
-    #     v = object.__hash__(self)
-    #     breakpoint()
-    #     return v
-
     def to_symtab_entry(self, *_) -> str:
         return "".join(
             [
                 str(self.feed_),
                 " ",
                 self.mcode_ + " " if self.mcode_ else "",
                 self.space_.name.lower(),
@@ -139,15 +164,19 @@
 
     @property
     def xyz(self):
         return self.update("order_", MovementOrder.XYZ)
 
     @property
     def relative(self):
-        return self.update("space_", MovementSpace.RELATIVE)
+        return self.update("relorabs_", MovementRelOrAbs.RELATIVE)
+
+    @property
+    def absolute(self):
+        return self.update("relorabs_", MovementRelOrAbs.ABSOLUTE)
 
     def feed(self, feed):
         return self.update("feed_", feed)
 
     def mcode(self, m_code):
         return self.update("mcode_", str(m_code))
 
@@ -163,12 +192,13 @@
                 do_goto_worker(self, "z", args, kwargs)
 
 
 nd.HasToSymTab.register(GotoWorker)
 goto = GotoWorker(
     want_bp_=False,
     space_=MovementSpace.WORK,
-    feed_=0.0,
+    relorabs_=MovementRelOrAbs.ABSOLUTE,
     order_=MovementOrder.XYZ,
+    feed_=0.0,
     probe_=False,
     mcode_="",
 )
```

### Comparing `p2g-0.2.4/p2g/haas.py` & `p2g-0.2.5/p2g/haas.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 MUST_SKIP = "M79"
 FEED_FAST = 650.0
 FEED_SLOW = 50.0
 PROBE_FAST = 50.0
 PROBE_SLOW = 10.0
 PROBE_ON = ["G65 P9832"]
 PROBE_H = p2g.Fixed[3](addr=2001)
-# OTS_ON = ["M59 P2", "G04 P1.0", "M59 P3"]
-OTS_ON = ["G65 P9855", "G103 P1"]
+OTS_ON = ["M59 P2", "G04 P1.0", "M59 P3"]
 OTS_OFF = ["M69 P2", "M68 P3"]
-SPINDLE_PROBE_ON = ["G65", "P9832"]
-SPINDLE_PROBE_OFF = ["G65", "P9833"]
+SPINDLE_PROBE_ON = "G65 P9832"
+SPINDLE_PROBE_OFF = "G65 P9833"
 NO_LOOKAHEAD = ["G103 P1", "G04 P1", "G04 P1", "G04 P1"]
 
 # MACHINE GEN BELOW
 NULL = p2g.Fixed(addr=0)
 MACRO_ARGUMENTS = p2g.Fixed[33](addr=1)
 # 34 .. 99 - ..
 GP_SAVED1 = p2g.Fixed[100](addr=100)
```

### Comparing `p2g-0.2.4/p2g/lib.py` & `p2g-0.2.5/p2g/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import dataclasses
+import functools
 import sys
 import typing
 
 from p2g import gbl
 
 
 def max_str_len(lines):
@@ -134,19 +135,43 @@
 
     def read(self):
         return SimpleIBuf.fromstdin
 
 
 @contextlib.contextmanager
 def openr(name):
-    if str(name) == "<null>":
+    if str(name) == "<stdin>":
+        yield SimpleIBuf("") if gbl.config.debug else sys.stdin
+    elif str(name) == "<null>":
         yield SimpleIBuf("")
     else:
         with open(name, "r", encoding="utf-8") as rfile:
             yield rfile
 
 
-# a print which could be quieted.
-def qprint(*args):
-    if gbl.opts["--quiet"]:
-        return
-    print(*args)
+def log(*args):
+    if gbl.config.debug:
+        print(*args)
+
+
+@functools.cache
+def logread(handle):
+    res = handle.read()
+    log(res)
+    return res
+
+
+# unwind a list of lists etc
+# can turn generators of lists of strings into
+# space joined string.
+
+
+def unwind1(args):
+    if isinstance(args, str):
+        yield args
+    else:
+        for el in args:
+            yield from unwind1(el)
+
+
+def unwind(args):
+    return " ".join(unwind1(args))
```

### Comparing `p2g-0.2.4/p2g/main.py` & `p2g-0.2.5/p2g/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,31 +2,29 @@
 import datetime
 import pathlib
 import shutil
 import sys
 
 import docopt
 
-from loguru import logger
-
 from p2g import debug
 from p2g import err
 from p2g import gbl
 from p2g import lib
 from p2g import makestdvars
 from p2g import version
 from p2g import walk
 
 
 DOC = """
 Turns a python program into a gcode program.
 
 Usage:
-   p2g [options] gen <srcfile>
-   p2g [options] ngen <srcfile>
+   p2g [options] gen [ <srcfile> ]
+   p2g [options] ngen [ <srcfile> ]
    p2g [options] test
    p2g [options] examples
    p2g [options] version
    p2g [options] stdvars [--txt=<txtfile>] [--dev=<devfile>] [--py=<pyfile>] [--org=<orgfile>]
 
 Try:
    p2g gen -o ../nc/O05AC.nc vf3/vicecenter.py
@@ -52,24 +50,21 @@
    p2g stdvars
        Regenerate machine specific definitions.
 
 Options:
     -o <file> --out=<file>   Output file, [default: <stdout>]
     --outdir <dir>           Output directory, [default: .]
     -h --help                This.
-    -q --quiet               Make less noise.
     --relative-paths         Errors contain paths relative to current directory.
     --relative-lines         Errors contain linenumbers relative to start of function.
     --job=<pattern>             Job name, [default: O0001]
     --function=<name>        Function to compile, [default: <last function in file>]
     --debug                  Enter debugging code. [default: False]
     --recursive              Notify when called by self. [default: False]
-    --logfile=<logfile>      Turn on logger.and send to <logfile> [default: <stdout>]
-    --loglevel=<loglevel>    Set logger.level [default: ERROR]
-    --break-on-error         Breakpoint on error.
+    --break                  Breakpoint on error.
 
     output pattern may include <time> which will create a decrementing
     prefix for the output file which makes looking for the .nc in a
     crowded directory simpler.
 
     eg  --out="~/_nc_/<time>O001-foo.nc" foo.py
     makes an output of the form ~/_nc_/001234O001-foo.nc
@@ -87,48 +82,31 @@
 
     outdir = gbl.opts["--outdir"]
     outdir.mkdir(exist_ok=True, parents=True)
 
     srcnames = []
     for src in examples:
         dst_name = outdir / src.parts[-1]
-        lib.qprint(f"Copying {src} {dst_name}")
+        print(f"Copying {src} {dst_name}")
         shutil.copy(src, dst_name)
         srcnames.append(dst_name)
     for job in ["vicecenter", "probecalibrate"]:
         top_name = outdir / (job + ".py")
         out_name = outdir / (job + ".nc")
         sysargs = [
             "--out",
             str(out_name),
             "gen",
             str(top_name),
         ]
 
-        lib.qprint(f"Running {' '.join(sysargs)}")
+        print(f"Running {' '.join(sysargs)}")
         main(sysargs)
 
 
-def setup_logger():
-    loglevel = gbl.opts["--loglevel"]
-
-    logfile = gbl.opts["--logfile"]
-    if logfile == "<stdout>":
-        logfile = sys.stdout
-
-    logger.remove()
-    logger.add(
-        logfile,
-        level=loglevel,
-        format="{message}",
-    )
-
-    logger.info(f"Logging on {gbl.opts['--loglevel']} {logfile}")
-
-
 def output_file_name():
     now = datetime.datetime.now()
     prev_midnight = now.replace(hour=0, minute=0, second=0, microsecond=0)
     next_midnight = 24 * 60
     mins_togo = next_midnight - (now - prev_midnight).seconds // 60
 
     out_name = "-"
@@ -140,28 +118,30 @@
     return out_name
 
 
 def do_gen():
     gbl.config.in_pytest = False
 
     src_name = gbl.opts["<srcfile>"]
+    if src_name is None or src_name == "-":
+        src_name = "<stdin>"
     src_path = pathlib.Path(src_name)
     job_name = src_path.stem
 
     if gbl.opts["--job"] != "<srcfilename>":
         job_name = gbl.opts["--job"]
 
     func_name = gbl.opts["--function"]
 
     output_name = gbl.opts["--out"]
 
-    logger.info(f"src: {src_path}")
-    logger.info(f"fnc: {func_name}")
-    logger.info(f"job: {job_name}")
-    logger.info(f"output: {output_name}")
+    lib.log(f"src: {src_path}")
+    lib.log(f"fnc: {func_name}")
+    lib.log(f"job: {job_name}")
+    lib.log(f"output: {output_name}")
     try:
         res = walk.compile2g(func_name, src_path, job_name=job_name, in_pytest=False)
         lib.write_nl_lines(res, output_name)
         return 0
     except err.CompilerError as exn:
         exn.report_error(absolute_lines=True)
     except FileNotFoundError as exn:
@@ -172,23 +152,22 @@
     if gbl.opts["--recursive"]:
         return 0
     return 1
 
 
 def main(options=None):
     gbl.opts = docopt.docopt(DOC, options)
-
     gbl.config.debug = gbl.opts["--debug"]
+
     gbl.config.opt_relative_paths = gbl.opts["--relative-paths"]
     gbl.config.opt_relative_lines = gbl.opts["--relative-lines"]
+    gbl.config.bp_on_error = gbl.opts["--break"]
 
     gbl.opts["--outdir"] = pathlib.Path(gbl.opts["--outdir"])
 
-    setup_logger()
-    logger.info(options)
     gbl.opts["--out"] = output_file_name()
 
     if gbl.opts["version"]:
         with lib.openw(gbl.opts["--out"]) as out:
             print(f"Version: p2g {version.__version__}", file=out)
 
     if gbl.opts["examples"]:
```

### Comparing `p2g-0.2.4/p2g/makestdvars.py` & `p2g-0.2.5/p2g/makestdvars.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,32 +46,30 @@
 class MacroVar:
     def __init__(self, *, key, addr, alias=None, size=None, name="", typ=""):
         self.typ = typ
         self.key = key
         self.addr = addr
 
         self.name = name
-        self._alias = alias
+        self.alias = alias
         self.size = size
         suffix = ""
         self.last = None
         if isinstance(self.size, NAXES):
+            self.size_as_text = "naxes"
             self.last = NAXES
             suffix = "…"
         else:
             self.last = self.addr + self.size - 1
+            # that's a non breaking space
+            self.size_as_text = f"{self.size:5}"
+
             if self.last != self.addr:
                 suffix = f" … #{self.last:5}"
-        self.range_as_text = f"#{self.addr:5}{suffix}"
-
-    @property
-    def alias_name(self):
-        if self._alias:
-            return self._alias.name
-        return ""
+        self.range_as_text = f"#{self.addr:5}{suffix}".center(15)
 
     def for_regen(self):
         funcname = self.__class__.__qualname__
         res = [str(self.addr)]
         if self.size is not None:
             res.append(f"size={self.size}")
         restxt = ", ".join(res)
@@ -84,15 +82,19 @@
             str(self.size),
             self.key,
             self.typ,
             self.name,
         )
 
     def for_org(self):
-        return f"| ={self.name}= | ~{self.size}~ | ~{self.range_as_text}~ |\n"
+        return (
+            f"| <code>{self.name}</code> "
+            + f"| <code>{self.size_as_text}</code>"
+            + f"| <code>{self.range_as_text}</code> |\n"
+        )
 
     def for_py_out(self):
         return f"# {self.addr} .. {self.last} {self.name} .."
 
     def __lt__(self, other):
         return self.addr < other.addr
 
@@ -140,18 +142,20 @@
 
 
 class Alias(MacroVar):
     def __init__(self, src):
         super().__init__(key="A", addr=src.addr, size=src.size, alias=src)
 
     def for_regen(self):
-        return f"{def_prefix(self.name.ljust(20))} = alias({def_prefix}{self.alias_name})"
+        assert self.alias is not None
+        return f"{def_prefix(self.name.ljust(20))} = alias({def_prefix}{self.alias.name})"
 
     def for_py_out(self):
-        return f"{def_prefix(self.name)} = {MAKE_PFX}alias({def_prefix(self.alias_name)})"
+        assert self.alias is not None
+        return f"{def_prefix(self.name)} = {MAKE_PFX}alias({def_prefix(self.alias.name)})"
 
     def for_txt(self):
         return (
             self.range_as_text,
             str(self.size),
             self.key,
             self.typ,
@@ -424,47 +428,37 @@
     guts.add_column("K", justify="right")
     guts.add_column("Type", justify="center")
     guts.add_column("Name", justify="left")
 
     snames = sorted(names.interesting)
     for el in snames:
         guts.add_row(*el.for_txt())
-        if el.alias_name:
-            guts.add_row(*el.for_txt())
+        if el.alias:
+            el = el.alias
 
-    with open(outname, "w", encoding="utf-8") as out:
+    with lib.openw(outname) as out:
         console = rich.console.Console(file=out)
         console.print(guts, style=None)
         print("Generated ", outname)
 
 
 def regen_out(outname, defs):
     with open(outname, "w", encoding="utf-8") as out:
         for el in sorted(defs.interesting):
             out.write("        " + el.for_regen())
 
 
 def org_out(outname, defs):
     with lib.openw(outname) as out:
-        #        out.write("1 2 3\n")
-
-        #        out.write("#+begin_example\n")
-
-        out.write("| Name | Size | Address |\n")
-        out.write("| / | <r> |  |\n")
-
+        out.write("| Name          |  Size | Address         |\n")
+        out.write("| --- | --- | --- |\n")
         for el in sorted(defs.interesting):
             if el.name != "-":
                 out.write(el.for_org())
 
-        out.write("|------|------|---------|\n")
-
-
-#        out.write("#+end_example\n")
-
 
 def py_out(target_filename, defs):
     tmp_filepath = pathlib.Path(target_filename).with_suffix(".tmp")
 
     with open(target_filename, encoding="utf-8") as inf:
         repl = re.match(
             "(.*?# MACHINE GEN BELOW.*?).*(.*?# MACHINE.*)",
```

### Comparing `p2g-0.2.4/p2g/mvarsorig` & `p2g-0.2.5/p2g/mvarsorig`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/nd.py` & `p2g-0.2.5/p2g/nd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import enum
+import typing
 
 
 class NodeModifier(enum.IntFlag):
     # so 0 is an error
     EMPTY = enum.auto()
 
     # ADDRESSES are always integers
@@ -20,14 +21,34 @@
     @abc.abstractmethod
     def to_symtab_entry(self, _addrs_used) -> str:
         return ""
 
 
 # common base class for scalar and vector.
 class EBase(abc.ABC):
+    @abc.abstractmethod
+    def everything(self) -> typing.Generator[typing.Any, None, None]:
+        ...
+
+    def get_at(self, _idx) -> typing.Any:
+        return None  # no cover
+
+    def set_at(self, _idx, _src):
+        pass  # no cover
+
+    def nelements(self):
+        return 1  # no cover
+
+    def get_slice(self, _slice) -> typing.Any:
+        return None  # no cover
+
+    @abc.abstractmethod
+    def get_address(self) -> int:
+        ...
+
     def to_gcode(self, _modifier: NodeModifier) -> str:
         return ""  # no cover
 
     # placeholder to east typechecking,
     # overwitten by op install machines.
     @abc.abstractmethod
     def __add__(self, _other):
```

### Comparing `p2g-0.2.4/p2g/op.py` & `p2g-0.2.5/p2g/op.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from p2g import opinfo
 from p2g import scalar
 from p2g import symbol
 from p2g import vector
 
 
 OptRes = typing.Optional[scalar.Scalar]
+ScalarScalar = typing.Union[scalar.Scalar, int, float, bool]
 
 op_byclass: typing.Dict[typing.Any, opinfo.Opinfo] = {}
 allops: typing.Dict[str, opinfo.Opinfo] = {}
 
 
 def parensif(cond, thing):
     if cond:
@@ -154,15 +155,15 @@
 
         return "".join(res)
 
     def __repr__(self):
         return f"({self.opfo.pyn} {self.child})"
 
 
-def make_scalar_unop(opfo, child: scalar.Scalar):
+def make_scalar_unop(opfo, child: ScalarScalar):
     child = scalar.wrap_scalar(child)
     if opfo.opt1 and (res := opfo.opt1(opfo, child)) is not None:
         return res
 
     if isinstance(child, scalar.Constant):
         return scalar.wrap_scalar(getattr(child.value, opfo.mth)())
```

### Comparing `p2g-0.2.4/p2g/opinfo.py` & `p2g-0.2.5/p2g/opinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ast
-
 # just information about operators.
 # pylint: disable=too-many-instance-attributes
 import dataclasses
 import typing
 
 
 def opt_null(*_):
```

### Comparing `p2g-0.2.4/p2g/ptest.py` & `p2g-0.2.5/p2g/ptest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import functools
 import inspect
 import itertools
 import pathlib
 import typing
 
-import pytest
-
-from loguru import logger
-
 from p2g import err
 from p2g import gbl
 from p2g import lib
 from p2g import walk
 
 
-USE_FILENAME = False
 # takes fn, works out where it lives, where to find golden output and
 # where to put test output
-# <filename>.py (test_zap) will make a tests/golden/<filename>test_zap.nc file.
-# the <filename> part is optional
+# test_foo.py (test_zap) will make a tests/golden/test_foo_test_zap.nc file.
 
 
 def make_file_path(func, new_suffix) -> pathlib.Path:
     # this_file_path <- <somewhere>/ptest.py
     this_file_path = pathlib.Path(__file__)
     # this_file_directory <- <somewhere>/p2g
     this_file_directory = this_file_path.parent
 
     # file_part <- function's filename
-    file_part = (
-        str(pathlib.Path(func.__code__.co_filename).stem) + "_" if USE_FILENAME else ""
-    )
+    file_part = str(pathlib.Path(func.__code__.co_filename).stem)
+    #    file_part = file_part.replace("test_", "")
+
     # can be in <srcdir>/tests or ../tests depending upon
     # if run installed or not. Look for testdir.
 
     for tests_dir in [
         this_file_directory / "tests",
         this_file_directory.parent / "tests",
     ]:
@@ -45,15 +39,15 @@
 
     # generated_dir <- <somewhere>/tests/golden
     generated_dir = tests_dir / "golden"
     generated_dir.mkdir(exist_ok=True)
     #  <somewhere>/tests/golden/foo_zap.nc
 
     #    new_filename = func.__name__.replace("test", file_part)
-    new_filename = file_part + func.__name__
+    new_filename = file_part + "_" + func.__name__
     return (generated_dir / new_filename).with_suffix(new_suffix)
 
 
 def strip_comments(txt):
     txt = txt.replace(" ", "")
     idx = txt.find("(")
     if idx >= 0:
@@ -72,15 +66,15 @@
 def strip_lines_comments(block):
     for line in block:
         yield strip_comments(line)
 
 
 # find differences in stuff which isn't commented.
 # return a set of lines with diffs.
-def find_differences_(
+def find_differences(
     golden_data: typing.Sequence[str],
     callow_data: typing.Sequence[str],
     check_comments: bool,
 ):
     lhs_src = golden_data
     rhs_src = callow_data
     if not check_comments:
@@ -93,21 +87,16 @@
         itertools.zip_longest(lhs_src, rhs_src, fillvalue="")
     ):
         if want != got:
             diffs.add(line)
     return diffs
 
 
-find_differences = lib.g2l(find_differences_)
-
-
 @lib.g2l
-def format_differences(
-    marks, golden_data: list[str], callow_data: list[str]
-) -> typing.Iterable:
+def format_differences(marks, golden_data: list[str], callow_data: list[str]):
     fromto = slice(max(min(marks) - 4, 0), min(marks) + 10)
 
     lhs_width = max(len(x) for x in golden_data[fromto])
 
     def fmt(lhs, middle, rhs):
         return lhs.ljust(lhs_width) + middle + rhs
 
@@ -126,15 +115,15 @@
             rhs,
         )
 
 
 def writelines(fn, suffix, txt, comment):
     path = make_file_path(fn, suffix)
     print(f"WRRTIGIN {comment} to ", path)
-    logger.error(f"Ptest error, writing to {comment}")
+    lib.log(f"Ptest error, writing to {comment}")
     return path.write_text(lib.nljoin(txt))
 
 
 # when a test fails, create source which would
 # have passed.
 
 
@@ -153,38 +142,44 @@
     while lines and not lines[0].startswith("def"):
         lines = lines[1:]
 
     writelines(fn, ".decorator", tofix + lines, "creating decorator")
 
 
 # compile fn, return generated errors or text.
-
-
+@lib.g2l
 def get_all_comp_outputs(fn):
     try:
         outlines = walk.compile2g(
             fn.__name__,
             inspect.getsourcefile(fn),
             job_name=None,
             in_pytest=True,
         )
     except err.CompilerError as exn:
         outlines = exn.error_lines(absolute_lines=False, topfn=fn)
     return outlines
 
 
+@lib.g2l
+def read_and_trim(path):
+    lines = lib.splitnl(path.read_text())
+    for line in lines:
+        yield line
+
+
 # when called from test, exceptions are sent to output file
 # as well as being passed up.
 
 
 # compile code and compare output with file.
 
 
 def check_must_be_worker(fn, gold_data, check_comments=False):
-    callow_data = get_all_comp_outputs(fn)
+    callow_data = list(get_all_comp_outputs(fn))
 
     markers = find_differences(gold_data, callow_data, check_comments)
 
     if not markers:
         return
     etext = format_differences(markers, gold_data, callow_data)
 
@@ -194,43 +189,39 @@
         return
 
     # if running in pytest then exist out gracefully for them.
     # otherwise, running in debug harness.
     if gbl.config.debug:  # for debug
         err.compiler(f"ptest error {lib.nljoin(etext)}")
 
-    pytest.fail(lib.nljoin(etext))  # for debug
-
-
-def read_and_trim(path):
-    return lib.splitnl(path.read_text())
+    assert False, lib.nljoin(etext)  # for debug
 
 
 def check_golden_worker(fn, check_comments):
-    callow = get_all_comp_outputs(fn)
+    callow = list(get_all_comp_outputs(fn))
 
     gold_path = make_file_path(fn, ".nc")
     if gold_path.exists():
-        gold_data = read_and_trim(gold_path)
+        gold_data = list(read_and_trim(gold_path))
 
         markers = find_differences(gold_data, callow, check_comments)
         if not markers:
             return
         etext = format_differences(markers, gold_data, callow)
 
-        writelines(fn, ".got", callow, "compare error")
+        writelines(fn, ".got", callow, "compare fail so")
 
         # if running in pytest then exist out gracefully for them.
         # otherwise, running in debug harness.
         if gbl.config.debug:  # for debug
             for line in etext:
                 print(line)
             err.compiler(f"ptest error {lib.nljoin(etext)}")
 
-        pytest.fail(lib.nljoin(etext))
+        assert False, lib.nljoin(etext)
 
     else:
         # no source gold, make it.
         writelines(fn, ".nc", callow, "no source gold, create")
 
 
 # decorator for tests, turns the node into ast and calls
```

### Comparing `p2g-0.2.4/p2g/scalar.py` & `p2g-0.2.5/p2g/scalar.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,17 +133,14 @@
     if res is not None:
         return res
 
     return thing.to_scalar()
 
 
 # make a range between wrapped items and yield ints
-def urange(start, stop, step=None):
+def urange(start, stop, step=1):
     stop = int(stop)
-    if step is None:
-        step = 1
-    else:
-        step = int(step)
+    step = int(step)
 
     tmp = list(range(int(start), stop, step))
     for el in tmp:
         yield el
```

### Comparing `p2g-0.2.4/p2g/stat.py` & `p2g-0.2.5/p2g/stat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import abc
 import dataclasses
 import itertools
 import typing
 
-from loguru import logger
-
 from p2g import err
 from p2g import gbl
 from p2g import lib
 from p2g import nd
 
 
 COMMENT_INDENT = 34
@@ -27,15 +25,15 @@
         self.idx = idx
         self.used = False
 
     def as_gcode_ref(self):
         return f"{self.idx}"
 
     def as_gcode_definition(self):
-        return f"L{self.idx}"
+        return f"N{self.idx}"
 
 
 # auto comment is a comment which comes from
 # the source, rather than being typed.
 # we take liberties to increase information density.
 
 
@@ -60,44 +58,41 @@
 
     if guts.startswith("    "):
         guts = guts[4:]
 
     return "( " + guts.ljust(30) + ")"
 
 
-def workout_comtxt(pos, comtxt, blockstate):
-    if comtxt == "<no comment>":
-        return ""
-
-    if not comtxt:
-        comtxt = err.src_code_from_node_place(pos)
-    comtxt = compress_and_clean(comtxt)
-    if comtxt == blockstate.prev_comtxt:
-        comtxt = ""
-    else:
-        blockstate.prev_comtxt = comtxt
-    return comtxt
-
-
 @dataclasses.dataclass
 class StatBase(abc.ABC):
-    _comtxt: str
+    _comment: str
 
-    # empty comment means use src if possible.
-    # <no comment> means no comment
-    def __init__(self, comtxt=""):
+    def __init__(self, comment_txt=None):
         self.pos = err.state.last_pos
-        self._comtxt = comtxt
+
+        # if specifically asked for none, then we're done.
+        if comment_txt == "<none>":
+            self._comment = ""
+        else:
+            # no comment supplied, then use source line.
+            if not comment_txt:
+                comment_txt = err.src_code_from_node_place(self.pos)
+            comment_txt = compress_and_clean(comment_txt)
+            self._comment = comment_txt
 
     def to_line_lhs(self) -> list[str]:
-        return []  # no cover
+        raise AssertionError
 
     @lib.g2l
     def to_full_lines(self, blockstate):
-        comtxt = workout_comtxt(self.pos, self._comtxt, blockstate)
+        comtxt = self._comment
+        if comtxt == blockstate.prev_comtxt:
+            comtxt = ""
+        else:
+            blockstate.prev_comtxt = comtxt
 
         for code_txt, com_txt in itertools.zip_longest(
             self.to_line_lhs(),
             [comtxt],
             fillvalue="",
         ):
             # If code would leak into comment, put out the comment on
@@ -182,15 +177,15 @@
             if line.strip():
                 yield "( " + clean_comment_chars(line) + " )"
             else:
                 yield ""
 
 
 def add_stat(stat):
-    logger.info(f"Adding {stat}")
+    lib.log(f"Adding {stat}")
     Nest.add_stat(stat)
 
 
 def comment(*lines):
     add_stat(CommentLines(" "))
     add_stat(CommentLines(lines))
 
@@ -228,28 +223,29 @@
         yield NORMAL_PREFIX + lhs + rhs
 
 
 @dataclasses.dataclass
 class Code(StatBase):
     txt: str
 
-    def __init__(self, txt, ctxt):
-        super().__init__(ctxt)
-        self.txt = txt
+    def __init__(self, txtargs, comment_txt=""):
+        super().__init__(comment_txt=comment_txt)
+
+        self.txt = lib.unwind(txtargs)
 
     def to_line_lhs(self):
         yield NORMAL_PREFIX + self.txt
 
 
 @dataclasses.dataclass
 class Dprint(StatBase):
     txt: str
 
     def __init__(self, txt):
-        super().__init__("<no comment>")
+        super().__init__("<none>")
         self.txt = txt
 
     def to_line_lhs(self):
         yield "DPRNT[" + self.txt + "]"
 
 
 class Set(StatBase):
@@ -270,22 +266,29 @@
 
 
 def append_set(dst, src, comtxt=""):
     if not lib.same(dst, src):
         add_stat(Set(dst, src, comtxt))
 
 
-def code(txt, comtxt: str = ""):
-    if isinstance(txt, str):
-        add_stat(Code(txt, comtxt))
-        return
-
-    for line in txt:
-        code(str(line), comtxt)
-        comtxt = ""
+def code(*txtargs, comment_txt: str = ""):
+    add_stat(Code(txtargs, comment_txt=comment_txt))
+
+
+def codenl(txtlst, comtxt: str = ""):
+    if isinstance(txtlst, str):
+        add_stat(Code(txtlst, comtxt))
+    else:
+        for txt in txtlst:
+            codenl(txt, comtxt)
+            comtxt = ""
+
+
+# take list of args and chain them
+# and then join. Take care with strings.
 
 
 @dataclasses.dataclass
 class LabelDef(StatBase):
     labeldef: Label
 
     def __init__(self, labeldef: Label):
```

### Comparing `p2g-0.2.4/p2g/symbol.py` & `p2g-0.2.5/p2g/symbol.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/golden/vicecenter.gold` & `p2g-0.2.5/p2g/tests/golden/vicecenter_vicecenter.nc`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-( brc                    :  #102.x  #103.y          )
-( cursor                 :  #104.x  #105.y          )
-( error                  :  #106.x  #107.y          )
-( G55                    : #5241.x #5242.y #5243.z  )
-( its                    :  #106.x                  )
-( MACHINE_POS            : #5021.x #5022.y #5023.z  )
-( output                 :  #102.x  #103.y          )
-( output                 :  #100.x  #101.y          )
-( PROBE_R                :  #556.x  #557.y          )
-( SKIP_POS               : #5061.x #5062.y #5063.z  )
-( tlc                    :  #100.x  #101.y          )
-( WCS                    : #5241.x #5242.y #5243.z  )
-( amax                   :  14.000,  8.000,  3.000  )
-( amin                   :   7.000,  4.000, -5.000  )
-( backoff                :   0.100,  0.100,  0.100  )
-( delta                  :   0.750,  0.400          )
-( iota                   :   0.025,  0.025,  0.025  )
-( MACHINE_ABS_ABOVE_VICE : -28.000,-10.000,-16.000  )
-( start_search           :   0.000, -2.000          )
-( start_search           :  -3.500,  0.000          )
-( start_search           :   0.000,  2.000          )
-( start_search           :   3.500,  0.000          )
-( stop_search            :   0.000, -4.000          )
-( stop_search            :   7.000,  0.000          )
-( stop_search            :  -7.000,  0.000          )
-( stop_search            :   0.000,  4.000          )
-( fast_probe             : 10.0 M79 work xyz probe  )
+( brc                    :  #102.x  #103.y             )
+( cursor                 :  #104.x  #105.y             )
+( error                  :  #106.x  #107.y             )
+( G55                    : #5241.x #5242.y #5243.z     )
+( its                    :  #106.x                     )
+( MACHINE_POS            : #5021.x #5022.y #5023.z     )
+( output                 :  #100.x  #101.y             )
+( output                 :  #102.x  #103.y             )
+( PROBE_R                :  #556.x  #557.y             )
+( SKIP_POS               : #5061.x #5062.y #5063.z     )
+( tlc                    :  #100.x  #101.y             )
+( WCS                    : #5241.x #5242.y #5243.z     )
+( amax                   :  14.000,  8.000,  3.000     )
+( amin                   :   7.000,  4.000, -5.000     )
+( backoff                :   0.100,  0.100,  0.100     )
+( delta                  :   0.750,  0.400             )
+( iota                   :   0.025,  0.025,  0.025     )
+( MACHINE_ABS_ABOVE_VICE : -28.000,-10.000,-16.000     )
+( start_search           :  -3.500,  0.000             )
+( start_search           :   0.000, -2.000             )
+( start_search           :   0.000,  2.000             )
+( start_search           :   3.500,  0.000             )
+( stop_search            :   7.000,  0.000             )
+( stop_search            :   0.000,  4.000             )
+( stop_search            :  -7.000,  0.000             )
+( stop_search            :   0.000, -4.000             )
+( fast_mabs_probe        : 10.0 M79 machine xyz probe  )
+( slow_probe             : 10.0 M79 work xyz probe     )
 
 ( Find center of plate in vice, )
 (  result in [#5241]            )
 ( Search Constraints:           )
 ( start:                        )
 (   -28.0, -13.0, -16.0         )
 ( boundary:                     )
@@ -45,30 +46,32 @@
   G103 P1
   G04 P1
   G04 P1
   G04 P1
 ( set_wcs[st.WCS]               )
   G55
 ( st.goto.machine[z=0]          )
-  G01 G90 G53 F65. z0.
+  G01 G53 G90 F65. z0.
 ( st.goto.machine.xy_then_z[sch.above])
-  G01 G90 G53 F65. x-28. y-13.
-  G01 G90 G53 F65. z-16.
+  G01 G53 G90 F65. x-28. y-13.
+  G01 G53 G90 F65. z-16.
 
 ( find top z roughly set [#5241].z. )
 ( st.WCS.xyz = MACHINE_POS.xyz  )
   #5241= #5021
   #5242= #5022
   #5243= #5023
-( st.fast_probe[z=sch.amin.z]   )
-  G01 G90 G31 M79 F10. z-5.
+( st.fast_mabs_probe[z=sch.amin.z])
+  G01 G53 G90 G31 M79 F10. z-5.
 ( st.WCS.z = MACHINE_POS.z      )
   #5243= #5023
 
-  (# 3006) = 101 ( check g55 )
+
+  (# 3006) = 101 (check g55)
+
 
 
 ( now work.z should be 0 at surface )
 ( and work.xy roughly middle        )
 ( st.goto[z=sch.skim_distance]  )
   G01 G90 F65. z0.3
 ( st.cursor = Var[2][0, 0]      )
@@ -77,43 +80,47 @@
 
 
 ( quickly move probe to find left edge )
 (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #106= 5.6667
 ( cursor[di.cur_axis] = start_search[di.cur_axis])
   #104= -3.5
+( st.goto.xy_then_z[cursor]     )
+  G01 G90 F65. x#104 y#105
 ( while its > 0:                )
-L1000
+N1000
   IF [#106 LE 0.] GOTO 1002
-(     st.goto[cursor]           )
+(     st.goto.z_then_xy[cursor] )
   G01 G90 F65. x#104 y#105
-(     st.fast_probe[z=sch.search_depth])
-  G01 G90 G31 M79 F10. z-0.1
+(     st.fast_mabs_probe[z=sch.search_depth])
+  G01 G53 G90 G31 M79 F10. z-0.1
 (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   IF [#5063 LT -0.075] GOTO 1001
 (     cursor.xy += delta        )
   #104= #104 - 0.75
 (     its -= 1                  )
   #106= #106 - 1.
   GOTO 1000
-L1002
+N1002
+
+
+  (# 3000) = 101 (search for left failed)
 
-  (# 3000) = 101 ( search for left failed )
 
 (     st.alarm[f"search for {di.name} failed"])
-L1001
+N1001
 
 ( back off a bit to the left, then slowly probe  )
 ( rightwards for precise measurement.            )
 ( cursor.xy += sch.backoff * di.dxdy)
   #104= #104 - 0.1
 ( st.goto[cursor.xy]            )
   G01 G90 F65. x#104 y#105
-( st.slow_probe[[0, 0]]         )
-  G01 G90 G31 M79 F10. x0. y0.
+( st.slow_mabs_probe[[0, 0]]    )
+  G01 G53 G90 G31 M79 F10. x0. y0.
 ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
   #100= #5061 - #556
 
 ( reposition above surface skim height, )
 ( just inside left edge                 )
 ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G91 F65. x-0.1 y0.
@@ -126,43 +133,47 @@
 
 
 ( quickly move probe to find near edge )
 (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #106= 6.
 ( cursor[di.cur_axis] = start_search[di.cur_axis])
   #105= -2.
+( st.goto.xy_then_z[cursor]     )
+  G01 G90 F65. x#104 y#105
 ( while its > 0:                )
-L1003
+N1003
   IF [#106 LE 0.] GOTO 1005
-(     st.goto[cursor]           )
+(     st.goto.z_then_xy[cursor] )
   G01 G90 F65. x#104 y#105
-(     st.fast_probe[z=sch.search_depth])
-  G01 G90 G31 M79 F10. z-0.1
+(     st.fast_mabs_probe[z=sch.search_depth])
+  G01 G53 G90 G31 M79 F10. z-0.1
 (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   IF [#5063 LT -0.075] GOTO 1004
 (     cursor.xy += delta        )
   #105= #105 - 0.4
 (     its -= 1                  )
   #106= #106 - 1.
   GOTO 1003
-L1005
+N1005
+
+
+  (# 3000) = 101 (search for near failed)
 
-  (# 3000) = 101 ( search for near failed )
 
 (     st.alarm[f"search for {di.name} failed"])
-L1004
+N1004
 
 ( back off a bit to the near, then slowly probe  )
 ( farwards for precise measurement.              )
 ( cursor.xy += sch.backoff * di.dxdy)
   #105= #105 - 0.1
 ( st.goto[cursor.xy]            )
   G01 G90 F65. x#104 y#105
-( st.slow_probe[[0, 0]]         )
-  G01 G90 G31 M79 F10. x0. y0.
+( st.slow_mabs_probe[[0, 0]]    )
+  G01 G53 G90 G31 M79 F10. x0. y0.
 ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
   #103= #5062 - #557
 
 ( reposition above surface skim height, )
 ( just inside near edge                 )
 ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G91 F65. x0. y-0.1
@@ -175,43 +186,47 @@
 
 
 ( quickly move probe to find far edge )
 (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #106= 6.
 ( cursor[di.cur_axis] = start_search[di.cur_axis])
   #105= 2.
+( st.goto.xy_then_z[cursor]     )
+  G01 G90 F65. x#104 y#105
 ( while its > 0:                )
-L1006
+N1006
   IF [#106 LE 0.] GOTO 1008
-(     st.goto[cursor]           )
+(     st.goto.z_then_xy[cursor] )
   G01 G90 F65. x#104 y#105
-(     st.fast_probe[z=sch.search_depth])
-  G01 G90 G31 M79 F10. z-0.1
+(     st.fast_mabs_probe[z=sch.search_depth])
+  G01 G53 G90 G31 M79 F10. z-0.1
 (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   IF [#5063 LT -0.075] GOTO 1007
 (     cursor.xy += delta        )
   #105= #105 + 0.4
 (     its -= 1                  )
   #106= #106 - 1.
   GOTO 1006
-L1008
+N1008
+
+
+  (# 3000) = 101 (search for far failed)
 
-  (# 3000) = 101 ( search for far failed )
 
 (     st.alarm[f"search for {di.name} failed"])
-L1007
+N1007
 
 ( back off a bit to the far, then slowly probe  )
 ( nearwards for precise measurement.            )
 ( cursor.xy += sch.backoff * di.dxdy)
   #105= #105 + 0.1
 ( st.goto[cursor.xy]            )
   G01 G90 F65. x#104 y#105
-( st.slow_probe[[0, 0]]         )
-  G01 G90 G31 M79 F10. x0. y0.
+( st.slow_mabs_probe[[0, 0]]    )
+  G01 G53 G90 G31 M79 F10. x0. y0.
 ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
   #101= #5062 + #557
 
 ( reposition above surface skim height, )
 ( just inside far edge                  )
 ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G91 F65. x0. y0.1
@@ -226,43 +241,47 @@
 
 
 ( quickly move probe to find right edge )
 (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #106= 5.6667
 ( cursor[di.cur_axis] = start_search[di.cur_axis])
   #104= 3.5
+( st.goto.xy_then_z[cursor]     )
+  G01 G90 F65. x#104 y#105
 ( while its > 0:                )
-L1009
+N1009
   IF [#106 LE 0.] GOTO 1011
-(     st.goto[cursor]           )
+(     st.goto.z_then_xy[cursor] )
   G01 G90 F65. x#104 y#105
-(     st.fast_probe[z=sch.search_depth])
-  G01 G90 G31 M79 F10. z-0.1
+(     st.fast_mabs_probe[z=sch.search_depth])
+  G01 G53 G90 G31 M79 F10. z-0.1
 (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   IF [#5063 LT -0.075] GOTO 1010
 (     cursor.xy += delta        )
   #104= #104 + 0.75
 (     its -= 1                  )
   #106= #106 - 1.
   GOTO 1009
-L1011
+N1011
+
+
+  (# 3000) = 101 (search for right failed)
 
-  (# 3000) = 101 ( search for right failed )
 
 (     st.alarm[f"search for {di.name} failed"])
-L1010
+N1010
 
 ( back off a bit to the right, then slowly probe  )
 ( leftwards for precise measurement.              )
 ( cursor.xy += sch.backoff * di.dxdy)
   #104= #104 + 0.1
 ( st.goto[cursor.xy]            )
   G01 G90 F65. x#104 y#105
-( st.slow_probe[[0, 0]]         )
-  G01 G90 G31 M79 F10. x0. y0.
+( st.slow_mabs_probe[[0, 0]]    )
+  G01 G53 G90 G31 M79 F10. x0. y0.
 ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
   #102= #5061 + #556
 
 ( reposition above surface skim height, )
 ( just inside right edge                )
 ( st.goto.relative[sch.backoff.xy * di.dxdy])
   G01 G91 F65. x0.1 y0.
@@ -287,10 +306,12 @@
 
 (  final slow probe to find the surface z )
 ( st.slow_probe[z=sch.search_depth])
   G01 G90 G31 M79 F10. z-0.1
 ( st.WCS.z = SKIP_POS.z         )
   #5243= #5063
 ( st.goto.machine[z=sch.above.z])
-  G01 G90 G53 F65. z-16.
+  G01 G53 G90 F65. z-16.
+
+
+  (# 3000) = 101 ( what changed)
 
-  (# 3000) = 101 (  what changed )
```

### Comparing `p2g-0.2.4/p2g/tests/test_axes.py` & `p2g-0.2.5/p2g/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_basic.py` & `p2g-0.2.5/p2g/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_builtins.py` & `p2g-0.2.5/p2g/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_coords.py` & `p2g-0.2.5/p2g/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_error.py` & `p2g-0.2.5/p2g/tests/test_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,34 +15,24 @@
 
 
 def fish():
     PROBE.x = 9
 
 
 @pytest.mark.xfail
-@p2g.must_be_cc(
+@p2g.must_be(
     "( PROBE.x = 9                   )",
     " error  #5061= 9.",
     '(  "quote escape" )',
 )
 def test_forcefail():
     PROBE.x = 9
     p2g.com(' "quote escape"')
 
 
-@p2g.must_be_cc(
-    "( PROBE.x = 9                   )",
-    "  #5061= 9.",
-    '(  "quote escape" )',
-)
-def test_quoteok0():
-    PROBE.x = 9
-    p2g.com(' "quote escape"')
-
-
 @p2g.must_be(
     "Can only take address of something with location.",
     "p2g/tests/test_error.py:7:20:21:     f = p2g.address(9)",
     "                                                     ^",
 )
 def test_cerror_addressof0():
     f = p2g.address(9)
```

### Comparing `p2g-0.2.4/p2g/tests/test_example.py` & `p2g-0.2.5/p2g/tests/test_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 # isort: skip_file
 # sys.path.insert(0, "./examples")
 # ys.path.insert(0, "..")
 # sys.path.insert(0, ".")
 # sys.path.insert(0, "../..")
-sys.path.insert(0, "./p2g/examples")
+# sys.path.insert(0, "./p2g/examples")
 # import examples
 # import examples.probecalibrate
 # import examples.vicecenter
 import p2g.examples.probecalibrate
 import p2g.examples.vicecenter
```

### Comparing `p2g-0.2.4/p2g/tests/test_expr.py` & `p2g-0.2.5/p2g/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_for.py` & `p2g-0.2.5/p2g/tests/test_for.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from p2g import *
 
 
 @must_be(
     "( for i in range[10]:           )",
     "  #101= 0.",
-    "L1000",
+    "N1000",
     "  IF [#101 GE 10.] GOTO 1002",
     "DPRNT[got*[#101]]",
     '(     dprint[f"got {i}"]        )',
     "  #101= #101 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
 )
 def test_for0():
     for i in range(10):
         dprint(f"got {i}")
 
 
 @must_be(
@@ -28,20 +28,20 @@
         dprint(f"got {i.var}")
 
 
 @must_be(
     "( fish )",
     "( for x in range[1, 20]:        )",
     "  #102= 1.",
-    "L1000",
+    "N1000",
     "  IF [#102 GE 20.] GOTO 1002",
     "(     pass                      )",
     "  #102= #102 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
 )
 def test_for2():
     x = Var()
     com("fish")
     for x in range(1, 20):
         pass
 
@@ -52,21 +52,21 @@
     "  #101= 2.",
     "  #102= 3.",
     "  #103= 4.",
     "( j = Var[0]                    )",
     "  #104= 0.",
     "( for v in x:                   )",
     "  #105= 100.",
-    "L1000",
+    "N1000",
     "  IF [#105 GE 104.] GOTO 1002",
     "(     j += v                    )",
     "  #104= #104 + #[#105]",
     "  #105= #105 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
 )
 def test_for4():
     x = Var(1, 2, 3, 4)
     j = Var(0)
     for v in x:
         j += v
```

### Comparing `p2g-0.2.4/p2g/tests/test_func.py` & `p2g-0.2.5/p2g/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_goto.py` & `p2g-0.2.5/p2g/tests/test_goto.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,36 +7,53 @@
     "                                                        ^",
 )
 def test_cerror_no_feed():
     p2g.goto.work(1, 2, 3)
 
 
 @p2g.must_be(
-    "( m.relative[1, 2]              )",
-    "  G01 G91 F20. x1. y2.        ",
-    "( GotoWorker[want_bp_=False, space_=<MovementSpace.WORK: 1>, feed_=20, order_=<MovementOrder.XYZ: 1>, probe_=False, mcode_=''] )",
+    "( mgoto.relative[1, 2]          )",
+    "  G01 G91 F20. x1. y2.",
 )
 def test_goto_rel():
     mgoto = p2g.goto.feed(20)
     mgoto.relative(1, 2)
     p2g.comment(mgoto)
 
 
 @p2g.must_be(
+    "( mgoto[1, 2]                   )",
+    "  G01 G90 F20. x1. y2.",
+    "( mgoto[1, 3]                   )",
+    "  G01 G90 F20. x1. y3.",
+    "( mgoto[3, 4]                   )",
+    "  G01 G91 F20. x3. y4.",
+)
+def test_goto_abs():
+    mgoto = p2g.goto.absolute.feed(20)
+    mgoto(1, 2)
+    mgoto(1, 3)
+    xgoto = mgoto.relative
+    xgoto(3, 4)
+
+    p2g.comment(mgoto)
+
+
+@p2g.must_be(
     "( p2.feed[12].z_then_xy[1, 2, 3])",
     "  G01 G90 F12. z3.            ",
     "  G01 G90 F12. x1. y2.",
 )
 def test_order0():
     p2g.goto.feed(12).z_then_xy(1, 2, 3)
 
 
 @p2g.must_be(
-    "( p2.xy_then_z.feed[9].relative[1, 2, 3])",
-    "  G01 G91 F9. x1. y2.         ",
+    "( goto.xy_then_z.feed[9].relative[1, 2, 3])",
+    "  G01 G91 F9. x1. y2.",
     "  G01 G91 F9. z3.",
 )
 def test_order1():
     p2g.goto.xy_then_z.feed(9).relative(1, 2, 3)
 
 
 @p2g.must_be(
@@ -71,12 +88,55 @@
 )
 def test_probe1():
     p2g.goto.feed(123).z_then_xy(1, 2, 3)
 
 
 @p2g.must_be(
     "( goto.r9810.feed[7].z_then_xy[1, 2, 3])",
-    "  G01 G65 R9810 F7. z3.",
-    "  G01 G65 R9810 F7. x1. y2.",
+    "  G65 R9810 F7. z3.",
+    "  G65 R9810 F7. x1. y2.",
 )
 def test_safemove():
     p2g.goto.r9810.feed(7).z_then_xy(1, 2, 3)
+
+
+@p2g.must_be(
+    "( mgoto.relative[1, 2]          )",
+    "  G01 G91 F20. x1. y2.",
+    "( mgoto[3, 4]                   )",
+    "  G01 G90 F20. x3. y4.",
+    "  G01 G91 F20. x3. y4.",
+)
+def test_goto_rel_and_change():
+    mgoto = p2g.goto.feed(20)
+    mgoto.relative(1, 2)
+    mgoto = mgoto.absolute
+    mgoto(3, 4)
+    mgoto = mgoto.relative
+    mgoto(3, 4)
+
+
+@p2g.must_be(
+    "Relative with 9810 move is illegal.",
+    "p2g/tests/test_goto.py:7:52:53:     p2g.goto.r9810.feed(7).relative.z_then_xy(1, 2, 3)",
+    "                                                                                    ^",
+)
+def test_cerror_9810_1():
+    p2g.goto.r9810.feed(7).relative.z_then_xy(1, 2, 3)
+
+
+@p2g.must_be(
+    "Probe with 9810 move is illegal.",
+    "p2g/tests/test_goto.py:7:49:50:     p2g.goto.r9810.feed(7).probe.z_then_xy(1, 2, 3)",
+    "                                                                                 ^",
+)
+def test_cerror_9810_2():
+    p2g.goto.r9810.feed(7).probe.z_then_xy(1, 2, 3)
+
+
+@p2g.must_be(
+    "MCODE with 9810 move is illegal.",
+    'p2g/tests/test_goto.py:7:54:55:     p2g.goto.r9810.feed(7).mcode("a").z_then_xy(1, 2, 3)',
+    "                                                                                      ^",
+)
+def test_cerror_9810_3():
+    p2g.goto.r9810.feed(7).mcode("a").z_then_xy(1, 2, 3)
```

### Comparing `p2g-0.2.4/p2g/tests/test_interp.py` & `p2g-0.2.5/p2g/tests/test_interp.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,36 @@
 V = p2g.Fixed[10](addr=200)
 
 
 def decor(fn):
     return fn
 
 
+@p2g.must_be(
+    "(     V[1] = 12                 )",
+    "  #201= 12.",
+)
+def test_shortcut_if0():
+    if 0:
+        V[0] = 7
+    else:
+        V[1] = 12
+
+
+@p2g.must_be(
+    "(     V[0] = 7                  )",
+    "  #200= 7.",
+)
+def test_shortcut_if1():
+    if 1:
+        V[0] = 7
+    else:
+        V[1] = 12
+
+
 @decor
 class F:
     def __init__(self):
         pass
 
 
 @p2g.must_be(
@@ -32,25 +54,25 @@
     r = 1 or 2 or 3
     r = 3 and 9
     V[0] = r
 
 
 @p2g.must_be(
     "( while V[0] < 10:              )",
-    "L1000                         ",
+    "N1000                         ",
     "  IF [#200 GE 10.] GOTO 1002",
     "(     V[0] += 1                 )",
     "  #200= #200 + 1.             ",
     "(     break                     )",
     "  GOTO 1001                   ",
     "(     V[1] += 9                 )",
     "  #201= #201 + 9.             ",
     "  GOTO 1000",
-    "L1001",
-    "L1002",
+    "N1001",
+    "N1002",
     "( V[2] = 7                      )",
     "  #202= 7.                    ",
 )
 def test_break():
     while V[0] < 10:
         V[0] += 1
         break
@@ -92,24 +114,24 @@
 def test_cerror_with():
     with foo():
         V[0] = 1
 
 
 @p2g.must_be(
     "( while V[0] < 10:              )",
-    "L1000                         ",
+    "N1000                         ",
     "  IF [#200 GE 10.] GOTO 1002",
     "(     V[0] += 1                 )",
     "  #200= #200 + 1.             ",
     "(     continue                  )",
     "  GOTO 1000                   ",
     "(     V[1] += 9                 )",
     "  #201= #201 + 9.             ",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
     "( V[2] = 7                      )",
     "  #202= 7.                    ",
 )
 def test_continue():
     while V[0] < 10:
         V[0] += 1
         continue
@@ -175,19 +197,19 @@
     "( if PROBE.x > 9:               )",
     "  IF [#5061 LE 9.] GOTO 1000  ",
     "(     if PROBE.y > 10:          )",
     "  IF [#5062 LE 10.] GOTO 1002 ",
     "(         V[0] = 3              )",
     "  #200= 3.                    ",
     "  GOTO 1003",
-    "L1002",
-    "L1003",
+    "N1002",
+    "N1003",
     "  GOTO 1001",
-    "L1000",
-    "L1001",
+    "N1000",
+    "N1001",
 )
 def test_ifs():
     if PROBE.x > 9:
         if PROBE.y > 10:
             V[0] = 3
 
 
@@ -285,25 +307,25 @@
 def test_set():
     r = {1, 2, 3}
     V[0] = len(r)
 
 
 @p2g.must_be(
     "( while V[0] < 10:              )",
-    "L1000                         ",
+    "N1000                         ",
     "  IF [#200 GE 10.] GOTO 1002",
     "(     if V[2]:                  )",
     "  IF [#202] GOTO 1001         ",
     "(     V[0] += 1                 )",
     "  #200= #200 + 1.             ",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
     "(     V[1] = 10                 )",
     "  #201= 10.                   ",
-    "L1001",
+    "N1001",
     "( V[2] = 123                    )",
     "  #202= 123.                  ",
 )
 def test_while():
     while V[0] < 10:
         if V[2]:
             break
```

### Comparing `p2g-0.2.4/p2g/tests/test_linenos.py` & `p2g-0.2.5/p2g/tests/test_linenos.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_main.py` & `p2g-0.2.5/p2g/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     got = capfd.readouterr()
     assert "Version: p2g" in got.out
 
 
 def write_func(test_file):
     test_file.write_text(
         "import p2g\n"
-        "def test():\n"
+        "def testfish():\n"
         "      X=p2g.Fixed[1](123,addr=200)\n"
         "      X=p2g.Fixed[7](1,2,3,4,5,6,7,addr=300)\n",
         encoding="utf-8",
     )
 
 
 def test_native_job_tmpdir(tmpdir):
@@ -101,15 +101,24 @@
         ]
     )
     tfun = capfd.readouterr()
     assert "No such function" in tfun.err
 
 
 def test_native_cli_tmpdir_examples(tmpdir):
-    p2g.main(["--outdir", tmpdir, "-q", "examples"])
+    p2g.main(["--outdir", tmpdir, "examples"])
+
+
+def test_native_stdin():
+    p2g.main(
+        [
+            "--debug",
+            "gen",
+        ]
+    )
 
 
 def test_native_capfd_tmpdir_stdout(capfd, tmpdir):
     tmpfile = tmpdir / "test.py"
     write_func(tmpfile)
     p2g.main(
         [
@@ -118,14 +127,15 @@
             "--job=O123",
             str(tmpfile),
             f"--out=-",
         ]
     )
     tmpdata = capfd.readouterr()
     assert "O123" in tmpdata.out
+    assert "testfish" in tmpdata.out
 
 
 def test_native_fake_capture0():
     with p2g.lib.CaptureO(0) as x:
         print("HI")
     assert x.out.startswith("HI")
 
@@ -139,15 +149,15 @@
 def test_native_fake_capture2():
     with p2g.lib.CaptureO(0) as x:
         print("HI")
         assert x.readouterr().out.startswith("HI")
 
 
 def test_native_logger_capfd_setup(capfd):
-    p2g.main(["--recursive", "--logfile=-", "--loglevel=INFO", "version"])
+    p2g.main(["--recursive", "--debug", "version"])
     got = capfd.readouterr()
     assert "Version:" in got.out
 
 
 # @pytest.mark.skip
 # def test_typeguard_setup():
 #     assert "typeguard" in sys.modules.keys()
```

### Comparing `p2g-0.2.4/p2g/tests/test_makestdvars.py` & `p2g-0.2.5/p2g/tests/test_makestdvars.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_meta.py` & `p2g-0.2.5/p2g/tests/test_meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,64 +5,60 @@
 
 # make sure the testing is working.
 import pytest
 
 import p2g
 
 
-this_path = pathlib.Path(__file__)
-golden_dir = this_path.parent / "golden"
-
-# gold file is there, but broken.
-# check creation of got file.
-
-simple_xfail1_got = golden_dir / "test_simple_xfail1.got"
-simple_xfail1_nc = golden_dir / "test_simple_xfail1.nc"
-
-
-@p2g.check_golden()
-@pytest.mark.xfail()
-def test_simple_xfail1():
-    simple_xfail1_nc.write_text("fail")
-    p2g.com("A comment")
-    CURSOR = p2g.Fixed(addr=100)
-    CURSOR.x = 9
-
-
-def test_native_check_and_remove_golden():
-    assert simple_xfail1_got.read_text() == (
-        "( A comment )\n( CURSOR.x = 9                  )\n  #100= 9."
-    )
-    simple_xfail1_nc.unlink()
-    simple_xfail1_got.unlink()
-
-
-p2g.must_be("err")
-
-
+@p2g.must_be()
 def test_simple_ok():
     print("WORKING")
     a = 3
 
 
+this_path = pathlib.Path(__file__)
+golden_dir = this_path.parent / "golden"
+
+
 # simple fn to output to stdout
 def tolist_worker():
     p2g.Fixed(2, addr=100)
 
 
 # two phases 'cause fixtures don't work on interp functions.
 def test_native_tolist():
     got = p2g.walk.compile2g("tolist_worker", __file__, job_name=None, in_pytest=True)
 
     r = "#100" in got[1]
     assert r
 
 
+# # gold file is there, but broken.
+# meta_make_bad_gold_path = golden_dir / "test_meta_test_native_simple_xfail1.nc"
+
+
+# def make_bad_gold():
+#     meta_make_bad_gold_path.write_text("fail")
+
+
+# @p2g.check_golden()
+# @pytest.mark.xfail()
+# def test_native_simple_xfail1():
+#     p2g.com("A comment")
+#     CURSOR = p2g.Fixed(addr=100)
+#     CURSOR.x = 9
+
+
+# def test_native_check_and_remove_golden():
+#     assert "A comment" in meta_make_bad_gold_path.read_text()
+#     meta_make_bad_gold_path.unlink()
+
+
 # test what happens when file is no there.
-make_golden_path = golden_dir / "test_native_transitory_golden.nc"
+make_golden_path = golden_dir / "test_meta_test_native_transitory_golden.nc"
 
 
 # output file not there, so test fails,
 # but file is created
 @p2g.check_golden()
 def test_native_transitory_golden():
     CURSOR = p2g.Fixed(addr=100)
@@ -71,37 +67,58 @@
 
 # # so can be tested here.
 def test_native_golden_exists():
     assert make_golden_path.exists()
     make_golden_path.unlink()
 
 
-meta_decorate_seed = golden_dir / "test_decorate_seed.decorator"
+gold_compare_fail = golden_dir / "test_meta_test_native_gold_compare_fail.nc"
+# test when there is a file but its wrong.
+
+
+@p2g.check_golden()
+@pytest.mark.xfail
+def test_native_gold_compare_fail():
+    # not going to match.
+    gold_compare_fail.write_text("BAD")
+
+
+@p2g.must_be()
+def test_cleanup():
+    gold_compare_fail.unlink()
+
+
+meta_decorate_seed = golden_dir / "test_meta_test_decorate_seed.decorator"
 
 
 def test_native_remove_seed():
     meta_decorate_seed.unlink(missing_ok=True)
     assert not meta_decorate_seed.exists()
 
 
 # the force inserts an error  in the output
 # so the test fails, but generates them
 # error output.
 
-meta_decorator_path = golden_dir / "test_native_decorate_seed.decorator"
+meta_decorator_path = golden_dir / "test_meta_test_native_decorate_seed.decorator"
 
 
 @p2g.must_be("FORCE")
 def test_native_decorate_seed():
     CURSOR = p2g.Fixed(17, addr=100)
 
 
 def test_native_seed_exists():
     print("GOT ", meta_decorate_seed)
     assert meta_decorator_path.exists()
     meta_decorator_path.unlink()
 
 
+@pytest.mark.xfail
+def test_forcefail():
+    fish = pop
+
+
 #    assert False
 
 
 # expected fail        test_broken()
```

### Comparing `p2g-0.2.4/p2g/tests/test_nt1.py` & `p2g-0.2.5/p2g/tests/test_nt1.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_op.py` & `p2g-0.2.5/p2g/tests/test_op.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_smoke.py` & `p2g-0.2.5/p2g/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_str.py` & `p2g-0.2.5/p2g/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_symtab.py` & `p2g-0.2.5/p2g/tests/test_symtab.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_tuple.py` & `p2g-0.2.5/p2g/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_vars.py` & `p2g-0.2.5/p2g/tests/test_vars.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/tests/test_vector.py` & `p2g-0.2.5/p2g/tests/test_vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     "  #41= 2.",
     "  #42= 3.14",
     "  #43= 4.",
     "  #44= 5.",
     "  #45= 6.",
     "( for j in range[3]:            )",
     "  #109= 0.",
-    "L1000",
+    "N1000",
     "  IF [#109 GE 3.] GOTO 1002",
     "(     ptr[j.var + 2] = [j + 2] ** 2 + 17)",
     "  #[#109 + 402]= POW[#109 + 2.,2.] + 17.",
     "  #109= #109 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
 )
 def test_const_deref_addresses():
     st = add_some_symbols()
     ptrb = st.txyz
 
     idx = p2g.Fixed(
         150,
@@ -218,39 +218,39 @@
     fish = p2g.Fixed(addr=300)
     fish.var = nw[idx // 1]
 
 
 @p2g.must_be(
     "( for j in range[7, 10]:        )",
     "  #102= 7.",
-    "L1000",
+    "N1000",
     "  IF [#102 GE 10.] GOTO 1002",
     "(     ptr[j] = 12               )",
     "  #[#102 + 300]= 12.",
     "  #102= #102 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
     "( for j in range[7, 10]:        )",
     "  #112= 7.",
-    "L1003",
+    "N1003",
     "  IF [#112 GE 10.] GOTO 1005",
     "(     ptr[j] = j                )",
     "  #[#112 + 300]= #112",
     "  #112= #112 + 1.",
     "  GOTO 1003",
-    "L1005",
+    "N1005",
     "( for j in range[2, 7]:         )",
     "  #114= 2.",
-    "L1006",
+    "N1006",
     "  IF [#114 GE 7.] GOTO 1008",
     "(     ptr[j] = [j + 2] ** 2 + 17)",
     "  #[#114 + 300]= POW[#114 + 2.,2.] + 17.",
     "  #114= #114 + 1.",
     "  GOTO 1006",
-    "L1008",
+    "N1008",
 )
 def test_var_deref_addresses():
     j = p2g.Var()
 
     ptr = p2g.Fixed[10](addr=300)
 
     for j in range(7, 10):
@@ -350,27 +350,27 @@
 
 
 @p2g.must_be(
     "( mx = Var[flutes[0]]           )",
     "  #101= #200",
     "( for i in flutes[1:]:          )",
     "  #102= 201.",
-    "L1000",
+    "N1000",
     "  IF [#102 GE 210.] GOTO 1002",
     "  #100= #[#102]",
     "(     if i > mx:                )",
     "  IF [#100 LE #101] GOTO 1003",
     "(         mx = i                )",
     "  #101= #100",
     "  GOTO 1004",
-    "L1003",
-    "L1004",
+    "N1003",
+    "N1004",
     "  #102= #102 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
 )
 def test_find_flutes():
     i = p2g.Var()
     flutes = p2g.Fixed[10](addr=200)
     mx = p2g.Var(flutes[0])
     for i in flutes[1:]:
         if i > mx:
@@ -386,21 +386,21 @@
 
 
 @p2g.must_be(
     "( mx = Var[TOOL_TBL_FLUTES[0]]  )",
     "  #100= #300",
     "( for i in TOOL_TBL_FLUTES[1:]: )",
     "  #101= 301.",
-    "L1000",
+    "N1000",
     "  IF [#101 GE 400.] GOTO 1002",
     "(     mx = max[mx, i]           )",
     "  #100= #100 * [#100 GT #[#101]] + #[#101] * [#100 LE #[#101]]",
     "  #101= #101 + 1.",
     "  GOTO 1000",
-    "L1002",
+    "N1002",
     "( MESSAGE.var = mx              )",
     "  #3006= #100",
 )
 def test_find_max_way2():
     # stop with alarm code as max # flutes in table.
 
     mx = p2g.Var(TOOL_TBL_FLUTES[0])
```

### Comparing `p2g-0.2.4/p2g/thanksto` & `p2g-0.2.5/p2g/thanksto`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/vector.py` & `p2g-0.2.5/p2g/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     def nelements(self):
         return int(self._size)
 
     def everything(self):
         return (
             self.get_at(scalar.wrap_scalar(idx))
-            for idx in scalar.urange(0, self._size, self._step)
+            for idx in scalar.urange(0, self._size, int(self._step))
         )
 
     def get_at(self, idx: scalar.Scalar):
         if isinstance(idx, scalar.Constant):
             fidx = int(idx)
             if not 0 <= fidx < int(self._size):
                 err.compiler(
@@ -193,18 +193,18 @@
 
     def get_slice(self, index: slice):
         tmp = (list(range(self.nelements())))[index]
         step = 0
         if len(tmp) > 1:
             step = tmp[1] - tmp[0]
 
-        first = int(self._addr) + tmp[0]
+        addr = self._addr + tmp[0]
         size = tmp[-1] - tmp[0] + 1
-        step = int(step)
-        return MemVec(first, size, step)
+        assert addr is not None
+        return MemVec(addr, size, step)
 
     def __setitem__(self, indexes, src):
         if isinstance(indexes, slice):
             indexes = list(range(*indexes.indices(self.nelements())))
         indexes = wrap_maybe_vec(indexes)
         src = wrap_maybe_vec(src)
         for idx, sel in zip(indexes.everything(), src.forever()):
```

### Comparing `p2g-0.2.4/p2g/visible.py` & `p2g-0.2.5/p2g/visible.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     #    ._wcs = (val._addr - 5221) // 20 + 54
     if new_base is not None:
         gbl.iface.ebss = new_base
     return gbl.iface.ebss
 
 
 def message(dst, txt: str):
-    stat.code(f"{dst[0]} = 101 ( {txt} )", "<no comment>")
+    stat.code(f"{dst[0]} = 101 ({txt})", comment_txt="<none>")
 
 
 def as_address(src):
     return src
 
 
 def address(src):
```

### Comparing `p2g-0.2.4/p2g/walk.py` & `p2g-0.2.5/p2g/walk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import abc
 import ast
 import dataclasses
 import pathlib
 import re
 import sys
-import typing
-
-from loguru import logger
 
 from p2g import axis
 from p2g import coords
 from p2g import err
 from p2g import gbl
 from p2g import lib
+from p2g import nd
 from p2g import op
 from p2g import scalar
 from p2g import stat
 from p2g import symbol
 from p2g import vector
 from p2g import walkbase
 from p2g import walkexpr
@@ -33,23 +31,20 @@
         next(src_gen)
         err.compiler("Too many values to unpack.")
 
     except StopIteration:
         pass
 
 
-# pytype seems wrong?
-
-
 def handle_assign(self, target, val):
     if not isinstance(target, ast.Tuple):
         self.visit_store(target, val)
         return
 
-    src_gen = iter(val)  # pytype: disable=wrong-arg-types
+    src_gen = iter(val)
     try:
         for dst_idx, dst_el in enumerate(target.elts):
             if isinstance(dst_el, ast.Starred):
                 src_togo = list(src_gen)
                 break_i = len(src_togo) - (len(target.elts) - dst_idx - 1)
                 self.visit_store(dst_el.value, src_togo[:break_i])
                 src_gen = iter(src_togo[break_i:])
@@ -140,15 +135,15 @@
                 op.make_scalar_add(scalar.wrap_scalar(self.var), self.rang.step),
             )
         )
 
 
 @dataclasses.dataclass
 class ItrSlice:
-    ptr: typing.Any
+    ptr: nd.EBase
     pastptr: scalar.Scalar
     step: scalar.Scalar
     var: ast.AST
 
     def __init__(self, itr, interp, target):
         self.interp = interp
         self.target = target
@@ -296,29 +291,40 @@
         stat.add_stat(stat.Goto(self.loop.lbreak))
 
     def _visit_continue(self, _):
         stat.add_stat(stat.Goto(self.loop.lcontinue))
 
     def _visit_if(self, node):
         #   for nicer looking code
+        # for a conditional break.
         if isinstance(node.body[0], ast.Break):
             exp = op.make_scalar_unop(op.a2opfo(ast.UAdd), self.visit(node.test))
             self.loop.lbreak.used = True
             stat.add_stat(stat.If(exp, self.loop.lbreak))
             return
 
         elsepart = stat.next_label()
         donepart = stat.next_label()
-        exp1 = op.make_scalar_unop(op.a2opfo(ast.Not), self.visit(node.test))
-        stat.add_stat(stat.If(exp1, on_t=elsepart))
-        self.visit_slist(node.body)
-        stat.add_stat(stat.Goto(donepart))
-        stat.add_stat(stat.LabelDef(elsepart))
-        self.visit_slist(node.orelse)
-        stat.add_stat(stat.LabelDef(donepart))
+
+        cond = op.make_scalar_unop(op.a2opfo(ast.UAdd), self.visit(node.test))
+
+        # nice code for if with constant.
+        if cond.is_constant:
+            if cond:
+                self.visit_slist(node.body)
+            else:
+                self.visit_slist(node.orelse)
+        else:
+            exp1 = op.make_scalar_unop(op.a2opfo(ast.Not), cond)
+            stat.add_stat(stat.If(exp1, on_t=elsepart))
+            self.visit_slist(node.body)
+            stat.add_stat(stat.Goto(donepart))
+            stat.add_stat(stat.LabelDef(elsepart))
+            self.visit_slist(node.orelse)
+            stat.add_stat(stat.LabelDef(donepart))
 
     def _visit_import(self, node):
         for n in node.names:
             self.ns[n.asname or n.name] = __import__(n.name)
 
     def _visit_importfrom(self, node):
         mod = __import__(
@@ -398,53 +404,42 @@
         return func_name_arg
     function_to_call = "no function in file"
     for fname in find_defined_funcs(sourcelines):
         function_to_call = fname
     return function_to_call
 
 
-def compile2g_(func_name_arg, srcfile_name, job_name, in_pytest, args=None):
+@lib.g2l
+def compile2g(func_name_arg, srcfile_name, job_name, in_pytest, args=None):
     gbl.config.in_pytest = in_pytest
 
     srcpath = pathlib.Path(srcfile_name)
 
     with lib.openr(srcpath) as inf:
         sys.path.insert(0, str(srcpath.parent))
 
         with stat.Nest(in_pytest) as cursor:
             axis.NAMES = "xyz"
             gbl.iface.reset()
 
             symbol.Table.reset()
 
-            logger.debug(f"Starting {func_name_arg} {cursor.next_label}")
-            sourcelines = inf.read()
+            lib.log(f"Starting {func_name_arg} {cursor.next_label}")
+            sourcelines = lib.logread(inf)
             node = ast.parse(sourcelines)
             # load everything
             walker = compile_all(node, srcfile_name)
+
             if node.body:
                 walkfunc.digest_top(
                     walker,
                     find_main_func_name(sourcelines, func_name_arg),
                     srcpath,
                     job_name,
                     args,
                 )
             # can't use generator 'cause need
             # mods to varrefs for symbol table
             res = list(cursor.to_full_lines())
 
             yield from symbol.Table.yield_lines()
             yield from res
-
-
-compile2g = lib.g2l(compile2g_)
-
-# class WantInline:
-#     def __init__(self, fn):
-#         self.fn = fn
-
-
-# # at definition of an inline function,
-# # just remember the tree name.
-# def inline(fn):
-#     return WantInline(fn)
```

### Comparing `p2g-0.2.4/p2g/walkbase.py` & `p2g-0.2.5/p2g/walkbase.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/walkexpr.py` & `p2g-0.2.5/p2g/walkexpr.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.4/p2g/walkfunc.py` & `p2g-0.2.5/p2g/walkfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     walker.func_name = func_def.func_name
 
     # We need to switch from dynamic execution scope to lexical scope
     # in which function was defined (then switch back on return).
     dyna_scope = walker.ns
     walker.ns = func_def.lexical_scope
     res = None
+
     with walker.pushpopns(walkns.FunctionNS()):
         formals_dict = gather_func_formals(func_def, *args, **kwargs)
 
         walker.ns.guts.update(formals_dict)
 
         res = walker.visit_slist(func_def.node.body)
 
@@ -139,19 +140,18 @@
     call: bool
 
     gen: list[stat.StatBase]
 
     def __init__(self, walker, node):
         self.call = False
         self.gen = []
-        for decorator in node.decorator_list:
-            walker.visit(decorator)
+        self.func_name = node.name
 
         self.file_name = walker.module_ns["__file__"]
-        self.func_name = node.name
+
         self.node = node
         self.walker = walker
         self.lexical_scope = walker.ns
 
     def __call__(self, *args, **kwargs):
         return inline(self, *args, **kwargs)
 
@@ -185,26 +185,29 @@
                 kwargs.update(val)
             else:
                 kwargs[keyword.arg] = val
         self.args = args
         self.kwargs = kwargs
 
 
+def funcall(target, *args, **kwargs):
+    return target(*args, **kwargs)
+
+
 class WalkFunc(walkbase.WalkBase):
     def _visit_call(self, node):
         defn = self.visit(node.func)
         desc = FuncArgsDescr(self, node)
         if defn.__module__ == "p2g.builtin":
             return op.make_scalar_func(defn.__name__, *desc.args)
 
         #        return desc.callit(*desc.args, **desc.kwargs)
         # f = interpfunc(desc.func)
         # return f
-
-        return defn(*desc.args, **desc.kwargs)
+        return funcall(defn, *desc.args, **desc.kwargs)
 
     def _visit_functiondef(self, node):
         desc = FuncDefWrap(self, node)
         #        self.funcmaps[node.name] = desc
         ifunc = interpfunc(desc)
         self.ns[node.name] = ifunc
 
@@ -215,19 +218,19 @@
     try:
         fncdef = walker.ns[func_name]
         desc = fncdef(Marker())
     except KeyError:
         err.compiler(f"No such function '{func_name}' in '{srcpath}'.")
 
     if not gbl.config.in_pytest:
-        stat.add_stat(stat.Code(job_name, srcpath.stem.upper()))
+        stat.code([job_name], comment_txt=func_name)
 
     if gbl.config.bp_on_error:  # no cover
         inline(desc, *args)
     else:
         try:
             inline(desc, *args)
         except (AttributeError, IndexError) as exn:
             err.compiler(exn)
 
     if not gbl.config.in_pytest:
-        stat.add_stat(stat.Code("M30", None))
+        stat.add_stat(stat.Code("M30", "<none>"))
```

### Comparing `p2g-0.2.4/p2g/walkns.py` & `p2g-0.2.5/p2g/walkns.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,23 +66,14 @@
     while ns:
         if not isinstance(ns, ClassNS):
             yield ns
 
         ns = ns.parent
 
 
-def find_ns(first_ns, nid):
-    for ns in scan_namespaces(first_ns):
-        res = ns.get(nid)
-        if res is UNDEF:
-            continue
-        return res, ns
-    return UNDEF, None
-
-
 def resolve_nonlocal(name, ns):
     while ns:
         res = ns.get(name)
         if res is not UNDEF and res is not NONLOCAL:
             if isinstance(ns, ModuleNS):
                 break
             return ns
@@ -97,29 +88,37 @@
     elif res is NONLOCAL:
         dstns = resolve_nonlocal(nid, self.ns.parent)
     else:
         dstns = self.ns
     return dstns
 
 
+def find_ns(first_ns, nid):
+    for ns in scan_namespaces(first_ns):
+        res = ns.get(nid)
+        if res is UNDEF:
+            continue
+        return res, ns
+    return UNDEF, None
+
+
 def _handle_visit_name_load(self, node):
     res, ns = find_ns(self.ns, node.id)
-
     if ns is None:
         try:
             return getattr(builtins, node.id)
         except AttributeError:
             err.compiler(f"{node.id} is not defined.")
 
     if res is GLOBAL:
         res = self.module_ns.get(node.id)
     elif res is NONLOCAL:
         ns = resolve_nonlocal(node.id, ns.parent)
         res = ns[node.id]
-
+    assert res is not UNDEF
     symbol.Table.remember_load(node.id, res)
     return res
 
 
 def handle_visit_name_del(self, node):
     res = self.ns.get(node.id)
     if res is UNDEF:
```

### Comparing `p2g-0.2.4/pyproject.toml` & `p2g-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 
 
 
 name = "p2g"
-version = "0.2.4"
+version = "0.2.5"
 description = "Transpile python into cnc gcode."
 authors = ["sac <sac@0x5ac.com>"]
 readme = "README.rst"
 license = "MIT"
 keywords = ["cnc", "gcode", "mill", "haas"]
 classifiers = [
 "Development Status :: 3 - Alpha",
@@ -26,18 +26,18 @@
 ]
 
 
 [tool.poetry.dependencies]
 
 python = "^3.10"
 docopt = "^0.6.2"
-pytest =  "^7.3.1"
+
 typeguard = "^3.0.2"
 rich = "^13.3.4"
-loguru = "^0.7.0"
+
 [tool.poetry.scripts]
 p2g = "p2g.main:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = {extras = ["all"], version = "^7.3.1"}
 pytest-cov = "^4.0.0"
 coverage = "^7.2.3"
@@ -51,19 +51,27 @@
 ssort = "^0.11.6"
 tox = "^4.5.1"
 deptry = "^0.8.0"
 mccabe = "^0.7.0"
 wrapt = "^1.15.0"
 dill = "^0.3.6"
 autoflake = "^2.1.1"
+ruff = "^0.0.272"
+pyright = "^1.1.314"
 
+[tool.deptry]
+ignore_missing = [ "csearch" , "defs", "pytest" ]
+ignore_obsolete = [  "typeguard" ]
+extend_exclude = [ 'p2g/tests' ] 
 [tool.pyright]
 disable = "N802"
 ignore = ["N802"]
 include = ["p2g/*.py"]
+exclude= [ "p2g/tests" , "p2g/doc", "p2g/examples"]
+omit = ['p2g/tests/*.py']
 [tool.isort]
 force_alphabetical_sort_within_sections = true
 #force_single_line = true
 combine_as_imports = true
 lines_between_types = 1
 known_localfolder = "p2g"
 lines_after_imports = 2
@@ -134,15 +142,15 @@
 [tool.coverage.run]
 
 #include = ["p2g/*.py"]
 
 
 [tool.coverage.report]
 include = ["p2g/*.py"]
-exclude_lines = ["NotImplemented", "for debug",  "no cover","@(abc\\.)?abstractmethod" ]
+exclude_lines = ["NotImplemented", "AssertionError", "for debug",  "no cover","@(abc\\.)?abstractmethod" ]
 
 omit = ["p2g/tests/*.py","p2g/examples/*.py","p2g/__main__.py"]
 
 
 [tool.flake8]
 ignore = ['E231', 'E241', "T201", "SCS109", "B601", "IF100","SCS108", "S101","W503",
 'G004','E203', 'R504']
```

