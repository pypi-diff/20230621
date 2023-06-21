# Comparing `tmp/yellowdog-python-examples-6.0.2.tar.gz` & `tmp/yellowdog-python-examples-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.2.tar", last modified: Tue Jun 20 15:24:16 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.3.tar", last modified: Wed Jun 21 15:21:00 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.2.tar` & `yellowdog-python-examples-6.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.870418 yellowdog-python-examples-6.0.2/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.2/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-20 15:24:16.870472 yellowdog-python-examples-6.0.2/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.2/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   110946 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.2/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-20 15:24:16.870742 yellowdog-python-examples-6.0.2/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.2/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.869529 yellowdog-python-examples-6.0.2/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.2/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.2/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.2/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.2/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.2/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.2/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.2/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.2/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.2/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-06-20 14:36:54.000000 yellowdog-python-examples-6.0.2/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3471 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.2/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     3002 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.870316 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.795598 yellowdog-python-examples-6.0.3/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.3/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-21 15:21:00.795687 yellowdog-python-examples-6.0.3/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.3/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   110945 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.3/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-21 15:21:00.795998 yellowdog-python-examples-6.0.3/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.3/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.794636 yellowdog-python-examples-6.0.3/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.3/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.3/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.3/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.3/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.3/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.3/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.3/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.3/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.3/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.3/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-06-20 14:36:54.000000 yellowdog-python-examples-6.0.3/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.3/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.3/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.3/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2995 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.3/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-21 15:21:00.795471 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-21 15:21:00.000000 yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.2/LICENSE` & `yellowdog-python-examples-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/PKG-INFO` & `yellowdog-python-examples-6.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.2
+Version: 6.0.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.2/PYPI_README.md` & `yellowdog-python-examples-6.0.3/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/README.md` & `yellowdog-python-examples-6.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -986,5950 +986,5950 @@
 00003d90: 7565 206f 6620 7468 6520 656e 7669 726f  ue of the enviro
 00003da0: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
 00003db0: 4854 5450 535f 5052 4f58 5960 2069 6620  HTTPS_PROXY` if 
 00003dc0: 726f 7574 696e 6720 7468 726f 7567 6820  routing through 
 00003dd0: 6120 7072 6f78 7920 6973 2072 6571 7569  a proxy is requi
 00003de0: 7265 642e 0a0a 496e 2061 6464 6974 696f  red...In additio
 00003df0: 6e2c 2074 6865 2063 6f6d 6d61 6e64 7320  n, the commands 
-00003e00: 6361 6e20 7573 6520 5072 6f78 7920 4175  can use Proxy Au
-00003e10: 746f 2d43 6f6e 6669 6775 7261 7469 6f6e  to-Configuration
-00003e20: 2028 5041 4329 2069 6620 7468 6520 602d   (PAC) if the `-
-00003e30: 2d70 6163 6020 636f 6d6d 616e 6420 6c69  -pac` command li
-00003e40: 6e65 206f 7074 696f 6e20 6973 2073 7065  ne option is spe
-00003e50: 6369 6669 6564 2c20 6f72 2069 6620 7468  cified, or if th
-00003e60: 6520 6075 7365 5041 4360 2070 726f 7065  e `usePAC` prope
-00003e70: 7274 7920 6973 2073 6574 2074 6f20 6074  rty is set to `t
-00003e80: 7275 6560 2069 6e20 7468 6520 605b 636f  rue` in the `[co
-00003e90: 6d6d 6f6e 5d60 2073 6563 7469 6f6e 206f  mmon]` section o
-00003ea0: 6620 7468 6520 6063 6f6e 6669 672e 746f  f the `config.to
-00003eb0: 6d6c 6020 6669 6c65 2e0a 0a23 2320 5370  ml` file...## Sp
-00003ec0: 6563 6966 7969 6e67 2043 6f6d 6d6f 6e20  ecifying Common 
-00003ed0: 5072 6f70 6572 7469 6573 2075 7369 6e67  Properties using
-00003ee0: 2074 6865 2043 6f6d 6d61 6e64 204c 696e   the Command Lin
-00003ef0: 6520 6f72 2045 6e76 6972 6f6e 6d65 6e74  e or Environment
-00003f00: 2056 6172 6961 626c 6573 0a0a 416c 6c20   Variables..All 
-00003f10: 7468 6520 636f 6d6d 6f6e 2070 726f 7065  the common prope
-00003f20: 7274 6965 7320 6361 6e20 6265 2073 6574  rties can be set
-00003f30: 2075 7369 6e67 2063 6f6d 6d61 6e64 206c   using command l
-00003f40: 696e 6520 6f70 7469 6f6e 732c 206f 7220  ine options, or 
-00003f50: 696e 2065 6e76 6972 6f6e 6d65 6e74 2076  in environment v
-00003f60: 6172 6961 626c 6573 2e0a 0a54 6865 202a  ariables...The *
-00003f70: 2a63 6f6d 6d61 6e64 206c 696e 6520 6f70  *command line op
-00003f80: 7469 6f6e 732a 2a20 6172 6520 6173 2066  tions** are as f
-00003f90: 6f6c 6c6f 7773 3a0a 0a2d 2060 2d2d 6b65  ollows:..- `--ke
-00003fa0: 7960 206f 7220 602d 6b60 0a2d 2060 2d2d  y` or `-k`.- `--
-00003fb0: 7365 6372 6574 6020 6f72 2060 2d73 600a  secret` or `-s`.
-00003fc0: 2d20 602d 2d6e 616d 6573 7061 6365 6020  - `--namespace` 
-00003fd0: 6f72 2060 2d6e 600a 2d20 602d 2d74 6167  or `-n`.- `--tag
-00003fe0: 6020 6f72 2060 2d74 600a 2d20 602d 2d75  ` or `-t`.- `--u
-00003ff0: 726c 6020 6f72 2060 2d75 600a 2d20 602d  rl` or `-u`.- `-
-00004000: 2d70 6163 600a 0a54 6865 7365 206f 7074  -pac`..These opt
-00004010: 696f 6e73 2063 616e 2061 6c73 6f20 6265  ions can also be
-00004020: 206c 6973 7465 6420 6279 2072 756e 6e69   listed by runni
-00004030: 6e67 2061 2063 6f6d 6d61 6e64 2077 6974  ng a command wit
-00004040: 6820 7468 6520 602d 2d68 656c 7060 206f  h the `--help` o
-00004050: 7220 602d 6860 206f 7074 696f 6e2e 0a0a  r `-h` option...
-00004060: 5468 6520 2a2a 656e 7669 726f 6e6d 656e  The **environmen
-00004070: 7420 7661 7269 6162 6c65 732a 2a20 6172  t variables** ar
-00004080: 6520 6173 2066 6f6c 6c6f 7773 3a0a 0a2d  e as follows:..-
-00004090: 2060 5944 5f4b 4559 600a 2d20 6059 445f   `YD_KEY`.- `YD_
-000040a0: 5345 4352 4554 600a 2d20 6059 445f 4e41  SECRET`.- `YD_NA
-000040b0: 4d45 5350 4143 4560 0a2d 2060 5944 5f54  MESPACE`.- `YD_T
-000040c0: 4147 600a 2d20 6059 445f 5552 4c60 0a0a  AG`.- `YD_URL`..
-000040d0: 5768 656e 2073 6574 7469 6e67 2074 6865  When setting the
-000040e0: 2076 616c 7565 206f 6620 7468 6520 6162   value of the ab
-000040f0: 6f76 6520 7072 6f70 6572 7469 6573 2c20  ove properties, 
-00004100: 6120 7072 6f70 6572 7479 2073 6574 206f  a property set o
-00004110: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
-00004120: 6e65 2074 616b 6573 2070 7265 6365 6465  ne takes precede
-00004130: 6e63 6520 6f76 6572 206f 6e65 2073 6574  nce over one set
-00004140: 2076 6961 2061 6e20 656e 7669 726f 6e6d   via an environm
-00004150: 656e 7420 7661 7269 6162 6c65 2c20 616e  ent variable, an
-00004160: 6420 626f 7468 2074 616b 6520 7072 6563  d both take prec
-00004170: 6564 656e 6365 206f 7665 7220 6120 7661  edence over a va
-00004180: 6c75 6520 7365 7420 696e 2061 2063 6f6e  lue set in a con
-00004190: 6669 6775 7261 7469 6f6e 2066 696c 652e  figuration file.
-000041a0: 0a0a 4966 2061 6c6c 2074 6865 2072 6571  ..If all the req
-000041b0: 7569 7265 6420 636f 6d6d 6f6e 2070 726f  uired common pro
-000041c0: 7065 7274 6965 7320 6172 6520 7365 7420  perties are set 
-000041d0: 7573 696e 6720 7468 6520 636f 6d6d 616e  using the comman
-000041e0: 6420 6c69 6e65 206f 7220 656e 7669 726f  d line or enviro
-000041f0: 6e6d 656e 7420 7661 7269 6162 6c65 732c  nment variables,
-00004200: 2074 6865 6e20 7468 6520 656e 7469 7265   then the entire
-00004210: 2060 636f 6d6d 6f6e 6020 7365 6374 696f   `common` sectio
-00004220: 6e20 6f66 2074 6865 2054 4f4d 4c20 6669  n of the TOML fi
-00004230: 6c65 2063 616e 2062 6520 6f6d 6974 7465  le can be omitte
-00004240: 642e 0a0a 2323 2056 6172 6961 626c 6520  d...## Variable 
-00004250: 5375 6273 7469 7475 7469 6f6e 7320 696e  Substitutions in
-00004260: 2043 6f6d 6d6f 6e20 5072 6f70 6572 7469   Common Properti
-00004270: 6573 0a0a 4e6f 7465 2074 6865 2075 7365  es..Note the use
-00004280: 206f 6620 607b 7b75 7365 726e 616d 657d   of `{{username}
-00004290: 7d60 2069 6e20 7468 6520 7661 6c75 6520  }` in the value 
-000042a0: 6f66 2074 6865 2060 7461 6760 2070 726f  of the `tag` pro
-000042b0: 7065 7274 793a 2074 6869 7320 6973 2061  perty: this is a
-000042c0: 202a 2a76 6172 6961 626c 6520 7375 6273   **variable subs
-000042d0: 7469 7475 7469 6f6e 2a2a 2074 6861 7420  titution** that 
-000042e0: 6361 6e20 6f70 7469 6f6e 616c 6c79 2062  can optionally b
-000042f0: 6520 7573 6564 2074 6f20 696e 7365 7274  e used to insert
-00004300: 2074 6865 206c 6f67 696e 2075 7365 726e   the login usern
-00004310: 616d 6520 6f66 2074 6865 2075 7365 7220  ame of the user 
-00004320: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00004330: 616e 6473 2e20 536f 2c20 666f 7220 7573  ands. So, for us
-00004340: 6572 6e61 6d65 2060 6162 6360 2c20 7468  ername `abc`, th
-00004350: 6520 6074 6167 6020 776f 756c 6420 6265  e `tag` would be
-00004360: 2073 6574 2074 6f20 6074 6573 7469 6e67   set to `testing
-00004370: 2d61 6263 602e 2054 6869 7320 6361 6e20  -abc`. This can 
-00004380: 6265 2068 656c 7066 756c 2074 6f20 6469  be helpful to di
-00004390: 7361 6d62 6967 7561 7465 206d 756c 7469  sambiguate multi
-000043a0: 706c 6520 7573 6572 7320 7275 6e6e 696e  ple users runnin
-000043b0: 6720 7769 7468 2074 6865 2073 616d 6520  g with the same 
-000043c0: 636f 6e66 6967 7572 6174 696f 6e20 6461  configuration da
-000043d0: 7461 2e0a 0a56 6172 6961 626c 6520 7375  ta...Variable su
-000043e0: 6273 7469 7475 7469 6f6e 7320 6172 6520  bstitutions are 
-000043f0: 6469 7363 7573 7365 6420 6265 6c6f 772e  discussed below.
-00004400: 0a0a 2320 5661 7269 6162 6c65 2053 7562  ..# Variable Sub
-00004410: 7374 6974 7574 696f 6e73 0a0a 5661 7269  stitutions..Vari
-00004420: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00004430: 6e73 2070 726f 7669 6465 2061 2070 6f77  ns provide a pow
-00004440: 6572 6675 6c20 7761 7920 6f66 2069 6e74  erful way of int
-00004450: 726f 6475 6369 6e67 2076 6172 6961 626c  roducing variabl
-00004460: 6520 7661 6c75 6573 2069 6e74 6f20 544f  e values into TO
-00004470: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-00004480: 2066 696c 6573 2c20 576f 726b 2052 6571   files, Work Req
-00004490: 7569 7265 6d65 6e74 204a 534f 4e20 6465  uirement JSON de
-000044a0: 6669 6e69 7469 6f6e 732c 2061 6e64 2057  finitions, and W
-000044b0: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
-000044c0: 6465 6669 6e69 7469 6f6e 732e 2054 6865  definitions. The
-000044d0: 7920 6361 6e20 6265 2069 6e63 6c75 6465  y can be include
-000044e0: 6420 696e 2074 6865 2076 616c 7565 206f  d in the value o
-000044f0: 6620 616e 7920 7072 6f70 6572 7479 2069  f any property i
-00004500: 6e20 6561 6368 206f 6620 7468 6573 6520  n each of these 
-00004510: 6f62 6a65 6374 732c 2069 6e63 6c75 6469  objects, includi
-00004520: 6e67 2069 6e20 7661 6c75 6573 2077 6974  ng in values wit
-00004530: 6869 6e20 6c69 7374 7320 2865 2e67 2e2c  hin lists (e.g.,
-00004540: 2066 6f72 2074 6865 2060 6172 6775 6d65   for the `argume
-00004550: 6e74 7360 2070 726f 7065 7274 7929 2061  nts` property) a
-00004560: 6e64 2061 7272 6179 7320 2865 2e67 2e2c  nd arrays (e.g.,
-00004570: 2074 6865 2060 656e 7669 726f 6e6d 656e   the `environmen
-00004580: 7460 2070 726f 7065 7274 7929 2e0a 0a56  t` property)...V
-00004590: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
-000045a0: 7469 6f6e 7320 6172 6520 6578 7072 6573  tions are expres
-000045b0: 7365 6420 7573 696e 6720 607b 7b76 6172  sed using `{{var
-000045c0: 6961 626c 657d 7d60 206e 6f74 6174 696f  iable}}` notatio
-000045d0: 6e2c 2077 6865 7265 2074 6865 2065 7870  n, where the exp
-000045e0: 7265 7373 696f 6e20 6973 2072 6570 6c61  ression is repla
-000045f0: 6365 6420 6279 2074 6865 2076 616c 7565  ced by the value
-00004600: 206f 6620 6076 6172 6961 626c 6560 2e0a   of `variable`..
-00004610: 0a53 7562 7374 6974 7574 696f 6e73 2063  .Substitutions c
-00004620: 616e 2061 6c73 6f20 6265 2070 6572 666f  an also be perfo
-00004630: 726d 6564 2066 6f72 206e 6f6e 2d73 7472  rmed for non-str
-00004640: 696e 6720 286e 756d 6265 7220 616e 6420  ing (number and 
-00004650: 626f 6f6c 6561 6e29 2076 616c 7565 7320  boolean) values 
-00004660: 7573 696e 6720 7468 6520 606e 756d 3a60  using the `num:`
-00004670: 2061 6e64 2060 626f 6f6c 3a60 2070 7265   and `bool:` pre
-00004680: 6669 7865 7320 7769 7468 696e 2074 6865  fixes within the
-00004690: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-000046a0: 7475 7469 6f6e 3a0a 0a2d 2044 6566 696e  tution:..- Defin
-000046b0: 6520 7468 6520 7661 7269 6162 6c65 2073  e the variable s
-000046c0: 7562 7374 6974 7574 696f 6e20 7573 696e  ubstitution usin
-000046d0: 6720 6f6e 6520 6f66 2074 6865 2066 6f6c  g one of the fol
-000046e0: 6c6f 7769 6e67 2070 6174 7465 726e 733a  lowing patterns:
-000046f0: 2060 227b 7b6e 756d 3a6d 795f 696e 747d   `"{{num:my_int}
-00004700: 7d22 602c 2060 227b 7b6e 756d 3a6d 795f  }"`, `"{{num:my_
-00004710: 666c 6f61 747d 7d22 602c 2060 227b 7b62  float}}"`, `"{{b
-00004720: 6f6f 6c3a 6d79 5f62 6f6f 6c7d 7d22 600a  ool:my_bool}}"`.
-00004730: 2d20 5661 7269 6162 6c65 2064 6566 696e  - Variable defin
-00004740: 6974 696f 6e73 2073 7570 706c 6965 6420  itions supplied 
-00004750: 6f6e 2074 6865 2063 6f6d 6d61 6e64 206c  on the command l
-00004760: 696e 6520 776f 756c 6420 7468 656e 2062  ine would then b
-00004770: 6520 6f66 2074 6865 2066 6f72 6d3a 2060  e of the form: `
-00004780: 2d6d 206d 795f 696e 743d 3520 2d6d 206d  -m my_int=5 -m m
-00004790: 795f 666c 6f61 743d 322e 3520 2d6d 206d  y_float=2.5 -m m
-000047a0: 795f 626f 6f6c 3d74 7275 6560 0a2d 2049  y_bool=true`.- I
-000047b0: 6e20 7468 6520 7072 6f63 6573 7365 6420  n the processed 
-000047c0: 4a53 4f4e 206f 7220 544f 4d4c 2c20 7468  JSON or TOML, th
-000047d0: 6573 6520 7661 6c75 6573 2077 6f75 6c64  ese values would
-000047e0: 2062 6563 6f6d 6520 6035 602c 2060 322e   become `5`, `2.
-000047f0: 3560 2061 6e64 2060 7472 7565 602c 2072  5` and `true`, r
-00004800: 6573 7065 6374 6976 656c 792c 2063 6f6e  espectively, con
-00004810: 7665 7274 6564 2066 726f 6d20 7374 7269  verted from stri
-00004820: 6e67 7320 746f 2074 6865 6972 2063 6f72  ngs to their cor
-00004830: 7265 6374 204a 534f 4e20 7479 7065 730a  rect JSON types.
-00004840: 0a23 2320 4465 6661 756c 7420 5661 7269  .## Default Vari
-00004850: 6162 6c65 730a 0a54 6865 2066 6f6c 6c6f  ables..The follo
-00004860: 7769 6e67 2073 7562 7374 6974 7574 696f  wing substitutio
-00004870: 6e73 2061 7265 2061 7574 6f6d 6174 6963  ns are automatic
-00004880: 616c 6c79 2063 7265 6174 6564 2061 6e64  ally created and
-00004890: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
-000048a0: 616e 7920 7365 6374 696f 6e20 6f66 2074  any section of t
-000048b0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-000048c0: 2066 696c 652c 206f 7220 696e 2061 6e79   file, or in any
-000048d0: 204a 534f 4e20 7370 6563 6966 6963 6174   JSON specificat
-000048e0: 696f 6e3a 0a0a 7c20 4469 7265 6374 6976  ion:..| Directiv
-000048f0: 6520 2020 2020 2020 7c20 4465 7363 7269  e       | Descri
-00004900: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
+00003e00: 6361 6e20 7573 6520 7072 6f78 7920 6175  can use proxy au
+00003e10: 746f 636f 6e66 6967 7572 6174 696f 6e20  toconfiguration 
+00003e20: 2850 4143 2920 6966 2074 6865 2060 2d2d  (PAC) if the `--
+00003e30: 7061 6360 2063 6f6d 6d61 6e64 206c 696e  pac` command lin
+00003e40: 6520 6f70 7469 6f6e 2069 7320 7370 6563  e option is spec
+00003e50: 6966 6965 642c 206f 7220 6966 2074 6865  ified, or if the
+00003e60: 2060 7573 6550 4143 6020 7072 6f70 6572   `usePAC` proper
+00003e70: 7479 2069 7320 7365 7420 746f 2060 7472  ty is set to `tr
+00003e80: 7565 6020 696e 2074 6865 2060 5b63 6f6d  ue` in the `[com
+00003e90: 6d6f 6e5d 6020 7365 6374 696f 6e20 6f66  mon]` section of
+00003ea0: 2074 6865 2060 636f 6e66 6967 2e74 6f6d   the `config.tom
+00003eb0: 6c60 2066 696c 652e 0a0a 2323 2053 7065  l` file...## Spe
+00003ec0: 6369 6679 696e 6720 436f 6d6d 6f6e 2050  cifying Common P
+00003ed0: 726f 7065 7274 6965 7320 7573 696e 6720  roperties using 
+00003ee0: 7468 6520 436f 6d6d 616e 6420 4c69 6e65  the Command Line
+00003ef0: 206f 7220 456e 7669 726f 6e6d 656e 7420   or Environment 
+00003f00: 5661 7269 6162 6c65 730a 0a41 6c6c 2074  Variables..All t
+00003f10: 6865 2063 6f6d 6d6f 6e20 7072 6f70 6572  he common proper
+00003f20: 7469 6573 2063 616e 2062 6520 7365 7420  ties can be set 
+00003f30: 7573 696e 6720 636f 6d6d 616e 6420 6c69  using command li
+00003f40: 6e65 206f 7074 696f 6e73 2c20 6f72 2069  ne options, or i
+00003f50: 6e20 656e 7669 726f 6e6d 656e 7420 7661  n environment va
+00003f60: 7269 6162 6c65 732e 0a0a 5468 6520 2a2a  riables...The **
+00003f70: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
+00003f80: 696f 6e73 2a2a 2061 7265 2061 7320 666f  ions** are as fo
+00003f90: 6c6c 6f77 733a 0a0a 2d20 602d 2d6b 6579  llows:..- `--key
+00003fa0: 6020 6f72 2060 2d6b 600a 2d20 602d 2d73  ` or `-k`.- `--s
+00003fb0: 6563 7265 7460 206f 7220 602d 7360 0a2d  ecret` or `-s`.-
+00003fc0: 2060 2d2d 6e61 6d65 7370 6163 6560 206f   `--namespace` o
+00003fd0: 7220 602d 6e60 0a2d 2060 2d2d 7461 6760  r `-n`.- `--tag`
+00003fe0: 206f 7220 602d 7460 0a2d 2060 2d2d 7572   or `-t`.- `--ur
+00003ff0: 6c60 206f 7220 602d 7560 0a2d 2060 2d2d  l` or `-u`.- `--
+00004000: 7061 6360 0a0a 5468 6573 6520 6f70 7469  pac`..These opti
+00004010: 6f6e 7320 6361 6e20 616c 736f 2062 6520  ons can also be 
+00004020: 6c69 7374 6564 2062 7920 7275 6e6e 696e  listed by runnin
+00004030: 6720 6120 636f 6d6d 616e 6420 7769 7468  g a command with
+00004040: 2074 6865 2060 2d2d 6865 6c70 6020 6f72   the `--help` or
+00004050: 2060 2d68 6020 6f70 7469 6f6e 2e0a 0a54   `-h` option...T
+00004060: 6865 202a 2a65 6e76 6972 6f6e 6d65 6e74  he **environment
+00004070: 2076 6172 6961 626c 6573 2a2a 2061 7265   variables** are
+00004080: 2061 7320 666f 6c6c 6f77 733a 0a0a 2d20   as follows:..- 
+00004090: 6059 445f 4b45 5960 0a2d 2060 5944 5f53  `YD_KEY`.- `YD_S
+000040a0: 4543 5245 5460 0a2d 2060 5944 5f4e 414d  ECRET`.- `YD_NAM
+000040b0: 4553 5041 4345 600a 2d20 6059 445f 5441  ESPACE`.- `YD_TA
+000040c0: 4760 0a2d 2060 5944 5f55 524c 600a 0a57  G`.- `YD_URL`..W
+000040d0: 6865 6e20 7365 7474 696e 6720 7468 6520  hen setting the 
+000040e0: 7661 6c75 6520 6f66 2074 6865 2061 626f  value of the abo
+000040f0: 7665 2070 726f 7065 7274 6965 732c 2061  ve properties, a
+00004100: 2070 726f 7065 7274 7920 7365 7420 6f6e   property set on
+00004110: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00004120: 6520 7461 6b65 7320 7072 6563 6564 656e  e takes preceden
+00004130: 6365 206f 7665 7220 6f6e 6520 7365 7420  ce over one set 
+00004140: 7669 6120 616e 2065 6e76 6972 6f6e 6d65  via an environme
+00004150: 6e74 2076 6172 6961 626c 652c 2061 6e64  nt variable, and
+00004160: 2062 6f74 6820 7461 6b65 2070 7265 6365   both take prece
+00004170: 6465 6e63 6520 6f76 6572 2061 2076 616c  dence over a val
+00004180: 7565 2073 6574 2069 6e20 6120 636f 6e66  ue set in a conf
+00004190: 6967 7572 6174 696f 6e20 6669 6c65 2e0a  iguration file..
+000041a0: 0a49 6620 616c 6c20 7468 6520 7265 7175  .If all the requ
+000041b0: 6972 6564 2063 6f6d 6d6f 6e20 7072 6f70  ired common prop
+000041c0: 6572 7469 6573 2061 7265 2073 6574 2075  erties are set u
+000041d0: 7369 6e67 2074 6865 2063 6f6d 6d61 6e64  sing the command
+000041e0: 206c 696e 6520 6f72 2065 6e76 6972 6f6e   line or environ
+000041f0: 6d65 6e74 2076 6172 6961 626c 6573 2c20  ment variables, 
+00004200: 7468 656e 2074 6865 2065 6e74 6972 6520  then the entire 
+00004210: 6063 6f6d 6d6f 6e60 2073 6563 7469 6f6e  `common` section
+00004220: 206f 6620 7468 6520 544f 4d4c 2066 696c   of the TOML fil
+00004230: 6520 6361 6e20 6265 206f 6d69 7474 6564  e can be omitted
+00004240: 2e0a 0a23 2320 5661 7269 6162 6c65 2053  ...## Variable S
+00004250: 7562 7374 6974 7574 696f 6e73 2069 6e20  ubstitutions in 
+00004260: 436f 6d6d 6f6e 2050 726f 7065 7274 6965  Common Propertie
+00004270: 730a 0a4e 6f74 6520 7468 6520 7573 6520  s..Note the use 
+00004280: 6f66 2060 7b7b 7573 6572 6e61 6d65 7d7d  of `{{username}}
+00004290: 6020 696e 2074 6865 2076 616c 7565 206f  ` in the value o
+000042a0: 6620 7468 6520 6074 6167 6020 7072 6f70  f the `tag` prop
+000042b0: 6572 7479 3a20 7468 6973 2069 7320 6120  erty: this is a 
+000042c0: 2a2a 7661 7269 6162 6c65 2073 7562 7374  **variable subst
+000042d0: 6974 7574 696f 6e2a 2a20 7468 6174 2063  itution** that c
+000042e0: 616e 206f 7074 696f 6e61 6c6c 7920 6265  an optionally be
+000042f0: 2075 7365 6420 746f 2069 6e73 6572 7420   used to insert 
+00004300: 7468 6520 6c6f 6769 6e20 7573 6572 6e61  the login userna
+00004310: 6d65 206f 6620 7468 6520 7573 6572 2072  me of the user r
+00004320: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
+00004330: 6e64 732e 2053 6f2c 2066 6f72 2075 7365  nds. So, for use
+00004340: 726e 616d 6520 6061 6263 602c 2074 6865  rname `abc`, the
+00004350: 2060 7461 6760 2077 6f75 6c64 2062 6520   `tag` would be 
+00004360: 7365 7420 746f 2060 7465 7374 696e 672d  set to `testing-
+00004370: 6162 6360 2e20 5468 6973 2063 616e 2062  abc`. This can b
+00004380: 6520 6865 6c70 6675 6c20 746f 2064 6973  e helpful to dis
+00004390: 616d 6269 6775 6174 6520 6d75 6c74 6970  ambiguate multip
+000043a0: 6c65 2075 7365 7273 2072 756e 6e69 6e67  le users running
+000043b0: 2077 6974 6820 7468 6520 7361 6d65 2063   with the same c
+000043c0: 6f6e 6669 6775 7261 7469 6f6e 2064 6174  onfiguration dat
+000043d0: 612e 0a0a 5661 7269 6162 6c65 2073 7562  a...Variable sub
+000043e0: 7374 6974 7574 696f 6e73 2061 7265 2064  stitutions are d
+000043f0: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
+00004400: 0a23 2056 6172 6961 626c 6520 5375 6273  .# Variable Subs
+00004410: 7469 7475 7469 6f6e 730a 0a56 6172 6961  titutions..Varia
+00004420: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
+00004430: 7320 7072 6f76 6964 6520 6120 706f 7765  s provide a powe
+00004440: 7266 756c 2077 6179 206f 6620 696e 7472  rful way of intr
+00004450: 6f64 7563 696e 6720 7661 7269 6162 6c65  oducing variable
+00004460: 2076 616c 7565 7320 696e 746f 2054 4f4d   values into TOM
+00004470: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+00004480: 6669 6c65 732c 2057 6f72 6b20 5265 7175  files, Work Requ
+00004490: 6972 656d 656e 7420 4a53 4f4e 2064 6566  irement JSON def
+000044a0: 696e 6974 696f 6e73 2c20 616e 6420 576f  initions, and Wo
+000044b0: 726b 6572 2050 6f6f 6c20 4a53 4f4e 2064  rker Pool JSON d
+000044c0: 6566 696e 6974 696f 6e73 2e20 5468 6579  efinitions. They
+000044d0: 2063 616e 2062 6520 696e 636c 7564 6564   can be included
+000044e0: 2069 6e20 7468 6520 7661 6c75 6520 6f66   in the value of
+000044f0: 2061 6e79 2070 726f 7065 7274 7920 696e   any property in
+00004500: 2065 6163 6820 6f66 2074 6865 7365 206f   each of these o
+00004510: 626a 6563 7473 2c20 696e 636c 7564 696e  bjects, includin
+00004520: 6720 696e 2076 616c 7565 7320 7769 7468  g in values with
+00004530: 696e 206c 6973 7473 2028 652e 672e 2c20  in lists (e.g., 
+00004540: 666f 7220 7468 6520 6061 7267 756d 656e  for the `argumen
+00004550: 7473 6020 7072 6f70 6572 7479 2920 616e  ts` property) an
+00004560: 6420 6172 7261 7973 2028 652e 672e 2c20  d arrays (e.g., 
+00004570: 7468 6520 6065 6e76 6972 6f6e 6d65 6e74  the `environment
+00004580: 6020 7072 6f70 6572 7479 292e 0a0a 5661  ` property)...Va
+00004590: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+000045a0: 696f 6e73 2061 7265 2065 7870 7265 7373  ions are express
+000045b0: 6564 2075 7369 6e67 2060 7b7b 7661 7269  ed using `{{vari
+000045c0: 6162 6c65 7d7d 6020 6e6f 7461 7469 6f6e  able}}` notation
+000045d0: 2c20 7768 6572 6520 7468 6520 6578 7072  , where the expr
+000045e0: 6573 7369 6f6e 2069 7320 7265 706c 6163  ession is replac
+000045f0: 6564 2062 7920 7468 6520 7661 6c75 6520  ed by the value 
+00004600: 6f66 2060 7661 7269 6162 6c65 602e 0a0a  of `variable`...
+00004610: 5375 6273 7469 7475 7469 6f6e 7320 6361  Substitutions ca
+00004620: 6e20 616c 736f 2062 6520 7065 7266 6f72  n also be perfor
+00004630: 6d65 6420 666f 7220 6e6f 6e2d 7374 7269  med for non-stri
+00004640: 6e67 2028 6e75 6d62 6572 2061 6e64 2062  ng (number and b
+00004650: 6f6f 6c65 616e 2920 7661 6c75 6573 2075  oolean) values u
+00004660: 7369 6e67 2074 6865 2060 6e75 6d3a 6020  sing the `num:` 
+00004670: 616e 6420 6062 6f6f 6c3a 6020 7072 6566  and `bool:` pref
+00004680: 6978 6573 2077 6974 6869 6e20 7468 6520  ixes within the 
+00004690: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+000046a0: 7574 696f 6e3a 0a0a 2d20 4465 6669 6e65  ution:..- Define
+000046b0: 2074 6865 2076 6172 6961 626c 6520 7375   the variable su
+000046c0: 6273 7469 7475 7469 6f6e 2075 7369 6e67  bstitution using
+000046d0: 206f 6e65 206f 6620 7468 6520 666f 6c6c   one of the foll
+000046e0: 6f77 696e 6720 7061 7474 6572 6e73 3a20  owing patterns: 
+000046f0: 6022 7b7b 6e75 6d3a 6d79 5f69 6e74 7d7d  `"{{num:my_int}}
+00004700: 2260 2c20 6022 7b7b 6e75 6d3a 6d79 5f66  "`, `"{{num:my_f
+00004710: 6c6f 6174 7d7d 2260 2c20 6022 7b7b 626f  loat}}"`, `"{{bo
+00004720: 6f6c 3a6d 795f 626f 6f6c 7d7d 2260 0a2d  ol:my_bool}}"`.-
+00004730: 2056 6172 6961 626c 6520 6465 6669 6e69   Variable defini
+00004740: 7469 6f6e 7320 7375 7070 6c69 6564 206f  tions supplied o
+00004750: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
+00004760: 6e65 2077 6f75 6c64 2074 6865 6e20 6265  ne would then be
+00004770: 206f 6620 7468 6520 666f 726d 3a20 602d   of the form: `-
+00004780: 6d20 6d79 5f69 6e74 3d35 202d 6d20 6d79  m my_int=5 -m my
+00004790: 5f66 6c6f 6174 3d32 2e35 202d 6d20 6d79  _float=2.5 -m my
+000047a0: 5f62 6f6f 6c3d 7472 7565 600a 2d20 496e  _bool=true`.- In
+000047b0: 2074 6865 2070 726f 6365 7373 6564 204a   the processed J
+000047c0: 534f 4e20 6f72 2054 4f4d 4c2c 2074 6865  SON or TOML, the
+000047d0: 7365 2076 616c 7565 7320 776f 756c 6420  se values would 
+000047e0: 6265 636f 6d65 2060 3560 2c20 6032 2e35  become `5`, `2.5
+000047f0: 6020 616e 6420 6074 7275 6560 2c20 7265  ` and `true`, re
+00004800: 7370 6563 7469 7665 6c79 2c20 636f 6e76  spectively, conv
+00004810: 6572 7465 6420 6672 6f6d 2073 7472 696e  erted from strin
+00004820: 6773 2074 6f20 7468 6569 7220 636f 7272  gs to their corr
+00004830: 6563 7420 4a53 4f4e 2074 7970 6573 0a0a  ect JSON types..
+00004840: 2323 2044 6566 6175 6c74 2056 6172 6961  ## Default Varia
+00004850: 626c 6573 0a0a 5468 6520 666f 6c6c 6f77  bles..The follow
+00004860: 696e 6720 7375 6273 7469 7475 7469 6f6e  ing substitution
+00004870: 7320 6172 6520 6175 746f 6d61 7469 6361  s are automatica
+00004880: 6c6c 7920 6372 6561 7465 6420 616e 6420  lly created and 
+00004890: 6361 6e20 6265 2075 7365 6420 696e 2061  can be used in a
+000048a0: 6e79 2073 6563 7469 6f6e 206f 6620 7468  ny section of th
+000048b0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+000048c0: 6669 6c65 2c20 6f72 2069 6e20 616e 7920  file, or in any 
+000048d0: 4a53 4f4e 2073 7065 6369 6669 6361 7469  JSON specificati
+000048e0: 6f6e 3a0a 0a7c 2044 6972 6563 7469 7665  on:..| Directive
+000048f0: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
+00004900: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
 00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 207c 2045 7861 6d70 6c65 206f 6620     | Example of 
-00004950: 5375 6273 7469 7475 7469 6f6e 207c 0a7c  Substitution |.|
-00004960: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00004970: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
+00004940: 2020 7c20 4578 616d 706c 6520 6f66 2053    | Example of S
+00004950: 7562 7374 6974 7574 696f 6e20 7c0a 7c3a  ubstitution |.|:
+00004960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004970: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
 00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00004990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000049a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000049b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
+000049b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
 000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000049d0: 2d2d 2d2d 2d2d 7c0a 7c20 607b 7b75 7365  ------|.| `{{use
-000049e0: 726e 616d 657d 7d60 2020 7c20 5468 6520  rname}}`  | The 
-000049f0: 6375 7272 656e 7420 7573 6572 2773 206c  current user's l
-00004a00: 6f67 696e 2075 7365 726e 616d 652c 206c  ogin username, l
-00004a10: 6f77 6572 2063 6173 652c 2073 7061 6365  ower case, space
-00004a20: 7320 7265 706c 6163 6564 2020 2020 2020  s replaced      
-00004a30: 2020 2020 207c 206a 616e 655f 736d 6974       | jane_smit
-00004a40: 6820 2020 2020 2020 2020 2020 2020 207c  h              |
-00004a50: 0a7c 2060 7b7b 6461 7465 7d7d 6020 2020  .| `{{date}}`   
-00004a60: 2020 207c 2054 6865 2063 7572 7265 6e74     | The current
-00004a70: 2064 6174 6520 2855 5443 293a 2059 5959   date (UTC): YYY
-00004a80: 594d 4d44 4420 2020 2020 2020 2020 2020  YMMDD           
+000049d0: 2d2d 2d2d 2d7c 0a7c 2060 7b7b 7573 6572  -----|.| `{{user
+000049e0: 6e61 6d65 7d7d 6020 207c 2054 6865 2063  name}}`  | The c
+000049f0: 7572 7265 6e74 2075 7365 7227 7320 6c6f  urrent user's lo
+00004a00: 6769 6e20 7573 6572 6e61 6d65 2c20 6c6f  gin username, lo
+00004a10: 7765 7220 6361 7365 2c20 7370 6163 6573  wer case, spaces
+00004a20: 2072 6570 6c61 6365 6420 2020 2020 2020   replaced       
+00004a30: 2020 2020 7c20 6a61 6e65 5f73 6d69 7468      | jane_smith
+00004a40: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00004a50: 7c20 607b 7b64 6174 657d 7d60 2020 2020  | `{{date}}`    
+00004a60: 2020 7c20 5468 6520 6375 7272 656e 7420    | The current 
+00004a70: 6461 7465 2028 5554 4329 3a20 5959 5959  date (UTC): YYYY
+00004a80: 4d4d 4444 2020 2020 2020 2020 2020 2020  MMDD            
 00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00004ab0: 3230 3232 3130 3237 2020 2020 2020 2020  20221027        
-00004ac0: 2020 2020 2020 2020 7c0a 7c20 607b 7b74          |.| `{{t
-00004ad0: 696d 657d 7d60 2020 2020 2020 7c20 5468  ime}}`      | Th
-00004ae0: 6520 6375 7272 656e 7420 7469 6d65 2028  e current time (
-00004af0: 5554 4329 3a20 4848 4d4d 5353 2020 2020  UTC): HHMMSS    
+00004aa0: 2020 2020 2020 2020 2020 2020 207c 2032               | 2
+00004ab0: 3032 3231 3032 3720 2020 2020 2020 2020  0221027         
+00004ac0: 2020 2020 2020 207c 0a7c 2060 7b7b 7469         |.| `{{ti
+00004ad0: 6d65 7d7d 6020 2020 2020 207c 2054 6865  me}}`      | The
+00004ae0: 2063 7572 7265 6e74 2074 696d 6520 2855   current time (U
+00004af0: 5443 293a 2048 484d 4d53 5320 2020 2020  TC): HHMMSS     
 00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 207c 2031 3633 3032 3620         | 163026 
+00004b20: 2020 2020 2020 7c20 3136 3330 3236 2020        | 163026  
 00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 207c 0a7c 2060 7b7b 6461 7465 7469 6d65   |.| `{{datetime
-00004b50: 7d7d 6020 207c 2043 6f6e 6361 7465 6e61  }}`  | Concatena
-00004b60: 7469 6f6e 206f 6620 7468 6520 6461 7465  tion of the date
-00004b70: 2061 6e64 2074 696d 6520 6162 6f76 652c   and time above,
-00004b80: 2077 6974 6820 6120 272d 2720 7365 7061   with a '-' sepa
-00004b90: 7261 746f 7220 2020 2020 2020 2020 2020  rator           
-00004ba0: 7c20 3230 3232 3130 3237 2d31 3633 3032  | 20221027-16302
-00004bb0: 3620 2020 2020 2020 2020 7c0a 7c20 607b  6         |.| `{
-00004bc0: 7b72 616e 646f 6d7d 7d60 2020 2020 7c20  {random}}`    | 
-00004bd0: 4120 7261 6e64 6f6d 2c20 7468 7265 6520  A random, three 
-00004be0: 6469 6769 7420 6865 7861 6465 6369 6d61  digit hexadecima
-00004bf0: 6c20 6e75 6d62 6572 2028 6c6f 7765 7220  l number (lower 
-00004c00: 6361 7365 2920 2020 2020 2020 2020 2020  case)           
-00004c10: 2020 2020 2020 2020 207c 2061 3163 2020           | a1c  
+00004b40: 7c0a 7c20 607b 7b64 6174 6574 696d 657d  |.| `{{datetime}
+00004b50: 7d60 2020 7c20 436f 6e63 6174 656e 6174  }`  | Concatenat
+00004b60: 696f 6e20 6f66 2074 6865 2064 6174 6520  ion of the date 
+00004b70: 616e 6420 7469 6d65 2061 626f 7665 2c20  and time above, 
+00004b80: 7769 7468 2061 2027 2d27 2073 6570 6172  with a '-' separ
+00004b90: 6174 6f72 2020 2020 2020 2020 2020 207c  ator           |
+00004ba0: 2032 3032 3231 3032 372d 3136 3330 3236   20221027-163026
+00004bb0: 2020 2020 2020 2020 207c 0a7c 2060 7b7b           |.| `{{
+00004bc0: 7261 6e64 6f6d 7d7d 6020 2020 207c 2041  random}}`    | A
+00004bd0: 2072 616e 646f 6d2c 2074 6872 6565 2064   random, three d
+00004be0: 6967 6974 2068 6578 6164 6563 696d 616c  igit hexadecimal
+00004bf0: 206e 756d 6265 7220 286c 6f77 6572 2063   number (lower c
+00004c00: 6173 6529 2020 2020 2020 2020 2020 2020  ase)            
+00004c10: 2020 2020 2020 2020 7c20 6131 6320 2020          | a1c   
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 207c 0a7c 2060 7b7b 6e61 6d65 7370     |.| `{{namesp
-00004c40: 6163 657d 7d60 207c 2054 6865 2060 6e61  ace}}` | The `na
-00004c50: 6d65 7370 6163 6560 2070 726f 7065 7274  mespace` propert
-00004c60: 792e 204e 6f74 6520 7468 6174 2060 6e61  y. Note that `na
-00004c70: 6d65 7370 6163 6560 206d 7573 742c 206f  mespace` must, o
-00004c80: 6620 636f 7572 7365 2c20 6265 2073 6574  f course, be set
-00004c90: 2e20 7c20 6d79 5f6e 616d 6573 7061 6365  . | my_namespace
-00004ca0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00004cb0: 607b 7b74 6167 7d7d 6020 2020 2020 2020  `{{tag}}`       
-00004cc0: 7c20 5468 6520 6074 6167 6020 7072 6f70  | The `tag` prop
-00004cd0: 6572 7479 2e20 4e6f 7465 2074 6861 7420  erty. Note that 
-00004ce0: 6074 6167 6020 6d75 7374 2062 6520 7365  `tag` must be se
-00004cf0: 742e 2020 2020 2020 2020 2020 2020 2020  t.              
-00004d00: 2020 2020 2020 2020 2020 207c 206d 795f             | my_
-00004d10: 7461 6720 2020 2020 2020 2020 2020 2020  tag             
-00004d20: 2020 2020 207c 0a7c 2060 7b7b 6b65 797d       |.| `{{key}
-00004d30: 7d60 2020 2020 2020 207c 2054 6865 2061  }`       | The a
-00004d40: 7070 6c69 6361 7469 6f6e 2060 6b65 7960  pplication `key`
-00004d50: 2070 726f 7065 7274 792e 2020 2020 2020   property.      
+00004c30: 2020 7c0a 7c20 607b 7b6e 616d 6573 7061    |.| `{{namespa
+00004c40: 6365 7d7d 6020 7c20 5468 6520 606e 616d  ce}}` | The `nam
+00004c50: 6573 7061 6365 6020 7072 6f70 6572 7479  espace` property
+00004c60: 2e20 4e6f 7465 2074 6861 7420 606e 616d  . Note that `nam
+00004c70: 6573 7061 6365 6020 6d75 7374 2c20 6f66  espace` must, of
+00004c80: 2063 6f75 7273 652c 2062 6520 7365 742e   course, be set.
+00004c90: 207c 206d 795f 6e61 6d65 7370 6163 6520   | my_namespace 
+00004ca0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00004cb0: 7b7b 7461 677d 7d60 2020 2020 2020 207c  {{tag}}`       |
+00004cc0: 2054 6865 2060 7461 6760 2070 726f 7065   The `tag` prope
+00004cd0: 7274 792e 204e 6f74 6520 7468 6174 2060  rty. Note that `
+00004ce0: 7461 6760 206d 7573 7420 6265 2073 6574  tag` must be set
+00004cf0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d00: 2020 2020 2020 2020 2020 7c20 6d79 5f74            | my_t
+00004d10: 6167 2020 2020 2020 2020 2020 2020 2020  ag              
+00004d20: 2020 2020 7c0a 7c20 607b 7b6b 6579 7d7d      |.| `{{key}}
+00004d30: 6020 2020 2020 2020 7c20 5468 6520 6170  `       | The ap
+00004d40: 706c 6963 6174 696f 6e20 606b 6579 6020  plication `key` 
+00004d50: 7072 6f70 6572 7479 2e20 2020 2020 2020  property.       
 00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00004d90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00004da0: 7c20 607b 7b73 6563 7265 747d 7d60 2020  | `{{secret}}`  
-00004db0: 2020 7c20 5468 6520 6170 706c 6963 6174    | The applicat
-00004dc0: 696f 6e20 6073 6563 7265 7460 2070 726f  ion `secret` pro
-00004dd0: 7065 7274 792e 2020 2020 2020 2020 2020  perty.          
+00004d80: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00004d90: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00004da0: 2060 7b7b 7365 6372 6574 7d7d 6020 2020   `{{secret}}`   
+00004db0: 207c 2054 6865 2061 7070 6c69 6361 7469   | The applicati
+00004dc0: 6f6e 2060 7365 6372 6574 6020 7072 6f70  on `secret` prop
+00004dd0: 6572 7479 2e20 2020 2020 2020 2020 2020  erty.           
 00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00004df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 207c 0a7c 2060 7b7b 7572         |.| `{{ur
-00004e20: 6c7d 7d60 2020 2020 2020 207c 2054 6865  l}}`       | The
-00004e30: 2050 6c61 7466 6f72 6d20 6075 726c 6020   Platform `url` 
-00004e40: 7072 6f70 6572 7479 2e20 2020 2020 2020  property.       
+00004e10: 2020 2020 2020 7c0a 7c20 607b 7b75 726c        |.| `{{url
+00004e20: 7d7d 6020 2020 2020 2020 7c20 5468 6520  }}`       | The 
+00004e30: 506c 6174 666f 726d 2060 7572 6c60 2070  Platform `url` p
+00004e40: 726f 7065 7274 792e 2020 2020 2020 2020  roperty.        
 00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 7c0a 0a46 6f72 2074 6865 2060 6461 7465  |..For the `date
-00004ea0: 602c 2060 7469 6d65 602c 2060 6461 7465  `, `time`, `date
-00004eb0: 7469 6d65 6020 616e 6420 6072 616e 646f  time` and `rando
-00004ec0: 6d60 2064 6972 6563 7469 7665 732c 2074  m` directives, t
-00004ed0: 6865 2073 616d 6520 7661 6c75 6573 2077  he same values w
-00004ee0: 696c 6c20 6265 2075 7365 6420 666f 7220  ill be used for 
-00004ef0: 7468 6520 6475 7261 7469 6f6e 206f 6620  the duration of 
-00004f00: 6120 636f 6d6d 616e 6420 2d2d 2069 2e65  a command -- i.e
-00004f10: 2e2c 2069 6620 607b 7b74 696d 657d 7d60  ., if `{{time}}`
-00004f20: 2069 7320 7573 6564 2077 6974 6869 6e20   is used within 
-00004f30: 6d75 6c74 6970 6c65 2070 726f 7065 7274  multiple propert
-00004f40: 6965 732c 2074 6865 2073 616d 6520 7661  ies, the same va
-00004f50: 6c75 6520 7769 6c6c 2062 6520 7573 6564  lue will be used
-00004f60: 2066 6f72 2065 6163 6820 7375 6273 7469   for each substi
-00004f70: 7475 7469 6f6e 2e0a 0a23 2320 5573 6572  tution...## User
-00004f80: 2d44 6566 696e 6564 2056 6172 6961 626c  -Defined Variabl
-00004f90: 6573 0a0a 4172 6269 7472 6172 7920 7661  es..Arbitrary va
-00004fa0: 7269 6162 6c65 7320 6361 6e20 6265 2073  riables can be s
-00004fb0: 7570 706c 6965 6420 7573 696e 6720 636f  upplied using co
-00004fc0: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
-00004fd0: 6e73 2c20 6279 2073 6574 7469 6e67 2065  ns, by setting e
-00004fe0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00004ff0: 626c 6573 2070 7265 6669 7865 6420 7769  bles prefixed wi
-00005000: 7468 2060 5944 5f56 4152 5f60 2c20 6f72  th `YD_VAR_`, or
-00005010: 2062 7920 696e 636c 7564 696e 6720 7468   by including th
-00005020: 6520 6469 7265 6374 6976 6573 2069 6e20  e directives in 
-00005030: 7468 6520 605b 636f 6d6d 6f6e 5d60 2073  the `[common]` s
-00005040: 6563 7469 6f6e 206f 6620 7468 6520 544f  ection of the TO
-00005050: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-00005060: 2066 696c 652e 0a0a 312e 2054 6865 202a   file...1. The *
-00005070: 2a63 6f6d 6d61 6e64 206c 696e 652a 2a20  *command line** 
-00005080: 6f70 7469 6f6e 2069 7320 602d 2d76 6172  option is `--var
-00005090: 6961 626c 6560 2028 6f72 2060 2d76 6029  iable` (or `-v`)
-000050a0: 2e20 466f 7220 6578 616d 706c 652c 2060  . For example, `
-000050b0: 7964 2d73 7562 6d69 7420 2d76 2070 726f  yd-submit -v pro
-000050c0: 6a65 6374 5f63 6f64 653d 7072 2d32 3133  ject_code=pr-213
-000050d0: 2d61 202d 7620 7275 6e5f 6964 3d31 3233  -a -v run_id=123
-000050e0: 3460 2077 696c 6c20 6573 7461 626c 6973  4` will establis
-000050f0: 6820 7477 6f20 6e65 7720 7661 7269 6162  h two new variab
-00005100: 6c65 7320 7468 6174 2063 616e 2062 6520  les that can be 
-00005110: 7573 6564 2061 7320 607b 7b70 726f 6a65  used as `{{proje
-00005120: 6374 5f63 6f64 657d 7d60 2061 6e64 2060  ct_code}}` and `
-00005130: 7b7b 7275 6e5f 6964 7d7d 602c 2077 6869  {{run_id}}`, whi
-00005140: 6368 2077 696c 6c20 6265 2073 7562 7374  ch will be subst
-00005150: 6974 7574 6564 2062 7920 6070 722d 3231  ituted by `pr-21
-00005160: 332d 6160 2061 6e64 2060 3132 3334 6020  3-a` and `1234` 
-00005170: 7265 7370 6563 7469 7665 6c79 2e0a 0a0a  respectively....
-00005180: 322e 2046 6f72 202a 2a65 6e76 6972 6f6e  2. For **environ
-00005190: 6d65 6e74 2076 6172 6961 626c 6573 2a2a  ment variables**
-000051a0: 2c20 7365 7474 696e 6720 7468 6520 7661  , setting the va
-000051b0: 7269 6162 6c65 2060 5944 5f56 4152 5f70  riable `YD_VAR_p
-000051c0: 726f 6a65 6374 5f63 6f64 653d 2270 722d  roject_code="pr-
-000051d0: 3231 332d 6122 6020 7769 6c6c 2063 7265  213-a"` will cre
-000051e0: 6174 6520 6120 6e65 7720 7661 7269 6162  ate a new variab
-000051f0: 6c65 2074 6861 7420 6361 6e20 6265 2075  le that can be u
-00005200: 7365 6420 6173 2060 7b7b 7072 6f6a 6563  sed as `{{projec
-00005210: 745f 636f 6465 7d7d 602c 2077 6869 6368  t_code}}`, which
-00005220: 2077 696c 6c20 6265 2073 7562 7374 6974   will be substit
-00005230: 7574 6564 2062 7920 6070 722d 3231 332d  uted by `pr-213-
-00005240: 6160 2e0a 0a0a 332e 2046 6f72 202a 2a73  a`....3. For **s
-00005250: 6574 7469 6e67 2077 6974 6869 6e20 7468  etting within th
-00005260: 6520 544f 4d4c 2066 696c 652a 2a2c 2069  e TOML file**, i
-00005270: 6e63 6c75 6465 2061 202a 2a60 7661 7269  nclude a **`vari
-00005280: 6162 6c65 7360 2a2a 2074 6162 6c65 2069  ables`** table i
-00005290: 6e20 7468 6520 605b 636f 6d6d 6f6e 5d60  n the `[common]`
-000052a0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-000052b0: 6669 6c65 2e20 452e 672e 2c20 6076 6172  file. E.g., `var
-000052c0: 6961 626c 6573 203d 207b 7072 6f6a 6563  iables = {projec
-000052d0: 745f 636f 6465 203d 2022 7072 2d32 3133  t_code = "pr-213
-000052e0: 6122 2c20 7275 6e5f 6964 203d 2022 3132  a", run_id = "12
-000052f0: 3334 227d 602e 204e 6f74 6520 7468 6174  34"}`. Note that
-00005300: 2074 6869 7320 6361 6e20 616c 736f 2075   this can also u
-00005310: 7365 2074 6865 2066 6f72 6d3a 0a0a 6060  se the form:..``
-00005320: 6074 6f6d 6c0a 5b63 6f6d 6d6f 6e2e 7661  `toml.[common.va
-00005330: 7269 6162 6c65 735d 0a70 726f 6a65 6374  riables].project
-00005340: 5f63 6f64 6520 3d20 2270 722d 3231 3361  _code = "pr-213a
-00005350: 220a 7275 6e5f 6964 203d 2022 3132 3334  ".run_id = "1234
-00005360: 220a 6060 600a 0a44 6972 6563 7469 7665  ".```..Directive
-00005370: 7320 7365 7420 6f6e 2074 6865 2063 6f6d  s set on the com
-00005380: 6d61 6e64 206c 696e 6520 7461 6b65 2070  mand line take p
-00005390: 7265 6365 6465 6e63 6520 6f76 6572 2064  recedence over d
-000053a0: 6972 6563 7469 7665 7320 7365 7420 696e  irectives set in
-000053b0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-000053c0: 6961 626c 6573 2c20 616e 6420 626f 7468  iables, and both
-000053d0: 206f 6620 7468 656d 2074 616b 6520 7072   of them take pr
-000053e0: 6563 6564 656e 6365 206f 7665 7220 6469  ecedence over di
-000053f0: 7265 6374 6976 6573 2073 6574 2069 6e20  rectives set in 
-00005400: 6120 544f 4d4c 2066 696c 652e 0a0a 5468  a TOML file...Th
-00005410: 6973 206d 6574 686f 6420 6361 6e20 6265  is method can be
-00005420: 2075 7365 6420 746f 206f 7665 7272 6964   used to overrid
-00005430: 6520 7468 6520 6465 6661 756c 7420 6469  e the default di
-00005440: 7265 6374 6976 6573 2c20 652e 672e 2c20  rectives, e.g., 
-00005450: 7365 7474 696e 6720 602d 7620 7573 6572  setting `-v user
-00005460: 6e61 6d65 3d22 6f74 6865 722d 7573 6572  name="other-user
-00005470: 2260 2077 696c 6c20 6f76 6572 7269 6465  "` will override
-00005480: 2074 6865 2064 6566 6175 6c74 2060 7b7b   the default `{{
-00005490: 7573 6572 6e61 6d65 7d7d 6020 6469 7265  username}}` dire
-000054a0: 6374 6976 652e 0a0a 2323 204e 6573 7465  ctive...## Neste
-000054b0: 6420 5661 7269 6162 6c65 730a 0a49 6e20  d Variables..In 
-000054c0: 7468 6520 6361 7365 206f 6620 2a2a 544f  the case of **TO
-000054d0: 4d4c 2070 726f 7065 7274 6965 7320 6f6e  ML properties on
-000054e0: 6c79 2a2a 2c20 7661 7269 6162 6c65 2073  ly**, variable s
-000054f0: 7562 7374 6974 7574 696f 6e73 2063 616e  ubstitutions can
-00005500: 2062 6520 6e65 7374 6564 2e0a 0a46 6f72   be nested...For
-00005510: 2065 7861 6d70 6c65 2c20 6966 206f 6e65   example, if one
-00005520: 2077 616e 7465 6420 746f 2073 656c 6563   wanted to selec
-00005530: 7420 6120 6469 6666 6572 656e 7420 6074  t a different `t
-00005540: 656d 706c 6174 6549 6460 2066 6f72 2061  emplateId` for a
-00005550: 2057 6f72 6b65 7220 506f 6f6c 2064 6570   Worker Pool dep
-00005560: 656e 6469 6e67 206f 6e20 7468 6520 7661  ending on the va
-00005570: 6c75 6520 6f66 2061 2060 7265 6769 6f6e  lue of a `region
-00005580: 6020 7661 7269 6162 6c65 2c20 6f6e 6520  ` variable, one 
-00005590: 636f 756c 6420 7573 6520 7468 6520 666f  could use the fo
-000055a0: 6c6c 6f77 696e 673a 0a0a 6060 6074 6f6d  llowing:..```tom
-000055b0: 6c0a 5b63 6f6d 6d6f 6e2e 7661 7269 6162  l.[common.variab
-000055c0: 6c65 735d 0a20 2020 2074 656d 706c 6174  les].    templat
-000055d0: 655f 6c6f 6e64 6f6e 203d 2022 7964 6964  e_london = "ydid
-000055e0: 3a63 7274 3a36 3545 4634 463a 6134 6437  :crt:65EF4F:a4d7
-000055f0: 3537 6366 2d62 3637 612d 3465 6236 2d62  57cf-b67a-4eb6-b
-00005600: 6433 392d 3861 3666 6664 3436 6338 6634  d39-8a6ffd46c8f4
-00005610: 220a 2020 2020 7465 6d70 6c61 7465 5f70  ".    template_p
-00005620: 686f 656e 6978 203d 2022 7964 6964 3a63  hoenix = "ydid:c
-00005630: 7274 3a36 3545 4634 463a 6534 3233 3964  rt:65EF4F:e4239d
-00005640: 6563 2d37 3863 322d 3432 3163 2d61 3766  ec-78c2-421c-a7f
-00005650: 332d 3731 6536 3162 3732 3934 3666 220a  3-71e61b72946f".
-00005660: 2020 2020 7465 6d70 6c61 7465 5f66 7261      template_fra
-00005670: 6e6b 6675 7274 203d 2022 7964 6964 3a63  nkfurt = "ydid:c
-00005680: 7274 3a36 3545 4634 463a 3332 3936 3032  rt:65EF4F:329602
-00005690: 6366 2d35 3934 352d 3461 6164 2d61 3238  cf-5945-4aad-a28
-000056a0: 382d 6561 3432 3464 3634 6435 3565 220a  8-ea424d64d55e".
-000056b0: 0a5b 636f 6d6d 6f6e 2e77 6f72 6b65 7250  .[common.workerP
-000056c0: 6f6f 6c5d 0a20 2020 2074 656d 706c 6174  ool].    templat
-000056d0: 6549 6420 3d20 227b 7b74 656d 706c 6174  eId = "{{templat
-000056e0: 655f 7b7b 7265 6769 6f6e 7d7d 7d7d 220a  e_{{region}}}}".
-000056f0: 6060 600a 0a54 6865 6e2c 2069 6620 6f6e  ```..Then, if on
-00005700: 6520 7573 6564 2060 7964 2d70 726f 7669  e used `yd-provi
-00005710: 7369 6f6e 202d 7620 7265 6769 6f6e 3d70  sion -v region=p
-00005720: 686f 656e 6978 602c 2074 6865 2060 7465  hoenix`, the `te
-00005730: 6d70 6c61 7465 4964 6020 7072 6f70 6572  mplateId` proper
-00005740: 7479 2077 6f75 6c64 2066 6972 7374 2072  ty would first r
-00005750: 6573 6f6c 7665 2074 6f20 6022 7b7b 7465  esolve to `"{{te
-00005760: 6d70 6c61 7465 5f70 6865 6f6e 6978 7d7d  mplate_pheonix}}
-00005770: 2260 2c20 616e 6420 7468 656e 2074 6f20  "`, and then to 
-00005780: 6022 7964 6964 3a63 7274 3a36 3545 4634  `"ydid:crt:65EF4
-00005790: 463a 6534 3233 3964 6563 2d37 3863 322d  F:e4239dec-78c2-
-000057a0: 3432 3163 2d61 3766 332d 3731 6536 3162  421c-a7f3-71e61b
-000057b0: 3732 3934 3666 2260 2e0a 0a4e 6573 7469  72946f"`...Nesti
-000057c0: 6e67 2063 616e 2062 6520 7570 2074 6f20  ng can be up to 
-000057d0: 7468 7265 6520 6c65 7665 6c73 2064 6565  three levels dee
-000057e0: 7020 696e 636c 7564 696e 6720 7468 6520  p including the 
-000057f0: 746f 7020 6c65 7665 6c2e 0a0a 2320 576f  top level...# Wo
-00005800: 726b 2052 6571 7569 7265 6d65 6e74 2050  rk Requirement P
-00005810: 726f 7065 7274 6965 730a 0a54 6865 2060  roperties..The `
-00005820: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
-00005830: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-00005840: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00005850: 6c65 2069 7320 6f70 7469 6f6e 616c 2e20  le is optional. 
-00005860: 4974 2773 2075 7365 6420 6f6e 6c79 2062  It's used only b
-00005870: 7920 7468 6520 6079 642d 7375 626d 6974  y the `yd-submit
-00005880: 6020 636f 6d6d 616e 642c 2061 6e64 2063  ` command, and c
-00005890: 6f6e 7472 6f6c 7320 7468 6520 576f 726b  ontrols the Work
-000058a0: 2052 6571 7569 7265 6d65 6e74 2074 6861   Requirement tha
-000058b0: 7420 6973 2073 7562 6d69 7474 6564 2074  t is submitted t
-000058c0: 6f20 7468 6520 506c 6174 666f 726d 2e0a  o the Platform..
-000058d0: 0a54 6865 2064 6574 6169 6c73 206f 6620  .The details of 
-000058e0: 6120 576f 726b 2052 6571 7569 7265 6d65  a Work Requireme
-000058f0: 6e74 2074 6f20 6265 2073 7562 6d69 7474  nt to be submitt
-00005900: 6564 2063 616e 2062 6520 6361 7074 7572  ed can be captur
-00005910: 6564 2065 6e74 6972 656c 7920 7769 7468  ed entirely with
-00005920: 696e 2074 6865 2054 4f4d 4c20 636f 6e66  in the TOML conf
-00005930: 6967 7572 6174 696f 6e20 6669 6c65 2066  iguration file f
-00005940: 6f72 2073 696d 706c 6520 6578 616d 706c  or simple exampl
-00005950: 6573 2e20 4d6f 7265 2063 6f6d 706c 6578  es. More complex
-00005960: 2065 7861 6d70 6c65 7320 6361 7074 7572   examples captur
-00005970: 6520 7468 6520 576f 726b 2052 6571 7569  e the Work Requi
-00005980: 7265 6d65 6e74 2069 6e20 6120 636f 6d62  rement in a comb
-00005990: 696e 6174 696f 6e20 6f66 2074 6865 2054  ination of the T
-000059a0: 4f4d 4c20 6669 6c65 2070 6c75 7320 6120  OML file plus a 
-000059b0: 4a53 4f4e 2064 6f63 756d 656e 742c 206f  JSON document, o
-000059c0: 7220 696e 2061 204a 534f 4e20 646f 6375  r in a JSON docu
-000059d0: 6d65 6e74 206f 6e6c 792e 0a0a 2323 2057  ment only...## W
-000059e0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-000059f0: 4a53 4f4e 2046 696c 6520 5374 7275 6374  JSON File Struct
-00005a00: 7572 650a 0a57 6f72 6b20 5265 7175 6972  ure..Work Requir
-00005a10: 656d 656e 7473 2061 7265 2072 6570 7265  ements are repre
-00005a20: 7365 6e74 6564 2069 6e20 4a53 4f4e 2064  sented in JSON d
-00005a30: 6f63 756d 656e 7473 2075 7369 6e67 2061  ocuments using a
-00005a40: 2063 6f6e 7461 696e 6d65 6e74 2068 6965   containment hie
-00005a50: 7261 7263 6879 206f 6620 6120 2a2a 576f  rarchy of a **Wo
-00005a60: 726b 2052 6571 7569 7265 6d65 6e74 2a2a  rk Requirement**
-00005a70: 2063 6f6e 7461 696e 696e 6720 6120 2a2a   containing a **
-00005a80: 6c69 7374 206f 6620 5461 736b 2047 726f  list of Task Gro
-00005a90: 7570 732a 2a2c 2063 6f6e 7461 696e 696e  ups**, containin
-00005aa0: 6720 6120 2a2a 6c69 7374 206f 6620 5461  g a **list of Ta
-00005ab0: 736b 732a 2a2e 0a0a 4120 7665 7279 2073  sks**...A very s
-00005ac0: 696d 706c 6520 6578 616d 706c 6520 646f  imple example do
-00005ad0: 6375 6d65 6e74 2069 7320 7368 6f77 6e20  cument is shown 
-00005ae0: 6265 6c6f 7720 7769 7468 2061 2074 6f70  below with a top
-00005af0: 2d6c 6576 656c 2057 6f72 6b20 5265 7175  -level Work Requ
-00005b00: 6972 656d 656e 7420 636f 6e74 6169 6e69  irement containi
-00005b10: 6e67 2074 776f 2054 6173 6b20 4772 6f75  ng two Task Grou
-00005b20: 7073 2065 6163 6820 636f 6e74 6169 6e69  ps each containi
-00005b30: 6e67 2074 776f 2054 6173 6b73 2c20 6561  ng two Tasks, ea
-00005b40: 6368 2077 6974 6820 6120 6469 6666 6572  ch with a differ
-00005b50: 656e 7420 7365 7420 6f66 2061 7267 756d  ent set of argum
-00005b60: 656e 7473 2074 6f20 6265 2070 6173 7365  ents to be passe
-00005b70: 6420 746f 2074 6865 2054 6173 6b2e 0a0a  d to the Task...
-00005b80: 6060 606a 736f 6e0a 7b0a 2020 2274 6173  ```json.{.  "tas
-00005b90: 6b47 726f 7570 7322 3a20 5b0a 2020 2020  kGroups": [.    
-00005ba0: 7b0a 2020 2020 2020 2274 6173 6b73 223a  {.      "tasks":
-00005bb0: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
-00005bc0: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
-00005bd0: 7322 3a20 5b31 2c20 322c 2033 5d0a 2020  s": [1, 2, 3].  
-00005be0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00005bf0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-00005c00: 6775 6d65 6e74 7322 3a20 5b34 2c20 352c  guments": [4, 5,
-00005c10: 2036 5d0a 2020 2020 2020 2020 7d0a 2020   6].        }.  
-00005c20: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
-00005c30: 207b 0a20 2020 2020 2022 7461 736b 7322   {.      "tasks"
-00005c40: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00005c50: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00005c60: 7473 223a 205b 372c 2038 2c20 395d 0a20  ts": [7, 8, 9]. 
-00005c70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00005c80: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
-00005c90: 7267 756d 656e 7473 223a 205b 3130 2c20  rguments": [10, 
-00005ca0: 3131 2c20 3132 5d0a 2020 2020 2020 2020  11, 12].        
-00005cb0: 7d0a 2020 2020 2020 5d0a 2020 2020 7d0a  }.      ].    }.
-00005cc0: 2020 5d0a 7d0a 0a60 6060 0a0a 546f 2073    ].}..```..To s
-00005cd0: 7065 6369 6679 2074 6865 2066 696c 6520  pecify the file 
-00005ce0: 636f 6e74 6169 6e69 6e67 2074 6865 204a  containing the J
-00005cf0: 534f 4e20 646f 6375 6d65 6e74 2c20 6569  SON document, ei
-00005d00: 7468 6572 2070 6f70 756c 6174 6520 7468  ther populate th
-00005d10: 6520 6077 6f72 6b52 6571 7569 7265 6d65  e `workRequireme
-00005d20: 6e74 4461 7461 6020 7072 6f70 6572 7479  ntData` property
-00005d30: 2069 6e20 7468 6520 6077 6f72 6b52 6571   in the `workReq
-00005d40: 7569 7265 6d65 6e74 6020 7365 6374 696f  uirement` sectio
-00005d50: 6e20 6f66 2074 6865 2054 4f4d 4c20 636f  n of the TOML co
-00005d60: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00005d70: 2077 6974 6820 7468 6520 4a53 4f4e 2066   with the JSON f
-00005d80: 696c 656e 616d 652c 206f 7220 7370 6563  ilename, or spec
-00005d90: 6966 7920 6974 206f 6e20 7468 6520 636f  ify it on the co
-00005da0: 6d6d 616e 6420 6c69 6e65 2075 7369 6e67  mmand line using
-00005db0: 2074 6865 2060 2d2d 776f 726b 2d72 6571   the `--work-req
-00005dc0: 7569 7265 6d65 6e74 6020 6f72 2060 2d72  uirement` or `-r
-00005dd0: 6020 6f70 7469 6f6e 7320 2877 6869 6368  ` options (which
-00005de0: 2077 696c 6c20 6f76 6572 7269 6465 2074   will override t
-00005df0: 6865 2070 726f 7065 7274 7920 696e 2074  he property in t
-00005e00: 6865 2054 4f4d 4c20 6669 6c65 292c 2065  he TOML file), e
-00005e10: 2e67 2e0a 0a60 7964 2d73 7562 6d69 7420  .g...`yd-submit 
-00005e20: 2d2d 636f 6e66 6967 206d 7963 6f6e 6669  --config myconfi
-00005e30: 672e 746f 6d6c 202d 2d77 6f72 6b2d 7265  g.toml --work-re
-00005e40: 7175 6972 656d 656e 7420 6d79 5f77 6f72  quirement my_wor
-00005e50: 6b72 6571 2e6a 736f 6e60 0a0a 2323 2050  kreq.json`..## P
-00005e60: 726f 7065 7274 7920 496e 6865 7269 7461  roperty Inherita
-00005e70: 6e63 650a 0a54 6f20 7369 6d70 6c69 6679  nce..To simplify
-00005e80: 2074 6865 2064 6566 696e 6974 696f 6e20   the definition 
-00005e90: 6f66 2057 6f72 6b20 5265 7175 6972 656d  of Work Requirem
-00005ea0: 656e 7473 2c20 7468 6572 6520 6973 2061  ents, there is a
-00005eb0: 2070 726f 7065 7274 7920 696e 6865 7269   property inheri
-00005ec0: 7461 6e63 6520 6d65 6368 616e 6973 6d2e  tance mechanism.
-00005ed0: 2050 726f 7065 7274 6965 7320 7468 6174   Properties that
-00005ee0: 2061 7265 2073 6574 2061 7420 6120 6869   are set at a hi
-00005ef0: 6768 6572 206c 6576 656c 2069 6e20 7468  gher level in th
-00005f00: 6520 6869 6572 6172 6368 7920 6172 6520  e hierarchy are 
-00005f10: 696e 6865 7269 7465 6420 6174 206c 6f77  inherited at low
-00005f20: 6572 206c 6576 656c 732c 2075 6e6c 6573  er levels, unles
-00005f30: 7320 6578 706c 6963 6974 6c79 206f 7665  s explicitly ove
-00005f40: 7272 6964 6465 6e2e 0a0a 5468 6973 206d  rridden...This m
-00005f50: 6561 6e73 2074 6861 7420 6120 7072 6f70  eans that a prop
-00005f60: 6572 7479 2073 6574 2069 6e20 7468 6520  erty set in the 
-00005f70: 6077 6f72 6b52 6571 7569 7265 6d65 6e74  `workRequirement
-00005f80: 6020 7365 6374 696f 6e20 6f66 2074 6865  ` section of the
-00005f90: 2054 4f4d 4c20 6669 6c65 2063 616e 2062   TOML file can b
-00005fa0: 6520 696e 6865 7269 7465 6420 7375 6363  e inherited succ
-00005fb0: 6573 7369 7665 6c79 2062 7920 7468 6520  essively by the 
-00005fc0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00005fd0: 2c20 5461 736b 2047 726f 7570 7320 616e  , Task Groups an
-00005fe0: 6420 5461 736b 7320 696e 2074 6865 204a  d Tasks in the J
-00005ff0: 534f 4e20 646f 6375 6d65 6e74 2028 6173  SON document (as
-00006000: 7375 6d69 6e67 2074 6865 2070 726f 7065  suming the prope
-00006010: 7274 7920 6973 2076 616c 6964 2061 7420  rty is valid at 
-00006020: 6561 6368 206c 6576 656c 292e 2020 4865  each level).  He
-00006030: 6e63 652c 2054 6173 6b73 2069 6e68 6572  nce, Tasks inher
-00006040: 6974 2066 726f 6d20 5461 736b 2047 726f  it from Task Gro
-00006050: 7570 732c 2077 6869 6368 2069 6e68 6572  ups, which inher
-00006060: 6974 2066 726f 6d20 7468 6520 576f 726b  it from the Work
-00006070: 2052 6571 7569 7265 6d65 6e74 2069 6e20   Requirement in 
-00006080: 7468 6520 4a53 4f4e 2064 6f63 756d 656e  the JSON documen
-00006090: 742c 2077 6869 6368 2069 6e68 6572 6974  t, which inherit
-000060a0: 7320 6672 6f6d 2074 6865 2060 776f 726b  s from the `work
-000060b0: 5265 7175 6972 656d 656e 7460 2070 726f  Requirement` pro
-000060c0: 7065 7274 6965 7320 696e 2074 6865 2054  perties in the T
-000060d0: 4f4d 4c20 6669 6c65 2e0a 0a4f 7665 7272  OML file...Overr
-000060e0: 6964 6465 6e20 7072 6f70 6572 7469 6573  idden properties
-000060f0: 2061 7265 2061 6c73 6f20 696e 6865 7269   are also inheri
-00006100: 7465 642e 2045 2e67 2e2c 2069 6620 6120  ted. E.g., if a 
-00006110: 7072 6f70 6572 7479 2069 7320 7365 7420  property is set 
-00006120: 6174 2074 6865 2054 6173 6b20 4772 6f75  at the Task Grou
-00006130: 7020 6c65 7665 6c2c 2069 7420 7769 6c6c  p level, it will
-00006140: 2062 6520 696e 6865 7269 7465 6420 6279   be inherited by
-00006150: 2074 6865 2054 6173 6b73 2069 6e20 7468   the Tasks in th
-00006160: 6174 2054 6173 6b20 4772 6f75 7020 756e  at Task Group un
-00006170: 6c65 7373 2065 7870 6c69 6369 746c 7920  less explicitly 
-00006180: 6f76 6572 7269 6464 656e 2e0a 0a23 2320  overridden...## 
-00006190: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-000061a0: 2050 726f 7065 7274 7920 4469 6374 696f   Property Dictio
-000061b0: 6e61 7279 0a0a 5468 6520 666f 6c6c 6f77  nary..The follow
-000061c0: 696e 6720 7461 626c 6520 6f75 746c 696e  ing table outlin
-000061d0: 6573 2061 6c6c 2074 6865 2070 726f 7065  es all the prope
-000061e0: 7274 6965 7320 6176 6169 6c61 626c 6520  rties available 
-000061f0: 666f 7220 6465 6669 6e69 6e67 2057 6f72  for defining Wor
-00006200: 6b20 5265 7175 6972 656d 656e 7473 2c20  k Requirements, 
-00006210: 616e 6420 7468 6520 6c65 7665 6c73 2061  and the levels a
-00006220: 7420 7768 6963 6820 7468 6579 2061 7265  t which they are
-00006230: 2061 6c6c 6f77 6564 2074 6f20 6265 2075   allowed to be u
-00006240: 7365 642e 2053 6f2c 2066 6f72 2065 7861  sed. So, for exa
-00006250: 6d70 6c65 2c20 7468 6520 6070 726f 7669  mple, the `provi
-00006260: 6465 7260 2070 726f 7065 7274 7920 6361  der` property ca
-00006270: 6e20 6265 2073 6574 2069 6e20 7468 6520  n be set in the 
-00006280: 544f 4d4c 2066 696c 652c 2061 7420 7468  TOML file, at th
-00006290: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-000062a0: 6e74 204c 6576 656c 206f 7220 6174 2074  nt Level or at t
-000062b0: 6865 2054 6173 6b20 4772 6f75 7020 4c65  he Task Group Le
-000062c0: 7665 6c2c 2062 7574 206e 6f74 2061 7420  vel, but not at 
-000062d0: 7468 6520 5461 736b 206c 6576 656c 2c20  the Task level, 
-000062e0: 616e 6420 7072 6f70 6572 7479 2060 6465  and property `de
-000062f0: 7065 6e64 656e 744f 6e60 2063 616e 206f  pendentOn` can o
-00006300: 6e6c 7920 6265 2073 6574 2061 7420 7468  nly be set at th
-00006310: 6520 5461 736b 2047 726f 7570 206c 6576  e Task Group lev
-00006320: 656c 2e0a 0a41 6c6c 2070 726f 7065 7274  el...All propert
-00006330: 6965 7320 6172 6520 6f70 7469 6f6e 616c  ies are optional
-00006340: 2065 7863 6570 7420 666f 7220 2a2a 6074   except for **`t
-00006350: 6173 6b54 7970 6560 2a2a 2028 6f72 202a  askType`** (or *
-00006360: 2a60 7461 736b 5479 7065 7360 2a2a 292e  *`taskTypes`**).
-00006370: 0a0a 7c20 5072 6f70 6572 7479 204e 616d  ..| Property Nam
-00006380: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
-00006390: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
+00004e70: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00004e80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004e90: 0a0a 466f 7220 7468 6520 6064 6174 6560  ..For the `date`
+00004ea0: 2c20 6074 696d 6560 2c20 6064 6174 6574  , `time`, `datet
+00004eb0: 696d 6560 2061 6e64 2060 7261 6e64 6f6d  ime` and `random
+00004ec0: 6020 6469 7265 6374 6976 6573 2c20 7468  ` directives, th
+00004ed0: 6520 7361 6d65 2076 616c 7565 7320 7769  e same values wi
+00004ee0: 6c6c 2062 6520 7573 6564 2066 6f72 2074  ll be used for t
+00004ef0: 6865 2064 7572 6174 696f 6e20 6f66 2061  he duration of a
+00004f00: 2063 6f6d 6d61 6e64 202d 2d20 692e 652e   command -- i.e.
+00004f10: 2c20 6966 2060 7b7b 7469 6d65 7d7d 6020  , if `{{time}}` 
+00004f20: 6973 2075 7365 6420 7769 7468 696e 206d  is used within m
+00004f30: 756c 7469 706c 6520 7072 6f70 6572 7469  ultiple properti
+00004f40: 6573 2c20 7468 6520 7361 6d65 2076 616c  es, the same val
+00004f50: 7565 2077 696c 6c20 6265 2075 7365 6420  ue will be used 
+00004f60: 666f 7220 6561 6368 2073 7562 7374 6974  for each substit
+00004f70: 7574 696f 6e2e 0a0a 2323 2055 7365 722d  ution...## User-
+00004f80: 4465 6669 6e65 6420 5661 7269 6162 6c65  Defined Variable
+00004f90: 730a 0a41 7262 6974 7261 7279 2076 6172  s..Arbitrary var
+00004fa0: 6961 626c 6573 2063 616e 2062 6520 7375  iables can be su
+00004fb0: 7070 6c69 6564 2075 7369 6e67 2063 6f6d  pplied using com
+00004fc0: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
+00004fd0: 732c 2062 7920 7365 7474 696e 6720 656e  s, by setting en
+00004fe0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00004ff0: 6c65 7320 7072 6566 6978 6564 2077 6974  les prefixed wit
+00005000: 6820 6059 445f 5641 525f 602c 206f 7220  h `YD_VAR_`, or 
+00005010: 6279 2069 6e63 6c75 6469 6e67 2074 6865  by including the
+00005020: 2064 6972 6563 7469 7665 7320 696e 2074   directives in t
+00005030: 6865 2060 5b63 6f6d 6d6f 6e5d 6020 7365  he `[common]` se
+00005040: 6374 696f 6e20 6f66 2074 6865 2054 4f4d  ction of the TOM
+00005050: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+00005060: 6669 6c65 2e0a 0a31 2e20 5468 6520 2a2a  file...1. The **
+00005070: 636f 6d6d 616e 6420 6c69 6e65 2a2a 206f  command line** o
+00005080: 7074 696f 6e20 6973 2060 2d2d 7661 7269  ption is `--vari
+00005090: 6162 6c65 6020 286f 7220 602d 7660 292e  able` (or `-v`).
+000050a0: 2046 6f72 2065 7861 6d70 6c65 2c20 6079   For example, `y
+000050b0: 642d 7375 626d 6974 202d 7620 7072 6f6a  d-submit -v proj
+000050c0: 6563 745f 636f 6465 3d70 722d 3231 332d  ect_code=pr-213-
+000050d0: 6120 2d76 2072 756e 5f69 643d 3132 3334  a -v run_id=1234
+000050e0: 6020 7769 6c6c 2065 7374 6162 6c69 7368  ` will establish
+000050f0: 2074 776f 206e 6577 2076 6172 6961 626c   two new variabl
+00005100: 6573 2074 6861 7420 6361 6e20 6265 2075  es that can be u
+00005110: 7365 6420 6173 2060 7b7b 7072 6f6a 6563  sed as `{{projec
+00005120: 745f 636f 6465 7d7d 6020 616e 6420 607b  t_code}}` and `{
+00005130: 7b72 756e 5f69 647d 7d60 2c20 7768 6963  {run_id}}`, whic
+00005140: 6820 7769 6c6c 2062 6520 7375 6273 7469  h will be substi
+00005150: 7475 7465 6420 6279 2060 7072 2d32 3133  tuted by `pr-213
+00005160: 2d61 6020 616e 6420 6031 3233 3460 2072  -a` and `1234` r
+00005170: 6573 7065 6374 6976 656c 792e 0a0a 0a32  espectively....2
+00005180: 2e20 466f 7220 2a2a 656e 7669 726f 6e6d  . For **environm
+00005190: 656e 7420 7661 7269 6162 6c65 732a 2a2c  ent variables**,
+000051a0: 2073 6574 7469 6e67 2074 6865 2076 6172   setting the var
+000051b0: 6961 626c 6520 6059 445f 5641 525f 7072  iable `YD_VAR_pr
+000051c0: 6f6a 6563 745f 636f 6465 3d22 7072 2d32  oject_code="pr-2
+000051d0: 3133 2d61 2260 2077 696c 6c20 6372 6561  13-a"` will crea
+000051e0: 7465 2061 206e 6577 2076 6172 6961 626c  te a new variabl
+000051f0: 6520 7468 6174 2063 616e 2062 6520 7573  e that can be us
+00005200: 6564 2061 7320 607b 7b70 726f 6a65 6374  ed as `{{project
+00005210: 5f63 6f64 657d 7d60 2c20 7768 6963 6820  _code}}`, which 
+00005220: 7769 6c6c 2062 6520 7375 6273 7469 7475  will be substitu
+00005230: 7465 6420 6279 2060 7072 2d32 3133 2d61  ted by `pr-213-a
+00005240: 602e 0a0a 0a33 2e20 466f 7220 2a2a 7365  `....3. For **se
+00005250: 7474 696e 6720 7769 7468 696e 2074 6865  tting within the
+00005260: 2054 4f4d 4c20 6669 6c65 2a2a 2c20 696e   TOML file**, in
+00005270: 636c 7564 6520 6120 2a2a 6076 6172 6961  clude a **`varia
+00005280: 626c 6573 602a 2a20 7461 626c 6520 696e  bles`** table in
+00005290: 2074 6865 2060 5b63 6f6d 6d6f 6e5d 6020   the `[common]` 
+000052a0: 7365 6374 696f 6e20 6f66 2074 6865 2066  section of the f
+000052b0: 696c 652e 2045 2e67 2e2c 2060 7661 7269  ile. E.g., `vari
+000052c0: 6162 6c65 7320 3d20 7b70 726f 6a65 6374  ables = {project
+000052d0: 5f63 6f64 6520 3d20 2270 722d 3231 3361  _code = "pr-213a
+000052e0: 222c 2072 756e 5f69 6420 3d20 2231 3233  ", run_id = "123
+000052f0: 3422 7d60 2e20 4e6f 7465 2074 6861 7420  4"}`. Note that 
+00005300: 7468 6973 2063 616e 2061 6c73 6f20 7573  this can also us
+00005310: 6520 7468 6520 666f 726d 3a0a 0a60 6060  e the form:..```
+00005320: 746f 6d6c 0a5b 636f 6d6d 6f6e 2e76 6172  toml.[common.var
+00005330: 6961 626c 6573 5d0a 7072 6f6a 6563 745f  iables].project_
+00005340: 636f 6465 203d 2022 7072 2d32 3133 6122  code = "pr-213a"
+00005350: 0a72 756e 5f69 6420 3d20 2231 3233 3422  .run_id = "1234"
+00005360: 0a60 6060 0a0a 4469 7265 6374 6976 6573  .```..Directives
+00005370: 2073 6574 206f 6e20 7468 6520 636f 6d6d   set on the comm
+00005380: 616e 6420 6c69 6e65 2074 616b 6520 7072  and line take pr
+00005390: 6563 6564 656e 6365 206f 7665 7220 6469  ecedence over di
+000053a0: 7265 6374 6976 6573 2073 6574 2069 6e20  rectives set in 
+000053b0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+000053c0: 6162 6c65 732c 2061 6e64 2062 6f74 6820  ables, and both 
+000053d0: 6f66 2074 6865 6d20 7461 6b65 2070 7265  of them take pre
+000053e0: 6365 6465 6e63 6520 6f76 6572 2064 6972  cedence over dir
+000053f0: 6563 7469 7665 7320 7365 7420 696e 2061  ectives set in a
+00005400: 2054 4f4d 4c20 6669 6c65 2e0a 0a54 6869   TOML file...Thi
+00005410: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
+00005420: 7573 6564 2074 6f20 6f76 6572 7269 6465  used to override
+00005430: 2074 6865 2064 6566 6175 6c74 2064 6972   the default dir
+00005440: 6563 7469 7665 732c 2065 2e67 2e2c 2073  ectives, e.g., s
+00005450: 6574 7469 6e67 2060 2d76 2075 7365 726e  etting `-v usern
+00005460: 616d 653d 226f 7468 6572 2d75 7365 7222  ame="other-user"
+00005470: 6020 7769 6c6c 206f 7665 7272 6964 6520  ` will override 
+00005480: 7468 6520 6465 6661 756c 7420 607b 7b75  the default `{{u
+00005490: 7365 726e 616d 657d 7d60 2064 6972 6563  sername}}` direc
+000054a0: 7469 7665 2e0a 0a23 2320 4e65 7374 6564  tive...## Nested
+000054b0: 2056 6172 6961 626c 6573 0a0a 496e 2074   Variables..In t
+000054c0: 6865 2063 6173 6520 6f66 202a 2a54 4f4d  he case of **TOM
+000054d0: 4c20 7072 6f70 6572 7469 6573 206f 6e6c  L properties onl
+000054e0: 792a 2a2c 2076 6172 6961 626c 6520 7375  y**, variable su
+000054f0: 6273 7469 7475 7469 6f6e 7320 6361 6e20  bstitutions can 
+00005500: 6265 206e 6573 7465 642e 0a0a 466f 7220  be nested...For 
+00005510: 6578 616d 706c 652c 2069 6620 6f6e 6520  example, if one 
+00005520: 7761 6e74 6564 2074 6f20 7365 6c65 6374  wanted to select
+00005530: 2061 2064 6966 6665 7265 6e74 2060 7465   a different `te
+00005540: 6d70 6c61 7465 4964 6020 666f 7220 6120  mplateId` for a 
+00005550: 576f 726b 6572 2050 6f6f 6c20 6465 7065  Worker Pool depe
+00005560: 6e64 696e 6720 6f6e 2074 6865 2076 616c  nding on the val
+00005570: 7565 206f 6620 6120 6072 6567 696f 6e60  ue of a `region`
+00005580: 2076 6172 6961 626c 652c 206f 6e65 2063   variable, one c
+00005590: 6f75 6c64 2075 7365 2074 6865 2066 6f6c  ould use the fol
+000055a0: 6c6f 7769 6e67 3a0a 0a60 6060 746f 6d6c  lowing:..```toml
+000055b0: 0a5b 636f 6d6d 6f6e 2e76 6172 6961 626c  .[common.variabl
+000055c0: 6573 5d0a 2020 2020 7465 6d70 6c61 7465  es].    template
+000055d0: 5f6c 6f6e 646f 6e20 3d20 2279 6469 643a  _london = "ydid:
+000055e0: 6372 743a 3635 4546 3446 3a61 3464 3735  crt:65EF4F:a4d75
+000055f0: 3763 662d 6236 3761 2d34 6562 362d 6264  7cf-b67a-4eb6-bd
+00005600: 3339 2d38 6136 6666 6434 3663 3866 3422  39-8a6ffd46c8f4"
+00005610: 0a20 2020 2074 656d 706c 6174 655f 7068  .    template_ph
+00005620: 6f65 6e69 7820 3d20 2279 6469 643a 6372  oenix = "ydid:cr
+00005630: 743a 3635 4546 3446 3a65 3432 3339 6465  t:65EF4F:e4239de
+00005640: 632d 3738 6332 2d34 3231 632d 6137 6633  c-78c2-421c-a7f3
+00005650: 2d37 3165 3631 6237 3239 3436 6622 0a20  -71e61b72946f". 
+00005660: 2020 2074 656d 706c 6174 655f 6672 616e     template_fran
+00005670: 6b66 7572 7420 3d20 2279 6469 643a 6372  kfurt = "ydid:cr
+00005680: 743a 3635 4546 3446 3a33 3239 3630 3263  t:65EF4F:329602c
+00005690: 662d 3539 3435 2d34 6161 642d 6132 3838  f-5945-4aad-a288
+000056a0: 2d65 6134 3234 6436 3464 3535 6522 0a0a  -ea424d64d55e"..
+000056b0: 5b63 6f6d 6d6f 6e2e 776f 726b 6572 506f  [common.workerPo
+000056c0: 6f6c 5d0a 2020 2020 7465 6d70 6c61 7465  ol].    template
+000056d0: 4964 203d 2022 7b7b 7465 6d70 6c61 7465  Id = "{{template
+000056e0: 5f7b 7b72 6567 696f 6e7d 7d7d 7d22 0a60  _{{region}}}}".`
+000056f0: 6060 0a0a 5468 656e 2c20 6966 206f 6e65  ``..Then, if one
+00005700: 2075 7365 6420 6079 642d 7072 6f76 6973   used `yd-provis
+00005710: 696f 6e20 2d76 2072 6567 696f 6e3d 7068  ion -v region=ph
+00005720: 6f65 6e69 7860 2c20 7468 6520 6074 656d  oenix`, the `tem
+00005730: 706c 6174 6549 6460 2070 726f 7065 7274  plateId` propert
+00005740: 7920 776f 756c 6420 6669 7273 7420 7265  y would first re
+00005750: 736f 6c76 6520 746f 2060 227b 7b74 656d  solve to `"{{tem
+00005760: 706c 6174 655f 7068 656f 6e69 787d 7d22  plate_pheonix}}"
+00005770: 602c 2061 6e64 2074 6865 6e20 746f 2060  `, and then to `
+00005780: 2279 6469 643a 6372 743a 3635 4546 3446  "ydid:crt:65EF4F
+00005790: 3a65 3432 3339 6465 632d 3738 6332 2d34  :e4239dec-78c2-4
+000057a0: 3231 632d 6137 6633 2d37 3165 3631 6237  21c-a7f3-71e61b7
+000057b0: 3239 3436 6622 602e 0a0a 4e65 7374 696e  2946f"`...Nestin
+000057c0: 6720 6361 6e20 6265 2075 7020 746f 2074  g can be up to t
+000057d0: 6872 6565 206c 6576 656c 7320 6465 6570  hree levels deep
+000057e0: 2069 6e63 6c75 6469 6e67 2074 6865 2074   including the t
+000057f0: 6f70 206c 6576 656c 2e0a 0a23 2057 6f72  op level...# Wor
+00005800: 6b20 5265 7175 6972 656d 656e 7420 5072  k Requirement Pr
+00005810: 6f70 6572 7469 6573 0a0a 5468 6520 6077  operties..The `w
+00005820: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
+00005830: 7365 6374 696f 6e20 6f66 2074 6865 2063  section of the c
+00005840: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+00005850: 6520 6973 206f 7074 696f 6e61 6c2e 2049  e is optional. I
+00005860: 7427 7320 7573 6564 206f 6e6c 7920 6279  t's used only by
+00005870: 2074 6865 2060 7964 2d73 7562 6d69 7460   the `yd-submit`
+00005880: 2063 6f6d 6d61 6e64 2c20 616e 6420 636f   command, and co
+00005890: 6e74 726f 6c73 2074 6865 2057 6f72 6b20  ntrols the Work 
+000058a0: 5265 7175 6972 656d 656e 7420 7468 6174  Requirement that
+000058b0: 2069 7320 7375 626d 6974 7465 6420 746f   is submitted to
+000058c0: 2074 6865 2050 6c61 7466 6f72 6d2e 0a0a   the Platform...
+000058d0: 5468 6520 6465 7461 696c 7320 6f66 2061  The details of a
+000058e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000058f0: 7420 746f 2062 6520 7375 626d 6974 7465  t to be submitte
+00005900: 6420 6361 6e20 6265 2063 6170 7475 7265  d can be capture
+00005910: 6420 656e 7469 7265 6c79 2077 6974 6869  d entirely withi
+00005920: 6e20 7468 6520 544f 4d4c 2063 6f6e 6669  n the TOML confi
+00005930: 6775 7261 7469 6f6e 2066 696c 6520 666f  guration file fo
+00005940: 7220 7369 6d70 6c65 2065 7861 6d70 6c65  r simple example
+00005950: 732e 204d 6f72 6520 636f 6d70 6c65 7820  s. More complex 
+00005960: 6578 616d 706c 6573 2063 6170 7475 7265  examples capture
+00005970: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+00005980: 656d 656e 7420 696e 2061 2063 6f6d 6269  ement in a combi
+00005990: 6e61 7469 6f6e 206f 6620 7468 6520 544f  nation of the TO
+000059a0: 4d4c 2066 696c 6520 706c 7573 2061 204a  ML file plus a J
+000059b0: 534f 4e20 646f 6375 6d65 6e74 2c20 6f72  SON document, or
+000059c0: 2069 6e20 6120 4a53 4f4e 2064 6f63 756d   in a JSON docum
+000059d0: 656e 7420 6f6e 6c79 2e0a 0a23 2320 576f  ent only...## Wo
+000059e0: 726b 2052 6571 7569 7265 6d65 6e74 204a  rk Requirement J
+000059f0: 534f 4e20 4669 6c65 2053 7472 7563 7475  SON File Structu
+00005a00: 7265 0a0a 576f 726b 2052 6571 7569 7265  re..Work Require
+00005a10: 6d65 6e74 7320 6172 6520 7265 7072 6573  ments are repres
+00005a20: 656e 7465 6420 696e 204a 534f 4e20 646f  ented in JSON do
+00005a30: 6375 6d65 6e74 7320 7573 696e 6720 6120  cuments using a 
+00005a40: 636f 6e74 6169 6e6d 656e 7420 6869 6572  containment hier
+00005a50: 6172 6368 7920 6f66 2061 202a 2a57 6f72  archy of a **Wor
+00005a60: 6b20 5265 7175 6972 656d 656e 742a 2a20  k Requirement** 
+00005a70: 636f 6e74 6169 6e69 6e67 2061 202a 2a6c  containing a **l
+00005a80: 6973 7420 6f66 2054 6173 6b20 4772 6f75  ist of Task Grou
+00005a90: 7073 2a2a 2c20 636f 6e74 6169 6e69 6e67  ps**, containing
+00005aa0: 2061 202a 2a6c 6973 7420 6f66 2054 6173   a **list of Tas
+00005ab0: 6b73 2a2a 2e0a 0a41 2076 6572 7920 7369  ks**...A very si
+00005ac0: 6d70 6c65 2065 7861 6d70 6c65 2064 6f63  mple example doc
+00005ad0: 756d 656e 7420 6973 2073 686f 776e 2062  ument is shown b
+00005ae0: 656c 6f77 2077 6974 6820 6120 746f 702d  elow with a top-
+00005af0: 6c65 7665 6c20 576f 726b 2052 6571 7569  level Work Requi
+00005b00: 7265 6d65 6e74 2063 6f6e 7461 696e 696e  rement containin
+00005b10: 6720 7477 6f20 5461 736b 2047 726f 7570  g two Task Group
+00005b20: 7320 6561 6368 2063 6f6e 7461 696e 696e  s each containin
+00005b30: 6720 7477 6f20 5461 736b 732c 2065 6163  g two Tasks, eac
+00005b40: 6820 7769 7468 2061 2064 6966 6665 7265  h with a differe
+00005b50: 6e74 2073 6574 206f 6620 6172 6775 6d65  nt set of argume
+00005b60: 6e74 7320 746f 2062 6520 7061 7373 6564  nts to be passed
+00005b70: 2074 6f20 7468 6520 5461 736b 2e0a 0a60   to the Task...`
+00005b80: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
+00005b90: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+00005ba0: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+00005bb0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00005bc0: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
+00005bd0: 223a 205b 312c 2032 2c20 335d 0a20 2020  ": [1, 2, 3].   
+00005be0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00005bf0: 7b0a 2020 2020 2020 2020 2020 2261 7267  {.          "arg
+00005c00: 756d 656e 7473 223a 205b 342c 2035 2c20  uments": [4, 5, 
+00005c10: 365d 0a20 2020 2020 2020 207d 0a20 2020  6].        }.   
+00005c20: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
+00005c30: 7b0a 2020 2020 2020 2274 6173 6b73 223a  {.      "tasks":
+00005c40: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
+00005c50: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
+00005c60: 7322 3a20 5b37 2c20 382c 2039 5d0a 2020  s": [7, 8, 9].  
+00005c70: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00005c80: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+00005c90: 6775 6d65 6e74 7322 3a20 5b31 302c 2031  guments": [10, 1
+00005ca0: 312c 2031 325d 0a20 2020 2020 2020 207d  1, 12].        }
+00005cb0: 0a20 2020 2020 205d 0a20 2020 207d 0a20  .      ].    }. 
+00005cc0: 205d 0a7d 0a0a 6060 600a 0a54 6f20 7370   ].}..```..To sp
+00005cd0: 6563 6966 7920 7468 6520 6669 6c65 2063  ecify the file c
+00005ce0: 6f6e 7461 696e 696e 6720 7468 6520 4a53  ontaining the JS
+00005cf0: 4f4e 2064 6f63 756d 656e 742c 2065 6974  ON document, eit
+00005d00: 6865 7220 706f 7075 6c61 7465 2074 6865  her populate the
+00005d10: 2060 776f 726b 5265 7175 6972 656d 656e   `workRequiremen
+00005d20: 7444 6174 6160 2070 726f 7065 7274 7920  tData` property 
+00005d30: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
+00005d40: 6972 656d 656e 7460 2073 6563 7469 6f6e  irement` section
+00005d50: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
+00005d60: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+00005d70: 7769 7468 2074 6865 204a 534f 4e20 6669  with the JSON fi
+00005d80: 6c65 6e61 6d65 2c20 6f72 2073 7065 6369  lename, or speci
+00005d90: 6679 2069 7420 6f6e 2074 6865 2063 6f6d  fy it on the com
+00005da0: 6d61 6e64 206c 696e 6520 7573 696e 6720  mand line using 
+00005db0: 7468 6520 602d 2d77 6f72 6b2d 7265 7175  the `--work-requ
+00005dc0: 6972 656d 656e 7460 206f 7220 602d 7260  irement` or `-r`
+00005dd0: 206f 7074 696f 6e73 2028 7768 6963 6820   options (which 
+00005de0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
+00005df0: 6520 7072 6f70 6572 7479 2069 6e20 7468  e property in th
+00005e00: 6520 544f 4d4c 2066 696c 6529 2c20 652e  e TOML file), e.
+00005e10: 672e 0a0a 6079 642d 7375 626d 6974 202d  g...`yd-submit -
+00005e20: 2d63 6f6e 6669 6720 6d79 636f 6e66 6967  -config myconfig
+00005e30: 2e74 6f6d 6c20 2d2d 776f 726b 2d72 6571  .toml --work-req
+00005e40: 7569 7265 6d65 6e74 206d 795f 776f 726b  uirement my_work
+00005e50: 7265 712e 6a73 6f6e 600a 0a23 2320 5072  req.json`..## Pr
+00005e60: 6f70 6572 7479 2049 6e68 6572 6974 616e  operty Inheritan
+00005e70: 6365 0a0a 546f 2073 696d 706c 6966 7920  ce..To simplify 
+00005e80: 7468 6520 6465 6669 6e69 7469 6f6e 206f  the definition o
+00005e90: 6620 576f 726b 2052 6571 7569 7265 6d65  f Work Requireme
+00005ea0: 6e74 732c 2074 6865 7265 2069 7320 6120  nts, there is a 
+00005eb0: 7072 6f70 6572 7479 2069 6e68 6572 6974  property inherit
+00005ec0: 616e 6365 206d 6563 6861 6e69 736d 2e20  ance mechanism. 
+00005ed0: 5072 6f70 6572 7469 6573 2074 6861 7420  Properties that 
+00005ee0: 6172 6520 7365 7420 6174 2061 2068 6967  are set at a hig
+00005ef0: 6865 7220 6c65 7665 6c20 696e 2074 6865  her level in the
+00005f00: 2068 6965 7261 7263 6879 2061 7265 2069   hierarchy are i
+00005f10: 6e68 6572 6974 6564 2061 7420 6c6f 7765  nherited at lowe
+00005f20: 7220 6c65 7665 6c73 2c20 756e 6c65 7373  r levels, unless
+00005f30: 2065 7870 6c69 6369 746c 7920 6f76 6572   explicitly over
+00005f40: 7269 6464 656e 2e0a 0a54 6869 7320 6d65  ridden...This me
+00005f50: 616e 7320 7468 6174 2061 2070 726f 7065  ans that a prope
+00005f60: 7274 7920 7365 7420 696e 2074 6865 2060  rty set in the `
+00005f70: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+00005f80: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+00005f90: 544f 4d4c 2066 696c 6520 6361 6e20 6265  TOML file can be
+00005fa0: 2069 6e68 6572 6974 6564 2073 7563 6365   inherited succe
+00005fb0: 7373 6976 656c 7920 6279 2074 6865 2057  ssively by the W
+00005fc0: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
+00005fd0: 2054 6173 6b20 4772 6f75 7073 2061 6e64   Task Groups and
+00005fe0: 2054 6173 6b73 2069 6e20 7468 6520 4a53   Tasks in the JS
+00005ff0: 4f4e 2064 6f63 756d 656e 7420 2861 7373  ON document (ass
+00006000: 756d 696e 6720 7468 6520 7072 6f70 6572  uming the proper
+00006010: 7479 2069 7320 7661 6c69 6420 6174 2065  ty is valid at e
+00006020: 6163 6820 6c65 7665 6c29 2e20 2048 656e  ach level).  Hen
+00006030: 6365 2c20 5461 736b 7320 696e 6865 7269  ce, Tasks inheri
+00006040: 7420 6672 6f6d 2054 6173 6b20 4772 6f75  t from Task Grou
+00006050: 7073 2c20 7768 6963 6820 696e 6865 7269  ps, which inheri
+00006060: 7420 6672 6f6d 2074 6865 2057 6f72 6b20  t from the Work 
+00006070: 5265 7175 6972 656d 656e 7420 696e 2074  Requirement in t
+00006080: 6865 204a 534f 4e20 646f 6375 6d65 6e74  he JSON document
+00006090: 2c20 7768 6963 6820 696e 6865 7269 7473  , which inherits
+000060a0: 2066 726f 6d20 7468 6520 6077 6f72 6b52   from the `workR
+000060b0: 6571 7569 7265 6d65 6e74 6020 7072 6f70  equirement` prop
+000060c0: 6572 7469 6573 2069 6e20 7468 6520 544f  erties in the TO
+000060d0: 4d4c 2066 696c 652e 0a0a 4f76 6572 7269  ML file...Overri
+000060e0: 6464 656e 2070 726f 7065 7274 6965 7320  dden properties 
+000060f0: 6172 6520 616c 736f 2069 6e68 6572 6974  are also inherit
+00006100: 6564 2e20 452e 672e 2c20 6966 2061 2070  ed. E.g., if a p
+00006110: 726f 7065 7274 7920 6973 2073 6574 2061  roperty is set a
+00006120: 7420 7468 6520 5461 736b 2047 726f 7570  t the Task Group
+00006130: 206c 6576 656c 2c20 6974 2077 696c 6c20   level, it will 
+00006140: 6265 2069 6e68 6572 6974 6564 2062 7920  be inherited by 
+00006150: 7468 6520 5461 736b 7320 696e 2074 6861  the Tasks in tha
+00006160: 7420 5461 736b 2047 726f 7570 2075 6e6c  t Task Group unl
+00006170: 6573 7320 6578 706c 6963 6974 6c79 206f  ess explicitly o
+00006180: 7665 7272 6964 6465 6e2e 0a0a 2323 2057  verridden...## W
+00006190: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+000061a0: 5072 6f70 6572 7479 2044 6963 7469 6f6e  Property Diction
+000061b0: 6172 790a 0a54 6865 2066 6f6c 6c6f 7769  ary..The followi
+000061c0: 6e67 2074 6162 6c65 206f 7574 6c69 6e65  ng table outline
+000061d0: 7320 616c 6c20 7468 6520 7072 6f70 6572  s all the proper
+000061e0: 7469 6573 2061 7661 696c 6162 6c65 2066  ties available f
+000061f0: 6f72 2064 6566 696e 696e 6720 576f 726b  or defining Work
+00006200: 2052 6571 7569 7265 6d65 6e74 732c 2061   Requirements, a
+00006210: 6e64 2074 6865 206c 6576 656c 7320 6174  nd the levels at
+00006220: 2077 6869 6368 2074 6865 7920 6172 6520   which they are 
+00006230: 616c 6c6f 7765 6420 746f 2062 6520 7573  allowed to be us
+00006240: 6564 2e20 536f 2c20 666f 7220 6578 616d  ed. So, for exam
+00006250: 706c 652c 2074 6865 2060 7072 6f76 6964  ple, the `provid
+00006260: 6572 6020 7072 6f70 6572 7479 2063 616e  er` property can
+00006270: 2062 6520 7365 7420 696e 2074 6865 2054   be set in the T
+00006280: 4f4d 4c20 6669 6c65 2c20 6174 2074 6865  OML file, at the
+00006290: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000062a0: 7420 4c65 7665 6c20 6f72 2061 7420 7468  t Level or at th
+000062b0: 6520 5461 736b 2047 726f 7570 204c 6576  e Task Group Lev
+000062c0: 656c 2c20 6275 7420 6e6f 7420 6174 2074  el, but not at t
+000062d0: 6865 2054 6173 6b20 6c65 7665 6c2c 2061  he Task level, a
+000062e0: 6e64 2070 726f 7065 7274 7920 6064 6570  nd property `dep
+000062f0: 656e 6465 6e74 4f6e 6020 6361 6e20 6f6e  endentOn` can on
+00006300: 6c79 2062 6520 7365 7420 6174 2074 6865  ly be set at the
+00006310: 2054 6173 6b20 4772 6f75 7020 6c65 7665   Task Group leve
+00006320: 6c2e 0a0a 416c 6c20 7072 6f70 6572 7469  l...All properti
+00006330: 6573 2061 7265 206f 7074 696f 6e61 6c20  es are optional 
+00006340: 6578 6365 7074 2066 6f72 202a 2a60 7461  except for **`ta
+00006350: 736b 5479 7065 602a 2a20 286f 7220 2a2a  skType`** (or **
+00006360: 6074 6173 6b54 7970 6573 602a 2a29 2e0a  `taskTypes`**)..
+00006370: 0a7c 2050 726f 7065 7274 7920 4e61 6d65  .| Property Name
+00006380: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006390: 4465 7363 7269 7074 696f 6e20 2020 2020  Description     
 000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2020 2020 2020 2020 2020 7c20 544f 4d4c            | TOML
-00006440: 207c 2057 5220 207c 2054 4772 7020 7c20   | WR  | TGrp | 
-00006450: 5461 736b 207c 0a7c 3a2d 2d2d 2d2d 2d2d  Task |.|:-------
+00006430: 2020 2020 2020 2020 207c 2054 4f4d 4c20           | TOML 
+00006440: 7c20 5752 2020 7c20 5447 7270 207c 2054  | WR  | TGrp | T
+00006450: 6173 6b20 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d  ask |.|:--------
 00006460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006470: 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ----|:----------
+00006470: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
 00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00006500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00006520: 3a2d 2d2d 2d2d 7c3a 2d2d 2d2d 7c3a 2d2d  :-----|:----|:--
-00006530: 2d2d 2d7c 3a2d 2d2d 2d2d 7c0a 7c20 6061  ---|:-----|.| `a
-00006540: 7267 756d 656e 7473 6020 2020 2020 2020  rguments`       
-00006550: 2020 2020 2020 2020 207c 2054 6865 206c           | The l
-00006560: 6973 7420 6f66 2061 7267 756d 656e 7473  ist of arguments
-00006570: 2074 6f20 6265 2070 6173 7365 6420 746f   to be passed to
-00006580: 2074 6865 2054 6173 6b20 7768 656e 2069   the Task when i
-00006590: 7420 6973 2065 7865 6375 7465 642e 2045  t is executed. E
-000065a0: 2e67 2e3a 2060 5b31 2c20 2254 776f 225d  .g.: `[1, "Two"]
-000065b0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a  --------------|:
+00006520: 2d2d 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d  -----|:----|:---
+00006530: 2d2d 7c3a 2d2d 2d2d 2d7c 0a7c 2060 6172  --|:-----|.| `ar
+00006540: 6775 6d65 6e74 7360 2020 2020 2020 2020  guments`        
+00006550: 2020 2020 2020 2020 7c20 5468 6520 6c69          | The li
+00006560: 7374 206f 6620 6172 6775 6d65 6e74 7320  st of arguments 
+00006570: 746f 2062 6520 7061 7373 6564 2074 6f20  to be passed to 
+00006580: 7468 6520 5461 736b 2077 6865 6e20 6974  the Task when it
+00006590: 2069 7320 6578 6563 7574 6564 2e20 452e   is executed. E.
+000065a0: 672e 3a20 605b 312c 2022 5477 6f22 5d60  g.: `[1, "Two"]`
+000065b0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-00006610: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
-00006620: 0a7c 2060 6361 7074 7572 6554 6173 6b4f  .| `captureTaskO
-00006630: 7574 7075 7460 2020 2020 2020 2020 7c20  utput`        | 
-00006640: 5768 6574 6865 7220 7468 6520 636f 6e73  Whether the cons
-00006650: 6f6c 6520 6f75 7470 7574 206f 6620 6120  ole output of a 
-00006660: 5461 736b 2773 2070 726f 6365 7373 2073  Task's process s
-00006670: 686f 756c 6420 6265 2075 706c 6f61 6465  hould be uploade
-00006680: 6420 746f 2074 6865 2059 656c 6c6f 7744  d to the YellowD
-00006690: 6f67 204f 626a 6563 7420 5374 6f72 6520  og Object Store 
-000066a0: 6f6e 2054 6173 6b20 636f 6d70 6c65 7469  on Task completi
-000066b0: 6f6e 2e20 4465 6661 756c 743a 2060 7472  on. Default: `tr
-000066c0: 7565 602e 2020 2020 2020 2020 2020 2020  ue`.            
+00006600: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00006610: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
+00006620: 7c20 6063 6170 7475 7265 5461 736b 4f75  | `captureTaskOu
+00006630: 7470 7574 6020 2020 2020 2020 207c 2057  tput`        | W
+00006640: 6865 7468 6572 2074 6865 2063 6f6e 736f  hether the conso
+00006650: 6c65 206f 7574 7075 7420 6f66 2061 2054  le output of a T
+00006660: 6173 6b27 7320 7072 6f63 6573 7320 7368  ask's process sh
+00006670: 6f75 6c64 2062 6520 7570 6c6f 6164 6564  ould be uploaded
+00006680: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
+00006690: 6720 4f62 6a65 6374 2053 746f 7265 206f  g Object Store o
+000066a0: 6e20 5461 736b 2063 6f6d 706c 6574 696f  n Task completio
+000066b0: 6e2e 2044 6566 6175 6c74 3a20 6074 7275  n. Default: `tru
+000066c0: 6560 2e20 2020 2020 2020 2020 2020 2020  e`.             
 000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-000066f0: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
-00006700: 6573 2020 7c0a 7c20 6063 6f6d 706c 6574  es  |.| `complet
-00006710: 6564 5461 736b 5474 6c60 2020 2020 2020  edTaskTtl`      
-00006720: 2020 207c 2054 6865 2074 696d 6520 2869     | The time (i
-00006730: 6e20 6d69 6e75 7465 7329 2074 6f20 6c69  n minutes) to li
-00006740: 7665 2066 6f72 2063 6f6d 706c 6574 6564  ve for completed
-00006750: 2054 6173 6b73 2e20 4966 2073 6574 2c20   Tasks. If set, 
-00006760: 5461 736b 7320 7468 6174 2068 6176 6520  Tasks that have 
-00006770: 6265 656e 2063 6f6d 706c 6574 6564 2066  been completed f
-00006780: 6f72 206c 6f6e 6765 7220 7468 616e 2074  or longer than t
-00006790: 6869 7320 7065 7269 6f64 2077 696c 6c20  his period will 
-000067a0: 6265 2064 656c 6574 6564 2e20 452e 672e  be deleted. E.g.
-000067b0: 3a20 6031 302e 3060 2e20 2020 2020 2020  : `10.0`.       
-000067c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000067d0: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
-000067e0: 2020 7c20 2020 2020 207c 0a7c 2060 6373    |      |.| `cs
-000067f0: 7646 696c 6560 2020 2020 2020 2020 2020  vFile`          
-00006800: 2020 2020 2020 2020 7c20 5468 6520 6e61          | The na
-00006810: 6d65 206f 6620 7468 6520 4353 5620 6669  me of the CSV fi
-00006820: 6c65 2075 7365 6420 746f 2064 6572 6976  le used to deriv
-00006830: 6520 5461 736b 2064 6174 612e 2041 6e20  e Task data. An 
-00006840: 616c 7465 726e 6174 6976 6520 746f 2060  alternative to `
-00006850: 6373 7646 696c 6573 6020 7468 6174 2063  csvFiles` that c
-00006860: 616e 2062 6520 7573 6564 2077 6865 6e20  an be used when 
-00006870: 7468 6572 6527 7320 6f6e 6c79 2061 2073  there's only a s
-00006880: 696e 676c 6520 4353 5620 6669 6c65 2e20  ingle CSV file. 
-00006890: 452e 672e 2060 2266 696c 652e 6373 7622  E.g. `"file.csv"
-000068a0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
-000068b0: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
-000068c0: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
-000068d0: 7c20 6063 7376 4669 6c65 7360 2020 2020  | `csvFiles`    
-000068e0: 2020 2020 2020 2020 2020 2020 207c 2041               | A
-000068f0: 206c 6973 7420 6f66 2043 5356 2066 696c   list of CSV fil
-00006900: 6573 2075 7365 6420 746f 2064 6572 6976  es used to deriv
-00006910: 6520 5461 736b 2064 6174 612e 2045 2e67  e Task data. E.g
-00006920: 2e20 605b 2266 696c 652e 6373 7622 2c20  . `["file.csv", 
-00006930: 2266 696c 655f 322e 6373 763a 325d 602e  "file_2.csv:2]`.
+000066e0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+000066f0: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+00006700: 7320 207c 0a7c 2060 636f 6d70 6c65 7465  s  |.| `complete
+00006710: 6454 6173 6b54 746c 6020 2020 2020 2020  dTaskTtl`       
+00006720: 2020 7c20 5468 6520 7469 6d65 2028 696e    | The time (in
+00006730: 206d 696e 7574 6573 2920 746f 206c 6976   minutes) to liv
+00006740: 6520 666f 7220 636f 6d70 6c65 7465 6420  e for completed 
+00006750: 5461 736b 732e 2049 6620 7365 742c 2054  Tasks. If set, T
+00006760: 6173 6b73 2074 6861 7420 6861 7665 2062  asks that have b
+00006770: 6565 6e20 636f 6d70 6c65 7465 6420 666f  een completed fo
+00006780: 7220 6c6f 6e67 6572 2074 6861 6e20 7468  r longer than th
+00006790: 6973 2070 6572 696f 6420 7769 6c6c 2062  is period will b
+000067a0: 6520 6465 6c65 7465 642e 2045 2e67 2e3a  e deleted. E.g.:
+000067b0: 2060 3130 2e30 602e 2020 2020 2020 2020   `10.0`.        
+000067c0: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+000067d0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+000067e0: 207c 2020 2020 2020 7c0a 7c20 6063 7376   |      |.| `csv
+000067f0: 4669 6c65 6020 2020 2020 2020 2020 2020  File`           
+00006800: 2020 2020 2020 207c 2054 6865 206e 616d         | The nam
+00006810: 6520 6f66 2074 6865 2043 5356 2066 696c  e of the CSV fil
+00006820: 6520 7573 6564 2074 6f20 6465 7269 7665  e used to derive
+00006830: 2054 6173 6b20 6461 7461 2e20 416e 2061   Task data. An a
+00006840: 6c74 6572 6e61 7469 7665 2074 6f20 6063  lternative to `c
+00006850: 7376 4669 6c65 7360 2074 6861 7420 6361  svFiles` that ca
+00006860: 6e20 6265 2075 7365 6420 7768 656e 2074  n be used when t
+00006870: 6865 7265 2773 206f 6e6c 7920 6120 7369  here's only a si
+00006880: 6e67 6c65 2043 5356 2066 696c 652e 2045  ngle CSV file. E
+00006890: 2e67 2e20 6022 6669 6c65 2e63 7376 2260  .g. `"file.csv"`
+000068a0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+000068b0: 2020 7c20 5965 7320 207c 2020 2020 207c    | Yes  |     |
+000068c0: 2020 2020 2020 7c20 2020 2020 207c 0a7c        |      |.|
+000068d0: 2060 6373 7646 696c 6573 6020 2020 2020   `csvFiles`     
+000068e0: 2020 2020 2020 2020 2020 2020 7c20 4120              | A 
+000068f0: 6c69 7374 206f 6620 4353 5620 6669 6c65  list of CSV file
+00006900: 7320 7573 6564 2074 6f20 6465 7269 7665  s used to derive
+00006910: 2054 6173 6b20 6461 7461 2e20 452e 672e   Task data. E.g.
+00006920: 2060 5b22 6669 6c65 2e63 7376 222c 2022   `["file.csv", "
+00006930: 6669 6c65 5f32 2e63 7376 3a32 5d60 2e20  file_2.csv:2]`. 
 00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-000069a0: 2020 2020 207c 2020 2020 2020 7c20 2020       |      |   
-000069b0: 2020 207c 0a7c 2060 6465 7065 6e64 656e     |.| `dependen
-000069c0: 744f 6e60 2020 2020 2020 2020 2020 2020  tOn`            
-000069d0: 2020 7c20 5468 6520 6e61 6d65 206f 6620    | The name of 
-000069e0: 616e 6f74 6865 7220 5461 736b 2047 726f  another Task Gro
-000069f0: 7570 2077 6974 6869 6e20 7468 6520 7361  up within the sa
-00006a00: 6d65 2057 6f72 6b20 5265 7175 6972 656d  me Work Requirem
-00006a10: 656e 7420 7468 6174 206d 7573 7420 6265  ent that must be
-00006a20: 2073 7563 6365 7373 6675 6c6c 7920 636f   successfully co
-00006a30: 6d70 6c65 7465 6420 6265 666f 7265 2074  mpleted before t
-00006a40: 6865 2054 6173 6b20 4772 6f75 7020 6973  he Task Group is
-00006a50: 2073 7461 7274 6564 2e20 452e 672e 2060   started. E.g. `
-00006a60: 2274 6173 6b5f 6772 6f75 705f 3122 602e  "task_group_1"`.
-00006a70: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00006a80: 2020 2020 7c20 2020 2020 7c20 5965 7320      |     | Yes 
-00006a90: 207c 2020 2020 2020 7c0a 7c20 6064 6f63   |      |.| `doc
-00006aa0: 6b65 7245 6e76 6972 6f6e 6d65 6e74 6020  kerEnvironment` 
-00006ab0: 2020 2020 2020 207c 2054 6865 2065 6e76         | The env
-00006ac0: 6972 6f6e 6d65 6e74 2074 6f20 6265 2070  ironment to be p
-00006ad0: 6173 7365 6420 746f 2061 2044 6f63 6b65  assed to a Docke
-00006ae0: 7220 636f 6e74 6169 6e65 722e 204f 6e6c  r container. Onl
-00006af0: 7920 7573 6564 2062 7920 7468 6520 6064  y used by the `d
-00006b00: 6f63 6b65 7260 2054 6173 6b20 5479 7065  ocker` Task Type
-00006b10: 2e20 452e 672e 2c20 4a53 4f4e 3a20 607b  . E.g., JSON: `{
-00006b20: 2256 4152 5f31 223a 2022 6162 6322 7d60  "VAR_1": "abc"}`
-00006b30: 2c20 544f 4d4c 3a20 607b 5641 525f 3120  , TOML: `{VAR_1 
-00006b40: 3d20 2261 6263 222c 2056 4152 5f32 203d  = "abc", VAR_2 =
-00006b50: 2022 6465 6622 7d60 2e20 2020 2020 2020   "def"}`.       
-00006b60: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-00006b70: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
-00006b80: 2060 646f 636b 6572 5061 7373 776f 7264   `dockerPassword
-00006b90: 6020 2020 2020 2020 2020 2020 7c20 5468  `           | Th
-00006ba0: 6520 7061 7373 776f 7264 2066 6f72 2044  e password for D
-00006bb0: 6f63 6b65 7248 7562 2c20 6f6e 6c79 2075  ockerHub, only u
-00006bc0: 7365 6420 6279 2074 6865 2060 646f 636b  sed by the `dock
-00006bd0: 6572 6020 5461 736b 2054 7970 652e 2045  er` Task Type. E
-00006be0: 2c67 2e2c 2060 226d 795f 7061 7373 776f  ,g., `"my_passwo
-00006bf0: 7264 2260 2e20 2020 2020 2020 2020 2020  rd"`.           
+00006990: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+000069a0: 2020 2020 7c20 2020 2020 207c 2020 2020      |      |    
+000069b0: 2020 7c0a 7c20 6064 6570 656e 6465 6e74    |.| `dependent
+000069c0: 4f6e 6020 2020 2020 2020 2020 2020 2020  On`             
+000069d0: 207c 2054 6865 206e 616d 6520 6f66 2061   | The name of a
+000069e0: 6e6f 7468 6572 2054 6173 6b20 4772 6f75  nother Task Grou
+000069f0: 7020 7769 7468 696e 2074 6865 2073 616d  p within the sam
+00006a00: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+00006a10: 6e74 2074 6861 7420 6d75 7374 2062 6520  nt that must be 
+00006a20: 7375 6363 6573 7366 756c 6c79 2063 6f6d  successfully com
+00006a30: 706c 6574 6564 2062 6566 6f72 6520 7468  pleted before th
+00006a40: 6520 5461 736b 2047 726f 7570 2069 7320  e Task Group is 
+00006a50: 7374 6172 7465 642e 2045 2e67 2e20 6022  started. E.g. `"
+00006a60: 7461 736b 5f67 726f 7570 5f31 2260 2e20  task_group_1"`. 
+00006a70: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00006a80: 2020 207c 2020 2020 207c 2059 6573 2020     |     | Yes  
+00006a90: 7c20 2020 2020 207c 0a7c 2060 646f 636b  |      |.| `dock
+00006aa0: 6572 456e 7669 726f 6e6d 656e 7460 2020  erEnvironment`  
+00006ab0: 2020 2020 2020 7c20 5468 6520 656e 7669        | The envi
+00006ac0: 726f 6e6d 656e 7420 746f 2062 6520 7061  ronment to be pa
+00006ad0: 7373 6564 2074 6f20 6120 446f 636b 6572  ssed to a Docker
+00006ae0: 2063 6f6e 7461 696e 6572 2e20 4f6e 6c79   container. Only
+00006af0: 2075 7365 6420 6279 2074 6865 2060 646f   used by the `do
+00006b00: 636b 6572 6020 5461 736b 2054 7970 652e  cker` Task Type.
+00006b10: 2045 2e67 2e2c 204a 534f 4e3a 2060 7b22   E.g., JSON: `{"
+00006b20: 5641 525f 3122 3a20 2261 6263 227d 602c  VAR_1": "abc"}`,
+00006b30: 2054 4f4d 4c3a 2060 7b56 4152 5f31 203d   TOML: `{VAR_1 =
+00006b40: 2022 6162 6322 2c20 5641 525f 3220 3d20   "abc", VAR_2 = 
+00006b50: 2264 6566 227d 602e 2020 2020 2020 2020  "def"}`.        
+00006b60: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+00006b70: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
+00006b80: 6064 6f63 6b65 7250 6173 7377 6f72 6460  `dockerPassword`
+00006b90: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+00006ba0: 2070 6173 7377 6f72 6420 666f 7220 446f   password for Do
+00006bb0: 636b 6572 4875 622c 206f 6e6c 7920 7573  ckerHub, only us
+00006bc0: 6564 2062 7920 7468 6520 6064 6f63 6b65  ed by the `docke
+00006bd0: 7260 2054 6173 6b20 5479 7065 2e20 452c  r` Task Type. E,
+00006be0: 672e 2c20 6022 6d79 5f70 6173 7377 6f72  g., `"my_passwor
+00006bf0: 6422 602e 2020 2020 2020 2020 2020 2020  d"`.            
 00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00006c50: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
-00006c60: 2020 7c0a 7c20 6064 6f63 6b65 7255 7365    |.| `dockerUse
-00006c70: 726e 616d 6560 2020 2020 2020 2020 2020  rname`          
-00006c80: 207c 2054 6865 2075 7365 726e 616d 6520   | The username 
-00006c90: 666f 7220 446f 636b 6572 4875 622c 206f  for DockerHub, o
-00006ca0: 6e6c 7920 7573 6564 2062 7920 7468 6520  nly used by the 
-00006cb0: 6064 6f63 6b65 7260 2054 6173 6b20 5479  `docker` Task Ty
-00006cc0: 7065 2e20 452c 672e 2c20 6022 6d79 5f75  pe. E,g., `"my_u
-00006cd0: 7365 726e 616d 6522 602e 2020 2020 2020  sername"`.      
+00006c40: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+00006c50: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
+00006c60: 207c 0a7c 2060 646f 636b 6572 5573 6572   |.| `dockerUser
+00006c70: 6e61 6d65 6020 2020 2020 2020 2020 2020  name`           
+00006c80: 7c20 5468 6520 7573 6572 6e61 6d65 2066  | The username f
+00006c90: 6f72 2044 6f63 6b65 7248 7562 2c20 6f6e  or DockerHub, on
+00006ca0: 6c79 2075 7365 6420 6279 2074 6865 2060  ly used by the `
+00006cb0: 646f 636b 6572 6020 5461 736b 2054 7970  docker` Task Typ
+00006cc0: 652e 2045 2c67 2e2c 2060 226d 795f 7573  e. E,g., `"my_us
+00006cd0: 6572 6e61 6d65 2260 2e20 2020 2020 2020  ername"`.       
 00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-00006d30: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-00006d40: 7c20 5965 7320 207c 0a7c 2060 656e 7669  | Yes  |.| `envi
-00006d50: 726f 6e6d 656e 7460 2020 2020 2020 2020  ronment`        
-00006d60: 2020 2020 2020 7c20 5468 6520 656e 7669        | The envi
-00006d70: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00006d80: 7320 746f 2073 6574 2066 6f72 2061 2054  s to set for a T
-00006d90: 6173 6b20 7768 656e 2069 7427 7320 6578  ask when it's ex
-00006da0: 6563 7574 6564 2e20 452e 672e 2c20 4a53  ecuted. E.g., JS
-00006db0: 4f4e 3a20 607b 2256 4152 5f31 223a 2022  ON: `{"VAR_1": "
-00006dc0: 6162 6322 2c20 2256 4152 5f32 223a 2022  abc", "VAR_2": "
-00006dd0: 6465 6622 7d60 2c20 544f 4d4c 3a20 607b  def"}`, TOML: `{
-00006de0: 5641 525f 3120 3d20 2261 6263 222c 2056  VAR_1 = "abc", V
-00006df0: 4152 5f32 203d 2022 6465 6622 7d60 2e20  AR_2 = "def"}`. 
+00006d20: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+00006d30: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00006d40: 2059 6573 2020 7c0a 7c20 6065 6e76 6972   Yes  |.| `envir
+00006d50: 6f6e 6d65 6e74 6020 2020 2020 2020 2020  onment`         
+00006d60: 2020 2020 207c 2054 6865 2065 6e76 6972       | The envir
+00006d70: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00006d80: 2074 6f20 7365 7420 666f 7220 6120 5461   to set for a Ta
+00006d90: 736b 2077 6865 6e20 6974 2773 2065 7865  sk when it's exe
+00006da0: 6375 7465 642e 2045 2e67 2e2c 204a 534f  cuted. E.g., JSO
+00006db0: 4e3a 2060 7b22 5641 525f 3122 3a20 2261  N: `{"VAR_1": "a
+00006dc0: 6263 222c 2022 5641 525f 3222 3a20 2264  bc", "VAR_2": "d
+00006dd0: 6566 227d 602c 2054 4f4d 4c3a 2060 7b56  ef"}`, TOML: `{V
+00006de0: 4152 5f31 203d 2022 6162 6322 2c20 5641  AR_1 = "abc", VA
+00006df0: 525f 3220 3d20 2264 6566 227d 602e 2020  R_2 = "def"}`.  
 00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00006e20: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
-00006e30: 6065 7863 6c75 7369 7665 576f 726b 6572  `exclusiveWorker
-00006e40: 7360 2020 2020 2020 2020 207c 2049 6620  s`         | If 
-00006e50: 7472 7565 2c20 7468 656e 2064 6f20 6e6f  true, then do no
-00006e60: 7420 616c 6c6f 7720 636c 6169 6d65 6420  t allow claimed 
-00006e70: 576f 726b 6572 7320 746f 2062 6520 7368  Workers to be sh
-00006e80: 6172 6564 2077 6974 6820 6f74 6865 7220  ared with other 
-00006e90: 5461 736b 2047 726f 7570 733b 206f 7468  Task Groups; oth
-00006ea0: 6572 7769 7365 2c20 576f 726b 6572 7320  erwise, Workers 
-00006eb0: 6361 6e20 6265 2073 6861 7265 642e 2044  can be shared. D
-00006ec0: 6566 6175 6c74 3a60 6661 6c73 6560 2e20  efault:`false`. 
+00006e10: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+00006e20: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+00006e30: 6578 636c 7573 6976 6557 6f72 6b65 7273  exclusiveWorkers
+00006e40: 6020 2020 2020 2020 2020 7c20 4966 2074  `         | If t
+00006e50: 7275 652c 2074 6865 6e20 646f 206e 6f74  rue, then do not
+00006e60: 2061 6c6c 6f77 2063 6c61 696d 6564 2057   allow claimed W
+00006e70: 6f72 6b65 7273 2074 6f20 6265 2073 6861  orkers to be sha
+00006e80: 7265 6420 7769 7468 206f 7468 6572 2054  red with other T
+00006e90: 6173 6b20 4772 6f75 7073 3b20 6f74 6865  ask Groups; othe
+00006ea0: 7277 6973 652c 2057 6f72 6b65 7273 2063  rwise, Workers c
+00006eb0: 616e 2062 6520 7368 6172 6564 2e20 4465  an be shared. De
+00006ec0: 6661 756c 743a 6066 616c 7365 602e 2020  fault:`false`.  
 00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00006f00: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
-00006f10: 207c 0a7c 2060 6578 6563 7574 6162 6c65   |.| `executable
-00006f20: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00006f30: 7c20 5468 6520 2765 7865 6375 7461 626c  | The 'executabl
-00006f40: 6527 2074 6f20 7275 6e20 7768 656e 2061  e' to run when a
-00006f50: 2042 6173 6820 6f72 2044 6f63 6b65 7220   Bash or Docker 
-00006f60: 5461 736b 2069 7320 6578 6563 7574 6564  Task is executed
-00006f70: 2e20 4261 7368 2073 6372 6970 7420 666f  . Bash script fo
-00006f80: 7220 4261 7368 2c20 636f 6e74 6169 6e65  r Bash, containe
-00006f90: 7220 696d 6167 6520 666f 7220 446f 636b  r image for Dock
-00006fa0: 6572 2e20 4f70 7469 6f6e 616c 3a20 6f6d  er. Optional: om
-00006fb0: 6974 2074 6f20 7375 7070 7265 7373 2061  it to suppress a
-00006fc0: 7574 6f6d 6174 6963 2070 726f 6365 7373  utomatic process
-00006fd0: 696e 672e 2020 2020 2020 207c 2059 6573  ing.       | Yes
-00006fe0: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00006ff0: 2059 6573 2020 7c0a 7c20 6066 696e 6973   Yes  |.| `finis
-00007000: 6849 6641 6c6c 5461 736b 7346 696e 6973  hIfAllTasksFinis
-00007010: 6865 6460 207c 2049 6620 7472 7565 2c20  hed` | If true, 
-00007020: 7468 6520 5461 736b 2047 726f 7570 2077  the Task Group w
-00007030: 696c 6c20 6669 6e69 7368 2061 7574 6f6d  ill finish autom
-00007040: 6174 6963 616c 6c79 2069 6620 616c 6c20  atically if all 
-00007050: 636f 6e74 6169 6e65 6420 7461 736b 7320  contained tasks 
-00007060: 6669 6e69 7368 2e20 4465 6661 756c 743a  finish. Default:
-00007070: 6074 7275 6560 2e20 2020 2020 2020 2020  `true`.         
+00006ef0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00006f00: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
+00006f10: 7c0a 7c20 6065 7865 6375 7461 626c 6560  |.| `executable`
+00006f20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006f30: 2054 6865 2027 6578 6563 7574 6162 6c65   The 'executable
+00006f40: 2720 746f 2072 756e 2077 6865 6e20 6120  ' to run when a 
+00006f50: 4261 7368 206f 7220 446f 636b 6572 2054  Bash or Docker T
+00006f60: 6173 6b20 6973 2065 7865 6375 7465 642e  ask is executed.
+00006f70: 2042 6173 6820 7363 7269 7074 2066 6f72   Bash script for
+00006f80: 2042 6173 682c 2063 6f6e 7461 696e 6572   Bash, container
+00006f90: 2069 6d61 6765 2066 6f72 2044 6f63 6b65   image for Docke
+00006fa0: 722e 204f 7074 696f 6e61 6c3a 206f 6d69  r. Optional: omi
+00006fb0: 7420 746f 2073 7570 7072 6573 7320 6175  t to suppress au
+00006fc0: 746f 6d61 7469 6320 7072 6f63 6573 7369  tomatic processi
+00006fd0: 6e67 2e20 2020 2020 2020 7c20 5965 7320  ng.       | Yes 
+00006fe0: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
+00006ff0: 5965 7320 207c 0a7c 2060 6669 6e69 7368  Yes  |.| `finish
+00007000: 4966 416c 6c54 6173 6b73 4669 6e69 7368  IfAllTasksFinish
+00007010: 6564 6020 7c20 4966 2074 7275 652c 2074  ed` | If true, t
+00007020: 6865 2054 6173 6b20 4772 6f75 7020 7769  he Task Group wi
+00007030: 6c6c 2066 696e 6973 6820 6175 746f 6d61  ll finish automa
+00007040: 7469 6361 6c6c 7920 6966 2061 6c6c 2063  tically if all c
+00007050: 6f6e 7461 696e 6564 2074 6173 6b73 2066  ontained tasks f
+00007060: 696e 6973 682e 2044 6566 6175 6c74 3a60  inish. Default:`
+00007070: 7472 7565 602e 2020 2020 2020 2020 2020  true`.          
 00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-000070d0: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
-000070e0: 6669 6e69 7368 4966 416e 7954 6173 6b46  finishIfAnyTaskF
-000070f0: 6169 6c65 6460 2020 2020 7c20 4966 2074  ailed`    | If t
-00007100: 7275 652c 2074 6865 2054 6173 6b20 4772  rue, the Task Gr
-00007110: 6f75 7020 7769 6c6c 2062 6520 6661 696c  oup will be fail
-00007120: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
-00007130: 2069 6620 616e 7920 636f 6e74 6169 6e65   if any containe
-00007140: 6420 7461 736b 7320 6661 696c 2e20 4465  d tasks fail. De
-00007150: 6661 756c 743a 6066 616c 7365 602e 2020  fault:`false`.  
+000070b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000070c0: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
+000070d0: 7320 207c 2020 2020 2020 7c0a 7c20 6066  s  |      |.| `f
+000070e0: 696e 6973 6849 6641 6e79 5461 736b 4661  inishIfAnyTaskFa
+000070f0: 696c 6564 6020 2020 207c 2049 6620 7472  iled`    | If tr
+00007100: 7565 2c20 7468 6520 5461 736b 2047 726f  ue, the Task Gro
+00007110: 7570 2077 696c 6c20 6265 2066 6169 6c65  up will be faile
+00007120: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
+00007130: 6966 2061 6e79 2063 6f6e 7461 696e 6564  if any contained
+00007140: 2074 6173 6b73 2066 6169 6c2e 2044 6566   tasks fail. Def
+00007150: 6175 6c74 3a60 6661 6c73 6560 2e20 2020  ault:`false`.   
 00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-000071b0: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
-000071c0: 7c0a 7c20 6066 6c61 7474 656e 496e 7075  |.| `flattenInpu
-000071d0: 7450 6174 6873 6020 2020 2020 2020 207c  tPaths`        |
-000071e0: 2044 6574 6572 6d69 6e65 7320 7768 6574   Determines whet
-000071f0: 6865 7220 696e 7075 7420 6f62 6a65 6374  her input object
-00007200: 2070 6174 6873 2073 686f 756c 6420 6265   paths should be
-00007210: 2066 6c61 7474 656e 6564 2028 692e 652e   flattened (i.e.
-00007220: 2c20 6469 7265 6374 6f72 7920 7374 7275  , directory stru
-00007230: 6374 7572 6520 7265 6d6f 7665 6429 2077  cture removed) w
-00007240: 6865 6e20 646f 776e 6c6f 6164 6564 2074  hen downloaded t
-00007250: 6f20 6120 6e6f 6465 2e20 4465 6661 756c  o a node. Defaul
-00007260: 743a 2060 6661 6c73 6560 2e20 2020 2020  t: `false`.     
+000071a0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+000071b0: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
+000071c0: 0a7c 2060 666c 6174 7465 6e49 6e70 7574  .| `flattenInput
+000071d0: 5061 7468 7360 2020 2020 2020 2020 7c20  Paths`        | 
+000071e0: 4465 7465 726d 696e 6573 2077 6865 7468  Determines wheth
+000071f0: 6572 2069 6e70 7574 206f 626a 6563 7420  er input object 
+00007200: 7061 7468 7320 7368 6f75 6c64 2062 6520  paths should be 
+00007210: 666c 6174 7465 6e65 6420 2869 2e65 2e2c  flattened (i.e.,
+00007220: 2064 6972 6563 746f 7279 2073 7472 7563   directory struc
+00007230: 7475 7265 2072 656d 6f76 6564 2920 7768  ture removed) wh
+00007240: 656e 2064 6f77 6e6c 6f61 6465 6420 746f  en downloaded to
+00007250: 2061 206e 6f64 652e 2044 6566 6175 6c74   a node. Default
+00007260: 3a20 6066 616c 7365 602e 2020 2020 2020  : `false`.      
 00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-00007290: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
-000072a0: 5965 7320 207c 0a7c 2060 666c 6174 7465  Yes  |.| `flatte
-000072b0: 6e55 706c 6f61 6450 6174 6873 6020 2020  nUploadPaths`   
-000072c0: 2020 2020 7c20 4967 6e6f 7265 206c 6f63      | Ignore loc
-000072d0: 616c 2064 6972 6563 746f 7279 2070 6174  al directory pat
-000072e0: 6873 2077 6865 6e20 7570 6c6f 6164 696e  hs when uploadin
-000072f0: 6720 6669 6c65 7320 746f 2074 6865 204f  g files to the O
-00007300: 626a 6563 7420 5374 6f72 653b 2070 6c61  bject Store; pla
-00007310: 6365 2069 6e20 603c 6e61 6d65 7370 6163  ce in `<namespac
-00007320: 653e 3a3c 776f 726b 2d72 6571 2d6e 616d  e>:<work-req-nam
-00007330: 653e 2f60 2e20 4465 6661 756c 743a 2060  e>/`. Default: `
-00007340: 6661 6c73 6560 2e20 2020 2020 2020 2020  false`.         
+00007280: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+00007290: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
+000072a0: 6573 2020 7c0a 7c20 6066 6c61 7474 656e  es  |.| `flatten
+000072b0: 5570 6c6f 6164 5061 7468 7360 2020 2020  UploadPaths`    
+000072c0: 2020 207c 2049 676e 6f72 6520 6c6f 6361     | Ignore loca
+000072d0: 6c20 6469 7265 6374 6f72 7920 7061 7468  l directory path
+000072e0: 7320 7768 656e 2075 706c 6f61 6469 6e67  s when uploading
+000072f0: 2066 696c 6573 2074 6f20 7468 6520 4f62   files to the Ob
+00007300: 6a65 6374 2053 746f 7265 3b20 706c 6163  ject Store; plac
+00007310: 6520 696e 2060 3c6e 616d 6573 7061 6365  e in `<namespace
+00007320: 3e3a 3c77 6f72 6b2d 7265 712d 6e61 6d65  >:<work-req-name
+00007330: 3e2f 602e 2044 6566 6175 6c74 3a20 6066  >/`. Default: `f
+00007340: 616c 7365 602e 2020 2020 2020 2020 2020  alse`.          
 00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007370: 2059 6573 2020 7c20 5965 7320 7c20 2020   Yes  | Yes |   
-00007380: 2020 207c 2020 2020 2020 7c0a 7c20 6066     |      |.| `f
-00007390: 756c 6669 6c4f 6e53 7562 6d69 7460 2020  ulfilOnSubmit`  
-000073a0: 2020 2020 2020 2020 207c 2049 6e64 6963           | Indic
-000073b0: 6174 6573 2069 6620 7468 6520 576f 726b  ates if the Work
-000073c0: 2052 6571 7569 7265 6d65 6e74 2073 686f   Requirement sho
-000073d0: 756c 6420 6265 2066 756c 6669 6c6c 6564  uld be fulfilled
-000073e0: 2077 6865 6e20 6974 2069 7320 7375 626d   when it is subm
-000073f0: 6974 7465 642c 2072 6174 6865 7220 7468  itted, rather th
-00007400: 616e 2062 6569 6e67 2061 6c6c 6f77 6564  an being allowed
-00007410: 2074 6f20 7761 6974 2069 6e20 5045 4e44   to wait in PEND
-00007420: 494e 4720 7374 6174 7573 2e20 4465 6661  ING status. Defa
-00007430: 756c 743a 6066 616c 7365 602e 2020 2020  ult:`false`.    
+00007360: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007370: 5965 7320 207c 2059 6573 207c 2020 2020  Yes  | Yes |    
+00007380: 2020 7c20 2020 2020 207c 0a7c 2060 6675    |      |.| `fu
+00007390: 6c66 696c 4f6e 5375 626d 6974 6020 2020  lfilOnSubmit`   
+000073a0: 2020 2020 2020 2020 7c20 496e 6469 6361          | Indica
+000073b0: 7465 7320 6966 2074 6865 2057 6f72 6b20  tes if the Work 
+000073c0: 5265 7175 6972 656d 656e 7420 7368 6f75  Requirement shou
+000073d0: 6c64 2062 6520 6675 6c66 696c 6c65 6420  ld be fulfilled 
+000073e0: 7768 656e 2069 7420 6973 2073 7562 6d69  when it is submi
+000073f0: 7474 6564 2c20 7261 7468 6572 2074 6861  tted, rather tha
+00007400: 6e20 6265 696e 6720 616c 6c6f 7765 6420  n being allowed 
+00007410: 746f 2077 6169 7420 696e 2050 454e 4449  to wait in PENDI
+00007420: 4e47 2073 7461 7475 732e 2044 6566 6175  NG status. Defau
+00007430: 6c74 3a60 6661 6c73 6560 2e20 2020 2020  lt:`false`.     
 00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007450: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-00007460: 207c 2020 2020 2020 7c20 2020 2020 207c   |      |      |
-00007470: 0a7c 2060 696e 7075 7473 6020 2020 2020  .| `inputs`     
-00007480: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007490: 5468 6520 6c69 7374 206f 6620 696e 7075  The list of inpu
-000074a0: 7420 6669 6c65 7320 746f 2062 6520 7570  t files to be up
-000074b0: 6c6f 6164 6564 2074 6f20 7468 6520 5965  loaded to the Ye
-000074c0: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
-000074d0: 746f 7265 2c20 616e 6420 7265 7175 6972  tore, and requir
-000074e0: 6564 2062 7920 7468 6520 5461 736b 2028  ed by the Task (
-000074f0: 696d 706c 6965 7320 6076 6572 6966 7941  implies `verifyA
-00007500: 7453 7461 7274 6029 2e20 452e 672e 2060  tStart`). E.g. `
-00007510: 5b22 612e 7368 222c 2022 622e 7368 225d  ["a.sh", "b.sh"]
-00007520: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
-00007530: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-00007540: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
-00007550: 6573 2020 7c0a 7c20 6069 6e70 7574 734f  es  |.| `inputsO
-00007560: 7074 696f 6e61 6c60 2020 2020 2020 2020  ptional`        
-00007570: 2020 207c 2041 206c 6973 7420 6f66 2069     | A list of i
-00007580: 6e70 7574 2066 696c 6573 2072 6571 7569  nput files requi
-00007590: 7265 6420 6279 2061 2054 6173 6b2c 2062  red by a Task, b
-000075a0: 7574 2077 6869 6368 2061 7265 206e 6f74  ut which are not
-000075b0: 2073 7562 6a65 6374 2074 6f20 7665 7269   subject to veri
-000075c0: 6669 6361 7469 6f6e 2e20 4361 6e20 636f  fication. Can co
-000075d0: 6e74 6169 6e20 7769 6c64 6361 7264 732e  ntain wildcards.
-000075e0: 2045 2e67 2e3a 2060 5b22 7461 736b 5f67   E.g.: `["task_g
-000075f0: 726f 7570 5f31 2f2a 2a2f 7265 7375 6c74  roup_1/**/result
-00007600: 732e 7478 7422 5d60 2e20 2020 2020 2020  s.txt"]`.       
-00007610: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007620: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
-00007630: 2020 7c20 5965 7320 207c 0a7c 2060 696e    | Yes  |.| `in
-00007640: 7374 616e 6365 5479 7065 7360 2020 2020  stanceTypes`    
-00007650: 2020 2020 2020 2020 7c20 5468 6520 6d61          | The ma
-00007660: 6368 696e 6520 696e 7374 616e 6365 2074  chine instance t
-00007670: 7970 6573 2074 6861 7420 6361 6e20 6265  ypes that can be
-00007680: 2075 7365 6420 746f 2065 7865 6375 7465   used to execute
-00007690: 2054 6173 6b73 2e20 452e 672e 2c20 605b   Tasks. E.g., `[
-000076a0: 2274 332e 6d69 6372 6f22 2c20 2274 3361  "t3.micro", "t3a
-000076b0: 2e6d 6963 726f 225d 602e 2020 2020 2020  .micro"]`.      
+00007450: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00007460: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
+00007470: 7c20 6069 6e70 7574 7360 2020 2020 2020  | `inputs`      
+00007480: 2020 2020 2020 2020 2020 2020 207c 2054               | T
+00007490: 6865 206c 6973 7420 6f66 2069 6e70 7574  he list of input
+000074a0: 2066 696c 6573 2074 6f20 6265 2075 706c   files to be upl
+000074b0: 6f61 6465 6420 746f 2074 6865 2059 656c  oaded to the Yel
+000074c0: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
+000074d0: 6f72 652c 2061 6e64 2072 6571 7569 7265  ore, and require
+000074e0: 6420 6279 2074 6865 2054 6173 6b20 2869  d by the Task (i
+000074f0: 6d70 6c69 6573 2060 7665 7269 6679 4174  mplies `verifyAt
+00007500: 5374 6172 7460 292e 2045 2e67 2e20 605b  Start`). E.g. `[
+00007510: 2261 2e73 6822 2c20 2262 2e73 6822 5d60  "a.sh", "b.sh"]`
+00007520: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00007530: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00007540: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+00007550: 7320 207c 0a7c 2060 696e 7075 7473 4f70  s  |.| `inputsOp
+00007560: 7469 6f6e 616c 6020 2020 2020 2020 2020  tional`         
+00007570: 2020 7c20 4120 6c69 7374 206f 6620 696e    | A list of in
+00007580: 7075 7420 6669 6c65 7320 7265 7175 6972  put files requir
+00007590: 6564 2062 7920 6120 5461 736b 2c20 6275  ed by a Task, bu
+000075a0: 7420 7768 6963 6820 6172 6520 6e6f 7420  t which are not 
+000075b0: 7375 626a 6563 7420 746f 2076 6572 6966  subject to verif
+000075c0: 6963 6174 696f 6e2e 2043 616e 2063 6f6e  ication. Can con
+000075d0: 7461 696e 2077 696c 6463 6172 6473 2e20  tain wildcards. 
+000075e0: 452e 672e 3a20 605b 2274 6173 6b5f 6772  E.g.: `["task_gr
+000075f0: 6f75 705f 312f 2a2a 2f72 6573 756c 7473  oup_1/**/results
+00007600: 2e74 7874 225d 602e 2020 2020 2020 2020  .txt"]`.        
+00007610: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+00007620: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+00007630: 207c 2059 6573 2020 7c0a 7c20 6069 6e73   | Yes  |.| `ins
+00007640: 7461 6e63 6554 7970 6573 6020 2020 2020  tanceTypes`     
+00007650: 2020 2020 2020 207c 2054 6865 206d 6163         | The mac
+00007660: 6869 6e65 2069 6e73 7461 6e63 6520 7479  hine instance ty
+00007670: 7065 7320 7468 6174 2063 616e 2062 6520  pes that can be 
+00007680: 7573 6564 2074 6f20 6578 6563 7574 6520  used to execute 
+00007690: 5461 736b 732e 2045 2e67 2e2c 2060 5b22  Tasks. E.g., `["
+000076a0: 7433 2e6d 6963 726f 222c 2022 7433 612e  t3.micro", "t3a.
+000076b0: 6d69 6372 6f22 5d60 2e20 2020 2020 2020  micro"]`.       
 000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-00007710: 7c20 5965 7320 207c 2020 2020 2020 7c0a  | Yes  |      |.
-00007720: 7c20 606d 6178 696d 756d 5461 736b 5265  | `maximumTaskRe
-00007730: 7472 6965 7360 2020 2020 2020 207c 2054  tries`       | T
-00007740: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-00007750: 7220 6f66 2074 696d 6573 2061 2054 6173  r of times a Tas
-00007760: 6b20 6361 6e20 6265 2072 6574 7269 6564  k can be retried
-00007770: 2061 6674 6572 2069 7420 6861 7320 6661   after it has fa
-00007780: 696c 6564 2e20 452e 672e 3a20 6035 602e  iled. E.g.: `5`.
+00007700: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00007710: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
+00007720: 2060 6d61 7869 6d75 6d54 6173 6b52 6574   `maximumTaskRet
+00007730: 7269 6573 6020 2020 2020 2020 7c20 5468  ries`       | Th
+00007740: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
+00007750: 206f 6620 7469 6d65 7320 6120 5461 736b   of times a Task
+00007760: 2063 616e 2062 6520 7265 7472 6965 6420   can be retried 
+00007770: 6166 7465 7220 6974 2068 6173 2066 6169  after it has fai
+00007780: 6c65 642e 2045 2e67 2e3a 2060 3560 2e20  led. E.g.: `5`. 
 00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-000077f0: 2059 6573 207c 2059 6573 2020 7c20 2020   Yes | Yes  |   
-00007800: 2020 207c 0a7c 2060 6d61 7857 6f72 6b65     |.| `maxWorke
-00007810: 7273 6020 2020 2020 2020 2020 2020 2020  rs`             
-00007820: 2020 7c20 5468 6520 6d61 7869 6d75 6d20    | The maximum 
-00007830: 6e75 6d62 6572 206f 6620 576f 726b 6572  number of Worker
-00007840: 7320 7468 6174 2063 616e 2062 6520 636c  s that can be cl
-00007850: 6169 6d65 6420 666f 7220 7468 6520 6173  aimed for the as
-00007860: 736f 6369 6174 6564 2054 6173 6b20 4772  sociated Task Gr
-00007870: 6f75 702e 2045 2e67 2e2c 2060 3130 602e  oup. E.g., `10`.
+000077e0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+000077f0: 5965 7320 7c20 5965 7320 207c 2020 2020  Yes | Yes  |    
+00007800: 2020 7c0a 7c20 606d 6178 576f 726b 6572    |.| `maxWorker
+00007810: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
+00007820: 207c 2054 6865 206d 6178 696d 756d 206e   | The maximum n
+00007830: 756d 6265 7220 6f66 2057 6f72 6b65 7273  umber of Workers
+00007840: 2074 6861 7420 6361 6e20 6265 2063 6c61   that can be cla
+00007850: 696d 6564 2066 6f72 2074 6865 2061 7373  imed for the ass
+00007860: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
+00007870: 7570 2e20 452e 672e 2c20 6031 3060 2e20  up. E.g., `10`. 
 00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-000078d0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-000078e0: 207c 2020 2020 2020 7c0a 7c20 606d 696e   |      |.| `min
-000078f0: 576f 726b 6572 7360 2020 2020 2020 2020  Workers`        
-00007900: 2020 2020 2020 207c 2054 6865 206d 696e         | The min
-00007910: 696d 756d 206e 756d 6265 7220 6f66 2057  imum number of W
-00007920: 6f72 6b65 7273 2074 6861 7420 7468 6520  orkers that the 
-00007930: 6173 736f 6369 6174 6564 2054 6173 6b20  associated Task 
-00007940: 4772 6f75 7020 7265 7175 6972 6573 2e20  Group requires. 
-00007950: 5468 6973 206d 616e 7920 776f 726b 6572  This many worker
-00007960: 7320 6d75 7374 2062 6520 636c 6169 6d65  s must be claime
-00007970: 6420 6265 666f 7265 2074 6865 2061 7373  d before the ass
-00007980: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
-00007990: 7570 2077 696c 6c20 7374 6172 7420 776f  up will start wo
-000079a0: 726b 696e 672e 2045 2e67 2e2c 2060 3160  rking. E.g., `1`
-000079b0: 2e20 7c20 5965 7320 207c 2059 6573 207c  . | Yes  | Yes |
-000079c0: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
-000079d0: 2060 6e61 6d65 6020 2020 2020 2020 2020   `name`         
-000079e0: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-000079f0: 6520 6e61 6d65 206f 6620 7468 6520 576f  e name of the Wo
-00007a00: 726b 2052 6571 7569 7265 6d65 6e74 2c20  rk Requirement, 
-00007a10: 5461 736b 2047 726f 7570 206f 7220 5461  Task Group or Ta
-00007a20: 736b 2e20 452e 672e 2c20 6022 7772 5f6e  sk. E.g., `"wr_n
-00007a30: 616d 6522 602e 204e 6f74 6520 7468 6174  ame"`. Note that
-00007a40: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
-00007a50: 6572 7479 2069 7320 6e6f 7420 696e 6865  erty is not inhe
-00007a60: 7269 7465 642e 2020 2020 2020 2020 2020  rited.          
+000078c0: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+000078d0: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+000078e0: 7c20 2020 2020 207c 0a7c 2060 6d69 6e57  |      |.| `minW
+000078f0: 6f72 6b65 7273 6020 2020 2020 2020 2020  orkers`         
+00007900: 2020 2020 2020 7c20 5468 6520 6d69 6e69        | The mini
+00007910: 6d75 6d20 6e75 6d62 6572 206f 6620 576f  mum number of Wo
+00007920: 726b 6572 7320 7468 6174 2074 6865 2061  rkers that the a
+00007930: 7373 6f63 6961 7465 6420 5461 736b 2047  ssociated Task G
+00007940: 726f 7570 2072 6571 7569 7265 732e 2054  roup requires. T
+00007950: 6869 7320 6d61 6e79 2077 6f72 6b65 7273  his many workers
+00007960: 206d 7573 7420 6265 2063 6c61 696d 6564   must be claimed
+00007970: 2062 6566 6f72 6520 7468 6520 6173 736f   before the asso
+00007980: 6369 6174 6564 2054 6173 6b20 4772 6f75  ciated Task Grou
+00007990: 7020 7769 6c6c 2073 7461 7274 2077 6f72  p will start wor
+000079a0: 6b69 6e67 2e20 452e 672e 2c20 6031 602e  king. E.g., `1`.
+000079b0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+000079c0: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
+000079d0: 606e 616d 6560 2020 2020 2020 2020 2020  `name`          
+000079e0: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+000079f0: 206e 616d 6520 6f66 2074 6865 2057 6f72   name of the Wor
+00007a00: 6b20 5265 7175 6972 656d 656e 742c 2054  k Requirement, T
+00007a10: 6173 6b20 4772 6f75 7020 6f72 2054 6173  ask Group or Tas
+00007a20: 6b2e 2045 2e67 2e2c 2060 2277 725f 6e61  k. E.g., `"wr_na
+00007a30: 6d65 2260 2e20 4e6f 7465 2074 6861 7420  me"`. Note that 
+00007a40: 7468 6520 606e 616d 6560 2070 726f 7065  the `name` prope
+00007a50: 7274 7920 6973 206e 6f74 2069 6e68 6572  rty is not inher
+00007a60: 6974 6564 2e20 2020 2020 2020 2020 2020  ited.           
 00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00007aa0: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
-00007ab0: 2020 7c0a 7c20 606f 7574 7075 7473 6020    |.| `outputs` 
+00007a90: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+00007aa0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
+00007ab0: 207c 0a7c 2060 6f75 7470 7574 7360 2020   |.| `outputs`  
 00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 207c 2054 6865 2066 696c 6573 2074 6f20   | The files to 
-00007ae0: 6265 2075 706c 6f61 6465 6420 746f 2074  be uploaded to t
-00007af0: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
-00007b00: 6563 7420 5374 6f72 6520 6279 2061 2057  ect Store by a W
-00007b10: 6f72 6b65 7220 6e6f 6465 206f 6e20 636f  orker node on co
-00007b20: 6d70 6c65 7469 6f6e 206f 6620 7468 6520  mpletion of the 
-00007b30: 5461 736b 2e20 452e 672e 2c20 605b 2272  Task. E.g., `["r
-00007b40: 6573 756c 7473 5f31 2e74 7874 222c 2022  esults_1.txt", "
-00007b50: 7265 7375 6c74 735f 322e 7478 7422 5d60  results_2.txt"]`
-00007b60: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-00007b80: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-00007b90: 7c20 5965 7320 207c 0a7c 2060 6f75 7470  | Yes  |.| `outp
-00007ba0: 7574 7352 6571 7569 7265 6460 2020 2020  utsRequired`    
-00007bb0: 2020 2020 2020 7c20 5468 6520 6669 6c65        | The file
-00007bc0: 7320 7468 6174 202a 6d75 7374 2a20 6265  s that *must* be
-00007bd0: 2075 706c 6f61 6465 6420 746f 2074 6865   uploaded to the
-00007be0: 2059 656c 6c6f 7744 6f67 204f 626a 6563   YellowDog Objec
-00007bf0: 7420 5374 6f72 6520 6279 2061 2057 6f72  t Store by a Wor
-00007c00: 6b65 7220 6e6f 6465 206f 6e20 636f 6d70  ker node on comp
-00007c10: 6c65 7469 6f6e 206f 6620 7468 6520 5461  letion of the Ta
-00007c20: 736b 2e20 5468 6520 5461 736b 2077 696c  sk. The Task wil
-00007c30: 6c20 6661 696c 2069 6620 616e 7920 6f75  l fail if any ou
-00007c40: 7470 7574 7320 6172 6520 756e 6176 6169  tputs are unavai
-00007c50: 6c61 626c 652e 2020 2020 2020 2020 2020  lable.          
-00007c60: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00007c70: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
-00007c80: 6070 7269 6f72 6974 7960 2020 2020 2020  `priority`      
-00007c90: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00007ca0: 2070 7269 6f72 6974 7920 6f66 2057 6f72   priority of Wor
-00007cb0: 6b20 5265 7175 6972 656d 656e 7473 2061  k Requirements a
-00007cc0: 6e64 2054 6173 6b20 4772 6f75 7073 2e20  nd Task Groups. 
-00007cd0: 4869 6768 6572 2070 7269 6f72 6974 7920  Higher priority 
-00007ce0: 6163 7175 6972 6573 2057 6f72 6b65 7273  acquires Workers
-00007cf0: 2061 6865 6164 206f 6620 6c6f 7765 7220   ahead of lower 
-00007d00: 7072 696f 7269 7479 2e20 452e 672e 2c20  priority. E.g., 
-00007d10: 6030 2e30 602e 2020 2020 2020 2020 2020  `0.0`.          
+00007ad0: 7c20 5468 6520 6669 6c65 7320 746f 2062  | The files to b
+00007ae0: 6520 7570 6c6f 6164 6564 2074 6f20 7468  e uploaded to th
+00007af0: 6520 5965 6c6c 6f77 446f 6720 4f62 6a65  e YellowDog Obje
+00007b00: 6374 2053 746f 7265 2062 7920 6120 576f  ct Store by a Wo
+00007b10: 726b 6572 206e 6f64 6520 6f6e 2063 6f6d  rker node on com
+00007b20: 706c 6574 696f 6e20 6f66 2074 6865 2054  pletion of the T
+00007b30: 6173 6b2e 2045 2e67 2e2c 2060 5b22 7265  ask. E.g., `["re
+00007b40: 7375 6c74 735f 312e 7478 7422 2c20 2272  sults_1.txt", "r
+00007b50: 6573 756c 7473 5f32 2e74 7874 225d 602e  esults_2.txt"]`.
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+00007b80: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00007b90: 2059 6573 2020 7c0a 7c20 606f 7574 7075   Yes  |.| `outpu
+00007ba0: 7473 5265 7175 6972 6564 6020 2020 2020  tsRequired`     
+00007bb0: 2020 2020 207c 2054 6865 2066 696c 6573       | The files
+00007bc0: 2074 6861 7420 2a6d 7573 742a 2062 6520   that *must* be 
+00007bd0: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
+00007be0: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
+00007bf0: 2053 746f 7265 2062 7920 6120 576f 726b   Store by a Work
+00007c00: 6572 206e 6f64 6520 6f6e 2063 6f6d 706c  er node on compl
+00007c10: 6574 696f 6e20 6f66 2074 6865 2054 6173  etion of the Tas
+00007c20: 6b2e 2054 6865 2054 6173 6b20 7769 6c6c  k. The Task will
+00007c30: 2066 6169 6c20 6966 2061 6e79 206f 7574   fail if any out
+00007c40: 7075 7473 2061 7265 2075 6e61 7661 696c  puts are unavail
+00007c50: 6162 6c65 2e20 2020 2020 2020 2020 2020  able.           
+00007c60: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+00007c70: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+00007c80: 7072 696f 7269 7479 6020 2020 2020 2020  priority`       
+00007c90: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
+00007ca0: 7072 696f 7269 7479 206f 6620 576f 726b  priority of Work
+00007cb0: 2052 6571 7569 7265 6d65 6e74 7320 616e   Requirements an
+00007cc0: 6420 5461 736b 2047 726f 7570 732e 2048  d Task Groups. H
+00007cd0: 6967 6865 7220 7072 696f 7269 7479 2061  igher priority a
+00007ce0: 6371 7569 7265 7320 576f 726b 6572 7320  cquires Workers 
+00007cf0: 6168 6561 6420 6f66 206c 6f77 6572 2070  ahead of lower p
+00007d00: 7269 6f72 6974 792e 2045 2e67 2e2c 2060  riority. E.g., `
+00007d10: 302e 3060 2e20 2020 2020 2020 2020 2020  0.0`.           
 00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00007d50: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
-00007d60: 207c 0a7c 2060 7072 6f76 6964 6572 7360   |.| `providers`
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 7c20 436f 6e73 7472 6169 6e73 2074 6865  | Constrains the
-00007d90: 2059 656c 6c6f 7744 6f67 2053 6368 6564   YellowDog Sched
-00007da0: 756c 6572 206f 6e6c 7920 746f 2065 7865  uler only to exe
-00007db0: 6375 7465 2074 6173 6b73 2066 726f 6d20  cute tasks from 
-00007dc0: 7468 6520 6173 736f 6369 6174 6564 2054  the associated T
-00007dd0: 6173 6b20 4772 6f75 7020 6f6e 2074 6865  ask Group on the
-00007de0: 2073 7065 6369 6669 6564 2070 726f 7669   specified provi
-00007df0: 6465 7273 2e20 452e 672e 2c20 605b 2241  ders. E.g., `["A
-00007e00: 5753 222c 2022 474f 4f47 4c45 225d 602e  WS", "GOOGLE"]`.
+00007d40: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00007d50: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
+00007d60: 7c0a 7c20 6070 726f 7669 6465 7273 6020  |.| `providers` 
+00007d70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007d80: 2043 6f6e 7374 7261 696e 7320 7468 6520   Constrains the 
+00007d90: 5965 6c6c 6f77 446f 6720 5363 6865 6475  YellowDog Schedu
+00007da0: 6c65 7220 6f6e 6c79 2074 6f20 6578 6563  ler only to exec
+00007db0: 7574 6520 7461 736b 7320 6672 6f6d 2074  ute tasks from t
+00007dc0: 6865 2061 7373 6f63 6961 7465 6420 5461  he associated Ta
+00007dd0: 736b 2047 726f 7570 206f 6e20 7468 6520  sk Group on the 
+00007de0: 7370 6563 6966 6965 6420 7072 6f76 6964  specified provid
+00007df0: 6572 732e 2045 2e67 2e2c 2060 5b22 4157  ers. E.g., `["AW
+00007e00: 5322 2c20 2247 4f4f 474c 4522 5d60 2e20  S", "GOOGLE"]`. 
 00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00007e30: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00007e40: 2020 2020 2020 7c0a 7c20 6072 616d 6020        |.| `ram` 
+00007e20: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+00007e30: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
+00007e40: 2020 2020 207c 0a7c 2060 7261 6d60 2020       |.| `ram`  
 00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 207c 2052 616e 6765 2063 6f6e       | Range con
-00007e70: 7374 7261 696e 7420 6f6e 2047 4220 6f66  straint on GB of
-00007e80: 2052 414d 2074 6861 7420 6172 6520 7265   RAM that are re
-00007e90: 7175 6972 6564 2074 6f20 6578 6563 7574  quired to execut
-00007ea0: 6520 5461 736b 732e 2045 2e67 2e2c 2060  e Tasks. E.g., `
-00007eb0: 5b32 2e35 2c20 342e 305d 602e 2020 2020  [2.5, 4.0]`.    
+00007e60: 2020 2020 7c20 5261 6e67 6520 636f 6e73      | Range cons
+00007e70: 7472 6169 6e74 206f 6e20 4742 206f 6620  traint on GB of 
+00007e80: 5241 4d20 7468 6174 2061 7265 2072 6571  RAM that are req
+00007e90: 7569 7265 6420 746f 2065 7865 6375 7465  uired to execute
+00007ea0: 2054 6173 6b73 2e20 452e 672e 2c20 605b   Tasks. E.g., `[
+00007eb0: 322e 352c 2034 2e30 5d60 2e20 2020 2020  2.5, 4.0]`.     
 00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00007f20: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
-00007f30: 7265 6769 6f6e 7360 2020 2020 2020 2020  regions`        
-00007f40: 2020 2020 2020 2020 2020 7c20 436f 6e73            | Cons
-00007f50: 7472 6169 6e73 2074 6865 2059 656c 6c6f  trains the Yello
-00007f60: 7744 6f67 2053 6368 6564 756c 6572 206f  wDog Scheduler o
-00007f70: 6e6c 7920 746f 2065 7865 6375 7465 2054  nly to execute T
-00007f80: 6173 6b73 2066 726f 6d20 7468 6520 6173  asks from the as
-00007f90: 736f 6369 6174 6564 2054 6173 6b20 4772  sociated Task Gr
-00007fa0: 6f75 7020 696e 2074 6865 2073 7065 6369  oup in the speci
-00007fb0: 6669 6564 2072 6567 696f 6e73 2e20 452e  fied regions. E.
-00007fc0: 672e 2c20 605b 2265 752d 7765 7374 2d32  g., `["eu-west-2
-00007fd0: 5d60 2e20 2020 2020 2020 2020 2020 2020  ]`.             
+00007f00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007f10: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
+00007f20: 7320 207c 2020 2020 2020 7c0a 7c20 6072  s  |      |.| `r
+00007f30: 6567 696f 6e73 6020 2020 2020 2020 2020  egions`         
+00007f40: 2020 2020 2020 2020 207c 2043 6f6e 7374           | Const
+00007f50: 7261 696e 7320 7468 6520 5965 6c6c 6f77  rains the Yellow
+00007f60: 446f 6720 5363 6865 6475 6c65 7220 6f6e  Dog Scheduler on
+00007f70: 6c79 2074 6f20 6578 6563 7574 6520 5461  ly to execute Ta
+00007f80: 736b 7320 6672 6f6d 2074 6865 2061 7373  sks from the ass
+00007f90: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
+00007fa0: 7570 2069 6e20 7468 6520 7370 6563 6966  up in the specif
+00007fb0: 6965 6420 7265 6769 6f6e 732e 2045 2e67  ied regions. E.g
+00007fc0: 2e2c 2060 5b22 6575 2d77 6573 742d 325d  ., `["eu-west-2]
+00007fd0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
 00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-00008000: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
-00008010: 7c0a 7c20 6074 6173 6b42 6174 6368 5369  |.| `taskBatchSi
-00008020: 7a65 6020 2020 2020 2020 2020 2020 207c  ze`            |
-00008030: 2044 6574 6572 6d69 6e65 7320 7468 6520   Determines the 
-00008040: 6261 7463 6820 7369 7a65 2075 7365 6420  batch size used 
-00008050: 746f 2061 6464 2054 6173 6b73 2074 6f20  to add Tasks to 
-00008060: 5461 736b 2047 726f 7570 732e 2044 6566  Task Groups. Def
-00008070: 6175 6c74 2069 7320 322c 3030 302e 2020  ault is 2,000.  
+00007ff0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+00008000: 207c 2059 6573 2020 7c20 2020 2020 207c   | Yes  |      |
+00008010: 0a7c 2060 7461 736b 4261 7463 6853 697a  .| `taskBatchSiz
+00008020: 6560 2020 2020 2020 2020 2020 2020 7c20  e`            | 
+00008030: 4465 7465 726d 696e 6573 2074 6865 2062  Determines the b
+00008040: 6174 6368 2073 697a 6520 7573 6564 2074  atch size used t
+00008050: 6f20 6164 6420 5461 736b 7320 746f 2054  o add Tasks to T
+00008060: 6173 6b20 4772 6f75 7073 2e20 4465 6661  ask Groups. Defa
+00008070: 756c 7420 6973 2032 2c30 3030 2e20 2020  ult is 2,000.   
 00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-000080e0: 207c 2020 2020 207c 2020 2020 2020 7c20   |     |      | 
-000080f0: 2020 2020 207c 0a7c 2060 7461 736b 436f       |.| `taskCo
-00008100: 756e 7460 2020 2020 2020 2020 2020 2020  unt`            
-00008110: 2020 2020 7c20 5468 6520 6e75 6d62 6572      | The number
-00008120: 206f 6620 7469 6d65 7320 746f 2065 7865   of times to exe
-00008130: 6375 7465 2074 6865 2054 6173 6b2e 2043  cute the Task. C
-00008140: 616e 2062 6520 7365 7420 696e 2074 6865  an be set in the
-00008150: 2054 4f4d 4c20 6669 6c65 206f 7220 696e   TOML file or in
-00008160: 2061 6e79 204a 534f 4e20 5461 736b 2047   any JSON Task G
-00008170: 726f 7570 2064 6566 696e 6974 696f 6e2e  roup definition.
-00008180: 204e 6f74 653a 206e 6f20 696e 6865 7269   Note: no inheri
-00008190: 7461 6e63 6520 6672 6f6d 2054 4f4d 4c20  tance from TOML 
-000081a0: 746f 204a 534f 4e2e 2020 2020 2020 2020  to JSON.        
-000081b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000081c0: 2059 6573 2020 7c20 2020 2020 7c20 5965   Yes  |     | Ye
-000081d0: 7320 207c 2020 2020 2020 7c0a 7c20 6074  s  |      |.| `t
-000081e0: 6173 6b44 6174 6160 2020 2020 2020 2020  askData`        
-000081f0: 2020 2020 2020 2020 207c 2054 6865 2064           | The d
-00008200: 6174 6120 746f 2062 6520 7061 7373 6564  ata to be passed
-00008210: 2074 6f20 7468 6520 576f 726b 6572 2077   to the Worker w
-00008220: 6865 6e20 7468 6520 5461 736b 2069 7320  hen the Task is 
-00008230: 7374 6172 7465 642e 2045 2e67 2e2c 2060  started. E.g., `
-00008240: 226d 7964 6174 6122 602e 2042 6563 6f6d  "mydata"`. Becom
-00008250: 6573 2066 696c 6520 6074 6173 6b64 6174  es file `taskdat
-00008260: 612e 7478 7460 2069 6e20 7468 6520 5461  a.txt` in the Ta
-00008270: 736b 2773 2077 6f72 6b69 6e67 2064 6972  sk's working dir
-00008280: 6563 746f 7279 2077 6865 6e20 5468 6520  ectory when The 
-00008290: 5461 736b 2065 7865 6375 7465 732e 2020  Task executes.  
-000082a0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-000082b0: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
-000082c0: 0a7c 2060 7461 736b 4461 7461 4669 6c65  .| `taskDataFile
-000082d0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
-000082e0: 506f 7075 6c61 7465 2074 6865 2060 7461  Populate the `ta
-000082f0: 736b 4461 7461 6020 7072 6f70 6572 7479  skData` property
-00008300: 2061 626f 7665 2077 6974 6820 7468 6520   above with the 
-00008310: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
-00008320: 7370 6563 6966 6965 6420 6669 6c65 2e20  specified file. 
-00008330: 452e 672e 2c20 6022 6d79 5f74 6173 6b5f  E.g., `"my_task_
-00008340: 6461 7461 5f66 696c 652e 7478 7422 602e  data_file.txt"`.
+000080d0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+000080e0: 7c20 2020 2020 7c20 2020 2020 207c 2020  |     |      |  
+000080f0: 2020 2020 7c0a 7c20 6074 6173 6b43 6f75      |.| `taskCou
+00008100: 6e74 6020 2020 2020 2020 2020 2020 2020  nt`             
+00008110: 2020 207c 2054 6865 206e 756d 6265 7220     | The number 
+00008120: 6f66 2074 696d 6573 2074 6f20 6578 6563  of times to exec
+00008130: 7574 6520 7468 6520 5461 736b 2e20 4361  ute the Task. Ca
+00008140: 6e20 6265 2073 6574 2069 6e20 7468 6520  n be set in the 
+00008150: 544f 4d4c 2066 696c 6520 6f72 2069 6e20  TOML file or in 
+00008160: 616e 7920 4a53 4f4e 2054 6173 6b20 4772  any JSON Task Gr
+00008170: 6f75 7020 6465 6669 6e69 7469 6f6e 2e20  oup definition. 
+00008180: 4e6f 7465 3a20 6e6f 2069 6e68 6572 6974  Note: no inherit
+00008190: 616e 6365 2066 726f 6d20 544f 4d4c 2074  ance from TOML t
+000081a0: 6f20 4a53 4f4e 2e20 2020 2020 2020 2020  o JSON.         
+000081b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000081c0: 5965 7320 207c 2020 2020 207c 2059 6573  Yes  |     | Yes
+000081d0: 2020 7c20 2020 2020 207c 0a7c 2060 7461    |      |.| `ta
+000081e0: 736b 4461 7461 6020 2020 2020 2020 2020  skData`         
+000081f0: 2020 2020 2020 2020 7c20 5468 6520 6461          | The da
+00008200: 7461 2074 6f20 6265 2070 6173 7365 6420  ta to be passed 
+00008210: 746f 2074 6865 2057 6f72 6b65 7220 7768  to the Worker wh
+00008220: 656e 2074 6865 2054 6173 6b20 6973 2073  en the Task is s
+00008230: 7461 7274 6564 2e20 452e 672e 2c20 6022  tarted. E.g., `"
+00008240: 6d79 6461 7461 2260 2e20 4265 636f 6d65  mydata"`. Become
+00008250: 7320 6669 6c65 2060 7461 736b 6461 7461  s file `taskdata
+00008260: 2e74 7874 6020 696e 2074 6865 2054 6173  .txt` in the Tas
+00008270: 6b27 7320 776f 726b 696e 6720 6469 7265  k's working dire
+00008280: 6374 6f72 7920 7768 656e 2054 6865 2054  ctory when The T
+00008290: 6173 6b20 6578 6563 7574 6573 2e20 2020  ask executes.   
+000082a0: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+000082b0: 7c20 5965 7320 207c 2059 6573 2020 7c0a  | Yes  | Yes  |.
+000082c0: 7c20 6074 6173 6b44 6174 6146 696c 6560  | `taskDataFile`
+000082d0: 2020 2020 2020 2020 2020 2020 207c 2050               | P
+000082e0: 6f70 756c 6174 6520 7468 6520 6074 6173  opulate the `tas
+000082f0: 6b44 6174 6160 2070 726f 7065 7274 7920  kData` property 
+00008300: 6162 6f76 6520 7769 7468 2074 6865 2063  above with the c
+00008310: 6f6e 7465 6e74 7320 6f66 2074 6865 2073  ontents of the s
+00008320: 7065 6369 6669 6564 2066 696c 652e 2045  pecified file. E
+00008330: 2e67 2e2c 2060 226d 795f 7461 736b 5f64  .g., `"my_task_d
+00008340: 6174 615f 6669 6c65 2e74 7874 2260 2e20  ata_file.txt"`. 
 00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-00008390: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
-000083a0: 6573 2020 7c0a 7c20 6074 6173 6b4e 616d  es  |.| `taskNam
-000083b0: 6560 2020 2020 2020 2020 2020 2020 2020  e`              
-000083c0: 2020 207c 2054 6865 206e 616d 6520 746f     | The name to
-000083d0: 2075 7365 2066 6f72 2074 6865 2054 6173   use for the Tas
-000083e0: 6b2e 204f 6e6c 7920 7573 6162 6c65 2069  k. Only usable i
-000083f0: 6e20 7468 6520 544f 4d4c 2066 696c 652e  n the TOML file.
-00008400: 204d 6f73 746c 7920 7573 6566 756c 2069   Mostly useful i
-00008410: 6e20 636f 6e6a 756e 6374 696f 6e20 7769  n conjunction wi
-00008420: 7468 2043 5356 2054 6173 6b20 6461 7461  th CSV Task data
-00008430: 2e20 452e 672e 2c20 6022 6d79 5f74 6173  . E.g., `"my_tas
-00008440: 6b5f 6e75 6d62 6572 5f7b 7b74 6173 6b5f  k_number_{{task_
-00008450: 6e75 6d62 6572 7d7d 2260 2e20 2020 2020  number}}"`.     
-00008460: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00008470: 5965 7320 207c 2020 2020 207c 2020 2020  Yes  |     |    
-00008480: 2020 7c20 2020 2020 207c 0a7c 2060 7461    |      |.| `ta
-00008490: 736b 4772 6f75 704e 616d 6560 2020 2020  skGroupName`    
-000084a0: 2020 2020 2020 2020 7c20 5468 6520 6e61          | The na
-000084b0: 6d65 2074 6f20 7573 6520 666f 7220 7468  me to use for th
-000084c0: 6520 5461 736b 2047 726f 7570 2e20 4f6e  e Task Group. On
-000084d0: 6c79 2075 7361 626c 6520 696e 2074 6865  ly usable in the
-000084e0: 2054 4f4d 4c20 6669 6c65 2e20 452e 672e   TOML file. E.g.
-000084f0: 2c20 6022 6d79 5f74 675f 6e75 6d62 6572  , `"my_tg_number
-00008500: 5f7b 7b74 6173 6b5f 6772 6f75 705f 6e75  _{{task_group_nu
-00008510: 6d62 6572 7d7d 2260 2e20 2020 2020 2020  mber}}"`.       
+00008380: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00008390: 2059 6573 207c 2059 6573 2020 7c20 5965   Yes | Yes  | Ye
+000083a0: 7320 207c 0a7c 2060 7461 736b 4e61 6d65  s  |.| `taskName
+000083b0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+000083c0: 2020 7c20 5468 6520 6e61 6d65 2074 6f20    | The name to 
+000083d0: 7573 6520 666f 7220 7468 6520 5461 736b  use for the Task
+000083e0: 2e20 4f6e 6c79 2075 7361 626c 6520 696e  . Only usable in
+000083f0: 2074 6865 2054 4f4d 4c20 6669 6c65 2e20   the TOML file. 
+00008400: 4d6f 7374 6c79 2075 7365 6675 6c20 696e  Mostly useful in
+00008410: 2063 6f6e 6a75 6e63 7469 6f6e 2077 6974   conjunction wit
+00008420: 6820 4353 5620 5461 736b 2064 6174 612e  h CSV Task data.
+00008430: 2045 2e67 2e2c 2060 226d 795f 7461 736b   E.g., `"my_task
+00008440: 5f6e 756d 6265 725f 7b7b 7461 736b 5f6e  _number_{{task_n
+00008450: 756d 6265 727d 7d22 602e 2020 2020 2020  umber}}"`.      
+00008460: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+00008470: 6573 2020 7c20 2020 2020 7c20 2020 2020  es  |     |     
+00008480: 207c 2020 2020 2020 7c0a 7c20 6074 6173   |      |.| `tas
+00008490: 6b47 726f 7570 4e61 6d65 6020 2020 2020  kGroupName`     
+000084a0: 2020 2020 2020 207c 2054 6865 206e 616d         | The nam
+000084b0: 6520 746f 2075 7365 2066 6f72 2074 6865  e to use for the
+000084c0: 2054 6173 6b20 4772 6f75 702e 204f 6e6c   Task Group. Onl
+000084d0: 7920 7573 6162 6c65 2069 6e20 7468 6520  y usable in the 
+000084e0: 544f 4d4c 2066 696c 652e 2045 2e67 2e2c  TOML file. E.g.,
+000084f0: 2060 226d 795f 7467 5f6e 756d 6265 725f   `"my_tg_number_
+00008500: 7b7b 7461 736b 5f67 726f 7570 5f6e 756d  {{task_group_num
+00008510: 6265 727d 7d22 602e 2020 2020 2020 2020  ber}}"`.        
 00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
-00008560: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
-00008570: 7c20 6074 6173 6b54 7970 6560 2020 2020  | `taskType`    
-00008580: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-00008590: 6865 2054 6173 6b20 5479 7065 206f 6620  he Task Type of 
-000085a0: 6120 5461 736b 2e20 452e 672e 2c20 6022  a Task. E.g., `"
-000085b0: 646f 636b 6572 2260 2e20 2020 2020 2020  docker"`.       
+00008550: 2020 7c20 5965 7320 207c 2020 2020 207c    | Yes  |     |
+00008560: 2020 2020 2020 7c20 2020 2020 207c 0a7c        |      |.|
+00008570: 2060 7461 736b 5479 7065 6020 2020 2020   `taskType`     
+00008580: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+00008590: 6520 5461 736b 2054 7970 6520 6f66 2061  e Task Type of a
+000085a0: 2054 6173 6b2e 2045 2e67 2e2c 2060 2264   Task. E.g., `"d
+000085b0: 6f63 6b65 7222 602e 2020 2020 2020 2020  ocker"`.        
 000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-00008640: 2020 2020 207c 2020 2020 2020 7c20 5965       |      | Ye
-00008650: 7320 207c 0a7c 2060 7461 736b 5479 7065  s  |.| `taskType
-00008660: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
-00008670: 2020 7c20 5468 6520 6c69 7374 206f 6620    | The list of 
-00008680: 5461 736b 2054 7970 6573 2072 6571 7569  Task Types requi
-00008690: 7265 6420 6279 2074 6865 2072 616e 6765  red by the range
-000086a0: 206f 6620 5461 736b 7320 696e 2061 2054   of Tasks in a T
-000086b0: 6173 6b20 4772 6f75 702e 2045 2e67 2e2c  ask Group. E.g.,
-000086c0: 2060 5b22 646f 636b 6572 222c 2062 6173   `["docker", bas
-000086d0: 6822 5d60 2e20 2020 2020 2020 2020 2020  h"]`.           
+00008630: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00008640: 2020 2020 7c20 2020 2020 207c 2059 6573      |      | Yes
+00008650: 2020 7c0a 7c20 6074 6173 6b54 7970 6573    |.| `taskTypes
+00008660: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00008670: 207c 2054 6865 206c 6973 7420 6f66 2054   | The list of T
+00008680: 6173 6b20 5479 7065 7320 7265 7175 6972  ask Types requir
+00008690: 6564 2062 7920 7468 6520 7261 6e67 6520  ed by the range 
+000086a0: 6f66 2054 6173 6b73 2069 6e20 6120 5461  of Tasks in a Ta
+000086b0: 736b 2047 726f 7570 2e20 452e 672e 2c20  sk Group. E.g., 
+000086c0: 605b 2264 6f63 6b65 7222 2c20 6261 7368  `["docker", bash
+000086d0: 225d 602e 2020 2020 2020 2020 2020 2020  "]`.            
 000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00008720: 2020 2020 7c20 5965 7320 7c20 5965 7320      | Yes | Yes 
-00008730: 207c 2020 2020 2020 7c0a 7c20 6074 6173   |      |.| `tas
-00008740: 6b73 5065 7257 6f72 6b65 7260 2020 2020  ksPerWorker`    
-00008750: 2020 2020 2020 207c 2044 6574 6572 6d69         | Determi
-00008760: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
-00008770: 6620 576f 726b 6572 2063 6c61 696d 7320  f Worker claims 
-00008780: 6261 7365 6420 6f6e 2073 706c 6974 7469  based on splitti
-00008790: 6e67 2074 6865 206e 756d 6265 7220 6f66  ng the number of
-000087a0: 2075 6e66 696e 6973 6865 6420 5461 736b   unfinished Task
-000087b0: 7320 6163 726f 7373 2057 6f72 6b65 7273  s across Workers
-000087c0: 2e20 452e 672e 2c20 6031 602e 2020 2020  . E.g., `1`.    
+00008710: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00008720: 2020 207c 2059 6573 207c 2059 6573 2020     | Yes | Yes  
+00008730: 7c20 2020 2020 207c 0a7c 2060 7461 736b  |      |.| `task
+00008740: 7350 6572 576f 726b 6572 6020 2020 2020  sPerWorker`     
+00008750: 2020 2020 2020 7c20 4465 7465 726d 696e        | Determin
+00008760: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
+00008770: 2057 6f72 6b65 7220 636c 6169 6d73 2062   Worker claims b
+00008780: 6173 6564 206f 6e20 7370 6c69 7474 696e  ased on splittin
+00008790: 6720 7468 6520 6e75 6d62 6572 206f 6620  g the number of 
+000087a0: 756e 6669 6e69 7368 6564 2054 6173 6b73  unfinished Tasks
+000087b0: 2061 6372 6f73 7320 576f 726b 6572 732e   across Workers.
+000087c0: 2045 2e67 2e2c 2060 3160 2e20 2020 2020   E.g., `1`.     
 000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-00008810: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
-00008820: 2060 7570 6c6f 6164 4669 6c65 7360 2020   `uploadFiles`  
-00008830: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-00008840: 6520 6c69 7374 206f 6620 6669 6c65 7320  e list of files 
-00008850: 746f 2062 6520 7570 6c6f 6164 6564 2074  to be uploaded t
-00008860: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
-00008870: 4f62 6a65 6374 2053 746f 7265 2e20 452e  Object Store. E.
-00008880: 672e 2c20 284a 534f 4e29 3a20 605b 7b22  g., (JSON): `[{"
-00008890: 6c6f 6361 6c50 6174 6822 3a20 6669 6c65  localPath": file
-000088a0: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
-000088b0: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
-000088c0: 7874 227d 5d60 2e20 2020 2020 2020 2020  xt"}]`.         
+00008800: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+00008810: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
+00008820: 6075 706c 6f61 6446 696c 6573 6020 2020  `uploadFiles`   
+00008830: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+00008840: 206c 6973 7420 6f66 2066 696c 6573 2074   list of files t
+00008850: 6f20 6265 2075 706c 6f61 6465 6420 746f  o be uploaded to
+00008860: 2074 6865 2059 656c 6c6f 7744 6f67 204f   the YellowDog O
+00008870: 626a 6563 7420 5374 6f72 652e 2045 2e67  bject Store. E.g
+00008880: 2e2c 2028 4a53 4f4e 293a 2060 5b7b 226c  ., (JSON): `[{"l
+00008890: 6f63 616c 5061 7468 223a 2066 696c 655f  ocalPath": file_
+000088a0: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
+000088b0: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
+000088c0: 7422 7d5d 602e 2020 2020 2020 2020 2020  t"}]`.          
 000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-000088f0: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
-00008900: 2020 7c0a 7c20 6076 6370 7573 6020 2020    |.| `vcpus`   
+000088e0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+000088f0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
+00008900: 207c 0a7c 2060 7663 7075 7360 2020 2020   |.| `vcpus`    
 00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 207c 2052 616e 6765 2063 6f6e 7374 7261   | Range constra
-00008930: 696e 7420 6f6e 206e 756d 6265 7220 6f66  int on number of
-00008940: 2076 4350 5573 2074 6861 7420 6172 6520   vCPUs that are 
-00008950: 7265 7175 6972 6564 2074 6f20 6578 6563  required to exec
-00008960: 7574 6520 5461 736b 7320 452e 672e 2c20  ute Tasks E.g., 
-00008970: 605b 322e 302c 2034 2e30 5d60 2e20 2020  `[2.0, 4.0]`.   
+00008920: 7c20 5261 6e67 6520 636f 6e73 7472 6169  | Range constrai
+00008930: 6e74 206f 6e20 6e75 6d62 6572 206f 6620  nt on number of 
+00008940: 7643 5055 7320 7468 6174 2061 7265 2072  vCPUs that are r
+00008950: 6571 7569 7265 6420 746f 2065 7865 6375  equired to execu
+00008960: 7465 2054 6173 6b73 2045 2e67 2e2c 2060  te Tasks E.g., `
+00008970: 5b32 2e30 2c20 342e 305d 602e 2020 2020  [2.0, 4.0]`.    
 00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-000089d0: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-000089e0: 7c20 2020 2020 207c 0a7c 2060 7665 7269  |      |.| `veri
-000089f0: 6679 4174 5374 6172 7460 2020 2020 2020  fyAtStart`      
-00008a00: 2020 2020 2020 7c20 4120 6c69 7374 206f        | A list o
-00008a10: 6620 6669 6c65 7320 7265 7175 6972 6564  f files required
-00008a20: 2062 7920 6120 5461 736b 2e20 4d75 7374   by a Task. Must
-00008a30: 2062 6520 7072 6573 656e 7420 7768 656e   be present when
-00008a40: 2074 6865 2054 6173 6b20 6973 2072 6561   the Task is rea
-00008a50: 6479 2074 6f20 7374 6172 7420 6f72 2074  dy to start or t
-00008a60: 6865 2054 6173 6b20 7769 6c6c 2066 6169  he Task will fai
-00008a70: 6c2e 2045 2e67 2e3a 2060 5b22 7461 736b  l. E.g.: `["task
-00008a80: 5f67 726f 7570 5f31 2f74 6173 6b5f 312f  _group_1/task_1/
-00008a90: 7265 7375 6c74 732e 7478 7422 5d60 2e20  results.txt"]`. 
+000089c0: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+000089d0: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+000089e0: 2020 2020 2020 7c0a 7c20 6076 6572 6966        |.| `verif
+000089f0: 7941 7453 7461 7274 6020 2020 2020 2020  yAtStart`       
+00008a00: 2020 2020 207c 2041 206c 6973 7420 6f66       | A list of
+00008a10: 2066 696c 6573 2072 6571 7569 7265 6420   files required 
+00008a20: 6279 2061 2054 6173 6b2e 204d 7573 7420  by a Task. Must 
+00008a30: 6265 2070 7265 7365 6e74 2077 6865 6e20  be present when 
+00008a40: 7468 6520 5461 736b 2069 7320 7265 6164  the Task is read
+00008a50: 7920 746f 2073 7461 7274 206f 7220 7468  y to start or th
+00008a60: 6520 5461 736b 2077 696c 6c20 6661 696c  e Task will fail
+00008a70: 2e20 452e 672e 3a20 605b 2274 6173 6b5f  . E.g.: `["task_
+00008a80: 6772 6f75 705f 312f 7461 736b 5f31 2f72  group_1/task_1/r
+00008a90: 6573 756c 7473 2e74 7874 225d 602e 2020  esults.txt"]`.  
 00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00008ac0: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
-00008ad0: 6076 6572 6966 7957 6169 7460 2020 2020  `verifyWait`    
-00008ae0: 2020 2020 2020 2020 2020 207c 2041 206c             | A l
-00008af0: 6973 7420 6f66 2066 696c 6573 2072 6571  ist of files req
-00008b00: 7569 7265 6420 6279 2061 2054 6173 6b2e  uired by a Task.
-00008b10: 2054 6865 2054 6173 6b20 7769 6c6c 2077   The Task will w
-00008b20: 6169 7420 756e 7469 6c20 7468 6520 6669  ait until the fi
-00008b30: 6c65 7320 6172 6520 6176 6169 6c61 626c  les are availabl
-00008b40: 6520 6265 666f 7265 2073 7461 7274 696e  e before startin
-00008b50: 672e 2045 2e67 2e3a 2060 5b22 7461 736b  g. E.g.: `["task
-00008b60: 5f67 726f 7570 5f31 2f74 6173 6b5f 312f  _group_1/task_1/
-00008b70: 7265 7375 6c74 732e 7478 7422 5d60 2e20  results.txt"]`. 
+00008ab0: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+00008ac0: 6573 2020 7c20 5965 7320 207c 0a7c 2060  es  | Yes  |.| `
+00008ad0: 7665 7269 6679 5761 6974 6020 2020 2020  verifyWait`     
+00008ae0: 2020 2020 2020 2020 2020 7c20 4120 6c69            | A li
+00008af0: 7374 206f 6620 6669 6c65 7320 7265 7175  st of files requ
+00008b00: 6972 6564 2062 7920 6120 5461 736b 2e20  ired by a Task. 
+00008b10: 5468 6520 5461 736b 2077 696c 6c20 7761  The Task will wa
+00008b20: 6974 2075 6e74 696c 2074 6865 2066 696c  it until the fil
+00008b30: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
+00008b40: 2062 6566 6f72 6520 7374 6172 7469 6e67   before starting
+00008b50: 2e20 452e 672e 3a20 605b 2274 6173 6b5f  . E.g.: `["task_
+00008b60: 6772 6f75 705f 312f 7461 736b 5f31 2f72  group_1/task_1/r
+00008b70: 6573 756c 7473 2e74 7874 225d 602e 2020  esults.txt"]`.  
 00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00008ba0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
-00008bb0: 207c 0a7c 2060 776f 726b 6572 5461 6773   |.| `workerTags
-00008bc0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00008bd0: 7c20 5468 6520 6c69 7374 206f 6620 576f  | The list of Wo
-00008be0: 726b 6572 2054 6167 7320 7468 6174 2077  rker Tags that w
-00008bf0: 696c 6c20 6265 2075 7365 6420 746f 206d  ill be used to m
-00008c00: 6174 6368 2061 6761 696e 7374 2074 6865  atch against the
-00008c10: 2057 6f72 6b65 7220 5461 6720 6f66 2061   Worker Tag of a
-00008c20: 2063 616e 6469 6461 7465 2057 6f72 6b65   candidate Worke
-00008c30: 722e 2045 2e67 2e2c 2060 5b22 7461 675f  r. E.g., `["tag_
-00008c40: 7822 2c20 2274 6167 5f79 225d 602e 2020  x", "tag_y"]`.  
+00008b90: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00008ba0: 7320 7c20 5965 7320 207c 2059 6573 2020  s | Yes  | Yes  
+00008bb0: 7c0a 7c20 6077 6f72 6b65 7254 6167 7360  |.| `workerTags`
+00008bc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00008bd0: 2054 6865 206c 6973 7420 6f66 2057 6f72   The list of Wor
+00008be0: 6b65 7220 5461 6773 2074 6861 7420 7769  ker Tags that wi
+00008bf0: 6c6c 2062 6520 7573 6564 2074 6f20 6d61  ll be used to ma
+00008c00: 7463 6820 6167 6169 6e73 7420 7468 6520  tch against the 
+00008c10: 576f 726b 6572 2054 6167 206f 6620 6120  Worker Tag of a 
+00008c20: 6361 6e64 6964 6174 6520 576f 726b 6572  candidate Worker
+00008c30: 2e20 452e 672e 2c20 605b 2274 6167 5f78  . E.g., `["tag_x
+00008c40: 222c 2022 7461 675f 7922 5d60 2e20 2020  ", "tag_y"]`.   
 00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00008c80: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00008c90: 2020 2020 2020 7c0a 7c20 6077 6f72 6b52        |.| `workR
-00008ca0: 6571 7569 7265 6d65 6e74 4461 7461 6020  equirementData` 
-00008cb0: 2020 2020 207c 2054 6865 206e 616d 6520       | The name 
-00008cc0: 6f66 2074 6865 2066 696c 6520 636f 6e74  of the file cont
-00008cd0: 6169 6e69 6e67 2074 6865 204a 534f 4e20  aining the JSON 
-00008ce0: 646f 6375 6d65 6e74 2069 6e20 7768 6963  document in whic
-00008cf0: 6820 7468 6520 576f 726b 2052 6571 7569  h the Work Requi
-00008d00: 7265 6d65 6e74 2069 7320 6465 6669 6e65  rement is define
-00008d10: 642e 2045 2e67 2e2c 2060 2274 6573 745f  d. E.g., `"test_
-00008d20: 776f 726b 7265 712e 6a73 6f6e 2260 2e20  workreq.json"`. 
+00008c70: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+00008c80: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
+00008c90: 2020 2020 207c 0a7c 2060 776f 726b 5265       |.| `workRe
+00008ca0: 7175 6972 656d 656e 7444 6174 6160 2020  quirementData`  
+00008cb0: 2020 2020 7c20 5468 6520 6e61 6d65 206f      | The name o
+00008cc0: 6620 7468 6520 6669 6c65 2063 6f6e 7461  f the file conta
+00008cd0: 696e 696e 6720 7468 6520 4a53 4f4e 2064  ining the JSON d
+00008ce0: 6f63 756d 656e 7420 696e 2077 6869 6368  ocument in which
+00008cf0: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+00008d00: 656d 656e 7420 6973 2064 6566 696e 6564  ement is defined
+00008d10: 2e20 452e 672e 2c20 6022 7465 7374 5f77  . E.g., `"test_w
+00008d20: 6f72 6b72 6571 2e6a 736f 6e22 602e 2020  orkreq.json"`.  
 00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d60: 7c20 5965 7320 207c 2020 2020 207c 2020  | Yes  |     |  
-00008d70: 2020 2020 7c20 2020 2020 207c 0a0a 2323      |      |..##
-00008d80: 2041 7574 6f6d 6174 6963 2050 726f 7065   Automatic Prope
-00008d90: 7274 6965 730a 0a49 6e20 6164 6469 7469  rties..In additi
-00008da0: 6f6e 2074 6f20 7468 6520 696e 6865 7269  on to the inheri
-00008db0: 7461 6e63 6520 6d65 6368 616e 6973 6d2c  tance mechanism,
-00008dc0: 2073 6f6d 6520 7072 6f70 6572 7469 6573   some properties
-00008dd0: 2061 7265 2073 6574 2061 7574 6f6d 6174   are set automat
-00008de0: 6963 616c 6c79 2062 7920 7468 6520 6079  ically by the `y
-00008df0: 642d 7375 626d 6974 6020 636f 6d6d 616e  d-submit` comman
-00008e00: 642c 2061 7320 6120 7573 6167 6520 636f  d, as a usage co
-00008e10: 6e76 656e 6965 6e63 6520 6966 2074 6865  nvenience if the
-00008e20: 7927 7265 206e 6f74 2065 7870 6c69 6369  y're not explici
-00008e30: 746c 7920 7072 6f76 6964 6564 2e0a 0a23  tly provided...#
-00008e40: 2323 2057 6f72 6b20 5265 7175 6972 656d  ## Work Requirem
-00008e50: 656e 742c 2054 6173 6b20 4772 6f75 7020  ent, Task Group 
-00008e60: 616e 6420 5461 736b 204e 616d 696e 670a  and Task Naming.
-00008e70: 0a2d 2054 6865 202a 2a57 6f72 6b20 5265  .- The **Work Re
-00008e80: 7175 6972 656d 656e 742a 2a20 6e61 6d65  quirement** name
-00008e90: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
-00008ea0: 7920 7365 7420 7573 696e 6720 6120 636f  y set using a co
-00008eb0: 6e63 6174 656e 6174 696f 6e20 6f66 2074  ncatenation of t
-00008ec0: 6865 2060 7461 6760 2070 726f 7065 7274  he `tag` propert
-00008ed0: 792c 2061 2055 5443 2074 696d 6573 7461  y, a UTC timesta
-00008ee0: 6d70 2c20 616e 6420 7468 7265 6520 7261  mp, and three ra
-00008ef0: 6e64 6f6d 2068 6578 2063 6861 7261 6374  ndom hex charact
-00008f00: 6572 733a 2065 2c67 2c2e 2060 6d79 7461  ers: e,g,. `myta
-00008f10: 675f 3232 3130 3234 2d31 3535 3532 342d  g_221024-155524-
-00008f20: 3430 6160 2e0a 2d20 2a2a 5461 736b 2047  40a`..- **Task G
-00008f30: 726f 7570 2a2a 206e 616d 6573 2061 7265  roup** names are
-00008f40: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
-00008f50: 7265 6174 6564 2066 6f72 2061 6e79 2054  reated for any T
-00008f60: 6173 6b20 4772 6f75 7020 7468 6174 2069  ask Group that i
-00008f70: 7320 6e6f 7420 6578 706c 6963 6974 6c79  s not explicitly
-00008f80: 206e 616d 6564 2c20 7573 696e 6720 6e61   named, using na
-00008f90: 6d65 7320 6f66 2074 6865 2066 6f72 6d20  mes of the form 
-00008fa0: 6074 6173 6b5f 6772 6f75 705f 3160 2028  `task_group_1` (
-00008fb0: 6f72 2060 7461 736b 5f67 726f 7570 5f30  or `task_group_0
-00008fc0: 3160 2c20 6574 632e 2c20 666f 7220 6c61  1`, etc., for la
-00008fd0: 7267 6572 206e 756d 6265 7273 206f 6620  rger numbers of 
-00008fe0: 5461 736b 2047 726f 7570 7329 2e20 5461  Task Groups). Ta
-00008ff0: 736b 2047 726f 7570 206e 756d 6265 7273  sk Group numbers
-00009000: 2063 616e 2061 6c73 6f20 6265 2069 6e63   can also be inc
-00009010: 6c75 6465 6420 696e 2075 7365 722d 6465  luded in user-de
-00009020: 6669 6e65 6420 5461 736b 2047 726f 7570  fined Task Group
-00009030: 206e 616d 6573 2075 7369 6e67 2074 6865   names using the
-00009040: 2060 7b7b 7461 736b 5f67 726f 7570 5f6e   `{{task_group_n
-00009050: 756d 6265 727d 7d60 2076 6172 6961 626c  umber}}` variabl
-00009060: 6520 7375 6273 7469 7475 7469 6f6e 2064  e substitution d
-00009070: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
-00009080: 2d20 2a2a 5461 736b 2a2a 206e 616d 6573  - **Task** names
-00009090: 2061 7265 2061 7574 6f6d 6174 6963 616c   are automatical
-000090a0: 6c79 2063 7265 6174 6564 2066 6f72 2061  ly created for a
-000090b0: 6e79 2054 6173 6b20 7468 6174 2069 7320  ny Task that is 
-000090c0: 6e6f 7420 6578 706c 6963 6974 6c79 206e  not explicitly n
-000090d0: 616d 6564 2c20 7573 696e 6720 6e61 6d65  amed, using name
-000090e0: 7320 6f66 2074 6865 2066 6f72 6d20 6074  s of the form `t
-000090f0: 6173 6b5f 3160 2028 6f72 2060 7461 736b  ask_1` (or `task
-00009100: 5f30 3160 2c20 6574 632e 2c20 666f 7220  _01`, etc., for 
-00009110: 6c61 7267 6572 206e 756d 6265 7273 206f  larger numbers o
-00009120: 6620 5461 736b 7329 2e20 5468 6520 5461  f Tasks). The Ta
-00009130: 736b 2063 6f75 6e74 6572 2072 6573 6574  sk counter reset
-00009140: 7320 666f 7220 6561 6368 2064 6966 6665  s for each diffe
-00009150: 7265 6e74 2054 6173 6b20 4772 6f75 702e  rent Task Group.
-00009160: 2054 6173 6b20 6e75 6d62 6572 7320 6361   Task numbers ca
-00009170: 6e20 616c 736f 2062 6520 696e 636c 7564  n also be includ
-00009180: 6564 2069 6e20 7573 6572 2d64 6566 696e  ed in user-defin
-00009190: 6564 2054 6173 6b20 6e61 6d65 7320 7573  ed Task names us
-000091a0: 696e 6720 7468 6520 607b 7b74 6173 6b5f  ing the `{{task_
-000091b0: 6e75 6d62 6572 7d7d 6020 7661 7269 6162  number}}` variab
-000091c0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
-000091d0: 6469 7363 7573 7365 6420 6265 6c6f 772e  discussed below.
-000091e0: 0a0a 2323 2320 5461 736b 2054 7970 6573  ..### Task Types
-000091f0: 0a0a 2d20 4966 2060 7461 736b 5479 7065  ..- If `taskType
-00009200: 6020 6973 2073 6574 206f 6e6c 7920 6174  ` is set only at
-00009210: 2074 6865 2054 4f4d 4c20 6669 6c65 206c   the TOML file l
-00009220: 6576 656c 2c20 7468 656e 2060 7461 736b  evel, then `task
-00009230: 5479 7065 7360 2069 7320 6175 746f 6d61  Types` is automa
-00009240: 7469 6361 6c6c 7920 706f 7075 6c61 7465  tically populate
-00009250: 6420 666f 7220 5461 736b 2047 726f 7570  d for Task Group
-00009260: 732c 2075 6e6c 6573 7320 6f76 6572 7269  s, unless overri
-00009270: 6464 656e 2e0a 2d20 4966 2060 7461 736b  dden..- If `task
-00009280: 5479 7065 6020 6973 2073 6574 2061 7420  Type` is set at 
-00009290: 7468 6520 5461 736b 206c 6576 656c 2c20  the Task level, 
-000092a0: 7468 656e 2060 7461 736b 5479 7065 7360  then `taskTypes`
-000092b0: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
-000092c0: 7920 706f 7075 6c61 7465 6420 666f 7220  y populated for 
-000092d0: 7468 6520 5461 736b 2047 726f 7570 7320  the Task Groups 
-000092e0: 6c65 7665 6c20 7573 696e 6720 7468 6520  level using the 
-000092f0: 6163 6375 6d75 6c61 7465 6420 5461 736b  accumulated Task
-00009300: 2054 7970 6573 2066 726f 6d20 7468 6520   Types from the 
-00009310: 5461 736b 7320 696e 636c 7564 6564 2069  Tasks included i
-00009320: 6e20 6561 6368 2054 6173 6b20 4772 6f75  n each Task Grou
-00009330: 702c 2075 6e6c 6573 7320 6f76 6572 7269  p, unless overri
-00009340: 6464 656e 2e0a 2d20 4966 2060 7461 736b  dden..- If `task
-00009350: 5479 7065 7360 2069 7320 7365 7420 6174  Types` is set at
-00009360: 2074 6865 2054 6173 6b20 4772 6f75 7020   the Task Group 
-00009370: 4c65 7665 6c2c 2061 6e64 2068 6173 206f  Level, and has o
-00009380: 6e6c 7920 6f6e 6520 5461 736b 2054 7970  nly one Task Typ
-00009390: 6520 656e 7472 792c 2074 6865 6e20 6074  e entry, then `t
-000093a0: 6173 6b54 7970 6560 2069 7320 6175 746f  askType` is auto
-000093b0: 6d61 7469 6361 6c6c 7920 7365 7420 6174  matically set at
-000093c0: 2074 6865 2054 6173 6b20 4c65 7665 6c20   the Task Level 
-000093d0: 7573 696e 6720 7468 6520 7369 6e67 6c65  using the single
-000093e0: 2054 6173 6b20 5479 7065 2c20 756e 6c65   Task Type, unle
-000093f0: 7373 206f 7665 7272 6964 6465 6e2e 0a0a  ss overridden...
-00009400: 466f 7220 7468 6520 2a2a 6062 6173 6860  For the **`bash`
-00009410: 2a2a 2c20 2a2a 6070 6f77 6572 7368 656c  **, **`powershel
-00009420: 6c60 2a2a 2c20 2a2a 6063 6d64 602a 2a2f  l`**, **`cmd`**/
-00009430: 2a2a 6062 6174 602a 2a20 616e 6420 2a2a  **`bat`** and **
-00009440: 6064 6f63 6b65 7260 2a2a 2074 6173 6b20  `docker`** task 
-00009450: 7479 7065 732c 2073 6f6d 6520 6175 746f  types, some auto
-00009460: 6d61 7469 6320 7072 6f63 6573 7369 6e67  matic processing
-00009470: 2077 696c 6c20 6265 2070 6572 666f 726d   will be perform
-00009480: 6564 2069 6620 7468 6520 2a2a 6065 7865  ed if the **`exe
-00009490: 6375 7461 626c 6560 2a2a 2070 726f 7065  cutable`** prope
-000094a0: 7274 7920 6973 2073 6574 2e0a 0a23 2323  rty is set...###
-000094b0: 2320 4261 7368 2c20 5079 7468 6f6e 2c20  # Bash, Python, 
-000094c0: 506f 7765 7253 6865 6c6c 2061 6e64 2063  PowerShell and c
-000094d0: 6d64 2f62 6174 2054 6173 6b73 0a0a 4173  md/bat Tasks..As
-000094e0: 2061 2063 6f6e 7665 6e69 656e 6365 2c20   a convenience, 
-000094f0: 666f 7220 7468 6520 2a2a 6062 6173 6860  for the **`bash`
-00009500: 2a2a 2c20 2a2a 6070 7974 686f 6e60 2a2a  **, **`python`**
-00009510: 2c20 2a2a 6070 6f77 6572 7368 656c 6c60  , **`powershell`
-00009520: 2a2a 2c20 616e 6420 2a2a 6063 6d64 602a  **, and **`cmd`*
-00009530: 2a20 286f 7220 2a2a 6062 6174 602a 2a29  * (or **`bat`**)
-00009540: 2054 6173 6b20 5479 7065 732c 2074 6865   Task Types, the
-00009550: 2073 6372 6970 7420 6e6f 6d69 6e61 7465   script nominate
-00009560: 6420 696e 2074 6865 202a 2a60 6578 6563  d in the **`exec
-00009570: 7574 6162 6c65 602a 2a20 7072 6f70 6572  utable`** proper
-00009580: 7479 2069 7320 6175 746f 6d61 7469 6361  ty is automatica
-00009590: 6c6c 7920 6164 6465 6420 746f 2074 6865  lly added to the
-000095a0: 2060 696e 7075 7473 6020 6c69 7374 2028   `inputs` list (
-000095b0: 6966 206e 6f74 2061 6c72 6561 6479 2070  if not already p
-000095c0: 7265 7365 6e74 292e 2054 6869 7320 6d65  resent). This me
-000095d0: 616e 7320 7468 6520 7363 7269 7074 2066  ans the script f
-000095e0: 696c 6520 7769 6c6c 2062 6520 7570 6c6f  ile will be uplo
-000095f0: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
-00009600: 6374 2053 746f 7265 2c20 616e 6420 6d61  ct Store, and ma
-00009610: 6465 2061 2072 6571 7569 7265 6d65 6e74  de a requirement
-00009620: 206f 6620 7468 6520 5461 736b 2077 6865   of the Task whe
-00009630: 6e20 6974 2072 756e 732e 0a0a 5573 696e  n it runs...Usin
-00009640: 6720 6120 4261 7368 2054 6173 6b20 6173  g a Bash Task as
-00009650: 2061 6e20 6578 616d 706c 6520 2869 6e20   an example (in 
-00009660: 544f 4d4c 2066 6f72 6d29 3a0a 0a60 6060  TOML form):..```
-00009670: 746f 6d6c 0a74 6173 6b54 7970 6520 3d20  toml.taskType = 
-00009680: 2262 6173 6822 0a65 7865 6375 7461 626c  "bash".executabl
-00009690: 6520 3d20 226d 795f 6261 7368 5f73 6372  e = "my_bash_scr
-000096a0: 6970 742e 7368 220a 6172 6775 6d65 6e74  ipt.sh".argument
-000096b0: 7320 3d20 5b22 3122 2c20 2232 222c 2022  s = ["1", "2", "
-000096c0: 3322 5d0a 6060 600a 6973 2065 7175 6976  3"].```.is equiv
-000096d0: 616c 656e 7420 746f 3a0a 0a60 6060 746f  alent to:..```to
-000096e0: 6d6c 0a74 6173 6b54 7970 6520 3d20 2262  ml.taskType = "b
-000096f0: 6173 6822 0a69 6e70 7574 7320 3d20 5b22  ash".inputs = ["
-00009700: 6d79 5f62 6173 685f 7363 7269 7074 2e73  my_bash_script.s
-00009710: 6822 5d0a 6172 6775 6d65 6e74 7320 3d20  h"].arguments = 
-00009720: 5b22 7b7b 7772 5f6e 616d 657d 7d2f 6d79  ["{{wr_name}}/my
-00009730: 5f62 6173 685f 7363 7269 7074 2e73 6822  _bash_script.sh"
-00009740: 2c20 2231 222c 2022 3222 2c20 2233 225d  , "1", "2", "3"]
-00009750: 0a60 6060 0a0a 496e 2074 6865 2063 6173  .```..In the cas
-00009760: 6520 6f66 2057 696e 646f 7773 2062 6174  e of Windows bat
-00009770: 6368 2028 602e 6261 7460 2920 6669 6c65  ch (`.bat`) file
-00009780: 732c 2061 2060 2f63 6020 666c 6167 2069  s, a `/c` flag i
-00009790: 7320 7072 6570 656e 6465 6420 746f 2074  s prepended to t
-000097a0: 6865 2060 636d 642e 6578 6560 2061 7267  he `cmd.exe` arg
-000097b0: 756d 656e 7420 6c69 7374 2074 6f20 656e  ument list to en
-000097c0: 7375 7265 2063 6f72 7265 6374 2065 7865  sure correct exe
-000097d0: 6375 7469 6f6e 2062 6168 6176 696f 7572  cution bahaviour
-000097e0: 2e20 466f 7220 6578 616d 706c 653a 0a0a  . For example:..
-000097f0: 6060 6074 6f6d 6c0a 7461 736b 5479 7065  ```toml.taskType
-00009800: 203d 2022 636d 6422 2020 2320 6f72 2022   = "cmd"  # or "
-00009810: 6261 7422 0a65 7865 6375 7461 626c 6520  bat".executable 
-00009820: 3d20 226d 795f 7363 7269 7074 2e62 6174  = "my_script.bat
-00009830: 220a 6172 6775 6d65 6e74 7320 3d20 5b22  ".arguments = ["
-00009840: 3122 2c20 2232 222c 2022 3322 5d0a 6060  1", "2", "3"].``
-00009850: 600a 0a69 7320 6571 7569 7661 6c65 6e74  `..is equivalent
-00009860: 2074 6f3a 0a0a 6060 6074 6f6d 6c0a 7461   to:..```toml.ta
-00009870: 736b 5479 7065 203d 2022 636d 6422 2020  skType = "cmd"  
-00009880: 2320 6f72 2022 6261 7422 0a69 6e70 7574  # or "bat".input
-00009890: 7320 3d20 5b22 6d79 5f73 6372 6970 742e  s = ["my_script.
-000098a0: 6261 7422 5d0a 6172 6775 6d65 6e74 7320  bat"].arguments 
-000098b0: 3d20 5b22 2f63 222c 2022 7b7b 7772 5f6e  = ["/c", "{{wr_n
-000098c0: 616d 657d 7d5c 5c6d 795f 7363 7269 7074  ame}}\\my_script
-000098d0: 2e62 6174 222c 2022 3122 2c20 2232 222c  .bat", "1", "2",
-000098e0: 2022 3322 5d0a 6060 600a 0a4e 6f74 6520   "3"].```..Note 
-000098f0: 7468 6520 605c 5c60 2072 6571 7569 7265  the `\\` require
-00009900: 6d65 6e74 2066 6f72 2064 6972 6563 746f  ment for directo
-00009910: 7279 2073 6570 6172 6174 6f72 7320 7768  ry separators wh
-00009920: 656e 2064 6566 696e 696e 6720 5461 736b  en defining Task
-00009930: 7320 6f6e 2057 696e 646f 7773 2068 6f73  s on Windows hos
-00009940: 7473 2e20 4e6f 7465 2061 6c73 6f20 7468  ts. Note also th
-00009950: 6174 2074 6865 2060 2f63 6020 6973 2072  at the `/c` is r
-00009960: 6571 7569 7265 6420 7768 656e 2072 756e  equired when run
-00009970: 6e69 6e67 2063 6f6d 6d61 6e64 7320 6f72  ning commands or
-00009980: 2062 6174 6368 2073 6372 6970 7473 2075   batch scripts u
-00009990: 7369 6e67 2060 636d 642e 6578 6560 2c20  sing `cmd.exe`, 
-000099a0: 6f74 6865 7277 6973 6520 7468 6520 6063  otherwise the `c
-000099b0: 6d64 2e65 7865 6020 7072 6f63 6573 7320  md.exe` process 
-000099c0: 6372 6561 7465 6420 746f 2065 7865 6375  created to execu
-000099d0: 7465 2074 6865 2054 6173 6b20 7769 6c6c  te the Task will
-000099e0: 206e 6f74 2074 6572 6d69 6e61 7465 2e0a   not terminate..
-000099f0: 0a23 2323 2320 446f 636b 6572 2054 6173  .#### Docker Tas
-00009a00: 6b73 0a0a 466f 7220 7468 6520 2a2a 6064  ks..For the **`d
-00009a10: 6f63 6b65 7260 2a2a 2054 6173 6b20 5479  ocker`** Task Ty
-00009a20: 7065 2c20 7468 6520 7661 7269 6162 6c65  pe, the variable
-00009a30: 7320 7375 7070 6c69 6564 2069 6e20 7468  s supplied in th
-00009a40: 6520 6064 6f63 6b65 7245 6e76 6972 6f6e  e `dockerEnviron
-00009a50: 6d65 6e74 6020 7072 6f70 6572 7479 2061  ment` property a
-00009a60: 7265 2075 6e70 6163 6b65 6420 696e 746f  re unpacked into
-00009a70: 2074 6865 2061 7267 756d 656e 7420 6c69   the argument li
-00009a80: 7374 2061 7320 602d 2d65 6e76 6020 656e  st as `--env` en
-00009a90: 7472 6965 732c 2074 6865 2044 6f63 6b65  tries, the Docke
-00009aa0: 7220 636f 6e74 6169 6e65 7220 6e61 6d65  r container name
-00009ab0: 2073 7570 706c 6965 6420 696e 2074 6865   supplied in the
-00009ac0: 2060 6578 6563 7574 6162 6c65 6020 7072   `executable` pr
-00009ad0: 6f70 6572 7479 2069 7320 7468 656e 2061  operty is then a
-00009ae0: 6464 6564 2074 6f20 7468 6520 6172 6775  dded to the argu
-00009af0: 6d65 6e74 7320 6c69 7374 2c20 666f 6c6c  ments list, foll
-00009b00: 6f77 6564 2062 7920 7468 6520 6172 6775  owed by the argu
-00009b10: 6d65 6e74 7320 7375 7070 6c69 6564 2069  ments supplied i
-00009b20: 6e20 7468 6520 6061 7267 756d 656e 7473  n the `arguments
-00009b30: 6020 7072 6f70 6572 7479 2e20 5468 6520  ` property. The 
-00009b40: 6064 6f63 6b65 7255 7365 726e 616d 6560  `dockerUsername`
-00009b50: 2061 6e64 2060 646f 636b 6572 5061 7373   and `dockerPass
-00009b60: 776f 7264 6020 7072 6f70 6572 7469 6573  word` properties
-00009b70: 2c20 6966 2073 7570 706c 6965 642c 2061  , if supplied, a
-00009b80: 7265 2061 6464 6564 2074 6f20 7468 6520  re added to the 
-00009b90: 6065 6e76 6972 6f6e 6d65 6e74 6020 7072  `environment` pr
-00009ba0: 6f70 6572 7479 2e0a 0a46 6f72 2065 7861  operty...For exa
-00009bb0: 6d70 6c65 3a0a 6060 6074 6f6d 6c0a 7461  mple:.```toml.ta
-00009bc0: 736b 5479 7065 203d 2022 646f 636b 6572  skType = "docker
-00009bd0: 220a 6578 6563 7574 6162 6c65 203d 2022  ".executable = "
-00009be0: 6d79 5f64 6f63 6b65 7268 7562 5f72 6570  my_dockerhub_rep
-00009bf0: 6f2f 6d79 5f63 6f6e 7461 696e 6572 5f69  o/my_container_i
-00009c00: 6d61 6765 220a 646f 636b 6572 456e 7669  mage".dockerEnvi
-00009c10: 726f 6e6d 656e 7420 3d20 7b45 3120 3d20  ronment = {E1 = 
-00009c20: 2245 6565 4f6e 6522 7d0a 646f 636b 6572  "EeeOne"}.docker
-00009c30: 5573 6572 6e61 6d65 203d 2022 6d79 5f75  Username = "my_u
-00009c40: 7365 7222 0a64 6f63 6b65 7250 6173 7377  ser".dockerPassw
-00009c50: 6f72 6420 3d20 226d 795f 7061 7373 776f  ord = "my_passwo
-00009c60: 7264 220a 6172 6775 6d65 6e74 7320 3d20  rd".arguments = 
-00009c70: 5b22 3122 2c20 2232 222c 2022 3322 5d0a  ["1", "2", "3"].
-00009c80: 6060 600a 0a69 7320 6571 7569 7661 6c65  ```..is equivale
-00009c90: 6e74 2074 6f20 7468 6520 666f 6c6c 6f77  nt to the follow
-00009ca0: 696e 6720 6265 696e 6720 7365 6e74 2066  ing being sent f
-00009cb0: 6f72 2070 726f 6365 7373 696e 6720 6279  or processing by
-00009cc0: 2074 6865 2060 646f 636b 6572 6020 5461   the `docker` Ta
-00009cd0: 736b 2054 7970 652c 2074 6865 2059 656c  sk Type, the Yel
-00009ce0: 6c6f 7744 6f67 2076 6572 7369 6f6e 206f  lowDog version o
-00009cf0: 6620 7768 6963 6820 7769 6c6c 206c 6f67  f which will log
-00009d00: 2069 6e20 746f 2074 6865 2044 6f63 6b65   in to the Docke
-00009d10: 7220 7265 706f 2028 6966 2072 6571 7569  r repo (if requi
-00009d20: 7265 6429 2074 6865 6e20 6973 7375 6520  red) then issue 
-00009d30: 6120 6064 6f63 6b65 7220 7275 6e60 2063  a `docker run` c
-00009d40: 6f6d 6d61 6e64 2077 6974 6820 7468 6520  ommand with the 
-00009d50: 6172 6775 6d65 6e74 7320 7375 7070 6c69  arguments suppli
-00009d60: 6564 3a0a 0a60 6060 746f 6d6c 0a74 6173  ed:..```toml.tas
-00009d70: 6b54 7970 6520 3d20 2264 6f63 6b65 7222  kType = "docker"
-00009d80: 0a61 7267 756d 656e 7473 203d 205b 222d  .arguments = ["-
-00009d90: 2d65 6e76 2045 313d 4565 654f 6e65 222c  -env E1=EeeOne",
-00009da0: 2022 6d79 5f64 6f63 6b65 7268 7562 7265   "my_dockerhubre
-00009db0: 706f 2f6d 795f 636f 6e74 6169 6e65 725f  po/my_container_
-00009dc0: 696d 6167 6522 2c20 2231 222c 2022 3222  image", "1", "2"
-00009dd0: 2c20 2233 225d 0a65 6e76 6972 6f6e 6d65  , "3"].environme
-00009de0: 6e74 203d 207b 444f 434b 4552 5f55 5345  nt = {DOCKER_USE
-00009df0: 524e 414d 4520 3d20 226d 795f 7573 6572  RNAME = "my_user
-00009e00: 222c 2044 4f43 4b45 525f 5041 5353 574f  ", DOCKER_PASSWO
-00009e10: 5244 203d 2022 6d79 5f70 6173 7377 6f72  RD = "my_passwor
-00009e20: 6422 7d0a 6060 600a 0a23 2323 2320 4261  d"}.```..#### Ba
-00009e30: 7368 2c20 5079 7468 6f6e 2c20 506f 7765  sh, Python, Powe
-00009e40: 7253 6865 6c6c 2c20 636d 642e 6578 652f  rShell, cmd.exe/
-00009e50: 6261 7463 682c 2061 6e64 2044 6f63 6b65  batch, and Docke
-00009e60: 7220 7769 7468 6f75 7420 4175 746f 6d61  r without Automa
-00009e70: 7469 6320 5072 6f63 6573 7369 6e67 0a0a  tic Processing..
-00009e80: 4966 2074 6865 2060 6578 6563 7574 6162  If the `executab
-00009e90: 6c65 6020 7072 6f70 6572 7479 2069 7320  le` property is 
-00009ea0: 6e6f 7420 7375 7070 6c69 6564 2c20 7468  not supplied, th
-00009eb0: 6520 6175 746f 6d61 7469 6320 7072 6f63  e automatic proc
-00009ec0: 6573 7369 6e67 2064 6573 6372 6962 6564  essing described
-00009ed0: 2061 626f 7665 2066 6f72 2060 6261 7368   above for `bash
-00009ee0: 602c 2060 7079 7468 6f6e 602c 2060 706f  `, `python`, `po
-00009ef0: 7765 7273 6865 6c6c 602c 2060 636d 6460  wershell`, `cmd`
-00009f00: 2028 6f72 2060 6261 7460 2920 616e 6420   (or `bat`) and 
-00009f10: 6064 6f63 6b65 7260 2074 6173 6b20 7479  `docker` task ty
-00009f20: 7065 7320 6973 206e 6f74 2061 7070 6c69  pes is not appli
-00009f30: 6564 2e0a 0a23 2323 2054 6173 6b20 436f  ed...### Task Co
-00009f40: 756e 7473 0a0a 5468 6973 2070 726f 7065  unts..This prope
-00009f50: 7274 7920 7769 6c6c 2065 7870 616e 6420  rty will expand 
-00009f60: 7468 6520 6e75 6d62 6572 206f 6620 5461  the number of Ta
-00009f70: 736b 7320 746f 206d 6174 6368 2060 7461  sks to match `ta
-00009f80: 736b 436f 756e 7460 2e0a 0a54 6865 2060  skCount`...The `
-00009f90: 7461 736b 436f 756e 7460 2070 726f 7065  taskCount` prope
-00009fa0: 7274 7920 6361 6e20 6265 2073 6574 206f  rty can be set o
-00009fb0: 6e6c 7920 696e 2074 6865 2060 776f 726b  nly in the `work
-00009fc0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
-00009fd0: 7469 6f6e 206f 6620 7468 6520 6063 6f6e  tion of the `con
-00009fe0: 6669 672e 746f 6d6c 6020 6669 6c65 2c20  fig.toml` file, 
-00009ff0: 6f72 2069 6e20 7468 6520 6074 6173 6b47  or in the `taskG
-0000a000: 726f 7570 6020 7365 6374 696f 6e28 7329  roup` section(s)
-0000a010: 206f 6620 6120 4a53 4f4e 2057 6f72 6b20   of a JSON Work 
-0000a020: 5265 7175 6972 656d 656e 7420 6465 6669  Requirement defi
-0000a030: 6e69 7469 6f6e 2e0a 0a49 6e20 7468 6520  nition...In the 
-0000a040: 666f 726d 6572 2063 6173 652c 2074 6865  former case, the
-0000a050: 2060 7461 736b 436f 756e 7460 2061 7070   `taskCount` app
-0000a060: 6c69 6573 206f 6e6c 7920 746f 2074 6865  lies only to the
-0000a070: 2054 6173 6b20 7370 6563 6966 6965 6420   Task specified 
-0000a080: 7769 7468 696e 2074 6865 2060 636f 6e66  within the `conf
-0000a090: 6967 2e74 6f6d 6c60 2066 696c 6520 616e  ig.toml` file an
-0000a0a0: 6420 6973 206e 6f74 2069 6e68 6572 6974  d is not inherit
-0000a0b0: 6564 2062 7920 4a53 4f4e 2057 6f72 6b20  ed by JSON Work 
-0000a0c0: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
-0000a0d0: 6966 6963 6174 696f 6e73 2e0a 0a49 6e20  ifications...In 
-0000a0e0: 7468 6520 6c61 7474 6572 2063 6173 652c  the latter case,
-0000a0f0: 2074 6865 2060 7461 736b 436f 756e 7460   the `taskCount`
-0000a100: 2061 7070 6c69 6573 2074 6f20 7468 6520   applies to the 
-0000a110: 5461 736b 2073 7065 6369 6669 6564 2077  Task specified w
-0000a120: 6974 6869 6e20 7468 6520 5461 736b 2047  ithin the Task G
-0000a130: 726f 7570 2c20 616e 6420 7468 6572 6520  roup, and there 
-0000a140: 6d75 7374 2062 6520 7a65 726f 206f 7220  must be zero or 
-0000a150: 6f6e 6520 5461 736b 2873 2920 6c69 7374  one Task(s) list
-0000a160: 6564 2077 6974 6869 6e20 7468 6520 6772  ed within the gr
-0000a170: 6f75 7020 6f72 2060 7461 736b 436f 756e  oup or `taskCoun
-0000a180: 7460 2069 7320 6967 6e6f 7265 642e 0a0a  t` is ignored...
-0000a190: 2323 2045 7861 6d70 6c65 730a 0a23 2323  ## Examples..###
-0000a1a0: 2054 4f4d 4c20 5072 6f70 6572 7469 6573   TOML Properties
-0000a1b0: 2069 6e20 7468 6520 6077 6f72 6b52 6571   in the `workReq
-0000a1c0: 7569 7265 6d65 6e74 6020 5365 6374 696f  uirement` Sectio
-0000a1d0: 6e0a 0a48 6572 6527 7320 616e 2065 7861  n..Here's an exa
-0000a1e0: 6d70 6c65 206f 6620 7468 6520 6077 6f72  mple of the `wor
-0000a1f0: 6b52 6571 7569 7265 6d65 6e74 6020 7365  kRequirement` se
-0000a200: 6374 696f 6e20 6f66 2061 2054 4f4d 4c20  ction of a TOML 
-0000a210: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-0000a220: 6c65 2c20 7368 6f77 696e 6720 616c 6c20  le, showing all 
-0000a230: 7468 6520 706f 7373 6962 6c65 2070 726f  the possible pro
-0000a240: 7065 7274 6965 7320 7468 6174 2063 616e  perties that can
-0000a250: 2062 6520 7365 743a 0a0a 6060 6074 6f6d   be set:..```tom
-0000a260: 6c0a 5b77 6f72 6b52 6571 7569 7265 6d65  l.[workRequireme
-0000a270: 6e74 5d0a 2020 2020 6172 6775 6d65 6e74  nt].    argument
-0000a280: 7320 3d20 5b22 3122 2c20 2254 574f 225d  s = ["1", "TWO"]
-0000a290: 0a20 2020 2063 6170 7475 7265 5461 736b  .    captureTask
-0000a2a0: 4f75 7470 7574 203d 2074 7275 650a 2020  Output = true.  
-0000a2b0: 2020 636f 6d70 6c65 7465 6454 6173 6b54    completedTaskT
-0000a2c0: 746c 203d 2031 300a 2020 2020 6373 7646  tl = 10.    csvF
-0000a2d0: 696c 6520 3d20 2266 696c 6531 2e63 7376  ile = "file1.csv
-0000a2e0: 220a 2020 2020 6373 7646 696c 6573 203d  ".    csvFiles =
-0000a2f0: 205b 2266 696c 6531 2e63 7376 222c 2022   ["file1.csv", "
-0000a300: 6669 6c65 332e 6373 763a 3322 5d0a 2020  file3.csv:3"].  
-0000a310: 2020 646f 636b 6572 456e 7669 726f 6e6d    dockerEnvironm
-0000a320: 656e 7420 3d20 7b4d 595f 444f 434b 4552  ent = {MY_DOCKER
-0000a330: 5f56 4152 203d 2031 3030 7d0a 2020 2020  _VAR = 100}.    
-0000a340: 646f 636b 6572 5061 7373 776f 7264 203d  dockerPassword =
-0000a350: 2022 6d79 5061 7373 776f 7264 220a 2020   "myPassword".  
-0000a360: 2020 646f 636b 6572 5573 6572 6e61 6d65    dockerUsername
-0000a370: 203d 2022 6d79 5573 6572 6e61 6d65 220a   = "myUsername".
-0000a380: 2020 2020 656e 7669 726f 6e6d 656e 7420      environment 
-0000a390: 3d20 7b4d 595f 5641 5220 3d20 3130 307d  = {MY_VAR = 100}
-0000a3a0: 0a20 2020 2065 7863 6c75 7369 7665 576f  .    exclusiveWo
-0000a3b0: 726b 6572 7320 3d20 6661 6c73 650a 2020  rkers = false.  
-0000a3c0: 2020 6578 6563 7574 6162 6c65 203d 2022    executable = "
-0000a3d0: 6d79 2d63 6f6e 7461 696e 6572 220a 2020  my-container".  
-0000a3e0: 2020 6669 6e69 7368 4966 416c 6c54 6173    finishIfAllTas
-0000a3f0: 6b73 4669 6e69 7368 6564 203d 2074 7275  ksFinished = tru
-0000a400: 650a 2020 2020 6669 6e69 7368 4966 416e  e.    finishIfAn
-0000a410: 7954 6173 6b46 6169 6c65 6420 3d20 6661  yTaskFailed = fa
-0000a420: 6c73 650a 2020 2020 666c 6174 7465 6e49  lse.    flattenI
-0000a430: 6e70 7574 5061 7468 7320 3d20 6661 6c73  nputPaths = fals
-0000a440: 650a 2020 2020 666c 6174 7465 6e55 706c  e.    flattenUpl
-0000a450: 6f61 6450 6174 6873 203d 2066 616c 7365  oadPaths = false
-0000a460: 0a20 2020 2066 756c 6669 6c4f 6e53 7562  .    fulfilOnSub
-0000a470: 6d69 7420 3d20 6661 6c73 650a 2020 2020  mit = false.    
-0000a480: 696e 7075 7473 203d 205b 0a20 2020 2020  inputs = [.     
-0000a490: 2020 2022 2e2e 2f61 7070 2f6d 6169 6e2e     "../app/main.
-0000a4a0: 7079 222c 0a20 2020 2020 2020 2022 2e2e  py",.        "..
-0000a4b0: 2f61 7070 2f72 6571 7569 7265 6d65 6e74  /app/requirement
-0000a4c0: 732e 7478 7422 0a20 2020 205d 0a20 2020  s.txt".    ].   
-0000a4d0: 2069 6e70 7574 734f 7074 696f 6e61 6c20   inputsOptional 
-0000a4e0: 3d20 5b22 6f70 7469 6f6e 616c 2e74 7874  = ["optional.txt
-0000a4f0: 225d 0a20 2020 2069 6e73 7461 6e63 6554  "].    instanceT
-0000a500: 7970 6573 203d 205b 2274 3361 2e6d 6963  ypes = ["t3a.mic
-0000a510: 726f 222c 2022 7433 2e6d 6963 726f 225d  ro", "t3.micro"]
-0000a520: 0a20 2020 206d 6178 576f 726b 6572 7320  .    maxWorkers 
-0000a530: 3d20 310a 2020 2020 6d61 7869 6d75 6d54  = 1.    maximumT
-0000a540: 6173 6b52 6574 7269 6573 203d 2030 0a20  askRetries = 0. 
-0000a550: 2020 206d 696e 576f 726b 6572 7320 3d20     minWorkers = 
-0000a560: 310a 2020 2020 6e61 6d65 203d 2022 6d79  1.    name = "my
-0000a570: 2d77 6f72 6b2d 7265 7175 6972 656d 656e  -work-requiremen
-0000a580: 7422 0a20 2020 206f 7574 7075 7473 203d  t".    outputs =
-0000a590: 205b 2272 6573 756c 7473 2e74 7874 225d   ["results.txt"]
-0000a5a0: 0a20 2020 206f 7574 7075 7473 5265 7175  .    outputsRequ
-0000a5b0: 6972 6564 203d 205b 2272 6573 756c 7473  ired = ["results
-0000a5c0: 5f72 6571 7569 7265 642e 7478 7422 5d0a  _required.txt"].
-0000a5d0: 2020 2020 7072 696f 7269 7479 203d 2030      priority = 0
-0000a5e0: 2e30 0a20 2020 2070 726f 7669 6465 7273  .0.    providers
-0000a5f0: 203d 205b 2241 5753 225d 0a20 2020 2072   = ["AWS"].    r
-0000a600: 616d 203d 205b 302e 352c 2032 2e30 5d0a  am = [0.5, 2.0].
-0000a610: 2020 2020 7265 6769 6f6e 7320 3d20 5b22      regions = ["
-0000a620: 6575 2d77 6573 742d 3222 5d0a 2020 2020  eu-west-2"].    
-0000a630: 7461 736b 4261 7463 6853 697a 6520 3d20  taskBatchSize = 
-0000a640: 3130 3030 0a20 2020 2074 6173 6b43 6f75  1000.    taskCou
-0000a650: 6e74 203d 2031 3030 0a20 2020 2074 6173  nt = 100.    tas
-0000a660: 6b44 6174 6120 3d20 226d 795f 6461 7461  kData = "my_data
-0000a670: 5f73 7472 696e 6722 0a20 2020 2074 6173  _string".    tas
-0000a680: 6b44 6174 6146 696c 6520 3d20 226d 795f  kDataFile = "my_
-0000a690: 6461 7461 5f66 696c 652e 7478 7422 0a20  data_file.txt". 
-0000a6a0: 2020 2074 6173 6b4e 616d 6520 3d20 226d     taskName = "m
-0000a6b0: 795f 7461 736b 5f6e 756d 6265 725f 7b7b  y_task_number_{{
-0000a6c0: 7461 736b 5f6e 756d 6265 727d 7d22 0a20  task_number}}". 
-0000a6d0: 2020 2074 6173 6b47 726f 7570 4e61 6d65     taskGroupName
-0000a6e0: 203d 2022 6d79 5f74 6173 6b5f 6772 6f75   = "my_task_grou
-0000a6f0: 705f 6e75 6d62 6572 5f7b 7b74 6173 6b5f  p_number_{{task_
-0000a700: 6772 6f75 705f 6e75 6d62 6572 7d7d 220a  group_number}}".
-0000a710: 2020 2020 7461 736b 5479 7065 203d 2022      taskType = "
-0000a720: 646f 636b 6572 220a 2020 2020 7461 736b  docker".    task
-0000a730: 7350 6572 576f 726b 6572 203d 2031 0a20  sPerWorker = 1. 
-0000a740: 2020 2075 706c 6f61 6446 696c 6573 203d     uploadFiles =
-0000a750: 205b 7b6c 6f63 616c 5061 7468 203d 2022   [{localPath = "
-0000a760: 6669 6c65 5f31 2e74 7874 222c 2075 706c  file_1.txt", upl
-0000a770: 6f61 6450 6174 6820 3d20 2266 696c 655f  oadPath = "file_
-0000a780: 312e 7478 7422 7d5d 0a20 2020 2076 6370  1.txt"}].    vcp
-0000a790: 7573 203d 205b 312c 2034 5d0a 2020 2020  us = [1, 4].    
-0000a7a0: 7665 7269 6679 4174 5374 6172 7420 3d20  verifyAtStart = 
-0000a7b0: 5b22 7265 6164 795f 7265 7375 6c74 732e  ["ready_results.
-0000a7c0: 7478 7422 5d0a 2020 2020 7665 7269 6679  txt"].    verify
-0000a7d0: 5761 6974 203d 205b 2277 6169 745f 666f  Wait = ["wait_fo
-0000a7e0: 725f 7265 7375 6c74 732e 7478 7422 5d0a  r_results.txt"].
-0000a7f0: 2020 2020 776f 726b 6572 5461 6773 203d      workerTags =
-0000a800: 205b 2274 6167 2d7b 7b75 7365 726e 616d   ["tag-{{usernam
-0000a810: 657d 7d22 5d0a 2020 2020 776f 726b 5265  e}}"].    workRe
-0000a820: 7175 6972 656d 656e 7444 6174 6120 3d20  quirementData = 
-0000a830: 2277 6f72 6b5f 7265 7175 6972 656d 656e  "work_requiremen
-0000a840: 742e 6a73 6f6e 220a 6060 600a 0a23 2323  t.json".```..###
-0000a850: 204a 534f 4e20 5072 6f70 6572 7469 6573   JSON Properties
-0000a860: 2061 7420 7468 6520 576f 726b 2052 6571   at the Work Req
-0000a870: 7569 7265 6d65 6e74 204c 6576 656c 0a0a  uirement Level..
-0000a880: 5368 6f77 696e 6720 616c 6c20 706f 7373  Showing all poss
-0000a890: 6962 6c65 2070 726f 7065 7274 6965 7320  ible properties 
-0000a8a0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
-0000a8b0: 6972 656d 656e 7420 6c65 7665 6c3a 0a0a  irement level:..
-0000a8c0: 6060 606a 736f 6e0a 7b0a 2020 2261 7267  ```json.{.  "arg
-0000a8d0: 756d 656e 7473 223a 205b 312c 2022 5457  uments": [1, "TW
-0000a8e0: 4f22 5d2c 0a20 2022 6361 7074 7572 6554  O"],.  "captureT
-0000a8f0: 6173 6b4f 7574 7075 7422 3a20 7472 7565  askOutput": true
-0000a900: 2c0a 2020 2263 6f6d 706c 6574 6564 5461  ,.  "completedTa
-0000a910: 736b 5474 6c22 3a20 3130 2c0a 2020 2264  skTtl": 10,.  "d
-0000a920: 6f63 6b65 7245 6e76 6972 6f6e 6d65 6e74  ockerEnvironment
-0000a930: 223a 207b 224d 595f 444f 434b 4552 5f56  ": {"MY_DOCKER_V
-0000a940: 4152 223a 2031 3030 7d2c 0a20 2022 646f  AR": 100},.  "do
-0000a950: 636b 6572 5061 7373 776f 7264 223a 2022  ckerPassword": "
-0000a960: 6d79 5061 7373 776f 7264 222c 0a20 2022  myPassword",.  "
-0000a970: 646f 636b 6572 5573 6572 6e61 6d65 223a  dockerUsername":
-0000a980: 2022 6d79 5573 6572 6e61 6d65 222c 0a20   "myUsername",. 
-0000a990: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-0000a9a0: 7b22 4d59 5f56 4152 223a 2031 3030 7d2c  {"MY_VAR": 100},
-0000a9b0: 0a20 2022 6578 636c 7573 6976 6557 6f72  .  "exclusiveWor
-0000a9c0: 6b65 7273 223a 2066 616c 7365 2c0a 2020  kers": false,.  
-0000a9d0: 2265 7865 6375 7461 626c 6522 3a20 226d  "executable": "m
-0000a9e0: 792d 636f 6e74 6169 6e65 7222 2c0a 2020  y-container",.  
-0000a9f0: 2266 696e 6973 6849 6641 6c6c 5461 736b  "finishIfAllTask
-0000aa00: 7346 696e 6973 6865 6422 3a20 7472 7565  sFinished": true
-0000aa10: 2c0a 2020 2266 696e 6973 6849 6641 6e79  ,.  "finishIfAny
-0000aa20: 5461 736b 4661 696c 6564 223a 2066 616c  TaskFailed": fal
-0000aa30: 7365 2c0a 2020 2266 6c61 7474 656e 496e  se,.  "flattenIn
-0000aa40: 7075 7450 6174 6873 223a 2066 616c 7365  putPaths": false
-0000aa50: 2c0a 2020 2266 6c61 7474 656e 5570 6c6f  ,.  "flattenUplo
-0000aa60: 6164 5061 7468 7322 3a20 6661 6c73 652c  adPaths": false,
-0000aa70: 0a20 2022 6675 6c66 696c 4f6e 5375 626d  .  "fulfilOnSubm
-0000aa80: 6974 223a 2066 616c 7365 2c0a 2020 2269  it": false,.  "i
-0000aa90: 6e70 7574 7322 3a20 5b22 6170 702f 6d61  nputs": ["app/ma
-0000aaa0: 696e 2e70 7922 2c20 2261 7070 2f72 6571  in.py", "app/req
-0000aab0: 7569 7265 6d65 6e74 732e 7478 7422 5d2c  uirements.txt"],
-0000aac0: 0a20 2022 696e 7075 7473 4f70 7469 6f6e  .  "inputsOption
-0000aad0: 616c 223a 205b 226f 7074 696f 6e61 6c2e  al": ["optional.
-0000aae0: 7478 7422 5d2c 0a20 2022 696e 7374 616e  txt"],.  "instan
-0000aaf0: 6365 5479 7065 7322 3a20 5b22 7433 612e  ceTypes": ["t3a.
-0000ab00: 6d69 6372 6f22 2c20 2274 332e 6d69 6372  micro", "t3.micr
-0000ab10: 6f22 5d2c 0a20 2022 6d61 7857 6f72 6b65  o"],.  "maxWorke
-0000ab20: 7273 223a 2031 2c0a 2020 226d 6178 696d  rs": 1,.  "maxim
-0000ab30: 756d 5461 736b 5265 7472 6965 7322 3a20  umTaskRetries": 
-0000ab40: 302c 0a20 2022 6d69 6e57 6f72 6b65 7273  0,.  "minWorkers
-0000ab50: 223a 2031 2c0a 2020 226e 616d 6522 3a20  ": 1,.  "name": 
-0000ab60: 226d 792d 776f 726b 2d72 6571 7569 7265  "my-work-require
-0000ab70: 6d65 6e74 222c 0a20 2022 6f75 7470 7574  ment",.  "output
-0000ab80: 7322 3a20 5b22 7265 7375 6c74 732e 7478  s": ["results.tx
-0000ab90: 7422 5d2c 0a20 2022 6f75 7470 7574 7352  t"],.  "outputsR
-0000aba0: 6571 7569 7265 6422 3a20 5b22 7265 7375  equired": ["resu
-0000abb0: 6c74 735f 7265 7175 6972 6564 2e74 7874  lts_required.txt
-0000abc0: 225d 2c0a 2020 2270 7269 6f72 6974 7922  "],.  "priority"
-0000abd0: 3a20 302e 302c 0a20 2022 7072 6f76 6964  : 0.0,.  "provid
-0000abe0: 6572 7322 3a20 5b22 4157 5322 5d2c 0a20  ers": ["AWS"],. 
-0000abf0: 2022 7261 6d22 3a20 5b30 2e35 2c20 325d   "ram": [0.5, 2]
-0000ac00: 2c0a 2020 2272 6567 696f 6e73 223a 205b  ,.  "regions": [
-0000ac10: 2265 752d 7765 7374 2d32 225d 2c0a 2020  "eu-west-2"],.  
-0000ac20: 2274 6173 6b44 6174 6122 3a20 226d 795f  "taskData": "my_
-0000ac30: 7461 736b 5f64 6174 615f 7374 7269 6e67  task_data_string
-0000ac40: 222c 0a20 2022 7461 736b 4461 7461 4669  ",.  "taskDataFi
-0000ac50: 6c65 223a 2022 6d79 5f64 6174 615f 6669  le": "my_data_fi
-0000ac60: 6c65 2e74 7874 222c 0a20 2022 7461 736b  le.txt",.  "task
-0000ac70: 5479 7065 7322 3a20 5b22 646f 636b 6572  Types": ["docker
-0000ac80: 225d 2c0a 2020 2274 6173 6b73 5065 7257  "],.  "tasksPerW
-0000ac90: 6f72 6b65 7222 3a20 312c 0a20 2022 7570  orker": 1,.  "up
-0000aca0: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
-0000acb0: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
-0000acc0: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
-0000acd0: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
-0000ace0: 7874 227d 5d2c 0a20 2022 7663 7075 7322  xt"}],.  "vcpus"
-0000acf0: 3a20 5b31 2c20 345d 2c0a 2020 2276 6572  : [1, 4],.  "ver
-0000ad00: 6966 7941 7453 7461 7274 223a 205b 2272  ifyAtStart": ["r
-0000ad10: 6561 6479 5f72 6573 756c 7473 2e74 7874  eady_results.txt
-0000ad20: 225d 2c0a 2020 2276 6572 6966 7957 6169  "],.  "verifyWai
-0000ad30: 7422 3a20 5b22 7761 6974 5f66 6f72 5f72  t": ["wait_for_r
-0000ad40: 6573 756c 7473 2e74 7874 225d 2c0a 2020  esults.txt"],.  
-0000ad50: 2277 6f72 6b65 7254 6167 7322 3a20 5b5d  "workerTags": []
-0000ad60: 2c0a 2020 2274 6173 6b47 726f 7570 7322  ,.  "taskGroups"
-0000ad70: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-0000ad80: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
-0000ad90: 2020 207b 7d0a 2020 2020 2020 5d0a 2020     {}.      ].  
-0000ada0: 2020 7d0a 2020 5d0a 7d0a 0a60 6060 0a0a    }.  ].}..```..
-0000adb0: 2323 2320 4a53 4f4e 2050 726f 7065 7274  ### JSON Propert
-0000adc0: 6965 7320 6174 2074 6865 2054 6173 6b20  ies at the Task 
-0000add0: 4772 6f75 7020 4c65 7665 6c0a 0a53 686f  Group Level..Sho
-0000ade0: 7769 6e67 2061 6c6c 2070 6f73 7369 626c  wing all possibl
-0000adf0: 6520 7072 6f70 6572 7469 6573 2061 7420  e properties at 
-0000ae00: 7468 6520 5461 736b 2047 726f 7570 206c  the Task Group l
-0000ae10: 6576 656c 3a0a 0a60 6060 6a73 6f6e 0a7b  evel:..```json.{
-0000ae20: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
-0000ae30: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-0000ae40: 6172 6775 6d65 6e74 7322 3a20 5b31 2c20  arguments": [1, 
-0000ae50: 2254 574f 225d 2c0a 2020 2020 2020 2263  "TWO"],.      "c
-0000ae60: 6170 7475 7265 5461 736b 4f75 7470 7574  aptureTaskOutput
-0000ae70: 223a 2074 7275 652c 0a20 2020 2020 2022  ": true,.      "
-0000ae80: 636f 6d70 6c65 7465 6454 6173 6b54 746c  completedTaskTtl
-0000ae90: 223a 2031 302c 0a20 2020 2020 2022 646f  ": 10,.      "do
-0000aea0: 636b 6572 456e 7669 726f 6e6d 656e 7422  ckerEnvironment"
-0000aeb0: 3a20 7b22 4d59 5f44 4f43 4b45 525f 5641  : {"MY_DOCKER_VA
-0000aec0: 5222 3a20 3130 307d 2c0a 2020 2020 2020  R": 100},.      
-0000aed0: 2264 6f63 6b65 7250 6173 7377 6f72 6422  "dockerPassword"
-0000aee0: 3a20 226d 7950 6173 7377 6f72 6422 2c0a  : "myPassword",.
-0000aef0: 2020 2020 2020 2264 6f63 6b65 7255 7365        "dockerUse
-0000af00: 726e 616d 6522 3a20 226d 7955 7365 726e  rname": "myUsern
-0000af10: 616d 6522 2c0a 2020 2020 2020 2265 6e76  ame",.      "env
-0000af20: 6972 6f6e 6d65 6e74 223a 207b 224d 595f  ironment": {"MY_
-0000af30: 5641 5222 3a20 3130 307d 2c0a 2020 2020  VAR": 100},.    
-0000af40: 2020 2265 7863 6c75 7369 7665 576f 726b    "exclusiveWork
-0000af50: 6572 7322 3a20 6661 6c73 652c 0a20 2020  ers": false,.   
-0000af60: 2020 2022 6578 6563 7574 6162 6c65 223a     "executable":
-0000af70: 2022 6d79 2d63 6f6e 7461 696e 6572 222c   "my-container",
-0000af80: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
-0000af90: 416c 6c54 6173 6b73 4669 6e69 7368 6564  AllTasksFinished
-0000afa0: 223a 2074 7275 652c 0a20 2020 2020 2022  ": true,.      "
-0000afb0: 6669 6e69 7368 4966 416e 7954 6173 6b46  finishIfAnyTaskF
-0000afc0: 6169 6c65 6422 3a20 6661 6c73 652c 0a20  ailed": false,. 
-0000afd0: 2020 2020 2022 666c 6174 7465 6e49 6e70       "flattenInp
-0000afe0: 7574 5061 7468 7322 3a20 6661 6c73 652c  utPaths": false,
-0000aff0: 0a20 2020 2020 2022 696e 7075 7473 223a  .      "inputs":
-0000b000: 205b 2261 7070 2f6d 6169 6e2e 7079 222c   ["app/main.py",
-0000b010: 2022 6170 702f 7265 7175 6972 656d 656e   "app/requiremen
-0000b020: 7473 2e74 7874 225d 2c0a 2020 2020 2020  ts.txt"],.      
-0000b030: 2269 6e70 7574 734f 7074 696f 6e61 6c22  "inputsOptional"
-0000b040: 3a20 5b22 6f70 7469 6f6e 616c 2e74 7874  : ["optional.txt
-0000b050: 225d 2c0a 2020 2020 2020 2269 6e73 7461  "],.      "insta
-0000b060: 6e63 6554 7970 6573 223a 205b 2274 3361  nceTypes": ["t3a
-0000b070: 2e6d 6963 726f 222c 2022 7433 2e6d 6963  .micro", "t3.mic
-0000b080: 726f 225d 2c0a 2020 2020 2020 226d 6178  ro"],.      "max
-0000b090: 696d 756d 5461 736b 5265 7472 6965 7322  imumTaskRetries"
-0000b0a0: 3a20 302c 0a20 2020 2020 2022 6d61 7857  : 0,.      "maxW
-0000b0b0: 6f72 6b65 7273 223a 2031 2c0a 2020 2020  orkers": 1,.    
-0000b0c0: 2020 226d 696e 576f 726b 6572 7322 3a20    "minWorkers": 
-0000b0d0: 312c 0a20 2020 2020 2022 6e61 6d65 223a  1,.      "name":
-0000b0e0: 2022 6669 7273 742d 7461 736b 2d67 726f   "first-task-gro
-0000b0f0: 7570 222c 0a20 2020 2020 2022 6f75 7470  up",.      "outp
-0000b100: 7574 7322 3a20 5b22 7265 7375 6c74 732e  uts": ["results.
-0000b110: 7478 7422 5d2c 0a20 2020 2020 2022 6f75  txt"],.      "ou
-0000b120: 7470 7574 7352 6571 7569 7265 6422 3a20  tputsRequired": 
-0000b130: 5b22 7265 7375 6c74 735f 7265 7175 6972  ["results_requir
-0000b140: 6564 2e74 7874 225d 2c0a 2020 2020 2020  ed.txt"],.      
-0000b150: 2270 7269 6f72 6974 7922 3a20 302e 302c  "priority": 0.0,
-0000b160: 0a20 2020 2020 2022 7072 6f76 6964 6572  .      "provider
-0000b170: 7322 3a20 5b22 4157 5322 5d2c 0a20 2020  s": ["AWS"],.   
-0000b180: 2020 2022 7261 6d22 3a20 5b30 2e35 2c20     "ram": [0.5, 
-0000b190: 325d 2c0a 2020 2020 2020 2272 6567 696f  2],.      "regio
-0000b1a0: 6e73 223a 205b 2265 752d 7765 7374 2d32  ns": ["eu-west-2
-0000b1b0: 225d 2c0a 2020 2020 2020 2274 6173 6b43  "],.      "taskC
-0000b1c0: 6f75 6e74 223a 2035 2c0a 2020 2020 2020  ount": 5,.      
-0000b1d0: 2274 6173 6b44 6174 6122 3a20 226d 795f  "taskData": "my_
-0000b1e0: 7461 736b 5f64 6174 615f 7374 7269 6e67  task_data_string
-0000b1f0: 222c 0a20 2020 2020 2022 7461 736b 4461  ",.      "taskDa
-0000b200: 7461 4669 6c65 223a 2022 6d79 5f64 6174  taFile": "my_dat
-0000b210: 615f 6669 6c65 2e74 7874 222c 0a20 2020  a_file.txt",.   
-0000b220: 2020 2022 7461 736b 5479 7065 7322 3a20     "taskTypes": 
-0000b230: 5b22 646f 636b 6572 225d 2c0a 2020 2020  ["docker"],.    
-0000b240: 2020 2274 6173 6b73 5065 7257 6f72 6b65    "tasksPerWorke
-0000b250: 7222 3a20 312c 0a20 2020 2020 2022 7570  r": 1,.      "up
-0000b260: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
-0000b270: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
-0000b280: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
-0000b290: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
-0000b2a0: 7874 227d 5d2c 0a20 2020 2020 2022 7663  xt"}],.      "vc
-0000b2b0: 7075 7322 3a20 5b31 2c20 345d 2c0a 2020  pus": [1, 4],.  
-0000b2c0: 2020 2020 2276 6572 6966 7941 7453 7461      "verifyAtSta
-0000b2d0: 7274 223a 205b 2272 6561 6479 5f72 6573  rt": ["ready_res
-0000b2e0: 756c 7473 2e74 7874 225d 2c0a 2020 2020  ults.txt"],.    
-0000b2f0: 2020 2276 6572 6966 7957 6169 7422 3a20    "verifyWait": 
-0000b300: 5b22 7761 6974 5f66 6f72 5f72 6573 756c  ["wait_for_resul
-0000b310: 7473 2e74 7874 225d 2c0a 2020 2020 2020  ts.txt"],.      
-0000b320: 2277 6f72 6b65 7254 6167 7322 3a20 5b5d  "workerTags": []
-0000b330: 2c0a 2020 2020 2020 2274 6173 6b73 223a  ,.      "tasks":
-0000b340: 205b 0a20 2020 2020 2020 207b 7d0a 2020   [.        {}.  
-0000b350: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
-0000b360: 207b 0a20 2020 2020 2022 6e61 6d65 223a   {.      "name":
-0000b370: 2022 7365 636f 6e64 2d74 6173 6b2d 6772   "second-task-gr
-0000b380: 6f75 7022 2c0a 2020 2020 2020 2264 6570  oup",.      "dep
-0000b390: 656e 6465 6e74 4f6e 223a 2022 6669 7273  endentOn": "firs
-0000b3a0: 742d 7461 736b 2d67 726f 7570 222c 0a20  t-task-group",. 
-0000b3b0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
-0000b3c0: 2020 2020 2020 2020 7b7d 0a20 2020 2020          {}.     
-0000b3d0: 205d 0a20 2020 207d 0a20 205d 0a7d 0a60   ].    }.  ].}.`
-0000b3e0: 6060 0a0a 2323 2320 4a53 4f4e 2050 726f  ``..### JSON Pro
-0000b3f0: 7065 7274 6965 7320 6174 2074 6865 2054  perties at the T
-0000b400: 6173 6b20 4c65 7665 6c0a 0a53 686f 7769  ask Level..Showi
-0000b410: 6e67 2061 6c6c 2070 6f73 7369 626c 6520  ng all possible 
-0000b420: 7072 6f70 6572 7469 6573 2061 7420 7468  properties at th
-0000b430: 6520 5461 736b 206c 6576 656c 3a0a 0a60  e Task level:..`
-0000b440: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
-0000b450: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
-0000b460: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-0000b470: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-0000b480: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
-0000b490: 223a 205b 312c 2032 5d2c 0a20 2020 2020  ": [1, 2],.     
-0000b4a0: 2020 2020 2022 6361 7074 7572 6554 6173       "captureTas
-0000b4b0: 6b4f 7574 7075 7422 3a20 7472 7565 2c0a  kOutput": true,.
-0000b4c0: 2020 2020 2020 2020 2020 2264 6f63 6b65            "docke
-0000b4d0: 7245 6e76 6972 6f6e 6d65 6e74 223a 207b  rEnvironment": {
-0000b4e0: 224d 595f 444f 434b 4552 5f56 4152 223a  "MY_DOCKER_VAR":
-0000b4f0: 2031 3030 7d2c 0a20 2020 2020 2020 2020   100},.         
-0000b500: 2022 646f 636b 6572 5061 7373 776f 7264   "dockerPassword
-0000b510: 223a 2022 6d79 5061 7373 776f 7264 222c  ": "myPassword",
-0000b520: 0a20 2020 2020 2020 2020 2022 646f 636b  .          "dock
-0000b530: 6572 5573 6572 6e61 6d65 223a 2022 6d79  erUsername": "my
-0000b540: 5573 6572 6e61 6d65 222c 0a20 2020 2020  Username",.     
-0000b550: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-0000b560: 7422 3a20 7b22 4d59 5f56 4152 223a 2031  t": {"MY_VAR": 1
-0000b570: 3030 7d2c 0a20 2020 2020 2020 2020 2022  00},.          "
-0000b580: 6578 6563 7574 6162 6c65 223a 2022 6d79  executable": "my
-0000b590: 2d63 6f6e 7461 696e 6572 222c 0a20 2020  -container",.   
-0000b5a0: 2020 2020 2020 2022 666c 6174 7465 6e49         "flattenI
-0000b5b0: 6e70 7574 5061 7468 7322 3a20 6661 6c73  nputPaths": fals
-0000b5c0: 652c 0a20 2020 2020 2020 2020 2022 696e  e,.          "in
-0000b5d0: 7075 7473 223a 205b 2261 7070 2f6d 6169  puts": ["app/mai
-0000b5e0: 6e2e 7079 222c 2022 6170 702f 7265 7175  n.py", "app/requ
-0000b5f0: 6972 656d 656e 7473 2e74 7874 225d 2c0a  irements.txt"],.
-0000b600: 2020 2020 2020 2020 2020 2269 6e70 7574            "input
-0000b610: 734f 7074 696f 6e61 6c22 3a20 5b22 6f70  sOptional": ["op
-0000b620: 7469 6f6e 616c 2e74 7874 225d 2c0a 2020  tional.txt"],.  
-0000b630: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-0000b640: 226d 792d 7461 736b 222c 0a20 2020 2020  "my-task",.     
-0000b650: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-0000b660: 5b22 7265 7375 6c74 732e 7478 7422 5d2c  ["results.txt"],
-0000b670: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
-0000b680: 7574 7352 6571 7569 7265 6422 3a20 5b22  utsRequired": ["
-0000b690: 7265 7375 6c74 735f 7265 7175 6972 6564  results_required
-0000b6a0: 2e74 7874 225d 2c0a 2020 2020 2020 2020  .txt"],.        
-0000b6b0: 2020 2274 6173 6b44 6174 6122 3a20 226d    "taskData": "m
-0000b6c0: 795f 7461 736b 5f64 6174 615f 7374 7269  y_task_data_stri
-0000b6d0: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
-0000b6e0: 7461 736b 4461 7461 4669 6c65 223a 2022  taskDataFile": "
-0000b6f0: 6d79 5f64 6174 615f 6669 6c65 2e74 7874  my_data_file.txt
-0000b700: 222c 0a20 2020 2020 2020 2020 2022 7461  ",.          "ta
-0000b710: 736b 5479 7065 223a 2022 646f 636b 6572  skType": "docker
-0000b720: 222c 0a20 2020 2020 2020 2020 2022 7570  ",.          "up
-0000b730: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
-0000b740: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
-0000b750: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
-0000b760: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
-0000b770: 7874 227d 5d2c 0a20 2020 2020 2020 2020  xt"}],.         
-0000b780: 2022 7665 7269 6679 4174 5374 6172 7422   "verifyAtStart"
-0000b790: 3a20 5b22 7265 6164 795f 7265 7375 6c74  : ["ready_result
-0000b7a0: 732e 7478 7422 5d2c 0a20 2020 2020 2020  s.txt"],.       
-0000b7b0: 2020 2022 7665 7269 6679 5761 6974 223a     "verifyWait":
-0000b7c0: 205b 2277 6169 745f 666f 725f 7265 7375   ["wait_for_resu
-0000b7d0: 6c74 732e 7478 7422 5d0a 2020 2020 2020  lts.txt"].      
-0000b7e0: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
-0000b7f0: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2320  }.  ].}.```..## 
-0000b800: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
-0000b810: 7574 696f 6e73 2069 6e20 576f 726b 2052  utions in Work R
-0000b820: 6571 7569 7265 6d65 6e74 2050 726f 7065  equirement Prope
-0000b830: 7274 6965 730a 0a56 6172 6961 626c 6520  rties..Variable 
-0000b840: 7375 6273 7469 7475 7469 6f6e 7320 6361  substitutions ca
-0000b850: 6e20 6265 2075 7365 6420 7769 7468 696e  n be used within
-0000b860: 2061 6e79 2070 726f 7065 7274 7920 7661   any property va
-0000b870: 6c75 6520 696e 2054 4f4d 4c20 636f 6e66  lue in TOML conf
-0000b880: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
-0000b890: 6f72 2057 6f72 6b20 5265 7175 6972 656d  or Work Requirem
-0000b8a0: 656e 7420 4a53 4f4e 2066 696c 6573 2e20  ent JSON files. 
-0000b8b0: 5365 6520 7468 6520 6465 7363 7269 7074  See the descript
-0000b8c0: 696f 6e20 5b61 626f 7665 5d28 2376 6172  ion [above](#var
-0000b8d0: 6961 626c 652d 7375 6273 7469 7475 7469  iable-substituti
-0000b8e0: 6f6e 7329 2066 6f72 206d 6f72 6520 6465  ons) for more de
-0000b8f0: 7461 696c 7320 6f6e 2076 6172 6961 626c  tails on variabl
-0000b900: 6520 7375 6273 7469 7475 7469 6f6e 732e  e substitutions.
-0000b910: 2054 6869 7320 6973 2061 2070 6f77 6572   This is a power
-0000b920: 6675 6c20 6665 6174 7572 6520 7468 6174  ful feature that
-0000b930: 2061 6c6c 6f77 7320 576f 726b 2052 6571   allows Work Req
-0000b940: 7569 7265 6d65 6e74 7320 746f 2062 6520  uirements to be 
-0000b950: 7061 7261 6d65 7465 7269 7365 6420 6279  parameterised by
-0000b960: 2073 7570 706c 7969 6e67 2076 616c 7565   supplying value
-0000b970: 7320 6f6e 2074 6865 2063 6f6d 6d61 6e64  s on the command
-0000b980: 206c 696e 652c 2076 6961 2065 6e76 6972   line, via envir
-0000b990: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-0000b9a0: 206f 7220 7669 6120 7468 6520 544f 4d4c   or via the TOML
-0000b9b0: 2066 696c 652e 0a0a 2323 2320 5461 736b   file...### Task
-0000b9c0: 2061 6e64 2054 6173 6b20 4772 6f75 7020   and Task Group 
-0000b9d0: 4e61 6d65 2053 7562 7374 6974 7574 696f  Name Substitutio
-0000b9e0: 6e0a 0a54 6865 2066 6f6c 6c6f 7769 6e67  n..The following
-0000b9f0: 206e 756d 6265 7269 6e67 2061 6e64 206e   numbering and n
-0000ba00: 616d 696e 6720 7375 6273 7469 7475 7469  aming substituti
-0000ba10: 6f6e 7320 6172 6520 6176 6169 6c61 626c  ons are availabl
-0000ba20: 6520 666f 7220 7573 6520 696e 2054 6173  e for use in Tas
-0000ba30: 6b20 616e 6420 5461 736b 2047 726f 7570  k and Task Group
-0000ba40: 206e 616d 696e 672c 206f 6e6c 7920 7768   naming, only wh
-0000ba50: 656e 2074 6865 2057 6f72 6b20 5265 7175  en the Work Requ
-0000ba60: 6972 656d 656e 7420 6973 2073 7065 6369  irement is speci
-0000ba70: 6669 6564 2061 7320 204a 534f 4e20 646f  fied as  JSON do
-0000ba80: 6375 6d65 6e74 2c20 692e 652e 2c20 7468  cument, i.e., th
-0000ba90: 6579 2063 616e 2062 6520 7573 6564 2069  ey can be used i
-0000baa0: 6e20 7468 6520 606e 616d 6560 2070 726f  n the `name` pro
-0000bab0: 7065 7274 6965 7320 666f 7220 5461 736b  perties for Task
-0000bac0: 7320 616e 6420 5461 736b 2047 726f 7570  s and Task Group
-0000bad0: 7320 696e 204a 534f 4e20 7370 6563 6966  s in JSON specif
-0000bae0: 6963 6174 696f 6e73 2e0a 0a54 6865 2066  ications...The f
-0000baf0: 6f6c 6c6f 7769 6e67 2074 6162 6c65 2064  ollowing table d
-0000bb00: 6566 696e 6573 2074 6865 2063 6f6e 7465  efines the conte
-0000bb10: 7874 2873 2920 696e 2077 6869 6368 2065  xt(s) in which e
-0000bb20: 6163 6820 7661 7269 6162 6c65 2063 616e  ach variable can
-0000bb30: 2062 6520 7573 6564 3a0a 0a7c 2044 6972   be used:..| Dir
-0000bb40: 6563 7469 7665 2020 2020 2020 2020 2020  ective          
-0000bb50: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
-0000bb60: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00008d50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00008d60: 2059 6573 2020 7c20 2020 2020 7c20 2020   Yes  |     |   
+00008d70: 2020 207c 2020 2020 2020 7c0a 0a23 2320     |      |..## 
+00008d80: 4175 746f 6d61 7469 6320 5072 6f70 6572  Automatic Proper
+00008d90: 7469 6573 0a0a 496e 2061 6464 6974 696f  ties..In additio
+00008da0: 6e20 746f 2074 6865 2069 6e68 6572 6974  n to the inherit
+00008db0: 616e 6365 206d 6563 6861 6e69 736d 2c20  ance mechanism, 
+00008dc0: 736f 6d65 2070 726f 7065 7274 6965 7320  some properties 
+00008dd0: 6172 6520 7365 7420 6175 746f 6d61 7469  are set automati
+00008de0: 6361 6c6c 7920 6279 2074 6865 2060 7964  cally by the `yd
+00008df0: 2d73 7562 6d69 7460 2063 6f6d 6d61 6e64  -submit` command
+00008e00: 2c20 6173 2061 2075 7361 6765 2063 6f6e  , as a usage con
+00008e10: 7665 6e69 656e 6365 2069 6620 7468 6579  venience if they
+00008e20: 2772 6520 6e6f 7420 6578 706c 6963 6974  're not explicit
+00008e30: 6c79 2070 726f 7669 6465 642e 0a0a 2323  ly provided...##
+00008e40: 2320 576f 726b 2052 6571 7569 7265 6d65  # Work Requireme
+00008e50: 6e74 2c20 5461 736b 2047 726f 7570 2061  nt, Task Group a
+00008e60: 6e64 2054 6173 6b20 4e61 6d69 6e67 0a0a  nd Task Naming..
+00008e70: 2d20 5468 6520 2a2a 576f 726b 2052 6571  - The **Work Req
+00008e80: 7569 7265 6d65 6e74 2a2a 206e 616d 6520  uirement** name 
+00008e90: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+00008ea0: 2073 6574 2075 7369 6e67 2061 2063 6f6e   set using a con
+00008eb0: 6361 7465 6e61 7469 6f6e 206f 6620 7468  catenation of th
+00008ec0: 6520 6074 6167 6020 7072 6f70 6572 7479  e `tag` property
+00008ed0: 2c20 6120 5554 4320 7469 6d65 7374 616d  , a UTC timestam
+00008ee0: 702c 2061 6e64 2074 6872 6565 2072 616e  p, and three ran
+00008ef0: 646f 6d20 6865 7820 6368 6172 6163 7465  dom hex characte
+00008f00: 7273 3a20 652c 672c 2e20 606d 7974 6167  rs: e,g,. `mytag
+00008f10: 5f32 3231 3032 342d 3135 3535 3234 2d34  _221024-155524-4
+00008f20: 3061 602e 0a2d 202a 2a54 6173 6b20 4772  0a`..- **Task Gr
+00008f30: 6f75 702a 2a20 6e61 6d65 7320 6172 6520  oup** names are 
+00008f40: 6175 746f 6d61 7469 6361 6c6c 7920 6372  automatically cr
+00008f50: 6561 7465 6420 666f 7220 616e 7920 5461  eated for any Ta
+00008f60: 736b 2047 726f 7570 2074 6861 7420 6973  sk Group that is
+00008f70: 206e 6f74 2065 7870 6c69 6369 746c 7920   not explicitly 
+00008f80: 6e61 6d65 642c 2075 7369 6e67 206e 616d  named, using nam
+00008f90: 6573 206f 6620 7468 6520 666f 726d 2060  es of the form `
+00008fa0: 7461 736b 5f67 726f 7570 5f31 6020 286f  task_group_1` (o
+00008fb0: 7220 6074 6173 6b5f 6772 6f75 705f 3031  r `task_group_01
+00008fc0: 602c 2065 7463 2e2c 2066 6f72 206c 6172  `, etc., for lar
+00008fd0: 6765 7220 6e75 6d62 6572 7320 6f66 2054  ger numbers of T
+00008fe0: 6173 6b20 4772 6f75 7073 292e 2054 6173  ask Groups). Tas
+00008ff0: 6b20 4772 6f75 7020 6e75 6d62 6572 7320  k Group numbers 
+00009000: 6361 6e20 616c 736f 2062 6520 696e 636c  can also be incl
+00009010: 7564 6564 2069 6e20 7573 6572 2d64 6566  uded in user-def
+00009020: 696e 6564 2054 6173 6b20 4772 6f75 7020  ined Task Group 
+00009030: 6e61 6d65 7320 7573 696e 6720 7468 6520  names using the 
+00009040: 607b 7b74 6173 6b5f 6772 6f75 705f 6e75  `{{task_group_nu
+00009050: 6d62 6572 7d7d 6020 7661 7269 6162 6c65  mber}}` variable
+00009060: 2073 7562 7374 6974 7574 696f 6e20 6469   substitution di
+00009070: 7363 7573 7365 6420 6265 6c6f 772e 0a2d  scussed below..-
+00009080: 202a 2a54 6173 6b2a 2a20 6e61 6d65 7320   **Task** names 
+00009090: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
+000090a0: 7920 6372 6561 7465 6420 666f 7220 616e  y created for an
+000090b0: 7920 5461 736b 2074 6861 7420 6973 206e  y Task that is n
+000090c0: 6f74 2065 7870 6c69 6369 746c 7920 6e61  ot explicitly na
+000090d0: 6d65 642c 2075 7369 6e67 206e 616d 6573  med, using names
+000090e0: 206f 6620 7468 6520 666f 726d 2060 7461   of the form `ta
+000090f0: 736b 5f31 6020 286f 7220 6074 6173 6b5f  sk_1` (or `task_
+00009100: 3031 602c 2065 7463 2e2c 2066 6f72 206c  01`, etc., for l
+00009110: 6172 6765 7220 6e75 6d62 6572 7320 6f66  arger numbers of
+00009120: 2054 6173 6b73 292e 2054 6865 2054 6173   Tasks). The Tas
+00009130: 6b20 636f 756e 7465 7220 7265 7365 7473  k counter resets
+00009140: 2066 6f72 2065 6163 6820 6469 6666 6572   for each differ
+00009150: 656e 7420 5461 736b 2047 726f 7570 2e20  ent Task Group. 
+00009160: 5461 736b 206e 756d 6265 7273 2063 616e  Task numbers can
+00009170: 2061 6c73 6f20 6265 2069 6e63 6c75 6465   also be include
+00009180: 6420 696e 2075 7365 722d 6465 6669 6e65  d in user-define
+00009190: 6420 5461 736b 206e 616d 6573 2075 7369  d Task names usi
+000091a0: 6e67 2074 6865 2060 7b7b 7461 736b 5f6e  ng the `{{task_n
+000091b0: 756d 6265 727d 7d60 2076 6172 6961 626c  umber}}` variabl
+000091c0: 6520 7375 6273 7469 7475 7469 6f6e 2064  e substitution d
+000091d0: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
+000091e0: 0a23 2323 2054 6173 6b20 5479 7065 730a  .### Task Types.
+000091f0: 0a2d 2049 6620 6074 6173 6b54 7970 6560  .- If `taskType`
+00009200: 2069 7320 7365 7420 6f6e 6c79 2061 7420   is set only at 
+00009210: 7468 6520 544f 4d4c 2066 696c 6520 6c65  the TOML file le
+00009220: 7665 6c2c 2074 6865 6e20 6074 6173 6b54  vel, then `taskT
+00009230: 7970 6573 6020 6973 2061 7574 6f6d 6174  ypes` is automat
+00009240: 6963 616c 6c79 2070 6f70 756c 6174 6564  ically populated
+00009250: 2066 6f72 2054 6173 6b20 4772 6f75 7073   for Task Groups
+00009260: 2c20 756e 6c65 7373 206f 7665 7272 6964  , unless overrid
+00009270: 6465 6e2e 0a2d 2049 6620 6074 6173 6b54  den..- If `taskT
+00009280: 7970 6560 2069 7320 7365 7420 6174 2074  ype` is set at t
+00009290: 6865 2054 6173 6b20 6c65 7665 6c2c 2074  he Task level, t
+000092a0: 6865 6e20 6074 6173 6b54 7970 6573 6020  hen `taskTypes` 
+000092b0: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+000092c0: 2070 6f70 756c 6174 6564 2066 6f72 2074   populated for t
+000092d0: 6865 2054 6173 6b20 4772 6f75 7073 206c  he Task Groups l
+000092e0: 6576 656c 2075 7369 6e67 2074 6865 2061  evel using the a
+000092f0: 6363 756d 756c 6174 6564 2054 6173 6b20  ccumulated Task 
+00009300: 5479 7065 7320 6672 6f6d 2074 6865 2054  Types from the T
+00009310: 6173 6b73 2069 6e63 6c75 6465 6420 696e  asks included in
+00009320: 2065 6163 6820 5461 736b 2047 726f 7570   each Task Group
+00009330: 2c20 756e 6c65 7373 206f 7665 7272 6964  , unless overrid
+00009340: 6465 6e2e 0a2d 2049 6620 6074 6173 6b54  den..- If `taskT
+00009350: 7970 6573 6020 6973 2073 6574 2061 7420  ypes` is set at 
+00009360: 7468 6520 5461 736b 2047 726f 7570 204c  the Task Group L
+00009370: 6576 656c 2c20 616e 6420 6861 7320 6f6e  evel, and has on
+00009380: 6c79 206f 6e65 2054 6173 6b20 5479 7065  ly one Task Type
+00009390: 2065 6e74 7279 2c20 7468 656e 2060 7461   entry, then `ta
+000093a0: 736b 5479 7065 6020 6973 2061 7574 6f6d  skType` is autom
+000093b0: 6174 6963 616c 6c79 2073 6574 2061 7420  atically set at 
+000093c0: 7468 6520 5461 736b 204c 6576 656c 2075  the Task Level u
+000093d0: 7369 6e67 2074 6865 2073 696e 676c 6520  sing the single 
+000093e0: 5461 736b 2054 7970 652c 2075 6e6c 6573  Task Type, unles
+000093f0: 7320 6f76 6572 7269 6464 656e 2e0a 0a46  s overridden...F
+00009400: 6f72 2074 6865 202a 2a60 6261 7368 602a  or the **`bash`*
+00009410: 2a2c 202a 2a60 706f 7765 7273 6865 6c6c  *, **`powershell
+00009420: 602a 2a2c 202a 2a60 636d 6460 2a2a 2f2a  `**, **`cmd`**/*
+00009430: 2a60 6261 7460 2a2a 2061 6e64 202a 2a60  *`bat`** and **`
+00009440: 646f 636b 6572 602a 2a20 7461 736b 2074  docker`** task t
+00009450: 7970 6573 2c20 736f 6d65 2061 7574 6f6d  ypes, some autom
+00009460: 6174 6963 2070 726f 6365 7373 696e 6720  atic processing 
+00009470: 7769 6c6c 2062 6520 7065 7266 6f72 6d65  will be performe
+00009480: 6420 6966 2074 6865 202a 2a60 6578 6563  d if the **`exec
+00009490: 7574 6162 6c65 602a 2a20 7072 6f70 6572  utable`** proper
+000094a0: 7479 2069 7320 7365 742e 0a0a 2323 2323  ty is set...####
+000094b0: 2042 6173 682c 2050 7974 686f 6e2c 2050   Bash, Python, P
+000094c0: 6f77 6572 5368 656c 6c20 616e 6420 636d  owerShell and cm
+000094d0: 642f 6261 7420 5461 736b 730a 0a41 7320  d/bat Tasks..As 
+000094e0: 6120 636f 6e76 656e 6965 6e63 652c 2066  a convenience, f
+000094f0: 6f72 2074 6865 202a 2a60 6261 7368 602a  or the **`bash`*
+00009500: 2a2c 202a 2a60 7079 7468 6f6e 602a 2a2c  *, **`python`**,
+00009510: 202a 2a60 706f 7765 7273 6865 6c6c 602a   **`powershell`*
+00009520: 2a2c 2061 6e64 202a 2a60 636d 6460 2a2a  *, and **`cmd`**
+00009530: 2028 6f72 202a 2a60 6261 7460 2a2a 2920   (or **`bat`**) 
+00009540: 5461 736b 2054 7970 6573 2c20 7468 6520  Task Types, the 
+00009550: 7363 7269 7074 206e 6f6d 696e 6174 6564  script nominated
+00009560: 2069 6e20 7468 6520 2a2a 6065 7865 6375   in the **`execu
+00009570: 7461 626c 6560 2a2a 2070 726f 7065 7274  table`** propert
+00009580: 7920 6973 2061 7574 6f6d 6174 6963 616c  y is automatical
+00009590: 6c79 2061 6464 6564 2074 6f20 7468 6520  ly added to the 
+000095a0: 6069 6e70 7574 7360 206c 6973 7420 2869  `inputs` list (i
+000095b0: 6620 6e6f 7420 616c 7265 6164 7920 7072  f not already pr
+000095c0: 6573 656e 7429 2e20 5468 6973 206d 6561  esent). This mea
+000095d0: 6e73 2074 6865 2073 6372 6970 7420 6669  ns the script fi
+000095e0: 6c65 2077 696c 6c20 6265 2075 706c 6f61  le will be uploa
+000095f0: 6465 6420 746f 2074 6865 204f 626a 6563  ded to the Objec
+00009600: 7420 5374 6f72 652c 2061 6e64 206d 6164  t Store, and mad
+00009610: 6520 6120 7265 7175 6972 656d 656e 7420  e a requirement 
+00009620: 6f66 2074 6865 2054 6173 6b20 7768 656e  of the Task when
+00009630: 2069 7420 7275 6e73 2e0a 0a55 7369 6e67   it runs...Using
+00009640: 2061 2042 6173 6820 5461 736b 2061 7320   a Bash Task as 
+00009650: 616e 2065 7861 6d70 6c65 2028 696e 2054  an example (in T
+00009660: 4f4d 4c20 666f 726d 293a 0a0a 6060 6074  OML form):..```t
+00009670: 6f6d 6c0a 7461 736b 5479 7065 203d 2022  oml.taskType = "
+00009680: 6261 7368 220a 6578 6563 7574 6162 6c65  bash".executable
+00009690: 203d 2022 6d79 5f62 6173 685f 7363 7269   = "my_bash_scri
+000096a0: 7074 2e73 6822 0a61 7267 756d 656e 7473  pt.sh".arguments
+000096b0: 203d 205b 2231 222c 2022 3222 2c20 2233   = ["1", "2", "3
+000096c0: 225d 0a60 6060 0a69 7320 6571 7569 7661  "].```.is equiva
+000096d0: 6c65 6e74 2074 6f3a 0a0a 6060 6074 6f6d  lent to:..```tom
+000096e0: 6c0a 7461 736b 5479 7065 203d 2022 6261  l.taskType = "ba
+000096f0: 7368 220a 696e 7075 7473 203d 205b 226d  sh".inputs = ["m
+00009700: 795f 6261 7368 5f73 6372 6970 742e 7368  y_bash_script.sh
+00009710: 225d 0a61 7267 756d 656e 7473 203d 205b  "].arguments = [
+00009720: 227b 7b77 725f 6e61 6d65 7d7d 2f6d 795f  "{{wr_name}}/my_
+00009730: 6261 7368 5f73 6372 6970 742e 7368 222c  bash_script.sh",
+00009740: 2022 3122 2c20 2232 222c 2022 3322 5d0a   "1", "2", "3"].
+00009750: 6060 600a 0a49 6e20 7468 6520 6361 7365  ```..In the case
+00009760: 206f 6620 5769 6e64 6f77 7320 6261 7463   of Windows batc
+00009770: 6820 2860 2e62 6174 6029 2066 696c 6573  h (`.bat`) files
+00009780: 2c20 6120 602f 6360 2066 6c61 6720 6973  , a `/c` flag is
+00009790: 2070 7265 7065 6e64 6564 2074 6f20 7468   prepended to th
+000097a0: 6520 6063 6d64 2e65 7865 6020 6172 6775  e `cmd.exe` argu
+000097b0: 6d65 6e74 206c 6973 7420 746f 2065 6e73  ment list to ens
+000097c0: 7572 6520 636f 7272 6563 7420 6578 6563  ure correct exec
+000097d0: 7574 696f 6e20 6261 6861 7669 6f75 722e  ution bahaviour.
+000097e0: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a60   For example:..`
+000097f0: 6060 746f 6d6c 0a74 6173 6b54 7970 6520  ``toml.taskType 
+00009800: 3d20 2263 6d64 2220 2023 206f 7220 2262  = "cmd"  # or "b
+00009810: 6174 220a 6578 6563 7574 6162 6c65 203d  at".executable =
+00009820: 2022 6d79 5f73 6372 6970 742e 6261 7422   "my_script.bat"
+00009830: 0a61 7267 756d 656e 7473 203d 205b 2231  .arguments = ["1
+00009840: 222c 2022 3222 2c20 2233 225d 0a60 6060  ", "2", "3"].```
+00009850: 0a0a 6973 2065 7175 6976 616c 656e 7420  ..is equivalent 
+00009860: 746f 3a0a 0a60 6060 746f 6d6c 0a74 6173  to:..```toml.tas
+00009870: 6b54 7970 6520 3d20 2263 6d64 2220 2023  kType = "cmd"  #
+00009880: 206f 7220 2262 6174 220a 696e 7075 7473   or "bat".inputs
+00009890: 203d 205b 226d 795f 7363 7269 7074 2e62   = ["my_script.b
+000098a0: 6174 225d 0a61 7267 756d 656e 7473 203d  at"].arguments =
+000098b0: 205b 222f 6322 2c20 227b 7b77 725f 6e61   ["/c", "{{wr_na
+000098c0: 6d65 7d7d 5c5c 6d79 5f73 6372 6970 742e  me}}\\my_script.
+000098d0: 6261 7422 2c20 2231 222c 2022 3222 2c20  bat", "1", "2", 
+000098e0: 2233 225d 0a60 6060 0a0a 4e6f 7465 2074  "3"].```..Note t
+000098f0: 6865 2060 5c5c 6020 7265 7175 6972 656d  he `\\` requirem
+00009900: 656e 7420 666f 7220 6469 7265 6374 6f72  ent for director
+00009910: 7920 7365 7061 7261 746f 7273 2077 6865  y separators whe
+00009920: 6e20 6465 6669 6e69 6e67 2054 6173 6b73  n defining Tasks
+00009930: 206f 6e20 5769 6e64 6f77 7320 686f 7374   on Windows host
+00009940: 732e 204e 6f74 6520 616c 736f 2074 6861  s. Note also tha
+00009950: 7420 7468 6520 602f 6360 2069 7320 7265  t the `/c` is re
+00009960: 7175 6972 6564 2077 6865 6e20 7275 6e6e  quired when runn
+00009970: 696e 6720 636f 6d6d 616e 6473 206f 7220  ing commands or 
+00009980: 6261 7463 6820 7363 7269 7074 7320 7573  batch scripts us
+00009990: 696e 6720 6063 6d64 2e65 7865 602c 206f  ing `cmd.exe`, o
+000099a0: 7468 6572 7769 7365 2074 6865 2060 636d  therwise the `cm
+000099b0: 642e 6578 6560 2070 726f 6365 7373 2063  d.exe` process c
+000099c0: 7265 6174 6564 2074 6f20 6578 6563 7574  reated to execut
+000099d0: 6520 7468 6520 5461 736b 2077 696c 6c20  e the Task will 
+000099e0: 6e6f 7420 7465 726d 696e 6174 652e 0a0a  not terminate...
+000099f0: 2323 2323 2044 6f63 6b65 7220 5461 736b  #### Docker Task
+00009a00: 730a 0a46 6f72 2074 6865 202a 2a60 646f  s..For the **`do
+00009a10: 636b 6572 602a 2a20 5461 736b 2054 7970  cker`** Task Typ
+00009a20: 652c 2074 6865 2076 6172 6961 626c 6573  e, the variables
+00009a30: 2073 7570 706c 6965 6420 696e 2074 6865   supplied in the
+00009a40: 2060 646f 636b 6572 456e 7669 726f 6e6d   `dockerEnvironm
+00009a50: 656e 7460 2070 726f 7065 7274 7920 6172  ent` property ar
+00009a60: 6520 756e 7061 636b 6564 2069 6e74 6f20  e unpacked into 
+00009a70: 7468 6520 6172 6775 6d65 6e74 206c 6973  the argument lis
+00009a80: 7420 6173 2060 2d2d 656e 7660 2065 6e74  t as `--env` ent
+00009a90: 7269 6573 2c20 7468 6520 446f 636b 6572  ries, the Docker
+00009aa0: 2063 6f6e 7461 696e 6572 206e 616d 6520   container name 
+00009ab0: 7375 7070 6c69 6564 2069 6e20 7468 6520  supplied in the 
+00009ac0: 6065 7865 6375 7461 626c 6560 2070 726f  `executable` pro
+00009ad0: 7065 7274 7920 6973 2074 6865 6e20 6164  perty is then ad
+00009ae0: 6465 6420 746f 2074 6865 2061 7267 756d  ded to the argum
+00009af0: 656e 7473 206c 6973 742c 2066 6f6c 6c6f  ents list, follo
+00009b00: 7765 6420 6279 2074 6865 2061 7267 756d  wed by the argum
+00009b10: 656e 7473 2073 7570 706c 6965 6420 696e  ents supplied in
+00009b20: 2074 6865 2060 6172 6775 6d65 6e74 7360   the `arguments`
+00009b30: 2070 726f 7065 7274 792e 2054 6865 2060   property. The `
+00009b40: 646f 636b 6572 5573 6572 6e61 6d65 6020  dockerUsername` 
+00009b50: 616e 6420 6064 6f63 6b65 7250 6173 7377  and `dockerPassw
+00009b60: 6f72 6460 2070 726f 7065 7274 6965 732c  ord` properties,
+00009b70: 2069 6620 7375 7070 6c69 6564 2c20 6172   if supplied, ar
+00009b80: 6520 6164 6465 6420 746f 2074 6865 2060  e added to the `
+00009b90: 656e 7669 726f 6e6d 656e 7460 2070 726f  environment` pro
+00009ba0: 7065 7274 792e 0a0a 466f 7220 6578 616d  perty...For exam
+00009bb0: 706c 653a 0a60 6060 746f 6d6c 0a74 6173  ple:.```toml.tas
+00009bc0: 6b54 7970 6520 3d20 2264 6f63 6b65 7222  kType = "docker"
+00009bd0: 0a65 7865 6375 7461 626c 6520 3d20 226d  .executable = "m
+00009be0: 795f 646f 636b 6572 6875 625f 7265 706f  y_dockerhub_repo
+00009bf0: 2f6d 795f 636f 6e74 6169 6e65 725f 696d  /my_container_im
+00009c00: 6167 6522 0a64 6f63 6b65 7245 6e76 6972  age".dockerEnvir
+00009c10: 6f6e 6d65 6e74 203d 207b 4531 203d 2022  onment = {E1 = "
+00009c20: 4565 654f 6e65 227d 0a64 6f63 6b65 7255  EeeOne"}.dockerU
+00009c30: 7365 726e 616d 6520 3d20 226d 795f 7573  sername = "my_us
+00009c40: 6572 220a 646f 636b 6572 5061 7373 776f  er".dockerPasswo
+00009c50: 7264 203d 2022 6d79 5f70 6173 7377 6f72  rd = "my_passwor
+00009c60: 6422 0a61 7267 756d 656e 7473 203d 205b  d".arguments = [
+00009c70: 2231 222c 2022 3222 2c20 2233 225d 0a60  "1", "2", "3"].`
+00009c80: 6060 0a0a 6973 2065 7175 6976 616c 656e  ``..is equivalen
+00009c90: 7420 746f 2074 6865 2066 6f6c 6c6f 7769  t to the followi
+00009ca0: 6e67 2062 6569 6e67 2073 656e 7420 666f  ng being sent fo
+00009cb0: 7220 7072 6f63 6573 7369 6e67 2062 7920  r processing by 
+00009cc0: 7468 6520 6064 6f63 6b65 7260 2054 6173  the `docker` Tas
+00009cd0: 6b20 5479 7065 2c20 7468 6520 5965 6c6c  k Type, the Yell
+00009ce0: 6f77 446f 6720 7665 7273 696f 6e20 6f66  owDog version of
+00009cf0: 2077 6869 6368 2077 696c 6c20 6c6f 6720   which will log 
+00009d00: 696e 2074 6f20 7468 6520 446f 636b 6572  in to the Docker
+00009d10: 2072 6570 6f20 2869 6620 7265 7175 6972   repo (if requir
+00009d20: 6564 2920 7468 656e 2069 7373 7565 2061  ed) then issue a
+00009d30: 2060 646f 636b 6572 2072 756e 6020 636f   `docker run` co
+00009d40: 6d6d 616e 6420 7769 7468 2074 6865 2061  mmand with the a
+00009d50: 7267 756d 656e 7473 2073 7570 706c 6965  rguments supplie
+00009d60: 643a 0a0a 6060 6074 6f6d 6c0a 7461 736b  d:..```toml.task
+00009d70: 5479 7065 203d 2022 646f 636b 6572 220a  Type = "docker".
+00009d80: 6172 6775 6d65 6e74 7320 3d20 5b22 2d2d  arguments = ["--
+00009d90: 656e 7620 4531 3d45 6565 4f6e 6522 2c20  env E1=EeeOne", 
+00009da0: 226d 795f 646f 636b 6572 6875 6272 6570  "my_dockerhubrep
+00009db0: 6f2f 6d79 5f63 6f6e 7461 696e 6572 5f69  o/my_container_i
+00009dc0: 6d61 6765 222c 2022 3122 2c20 2232 222c  mage", "1", "2",
+00009dd0: 2022 3322 5d0a 656e 7669 726f 6e6d 656e   "3"].environmen
+00009de0: 7420 3d20 7b44 4f43 4b45 525f 5553 4552  t = {DOCKER_USER
+00009df0: 4e41 4d45 203d 2022 6d79 5f75 7365 7222  NAME = "my_user"
+00009e00: 2c20 444f 434b 4552 5f50 4153 5357 4f52  , DOCKER_PASSWOR
+00009e10: 4420 3d20 226d 795f 7061 7373 776f 7264  D = "my_password
+00009e20: 227d 0a60 6060 0a0a 2323 2323 2042 6173  "}.```..#### Bas
+00009e30: 682c 2050 7974 686f 6e2c 2050 6f77 6572  h, Python, Power
+00009e40: 5368 656c 6c2c 2063 6d64 2e65 7865 2f62  Shell, cmd.exe/b
+00009e50: 6174 6368 2c20 616e 6420 446f 636b 6572  atch, and Docker
+00009e60: 2077 6974 686f 7574 2041 7574 6f6d 6174   without Automat
+00009e70: 6963 2050 726f 6365 7373 696e 670a 0a49  ic Processing..I
+00009e80: 6620 7468 6520 6065 7865 6375 7461 626c  f the `executabl
+00009e90: 6560 2070 726f 7065 7274 7920 6973 206e  e` property is n
+00009ea0: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
+00009eb0: 2061 7574 6f6d 6174 6963 2070 726f 6365   automatic proce
+00009ec0: 7373 696e 6720 6465 7363 7269 6265 6420  ssing described 
+00009ed0: 6162 6f76 6520 666f 7220 6062 6173 6860  above for `bash`
+00009ee0: 2c20 6070 7974 686f 6e60 2c20 6070 6f77  , `python`, `pow
+00009ef0: 6572 7368 656c 6c60 2c20 6063 6d64 6020  ershell`, `cmd` 
+00009f00: 286f 7220 6062 6174 6029 2061 6e64 2060  (or `bat`) and `
+00009f10: 646f 636b 6572 6020 7461 736b 2074 7970  docker` task typ
+00009f20: 6573 2069 7320 6e6f 7420 6170 706c 6965  es is not applie
+00009f30: 642e 0a0a 2323 2320 5461 736b 2043 6f75  d...### Task Cou
+00009f40: 6e74 730a 0a54 6869 7320 7072 6f70 6572  nts..This proper
+00009f50: 7479 2077 696c 6c20 6578 7061 6e64 2074  ty will expand t
+00009f60: 6865 206e 756d 6265 7220 6f66 2054 6173  he number of Tas
+00009f70: 6b73 2074 6f20 6d61 7463 6820 6074 6173  ks to match `tas
+00009f80: 6b43 6f75 6e74 602e 0a0a 5468 6520 6074  kCount`...The `t
+00009f90: 6173 6b43 6f75 6e74 6020 7072 6f70 6572  askCount` proper
+00009fa0: 7479 2063 616e 2062 6520 7365 7420 6f6e  ty can be set on
+00009fb0: 6c79 2069 6e20 7468 6520 6077 6f72 6b52  ly in the `workR
+00009fc0: 6571 7569 7265 6d65 6e74 6020 7365 6374  equirement` sect
+00009fd0: 696f 6e20 6f66 2074 6865 2060 636f 6e66  ion of the `conf
+00009fe0: 6967 2e74 6f6d 6c60 2066 696c 652c 206f  ig.toml` file, o
+00009ff0: 7220 696e 2074 6865 2060 7461 736b 4772  r in the `taskGr
+0000a000: 6f75 7060 2073 6563 7469 6f6e 2873 2920  oup` section(s) 
+0000a010: 6f66 2061 204a 534f 4e20 576f 726b 2052  of a JSON Work R
+0000a020: 6571 7569 7265 6d65 6e74 2064 6566 696e  equirement defin
+0000a030: 6974 696f 6e2e 0a0a 496e 2074 6865 2066  ition...In the f
+0000a040: 6f72 6d65 7220 6361 7365 2c20 7468 6520  ormer case, the 
+0000a050: 6074 6173 6b43 6f75 6e74 6020 6170 706c  `taskCount` appl
+0000a060: 6965 7320 6f6e 6c79 2074 6f20 7468 6520  ies only to the 
+0000a070: 5461 736b 2073 7065 6369 6669 6564 2077  Task specified w
+0000a080: 6974 6869 6e20 7468 6520 6063 6f6e 6669  ithin the `confi
+0000a090: 672e 746f 6d6c 6020 6669 6c65 2061 6e64  g.toml` file and
+0000a0a0: 2069 7320 6e6f 7420 696e 6865 7269 7465   is not inherite
+0000a0b0: 6420 6279 204a 534f 4e20 576f 726b 2052  d by JSON Work R
+0000a0c0: 6571 7569 7265 6d65 6e74 2073 7065 6369  equirement speci
+0000a0d0: 6669 6361 7469 6f6e 732e 0a0a 496e 2074  fications...In t
+0000a0e0: 6865 206c 6174 7465 7220 6361 7365 2c20  he latter case, 
+0000a0f0: 7468 6520 6074 6173 6b43 6f75 6e74 6020  the `taskCount` 
+0000a100: 6170 706c 6965 7320 746f 2074 6865 2054  applies to the T
+0000a110: 6173 6b20 7370 6563 6966 6965 6420 7769  ask specified wi
+0000a120: 7468 696e 2074 6865 2054 6173 6b20 4772  thin the Task Gr
+0000a130: 6f75 702c 2061 6e64 2074 6865 7265 206d  oup, and there m
+0000a140: 7573 7420 6265 207a 6572 6f20 6f72 206f  ust be zero or o
+0000a150: 6e65 2054 6173 6b28 7329 206c 6973 7465  ne Task(s) liste
+0000a160: 6420 7769 7468 696e 2074 6865 2067 726f  d within the gro
+0000a170: 7570 206f 7220 6074 6173 6b43 6f75 6e74  up or `taskCount
+0000a180: 6020 6973 2069 676e 6f72 6564 2e0a 0a23  ` is ignored...#
+0000a190: 2320 4578 616d 706c 6573 0a0a 2323 2320  # Examples..### 
+0000a1a0: 544f 4d4c 2050 726f 7065 7274 6965 7320  TOML Properties 
+0000a1b0: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
+0000a1c0: 6972 656d 656e 7460 2053 6563 7469 6f6e  irement` Section
+0000a1d0: 0a0a 4865 7265 2773 2061 6e20 6578 616d  ..Here's an exam
+0000a1e0: 706c 6520 6f66 2074 6865 2060 776f 726b  ple of the `work
+0000a1f0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
+0000a200: 7469 6f6e 206f 6620 6120 544f 4d4c 2063  tion of a TOML c
+0000a210: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+0000a220: 652c 2073 686f 7769 6e67 2061 6c6c 2074  e, showing all t
+0000a230: 6865 2070 6f73 7369 626c 6520 7072 6f70  he possible prop
+0000a240: 6572 7469 6573 2074 6861 7420 6361 6e20  erties that can 
+0000a250: 6265 2073 6574 3a0a 0a60 6060 746f 6d6c  be set:..```toml
+0000a260: 0a5b 776f 726b 5265 7175 6972 656d 656e  .[workRequiremen
+0000a270: 745d 0a20 2020 2061 7267 756d 656e 7473  t].    arguments
+0000a280: 203d 205b 2231 222c 2022 5457 4f22 5d0a   = ["1", "TWO"].
+0000a290: 2020 2020 6361 7074 7572 6554 6173 6b4f      captureTaskO
+0000a2a0: 7574 7075 7420 3d20 7472 7565 0a20 2020  utput = true.   
+0000a2b0: 2063 6f6d 706c 6574 6564 5461 736b 5474   completedTaskTt
+0000a2c0: 6c20 3d20 3130 0a20 2020 2063 7376 4669  l = 10.    csvFi
+0000a2d0: 6c65 203d 2022 6669 6c65 312e 6373 7622  le = "file1.csv"
+0000a2e0: 0a20 2020 2063 7376 4669 6c65 7320 3d20  .    csvFiles = 
+0000a2f0: 5b22 6669 6c65 312e 6373 7622 2c20 2266  ["file1.csv", "f
+0000a300: 696c 6533 2e63 7376 3a33 225d 0a20 2020  ile3.csv:3"].   
+0000a310: 2064 6f63 6b65 7245 6e76 6972 6f6e 6d65   dockerEnvironme
+0000a320: 6e74 203d 207b 4d59 5f44 4f43 4b45 525f  nt = {MY_DOCKER_
+0000a330: 5641 5220 3d20 3130 307d 0a20 2020 2064  VAR = 100}.    d
+0000a340: 6f63 6b65 7250 6173 7377 6f72 6420 3d20  ockerPassword = 
+0000a350: 226d 7950 6173 7377 6f72 6422 0a20 2020  "myPassword".   
+0000a360: 2064 6f63 6b65 7255 7365 726e 616d 6520   dockerUsername 
+0000a370: 3d20 226d 7955 7365 726e 616d 6522 0a20  = "myUsername". 
+0000a380: 2020 2065 6e76 6972 6f6e 6d65 6e74 203d     environment =
+0000a390: 207b 4d59 5f56 4152 203d 2031 3030 7d0a   {MY_VAR = 100}.
+0000a3a0: 2020 2020 6578 636c 7573 6976 6557 6f72      exclusiveWor
+0000a3b0: 6b65 7273 203d 2066 616c 7365 0a20 2020  kers = false.   
+0000a3c0: 2065 7865 6375 7461 626c 6520 3d20 226d   executable = "m
+0000a3d0: 792d 636f 6e74 6169 6e65 7222 0a20 2020  y-container".   
+0000a3e0: 2066 696e 6973 6849 6641 6c6c 5461 736b   finishIfAllTask
+0000a3f0: 7346 696e 6973 6865 6420 3d20 7472 7565  sFinished = true
+0000a400: 0a20 2020 2066 696e 6973 6849 6641 6e79  .    finishIfAny
+0000a410: 5461 736b 4661 696c 6564 203d 2066 616c  TaskFailed = fal
+0000a420: 7365 0a20 2020 2066 6c61 7474 656e 496e  se.    flattenIn
+0000a430: 7075 7450 6174 6873 203d 2066 616c 7365  putPaths = false
+0000a440: 0a20 2020 2066 6c61 7474 656e 5570 6c6f  .    flattenUplo
+0000a450: 6164 5061 7468 7320 3d20 6661 6c73 650a  adPaths = false.
+0000a460: 2020 2020 6675 6c66 696c 4f6e 5375 626d      fulfilOnSubm
+0000a470: 6974 203d 2066 616c 7365 0a20 2020 2069  it = false.    i
+0000a480: 6e70 7574 7320 3d20 5b0a 2020 2020 2020  nputs = [.      
+0000a490: 2020 222e 2e2f 6170 702f 6d61 696e 2e70    "../app/main.p
+0000a4a0: 7922 2c0a 2020 2020 2020 2020 222e 2e2f  y",.        "../
+0000a4b0: 6170 702f 7265 7175 6972 656d 656e 7473  app/requirements
+0000a4c0: 2e74 7874 220a 2020 2020 5d0a 2020 2020  .txt".    ].    
+0000a4d0: 696e 7075 7473 4f70 7469 6f6e 616c 203d  inputsOptional =
+0000a4e0: 205b 226f 7074 696f 6e61 6c2e 7478 7422   ["optional.txt"
+0000a4f0: 5d0a 2020 2020 696e 7374 616e 6365 5479  ].    instanceTy
+0000a500: 7065 7320 3d20 5b22 7433 612e 6d69 6372  pes = ["t3a.micr
+0000a510: 6f22 2c20 2274 332e 6d69 6372 6f22 5d0a  o", "t3.micro"].
+0000a520: 2020 2020 6d61 7857 6f72 6b65 7273 203d      maxWorkers =
+0000a530: 2031 0a20 2020 206d 6178 696d 756d 5461   1.    maximumTa
+0000a540: 736b 5265 7472 6965 7320 3d20 300a 2020  skRetries = 0.  
+0000a550: 2020 6d69 6e57 6f72 6b65 7273 203d 2031    minWorkers = 1
+0000a560: 0a20 2020 206e 616d 6520 3d20 226d 792d  .    name = "my-
+0000a570: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
+0000a580: 220a 2020 2020 6f75 7470 7574 7320 3d20  ".    outputs = 
+0000a590: 5b22 7265 7375 6c74 732e 7478 7422 5d0a  ["results.txt"].
+0000a5a0: 2020 2020 6f75 7470 7574 7352 6571 7569      outputsRequi
+0000a5b0: 7265 6420 3d20 5b22 7265 7375 6c74 735f  red = ["results_
+0000a5c0: 7265 7175 6972 6564 2e74 7874 225d 0a20  required.txt"]. 
+0000a5d0: 2020 2070 7269 6f72 6974 7920 3d20 302e     priority = 0.
+0000a5e0: 300a 2020 2020 7072 6f76 6964 6572 7320  0.    providers 
+0000a5f0: 3d20 5b22 4157 5322 5d0a 2020 2020 7261  = ["AWS"].    ra
+0000a600: 6d20 3d20 5b30 2e35 2c20 322e 305d 0a20  m = [0.5, 2.0]. 
+0000a610: 2020 2072 6567 696f 6e73 203d 205b 2265     regions = ["e
+0000a620: 752d 7765 7374 2d32 225d 0a20 2020 2074  u-west-2"].    t
+0000a630: 6173 6b42 6174 6368 5369 7a65 203d 2031  askBatchSize = 1
+0000a640: 3030 300a 2020 2020 7461 736b 436f 756e  000.    taskCoun
+0000a650: 7420 3d20 3130 300a 2020 2020 7461 736b  t = 100.    task
+0000a660: 4461 7461 203d 2022 6d79 5f64 6174 615f  Data = "my_data_
+0000a670: 7374 7269 6e67 220a 2020 2020 7461 736b  string".    task
+0000a680: 4461 7461 4669 6c65 203d 2022 6d79 5f64  DataFile = "my_d
+0000a690: 6174 615f 6669 6c65 2e74 7874 220a 2020  ata_file.txt".  
+0000a6a0: 2020 7461 736b 4e61 6d65 203d 2022 6d79    taskName = "my
+0000a6b0: 5f74 6173 6b5f 6e75 6d62 6572 5f7b 7b74  _task_number_{{t
+0000a6c0: 6173 6b5f 6e75 6d62 6572 7d7d 220a 2020  ask_number}}".  
+0000a6d0: 2020 7461 736b 4772 6f75 704e 616d 6520    taskGroupName 
+0000a6e0: 3d20 226d 795f 7461 736b 5f67 726f 7570  = "my_task_group
+0000a6f0: 5f6e 756d 6265 725f 7b7b 7461 736b 5f67  _number_{{task_g
+0000a700: 726f 7570 5f6e 756d 6265 727d 7d22 0a20  roup_number}}". 
+0000a710: 2020 2074 6173 6b54 7970 6520 3d20 2264     taskType = "d
+0000a720: 6f63 6b65 7222 0a20 2020 2074 6173 6b73  ocker".    tasks
+0000a730: 5065 7257 6f72 6b65 7220 3d20 310a 2020  PerWorker = 1.  
+0000a740: 2020 7570 6c6f 6164 4669 6c65 7320 3d20    uploadFiles = 
+0000a750: 5b7b 6c6f 6361 6c50 6174 6820 3d20 2266  [{localPath = "f
+0000a760: 696c 655f 312e 7478 7422 2c20 7570 6c6f  ile_1.txt", uplo
+0000a770: 6164 5061 7468 203d 2022 6669 6c65 5f31  adPath = "file_1
+0000a780: 2e74 7874 227d 5d0a 2020 2020 7663 7075  .txt"}].    vcpu
+0000a790: 7320 3d20 5b31 2c20 345d 0a20 2020 2076  s = [1, 4].    v
+0000a7a0: 6572 6966 7941 7453 7461 7274 203d 205b  erifyAtStart = [
+0000a7b0: 2272 6561 6479 5f72 6573 756c 7473 2e74  "ready_results.t
+0000a7c0: 7874 225d 0a20 2020 2076 6572 6966 7957  xt"].    verifyW
+0000a7d0: 6169 7420 3d20 5b22 7761 6974 5f66 6f72  ait = ["wait_for
+0000a7e0: 5f72 6573 756c 7473 2e74 7874 225d 0a20  _results.txt"]. 
+0000a7f0: 2020 2077 6f72 6b65 7254 6167 7320 3d20     workerTags = 
+0000a800: 5b22 7461 672d 7b7b 7573 6572 6e61 6d65  ["tag-{{username
+0000a810: 7d7d 225d 0a20 2020 2077 6f72 6b52 6571  }}"].    workReq
+0000a820: 7569 7265 6d65 6e74 4461 7461 203d 2022  uirementData = "
+0000a830: 776f 726b 5f72 6571 7569 7265 6d65 6e74  work_requirement
+0000a840: 2e6a 736f 6e22 0a60 6060 0a0a 2323 2320  .json".```..### 
+0000a850: 4a53 4f4e 2050 726f 7065 7274 6965 7320  JSON Properties 
+0000a860: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
+0000a870: 6972 656d 656e 7420 4c65 7665 6c0a 0a53  irement Level..S
+0000a880: 686f 7769 6e67 2061 6c6c 2070 6f73 7369  howing all possi
+0000a890: 626c 6520 7072 6f70 6572 7469 6573 2061  ble properties a
+0000a8a0: 7420 7468 6520 576f 726b 2052 6571 7569  t the Work Requi
+0000a8b0: 7265 6d65 6e74 206c 6576 656c 3a0a 0a60  rement level:..`
+0000a8c0: 6060 6a73 6f6e 0a7b 0a20 2022 6172 6775  ``json.{.  "argu
+0000a8d0: 6d65 6e74 7322 3a20 5b31 2c20 2254 574f  ments": [1, "TWO
+0000a8e0: 225d 2c0a 2020 2263 6170 7475 7265 5461  "],.  "captureTa
+0000a8f0: 736b 4f75 7470 7574 223a 2074 7275 652c  skOutput": true,
+0000a900: 0a20 2022 636f 6d70 6c65 7465 6454 6173  .  "completedTas
+0000a910: 6b54 746c 223a 2031 302c 0a20 2022 646f  kTtl": 10,.  "do
+0000a920: 636b 6572 456e 7669 726f 6e6d 656e 7422  ckerEnvironment"
+0000a930: 3a20 7b22 4d59 5f44 4f43 4b45 525f 5641  : {"MY_DOCKER_VA
+0000a940: 5222 3a20 3130 307d 2c0a 2020 2264 6f63  R": 100},.  "doc
+0000a950: 6b65 7250 6173 7377 6f72 6422 3a20 226d  kerPassword": "m
+0000a960: 7950 6173 7377 6f72 6422 2c0a 2020 2264  yPassword",.  "d
+0000a970: 6f63 6b65 7255 7365 726e 616d 6522 3a20  ockerUsername": 
+0000a980: 226d 7955 7365 726e 616d 6522 2c0a 2020  "myUsername",.  
+0000a990: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+0000a9a0: 224d 595f 5641 5222 3a20 3130 307d 2c0a  "MY_VAR": 100},.
+0000a9b0: 2020 2265 7863 6c75 7369 7665 576f 726b    "exclusiveWork
+0000a9c0: 6572 7322 3a20 6661 6c73 652c 0a20 2022  ers": false,.  "
+0000a9d0: 6578 6563 7574 6162 6c65 223a 2022 6d79  executable": "my
+0000a9e0: 2d63 6f6e 7461 696e 6572 222c 0a20 2022  -container",.  "
+0000a9f0: 6669 6e69 7368 4966 416c 6c54 6173 6b73  finishIfAllTasks
+0000aa00: 4669 6e69 7368 6564 223a 2074 7275 652c  Finished": true,
+0000aa10: 0a20 2022 6669 6e69 7368 4966 416e 7954  .  "finishIfAnyT
+0000aa20: 6173 6b46 6169 6c65 6422 3a20 6661 6c73  askFailed": fals
+0000aa30: 652c 0a20 2022 666c 6174 7465 6e49 6e70  e,.  "flattenInp
+0000aa40: 7574 5061 7468 7322 3a20 6661 6c73 652c  utPaths": false,
+0000aa50: 0a20 2022 666c 6174 7465 6e55 706c 6f61  .  "flattenUploa
+0000aa60: 6450 6174 6873 223a 2066 616c 7365 2c0a  dPaths": false,.
+0000aa70: 2020 2266 756c 6669 6c4f 6e53 7562 6d69    "fulfilOnSubmi
+0000aa80: 7422 3a20 6661 6c73 652c 0a20 2022 696e  t": false,.  "in
+0000aa90: 7075 7473 223a 205b 2261 7070 2f6d 6169  puts": ["app/mai
+0000aaa0: 6e2e 7079 222c 2022 6170 702f 7265 7175  n.py", "app/requ
+0000aab0: 6972 656d 656e 7473 2e74 7874 225d 2c0a  irements.txt"],.
+0000aac0: 2020 2269 6e70 7574 734f 7074 696f 6e61    "inputsOptiona
+0000aad0: 6c22 3a20 5b22 6f70 7469 6f6e 616c 2e74  l": ["optional.t
+0000aae0: 7874 225d 2c0a 2020 2269 6e73 7461 6e63  xt"],.  "instanc
+0000aaf0: 6554 7970 6573 223a 205b 2274 3361 2e6d  eTypes": ["t3a.m
+0000ab00: 6963 726f 222c 2022 7433 2e6d 6963 726f  icro", "t3.micro
+0000ab10: 225d 2c0a 2020 226d 6178 576f 726b 6572  "],.  "maxWorker
+0000ab20: 7322 3a20 312c 0a20 2022 6d61 7869 6d75  s": 1,.  "maximu
+0000ab30: 6d54 6173 6b52 6574 7269 6573 223a 2030  mTaskRetries": 0
+0000ab40: 2c0a 2020 226d 696e 576f 726b 6572 7322  ,.  "minWorkers"
+0000ab50: 3a20 312c 0a20 2022 6e61 6d65 223a 2022  : 1,.  "name": "
+0000ab60: 6d79 2d77 6f72 6b2d 7265 7175 6972 656d  my-work-requirem
+0000ab70: 656e 7422 2c0a 2020 226f 7574 7075 7473  ent",.  "outputs
+0000ab80: 223a 205b 2272 6573 756c 7473 2e74 7874  ": ["results.txt
+0000ab90: 225d 2c0a 2020 226f 7574 7075 7473 5265  "],.  "outputsRe
+0000aba0: 7175 6972 6564 223a 205b 2272 6573 756c  quired": ["resul
+0000abb0: 7473 5f72 6571 7569 7265 642e 7478 7422  ts_required.txt"
+0000abc0: 5d2c 0a20 2022 7072 696f 7269 7479 223a  ],.  "priority":
+0000abd0: 2030 2e30 2c0a 2020 2270 726f 7669 6465   0.0,.  "provide
+0000abe0: 7273 223a 205b 2241 5753 225d 2c0a 2020  rs": ["AWS"],.  
+0000abf0: 2272 616d 223a 205b 302e 352c 2032 5d2c  "ram": [0.5, 2],
+0000ac00: 0a20 2022 7265 6769 6f6e 7322 3a20 5b22  .  "regions": ["
+0000ac10: 6575 2d77 6573 742d 3222 5d2c 0a20 2022  eu-west-2"],.  "
+0000ac20: 7461 736b 4461 7461 223a 2022 6d79 5f74  taskData": "my_t
+0000ac30: 6173 6b5f 6461 7461 5f73 7472 696e 6722  ask_data_string"
+0000ac40: 2c0a 2020 2274 6173 6b44 6174 6146 696c  ,.  "taskDataFil
+0000ac50: 6522 3a20 226d 795f 6461 7461 5f66 696c  e": "my_data_fil
+0000ac60: 652e 7478 7422 2c0a 2020 2274 6173 6b54  e.txt",.  "taskT
+0000ac70: 7970 6573 223a 205b 2264 6f63 6b65 7222  ypes": ["docker"
+0000ac80: 5d2c 0a20 2022 7461 736b 7350 6572 576f  ],.  "tasksPerWo
+0000ac90: 726b 6572 223a 2031 2c0a 2020 2275 706c  rker": 1,.  "upl
+0000aca0: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
+0000acb0: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
+0000acc0: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
+0000acd0: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
+0000ace0: 7422 7d5d 2c0a 2020 2276 6370 7573 223a  t"}],.  "vcpus":
+0000acf0: 205b 312c 2034 5d2c 0a20 2022 7665 7269   [1, 4],.  "veri
+0000ad00: 6679 4174 5374 6172 7422 3a20 5b22 7265  fyAtStart": ["re
+0000ad10: 6164 795f 7265 7375 6c74 732e 7478 7422  ady_results.txt"
+0000ad20: 5d2c 0a20 2022 7665 7269 6679 5761 6974  ],.  "verifyWait
+0000ad30: 223a 205b 2277 6169 745f 666f 725f 7265  ": ["wait_for_re
+0000ad40: 7375 6c74 732e 7478 7422 5d2c 0a20 2022  sults.txt"],.  "
+0000ad50: 776f 726b 6572 5461 6773 223a 205b 5d2c  workerTags": [],
+0000ad60: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+0000ad70: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+0000ad80: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
+0000ad90: 2020 7b7d 0a20 2020 2020 205d 0a20 2020    {}.      ].   
+0000ada0: 207d 0a20 205d 0a7d 0a0a 6060 600a 0a23   }.  ].}..```..#
+0000adb0: 2323 204a 534f 4e20 5072 6f70 6572 7469  ## JSON Properti
+0000adc0: 6573 2061 7420 7468 6520 5461 736b 2047  es at the Task G
+0000add0: 726f 7570 204c 6576 656c 0a0a 5368 6f77  roup Level..Show
+0000ade0: 696e 6720 616c 6c20 706f 7373 6962 6c65  ing all possible
+0000adf0: 2070 726f 7065 7274 6965 7320 6174 2074   properties at t
+0000ae00: 6865 2054 6173 6b20 4772 6f75 7020 6c65  he Task Group le
+0000ae10: 7665 6c3a 0a0a 6060 606a 736f 6e0a 7b0a  vel:..```json.{.
+0000ae20: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
+0000ae30: 5b0a 2020 2020 7b0a 2020 2020 2020 2261  [.    {.      "a
+0000ae40: 7267 756d 656e 7473 223a 205b 312c 2022  rguments": [1, "
+0000ae50: 5457 4f22 5d2c 0a20 2020 2020 2022 6361  TWO"],.      "ca
+0000ae60: 7074 7572 6554 6173 6b4f 7574 7075 7422  ptureTaskOutput"
+0000ae70: 3a20 7472 7565 2c0a 2020 2020 2020 2263  : true,.      "c
+0000ae80: 6f6d 706c 6574 6564 5461 736b 5474 6c22  ompletedTaskTtl"
+0000ae90: 3a20 3130 2c0a 2020 2020 2020 2264 6f63  : 10,.      "doc
+0000aea0: 6b65 7245 6e76 6972 6f6e 6d65 6e74 223a  kerEnvironment":
+0000aeb0: 207b 224d 595f 444f 434b 4552 5f56 4152   {"MY_DOCKER_VAR
+0000aec0: 223a 2031 3030 7d2c 0a20 2020 2020 2022  ": 100},.      "
+0000aed0: 646f 636b 6572 5061 7373 776f 7264 223a  dockerPassword":
+0000aee0: 2022 6d79 5061 7373 776f 7264 222c 0a20   "myPassword",. 
+0000aef0: 2020 2020 2022 646f 636b 6572 5573 6572       "dockerUser
+0000af00: 6e61 6d65 223a 2022 6d79 5573 6572 6e61  name": "myUserna
+0000af10: 6d65 222c 0a20 2020 2020 2022 656e 7669  me",.      "envi
+0000af20: 726f 6e6d 656e 7422 3a20 7b22 4d59 5f56  ronment": {"MY_V
+0000af30: 4152 223a 2031 3030 7d2c 0a20 2020 2020  AR": 100},.     
+0000af40: 2022 6578 636c 7573 6976 6557 6f72 6b65   "exclusiveWorke
+0000af50: 7273 223a 2066 616c 7365 2c0a 2020 2020  rs": false,.    
+0000af60: 2020 2265 7865 6375 7461 626c 6522 3a20    "executable": 
+0000af70: 226d 792d 636f 6e74 6169 6e65 7222 2c0a  "my-container",.
+0000af80: 2020 2020 2020 2266 696e 6973 6849 6641        "finishIfA
+0000af90: 6c6c 5461 736b 7346 696e 6973 6865 6422  llTasksFinished"
+0000afa0: 3a20 7472 7565 2c0a 2020 2020 2020 2266  : true,.      "f
+0000afb0: 696e 6973 6849 6641 6e79 5461 736b 4661  inishIfAnyTaskFa
+0000afc0: 696c 6564 223a 2066 616c 7365 2c0a 2020  iled": false,.  
+0000afd0: 2020 2020 2266 6c61 7474 656e 496e 7075      "flattenInpu
+0000afe0: 7450 6174 6873 223a 2066 616c 7365 2c0a  tPaths": false,.
+0000aff0: 2020 2020 2020 2269 6e70 7574 7322 3a20        "inputs": 
+0000b000: 5b22 6170 702f 6d61 696e 2e70 7922 2c20  ["app/main.py", 
+0000b010: 2261 7070 2f72 6571 7569 7265 6d65 6e74  "app/requirement
+0000b020: 732e 7478 7422 5d2c 0a20 2020 2020 2022  s.txt"],.      "
+0000b030: 696e 7075 7473 4f70 7469 6f6e 616c 223a  inputsOptional":
+0000b040: 205b 226f 7074 696f 6e61 6c2e 7478 7422   ["optional.txt"
+0000b050: 5d2c 0a20 2020 2020 2022 696e 7374 616e  ],.      "instan
+0000b060: 6365 5479 7065 7322 3a20 5b22 7433 612e  ceTypes": ["t3a.
+0000b070: 6d69 6372 6f22 2c20 2274 332e 6d69 6372  micro", "t3.micr
+0000b080: 6f22 5d2c 0a20 2020 2020 2022 6d61 7869  o"],.      "maxi
+0000b090: 6d75 6d54 6173 6b52 6574 7269 6573 223a  mumTaskRetries":
+0000b0a0: 2030 2c0a 2020 2020 2020 226d 6178 576f   0,.      "maxWo
+0000b0b0: 726b 6572 7322 3a20 312c 0a20 2020 2020  rkers": 1,.     
+0000b0c0: 2022 6d69 6e57 6f72 6b65 7273 223a 2031   "minWorkers": 1
+0000b0d0: 2c0a 2020 2020 2020 226e 616d 6522 3a20  ,.      "name": 
+0000b0e0: 2266 6972 7374 2d74 6173 6b2d 6772 6f75  "first-task-grou
+0000b0f0: 7022 2c0a 2020 2020 2020 226f 7574 7075  p",.      "outpu
+0000b100: 7473 223a 205b 2272 6573 756c 7473 2e74  ts": ["results.t
+0000b110: 7874 225d 2c0a 2020 2020 2020 226f 7574  xt"],.      "out
+0000b120: 7075 7473 5265 7175 6972 6564 223a 205b  putsRequired": [
+0000b130: 2272 6573 756c 7473 5f72 6571 7569 7265  "results_require
+0000b140: 642e 7478 7422 5d2c 0a20 2020 2020 2022  d.txt"],.      "
+0000b150: 7072 696f 7269 7479 223a 2030 2e30 2c0a  priority": 0.0,.
+0000b160: 2020 2020 2020 2270 726f 7669 6465 7273        "providers
+0000b170: 223a 205b 2241 5753 225d 2c0a 2020 2020  ": ["AWS"],.    
+0000b180: 2020 2272 616d 223a 205b 302e 352c 2032    "ram": [0.5, 2
+0000b190: 5d2c 0a20 2020 2020 2022 7265 6769 6f6e  ],.      "region
+0000b1a0: 7322 3a20 5b22 6575 2d77 6573 742d 3222  s": ["eu-west-2"
+0000b1b0: 5d2c 0a20 2020 2020 2022 7461 736b 436f  ],.      "taskCo
+0000b1c0: 756e 7422 3a20 352c 0a20 2020 2020 2022  unt": 5,.      "
+0000b1d0: 7461 736b 4461 7461 223a 2022 6d79 5f74  taskData": "my_t
+0000b1e0: 6173 6b5f 6461 7461 5f73 7472 696e 6722  ask_data_string"
+0000b1f0: 2c0a 2020 2020 2020 2274 6173 6b44 6174  ,.      "taskDat
+0000b200: 6146 696c 6522 3a20 226d 795f 6461 7461  aFile": "my_data
+0000b210: 5f66 696c 652e 7478 7422 2c0a 2020 2020  _file.txt",.    
+0000b220: 2020 2274 6173 6b54 7970 6573 223a 205b    "taskTypes": [
+0000b230: 2264 6f63 6b65 7222 5d2c 0a20 2020 2020  "docker"],.     
+0000b240: 2022 7461 736b 7350 6572 576f 726b 6572   "tasksPerWorker
+0000b250: 223a 2031 2c0a 2020 2020 2020 2275 706c  ": 1,.      "upl
+0000b260: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
+0000b270: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
+0000b280: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
+0000b290: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
+0000b2a0: 7422 7d5d 2c0a 2020 2020 2020 2276 6370  t"}],.      "vcp
+0000b2b0: 7573 223a 205b 312c 2034 5d2c 0a20 2020  us": [1, 4],.   
+0000b2c0: 2020 2022 7665 7269 6679 4174 5374 6172     "verifyAtStar
+0000b2d0: 7422 3a20 5b22 7265 6164 795f 7265 7375  t": ["ready_resu
+0000b2e0: 6c74 732e 7478 7422 5d2c 0a20 2020 2020  lts.txt"],.     
+0000b2f0: 2022 7665 7269 6679 5761 6974 223a 205b   "verifyWait": [
+0000b300: 2277 6169 745f 666f 725f 7265 7375 6c74  "wait_for_result
+0000b310: 732e 7478 7422 5d2c 0a20 2020 2020 2022  s.txt"],.      "
+0000b320: 776f 726b 6572 5461 6773 223a 205b 5d2c  workerTags": [],
+0000b330: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+0000b340: 5b0a 2020 2020 2020 2020 7b7d 0a20 2020  [.        {}.   
+0000b350: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
+0000b360: 7b0a 2020 2020 2020 226e 616d 6522 3a20  {.      "name": 
+0000b370: 2273 6563 6f6e 642d 7461 736b 2d67 726f  "second-task-gro
+0000b380: 7570 222c 0a20 2020 2020 2022 6465 7065  up",.      "depe
+0000b390: 6e64 656e 744f 6e22 3a20 2266 6972 7374  ndentOn": "first
+0000b3a0: 2d74 6173 6b2d 6772 6f75 7022 2c0a 2020  -task-group",.  
+0000b3b0: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
+0000b3c0: 2020 2020 2020 207b 7d0a 2020 2020 2020         {}.      
+0000b3d0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
+0000b3e0: 600a 0a23 2323 204a 534f 4e20 5072 6f70  `..### JSON Prop
+0000b3f0: 6572 7469 6573 2061 7420 7468 6520 5461  erties at the Ta
+0000b400: 736b 204c 6576 656c 0a0a 5368 6f77 696e  sk Level..Showin
+0000b410: 6720 616c 6c20 706f 7373 6962 6c65 2070  g all possible p
+0000b420: 726f 7065 7274 6965 7320 6174 2074 6865  roperties at the
+0000b430: 2054 6173 6b20 6c65 7665 6c3a 0a0a 6060   Task level:..``
+0000b440: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
+0000b450: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+0000b460: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+0000b470: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+0000b480: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+0000b490: 3a20 5b31 2c20 325d 2c0a 2020 2020 2020  : [1, 2],.      
+0000b4a0: 2020 2020 2263 6170 7475 7265 5461 736b      "captureTask
+0000b4b0: 4f75 7470 7574 223a 2074 7275 652c 0a20  Output": true,. 
+0000b4c0: 2020 2020 2020 2020 2022 646f 636b 6572           "docker
+0000b4d0: 456e 7669 726f 6e6d 656e 7422 3a20 7b22  Environment": {"
+0000b4e0: 4d59 5f44 4f43 4b45 525f 5641 5222 3a20  MY_DOCKER_VAR": 
+0000b4f0: 3130 307d 2c0a 2020 2020 2020 2020 2020  100},.          
+0000b500: 2264 6f63 6b65 7250 6173 7377 6f72 6422  "dockerPassword"
+0000b510: 3a20 226d 7950 6173 7377 6f72 6422 2c0a  : "myPassword",.
+0000b520: 2020 2020 2020 2020 2020 2264 6f63 6b65            "docke
+0000b530: 7255 7365 726e 616d 6522 3a20 226d 7955  rUsername": "myU
+0000b540: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
+0000b550: 2020 2020 2265 6e76 6972 6f6e 6d65 6e74      "environment
+0000b560: 223a 207b 224d 595f 5641 5222 3a20 3130  ": {"MY_VAR": 10
+0000b570: 307d 2c0a 2020 2020 2020 2020 2020 2265  0},.          "e
+0000b580: 7865 6375 7461 626c 6522 3a20 226d 792d  xecutable": "my-
+0000b590: 636f 6e74 6169 6e65 7222 2c0a 2020 2020  container",.    
+0000b5a0: 2020 2020 2020 2266 6c61 7474 656e 496e        "flattenIn
+0000b5b0: 7075 7450 6174 6873 223a 2066 616c 7365  putPaths": false
+0000b5c0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
+0000b5d0: 7574 7322 3a20 5b22 6170 702f 6d61 696e  uts": ["app/main
+0000b5e0: 2e70 7922 2c20 2261 7070 2f72 6571 7569  .py", "app/requi
+0000b5f0: 7265 6d65 6e74 732e 7478 7422 5d2c 0a20  rements.txt"],. 
+0000b600: 2020 2020 2020 2020 2022 696e 7075 7473           "inputs
+0000b610: 4f70 7469 6f6e 616c 223a 205b 226f 7074  Optional": ["opt
+0000b620: 696f 6e61 6c2e 7478 7422 5d2c 0a20 2020  ional.txt"],.   
+0000b630: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+0000b640: 6d79 2d74 6173 6b22 2c0a 2020 2020 2020  my-task",.      
+0000b650: 2020 2020 226f 7574 7075 7473 223a 205b      "outputs": [
+0000b660: 2272 6573 756c 7473 2e74 7874 225d 2c0a  "results.txt"],.
+0000b670: 2020 2020 2020 2020 2020 226f 7574 7075            "outpu
+0000b680: 7473 5265 7175 6972 6564 223a 205b 2272  tsRequired": ["r
+0000b690: 6573 756c 7473 5f72 6571 7569 7265 642e  esults_required.
+0000b6a0: 7478 7422 5d2c 0a20 2020 2020 2020 2020  txt"],.         
+0000b6b0: 2022 7461 736b 4461 7461 223a 2022 6d79   "taskData": "my
+0000b6c0: 5f74 6173 6b5f 6461 7461 5f73 7472 696e  _task_data_strin
+0000b6d0: 6722 2c0a 2020 2020 2020 2020 2020 2274  g",.          "t
+0000b6e0: 6173 6b44 6174 6146 696c 6522 3a20 226d  askDataFile": "m
+0000b6f0: 795f 6461 7461 5f66 696c 652e 7478 7422  y_data_file.txt"
+0000b700: 2c0a 2020 2020 2020 2020 2020 2274 6173  ,.          "tas
+0000b710: 6b54 7970 6522 3a20 2264 6f63 6b65 7222  kType": "docker"
+0000b720: 2c0a 2020 2020 2020 2020 2020 2275 706c  ,.          "upl
+0000b730: 6f61 6446 696c 6573 223a 205b 7b22 6c6f  oadFiles": [{"lo
+0000b740: 6361 6c50 6174 6822 3a20 2266 696c 655f  calPath": "file_
+0000b750: 312e 7478 7422 2c20 2275 706c 6f61 6450  1.txt", "uploadP
+0000b760: 6174 6822 3a20 2266 696c 655f 312e 7478  ath": "file_1.tx
+0000b770: 7422 7d5d 2c0a 2020 2020 2020 2020 2020  t"}],.          
+0000b780: 2276 6572 6966 7941 7453 7461 7274 223a  "verifyAtStart":
+0000b790: 205b 2272 6561 6479 5f72 6573 756c 7473   ["ready_results
+0000b7a0: 2e74 7874 225d 2c0a 2020 2020 2020 2020  .txt"],.        
+0000b7b0: 2020 2276 6572 6966 7957 6169 7422 3a20    "verifyWait": 
+0000b7c0: 5b22 7761 6974 5f66 6f72 5f72 6573 756c  ["wait_for_resul
+0000b7d0: 7473 2e74 7874 225d 0a20 2020 2020 2020  ts.txt"].       
+0000b7e0: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
+0000b7f0: 0a20 205d 0a7d 0a60 6060 0a0a 2323 2056  .  ].}.```..## V
+0000b800: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
+0000b810: 7469 6f6e 7320 696e 2057 6f72 6b20 5265  tions in Work Re
+0000b820: 7175 6972 656d 656e 7420 5072 6f70 6572  quirement Proper
+0000b830: 7469 6573 0a0a 5661 7269 6162 6c65 2073  ties..Variable s
+0000b840: 7562 7374 6974 7574 696f 6e73 2063 616e  ubstitutions can
+0000b850: 2062 6520 7573 6564 2077 6974 6869 6e20   be used within 
+0000b860: 616e 7920 7072 6f70 6572 7479 2076 616c  any property val
+0000b870: 7565 2069 6e20 544f 4d4c 2063 6f6e 6669  ue in TOML confi
+0000b880: 6775 7261 7469 6f6e 2066 696c 6573 206f  guration files o
+0000b890: 7220 576f 726b 2052 6571 7569 7265 6d65  r Work Requireme
+0000b8a0: 6e74 204a 534f 4e20 6669 6c65 732e 2053  nt JSON files. S
+0000b8b0: 6565 2074 6865 2064 6573 6372 6970 7469  ee the descripti
+0000b8c0: 6f6e 205b 6162 6f76 655d 2823 7661 7269  on [above](#vari
+0000b8d0: 6162 6c65 2d73 7562 7374 6974 7574 696f  able-substitutio
+0000b8e0: 6e73 2920 666f 7220 6d6f 7265 2064 6574  ns) for more det
+0000b8f0: 6169 6c73 206f 6e20 7661 7269 6162 6c65  ails on variable
+0000b900: 2073 7562 7374 6974 7574 696f 6e73 2e20   substitutions. 
+0000b910: 5468 6973 2069 7320 6120 706f 7765 7266  This is a powerf
+0000b920: 756c 2066 6561 7475 7265 2074 6861 7420  ul feature that 
+0000b930: 616c 6c6f 7773 2057 6f72 6b20 5265 7175  allows Work Requ
+0000b940: 6972 656d 656e 7473 2074 6f20 6265 2070  irements to be p
+0000b950: 6172 616d 6574 6572 6973 6564 2062 7920  arameterised by 
+0000b960: 7375 7070 6c79 696e 6720 7661 6c75 6573  supplying values
+0000b970: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
+0000b980: 6c69 6e65 2c20 7669 6120 656e 7669 726f  line, via enviro
+0000b990: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+0000b9a0: 6f72 2076 6961 2074 6865 2054 4f4d 4c20  or via the TOML 
+0000b9b0: 6669 6c65 2e0a 0a23 2323 2054 6173 6b20  file...### Task 
+0000b9c0: 616e 6420 5461 736b 2047 726f 7570 204e  and Task Group N
+0000b9d0: 616d 6520 5375 6273 7469 7475 7469 6f6e  ame Substitution
+0000b9e0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
+0000b9f0: 6e75 6d62 6572 696e 6720 616e 6420 6e61  numbering and na
+0000ba00: 6d69 6e67 2073 7562 7374 6974 7574 696f  ming substitutio
+0000ba10: 6e73 2061 7265 2061 7661 696c 6162 6c65  ns are available
+0000ba20: 2066 6f72 2075 7365 2069 6e20 5461 736b   for use in Task
+0000ba30: 2061 6e64 2054 6173 6b20 4772 6f75 7020   and Task Group 
+0000ba40: 6e61 6d69 6e67 2c20 6f6e 6c79 2077 6865  naming, only whe
+0000ba50: 6e20 7468 6520 576f 726b 2052 6571 7569  n the Work Requi
+0000ba60: 7265 6d65 6e74 2069 7320 7370 6563 6966  rement is specif
+0000ba70: 6965 6420 6173 2020 4a53 4f4e 2064 6f63  ied as  JSON doc
+0000ba80: 756d 656e 742c 2069 2e65 2e2c 2074 6865  ument, i.e., the
+0000ba90: 7920 6361 6e20 6265 2075 7365 6420 696e  y can be used in
+0000baa0: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
+0000bab0: 6572 7469 6573 2066 6f72 2054 6173 6b73  erties for Tasks
+0000bac0: 2061 6e64 2054 6173 6b20 4772 6f75 7073   and Task Groups
+0000bad0: 2069 6e20 4a53 4f4e 2073 7065 6369 6669   in JSON specifi
+0000bae0: 6361 7469 6f6e 732e 0a0a 5468 6520 666f  cations...The fo
+0000baf0: 6c6c 6f77 696e 6720 7461 626c 6520 6465  llowing table de
+0000bb00: 6669 6e65 7320 7468 6520 636f 6e74 6578  fines the contex
+0000bb10: 7428 7329 2069 6e20 7768 6963 6820 6561  t(s) in which ea
+0000bb20: 6368 2076 6172 6961 626c 6520 6361 6e20  ch variable can 
+0000bb30: 6265 2075 7365 643a 0a0a 7c20 4469 7265  be used:..| Dire
+0000bb40: 6374 6976 6520 2020 2020 2020 2020 2020  ctive           
+0000bb50: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
+0000bb60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
 0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb80: 2020 2020 2020 2020 207c 2054 6173 6b20           | Task 
-0000bb90: 7c20 5461 736b 2047 726f 7570 207c 0a7c  | Task Group |.|
-0000bba0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-0000bbb0: 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  ---------|:-----
+0000bb80: 2020 2020 2020 2020 7c20 5461 736b 207c          | Task |
+0000bb90: 2054 6173 6b20 4772 6f75 7020 7c0a 7c3a   Task Group |.|:
+0000bba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bbb0: 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d  --------|:------
 0000bbc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000bbd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bbe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d  -------------|:-
-0000bbf0: 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ----|:----------
-0000bc00: 2d7c 0a7c 2060 7b7b 7461 736b 5f6e 756d  -|.| `{{task_num
-0000bc10: 6265 727d 7d60 2020 2020 2020 207c 2054  ber}}`       | T
-0000bc20: 6865 2063 7572 7265 6e74 2054 6173 6b20  he current Task 
-0000bc30: 6e75 6d62 6572 2020 2020 2020 2020 2020  number          
+0000bbe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
+0000bbf0: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
+0000bc00: 7c0a 7c20 607b 7b74 6173 6b5f 6e75 6d62  |.| `{{task_numb
+0000bc10: 6572 7d7d 6020 2020 2020 2020 7c20 5468  er}}`       | Th
+0000bc20: 6520 6375 7272 656e 7420 5461 736b 206e  e current Task n
+0000bc30: 756d 6265 7220 2020 2020 2020 2020 2020  umber           
 0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 207c 2059 6573 2020 7c20 2020 2020 2020   | Yes  |       
-0000bc60: 2020 2020 207c 0a7c 2060 7b7b 7461 736b       |.| `{{task
-0000bc70: 5f6e 616d 657d 7d60 2020 2020 2020 2020  _name}}`        
-0000bc80: 207c 2054 6865 2063 7572 7265 6e74 2054   | The current T
-0000bc90: 6173 6b20 6e61 6d65 2020 2020 2020 2020  ask name        
+0000bc50: 7c20 5965 7320 207c 2020 2020 2020 2020  | Yes  |        
+0000bc60: 2020 2020 7c0a 7c20 607b 7b74 6173 6b5f      |.| `{{task_
+0000bc70: 6e61 6d65 7d7d 6020 2020 2020 2020 2020  name}}`         
+0000bc80: 7c20 5468 6520 6375 7272 656e 7420 5461  | The current Ta
+0000bc90: 736b 206e 616d 6520 2020 2020 2020 2020  sk name         
 0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 2020 2020 207c 2059 6573 2020 7c20 2020       | Yes  |   
-0000bcc0: 2020 2020 2020 2020 207c 0a7c 2060 7b7b           |.| `{{
-0000bcd0: 7461 736b 5f67 726f 7570 5f6e 616d 657d  task_group_name}
-0000bce0: 7d60 2020 207c 2054 6865 2063 7572 7265  }`   | The curre
-0000bcf0: 6e74 2054 6173 6b20 4772 6f75 7020 6e61  nt Task Group na
-0000bd00: 6d65 2020 2020 2020 2020 2020 2020 2020  me              
-0000bd10: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-0000bd20: 7c20 2020 2020 2020 2020 2020 207c 0a7c  |            |.|
-0000bd30: 2060 7b7b 7461 736b 5f63 6f75 6e74 7d7d   `{{task_count}}
-0000bd40: 6020 2020 2020 2020 207c 2054 6865 206e  `        | The n
-0000bd50: 756d 6265 7220 6f66 2054 6173 6b73 2069  umber of Tasks i
-0000bd60: 6e20 7468 6520 6375 7272 656e 7420 5461  n the current Ta
-0000bd70: 736b 2047 726f 7570 2020 2020 207c 2059  sk Group     | Y
-0000bd80: 6573 2020 7c20 5965 7320 2020 2020 2020  es  | Yes       
-0000bd90: 207c 0a7c 2060 7b7b 7461 736b 5f67 726f   |.| `{{task_gro
-0000bda0: 7570 5f6e 756d 6265 727d 7d60 207c 2054  up_number}}` | T
-0000bdb0: 6865 2063 7572 7265 6e74 2054 6173 6b20  he current Task 
-0000bdc0: 4772 6f75 7020 6e75 6d62 6572 2020 2020  Group number    
+0000bcb0: 2020 2020 7c20 5965 7320 207c 2020 2020      | Yes  |    
+0000bcc0: 2020 2020 2020 2020 7c0a 7c20 607b 7b74          |.| `{{t
+0000bcd0: 6173 6b5f 6772 6f75 705f 6e61 6d65 7d7d  ask_group_name}}
+0000bce0: 6020 2020 7c20 5468 6520 6375 7272 656e  `   | The curren
+0000bcf0: 7420 5461 736b 2047 726f 7570 206e 616d  t Task Group nam
+0000bd00: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+0000bd10: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+0000bd20: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0000bd30: 607b 7b74 6173 6b5f 636f 756e 747d 7d60  `{{task_count}}`
+0000bd40: 2020 2020 2020 2020 7c20 5468 6520 6e75          | The nu
+0000bd50: 6d62 6572 206f 6620 5461 736b 7320 696e  mber of Tasks in
+0000bd60: 2074 6865 2063 7572 7265 6e74 2054 6173   the current Tas
+0000bd70: 6b20 4772 6f75 7020 2020 2020 7c20 5965  k Group     | Ye
+0000bd80: 7320 207c 2059 6573 2020 2020 2020 2020  s  | Yes        
+0000bd90: 7c0a 7c20 607b 7b74 6173 6b5f 6772 6f75  |.| `{{task_grou
+0000bda0: 705f 6e75 6d62 6572 7d7d 6020 7c20 5468  p_number}}` | Th
+0000bdb0: 6520 6375 7272 656e 7420 5461 736b 2047  e current Task G
+0000bdc0: 726f 7570 206e 756d 6265 7220 2020 2020  roup number     
 0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 207c 2059 6573 2020 7c20 5965 7320 2020   | Yes  | Yes   
-0000bdf0: 2020 2020 207c 0a7c 2060 7b7b 7461 736b       |.| `{{task
-0000be00: 5f67 726f 7570 5f63 6f75 6e74 7d7d 6020  _group_count}}` 
-0000be10: 207c 2054 6865 206e 756d 6265 7220 6f66   | The number of
-0000be20: 2054 6173 6b20 4772 6f75 7073 2069 6e20   Task Groups in 
-0000be30: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000be40: 6d65 6e74 207c 2059 6573 2020 7c20 5965  ment | Yes  | Ye
-0000be50: 7320 2020 2020 2020 207c 0a0a 496e 2061  s        |..In a
-0000be60: 6464 6974 696f 6e2c 202a 2a54 6173 6b73  ddition, **Tasks
-0000be70: 2a2a 2064 6566 696e 6564 2069 6e20 4a53  ** defined in JS
-0000be80: 4f4e 2064 6f63 756d 656e 7473 2063 616e  ON documents can
-0000be90: 2075 7365 2061 6e79 206f 6620 7468 6520   use any of the 
-0000bea0: 7375 6273 7469 7475 7469 6f6e 7320 6162  substitutions ab
-0000beb0: 6f76 6520 696e 2061 6e79 206f 6620 7468  ove in any of th
-0000bec0: 6569 7220 7072 6f70 6572 7469 6573 2c20  eir properties, 
-0000bed0: 6e6f 7420 6a75 7374 2060 6e61 6d65 602e  not just `name`.
-0000bee0: 0a0a 4e75 6d62 6572 7320 6172 6520 7a65  ..Numbers are ze
-0000bef0: 726f 2d70 6164 6465 6420 666f 7220 6e65  ro-padded for ne
-0000bf00: 6174 2066 6f72 6d61 7474 696e 6720 616e  at formatting an
-0000bf10: 6420 736f 7274 696e 672c 2065 2e67 2e2c  d sorting, e.g.,
-0000bf20: 2054 6173 6b20 6e75 6d62 6572 2060 3337   Task number `37
-0000bf30: 6020 6f66 2060 3130 3030 6020 5461 736b  ` of `1000` Task
-0000bf40: 7320 776f 756c 6420 6265 2073 7562 7374  s would be subst
-0000bf50: 6974 7574 6564 2061 7320 6030 3033 3760  ituted as `0037`
-0000bf60: 2e0a 0a41 7320 616e 2065 7861 6d70 6c65  ...As an example
-0000bf70: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
-0000bf80: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
-0000bf90: 656d 656e 743a 0a0a 6060 606a 736f 6e0a  ement:..```json.
-0000bfa0: 7b0a 2020 2274 6173 6b47 726f 7570 7322  {.  "taskGroups"
-0000bfb0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-0000bfc0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
-0000bfd0: 5f67 726f 7570 5f7b 7b74 6173 6b5f 6772  _group_{{task_gr
-0000bfe0: 6f75 705f 6e75 6d62 6572 7d7d 5f61 3122  oup_number}}_a1"
-0000bff0: 2c0a 2020 2020 2020 2265 7865 6375 7461  ,.      "executa
-0000c000: 626c 6522 3a20 2265 7831 2e73 6822 2c0a  ble": "ex1.sh",.
-0000c010: 2020 2020 2020 2274 6173 6b43 6f75 6e74        "taskCount
-0000c020: 223a 2032 2c0a 2020 2020 2020 2274 6173  ": 2,.      "tas
-0000c030: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
-0000c040: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
-0000c050: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
-0000c060: 736b 5f6e 756d 6265 727d 7d2d 6f66 2d7b  sk_number}}-of-{
-0000c070: 7b74 6173 6b5f 636f 756e 747d 7d22 2c0a  {task_count}}",.
-0000c080: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
-0000c090: 6f6e 6d65 6e74 223a 207b 2254 4153 4b5f  onment": {"TASK_
-0000c0a0: 4e55 4d42 4552 223a 2022 7b7b 7461 736b  NUMBER": "{{task
-0000c0b0: 5f6e 756d 6265 727d 7d22 7d0a 2020 2020  _number}}"}.    
-0000c0c0: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
-0000c0d0: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-0000c0e0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
-0000c0f0: 6b5f 6772 6f75 705f 7b7b 7461 736b 5f67  k_group_{{task_g
-0000c100: 726f 7570 5f6e 756d 6265 727d 7d5f 6231  roup_number}}_b1
-0000c110: 222c 0a20 2020 2020 2022 6578 6563 7574  ",.      "execut
-0000c120: 6162 6c65 223a 2022 6578 322e 7368 222c  able": "ex2.sh",
-0000c130: 0a20 2020 2020 2022 7461 736b 436f 756e  .      "taskCoun
-0000c140: 7422 3a20 322c 0a20 2020 2020 2022 7461  t": 2,.      "ta
-0000c150: 736b 7322 3a20 5b0a 2020 2020 2020 2020  sks": [.        
-0000c160: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
-0000c170: 6522 3a20 226d 795f 7461 736b 5f7b 7b74  e": "my_task_{{t
-0000c180: 6173 6b5f 6e75 6d62 6572 7d7d 2d6f 662d  ask_number}}-of-
-0000c190: 7b7b 7461 736b 5f63 6f75 6e74 7d7d 220a  {{task_count}}".
-0000c1a0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0000c1b0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
-0000c1c0: 600a 0a2e 2e2e 2077 6f75 6c64 2063 7265  `..... would cre
-0000c1d0: 6174 6520 5461 736b 2047 726f 7570 7320  ate Task Groups 
-0000c1e0: 6e61 6d65 6420 606d 795f 7461 736b 5f67  named `my_task_g
-0000c1f0: 726f 7570 5f31 5f61 3160 2061 6e64 2060  roup_1_a1` and `
-0000c200: 6d79 5f74 6173 6b5f 6772 6f75 705f 325f  my_task_group_2_
-0000c210: 6231 602c 2065 6163 6820 636f 6e74 6169  b1`, each contai
-0000c220: 6e69 6e67 2054 6173 6b73 206e 616d 6564  ning Tasks named
-0000c230: 2060 6d79 5f74 6173 6b5f 312d 6f66 2d32   `my_task_1-of-2
-0000c240: 602c 2060 6d79 5f74 6173 6b5f 322d 6f66  `, `my_task_2-of
-0000c250: 2d32 602e 0a0a 2323 2320 576f 726b 2052  -2`...### Work R
-0000c260: 6571 7569 7265 6d65 6e74 204e 616d 6520  equirement Name 
-0000c270: 5375 6273 7469 7475 7469 6f6e 0a0a 5468  Substitution..Th
-0000c280: 6520 6e61 6d65 206f 6620 7468 6520 576f  e name of the Wo
-0000c290: 726b 2052 6571 7569 7265 6d65 6e74 2069  rk Requirement i
-0000c2a0: 7473 656c 6620 6361 6e20 6265 2075 7365  tself can be use
-0000c2b0: 6420 7669 6120 7468 6520 7661 7269 6162  d via the variab
-0000c2c0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
-0000c2d0: 607b 7b77 725f 6e61 6d65 7d7d 602e 2054  `{{wr_name}}`. T
-0000c2e0: 6869 7320 6361 6e20 6265 2075 7365 6420  his can be used 
-0000c2f0: 616e 7977 6865 7265 2069 6e20 6120 544f  anywhere in a TO
-0000c300: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-0000c310: 2066 696c 6520 6f72 2069 6e20 6120 4a53   file or in a JS
-0000c320: 4f4e 2057 6f72 6b20 5265 7175 6972 656d  ON Work Requirem
-0000c330: 656e 742e 0a0a 2323 2044 7279 2d52 756e  ent...## Dry-Run
-0000c340: 6e69 6e67 2057 6f72 6b20 5265 7175 6972  ning Work Requir
-0000c350: 656d 656e 7420 5375 626d 6973 7369 6f6e  ement Submission
-0000c360: 730a 0a54 6f20 6578 616d 696e 6520 7468  s..To examine th
-0000c370: 6520 4a53 4f4e 2074 6861 7420 7769 6c6c  e JSON that will
-0000c380: 2061 6374 7561 6c6c 7920 6265 2073 656e   actually be sen
-0000c390: 7420 746f 2074 6865 2059 656c 6c6f 7744  t to the YellowD
-0000c3a0: 6f67 2041 5049 2061 6674 6572 2061 6c6c  og API after all
-0000c3b0: 2070 726f 6365 7373 696e 672c 2075 7365   processing, use
-0000c3c0: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
-0000c3d0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
-0000c3e0: 7469 6f6e 2077 6865 6e20 7275 6e6e 696e  tion when runnin
-0000c3f0: 6720 6079 642d 7375 626d 6974 602e 2054  g `yd-submit`. T
-0000c400: 6869 7320 7769 6c6c 2070 7269 6e74 2074  his will print t
-0000c410: 6865 2066 756c 6c79 2070 726f 6365 7373  he fully process
-0000c420: 6564 204a 534f 4e20 666f 7220 7468 6520  ed JSON for the 
-0000c430: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000c440: 2e20 4e6f 7468 696e 6720 7769 6c6c 2062  . Nothing will b
-0000c450: 6520 7375 626d 6974 7465 6420 746f 2074  e submitted to t
-0000c460: 6865 2050 6c61 7466 6f72 6d2e 0a0a 5468  he Platform...Th
-0000c470: 6520 6472 792d 7275 6e20 6973 2075 7365  e dry-run is use
-0000c480: 6675 6c20 666f 7220 696e 7370 6563 7469  ful for inspecti
-0000c490: 6e67 2074 6865 2072 6573 756c 7473 206f  ng the results o
-0000c4a0: 6620 616c 6c20 7468 6520 7072 6f63 6573  f all the proces
-0000c4b0: 7369 6e67 2074 6861 7427 7320 6265 656e  sing that's been
-0000c4c0: 2070 6572 666f 726d 6564 2e20 546f 2073   performed. To s
-0000c4d0: 7570 7072 6573 7320 616c 6c20 6f75 7470  uppress all outp
-0000c4e0: 7574 2065 7863 6570 7420 666f 7220 7468  ut except for th
-0000c4f0: 6520 4a53 4f4e 2069 7473 656c 662c 2075  e JSON itself, u
-0000c500: 7365 2074 6865 2060 2d2d 7175 6965 7460  se the `--quiet`
-0000c510: 2028 602d 7160 2920 636f 6d6d 616e 6420   (`-q`) command 
-0000c520: 6c69 6e65 206f 7074 696f 6e2e 0a0a 4e6f  line option...No
-0000c530: 7465 2074 6861 7420 7468 6520 6765 6e65  te that the gene
-0000c540: 7261 7465 6420 4a53 4f4e 2069 7320 6120  rated JSON is a 
-0000c550: 636f 6e73 6f6c 6964 6174 6564 2066 6f72  consolidated for
-0000c560: 6d20 6f66 2077 6861 7420 776f 756c 6420  m of what would 
-0000c570: 6265 2073 7562 6d69 7474 6564 2074 6f20  be submitted to 
-0000c580: 7468 6520 5965 6c6c 6f77 446f 6720 4150  the YellowDog AP
-0000c590: 492c 2061 6e64 2054 6173 6b73 2061 7265  I, and Tasks are
-0000c5a0: 2064 6566 696e 6564 2064 6972 6563 746c   defined directl
-0000c5b0: 7920 7769 7468 696e 2074 6865 6972 2054  y within their T
-0000c5c0: 6173 6b20 4772 6f75 7073 2066 6f72 2065  ask Groups for e
-0000c5d0: 6173 6520 6f66 2063 6f6d 7072 6568 656e  ase of comprehen
-0000c5e0: 7369 6f6e 2e20 496e 2061 6374 7561 6c20  sion. In actual 
-0000c5f0: 4150 4920 7375 626d 6973 7369 6f6e 732c  API submissions,
-0000c600: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-0000c610: 656d 656e 7420 7769 7468 2069 7473 2054  ement with its T
-0000c620: 6173 6b20 4772 6f75 7073 2069 7320 7375  ask Groups is su
-0000c630: 626d 6974 7465 6420 6669 7273 742c 2061  bmitted first, a
-0000c640: 6e64 2054 6173 6b73 2061 7265 2074 6865  nd Tasks are the
-0000c650: 6e20 6164 6465 6420 746f 2054 6173 6b20  n added to Task 
-0000c660: 4772 6f75 7073 2073 6570 6172 6174 656c  Groups separatel
-0000c670: 7920 696e 2073 7562 7365 7175 656e 7420  y in subsequent 
-0000c680: 4150 4920 6361 6c6c 732e 0a0a 4120 7369  API calls...A si
-0000c690: 6d70 6c65 2065 7861 6d70 6c65 206f 6620  mple example of 
-0000c6a0: 7468 6520 4a53 4f4e 206f 7574 7075 7420  the JSON output 
-0000c6b0: 6973 2073 686f 776e 2062 656c 6f77 2c20  is shown below, 
-0000c6c0: 7368 6f77 696e 6720 6120 576f 726b 2052  showing a Work R
-0000c6d0: 6571 7569 7265 6d65 6e74 2077 6974 6820  equirement with 
-0000c6e0: 6120 7369 6e67 6c65 2054 6173 6b20 4772  a single Task Gr
-0000c6f0: 6f75 702c 2063 6f6e 7461 696e 696e 6720  oup, containing 
-0000c700: 6120 7369 6e67 6c65 2054 6173 6b2e 0a0a  a single Task...
-0000c710: 6025 2079 642d 7375 626d 6974 202d 2d64  `% yd-submit --d
-0000c720: 7279 2d72 756e 202d 2d71 7569 6574 600a  ry-run --quiet`.
-0000c730: 6060 606a 736f 6e0a 7b0a 2020 2266 756c  ```json.{.  "ful
-0000c740: 6669 6c4f 6e53 7562 6d69 7422 3a20 6661  filOnSubmit": fa
-0000c750: 6c73 652c 0a20 2022 6e61 6d65 223a 2022  lse,.  "name": "
-0000c760: 7079 6578 2d62 6173 685f 3233 3031 3134  pyex-bash_230114
-0000c770: 2d30 3935 3530 342d 3533 6122 2c0a 2020  -095504-53a",.  
-0000c780: 226e 616d 6573 7061 6365 223a 2022 7079  "namespace": "py
-0000c790: 6578 616d 706c 6573 222c 0a20 2022 7072  examples",.  "pr
-0000c7a0: 696f 7269 7479 223a 2030 2c0a 2020 2274  iority": 0,.  "t
-0000c7b0: 6167 223a 2022 7079 6578 2d62 6173 6822  ag": "pyex-bash"
-0000c7c0: 2c0a 2020 2274 6173 6b47 726f 7570 7322  ,.  "taskGroups"
-0000c7d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-0000c7e0: 2266 696e 6973 6849 6641 6c6c 5461 736b  "finishIfAllTask
-0000c7f0: 7346 696e 6973 6865 6422 3a20 7472 7565  sFinished": true
-0000c800: 2c0a 2020 2020 2020 2266 696e 6973 6849  ,.      "finishI
-0000c810: 6641 6e79 5461 736b 4661 696c 6564 223a  fAnyTaskFailed":
-0000c820: 2066 616c 7365 2c0a 2020 2020 2020 226e   false,.      "n
-0000c830: 616d 6522 3a20 2274 6173 6b5f 6772 6f75  ame": "task_grou
-0000c840: 705f 3122 2c0a 2020 2020 2020 2270 7269  p_1",.      "pri
-0000c850: 6f72 6974 7922 3a20 302c 0a20 2020 2020  ority": 0,.     
-0000c860: 2022 7275 6e53 7065 6369 6669 6361 7469   "runSpecificati
-0000c870: 6f6e 223a 207b 0a20 2020 2020 2020 2022  on": {.        "
-0000c880: 6d61 7869 6d75 6d54 6173 6b52 6574 7269  maximumTaskRetri
-0000c890: 6573 223a 2030 2c0a 2020 2020 2020 2020  es": 0,.        
-0000c8a0: 2274 6173 6b54 7970 6573 223a 205b 2262  "taskTypes": ["b
-0000c8b0: 6173 6822 5d2c 0a20 2020 2020 2020 2022  ash"],.        "
-0000c8c0: 776f 726b 6572 5461 6773 223a 205b 2270  workerTags": ["p
-0000c8d0: 7965 782d 6261 7368 225d 0a20 2020 2020  yex-bash"].     
-0000c8e0: 207d 2c0a 2020 2020 2020 2274 6173 6b73   },.      "tasks
-0000c8f0: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
-0000c900: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-0000c910: 6e74 7322 3a20 5b22 7079 6578 2d62 6173  nts": ["pyex-bas
-0000c920: 685f 3233 3031 3134 2d30 3935 3530 342d  h_230114-095504-
-0000c930: 3533 612f 736c 6565 705f 7363 7269 7074  53a/sleep_script
-0000c940: 2e73 6822 5d2c 0a20 2020 2020 2020 2020  .sh"],.         
-0000c950: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-0000c960: 7b7d 2c0a 2020 2020 2020 2020 2020 2269  {},.          "i
-0000c970: 6e70 7574 7322 3a20 5b0a 2020 2020 2020  nputs": [.      
-0000c980: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0000c990: 2020 2020 2020 226f 626a 6563 744e 616d        "objectNam
-0000c9a0: 6550 6174 7465 726e 223a 2022 7079 6578  ePattern": "pyex
-0000c9b0: 2d62 6173 685f 3233 3031 3134 2d30 3935  -bash_230114-095
-0000c9c0: 3530 342d 3533 612f 736c 6565 705f 7363  504-53a/sleep_sc
-0000c9d0: 7269 7074 2e73 6822 2c0a 2020 2020 2020  ript.sh",.      
-0000c9e0: 2020 2020 2020 2020 2273 6f75 7263 6522          "source"
-0000c9f0: 3a20 2254 4153 4b5f 4e41 4d45 5350 4143  : "TASK_NAMESPAC
-0000ca00: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
-0000ca10: 2020 2276 6572 6966 6963 6174 696f 6e22    "verification"
-0000ca20: 3a20 2256 4552 4946 595f 5741 4954 220a  : "VERIFY_WAIT".
-0000ca30: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-0000ca40: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-0000ca50: 2020 2020 2022 6e61 6d65 223a 2022 7461       "name": "ta
-0000ca60: 736b 5f30 3122 2c0a 2020 2020 2020 2020  sk_01",.        
-0000ca70: 2020 226f 7574 7075 7473 223a 205b 0a20    "outputs": [. 
-0000ca80: 2020 2020 2020 2020 2020 207b 2261 6c77             {"alw
-0000ca90: 6179 7355 706c 6f61 6422 3a20 7472 7565  aysUpload": true
-0000caa0: 2c20 2272 6571 7569 7265 6422 3a20 6661  , "required": fa
-0000cab0: 6c73 652c 2022 736f 7572 6365 223a 2022  lse, "source": "
-0000cac0: 5052 4f43 4553 535f 4f55 5450 5554 227d  PROCESS_OUTPUT"}
-0000cad0: 0a20 2020 2020 2020 2020 205d 2c0a 2020  .          ],.  
-0000cae0: 2020 2020 2020 2020 2274 6173 6b54 7970          "taskTyp
-0000caf0: 6522 3a20 2262 6173 6822 0a20 2020 2020  e": "bash".     
-0000cb00: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
-0000cb10: 207d 0a20 205d 0a7d 0a60 6060 0a0a 2323   }.  ].}.```..##
-0000cb20: 2320 5375 626d 6974 7469 6e67 2027 5261  # Submitting 'Ra
-0000cb30: 7727 204a 534f 4e20 576f 726b 2052 6571  w' JSON Work Req
-0000cb40: 7569 7265 6d65 6e74 2053 7065 6369 6669  uirement Specifi
-0000cb50: 6361 7469 6f6e 730a 0a49 7427 7320 706f  cations..It's po
-0000cb60: 7373 6962 6c65 2074 6f20 7573 6520 7468  ssible to use th
-0000cb70: 6520 4a53 4f4e 206f 7574 7075 7420 6f66  e JSON output of
-0000cb80: 2060 7964 2d73 7562 6d69 7420 2d2d 6472   `yd-submit --dr
-0000cb90: 792d 7275 6e60 2028 7375 6368 2061 7320  y-run` (such as 
-0000cba0: 7468 6520 6578 616d 706c 6520 6162 6f76  the example abov
-0000cbb0: 6529 2061 7320 6120 7365 6c66 2d63 6f6e  e) as a self-con
-0000cbc0: 7461 696e 6564 2c20 6675 6c6c 792d 7370  tained, fully-sp
-0000cbd0: 6563 6966 6965 6420 576f 726b 2052 6571  ecified Work Req
-0000cbe0: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
-0000cbf0: 6361 7469 6f6e 2c20 7573 696e 6720 7468  cation, using th
-0000cc00: 6520 602d 2d6a 736f 6e2d 7261 7760 2028  e `--json-raw` (
-0000cc10: 6f72 2060 2d6a 6029 2063 6f6d 6d61 6e64  or `-j`) command
-0000cc20: 206c 696e 6520 6f70 7469 6f6e 2c20 692e   line option, i.
-0000cc30: 652e 3a20 6079 642d 7375 626d 6974 202d  e.: `yd-submit -
-0000cc40: 2d6a 736f 6e2d 7261 7720 3c66 696c 656e  -json-raw <filen
-0000cc50: 616d 652e 6a73 6f6e 3e60 2e0a 0a54 6869  ame.json>`...Thi
-0000cc60: 7320 7769 6c6c 2073 7562 6d69 7420 7468  s will submit th
-0000cc70: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-0000cc80: 6e74 2c20 7468 656e 2061 6464 2061 6c6c  nt, then add all
-0000cc90: 2074 6865 2073 7065 6369 6669 6564 2054   the specified T
-0000cca0: 6173 6b73 2e0a 0a4e 6f74 6520 7468 6174  asks...Note that
-0000ccb0: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-0000ccc0: 7475 7469 6f6e 7320 2a2a 6361 6e2a 2a20  tutions **can** 
-0000ccd0: 6265 2075 7365 6420 696e 2074 6865 2072  be used in the r
-0000cce0: 6177 204a 534f 4e20 6669 6c65 2c20 6a75  aw JSON file, ju
-0000ccf0: 7374 2061 7320 696e 2074 6865 206f 7468  st as in the oth
-0000cd00: 6572 2057 6f72 6b20 5265 7175 6972 656d  er Work Requirem
-0000cd10: 656e 7420 4a53 4f4e 2065 7861 6d70 6c65  ent JSON example
-0000cd20: 732c 2062 7574 2074 6865 7265 2069 7320  s, but there is 
-0000cd30: 6e6f 2070 726f 7065 7274 7920 696e 6865  no property inhe
-0000cd40: 7269 7461 6e63 652c 2069 6e63 6c75 6469  ritance, includi
-0000cd50: 6e67 2066 726f 6d20 7468 6520 605b 776f  ng from the `[wo
-0000cd60: 726b 5265 7175 6972 656d 656e 745d 6020  rkRequirement]` 
-0000cd70: 7365 6374 696f 6e20 6f66 2074 6865 2054  section of the T
-0000cd80: 4f4d 4c20 636f 6e66 6967 7572 6174 696f  OML configuratio
-0000cd90: 6e20 6f72 2066 726f 6d20 576f 726b 2052  n or from Work R
-0000cda0: 6571 7569 7265 6d65 6e74 2070 726f 7065  equirement prope
-0000cdb0: 7274 6965 7320 7375 7070 6c69 6564 206f  rties supplied o
-0000cdc0: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
-0000cdd0: 6e65 2e0a 0a4e 6f74 6520 7468 6174 2074  ne...Note that t
-0000cde0: 6865 7265 2069 7320 6e6f 2061 7574 6f6d  here is no autom
-0000cdf0: 6174 6963 2066 696c 6520 7570 6c6f 6164  atic file upload
-0000ce00: 2077 6865 6e20 7573 696e 6720 7468 6973   when using this
-0000ce10: 206f 7074 696f 6e2c 2073 6f20 616e 7920   option, so any 
-0000ce20: 6669 6c65 7320 7265 7175 6972 6564 2061  files required a
-0000ce30: 7420 7468 6520 7374 6172 7420 6f66 2074  t the start of t
-0000ce40: 6865 2074 6173 6b20 2873 7065 6369 6669  he task (specifi
-0000ce50: 6564 2075 7369 6e67 2060 5645 5249 4659  ed using `VERIFY
-0000ce60: 5f41 545f 5354 4152 5460 2920 6d75 7374  _AT_START`) must
-0000ce70: 2062 6520 7072 6573 656e 7420 6265 666f   be present befo
-0000ce80: 7265 2074 6865 2054 6173 6b73 2061 7265  re the Tasks are
-0000ce90: 2075 706c 6f61 6465 642c 206f 7220 7468   uploaded, or th
-0000cea0: 6520 5461 736b 7320 7769 6c6c 2066 6169  e Tasks will fai
-0000ceb0: 6c20 696d 6d65 6469 6174 656c 792e 2054  l immediately. T
-0000cec0: 6865 2060 7964 2d75 706c 6f61 6460 2063  he `yd-upload` c
-0000ced0: 6f6d 6d61 6e64 2063 616e 2062 6520 7573  ommand can be us
-0000cee0: 6564 2074 6f20 7570 6c6f 6164 2074 6865  ed to upload the
-0000cef0: 7365 2066 696c 6573 2c20 616e 6420 6079  se files, and `y
-0000cf00: 642d 7375 626d 6974 6020 7769 6c6c 2070  d-submit` will p
-0000cf10: 6175 7365 2074 6f20 616c 6c6f 7720 7468  ause to allow th
-0000cf20: 6973 2074 6f20 6861 7070 656e 2e0a 0a23  is to happen...#
-0000cf30: 2320 4669 6c65 2053 746f 7261 6765 204c  # File Storage L
-0000cf40: 6f63 6174 696f 6e73 2061 6e64 2046 696c  ocations and Fil
-0000cf50: 6520 5573 6167 650a 0a54 6869 7320 7365  e Usage..This se
-0000cf60: 6374 696f 6e20 6469 7363 7573 7365 7320  ction discusses 
-0000cf70: 686f 7720 746f 2075 706c 6f61 6420 6669  how to upload fi
-0000cf80: 6c65 7320 6672 6f6d 206c 6f63 616c 2073  les from local s
-0000cf90: 746f 7261 6765 2074 6f20 7468 6520 5965  torage to the Ye
-0000cfa0: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
-0000cfb0: 746f 7265 2c20 686f 7720 7468 6f73 6520  tore, how those 
-0000cfc0: 6669 6c65 7320 6172 6520 7472 616e 7366  files are transf
-0000cfd0: 6572 7265 6420 746f 2057 6f72 6b65 7220  erred to Worker 
-0000cfe0: 4e6f 6465 7320 666f 7220 5461 736b 2070  Nodes for Task p
-0000cff0: 726f 6365 7373 696e 672c 2068 6f77 2074  rocessing, how t
-0000d000: 6865 2072 6573 756c 7473 206f 6620 5461  he results of Ta
-0000d010: 736b 2070 726f 6365 7373 696e 6720 6172  sk processing ar
-0000d020: 6520 7265 7475 726e 6564 2062 7920 576f  e returned by Wo
-0000d030: 726b 6572 204e 6f64 6573 2c20 616e 6420  rker Nodes, and 
-0000d040: 686f 7720 6669 6c65 7320 6172 6520 7472  how files are tr
-0000d050: 616e 7366 6572 7265 6420 6261 636b 2066  ansferred back f
-0000d060: 726f 6d20 7468 6520 5965 6c6c 6f77 446f  rom the YellowDo
-0000d070: 6720 4f62 6a65 6374 2053 746f 7265 2074  g Object Store t
-0000d080: 6f20 6c6f 6361 6c20 7374 6f72 6167 652e  o local storage.
-0000d090: 0a0a 2323 2320 4669 6c65 7320 5570 6c6f  ..### Files Uplo
-0000d0a0: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
-0000d0b0: 6374 2053 746f 7265 2066 726f 6d20 4c6f  ct Store from Lo
-0000d0c0: 6361 6c20 5374 6f72 6167 650a 0a23 2323  cal Storage..###
-0000d0d0: 2320 4669 6c65 7320 696e 2074 6865 2060  # Files in the `
-0000d0e0: 696e 7075 7473 6020 4c69 7374 0a0a 5768  inputs` List..Wh
-0000d0f0: 656e 2061 2057 6f72 6b20 5265 7175 6972  en a Work Requir
-0000d100: 656d 656e 7420 6973 2073 7562 6d69 7474  ement is submitt
-0000d110: 6564 2075 7369 6e67 2060 7964 2d73 7562  ed using `yd-sub
-0000d120: 6d69 7460 2c20 6669 6c65 7320 6172 6520  mit`, files are 
-0000d130: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
-0000d140: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
-0000d150: 2053 746f 7265 2069 6620 7468 6579 2772   Store if they'r
-0000d160: 6520 696e 636c 7564 6564 2069 6e20 7468  e included in th
-0000d170: 6520 6c69 7374 206f 6620 6669 6c65 7320  e list of files 
-0000d180: 696e 2074 6865 2060 696e 7075 7473 6020  in the `inputs` 
-0000d190: 7072 6f70 6572 7479 2e20 2846 6f72 2074  property. (For t
-0000d1a0: 6865 2063 6173 6520 6f66 2074 6865 2060  he case of the `
-0000d1b0: 6261 7368 6020 5461 736b 2054 7970 652c  bash` Task Type,
-0000d1c0: 2074 6865 2073 6372 6970 7420 7370 6563   the script spec
-0000d1d0: 6966 6965 6420 696e 2074 6865 2060 6578  ified in the `ex
-0000d1e0: 6563 7574 6162 6c65 6020 7072 6f70 6572  ecutable` proper
-0000d1f0: 7479 2069 7320 616c 736f 2061 7574 6f6d  ty is also autom
-0000d200: 6174 6963 616c 6c79 2075 706c 6f61 6465  atically uploade
-0000d210: 6420 6173 2061 2063 6f6e 7665 6e69 656e  d as a convenien
-0000d220: 6365 2c20 6576 656e 2069 6620 6e6f 7420  ce, even if not 
-0000d230: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-0000d240: 6069 6e70 7574 7360 206c 6973 742e 290a  `inputs` list.).
-0000d250: 0a46 696c 6573 2061 7265 2075 706c 6f61  .Files are uploa
-0000d260: 6465 6420 746f 2074 6865 204e 616d 6573  ded to the Names
-0000d270: 7061 6365 2073 7065 6369 6669 6564 2069  pace specified i
-0000d280: 6e20 7468 6520 636f 6e66 6967 7572 6174  n the configurat
-0000d290: 696f 6e2e 2057 6974 6869 6e20 7468 6520  ion. Within the 
-0000d2a0: 4e61 6d65 7370 6163 652c 2065 6163 6820  Namespace, each 
-0000d2b0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000d2c0: 2068 6173 2061 2073 6570 6172 6174 6520   has a separate 
-0000d2d0: 666f 6c64 6572 2074 6861 7420 7368 6172  folder that shar
-0000d2e0: 6573 2074 6865 206e 616d 6520 6f66 2074  es the name of t
-0000d2f0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-0000d300: 656e 742c 2061 6e64 2069 6e20 7768 6963  ent, and in whic
-0000d310: 6820 616c 6c20 6669 6c65 7320 7265 6c61  h all files rela
-0000d320: 7465 6420 746f 2074 6865 2057 6f72 6b20  ted to the Work 
-0000d330: 5265 7175 6972 656d 656e 7420 6172 6520  Requirement are 
-0000d340: 7374 6f72 6564 2e0a 0a31 2e20 4669 6c65  stored...1. File
-0000d350: 7320 746f 2062 6520 7570 6c6f 6164 6564  s to be uploaded
-0000d360: 2074 6861 7420 6172 6520 696e 2074 6865   that are in the
-0000d370: 202a 2a73 616d 6520 6469 7265 6374 6f72   **same director
-0000d380: 7920 6173 2074 6865 2057 6f72 6b20 5265  y as the Work Re
-0000d390: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
-0000d3a0: 6963 6174 696f 6e2a 2a20 2874 6865 2054  ication** (the T
-0000d3b0: 4f4d 4c20 6f72 204a 534f 4e20 6669 6c65  OML or JSON file
-0000d3c0: 2920 6172 6520 7570 6c6f 6164 6564 2074  ) are uploaded t
-0000d3d0: 6f20 7468 6520 726f 6f74 206f 6620 7468  o the root of th
-0000d3e0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-0000d3f0: 6e74 2066 6f6c 6465 722e 0a0a 0a32 2e20  nt folder....2. 
-0000d400: 4669 6c65 7320 746f 2062 6520 7570 6c6f  Files to be uplo
-0000d410: 6164 6564 2074 6861 7420 6172 6520 696e  aded that are in
-0000d420: 202a 2a73 7562 6469 7265 6374 6f72 6965   **subdirectorie
-0000d430: 7320 6265 6c6f 7720 7468 6520 576f 726b  s below the Work
-0000d440: 2052 6571 7569 7265 6d65 6e74 2073 7065   Requirement spe
-0000d450: 6369 6669 6361 7469 6f6e 2c20 6f72 2077  cification, or w
-0000d460: 6865 7265 2061 6273 6f6c 7574 6520 7061  here absolute pa
-0000d470: 7468 6e61 6d65 7320 6172 6520 7375 7070  thnames are supp
-0000d480: 6c69 6564 2a2a 2061 7265 2070 6c61 6365  lied** are place
-0000d490: 6420 696e 2074 6865 204f 626a 6563 7420  d in the Object 
-0000d4a0: 5374 6f72 6520 696e 2064 6972 6563 746f  Store in directo
-0000d4b0: 7269 6573 2074 6861 7420 6d69 7272 6f72  ries that mirror
-0000d4c0: 2074 6865 6972 206c 6f63 616c 2073 746f   their local sto
-0000d4d0: 7261 6765 206c 6f63 6174 696f 6e73 2e0a  rage locations..
-0000d4e0: 0a0a 332e 2046 696c 6573 2074 6f20 6265  ..3. Files to be
-0000d4f0: 2075 706c 6f61 6465 6420 7468 6174 2061   uploaded that a
-0000d500: 7265 2069 6e20 2a2a 6469 7265 6374 6f72  re in **director
-0000d510: 6965 7320 7265 6c61 7469 7665 2074 6f20  ies relative to 
-0000d520: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000d530: 6d65 6e74 2073 7065 6369 6669 6361 7469  ment specificati
-0000d540: 6f6e 2c20 7573 696e 6720 602e 2e60 2072  on, using `..` r
-0000d550: 656c 6174 6976 6520 7061 7468 732a 2a20  elative paths** 
-0000d560: 6172 6520 706c 6163 6564 2069 6e20 4f62  are placed in Ob
-0000d570: 6a65 6374 2053 746f 7265 2064 6972 6563  ject Store direc
-0000d580: 746f 7269 6573 2069 6e20 7768 6963 6820  tories in which 
-0000d590: 7468 6520 602e 2e60 2070 6172 7473 206f  the `..` parts o
-0000d5a0: 6620 7468 6520 7061 7468 6e61 6d65 2061  f the pathname a
-0000d5b0: 7265 2072 6570 6c61 6365 6420 7769 7468  re replaced with
-0000d5c0: 2061 6e20 696e 7465 6765 7220 636f 756e   an integer coun
-0000d5d0: 7420 6f66 2074 6865 206e 756d 6265 7220  t of the number 
-0000d5e0: 6f66 2060 2e2e 6020 656e 7472 6965 7320  of `..` entries 
-0000d5f0: 2862 6563 6175 7365 2077 6520 6361 6e27  (because we can'
-0000d600: 7420 7573 6520 7468 6520 602e 2e60 2072  t use the `..` r
-0000d610: 656c 6174 6976 6520 666f 726d 2069 6e20  elative form in 
-0000d620: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
-0000d630: 292e 0a0a 4173 7375 6d69 6e67 2061 204e  )...Assuming a N
-0000d640: 616d 6573 7061 6365 2063 616c 6c65 6420  amespace called 
-0000d650: 6064 6576 656c 6f70 6d65 6e74 6020 616e  `development` an
-0000d660: 6420 6120 576f 726b 2052 6571 7569 7265  d a Work Require
-0000d670: 6d65 6e74 206e 616d 6564 2060 7465 7374  ment named `test
-0000d680: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000d690: 342d 3764 3260 2c20 7468 6520 666f 6c6c  4-7d2`, the foll
-0000d6a0: 6f77 696e 6720 6c6f 6361 7469 6f6e 7320  owing locations 
-0000d6b0: 6172 6520 7573 6564 2077 6865 6e20 7570  are used when up
-0000d6c0: 6c6f 6164 696e 6720 6669 6c65 7320 666f  loading files fo
-0000d6d0: 6c6c 6f77 696e 6720 7468 6520 7061 7474  llowing the patt
-0000d6e0: 6572 6e73 2061 626f 7665 3a0a 0a60 6060  erns above:..```
-0000d6f0: 7368 656c 6c0a 2269 6e70 7574 7322 203a  shell."inputs" :
-0000d700: 205b 2266 696c 655f 312e 7478 7422 5d20   ["file_1.txt"] 
-0000d710: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
-0000d720: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
-0000d730: 3230 3430 342d 3764 322f 6669 6c65 5f31  20404-7d2/file_1
-0000d740: 2e74 7874 0a22 696e 7075 7473 2220 3a20  .txt."inputs" : 
-0000d750: 5b22 6465 762f 6669 6c65 5f31 2e74 7874  ["dev/file_1.txt
-0000d760: 225d 202d 3e20 6465 7665 6c6f 706d 656e  "] -> developmen
-0000d770: 743a 3a74 6573 7472 756e 5f32 3231 3130  t::testrun_22110
-0000d780: 382d 3132 3034 3034 2d37 6432 2f64 6576  8-120404-7d2/dev
-0000d790: 2f66 696c 655f 312e 7478 740a 2269 6e70  /file_1.txt."inp
-0000d7a0: 7574 7322 203a 205b 222f 686f 6d65 2f64  uts" : ["/home/d
-0000d7b0: 6576 2f66 696c 655f 312e 7478 7422 5d20  ev/file_1.txt"] 
-0000d7c0: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
-0000d7d0: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
-0000d7e0: 3230 3430 342d 3764 322f 686f 6d65 2f64  20404-7d2/home/d
-0000d7f0: 6576 2f66 696c 655f 312e 7478 740a 2269  ev/file_1.txt."i
-0000d800: 6e70 7574 7322 203a 205b 222e 2e2f 6465  nputs" : ["../de
-0000d810: 762f 6669 6c65 5f31 2e74 7874 225d 202d  v/file_1.txt"] -
-0000d820: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
-0000d830: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000d840: 3034 3034 2d37 6432 2f31 2f64 6576 2f66  0404-7d2/1/dev/f
-0000d850: 696c 655f 312e 7478 740a 2269 6e70 7574  ile_1.txt."input
-0000d860: 7322 203a 205b 222e 2e2f 2e2e 2f64 6576  s" : ["../../dev
-0000d870: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
-0000d880: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
-0000d890: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
-0000d8a0: 3430 342d 3764 322f 322f 6465 762f 6669  404-7d2/2/dev/fi
-0000d8b0: 6c65 5f31 2e74 7874 0a60 6060 0a0a 2a2a  le_1.txt.```..**
-0000d8c0: 5573 696e 6720 6066 6c61 7474 656e 5570  Using `flattenUp
-0000d8d0: 6c6f 6164 5061 7468 7360 2a2a 0a0a 5468  loadPaths`**..Th
-0000d8e0: 6520 6066 6c61 7474 656e 5570 6c6f 6164  e `flattenUpload
-0000d8f0: 5061 7468 7360 2070 726f 7065 7274 7920  Paths` property 
-0000d900: 6361 6e20 6265 2075 7365 6420 746f 2073  can be used to s
-0000d910: 7570 7072 6573 7320 7468 6520 6d69 7272  uppress the mirr
-0000d920: 6f72 696e 6720 6f66 2061 6e79 206c 6f63  oring of any loc
-0000d930: 616c 2064 6972 6563 746f 7279 2073 7472  al directory str
-0000d940: 7563 7475 7265 2077 6865 6e20 7570 6c6f  ucture when uplo
-0000d950: 6164 696e 6720 6669 6c65 7320 746f 2074  ading files to t
-0000d960: 6865 204f 626a 6563 7420 5374 6f72 652e  he Object Store.
-0000d970: 2049 6620 7365 7420 746f 2060 7472 7565   If set to `true
-0000d980: 602c 2061 6c6c 2066 696c 6573 2077 696c  `, all files wil
-0000d990: 6c20 6265 2075 706c 6f61 6465 6420 746f  l be uploaded to
-0000d9a0: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
-0000d9b0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-0000d9c0: 7420 666f 6c64 6572 2e20 466f 7220 6578  t folder. For ex
-0000d9d0: 616d 706c 653a 0a0a 6060 6073 6865 6c6c  ample:..```shell
-0000d9e0: 0a22 696e 7075 7473 2220 3a20 5b22 6669  ."inputs" : ["fi
-0000d9f0: 6c65 5f31 2e74 7874 225d 202d 3e20 6465  le_1.txt"] -> de
-0000da00: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
-0000da10: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
-0000da20: 2d37 6432 2f66 696c 655f 312e 7478 740a  -7d2/file_1.txt.
-0000da30: 2269 6e70 7574 7322 203a 205b 2264 6576  "inputs" : ["dev
-0000da40: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
-0000da50: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
-0000da60: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
-0000da70: 3430 342d 3764 322f 6669 6c65 5f31 2e74  404-7d2/file_1.t
-0000da80: 7874 0a22 696e 7075 7473 2220 3a20 5b22  xt."inputs" : ["
-0000da90: 2f68 6f6d 652f 6465 762f 6669 6c65 5f31  /home/dev/file_1
-0000daa0: 2e74 7874 225d 202d 3e20 6465 7665 6c6f  .txt"] -> develo
-0000dab0: 706d 656e 743a 3a74 6573 7472 756e 5f32  pment::testrun_2
-0000dac0: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
-0000dad0: 2f66 696c 655f 312e 7478 740a 2269 6e70  /file_1.txt."inp
-0000dae0: 7574 7322 203a 205b 222e 2e2f 6465 762f  uts" : ["../dev/
-0000daf0: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000db00: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
-0000db10: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
-0000db20: 3034 2d37 6432 2f66 696c 655f 312e 7478  04-7d2/file_1.tx
-0000db30: 740a 2269 6e70 7574 7322 203a 205b 222e  t."inputs" : [".
-0000db40: 2e2f 2e2e 2f64 6576 2f66 696c 655f 312e  ./../dev/file_1.
-0000db50: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
-0000db60: 6d65 6e74 3a3a 7465 7374 7275 6e5f 3232  ment::testrun_22
-0000db70: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
-0000db80: 6669 6c65 5f31 2e74 7874 0a60 6060 0a0a  file_1.txt.```..
-0000db90: 5468 6520 7072 6f70 6572 7479 2064 6566  The property def
-0000dba0: 6175 6c74 2069 7320 6066 616c 7365 602e  ault is `false`.
-0000dbb0: 2054 6869 7320 7072 6f70 6572 7479 202a   This property *
-0000dbc0: 2a63 616e 206f 6e6c 7920 6265 2073 6574  *can only be set
-0000dbd0: 2061 7420 7468 6520 576f 726b 2052 6571   at the Work Req
-0000dbe0: 7569 7265 6d65 6e74 206c 6576 656c 2a2a  uirement level**
-0000dbf0: 2061 6e64 2077 696c 6c20 7468 6572 6566   and will theref
-0000dc00: 6f72 6520 6170 706c 7920 746f 2061 6c6c  ore apply to all
-0000dc10: 2054 6173 6b20 4772 6f75 7073 2061 6e64   Task Groups and
-0000dc20: 2054 6173 6b73 2077 6974 6869 6e20 6120   Tasks within a 
-0000dc30: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000dc40: 2e0a 0a57 6865 6e20 6669 6c65 7320 6170  ...When files ap
-0000dc50: 7065 6172 2069 6e20 7468 6520 6069 6e70  pear in the `inp
-0000dc60: 7574 7360 206c 6973 742c 2074 6865 7920  uts` list, they 
-0000dc70: 6172 6520 616c 736f 2061 7574 6f6d 6174  are also automat
-0000dc80: 6963 616c 6c79 2061 6464 6564 2074 6f20  ically added to 
-0000dc90: 7468 6520 6c69 7374 206f 6620 6669 6c65  the list of file
-0000dca0: 7320 7265 7175 6972 6564 2062 7920 7468  s required by th
-0000dcb0: 6520 7265 6c65 7661 6e74 2054 6173 6b28  e relevant Task(
-0000dcc0: 7329 2061 7320 6056 6572 6966 7941 7453  s) as `VerifyAtS
-0000dcd0: 7461 7274 6020 6465 7065 6e64 656e 6369  tart` dependenci
-0000dce0: 6573 2e0a 0a23 2323 2320 4669 6c65 7320  es...#### Files 
-0000dcf0: 696e 2074 6865 2060 7570 6c6f 6164 4669  in the `uploadFi
-0000dd00: 6c65 7360 204c 6973 740a 0a54 6865 2060  les` List..The `
-0000dd10: 7570 6c6f 6164 4669 6c65 7360 2070 726f  uploadFiles` pro
-0000dd20: 7065 7274 7920 616c 6c6f 7773 206d 6f72  perty allows mor
-0000dd30: 6520 666c 6578 6962 6c65 2063 6f6e 7472  e flexible contr
-0000dd40: 6f6c 206f 7665 7220 7468 6520 6669 6c65  ol over the file
-0000dd50: 7320 746f 2062 6520 7570 6c6f 6164 6564  s to be uploaded
-0000dd60: 2066 726f 6d20 6c6f 6361 6c20 7374 6f72   from local stor
-0000dd70: 6167 6520 746f 2074 6865 204f 626a 6563  age to the Objec
-0000dd80: 7420 5374 6f72 6520 7768 656e 2060 7964  t Store when `yd
-0000dd90: 2d73 7562 6d69 7460 2069 7320 7275 6e2e  -submit` is run.
-0000dda0: 2054 6865 2070 726f 7065 7274 7920 6361   The property ca
-0000ddb0: 6e20 6265 2075 7365 6420 6174 2061 6c6c  n be used at all
-0000ddc0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-0000ddd0: 7420 6c65 7665 6c73 2c20 6672 6f6d 2074  t levels, from t
-0000dde0: 6865 2054 4f4d 4c20 6669 6c65 2074 6872  he TOML file thr
-0000ddf0: 6f75 6768 2074 6f20 696e 6469 7669 6475  ough to individu
-0000de00: 616c 2054 6173 6b20 7370 6563 6966 6963  al Task specific
-0000de10: 6174 696f 6e73 2e0a 0a54 6865 2070 726f  ations...The pro
-0000de20: 7065 7274 7920 6973 2073 7570 706c 6965  perty is supplie
-0000de30: 6420 6173 2061 206c 6973 7420 6f66 2064  d as a list of d
-0000de40: 6963 7469 6f6e 6172 7920 6974 656d 732c  ictionary items,
-0000de50: 2065 6163 6820 6f66 2077 6869 6368 206d   each of which m
-0000de60: 7573 7420 696e 636c 7564 6520 7468 6520  ust include the 
-0000de70: 7072 6f70 6572 7469 6573 2060 6c6f 6361  properties `loca
-0000de80: 6c50 6174 6860 2061 6e64 2060 7570 6c6f  lPath` and `uplo
-0000de90: 6164 5061 7468 602e 200a 0a2d 2060 6c6f  adPath`. ..- `lo
-0000dea0: 6361 6c50 6174 6860 2073 7065 6369 6669  calPath` specifi
-0000deb0: 6573 2074 6865 2070 6174 686e 616d 6520  es the pathname 
-0000dec0: 6f66 2074 6865 2066 696c 6520 6f6e 206c  of the file on l
-0000ded0: 6f63 616c 2073 746f 7261 6765 0a2d 2060  ocal storage.- `
-0000dee0: 7570 6c6f 6164 5061 7468 6020 7370 6563  uploadPath` spec
-0000def0: 6966 6965 7320 7468 6520 6e61 6d65 2061  ifies the name a
-0000df00: 6e64 206c 6f63 6174 696f 6e20 6f66 2074  nd location of t
-0000df10: 6865 2066 696c 6527 7320 6465 7374 696e  he file's destin
-0000df20: 6174 696f 6e20 696e 2074 6865 204f 626a  ation in the Obj
-0000df30: 6563 7420 5374 6f72 650a 0a46 6f72 2065  ect Store..For e
-0000df40: 7861 6d70 6c65 2c20 696e 2054 4f4d 4c3a  xample, in TOML:
-0000df50: 0a60 6060 746f 6d6c 0a75 706c 6f61 6446  .```toml.uploadF
-0000df60: 696c 6573 203d 205b 0a20 2020 207b 6c6f  iles = [.    {lo
-0000df70: 6361 6c50 6174 6820 3d20 2266 696c 655f  calPath = "file_
-0000df80: 312e 7478 7422 2c20 7570 6c6f 6164 5061  1.txt", uploadPa
-0000df90: 7468 203d 2022 6669 6c65 5f31 2e74 7874  th = "file_1.txt
-0000dfa0: 227d 2c0a 2020 2020 7b6c 6f63 616c 5061  "},.    {localPa
-0000dfb0: 7468 203d 2022 6469 725f 322f 6669 6c65  th = "dir_2/file
-0000dfc0: 5f32 2e74 7874 222c 2075 706c 6f61 6450  _2.txt", uploadP
-0000dfd0: 6174 6820 3d20 223a 3a66 696c 655f 322e  ath = "::file_2.
-0000dfe0: 7478 7422 7d2c 0a20 2020 207b 6c6f 6361  txt"},.    {loca
-0000dff0: 6c50 6174 6820 3d20 2266 696c 655f 332e  lPath = "file_3.
-0000e000: 7478 7422 2c20 7570 6c6f 6164 5061 7468  txt", uploadPath
-0000e010: 203d 2022 6f74 6865 725f 6e61 6d65 7370   = "other_namesp
-0000e020: 6163 653a 3a66 696c 655f 332e 7478 7422  ace::file_3.txt"
-0000e030: 7d0a 5d0a 6060 600a 416e 6420 696e 204a  }.].```.And in J
-0000e040: 534f 4e2c 2077 6974 6820 7468 6520 7072  SON, with the pr
-0000e050: 6f70 6572 7479 2073 6574 2061 7420 7468  operty set at th
-0000e060: 6520 5461 736b 206c 6576 656c 2c20 7468  e Task level, th
-0000e070: 6520 7361 6d65 2073 7065 6369 6669 6361  e same specifica
-0000e080: 7469 6f6e 2077 6f75 6c64 2062 653a 0a60  tion would be:.`
-0000e090: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
-0000e0a0: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
-0000e0b0: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-0000e0c0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-0000e0d0: 2020 2020 2020 2275 706c 6f61 6446 696c        "uploadFil
-0000e0e0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
-0000e0f0: 2020 207b 226c 6f63 616c 5061 7468 223a     {"localPath":
-0000e100: 2022 6669 6c65 5f31 2e74 7874 222c 2022   "file_1.txt", "
-0000e110: 7570 6c6f 6164 5061 7468 223a 2022 6669  uploadPath": "fi
-0000e120: 6c65 5f31 2e74 7874 227d 2c0a 2020 2020  le_1.txt"},.    
-0000e130: 2020 2020 2020 2020 7b22 6c6f 6361 6c50          {"localP
-0000e140: 6174 6822 3a20 2264 6972 5f32 2f66 696c  ath": "dir_2/fil
-0000e150: 655f 322e 7478 7422 2c20 2275 706c 6f61  e_2.txt", "uploa
-0000e160: 6450 6174 6822 3a20 223a 3a66 696c 655f  dPath": "::file_
-0000e170: 322e 7478 7422 7d2c 0a20 2020 2020 2020  2.txt"},.       
-0000e180: 2020 2020 207b 226c 6f63 616c 5061 7468       {"localPath
-0000e190: 223a 2022 6669 6c65 5f33 2e74 7874 222c  ": "file_3.txt",
-0000e1a0: 2022 7570 6c6f 6164 5061 7468 223a 2022   "uploadPath": "
-0000e1b0: 6f74 6865 725f 6e61 6d65 7370 6163 653a  other_namespace:
-0000e1c0: 3a66 696c 655f 332e 7478 7422 7d0a 2020  :file_3.txt"}.  
-0000e1d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000e1e0: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
-0000e1f0: 7d0a 2020 5d0a 7d0a 6060 600a 0a57 6865  }.  ].}.```..Whe
-0000e200: 6e20 7275 6e6e 696e 6720 7468 6520 5079  n running the Py
-0000e210: 7468 6f6e 2045 7861 6d70 6c65 7320 636f  thon Examples co
-0000e220: 6d6d 616e 6473 206f 6e20 2a2a 5769 6e64  mmands on **Wind
-0000e230: 6f77 732a 2a20 686f 7374 732c 206e 6f74  ows** hosts, not
-0000e240: 6520 7468 6174 2065 6974 6865 7220 5769  e that either Wi
-0000e250: 6e64 6f77 7320 6f72 2055 6e69 7820 6469  ndows or Unix di
-0000e260: 7265 6374 6f72 7920 7365 7061 7261 746f  rectory separato
-0000e270: 7273 2063 616e 2062 6520 7573 6564 2066  rs can be used f
-0000e280: 6f72 2074 6865 2060 6c6f 6361 6c50 6174  or the `localPat
-0000e290: 6860 2070 6174 686e 616d 6573 2028 6f72  h` pathnames (or
-0000e2a0: 2074 6865 2070 6174 686e 616d 6573 2069   the pathnames i
-0000e2b0: 6e20 6069 6e70 7574 7360 292c 2062 7574  n `inputs`), but
-0000e2c0: 2074 6865 2055 6e69 7820 636f 6e76 656e   the Unix conven
-0000e2d0: 7469 6f6e 206d 7573 7420 6265 2075 7365  tion must be use
-0000e2e0: 6420 666f 7220 7468 6520 6075 706c 6f61  d for the `uploa
-0000e2f0: 6450 6174 6860 206e 616d 6573 2c20 652e  dPath` names, e.
-0000e300: 672e 3a0a 0a60 6060 746f 6d6c 0a75 706c  g.:..```toml.upl
-0000e310: 6f61 6446 696c 6573 203d 205b 0a20 2020  oadFiles = [.   
-0000e320: 207b 6c6f 6361 6c50 6174 6820 3d20 2264   {localPath = "d
-0000e330: 6972 5f32 5c5c 6669 6c65 5f32 2e74 7874  ir_2\\file_2.txt
-0000e340: 222c 2075 706c 6f61 6450 6174 6820 3d20  ", uploadPath = 
-0000e350: 223a 3a6d 795f 6469 7265 6374 6f72 792f  "::my_directory/
-0000e360: 6669 6c65 5f32 2e74 7874 227d 2c0a 5d0a  file_2.txt"},.].
-0000e370: 6060 600a 0a54 6865 2060 7570 6c6f 6164  ```..The `upload
-0000e380: 4669 6c65 7360 2070 726f 7065 7274 7920  Files` property 
-0000e390: 6361 6e20 616c 736f 2062 6520 7365 7420  can also be set 
-0000e3a0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
-0000e3b0: 6972 656d 656e 7420 616e 6420 5461 736b  irement and Task
-0000e3c0: 2047 726f 7570 206c 6576 656c 732c 2061   Group levels, a
-0000e3d0: 6e64 2070 726f 7065 7274 7920 696e 6865  nd property inhe
-0000e3e0: 7269 7461 6e63 6520 6f70 6572 6174 6573  ritance operates
-0000e3f0: 2061 7320 6e6f 726d 616c 2e0a 0a46 6f72   as normal...For
-0000e400: 2060 7570 6c6f 6164 5061 7468 602c 2074   `uploadPath`, t
-0000e410: 6865 2073 616d 6520 603a 3a60 206e 616d  he same `::` nam
-0000e420: 696e 6720 636f 6e76 656e 7469 6f6e 2069  ing convention i
-0000e430: 7320 6176 6169 6c61 626c 6520 6173 2069  s available as i
-0000e440: 7320 7573 6564 2069 6e20 7468 6520 6076  s used in the `v
-0000e450: 6572 6966 7941 7453 7461 7274 602c 2060  erifyAtStart`, `
-0000e460: 7665 7269 6679 5761 6974 6020 616e 6420  verifyWait` and 
-0000e470: 6069 6e70 7574 734f 7074 696f 6e61 6c60  `inputsOptional`
-0000e480: 2070 726f 7065 7274 6965 7320 6469 7363   properties disc
-0000e490: 7573 7365 6420 6265 6c6f 773a 0a0a 2d20  ussed below:..- 
-0000e4a0: 4966 2060 3a3a 6020 6973 206e 6f74 2075  If `::` is not u
-0000e4b0: 7365 642c 2074 6865 6e20 7468 6520 6669  sed, then the fi
-0000e4c0: 6c65 2069 7320 7570 6c6f 6164 6564 2072  le is uploaded r
-0000e4d0: 656c 6174 6976 6520 746f 2074 6865 2063  elative to the c
-0000e4e0: 7572 7265 6e74 206e 616d 6573 7061 6365  urrent namespace
-0000e4f0: 2069 6e20 6120 6469 7265 6374 6f72 7920   in a directory 
-0000e500: 6e61 6d65 6420 6166 7465 7220 7468 6520  named after the 
-0000e510: 6e61 6d65 206f 6620 7468 6520 576f 726b  name of the Work
-0000e520: 2052 6571 7569 7265 6d65 6e74 0a2d 2049   Requirement.- I
-0000e530: 6620 603a 3a60 2069 7320 7573 6564 2061  f `::` is used a
-0000e540: 7420 7468 6520 7374 6172 7420 6f66 2074  t the start of t
-0000e550: 6865 2060 7570 6c6f 6164 5061 7468 602c  he `uploadPath`,
-0000e560: 2074 6865 2066 696c 6520 6973 2075 706c   the file is upl
-0000e570: 6f61 6465 6420 7265 6c61 7469 7665 2074  oaded relative t
-0000e580: 6f20 7468 6520 726f 6f74 206f 6620 7468  o the root of th
-0000e590: 6520 6375 7272 656e 7420 6e61 6d65 7370  e current namesp
-0000e5a0: 6163 650a 2d20 4966 2060 3c6e 616d 6573  ace.- If `<names
-0000e5b0: 7061 6365 3e3a 3a60 2069 7320 7573 6564  pace>::` is used
-0000e5c0: 2061 7420 7468 6520 7374 6172 7420 6f66   at the start of
-0000e5d0: 2060 7570 6c6f 6164 5061 7468 602c 2074   `uploadPath`, t
-0000e5e0: 6865 2066 696c 6520 6973 2075 706c 6f61  he file is uploa
-0000e5f0: 6465 6420 7265 6c61 7469 7665 2074 6f20  ded relative to 
-0000e600: 7468 6520 726f 6f74 206f 6620 603c 6e61  the root of `<na
-0000e610: 6d65 7370 6163 653e 600a 0a45 6163 6820  mespace>`..Each 
-0000e620: 6669 6c65 2073 7065 6369 6669 6564 2069  file specified i
-0000e630: 6e20 7468 6520 6075 706c 6f61 6446 696c  n the `uploadFil
-0000e640: 6573 6020 6c69 7374 7320 7769 6c6c 206f  es` lists will o
-0000e650: 6e6c 7920 6265 2075 706c 6f61 6465 6420  nly be uploaded 
-0000e660: 6f6e 6365 2074 6f20 6561 6368 2075 6e69  once to each uni
-0000e670: 7175 6520 7570 6c6f 6164 206c 6f63 6174  que upload locat
-0000e680: 696f 6e20 666f 7220 616e 7920 6769 7665  ion for any give
-0000e690: 6e20 696e 766f 6361 7469 6f6e 206f 6620  n invocation of 
-0000e6a0: 6079 642d 7375 626d 6974 602e 0a0a 4966  `yd-submit`...If
-0000e6b0: 2061 2066 696c 6520 696e 2074 6865 2060   a file in the `
-0000e6c0: 7570 6c6f 6164 4669 6c65 7360 206c 6973  uploadFiles` lis
-0000e6d0: 7420 6973 2072 6571 7569 7265 6420 6279  t is required by
-0000e6e0: 2061 2054 6173 6b2c 2069 7420 6d75 7374   a Task, it must
-0000e6f0: 2073 6570 6172 6174 656c 7920 6265 2061   separately be a
-0000e700: 6464 6564 2074 6f20 7468 6520 6076 6572  dded to the `ver
-0000e710: 6966 7941 7453 7461 7274 6020 6f72 2060  ifyAtStart` or `
-0000e720: 7665 7269 6679 5761 6974 6020 6c69 7374  verifyWait` list
-0000e730: 7320 6469 7363 7573 7365 6420 6265 6c6f  s discussed belo
-0000e740: 772e 2054 6869 7320 6973 206e 6f74 2064  w. This is not d
-0000e750: 6f6e 6520 6175 746f 6d61 7469 6361 6c6c  one automaticall
-0000e760: 792e 204e 6f74 6520 616c 736f 2074 6861  y. Note also tha
-0000e770: 7420 7468 6520 6066 6c61 7474 656e 5570  t the `flattenUp
-0000e780: 6c6f 6164 5061 7468 7360 2070 726f 7065  loadPaths` prope
-0000e790: 7274 7920 6973 2069 676e 6f72 6564 2066  rty is ignored f
-0000e7a0: 6f72 2066 696c 6573 2069 6e20 7468 6520  or files in the 
-0000e7b0: 6075 706c 6f61 6446 696c 6573 6020 6c69  `uploadFiles` li
-0000e7c0: 7374 2e0a 0a23 2323 2046 696c 6520 4465  st...### File De
-0000e7d0: 7065 6e64 656e 6369 6573 2055 7369 6e67  pendencies Using
-0000e7e0: 2060 7665 7269 6679 4174 5374 6172 7460   `verifyAtStart`
-0000e7f0: 2061 6e64 2060 7665 7269 6679 5761 6974   and `verifyWait
-0000e800: 600a 0a49 7427 7320 706f 7373 6962 6c65  `..It's possible
-0000e810: 2074 6f20 6d61 6b65 2054 6173 6b73 2064   to make Tasks d
-0000e820: 6570 656e 6465 6e74 206f 6e20 7468 6520  ependent on the 
-0000e830: 7072 6573 656e 6365 206f 6620 6669 6c65  presence of file
-0000e840: 7320 696e 2074 6865 204f 626a 6563 7420  s in the Object 
-0000e850: 5374 6f72 6520 6279 2075 7369 6e67 2074  Store by using t
-0000e860: 6865 2060 7665 7269 6679 4174 5374 6172  he `verifyAtStar
-0000e870: 7460 2061 6e64 2060 7665 7269 6679 5761  t` and `verifyWa
-0000e880: 6974 6020 6c69 7374 732e 2054 6865 7365  it` lists. These
-0000e890: 2066 696c 6573 2061 7265 206e 6f74 2061   files are not a
-0000e8a0: 7574 6f6d 6174 6963 616c 6c79 2075 706c  utomatically upl
-0000e8b0: 6f61 6465 6420 7768 656e 2075 7369 6e67  oaded when using
-0000e8c0: 2060 7964 2d73 7562 6d69 7460 2073 6f20   `yd-submit` so 
-0000e8d0: 6172 6520 6569 7468 6572 2075 706c 6f61  are either uploa
-0000e8e0: 6465 6420 6d61 6e75 616c 6c79 2028 652e  ded manually (e.
-0000e8f0: 672e 2c20 6279 2075 7369 6e67 2060 7964  g., by using `yd
-0000e900: 2d75 706c 6f61 6460 292c 206f 7220 6172  -upload`), or ar
-0000e910: 6520 6372 6561 7465 6420 6173 2061 2072  e created as a r
-0000e920: 6573 756c 7420 6f66 2074 6865 2065 7865  esult of the exe
-0000e930: 6375 7469 6f6e 206f 6620 6f74 6865 7220  cution of other 
-0000e940: 5461 736b 732e 0a0a 4e6f 7465 2074 6861  Tasks...Note tha
-0000e950: 7420 6120 6769 7665 6e20 6669 6c65 2063  t a given file c
-0000e960: 616e 206f 6e6c 7920 6170 7065 6172 2069  an only appear i
-0000e970: 6e20 2a6f 6e65 2a20 6f66 2074 6865 2060  n *one* of the `
-0000e980: 696e 7075 7473 602c 2060 7665 7269 6679  inputs`, `verify
-0000e990: 4174 5374 6172 7460 206f 7220 6076 6572  AtStart` or `ver
-0000e9a0: 6966 7957 6169 7460 206c 6973 7473 2e0a  ifyWait` lists..
-0000e9b0: 0a54 6173 6b73 2077 6974 6820 6076 6572  .Tasks with `ver
-0000e9c0: 6966 7941 7453 7461 7274 6020 6465 7065  ifyAtStart` depe
-0000e9d0: 6e64 656e 6369 6573 2077 696c 6c20 6661  ndencies will fa
-0000e9e0: 696c 2069 6d6d 6564 6961 7465 6c79 2069  il immediately i
-0000e9f0: 6620 7468 6520 7265 7175 6972 6564 2066  f the required f
-0000ea00: 696c 6573 2061 7265 206e 6f74 2070 7265  iles are not pre
-0000ea10: 7365 6e74 2077 6865 6e20 7468 6520 5461  sent when the Ta
-0000ea20: 736b 2069 7320 7375 626d 6974 7465 642e  sk is submitted.
-0000ea30: 2054 6173 6b73 2077 6974 6820 6076 6572   Tasks with `ver
-0000ea40: 6966 7957 6169 7460 2064 6570 656e 6465  ifyWait` depende
-0000ea50: 6e63 6965 7320 7769 6c6c 206e 6f74 2062  ncies will not b
-0000ea60: 6563 6f6d 6520 6052 4541 4459 6020 746f  ecome `READY` to
-0000ea70: 2062 6520 7363 6865 6475 6c65 6420 746f   be scheduled to
-0000ea80: 2057 6f72 6b65 7273 2075 6e74 696c 2074   Workers until t
-0000ea90: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-0000eaa0: 6172 6520 7361 7469 7366 6965 642e 0a0a  are satisfied...
-0000eab0: 5768 656e 2073 7065 6369 6679 696e 6720  When specifying 
-0000eac0: 6669 6c65 7320 696e 2074 6865 2060 7665  files in the `ve
-0000ead0: 7269 6679 4174 5374 6172 7460 2061 6e64  rifyAtStart` and
-0000eae0: 2060 7665 7269 6679 5761 6974 6020 6c69   `verifyWait` li
-0000eaf0: 7374 732c 2061 7320 7769 7468 2074 6865  sts, as with the
-0000eb00: 2060 7570 6c6f 6164 5061 7468 6020 7072   `uploadPath` pr
-0000eb10: 6f70 6572 7479 2064 6973 6375 7373 6564  operty discussed
-0000eb20: 2061 626f 7665 2c20 7468 6520 6669 6c65   above, the file
-0000eb30: 206c 6f63 6174 696f 6e73 2063 616e 2062   locations can b
-0000eb40: 6520 2831 2920 7265 6c61 7469 7665 2074  e (1) relative t
-0000eb50: 6f20 7468 6520 576f 726b 2052 6571 7569  o the Work Requi
-0000eb60: 7265 6d65 6e74 206e 616d 6520 696e 2074  rement name in t
-0000eb70: 6865 2063 7572 7265 6e74 206e 616d 6573  he current names
-0000eb80: 7061 6365 2028 7468 6520 6465 6661 756c  pace (the defaul
-0000eb90: 7429 2c20 2832 2920 7265 6c61 7469 7665  t), (2) relative
-0000eba0: 2074 6f20 7468 6520 726f 6f74 206f 6620   to the root of 
-0000ebb0: 7468 6520 6375 7272 656e 7420 6e61 6d65  the current name
-0000ebc0: 7370 6163 652c 206f 7220 2833 2920 7265  space, or (3) re
-0000ebd0: 6c61 7469 7665 2074 6f20 7468 6520 726f  lative to the ro
-0000ebe0: 6f74 206f 6620 6120 6469 6666 6572 656e  ot of a differen
-0000ebf0: 7420 6e61 6d65 7370 6163 6520 696e 2074  t namespace in t
-0000ec00: 6865 2075 7365 7227 7320 4163 636f 756e  he user's Accoun
-0000ec10: 742e 0a0a 312e 2046 6f72 2066 696c 6573  t...1. For files
-0000ec20: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-0000ec30: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-0000ec40: 7420 6e61 6d65 2069 6e20 7468 6520 6375  t name in the cu
-0000ec50: 7272 656e 7420 6e61 6d65 7370 6163 652c  rrent namespace,
-0000ec60: 206a 7573 7420 7573 6520 7468 6520 6669   just use the fi
-0000ec70: 6c65 2070 6174 682c 2065 2e67 2e0a 6060  le path, e.g..``
-0000ec80: 6073 6865 6c6c 0a22 7665 7269 6679 5761  `shell."verifyWa
-0000ec90: 6974 223a 205b 2266 696c 655f 312e 7478  it": ["file_1.tx
-0000eca0: 7422 5d20 2d3e 2064 6576 656c 6f70 6d65  t"] -> developme
-0000ecb0: 6e74 3a74 6573 7472 756e 5f32 3231 3130  nt:testrun_22110
-0000ecc0: 382d 3132 3034 3034 2d37 6432 2f66 696c  8-120404-7d2/fil
-0000ecd0: 655f 312e 7478 740a 6060 600a 0a32 2e20  e_1.txt.```..2. 
-0000ece0: 466f 7220 6669 6c65 7320 7265 6c61 7469  For files relati
-0000ecf0: 7665 2074 6f20 7468 6520 726f 6f74 206f  ve to the root o
-0000ed00: 6620 7468 6520 6375 7272 656e 7420 6e61  f the current na
-0000ed10: 6d65 7370 6163 652c 2070 7265 6669 7820  mespace, prefix 
-0000ed20: 7468 6520 6669 6c65 2070 6174 6820 7769  the file path wi
-0000ed30: 7468 2060 3a3a 602c 2065 2e67 2e0a 6060  th `::`, e.g..``
-0000ed40: 6073 6865 6c6c 0a22 7665 7269 6679 5761  `shell."verifyWa
-0000ed50: 6974 223a 205b 223a 3a66 696c 655f 312e  it": ["::file_1.
-0000ed60: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
-0000ed70: 6d65 6e74 3a66 696c 655f 312e 7478 740a  ment:file_1.txt.
-0000ed80: 6060 600a 0a33 2e20 466f 7220 6669 6c65  ```..3. For file
-0000ed90: 7320 7265 6c61 7469 7665 2074 6f20 7468  s relative to th
-0000eda0: 6520 726f 6f74 206f 6620 6120 6469 6666  e root of a diff
-0000edb0: 6572 656e 7420 6e61 6d65 7370 6163 652c  erent namespace,
-0000edc0: 2070 7265 6669 7820 7468 6520 6669 6c65   prefix the file
-0000edd0: 2070 6174 6820 7769 7468 2074 6865 206e   path with the n
-0000ede0: 616d 6573 7061 6365 206e 616d 6520 616e  amespace name an
-0000edf0: 6420 603a 3a60 2c20 652e 672e 0a60 6060  d `::`, e.g..```
-0000ee00: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
-0000ee10: 7422 3a20 5b22 6f74 6865 725f 6e61 6d65  t": ["other_name
-0000ee20: 7370 6163 653a 3a66 696c 655f 312e 7478  space::file_1.tx
-0000ee30: 7422 5d20 2d3e 206f 7468 6572 5f6e 616d  t"] -> other_nam
-0000ee40: 6573 7061 6365 3a66 696c 655f 312e 7478  espace:file_1.tx
-0000ee50: 740a 6060 600a 0a54 6865 2075 7365 206f  t.```..The use o
-0000ee60: 6620 7468 6520 7468 7265 6520 6469 6666  f the three diff
-0000ee70: 6572 656e 7420 666f 726d 7320 6361 6e20  erent forms can 
-0000ee80: 6265 206d 6978 6564 2077 6974 6869 6e20  be mixed within 
-0000ee90: 6120 7369 6e67 6c65 206c 6973 742c 2065  a single list, e
-0000eea0: 2e67 2e3a 0a60 6060 7368 656c 6c0a 2276  .g.:.```shell."v
-0000eeb0: 6572 6966 7941 7453 7461 7274 223a 205b  erifyAtStart": [
-0000eec0: 2266 696c 655f 312e 7478 7422 2c20 223a  "file_1.txt", ":
-0000eed0: 3a64 6972 5f32 2f66 696c 655f 322e 7478  :dir_2/file_2.tx
-0000eee0: 7422 2c20 226f 7468 6572 5f6e 616d 6573  t", "other_names
-0000eef0: 7061 6365 3a3a 6469 725f 332f 6669 6c65  pace::dir_3/file
-0000ef00: 5f33 2e74 7874 225d 0a60 6060 0a0a 2323  _3.txt"].```..##
-0000ef10: 2320 4669 6c65 7320 446f 776e 6c6f 6164  # Files Download
-0000ef20: 6564 2055 7369 6e67 2060 696e 7075 7473  ed Using `inputs
-0000ef30: 4f70 7469 6f6e 616c 600a 0a54 6865 2060  Optional`..The `
-0000ef40: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
-0000ef50: 7072 6f70 6572 7479 2077 6f72 6b73 2069  property works i
-0000ef60: 6e20 6120 7369 6d69 6c61 7220 6661 7368  n a similar fash
-0000ef70: 696f 6e20 746f 2074 6865 2060 7665 7269  ion to the `veri
-0000ef80: 6679 2a60 2070 726f 7065 7274 6965 7320  fy*` properties 
-0000ef90: 6162 6f76 652c 2062 7574 2074 6865 2066  above, but the f
-0000efa0: 696c 6573 2073 7065 6369 6669 6564 2069  iles specified i
-0000efb0: 6e20 7468 6973 206c 6973 7420 6172 6520  n this list are 
-0000efc0: 6f70 7469 6f6e 616c 2e20 5468 6973 2070  optional. This p
-0000efd0: 726f 7065 7274 7920 616c 736f 2061 6c6c  roperty also all
-0000efe0: 6f77 7320 666f 7220 7468 6520 7573 6520  ows for the use 
-0000eff0: 6f66 2077 696c 6463 6172 6473 2060 2a60  of wildcards `*`
-0000f000: 2061 6e64 2060 2a2a 6020 746f 2063 6f6c   and `**` to col
-0000f010: 6c65 6374 2066 696c 6573 2075 7369 6e67  lect files using
-0000f020: 2077 696c 6463 6172 6420 7061 7468 732e   wildcard paths.
-0000f030: 2054 6865 202a 2a61 6e74 2a2a 2063 6f6e   The **ant** con
-0000f040: 7665 6e74 696f 6e73 2061 7265 2075 7365  ventions are use
-0000f050: 6420 666f 7220 7468 6573 6520 7769 6c64  d for these wild
-0000f060: 6361 7264 732e 0a0a 2323 2320 4669 6c65  cards...### File
-0000f070: 7320 446f 776e 6c6f 6164 6564 2074 6f20  s Downloaded to 
-0000f080: 6120 4e6f 6465 2066 6f72 2075 7365 2069  a Node for use i
-0000f090: 6e20 5461 736b 2045 7865 6375 7469 6f6e  n Task Execution
-0000f0a0: 0a0a 5768 656e 2061 2054 6173 6b20 6973  ..When a Task is
-0000f0b0: 2065 7865 6375 7465 6420 6279 2061 2057   executed by a W
-0000f0c0: 6f72 6b65 7220 6f6e 2061 204e 6f64 652c  orker on a Node,
-0000f0d0: 2069 7473 2072 6571 7569 7265 6420 6669   its required fi
-0000f0e0: 6c65 7320 6172 6520 646f 776e 6c6f 6164  les are download
-0000f0f0: 6564 2066 726f 6d20 7468 6520 4f62 6a65  ed from the Obje
-0000f100: 6374 2053 746f 7265 2070 7269 6f72 2074  ct Store prior t
-0000f110: 6f20 5461 736b 2065 7865 6375 7469 6f6e  o Task execution
-0000f120: 2e20 416e 7920 6669 6c65 206c 6973 7465  . Any file liste
-0000f130: 6420 696e 2074 6865 2060 696e 7075 7473  d in the `inputs
-0000f140: 6020 666f 7220 6120 5461 736b 2069 7320  ` for a Task is 
-0000f150: 6173 7375 6d65 6420 746f 2062 6520 7265  assumed to be re
-0000f160: 7175 6972 6564 2c20 616c 6f6e 6720 7769  quired, along wi
-0000f170: 7468 2061 6e79 2061 6464 6974 696f 6e61  th any additiona
-0000f180: 6c20 6669 6c65 7320 7370 6563 6966 6965  l files specifie
-0000f190: 6420 696e 2074 6865 2060 7665 7269 6679  d in the `verify
-0000f1a0: 4174 5374 6172 7460 2061 6e64 2060 7665  AtStart` and `ve
-0000f1b0: 7269 6679 5761 6974 6020 6c69 7374 732e  rifyWait` lists.
-0000f1c0: 2046 696c 6573 2073 7065 6369 6669 6564   Files specified
-0000f1d0: 2075 7369 6e67 2074 6865 2060 696e 7075   using the `inpu
-0000f1e0: 7473 4f70 7469 6f6e 616c 6020 7072 6f70  tsOptional` prop
-0000f1f0: 6572 7479 2061 7265 206f 7074 696f 6e61  erty are optiona
-0000f200: 6c6c 7920 646f 776e 6c6f 6164 6564 2066  lly downloaded f
-0000f210: 726f 6d20 7468 6520 4f62 6a65 6374 2053  rom the Object S
-0000f220: 746f 7265 2e20 284e 6f74 6520 7468 6174  tore. (Note that
-0000f230: 2061 2066 696c 6520 7368 6f75 6c64 206f   a file should o
-0000f240: 6e6c 7920 6170 7065 6172 2069 6e20 6f6e  nly appear in on
-0000f250: 6520 6f66 2074 6865 7365 2066 6f75 7220  e of these four 
-0000f260: 6c69 7374 732c 206f 7468 6572 7769 7365  lists, otherwise
-0000f270: 2060 7964 2d73 7562 6d69 7460 2077 696c   `yd-submit` wil
-0000f280: 6c20 7265 7475 726e 2061 6e20 6572 726f  l return an erro
-0000f290: 722e 290a 0a57 6865 6e20 6120 5461 736b  r.)..When a Task
-0000f2a0: 2069 7320 7374 6172 7465 6420 6279 2074   is started by t
-0000f2b0: 6865 2041 6765 6e74 2c20 6974 7320 776f  he Agent, its wo
-0000f2c0: 726b 696e 6720 6469 7265 6374 6f72 7920  rking directory 
-0000f2d0: 6861 7320 6120 7061 7474 6572 6e20 736f  has a pattern so
-0000f2e0: 6d65 7468 696e 6720 6c69 6b65 3a0a 0a60  mething like:..`
-0000f2f0: 2f76 6172 2f6f 7074 2f79 656c 6c6f 7764  /var/opt/yellowd
-0000f300: 6f67 2f79 642d 6167 656e 742d 342f 6461  og/yd-agent-4/da
-0000f310: 7461 2f77 6f72 6b65 7273 2f31 2f79 6469  ta/workers/1/ydi
-0000f320: 645f 7461 736b 5f44 3044 3044 305f 3638  d_task_D0D0D0_68
-0000f330: 6635 6535 6265 2d64 6339 332d 3439 6562  f5e5be-dc93-49eb
-0000f340: 2d61 3832 342d 3166 6364 6235 3266 3931  -a824-1fcdb52f91
-0000f350: 3935 5f31 5f31 600a 0a28 6079 6469 645f  95_1_1`..(`ydid_
-0000f360: 7461 736b 5f44 3044 3044 305f 3638 6635  task_D0D0D0_68f5
-0000f370: 6535 6265 2d64 6339 332d 3439 6562 2d61  e5be-dc93-49eb-a
-0000f380: 3832 342d 3166 6364 6235 3266 3931 3935  824-1fcdb52f9195
-0000f390: 5f31 5f31 6020 6973 2061 6e20 6570 6865  _1_1` is an ephe
-0000f3a0: 6d65 7261 6c20 6469 7265 6374 6f72 7920  meral directory 
-0000f3b0: 7468 6174 2069 7320 7265 6d6f 7665 6420  that is removed 
-0000f3c0: 6166 7465 7220 7468 6520 5461 736b 2066  after the Task f
-0000f3d0: 696e 6973 6865 7320 616e 6420 616e 7920  inishes and any 
-0000f3e0: 6f75 7470 7574 7320 6861 7665 2062 6565  outputs have bee
-0000f3f0: 6e20 7570 6c6f 6164 6564 2e29 0a0a 4669  n uploaded.)..Fi
-0000f400: 6c65 7320 7468 6174 2061 7265 2064 6f77  les that are dow
-0000f410: 6e6c 6f61 6465 6420 6279 2074 6865 2041  nloaded by the A
-0000f420: 6765 6e74 2070 7269 6f72 2074 6f20 5461  gent prior to Ta
-0000f430: 736b 2065 7865 6375 7469 6f6e 2061 7265  sk execution are
-0000f440: 206c 6f63 6174 6564 2061 7320 666f 6c6c   located as foll
-0000f450: 6f77 733a 0a0a 312e 2049 6620 7468 6520  ows:..1. If the 
-0000f460: 6066 6c61 7474 656e 496e 7075 7450 6174  `flattenInputPat
-0000f470: 6873 6020 7072 6f70 6572 7479 2069 7320  hs` property is 
-0000f480: 7365 7420 746f 2074 6865 2064 6566 6175  set to the defau
-0000f490: 6c74 206f 6620 6066 616c 7365 6020 666f  lt of `false` fo
-0000f4a0: 7220 7468 6520 5461 736b 2c20 7468 6520  r the Task, the 
-0000f4b0: 646f 776e 6c6f 6164 6564 206f 626a 6563  downloaded objec
-0000f4c0: 7473 2061 7265 2070 6c61 6365 6420 696e  ts are placed in
-0000f4d0: 2073 7562 6469 7265 6374 6f72 6965 7320   subdirectories 
-0000f4e0: 7468 6174 206d 6972 726f 7220 7468 6f73  that mirror thos
-0000f4f0: 6520 696e 2074 6865 204f 626a 6563 7420  e in the Object 
-0000f500: 5374 6f72 652c 2069 6e63 6c75 6469 6e67  Store, including
-0000f510: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-0000f520: 656d 656e 7420 6e61 6d65 2c20 7369 7475  ement name, situ
-0000f530: 6174 6564 2062 656e 6561 7468 2074 6865  ated beneath the
-0000f540: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
-0000f550: 7279 2e0a 0a0a 322e 2049 6620 7468 6520  ry....2. If the 
-0000f560: 6066 6c61 7474 656e 496e 7075 7450 6174  `flattenInputPat
-0000f570: 6873 6020 7072 6f70 6572 7479 2069 7320  hs` property is 
-0000f580: 7365 7420 746f 2060 7472 7565 6020 666f  set to `true` fo
-0000f590: 7220 7468 6520 5461 736b 2c20 7468 6520  r the Task, the 
-0000f5a0: 646f 776e 6c6f 6164 6564 206f 626a 6563  downloaded objec
-0000f5b0: 7473 2061 7265 2061 6c6c 2070 6c61 6365  ts are all place
-0000f5c0: 6420 6469 7265 6374 6c79 2069 6e20 726f  d directly in ro
-0000f5d0: 6f74 206f 6620 7468 6520 5461 736b 2773  ot of the Task's
-0000f5e0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
-0000f5f0: 7279 2e0a 0a46 6f72 2065 7861 6d70 6c65  ry...For example
-0000f600: 3a0a 0a60 6060 7368 656c 6c0a 4966 2074  :..```shell.If t
-0000f610: 6865 2072 6571 7569 7265 6420 6f62 6a65  he required obje
-0000f620: 6374 2069 733a 2064 6576 656c 6f70 6d65  ct is: developme
-0000f630: 6e74 3a3a 7465 7374 7275 6e5f 3232 3131  nt::testrun_2211
-0000f640: 3038 2d31 3230 3430 342d 3764 322f 6465  08-120404-7d2/de
-0000f650: 762f 6669 6c65 5f31 2e74 7874 0a0a 7468  v/file_1.txt..th
-0000f660: 656e 2c20 6966 2066 6c61 7474 656e 496e  en, if flattenIn
-0000f670: 7075 7450 6174 6873 2069 7320 6661 6c73  putPaths is fals
-0000f680: 652c 2074 6865 2066 696c 6520 7769 6c6c  e, the file will
-0000f690: 2062 6520 666f 756e 6420 6174 3a0a 202d   be found at:. -
-0000f6a0: 3e20 3c77 6f72 6b69 6e67 5f64 6972 6563  > <working_direc
-0000f6b0: 746f 7279 3e2f 7465 7374 7275 6e5f 3232  tory>/testrun_22
-0000f6c0: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
-0000f6d0: 6465 762f 6669 6c65 5f31 2e74 7874 0a20  dev/file_1.txt. 
-0000f6e0: 0a65 6c73 652c 2069 6620 666c 6174 7465  .else, if flatte
-0000f6f0: 6e49 6e70 7574 5061 7468 7320 6973 2074  nInputPaths is t
-0000f700: 7275 652c 2074 6865 2066 696c 6520 7769  rue, the file wi
-0000f710: 6c6c 2062 6520 666f 756e 6420 6174 3a0a  ll be found at:.
-0000f720: 202d 3e20 3c77 6f72 6b69 6e67 5f64 6972   -> <working_dir
-0000f730: 6563 746f 7279 3e2f 6669 6c65 5f31 2e74  ectory>/file_1.t
-0000f740: 7874 200a 200a 7768 6572 6520 3c77 6f72  xt . .where <wor
-0000f750: 6b69 6e67 5f64 6972 6563 746f 7279 3e20  king_directory> 
-0000f760: 6973 3a0a 2020 2f76 6172 2f6f 7074 2f79  is:.  /var/opt/y
-0000f770: 656c 6c6f 7764 6f67 2f79 642d 6167 656e  ellowdog/yd-agen
-0000f780: 742d 342f 6461 7461 2f77 6f72 6b65 7273  t-4/data/workers
-0000f790: 2f31 2f79 6469 645f 7461 736b 5f44 3044  /1/ydid_task_D0D
-0000f7a0: 3044 305f 3638 6635 6535 6265 2d64 6339  0D0_68f5e5be-dc9
-0000f7b0: 332d 3439 6562 2d61 3832 342d 3166 6364  3-49eb-a824-1fcd
-0000f7c0: 6235 3266 3931 3935 5f31 5f31 2f0a 6060  b52f9195_1_1/.``
-0000f7d0: 600a 0a4e 6f74 6520 7468 6174 2057 6f72  `..Note that Wor
-0000f7e0: 6b20 5265 7175 6972 656d 656e 7420 6e61  k Requirement na
-0000f7f0: 6d65 2028 652e 672e 2c20 6074 6573 7472  me (e.g., `testr
-0000f800: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
-0000f810: 2d37 6432 6029 2069 7320 6176 6169 6c61  -7d2`) is availa
-0000f820: 626c 6520 7669 6120 7468 6520 7661 7269  ble via the vari
-0000f830: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-0000f840: 6e20 6077 725f 6e61 6d65 602c 2073 6f20  n `wr_name`, so 
-0000f850: 7468 6973 2063 6f75 6c64 2062 6520 7375  this could be su
-0000f860: 7070 6c69 6564 2074 6f20 7468 6520 5461  pplied to the Ta
-0000f870: 736b 2074 6f20 6865 6c70 2069 7420 6c6f  sk to help it lo
-0000f880: 6361 7465 2069 7473 2064 6f77 6e6c 6f61  cate its downloa
-0000f890: 6465 6420 6669 6c65 732e 2046 6f72 2065  ded files. For e
-0000f8a0: 7861 6d70 6c65 2c20 696e 2074 6865 2060  xample, in the `
-0000f8b0: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
-0000f8c0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-0000f8d0: 6063 6f6e 6669 672e 746f 6d6c 6020 6669  `config.toml` fi
-0000f8e0: 6c65 2c20 4920 636f 756c 6420 7370 6563  le, I could spec
-0000f8f0: 6966 793a 0a0a 6060 6074 6f6d 6c0a 656e  ify:..```toml.en
-0000f900: 7669 726f 6e6d 656e 7420 3d20 7b57 525f  vironment = {WR_
-0000f910: 4449 5245 4354 4f52 5920 3d20 227b 7b77  DIRECTORY = "{{w
-0000f920: 725f 6e61 6d65 7d7d 227d 0a60 6060 0a0a  r_name}}"}.```..
-0000f930: 5468 6520 576f 726b 2052 6571 7569 7265  The Work Require
-0000f940: 6d65 6e74 206e 616d 6520 776f 756c 6420  ment name would 
-0000f950: 7468 656e 2062 6520 6176 6169 6c61 626c  then be availabl
-0000f960: 6520 746f 2074 6865 2054 6173 6b20 696e  e to the Task in
-0000f970: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
-0000f980: 2076 6172 6961 626c 6520 6024 5752 5f44   variable `$WR_D
-0000f990: 4952 4543 544f 5259 602e 0a0a 2323 2320  IRECTORY`...### 
-0000f9a0: 4669 6c65 7320 5570 6c6f 6164 6564 2066  Files Uploaded f
-0000f9b0: 726f 6d20 6120 4e6f 6465 2074 6f20 7468  rom a Node to th
-0000f9c0: 6520 4f62 6a65 6374 2053 746f 7265 2061  e Object Store a
-0000f9d0: 6674 6572 2054 6173 6b20 4578 6563 7574  fter Task Execut
-0000f9e0: 696f 6e0a 0a41 6674 6572 2054 6173 6b20  ion..After Task 
-0000f9f0: 636f 6d70 6c65 7469 6f6e 2c20 7468 6520  completion, the 
-0000fa00: 4167 656e 7420 7769 6c6c 2075 706c 6f61  Agent will uploa
-0000fa10: 6420 7370 6563 6966 6965 6420 6f75 7470  d specified outp
-0000fa20: 7574 2066 696c 6573 2074 6f20 7468 6520  ut files to the 
-0000fa30: 4f62 6a65 6374 2053 746f 7265 2e20 5468  Object Store. Th
-0000fa40: 6520 6669 6c65 7320 746f 2062 6520 7570  e files to be up
-0000fa50: 6c6f 6164 6564 2061 7265 2074 686f 7365  loaded are those
-0000fa60: 206c 6973 7465 6420 696e 2074 6865 2060   listed in the `
-0000fa70: 6f75 7470 7574 7360 2061 6e64 2060 6f75  outputs` and `ou
-0000fa80: 7470 7574 7352 6571 7569 7265 6460 2070  tputsRequired` p
-0000fa90: 726f 7065 7274 6965 7320 666f 7220 7468  roperties for th
-0000faa0: 6520 5461 736b 2e0a 0a49 6e20 6164 6469  e Task...In addi
-0000fab0: 7469 6f6e 2c20 7468 6520 636f 6e73 6f6c  tion, the consol
-0000fac0: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
-0000fad0: 5461 736b 2069 7320 6361 7074 7572 6564  Task is captured
-0000fae0: 2069 6e20 6120 6669 6c65 2063 616c 6c65   in a file calle
-0000faf0: 6420 6074 6173 6b6f 7574 7075 742e 7478  d `taskoutput.tx
-0000fb00: 7460 2069 6e20 7468 6520 726f 6f74 206f  t` in the root o
-0000fb10: 6620 7468 6520 5461 736b 2773 2077 6f72  f the Task's wor
-0000fb20: 6b69 6e67 2064 6972 6563 746f 7279 2e20  king directory. 
-0000fb30: 5768 6574 6865 7220 7468 6520 6074 6173  Whether the `tas
-0000fb40: 6b6f 7574 7075 742e 7478 7460 2066 696c  koutput.txt` fil
-0000fb50: 6520 6973 2075 706c 6f61 6465 6420 746f  e is uploaded to
-0000fb60: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
-0000fb70: 6520 6973 2064 6574 6572 6d69 6e65 6420  e is determined 
-0000fb80: 6279 2074 6865 2060 6361 7074 7572 6554  by the `captureT
-0000fb90: 6173 6b4f 7574 7075 7460 2070 726f 7065  askOutput` prope
-0000fba0: 7274 7920 666f 7220 7468 6520 5461 736b  rty for the Task
-0000fbb0: 2c20 616e 6420 7468 6973 2069 7320 7365  , and this is se
-0000fbc0: 7420 746f 2027 7472 7565 2720 6279 2064  t to 'true' by d
-0000fbd0: 6566 6175 6c74 2e0a 0a49 6620 5461 736b  efault...If Task
-0000fbe0: 206f 7574 7075 7473 2061 7265 2063 7265   outputs are cre
-0000fbf0: 6174 6564 2069 6e20 7375 6264 6972 6563  ated in subdirec
-0000fc00: 746f 7269 6573 2062 656c 6f77 2074 6865  tories below the
-0000fc10: 2054 6173 6b27 7320 776f 726b 696e 6720   Task's working 
-0000fc20: 6469 7265 6374 6f72 792c 2069 6e63 6c75  directory, inclu
-0000fc30: 6465 2074 6865 2064 6972 6563 746f 7269  de the directori
-0000fc40: 6573 2066 6f72 2066 696c 6573 2069 6e20  es for files in 
-0000fc50: 7468 6520 606f 7574 7075 7473 6020 7072  the `outputs` pr
-0000fc60: 6f70 6572 7479 2e20 452e 672e 2c20 6966  operty. E.g., if
-0000fc70: 2061 2054 6173 6b20 6372 6561 7465 7320   a Task creates 
-0000fc80: 6669 6c65 7320 6072 6573 756c 7473 2f6f  files `results/o
-0000fc90: 7065 6e66 6f61 6d2e 7461 722e 677a 6020  penfoam.tar.gz` 
-0000fca0: 616e 6420 6072 6573 756c 7473 2f6f 7065  and `results/ope
-0000fcb0: 6e66 6f61 6d2e 6c6f 6760 2c20 7468 656e  nfoam.log`, then
-0000fcc0: 2073 7065 6369 6679 2074 6865 7365 2066   specify these f
-0000fcd0: 6f72 2075 706c 6f61 6420 696e 2074 6865  or upload in the
-0000fce0: 2060 6f75 7470 7574 7360 2070 726f 7065   `outputs` prope
-0000fcf0: 7274 7920 6173 2066 6f6c 6c6f 7773 3a0a  rty as follows:.
-0000fd00: 0a60 226f 7574 7075 7473 223a 205b 2272  .`"outputs": ["r
-0000fd10: 6573 756c 7473 2f6f 7065 6e66 6f61 6d2e  esults/openfoam.
-0000fd20: 7461 722e 677a 222c 2022 7265 7375 6c74  tar.gz", "result
-0000fd30: 732f 6f70 656e 666f 616d 2e6c 6f67 225d  s/openfoam.log"]
-0000fd40: 600a 0a57 6865 6e20 6f75 7470 7574 2066  `..When output f
-0000fd50: 696c 6573 2061 7265 2075 706c 6f61 6465  iles are uploade
-0000fd60: 6420 746f 2074 6865 204f 626a 6563 7420  d to the Object 
-0000fd70: 5374 6f72 652c 2074 6865 7920 6172 6520  Store, they are 
-0000fd80: 706c 6163 6564 2069 6e20 6120 5461 736b  placed in a Task
-0000fd90: 2047 726f 7570 2061 6e64 2054 6173 6b20   Group and Task 
-0000fda0: 7370 6563 6966 6963 2064 6972 6563 746f  specific directo
-0000fdb0: 7279 2e20 536f 2c20 6966 2074 6865 204e  ry. So, if the N
-0000fdc0: 616d 6573 7061 6365 2069 7320 6064 6576  amespace is `dev
-0000fdd0: 656c 6f70 6d65 6e74 602c 2074 6865 2057  elopment`, the W
-0000fde0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-0000fdf0: 6973 2060 7465 7374 7275 6e5f 3232 3131  is `testrun_2211
-0000fe00: 3038 2d31 3230 3430 342d 3764 3260 2c20  08-120404-7d2`, 
-0000fe10: 7468 6520 5461 736b 2047 726f 7570 2069  the Task Group i
-0000fe20: 7320 6074 6173 6b5f 6772 6f75 705f 3160  s `task_group_1`
-0000fe30: 2061 6e64 2074 6865 2054 6173 6b20 6973   and the Task is
-0000fe40: 2060 7461 736b 5f31 602c 2074 6865 6e20   `task_1`, then 
-0000fe50: 7468 6520 6669 6c65 7320 6162 6f76 6520  the files above 
-0000fe60: 776f 756c 6420 6265 2075 706c 6f61 6465  would be uploade
-0000fe70: 6420 746f 2074 6865 204f 626a 6563 7420  d to the Object 
-0000fe80: 5374 6f72 6520 6173 2066 6f6c 6c6f 7773  Store as follows
-0000fe90: 3a0a 0a60 6060 7368 656c 6c0a 6465 7665  :..```shell.deve
-0000fea0: 6c6f 706d 656e 743a 3a74 6573 7472 756e  lopment::testrun
-0000feb0: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
-0000fec0: 6432 2f74 6173 6b5f 6772 6f75 705f 312f  d2/task_group_1/
-0000fed0: 7461 736b 5f31 2f72 6573 756c 7473 2f6f  task_1/results/o
-0000fee0: 7065 6e66 6f61 6d2e 7461 722e 677a 0a64  penfoam.tar.gz.d
-0000fef0: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
-0000ff00: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000ff10: 342d 3764 322f 7461 736b 5f67 726f 7570  4-7d2/task_group
-0000ff20: 5f31 2f74 6173 6b5f 312f 7265 7375 6c74  _1/task_1/result
-0000ff30: 732f 6f70 656e 666f 616d 2e6c 6f67 0a64  s/openfoam.log.d
-0000ff40: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
-0000ff50: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000ff60: 342d 3764 322f 7461 736b 5f67 726f 7570  4-7d2/task_group
-0000ff70: 5f31 2f74 6173 6b5f 312f 7461 736b 6f75  _1/task_1/taskou
-0000ff80: 7470 7574 2e74 7874 0a60 6060 0a0a 5468  tput.txt.```..Th
-0000ff90: 6520 2a2a 606f 7574 7075 7473 5265 7175  e **`outputsRequ
-0000ffa0: 6972 6564 602a 2a20 7072 6f70 6572 7479  ired`** property
-0000ffb0: 2063 616e 2062 6520 7573 6564 2069 6e73   can be used ins
-0000ffc0: 7465 6164 206f 6620 286f 7220 696e 2061  tead of (or in a
-0000ffd0: 6464 6974 696f 6e20 746f 2920 7468 6520  ddition to) the 
-0000ffe0: 606f 7574 7075 7473 6020 7072 6f70 6572  `outputs` proper
-0000fff0: 7479 2c20 6966 2074 6865 206f 7574 7075  ty, if the outpu
-00010000: 7420 6669 6c65 2873 2920 2a2a 6d75 7374  t file(s) **must
-00010010: 2a2a 2062 6520 6176 6169 6c61 626c 6520  ** be available 
-00010020: 666f 7220 7570 6c6f 6164 2074 6f20 7468  for upload to th
-00010030: 6520 4f62 6a65 6374 2053 746f 7265 2061  e Object Store a
-00010040: 7420 7468 6520 636f 6e63 6c75 7369 6f6e  t the conclusion
-00010050: 206f 6620 7468 6520 5461 736b 206f 7220   of the Task or 
-00010060: 7468 6520 5461 736b 2077 696c 6c20 6265  the Task will be
-00010070: 206d 6172 6b65 6420 6173 2060 4661 696c   marked as `Fail
-00010080: 6564 602c 2065 2e67 2e3a 0a0a 6022 6f75  ed`, e.g.:..`"ou
-00010090: 7470 7574 7352 6571 7569 7265 6422 3a20  tputsRequired": 
-000100a0: 5b22 7265 7375 6c74 732f 7072 6f63 6573  ["results/proces
-000100b0: 735f 6f75 7470 7574 2e74 7874 225d 600a  s_output.txt"]`.
-000100c0: 0a23 2323 2046 696c 6573 2044 6f77 6e6c  .### Files Downl
-000100d0: 6f61 6465 6420 6672 6f6d 2074 6865 204f  oaded from the O
-000100e0: 626a 6563 7420 5374 6f72 6520 746f 204c  bject Store to L
-000100f0: 6f63 616c 2053 746f 7261 6765 0a0a 5468  ocal Storage..Th
-00010100: 6520 6079 642d 646f 776e 6c6f 6164 6020  e `yd-download` 
-00010110: 636f 6d6d 616e 6420 7769 6c6c 2064 6f77  command will dow
-00010120: 6e6c 6f61 6420 616c 6c20 6f62 6a65 6374  nload all object
-00010130: 7320 6672 6f6d 2074 6865 204f 626a 6563  s from the Objec
-00010140: 7420 5374 6f72 6520 746f 2061 206c 6f63  t Store to a loc
-00010150: 616c 2064 6972 6563 746f 7279 2c20 6f6e  al directory, on
-00010160: 2061 2070 6572 2057 6f72 6b20 5265 7175   a per Work Requ
-00010170: 6972 656d 656e 7420 6261 7369 7320 2869  irement basis (i
-00010180: 6e63 6c75 6469 6e67 2061 6e79 2066 696c  ncluding any fil
-00010190: 6573 2074 6861 7420 6861 7665 2062 6565  es that have bee
-000101a0: 6e20 7570 6c6f 6164 6564 292e 2041 206c  n uploaded). A l
-000101b0: 6f63 616c 2064 6972 6563 746f 7279 2069  ocal directory i
-000101c0: 7320 6372 6561 7465 6420 7769 7468 2074  s created with t
-000101d0: 6865 2073 616d 6520 6e61 6d65 2061 7320  he same name as 
-000101e0: 7468 6520 4e61 6d65 7370 6163 6520 616e  the Namespace an
-000101f0: 6420 636f 6e74 6169 6e69 6e67 2074 6865  d containing the
-00010200: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00010210: 7420 6469 7265 6374 6f72 6965 732e 0a0a  t directories...
-00010220: 5573 6520 7468 6520 602d 2d69 6e74 6572  Use the `--inter
-00010230: 6163 7469 7665 6020 6f70 7469 6f6e 2077  active` option w
-00010240: 6974 6820 6079 642d 646f 776e 6c6f 6164  ith `yd-download
-00010250: 6020 746f 2073 656c 6563 7420 7768 6963  ` to select whic
-00010260: 6820 576f 726b 2052 6571 7569 7265 6d65  h Work Requireme
-00010270: 6e74 2873 2920 746f 2064 6f77 6e6c 6f61  nt(s) to downloa
-00010280: 642e 0a0a 466f 7220 7468 6520 6578 616d  d...For the exam
-00010290: 706c 6520 6162 6f76 652c 2060 7964 2d64  ple above, `yd-d
-000102a0: 6f77 6e6c 6f61 6460 2077 6f75 6c64 2063  ownload` would c
-000102b0: 7265 6174 6520 6120 6469 7265 6374 6f72  reate a director
-000102c0: 7920 6361 6c6c 6564 2060 6465 7665 6c6f  y called `develo
-000102d0: 706d 656e 7460 2069 6e20 7468 6520 6375  pment` in the cu
-000102e0: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
-000102f0: 7265 6374 6f72 792c 2063 6f6e 7461 696e  rectory, contain
-00010300: 696e 6720 736f 6d65 7468 696e 6720 6c69  ing something li
-00010310: 6b65 3a0a 0a60 6060 7368 656c 6c0a 6465  ke:..```shell.de
-00010320: 7665 6c6f 706d 656e 740a e294 94e2 9480  velopment.......
-00010330: e294 8020 7465 7374 7275 6e5f 3232 3131  ... testrun_2211
-00010340: 3038 2d31 3230 3430 342d 3764 320a 2020  08-120404-7d2.  
-00010350: 2020 e294 9ce2 9480 e294 8020 6261 7368    ......... bash
-00010360: 5f73 6372 6970 742e 7368 0a20 2020 20e2  _script.sh.    .
-00010370: 949c e294 80e2 9480 2066 696c 655f 312e  ........ file_1.
-00010380: 7478 740a 2020 2020 e294 94e2 9480 e294  txt.    ........
-00010390: 8020 7461 736b 5f67 726f 7570 5f31 0a20  . task_group_1. 
-000103a0: 2020 2020 2020 20e2 9494 e294 80e2 9480         .........
-000103b0: 2074 6173 6b5f 310a 2020 2020 2020 2020   task_1.        
-000103c0: 2020 2020 e294 9ce2 9480 e294 8020 7265      ......... re
-000103d0: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
-000103e0: 2020 e294 82c2 a0c2 a020 e294 9ce2 9480    ....... ......
-000103f0: e294 8020 6f70 656e 666f 616d 2e6c 6f67  ... openfoam.log
-00010400: 0a20 2020 2020 2020 2020 2020 20e2 9482  .            ...
-00010410: c2a0 c2a0 20e2 9494 e294 80e2 9480 206f  .... ......... o
-00010420: 7065 6e66 6f61 6d2e 7461 722e 677a 0a20  penfoam.tar.gz. 
-00010430: 2020 2020 2020 2020 2020 20e2 9494 e294             .....
-00010440: 80e2 9480 2074 6173 6b6f 7574 7075 742e  .... taskoutput.
-00010450: 7478 740a 6060 600a 0a4e 6f74 6520 7468  txt.```..Note th
-00010460: 6174 2065 7665 7279 7468 696e 6720 7769  at everything wi
-00010470: 7468 696e 2074 6865 2060 6e61 6d65 7370  thin the `namesp
-00010480: 6163 653a 3a77 6f72 6b2d 7265 7175 6972  ace::work-requir
-00010490: 656d 656e 7460 2064 6972 6563 746f 7279  ement` directory
-000104a0: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
-000104b0: 746f 7265 2069 7320 646f 776e 6c6f 6164  tore is download
-000104c0: 6564 2c20 696e 636c 7564 696e 6720 616e  ed, including an
-000104d0: 7920 6669 6c65 7320 7468 6174 2077 6572  y files that wer
-000104e0: 6520 7370 6563 6966 6965 6420 696e 2060  e specified in `
-000104f0: 696e 7075 7473 6020 616e 6420 7570 6c6f  inputs` and uplo
-00010500: 6164 6564 2061 7320 7061 7274 206f 6620  aded as part of 
-00010510: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-00010520: 6d65 6e74 2073 7562 6d69 7373 696f 6e2e  ment submission.
-00010530: 204d 756c 7469 706c 6520 5461 736b 2047   Multiple Task G
-00010540: 726f 7570 732c 2061 6e64 206d 756c 7469  roups, and multi
-00010550: 706c 6520 5461 736b 7320 7769 6c6c 2061  ple Tasks will a
-00010560: 6c6c 2061 7070 6561 7220 696e 2074 6865  ll appear in the
-00010570: 2064 6972 6563 746f 7279 2073 7472 7563   directory struc
-00010580: 7475 7265 2e0a 0a49 6620 7468 6520 6064  ture...If the `d
-00010590: 6576 656c 6f70 6d65 6e74 6020 6469 7265  evelopment` dire
-000105a0: 6374 6f72 7920 616c 7265 6164 7920 6578  ctory already ex
-000105b0: 6973 7473 2c20 6079 642d 646f 776e 6c6f  ists, `yd-downlo
-000105c0: 6164 6020 7769 6c6c 2074 7279 2060 6465  ad` will try `de
-000105d0: 7665 6c6f 706d 656e 742e 3031 602c 2065  velopment.01`, e
-000105e0: 7463 2e2c 2074 6f20 6176 6f69 6420 6f76  tc., to avoid ov
-000105f0: 6572 7772 6974 696e 6720 7072 6576 696f  erwriting previo
-00010600: 7573 2064 6f77 6e6c 6f61 6473 2e0a 0a23  us downloads...#
-00010610: 2320 5461 736b 2045 7865 6375 7469 6f6e  # Task Execution
-00010620: 2043 6f6e 7465 7874 0a0a 5468 6973 2073   Context..This s
-00010630: 6563 7469 6f6e 2064 6973 6375 7373 6573  ection discusses
-00010640: 2074 6865 2063 6f6e 7465 7874 2077 6974   the context wit
-00010650: 6869 6e20 7768 6963 6820 6120 5461 736b  hin which a Task
-00010660: 206f 7065 7261 7465 7320 7768 656e 2069   operates when i
-00010670: 7427 7320 6578 6563 7574 6564 2062 7920  t's executed by 
-00010680: 6120 576f 726b 6572 206f 6e20 6120 6e6f  a Worker on a no
-00010690: 6465 2e20 4974 2061 7070 6c69 6573 2073  de. It applies s
-000106a0: 7065 6369 6669 6361 6c6c 7920 746f 2074  pecifically to t
-000106b0: 6865 2059 656c 6c6f 7744 6f67 2041 6765  he YellowDog Age
-000106c0: 6e74 2072 756e 6e69 6e67 206f 6e20 6120  nt running on a 
-000106d0: 4c69 6e75 7820 6e6f 6465 2c20 616e 6420  Linux node, and 
-000106e0: 636f 6e66 6967 7572 6564 2075 7369 6e67  configured using
-000106f0: 2074 6865 2064 6566 6175 6c74 2075 7365   the default use
-00010700: 726e 616d 652c 2064 6972 6563 746f 7269  rname, directori
-00010710: 6573 2c20 6574 632e 2043 6f6e 6669 6775  es, etc. Configu
-00010720: 7261 7469 6f6e 7320 6361 6e20 7661 7279  rations can vary
-00010730: 2e0a 0a23 2323 2054 6173 6b20 4578 6563  ...### Task Exec
-00010740: 7574 696f 6e20 5374 6570 730a 0a57 6865  ution Steps..Whe
-00010750: 6e20 6120 5461 736b 2069 7320 616c 6c6f  n a Task is allo
-00010760: 6361 7465 6420 746f 2061 2057 6f72 6b65  cated to a Worke
-00010770: 7220 6f6e 2061 206e 6f64 6520 6279 2074  r on a node by t
-00010780: 6865 2059 656c 6c6f 7744 6f67 2053 6368  he YellowDog Sch
-00010790: 6564 756c 6572 2c20 7468 6520 666f 6c6c  eduler, the foll
-000107a0: 6f77 696e 6720 7374 6570 7320 6172 6520  owing steps are 
-000107b0: 666f 6c6c 6f77 6564 3a0a 0a31 2e20 5468  followed:..1. Th
-000107c0: 6520 4167 656e 7420 7275 6e6e 696e 6720  e Agent running 
-000107d0: 6f6e 2074 6865 206e 6f64 6520 646f 776e  on the node down
-000107e0: 6c6f 6164 7320 7468 6520 5461 736b 2773  loads the Task's
-000107f0: 2070 726f 7065 7274 6965 733a 2069 7473   properties: its
-00010800: 2060 7461 736b 5479 7065 602c 2020 6061   `taskType`,  `a
-00010810: 7267 756d 656e 7473 602c 2060 656e 7669  rguments`, `envi
-00010820: 726f 6e6d 656e 7460 2c20 6074 6173 6b64  ronment`, `taskd
-00010830: 6174 6160 2c20 616e 6420 2866 726f 6d20  ata`, and (from 
-00010840: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
-00010850: 2920 616e 7920 6669 6c65 7320 696e 2074  ) any files in t
-00010860: 6865 2060 696e 7075 7473 6020 6c69 7374  he `inputs` list
-00010870: 2061 6e64 2061 6e79 2061 7661 696c 6162   and any availab
-00010880: 6c65 2066 696c 6573 2069 6e20 7468 6520  le files in the 
-00010890: 6069 6e70 7574 734f 7074 696f 6e61 6c60  `inputsOptional`
-000108a0: 206c 6973 742e 0a32 2e20 5468 6573 6520   list..2. These 
-000108b0: 6669 6c65 7320 6172 6520 706c 6163 6564  files are placed
-000108c0: 2069 6e20 616e 2065 7068 656d 6572 616c   in an ephemeral
-000108d0: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
-000108e0: 6564 2066 6f72 2074 6869 7320 5461 736b  ed for this Task
-000108f0: 2773 2065 7865 6375 7469 6f6e 2c20 616e  's execution, an
-00010900: 6420 696e 746f 2077 6869 6368 2061 6e79  d into which any
-00010910: 206f 7574 7075 7420 6669 6c65 7320 6172   output files ar
-00010920: 6520 616c 736f 2070 6c61 6365 6420 6279  e also placed by
-00010930: 2064 6566 6175 6c74 2e0a 322e 2054 6865   default..2. The
-00010940: 2041 6765 6e74 2072 756e 7320 7468 6520   Agent runs the 
-00010950: 636f 6d6d 616e 6420 7370 6563 6966 6965  command specifie
-00010960: 6420 666f 7220 7468 6520 6074 6173 6b54  d for the `taskT
-00010970: 7970 6560 2069 6e20 7468 6520 4167 656e  ype` in the Agen
-00010980: 7427 7320 6061 7070 6c69 6361 7469 6f6e  t's `application
-00010990: 2e79 616d 6c60 2063 6f6e 6669 6775 7261  .yaml` configura
-000109a0: 7469 6f6e 2066 696c 652e 2054 6869 7320  tion file. This 
-000109b0: 646f 6e65 2061 7320 6120 7369 6d70 6c65  done as a simple
-000109c0: 2060 6578 6563 6020 6f66 2061 2073 7562   `exec` of a sub
-000109d0: 7072 6f63 6573 732e 0a33 2e20 5768 656e  process..3. When
-000109e0: 2074 6865 2054 6173 6b20 636f 6e63 6c75   the Task conclu
-000109f0: 6465 732c 2074 6865 2041 6765 6e74 2075  des, the Agent u
-00010a00: 7365 7320 7468 6520 6578 6974 2063 6f64  ses the exit cod
-00010a10: 6520 6f66 2074 6865 2073 7562 7072 6f63  e of the subproc
-00010a20: 6573 7320 746f 2072 6570 6f72 7420 7375  ess to report su
-00010a30: 6363 6573 7320 287a 6572 6f29 206f 7220  ccess (zero) or 
-00010a40: 6661 696c 7572 6520 286e 6f6e 2d7a 6572  failure (non-zer
-00010a50: 6f29 2e0a 342e 2054 6865 2041 6765 6e74  o)..4. The Agent
-00010a60: 2074 6865 6e20 6761 7468 6572 7320 616e   then gathers an
-00010a70: 7920 6669 6c65 7320 696e 2074 6865 2060  y files in the `
-00010a80: 6f75 7470 7574 7360 2061 6e64 2060 6f75  outputs` and `ou
-00010a90: 7470 7574 7352 6571 7569 7265 6460 206c  tputsRequired` l
-00010aa0: 6973 7473 2061 6e64 2075 706c 6f61 6473  ists and uploads
-00010ab0: 2074 6865 6d20 746f 2074 6865 204f 626a   them to the Obj
-00010ac0: 6563 7420 5374 6f72 652e 2049 6620 6120  ect Store. If a 
-00010ad0: 6669 6c65 2069 6e20 7468 6520 606f 7574  file in the `out
-00010ae0: 7075 7473 5265 7175 6972 6564 6020 6c69  putsRequired` li
-00010af0: 7374 2069 7320 6e6f 7420 666f 756e 642c  st is not found,
-00010b00: 2074 6865 2054 6173 6b20 7769 6c6c 2062   the Task will b
-00010b10: 6520 7265 706f 7274 6564 2061 7320 6661  e reported as fa
-00010b20: 696c 6564 2e20 5468 6520 4167 656e 7420  iled. The Agent 
-00010b30: 7769 6c6c 2061 6c73 6f20 6f70 7469 6f6e  will also option
-00010b40: 616c 6c79 2075 706c 6f61 6420 7468 6520  ally upload the 
-00010b50: 636f 6e73 6f6c 6520 6f75 7470 7574 2028  console output (
-00010b60: 696e 636c 7564 696e 6720 626f 7468 2060  including both `
-00010b70: 7374 646f 7574 6020 616e 6420 6073 7464  stdout` and `std
-00010b80: 6572 7260 2920 6f66 2074 6865 2054 6173  err`) of the Tas
-00010b90: 6b2c 2063 6f6e 7461 696e 6564 2069 6e20  k, contained in 
-00010ba0: 7468 6520 6074 6173 6b6f 7574 7075 742e  the `taskoutput.
-00010bb0: 7478 7460 2066 696c 652e 0a35 2e20 5468  txt` file..5. Th
-00010bc0: 6520 6570 6865 6d65 7261 6c20 5461 736b  e ephemeral Task
-00010bd0: 2064 6972 6563 746f 7279 2069 7320 7468   directory is th
-00010be0: 656e 2064 656c 6574 6564 2e0a 0a4e 6f74  en deleted...Not
-00010bf0: 6520 7468 6174 2069 6620 6120 5461 736b  e that if a Task
-00010c00: 2069 7320 6162 6f72 7465 6420 6475 7269   is aborted duri
-00010c10: 6e67 2065 7865 6375 7469 6f6e 2c20 7468  ng execution, th
-00010c20: 6520 5461 736b 2773 2073 7562 7072 6f63  e Task's subproc
-00010c30: 6573 7320 6973 2073 656e 7420 6120 6053  ess is sent a `S
-00010c40: 4947 494e 5460 2c20 616c 6c6f 7769 6e67  IGINT`, allowing
-00010c50: 2074 6865 2054 6173 6b20 616e 206f 7070   the Task an opp
-00010c60: 6f72 7475 6e69 7479 2074 6f20 7465 726d  ortunity to term
-00010c70: 696e 6174 6520 616e 7920 6368 696c 6420  inate any child 
-00010c80: 7072 6f63 6573 7365 7320 6f72 206f 7468  processes or oth
-00010c90: 6572 2072 6573 6f75 7263 6573 2028 652e  er resources (e.
-00010ca0: 672e 2c20 636f 6e74 6169 6e65 7273 2920  g., containers) 
-00010cb0: 7468 6174 206d 6179 2068 6176 6520 6265  that may have be
-00010cc0: 656e 2073 7461 7274 6564 2061 7320 7061  en started as pa
-00010cd0: 7274 206f 6620 5461 736b 2065 7865 6375  rt of Task execu
-00010ce0: 7469 6f6e 2e0a 0a4f 6e63 6520 7468 6520  tion...Once the 
-00010cf0: 7374 6570 7320 6162 6f76 6520 6861 7665  steps above have
-00010d00: 2062 6565 6e20 636f 6d70 6c65 7465 642c   been completed,
-00010d10: 2074 6865 2057 6f72 6b65 7220 6973 2072   the Worker is r
-00010d20: 6561 6479 2074 6f20 6163 6365 7074 2069  eady to accept i
-00010d30: 7473 206e 6578 7420 5461 736b 2066 726f  ts next Task fro
-00010d40: 6d20 7468 6520 5965 6c6c 6f77 446f 6720  m the YellowDog 
-00010d50: 7363 6865 6475 6c65 722e 0a0a 4e6f 7465  scheduler...Note
-00010d60: 2074 6861 7420 6966 2074 6865 2041 6765   that if the Age
-00010d70: 6e74 206f 6e20 6120 6e6f 6465 2068 6173  nt on a node has
-00010d80: 206d 756c 7469 706c 6520 576f 726b 6572   multiple Worker
-00010d90: 732c 2074 6865 6e20 5461 736b 7320 6172  s, then Tasks ar
-00010da0: 6520 6578 6563 7574 6564 2069 6e20 7061  e executed in pa
-00010db0: 7261 6c6c 656c 206f 6e20 7468 6520 6e6f  rallel on the no
-00010dc0: 6465 2061 6e64 2063 616e 2073 7461 7274  de and can start
-00010dd0: 2061 6e64 2073 746f 7020 696e 6465 7065   and stop indepe
-00010de0: 6e64 656e 746c 792e 0a0a 2323 2320 5468  ndently...### Th
-00010df0: 6520 5573 6572 2061 6e64 2047 726f 7570  e User and Group
-00010e00: 2075 7365 6420 666f 7220 5461 736b 730a   used for Tasks.
-00010e10: 0a42 7920 6465 6661 756c 742c 2074 6865  .By default, the
-00010e20: 2041 6765 6e74 2072 756e 7320 6173 2075   Agent runs as u
-00010e30: 7365 7220 616e 6420 6772 6f75 7020 6079  ser and group `y
-00010e40: 642d 6167 656e 7460 2c20 616e 6420 6865  d-agent`, and he
-00010e50: 6e63 6520 5461 736b 7320 616c 736f 2065  nce Tasks also e
-00010e60: 7865 6375 7465 2075 6e64 6572 2074 6869  xecute under thi
-00010e70: 7320 7573 6572 2e0a 0a60 7964 2d61 6765  s user...`yd-age
-00010e80: 6e74 6020 646f 6573 206e 6f74 2068 6176  nt` does not hav
-00010e90: 6520 6073 7564 6f60 2070 7269 7669 6c65  e `sudo` privile
-00010ea0: 6765 7320 6173 2073 7461 6e64 6172 642c  ges as standard,
-00010eb0: 2062 7574 2074 6869 7320 6361 6e20 6265   but this can be
-00010ec0: 2061 6464 6564 2069 6620 7265 7175 6972   added if requir
-00010ed0: 6564 2061 7420 696e 7374 616e 6365 2062  ed at instance b
-00010ee0: 6f6f 7420 7469 6d65 2076 6961 2074 6865  oot time via the
-00010ef0: 2060 7573 6572 4461 7461 6020 7072 6f70   `userData` prop
-00010f00: 6572 7479 206f 6620 6120 7072 6f76 6973  erty of a provis
-00010f10: 696f 6e69 6e67 2072 6571 7565 7374 2e20  ioning request. 
-00010f20: 452e 672e 2028 666f 7220 5562 756e 7475  E.g. (for Ubuntu
-00010f30: 293a 0a0a 6060 6073 6865 6c6c 0a75 7365  ):..```shell.use
-00010f40: 726d 6f64 202d 6147 2077 6865 656c 2079  rmod -aG wheel y
-00010f50: 642d 6167 656e 740a 6563 686f 202d 6520  d-agent.echo -e 
-00010f60: 2279 642d 6167 656e 745c 7441 4c4c 3d28  "yd-agent\tALL=(
-00010f70: 414c 4c29 5c74 4e4f 5041 5353 5744 3a20  ALL)\tNOPASSWD: 
-00010f80: 414c 4c22 203e 202f 6574 632f 7375 646f  ALL" > /etc/sudo
-00010f90: 6572 732e 642f 3032 302d 7964 2d61 6765  ers.d/020-yd-age
-00010fa0: 6e74 0a60 6060 0a0a 2323 2320 486f 6d65  nt.```..### Home
-00010fb0: 2044 6972 6563 746f 7279 2066 6f72 2060   Directory for `
-00010fc0: 7964 2d61 6765 6e74 600a 0a42 7920 6465  yd-agent`..By de
-00010fd0: 6661 756c 742c 2074 6865 2068 6f6d 6520  fault, the home 
-00010fe0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
-00010ff0: 2060 7964 2d61 6765 6e74 6020 7573 6572   `yd-agent` user
-00011000: 2069 7320 602f 6f70 742f 7965 6c6c 6f77   is `/opt/yellow
-00011010: 646f 672f 6167 656e 7460 2e20 5468 6973  dog/agent`. This
-00011020: 2064 6972 6563 746f 7279 2074 7970 6963   directory typic
-00011030: 616c 6c79 2063 6f6e 7461 696e 7320 7468  ally contains th
-00011040: 6520 6061 7070 6c69 6361 7469 6f6e 2e79  e `application.y
-00011050: 616d 6c60 2066 696c 6520 7573 6564 2074  aml` file used t
-00011060: 6f20 636f 6e66 6967 7572 6520 7468 6520  o configure the 
-00011070: 4167 656e 742c 2061 7320 7765 6c6c 2061  Agent, as well a
-00011080: 7320 616e 7920 7363 7269 7074 7320 7468  s any scripts th
-00011090: 6174 2061 7265 2075 7365 6420 746f 2065  at are used to e
-000110a0: 7865 6375 7465 2074 6865 2054 6173 6b20  xecute the Task 
-000110b0: 5479 7065 7320 7468 6174 2074 6865 206e  Types that the n
-000110c0: 6f64 6520 7375 7070 6f72 7473 2e0a 0a49  ode supports...I
-000110d0: 6620 6f6e 6520 7761 6e74 7320 746f 2053  f one wants to S
-000110e0: 5348 2074 6f20 616e 2069 6e73 7461 6e63  SH to an instanc
-000110f0: 6520 6173 2075 7365 7220 6079 642d 6167  e as user `yd-ag
-00011100: 656e 7460 2c20 7065 7268 6170 7320 666f  ent`, perhaps fo
-00011110: 7220 6465 6275 6767 696e 6720 7075 7270  r debugging purp
-00011120: 6f73 6573 2c20 5353 4820 6b65 7973 2063  oses, SSH keys c
-00011130: 616e 2062 6520 696e 7365 7274 6564 2076  an be inserted v
-00011140: 6961 2069 6e73 7461 6e63 6520 6075 7365  ia instance `use
-00011150: 7244 6174 6160 2c20 652e 672e 3a0a 0a60  rData`, e.g.:..`
-00011160: 6060 7368 656c 6c0a 5944 415f 484f 4d45  ``shell.YDA_HOME
-00011170: 3d2f 6f70 742f 7965 6c6c 6f77 646f 672f  =/opt/yellowdog/
-00011180: 6167 656e 740a 6d6b 6469 7220 2d70 2024  agent.mkdir -p $
-00011190: 5944 415f 484f 4d45 2f2e 7373 680a 6368  YDA_HOME/.ssh.ch
-000111a0: 6d6f 6420 6f67 2d72 7778 2024 5944 415f  mod og-rwx $YDA_
-000111b0: 484f 4d45 2f2e 7373 680a 6361 7420 3e3e  HOME/.ssh.cat >>
-000111c0: 2024 5944 415f 484f 4d45 2f2e 7373 682f   $YDA_HOME/.ssh/
-000111d0: 6175 7468 6f72 697a 6564 5f6b 6579 7320  authorized_keys 
-000111e0: 3c3c 2045 4f46 0a3c 3c49 6e73 6572 745f  << EOF.<<Insert_
-000111f0: 5075 626c 6963 5f6b 6579 5f48 6572 653e  Public_key_Here>
-00011200: 3e0a 454f 460a 6368 6d6f 6420 6f67 2d72  >.EOF.chmod og-r
-00011210: 7720 2459 4441 5f48 4f4d 452f 2e73 7368  w $YDA_HOME/.ssh
-00011220: 2f61 7574 686f 7269 7a65 645f 6b65 7973  /authorized_keys
-00011230: 0a63 686f 776e 202d 5220 7964 2d61 6765  .chown -R yd-age
-00011240: 6e74 3a79 642d 6167 656e 7420 2459 4441  nt:yd-agent $YDA
-00011250: 5f48 4f4d 452f 2e73 7368 0a60 6060 0a0a  _HOME/.ssh.```..
-00011260: 2323 2320 5461 736b 2045 7865 6375 7469  ### Task Executi
-00011270: 6f6e 2044 6972 6563 746f 7279 0a0a 4570  on Directory..Ep
-00011280: 6865 6d65 7261 6c20 5461 736b 2064 6972  hemeral Task dir
-00011290: 6563 746f 7269 6573 2061 7265 2062 7920  ectories are by 
-000112a0: 6465 6661 756c 7420 6372 6561 7465 6420  default created 
-000112b0: 756e 6465 7220 602f 7661 722f 6f70 742f  under `/var/opt/
-000112c0: 7965 6c6c 6f77 646f 672f 6167 656e 742f  yellowdog/agent/
-000112d0: 6461 7461 2f77 6f72 6b65 7273 602e 2054  data/workers`. T
-000112e0: 6869 7320 6469 7265 6374 6f72 7920 636f  his directory co
-000112f0: 6e74 6169 6e73 206f 6e65 206f 7220 6d6f  ntains one or mo
-00011300: 7265 206e 756d 6265 7265 6420 7375 6264  re numbered subd
-00011310: 6972 6563 746f 7269 6573 2077 6865 7265  irectories where
-00011320: 2065 6163 6820 6e75 6d62 6572 6564 2064   each numbered d
-00011330: 6972 6563 746f 7279 2063 6f72 7265 7370  irectory corresp
-00011340: 6f6e 6473 2074 6f20 6120 576f 726b 6572  onds to a Worker
-00011350: 206f 6e20 7468 6520 6e6f 6465 2e0a 0a28   on the node...(
-00011360: 4f6e 2057 696e 646f 7773 2068 6f73 7473  On Windows hosts
-00011370: 2c20 7468 6520 5461 736b 2064 6972 6563  , the Task direc
-00011380: 746f 7269 6573 2061 7265 2066 6f75 6e64  tories are found
-00011390: 2075 6e64 6572 2060 2541 7070 4461 7461   under `%AppData
-000113a0: 255c 7965 6c6c 6f77 646f 675c 6167 656e  %\yellowdog\agen
-000113b0: 745c 6461 7461 5c77 6f72 6b65 7273 602e  t\data\workers`.
-000113c0: 290a 0a57 6865 6e20 6120 5461 736b 2069  )..When a Task i
-000113d0: 7320 616c 6c6f 6361 7465 6420 746f 2061  s allocated to a
-000113e0: 206e 6f64 652c 2061 6e20 6570 6865 6d65   node, an epheme
-000113f0: 7261 6c20 6469 7265 6374 6f72 7920 6973  ral directory is
-00011400: 2063 7265 6174 6564 2075 6e64 6572 2074   created under t
-00011410: 6865 2061 7070 6c69 6361 626c 6520 576f  he applicable Wo
-00011420: 726b 6572 2064 6972 6563 746f 7279 2c20  rker directory, 
-00011430: 7769 7468 2061 206e 616d 6520 636f 7272  with a name corr
-00011440: 6573 706f 6e64 696e 6720 7468 6520 5965  esponding the Ye
-00011450: 6c6c 6f77 446f 6720 4944 2066 6f72 2074  llowDog ID for t
-00011460: 6865 2054 6173 6b2e 2046 6f72 2065 7861  he Task. For exa
-00011470: 6d70 6c65 2c20 7468 6973 2069 7320 616e  mple, this is an
-00011480: 2065 7068 656d 6572 616c 2064 6972 6563   ephemeral direc
-00011490: 746f 7279 2062 6569 6e67 2075 7365 6420  tory being used 
-000114a0: 6279 2057 6f72 6b65 7220 6e75 6d62 6572  by Worker number
-000114b0: 2060 3160 3a0a 0a60 2f76 6172 2f6f 7074   `1`:..`/var/opt
-000114c0: 2f79 656c 6c6f 7764 6f67 2f61 6765 6e74  /yellowdog/agent
-000114d0: 2f64 6174 612f 776f 726b 6572 732f 312f  /data/workers/1/
-000114e0: 7964 6964 5f74 6173 6b5f 3535 3945 4245  ydid_task_559EBE
-000114f0: 5f37 3439 3439 3333 362d 6163 3262 2d34  _74949336-ac2b-4
-00011500: 3831 312d 6137 6435 2d66 3365 6364 3937  811-a7d5-f3ecd97
-00011510: 3339 3930 385f 315f 3160 0a0a 5468 6973  39908_1_1`..This
-00011520: 2069 7320 7468 6520 6469 7265 6374 6f72   is the director
-00011530: 7920 696e 746f 2077 6869 6368 2064 6f77  y into which dow
-00011540: 6e6c 6f61 6465 6420 6f62 6a65 6374 7320  nloaded objects 
-00011550: 6172 6520 706c 6163 6564 2c20 616e 6420  are placed, and 
-00011560: 696e 2077 6869 6368 206f 7574 7075 7420  in which output 
-00011570: 6669 6c65 7320 6172 6520 6372 6561 7465  files are create
-00011580: 6420 6279 2064 6566 6175 6c74 2e20 5468  d by default. Th
-00011590: 6520 636f 6e73 6f6c 6520 6f75 7470 7574  e console output
-000115a0: 2060 7461 736b 6f75 7470 7574 2e74 7874   `taskoutput.txt
-000115b0: 6020 6669 6c65 2077 696c 6c20 616c 736f  ` file will also
-000115c0: 2062 6520 6372 6561 7465 6420 696e 2074   be created in t
-000115d0: 6869 7320 6469 7265 6374 6f72 792e 0a0a  his directory...
-000115e0: 5365 6520 7468 6520 5b46 696c 6573 2044  See the [Files D
-000115f0: 6f77 6e6c 6f61 6465 6420 746f 2061 204e  ownloaded to a N
-00011600: 6f64 655d 2823 6669 6c65 732d 646f 776e  ode](#files-down
-00011610: 6c6f 6164 6564 2d74 6f2d 612d 6e6f 6465  loaded-to-a-node
-00011620: 2d66 6f72 2d75 7365 2d69 6e2d 7461 736b  -for-use-in-task
-00011630: 2d65 7865 6375 7469 6f6e 2920 7365 6374  -execution) sect
-00011640: 696f 6e20 6162 6f76 6520 666f 7220 6d6f  ion above for mo
-00011650: 7265 2064 6574 6169 6c73 206f 6e20 686f  re details on ho
-00011660: 7720 6669 6c65 7320 696e 2074 6869 7320  w files in this 
-00011670: 6469 7265 6374 6f72 7920 6172 6520 6861  directory are ha
-00011680: 6e64 6c65 642e 0a0a 4174 2074 6865 2063  ndled...At the c
-00011690: 6f6e 636c 7573 696f 6e20 6f66 2074 6865  onclusion of the
-000116a0: 2054 6173 6b2c 2061 6674 6572 2061 6e79   Task, after any
-000116b0: 2066 696c 6573 2072 6571 7565 7374 6564   files requested
-000116c0: 2066 6f72 2075 706c 6f61 6420 6861 7665   for upload have
-000116d0: 2062 6565 6e20 7570 6c6f 6164 6564 2074   been uploaded t
-000116e0: 6f20 7468 6520 4f62 6a65 6374 2053 746f  o the Object Sto
-000116f0: 7265 2028 7365 6520 7468 6520 5b46 696c  re (see the [Fil
-00011700: 6573 2055 706c 6f61 6465 6420 6672 6f6d  es Uploaded from
-00011710: 2061 204e 6f64 655d 2823 6669 6c65 732d   a Node](#files-
-00011720: 7570 6c6f 6164 6564 2d66 726f 6d2d 612d  uploaded-from-a-
-00011730: 6e6f 6465 2d74 6f2d 7468 652d 6f62 6a65  node-to-the-obje
-00011740: 6374 2d73 746f 7265 2d61 6674 6572 2d74  ct-store-after-t
-00011750: 6173 6b2d 6578 6563 7574 696f 6e29 2073  ask-execution) s
-00011760: 6563 7469 6f6e 2066 6f72 206d 6f72 6520  ection for more 
-00011770: 696e 666f 726d 6174 696f 6e29 2c20 7468  information), th
-00011780: 6520 6079 6469 645f 7461 736b 5f35 3539  e `ydid_task_559
-00011790: 4542 455f 3734 3934 3933 3336 2d61 6332  EBE_74949336-ac2
-000117a0: 622d 3438 3131 2d61 3764 352d 6633 6563  b-4811-a7d5-f3ec
-000117b0: 6439 3733 3939 3038 5f31 5f31 6020 7769  d9739908_1_1` wi
-000117c0: 6c6c 2062 6520 7265 6d6f 7665 642e 0a0a  ll be removed...
-000117d0: 2323 2053 7065 6369 6679 696e 6720 576f  ## Specifying Wo
-000117e0: 726b 2052 6571 7569 7265 6d65 6e74 7320  rk Requirements 
-000117f0: 7573 696e 6720 4353 5620 4461 7461 0a0a  using CSV Data..
-00011800: 4353 5620 6461 7461 2066 696c 6573 2063  CSV data files c
-00011810: 616e 2062 6520 7573 6564 2074 6f20 6472  an be used to dr
-00011820: 6976 6520 7468 6520 6765 6e65 7261 7469  ive the generati
-00011830: 6f6e 206f 6620 6c69 7374 7320 6f66 2054  on of lists of T
-00011840: 6173 6b73 2c20 6173 2066 6f6c 6c6f 7773  asks, as follows
-00011850: 3a0a 0a2d 2041 202a 2a70 726f 746f 7479  :..- A **prototy
-00011860: 7065 2a2a 2054 6173 6b20 7370 6563 6966  pe** Task specif
-00011870: 6963 6174 696f 6e20 6973 2063 7265 6174  ication is creat
-00011880: 6564 2077 6974 6869 6e20 6120 4a53 4f4e  ed within a JSON
-00011890: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-000118a0: 7420 7370 6563 6966 6963 6174 696f 6e20  t specification 
-000118b0: 6f72 2069 6e20 7468 6520 6077 6f72 6b52  or in the `workR
-000118c0: 6571 7569 7265 6d65 6e74 6020 7365 6374  equirement` sect
-000118d0: 696f 6e20 6f66 2074 6865 2054 4f4d 4c20  ion of the TOML 
-000118e0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-000118f0: 6c65 0a2d 2054 6865 2070 726f 746f 7479  le.- The prototy
-00011900: 7065 2074 6173 6b20 696e 636c 7564 6573  pe task includes
-00011910: 206f 6e65 206f 7220 6d6f 7265 2076 6172   one or more var
-00011920: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00011930: 6f6e 730a 2d20 4120 4353 5620 6669 6c65  ons.- A CSV file
-00011940: 2069 7320 6372 6561 7465 642c 2077 6974   is created, wit
-00011950: 6820 7468 6520 2a2a 6865 6164 6572 732a  h the **headers*
-00011960: 2a20 2866 6972 7374 2072 6f77 2920 6d61  * (first row) ma
-00011970: 7463 6869 6e67 2074 6865 206e 616d 6573  tching the names
-00011980: 206f 6620 7468 6520 7661 7269 6162 6c65   of the variable
-00011990: 2073 7562 7374 6974 7574 696f 6e73 2069   substitutions i
-000119a0: 6e20 7468 6520 5461 736b 2070 726f 746f  n the Task proto
-000119b0: 7479 7065 0a2d 2045 6163 6820 7375 6273  type.- Each subs
-000119c0: 6571 7565 6e74 2072 6f77 206f 6620 7468  equent row of th
-000119d0: 6520 4353 5620 6669 6c65 2072 6570 7265  e CSV file repre
-000119e0: 7365 6e74 7320 6120 6e65 7720 5461 736b  sents a new Task
-000119f0: 2062 7569 6c74 2075 7369 6e67 2074 6865   built using the
-00011a00: 2070 726f 746f 7479 7065 2c20 7769 7468   prototype, with
-00011a10: 2074 6865 2076 6172 6961 626c 6573 2073   the variables s
-00011a20: 7562 7374 6974 7574 6564 2062 7920 7468  ubstituted by th
-00011a30: 6520 7661 6c75 6573 2069 6e20 7468 6520  e values in the 
-00011a40: 726f 770a 2d20 4120 5461 736b 2077 696c  row.- A Task wil
-00011a50: 6c20 6265 2063 7265 6174 6564 2066 6f72  l be created for
-00011a60: 2065 6163 6820 6461 7461 2072 6f77 0a0a   each data row..
-00011a70: 2323 2320 576f 726b 2052 6571 7569 7265  ### Work Require
-00011a80: 6d65 6e74 2043 5356 2044 6174 6120 4578  ment CSV Data Ex
-00011a90: 616d 706c 650a 0a41 7320 616e 2065 7861  ample..As an exa
-00011aa0: 6d70 6c65 2c20 636f 6e73 6964 6572 2074  mple, consider t
-00011ab0: 6865 2066 6f6c 6c6f 7769 6e67 204a 534f  he following JSO
-00011ac0: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
-00011ad0: 6e74 2060 7772 2e6a 736f 6e60 3a0a 0a60  nt `wr.json`:..`
-00011ae0: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
-00011af0: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
-00011b00: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-00011b10: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-00011b20: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
-00011b30: 223a 205b 227b 7b61 7267 5f31 7d7d 222c  ": ["{{arg_1}}",
-00011b40: 2022 7b7b 6172 675f 327d 7d22 2c20 227b   "{{arg_2}}", "{
-00011b50: 7b61 7267 5f33 7d7d 225d 2c0a 2020 2020  {arg_3}}"],.    
-00011b60: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
-00011b70: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
-00011b80: 223a 2022 7b7b 656e 765f 317d 7d22 7d0a  ": "{{env_1}}"}.
-00011b90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00011ba0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
-00011bb0: 600a 0a4e 6f74 6520 7468 6174 2074 6865  `..Note that the
-00011bc0: 2054 6173 6b20 4772 6f75 7020 6d75 7374   Task Group must
-00011bd0: 2063 6f6e 7461 696e 206f 6e6c 7920 6120   contain only a 
-00011be0: 7369 6e67 6c65 2054 6173 6b2c 2061 6374  single Task, act
-00011bf0: 696e 6720 6173 2074 6865 2070 726f 746f  ing as the proto
-00011c00: 7479 7065 2e0a 0a4e 6f77 2063 6f6e 7369  type...Now consi
-00011c10: 6465 7220 6120 4353 5620 6669 6c65 2060  der a CSV file `
-00011c20: 7772 5f64 6174 612e 6373 7660 2077 6974  wr_data.csv` wit
-00011c30: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
-00011c40: 636f 6e74 656e 7473 3a0a 0a60 6060 7465  contents:..```te
-00011c50: 7874 0a61 7267 5f31 2c20 6172 675f 322c  xt.arg_1, arg_2,
-00011c60: 2061 7267 5f33 2c20 656e 765f 310a 412c   arg_3, env_1.A,
-00011c70: 2020 2020 2042 2c20 2020 2020 432c 2020       B,     C,  
-00011c80: 2020 2045 2d31 0a44 2c20 2020 2020 452c     E-1.D,     E,
-00011c90: 2020 2020 2046 2c20 2020 2020 452d 320a       F,     E-2.
-00011ca0: 472c 2020 2020 2048 2c20 2020 2020 492c  G,     H,     I,
-00011cb0: 2020 2020 2045 2d33 0a60 6060 0a0a 4e6f       E-3.```..No
-00011cc0: 7465 2074 6861 7420 7468 6520 286f 7074  te that the (opt
-00011cd0: 696f 6e61 6c29 206c 6561 6469 6e67 2073  ional) leading s
-00011ce0: 7061 6365 7320 6166 7465 7220 6561 6368  paces after each
-00011cf0: 2063 6f6d 6d61 2061 7265 2069 676e 6f72   comma are ignor
-00011d00: 6564 2c20 6275 7420 7472 6169 6c69 6e67  ed, but trailing
-00011d10: 2073 7061 6365 7320 6172 6520 6e6f 7420   spaces are not 
-00011d20: 616e 6420 7769 6c6c 2066 6f72 6d20 7061  and will form pa
-00011d30: 7274 206f 6620 7468 6520 696d 706f 7274  rt of the import
-00011d40: 6564 2064 6174 612e 0a0a 4966 2074 6865  ed data...If the
-00011d50: 7365 2066 696c 6573 2061 7265 2070 726f  se files are pro
-00011d60: 6365 7373 6564 2075 7369 6e67 2060 7964  cessed using `yd
-00011d70: 2d73 7562 6d69 7420 2d72 2077 722e 6a73  -submit -r wr.js
-00011d80: 6f6e 202d 5620 7772 5f64 6174 612e 6373  on -V wr_data.cs
-00011d90: 7660 2c20 7468 6520 666f 6c6c 6f77 696e  v`, the followin
-00011da0: 6720 6578 7061 6e64 6564 206c 6973 7420  g expanded list 
-00011db0: 6f66 2074 6872 6565 2054 6173 6b73 2077  of three Tasks w
-00011dc0: 696c 6c20 6265 2063 7265 6174 6564 2070  ill be created p
-00011dd0: 7269 6f72 2074 6f20 6675 7274 6865 7220  rior to further 
-00011de0: 7072 6f63 6573 7369 6e67 2062 7920 7468  processing by th
-00011df0: 6520 6079 642d 7375 626d 6974 6020 7363  e `yd-submit` sc
-00011e00: 7269 7074 3a0a 0a60 6060 6a73 6f6e 0a7b  ript:..```json.{
-00011e10: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
-00011e20: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-00011e30: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
-00011e40: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
-00011e50: 7267 756d 656e 7473 223a 205b 2241 222c  rguments": ["A",
-00011e60: 2022 4222 2c20 2243 225d 2c0a 2020 2020   "B", "C"],.    
-00011e70: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
-00011e80: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
-00011e90: 223a 2022 452d 3122 7d0a 2020 2020 2020  ": "E-1"}.      
-00011ea0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00011eb0: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00011ec0: 6e74 7322 3a20 5b22 4422 2c20 2245 222c  nts": ["D", "E",
-00011ed0: 2022 4622 5d2c 0a20 2020 2020 2020 2020   "F"],.         
-00011ee0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-00011ef0: 7b22 454e 565f 5641 525f 3122 3a20 2245  {"ENV_VAR_1": "E
-00011f00: 2d32 227d 0a20 2020 2020 2020 207d 2c0a  -2"}.        },.
-00011f10: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00011f20: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
-00011f30: 205b 2247 222c 2022 4822 2c20 2249 225d   ["G", "H", "I"]
-00011f40: 2c0a 2020 2020 2020 2020 2020 2265 6e76  ,.          "env
-00011f50: 6972 6f6e 6d65 6e74 223a 207b 2245 4e56  ironment": {"ENV
-00011f60: 5f56 4152 5f31 223a 2022 452d 3322 7d0a  _VAR_1": "E-3"}.
-00011f70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00011f80: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
-00011f90: 600a 0a23 2323 2043 5356 2056 6172 6961  `..### CSV Varia
-00011fa0: 626c 6520 5375 6273 7469 7475 7469 6f6e  ble Substitution
-00011fb0: 730a 0a57 6865 6e20 7468 6520 4353 5620  s..When the CSV 
-00011fc0: 6669 6c65 2064 6174 6120 6973 2070 726f  file data is pro
-00011fd0: 6365 7373 6564 2c20 7468 6520 6f6e 6c79  cessed, the only
-00011fe0: 2073 7562 7374 6974 7574 696f 6e73 206d   substitutions m
-00011ff0: 6164 6520 6172 6520 7468 6f73 6520 7768  ade are those wh
-00012000: 6963 6820 6d61 7463 6820 7468 6520 7661  ich match the va
-00012010: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-00012020: 696f 6e73 2069 6e20 7468 6520 7072 6f74  ions in the prot
-00012030: 6f74 7970 6520 5461 736b 2e20 5468 6520  otype Task. The 
-00012040: 4353 5620 6669 6c65 2069 7320 7468 6520  CSV file is the 
-00012050: 2a2a 6f6e 6c79 2a2a 2073 6f75 7263 6520  **only** source 
-00012060: 6f66 2073 7562 7374 6974 7574 696f 6e73  of substitutions
-00012070: 2075 7365 6420 666f 7220 7468 6973 2070   used for this p
-00012080: 726f 6365 7373 696e 6720 7068 6173 653b  rocessing phase;
-00012090: 2061 6c6c 206f 7468 6572 2076 6172 6961   all other varia
-000120a0: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
-000120b0: 7320 2873 7570 706c 6965 6420 6f6e 2074  s (supplied on t
-000120c0: 6865 2063 6f6d 6d61 6e64 206c 696e 652c  he command line,
-000120d0: 2069 6e20 7468 6520 544f 4d4c 2063 6f6e   in the TOML con
-000120e0: 6669 6775 7261 7469 6f6e 2066 696c 652c  figuration file,
-000120f0: 206f 7220 6672 6f6d 2065 6e76 6972 6f6e   or from environ
-00012100: 6d65 6e74 2076 6172 6961 626c 6573 2920  ment variables) 
-00012110: 6172 6520 6967 6e6f 7265 6420 2d2d 2069  are ignored -- i
-00012120: 2e65 2e2c 2074 6865 7920 646f 206e 6f74  .e., they do not
-00012130: 206f 7665 7272 6964 6520 7468 6520 636f   override the co
-00012140: 6e74 656e 7473 206f 6620 7468 6520 4353  ntents of the CS
-00012150: 5620 6669 6c65 2e0a 0a41 6c6c 2076 6172  V file...All var
-00012160: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00012170: 6f6e 7320 756e 7265 6c61 7465 6420 746f  ons unrelated to
-00012180: 2074 6865 2043 5356 2066 696c 6520 6461   the CSV file da
-00012190: 7461 2061 7265 206c 6566 7420 756e 6368  ta are left unch
-000121a0: 616e 6765 642c 2066 6f72 2073 7562 7365  anged, for subse
-000121b0: 7175 656e 7420 7072 6f63 6573 7369 6e67  quent processing
-000121c0: 2062 7920 6079 642d 7375 626d 6974 602e   by `yd-submit`.
-000121d0: 0a0a 4966 2074 6865 2076 616c 7565 2074  ..If the value t
-000121e0: 6f20 6265 2069 6e73 6572 7465 6420 6973  o be inserted is
-000121f0: 2061 206e 756d 6265 7220 2861 6e20 696e   a number (an in
-00012200: 7465 6765 7220 6f72 2066 6c6f 6174 696e  teger or floatin
-00012210: 6720 706f 696e 7420 7661 6c75 6529 206f  g point value) o
-00012220: 7220 426f 6f6c 6561 6e2c 2074 6865 2060  r Boolean, the `
-00012230: 7b7b 6e75 6d3a 6d79 5f6e 756d 6265 725f  {{num:my_number_
-00012240: 7661 727d 7d60 2061 6e64 2060 7b7b 626f  var}}` and `{{bo
-00012250: 6f6c 3a6d 795f 626f 6f6c 6561 6e5f 7661  ol:my_boolean_va
-00012260: 727d 7d60 2066 6f72 6d73 2063 616e 2062  r}}` forms can b
-00012270: 6520 7573 6564 2069 6e20 7468 6520 4a53  e used in the JS
-00012280: 4f4e 2066 696c 652c 2061 7320 7769 7468  ON file, as with
-00012290: 2074 6865 6972 2075 7365 2069 6e20 6f74   their use in ot
-000122a0: 6865 7220 7061 7274 7320 6f66 2074 6865  her parts of the
-000122b0: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
-000122c0: 7265 6d65 6e74 2073 7065 6369 6669 6361  rement specifica
-000122d0: 7469 6f6e 2e20 5468 6520 7375 6273 7469  tion. The substi
-000122e0: 7475 7465 6420 7661 6c75 6520 7769 6c6c  tuted value will
-000122f0: 2061 7373 756d 6520 7468 6520 6e6f 6d69   assume the nomi
-00012300: 6e61 7465 6420 7479 7065 2072 6174 6865  nated type rathe
-00012310: 7220 7468 616e 2062 6569 6e67 2061 2073  r than being a s
-00012320: 7472 696e 672e 0a0a 2323 2320 5072 6f70  tring...### Prop
-00012330: 6572 7479 2049 6e68 6572 6974 616e 6365  erty Inheritance
-00012340: 0a0a 416c 6c20 7468 6520 7573 7561 6c20  ..All the usual 
-00012350: 7072 6f70 6572 7479 2069 6e68 6572 6974  property inherit
-00012360: 616e 6365 2066 6561 7475 7265 7320 6f70  ance features op
-00012370: 6572 6174 6520 6173 206e 6f72 6d61 6c2e  erate as normal.
-00012380: 2050 726f 7065 7274 6965 7320 6172 6520   Properties are 
-00012390: 696e 6865 7269 7465 6420 6672 6f6d 2074  inherited from t
-000123a0: 6865 2060 636f 6e66 6967 2e74 6f6d 6c60  he `config.toml`
-000123b0: 2066 696c 652c 2061 6e64 2066 726f 6d20   file, and from 
-000123c0: 7468 6520 7265 6c65 7661 6e74 2073 6563  the relevant sec
-000123d0: 7469 6f6e 7320 6f66 2074 6865 204a 534f  tions of the JSO
-000123e0: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
-000123f0: 6e74 2066 696c 652e 2041 6e79 2070 726f  nt file. Any pro
-00012400: 7065 7274 6965 7320 7365 7420 7769 7468  perties set with
-00012410: 696e 2061 2054 6173 6b20 7072 6f74 6f74  in a Task protot
-00012420: 7970 6520 6172 6520 636f 7069 6564 2074  ype are copied t
-00012430: 6f20 616c 6c20 7468 6520 6765 6e65 7261  o all the genera
-00012440: 7465 6420 5461 736b 732e 0a0a 2323 2320  ted Tasks...### 
-00012450: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
-00012460: 6f75 7073 2075 7369 6e67 204d 756c 7469  oups using Multi
-00012470: 706c 6520 4353 5620 4669 6c65 730a 0a54  ple CSV Files..T
-00012480: 6865 2075 7365 206f 6620 6d75 6c74 6970  he use of multip
-00012490: 6c65 2054 6173 6b20 4772 6f75 7073 2069  le Task Groups i
-000124a0: 7320 616c 736f 2073 7570 706f 7274 6564  s also supported
-000124b0: 2c20 6279 2075 7369 6e67 206f 6e65 2043  , by using one C
-000124c0: 5356 2066 696c 6520 7065 7220 5461 736b  SV file per Task
-000124d0: 2047 726f 7570 2e20 4561 6368 2054 6173   Group. Each Tas
-000124e0: 6b20 4772 6f75 7020 6d75 7374 2063 6f6e  k Group must con
-000124f0: 7461 696e 206f 6e6c 7920 6120 7369 6e67  tain only a sing
-00012500: 6c65 2070 726f 746f 7479 7065 2054 6173  le prototype Tas
-00012510: 6b2e 0a0a 5468 6520 4353 5620 6669 6c65  k...The CSV file
-00012520: 7320 6172 6520 7375 7070 6c69 6564 206f  s are supplied o
-00012530: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
-00012540: 6e65 2069 6e20 7468 6520 6f72 6465 7220  ne in the order 
-00012550: 6f66 2074 6865 2054 6173 6b20 4772 6f75  of the Task Grou
-00012560: 7073 2074 6f20 7768 6963 6820 7468 6579  ps to which they
-00012570: 2061 7070 6c79 2e20 466f 7220 6578 616d   apply. For exam
-00012580: 706c 652c 2069 6620 6077 725f 6a73 6f6e  ple, if `wr_json
-00012590: 6020 636f 6e74 6169 6e73 2074 776f 2054  ` contains two T
-000125a0: 6173 6b20 4772 6f75 7073 2c20 6173 2066  ask Groups, as f
-000125b0: 6f6c 6c6f 7773 3a0a 0a60 6060 6a73 6f6e  ollows:..```json
-000125c0: 0a7b 0a20 2022 7461 736b 4772 6f75 7073  .{.  "taskGroups
-000125d0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
-000125e0: 2022 7461 736b 7322 3a20 5b0a 2020 2020   "tasks": [.    
-000125f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00012600: 2261 7267 756d 656e 7473 223a 205b 227b  "arguments": ["{
-00012610: 7b61 7267 5f31 7d7d 222c 2022 7b7b 6172  {arg_1}}", "{{ar
-00012620: 675f 327d 7d22 2c20 227b 7b61 7267 5f33  g_2}}", "{{arg_3
-00012630: 7d7d 225d 2c0a 2020 2020 2020 2020 2020  }}"],.          
-00012640: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-00012650: 2245 4e56 5f56 4152 5f31 223a 2022 7b7b  "ENV_VAR_1": "{{
-00012660: 656e 765f 317d 7d22 7d0a 2020 2020 2020  env_1}}"}.      
-00012670: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
-00012680: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
-00012690: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
-000126a0: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
-000126b0: 7267 756d 656e 7473 223a 205b 227b 7b61  rguments": ["{{a
-000126c0: 7267 5f31 7d7d 222c 2022 7b7b 6172 675f  rg_1}}", "{{arg_
-000126d0: 327d 7d22 5d2c 0a20 2020 2020 2020 2020  2}}"],.         
-000126e0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-000126f0: 7b22 454e 565f 5641 525f 3122 3a20 227b  {"ENV_VAR_1": "{
-00012700: 7b65 6e76 5f31 7d7d 222c 2022 454e 565f  {env_1}}", "ENV_
-00012710: 5641 525f 3222 3a20 227b 7b65 6e76 5f32  VAR_2": "{{env_2
-00012720: 7d7d 227d 0a20 2020 2020 2020 207d 0a20  }}"}.        }. 
-00012730: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
-00012740: 0a7d 0a60 6060 0a0a 5468 6520 6079 642d  .}.```..The `yd-
-00012750: 7375 626d 6974 6020 636f 6d6d 616e 6420  submit` command 
-00012760: 776f 756c 6420 7468 656e 2062 6520 696e  would then be in
-00012770: 766f 6b65 6420 7769 7468 2061 2073 6570  voked with a sep
-00012780: 6172 6174 6520 4353 5620 6669 6c65 2066  arate CSV file f
-00012790: 6f72 2065 6163 6820 5461 736b 2047 726f  or each Task Gro
-000127a0: 7570 2c20 652e 672e 3a0a 0a60 6060 7368  up, e.g.:..```sh
-000127b0: 656c 6c0a 7964 2d73 7562 6d69 7420 2d72  ell.yd-submit -r
-000127c0: 2077 722e 6a73 6f6e 202d 5620 7772 5f64   wr.json -V wr_d
-000127d0: 6174 615f 7461 736b 5f67 726f 7570 5f31  ata_task_group_1
-000127e0: 2e63 7376 202d 5620 7772 5f64 6174 615f  .csv -V wr_data_
-000127f0: 7461 736b 5f67 726f 7570 5f32 2e63 7376  task_group_2.csv
-00012800: 0a60 6060 0a0a 4966 2074 6865 7265 2061  .```..If there a
-00012810: 7265 202a 2a66 6577 6572 2a2a 2043 5356  re **fewer** CSV
-00012820: 2066 696c 6573 2074 6861 6e20 5461 736b   files than Task
-00012830: 2047 726f 7570 7320 6120 7761 726e 696e   Groups a warnin
-00012840: 6720 7769 6c6c 2062 6520 7072 696e 7465  g will be printe
-00012850: 6420 616e 642c 2069 6620 7468 6572 6520  d and, if there 
-00012860: 6172 6520 276e 2720 4353 5620 6669 6c65  are 'n' CSV file
-00012870: 732c 2043 5356 2064 6174 6120 7072 6f63  s, CSV data proc
-00012880: 6573 7369 6e67 2077 696c 6c20 6265 2061  essing will be a
-00012890: 7070 6c69 6564 2074 6f20 7468 6520 6669  pplied to the fi
-000128a0: 7273 7420 276e 2720 5461 736b 2047 726f  rst 'n' Task Gro
-000128b0: 7570 7320 696e 2074 6865 2057 6f72 6b20  ups in the Work 
-000128c0: 5265 7175 6972 656d 656e 7420 6279 2064  Requirement by d
-000128d0: 6566 6175 6c74 2c20 696e 2074 6865 206f  efault, in the o
-000128e0: 7264 6572 2069 6e20 7768 6963 6820 7468  rder in which th
-000128f0: 6520 4353 5620 6669 6c65 7320 7765 7265  e CSV files were
-00012900: 2073 7570 706c 6965 642e 2049 6620 7468   supplied. If th
-00012910: 6572 6520 6172 6520 2a2a 6d6f 7265 2a2a  ere are **more**
-00012920: 2043 5356 2066 696c 6573 2074 6861 6e20   CSV files than 
-00012930: 5461 736b 2047 726f 7570 732c 2061 6e20  Task Groups, an 
-00012940: 6572 726f 7220 7769 6c6c 2062 6520 7261  error will be ra
-00012950: 6973 6564 2061 6e64 2070 726f 6365 7373  ised and process
-00012960: 696e 6720 7769 6c6c 2073 746f 702e 0a0a  ing will stop...
-00012970: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-00012980: 6f20 6170 706c 7920 4353 5620 6669 6c65  o apply CSV file
-00012990: 7320 6578 706c 6963 6974 6c79 2074 6f20  s explicitly to 
-000129a0: 7370 6563 6966 6963 2054 6173 6b20 4772  specific Task Gr
-000129b0: 6f75 7073 2c20 6279 2075 7369 6e67 2061  oups, by using a
-000129c0: 6e20 6f70 7469 6f6e 616c 202a 2a69 6e64  n optional **ind
-000129d0: 6578 2070 6f73 7466 6978 2a2a 2028 652e  ex postfix** (e.
-000129e0: 672e 2c20 603a 3260 2920 6174 2074 6865  g., `:2`) at the
-000129f0: 2065 6e64 206f 6620 6561 6368 2043 5356   end of each CSV
-00012a00: 2066 696c 656e 616d 652e 2046 6f72 2065   filename. For e
-00012a10: 7861 6d70 6c65 2c20 6966 2074 6865 7265  xample, if there
-00012a20: 2061 7265 2074 776f 2043 5356 2066 696c   are two CSV fil
-00012a30: 6573 2074 6f20 6265 2061 7070 6c69 6564  es to be applied
-00012a40: 2074 6f20 7468 6520 7365 636f 6e64 2061   to the second a
-00012a50: 6e64 2066 6f75 7274 6820 5461 736b 2047  nd fourth Task G
-00012a60: 726f 7570 7320 696e 2061 204a 534f 4e20  roups in a JSON 
-00012a70: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00012a80: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
-00012a90: 696e 6720 7379 6e74 6178 3a0a 0a60 6060  ing syntax:..```
-00012aa0: 7368 656c 6c0a 7964 2d73 7562 6d69 7420  shell.yd-submit 
-00012ab0: 2d72 2077 722e 6a73 6f6e 202d 5620 7772  -r wr.json -V wr
-00012ac0: 5f64 6174 615f 7461 736b 5f67 726f 7570  _data_task_group
-00012ad0: 5f32 2e63 7376 3a32 202d 5620 7772 5f64  _2.csv:2 -V wr_d
-00012ae0: 6174 615f 7461 736b 5f67 726f 7570 5f34  ata_task_group_4
-00012af0: 2e63 7376 3a34 0a60 6060 0a0a 416c 7465  .csv:4.```..Alte
-00012b00: 726e 6174 6976 656c 792c 2074 6865 202a  rnatively, the *
-00012b10: 2a54 6173 6b20 4772 6f75 7020 6e61 6d65  *Task Group name
-00012b20: 2a2a 2028 6966 2073 7570 706c 6965 6420  ** (if supplied 
-00012b30: 696e 2074 6865 204a 534f 4e20 6669 6c65  in the JSON file
-00012b40: 2920 6361 6e20 6265 2075 7365 6420 6173  ) can be used as
-00012b50: 2074 6865 2070 6f73 7466 6978 2e20 466f   the postfix. Fo
-00012b60: 7220 6578 616d 706c 652c 2069 6620 7468  r example, if th
-00012b70: 6520 5461 736b 2047 726f 7570 7320 6162  e Task Groups ab
-00012b80: 6f76 6520 6172 6520 6e61 6d65 6420 6074  ove are named `t
-00012b90: 675f 7477 6f60 2061 6e64 2060 7467 5f66  g_two` and `tg_f
-00012ba0: 6f75 7260 2c20 7468 6520 6079 642d 7375  our`, the `yd-su
-00012bb0: 626d 6974 6020 636f 6d6d 616e 6420 776f  bmit` command wo
-00012bc0: 756c 6420 6265 636f 6d65 3a0a 0a60 6060  uld become:..```
-00012bd0: 7368 656c 6c0a 7964 2d73 7562 6d69 7420  shell.yd-submit 
-00012be0: 2d72 2077 722e 6a73 6f6e 202d 5620 7772  -r wr.json -V wr
-00012bf0: 5f64 6174 615f 7461 736b 5f67 726f 7570  _data_task_group
-00012c00: 5f32 2e63 7376 3a74 675f 7477 6f20 2d56  _2.csv:tg_two -V
-00012c10: 2077 725f 6461 7461 5f74 6173 6b5f 6772   wr_data_task_gr
-00012c20: 6f75 705f 342e 6373 763a 7467 5f66 6f75  oup_4.csv:tg_fou
-00012c30: 720a 6060 600a 0a4e 6f74 6520 7468 6174  r.```..Note that
-00012c40: 206f 6e6c 7920 6f6e 6520 4353 5620 6669   only one CSV fi
-00012c50: 6c65 2063 616e 2062 6520 6170 706c 6965  le can be applie
-00012c60: 6420 746f 2061 6e79 2067 6976 656e 2054  d to any given T
-00012c70: 6173 6b20 4772 6f75 702e 2041 2073 696e  ask Group. A sin
-00012c80: 676c 6520 4353 5620 6669 6c65 2063 616e  gle CSV file can
-00012c90: 2c20 686f 7765 7665 722c 2062 6520 7265  , however, be re
-00012ca0: 7573 6564 2066 6f72 206d 756c 7469 706c  used for multipl
-00012cb0: 6520 5461 736b 2047 726f 7570 732e 0a0a  e Task Groups...
-00012cc0: 2323 2320 5573 696e 6720 4353 5620 4461  ### Using CSV Da
-00012cd0: 7461 2077 6974 6820 5369 6d70 6c65 2c20  ta with Simple, 
-00012ce0: 544f 4d4c 2d4f 6e6c 7920 576f 726b 2052  TOML-Only Work R
-00012cf0: 6571 7569 7265 6d65 6e74 2053 7065 6369  equirement Speci
-00012d00: 6669 6361 7469 6f6e 730a 0a49 7427 7320  fications..It's 
-00012d10: 706f 7373 6962 6c65 2074 6f20 7573 6520  possible to use 
-00012d20: 544f 4d4c 2065 7863 6c75 7369 7665 6c79  TOML exclusively
-00012d30: 2074 6f20 6465 7269 7665 2061 206c 6973   to derive a lis
-00012d40: 7420 6f66 2054 6173 6b73 2066 726f 6d20  t of Tasks from 
-00012d50: 4353 5620 6461 7461 202d 2d20 692e 652e  CSV data -- i.e.
-00012d60: 2c20 6120 4a53 4f4e 2057 6f72 6b20 5265  , a JSON Work Re
-00012d70: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
-00012d80: 6963 6174 696f 6e20 6973 206e 6f74 2072  ication is not r
-00012d90: 6571 7569 7265 642e 0a0a 546f 206d 616b  equired...To mak
-00012da0: 6520 7573 6520 6f66 2074 6869 733a 0a0a  e use of this:..
-00012db0: 312e 2045 6e73 7572 6520 7468 6174 206e  1. Ensure that n
-00012dc0: 6f20 4a53 4f4e 2057 6f72 6b20 5265 7175  o JSON Work Requ
-00012dd0: 6972 656d 656e 7420 646f 6375 6d65 6e74  irement document
-00012de0: 2069 7320 7370 6563 6966 6965 6420 286e   is specified (n
-00012df0: 6f20 6077 6f72 6b52 6571 7569 7265 6d65  o `workRequireme
-00012e00: 6e74 4461 7461 6020 696e 2074 6865 2054  ntData` in the T
-00012e10: 4f4d 4c20 6669 6c65 2c20 6f72 2060 2d2d  OML file, or `--
-00012e20: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
-00012e30: 6020 6f6e 2074 6865 2063 6f6d 6d61 6e64  ` on the command
-00012e40: 206c 696e 6529 0a32 2e20 496e 7365 7274   line).2. Insert
-00012e50: 2074 6865 2072 6571 7569 7265 6420 4353   the required CS
-00012e60: 562d 7375 7070 6c69 6564 2076 6172 6961  V-supplied varia
-00012e70: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
-00012e80: 7320 6469 7265 6374 6c79 2069 6e74 6f20  s directly into 
-00012e90: 7468 6520 544f 4d4c 2070 726f 7065 7274  the TOML propert
-00012ea0: 6965 732c 2065 2e67 2e20 6061 7267 756d  ies, e.g. `argum
-00012eb0: 656e 7473 203d 205b 227b 7b61 7267 5f31  ents = ["{{arg_1
-00012ec0: 7d7d 222c 2022 7b7b 6172 675f 327d 7d22  }}", "{{arg_2}}"
-00012ed0: 5d60 0a33 2e20 5370 6563 6966 7920 6120  ]`.3. Specify a 
-00012ee0: 7369 6e67 6c65 2043 5356 2066 696c 6520  single CSV file 
-00012ef0: 696e 2074 6865 2060 6373 7646 696c 6573  in the `csvFiles
-00012f00: 6020 544f 4d4c 2070 726f 7065 7274 792c  ` TOML property,
-00012f10: 2065 2e67 2e20 6063 7376 4669 6c65 7320   e.g. `csvFiles 
-00012f20: 3d20 5b22 7772 5f64 6174 612e 6373 7622  = ["wr_data.csv"
-00012f30: 5d60 2c20 6f72 2070 726f 7669 6465 2074  ]`, or provide t
-00012f40: 6865 2043 5356 2066 696c 6520 6f6e 2074  he CSV file on t
-00012f50: 6865 2063 6f6d 6d61 6e64 206c 696e 6520  he command line 
-00012f60: 602d 5620 7772 5f64 6174 612e 6373 7660  `-V wr_data.csv`
-00012f70: 0a0a 5768 656e 2060 7964 2d73 7562 6d69  ..When `yd-submi
-00012f80: 7460 2069 7320 7275 6e2c 2069 7420 7769  t` is run, it wi
-00012f90: 6c6c 2065 7870 616e 6420 7468 6520 5461  ll expand the Ta
-00012fa0: 736b 206c 6973 7420 746f 206d 6174 6368  sk list to match
-00012fb0: 2074 6865 206e 756d 6265 7220 6f66 2064   the number of d
-00012fc0: 6174 6120 726f 7773 2069 6e20 7468 6520  ata rows in the 
-00012fd0: 4353 5620 6669 6c65 2e0a 0a23 2323 2049  CSV file...### I
-00012fe0: 6e73 7065 6374 696e 6720 7468 6520 5265  nspecting the Re
-00012ff0: 7375 6c74 7320 6f66 2043 5356 2056 6172  sults of CSV Var
-00013000: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
-00013010: 6f6e 0a0a 5468 6520 602d 2d70 726f 6365  on..The `--proce
-00013020: 7373 2d63 7376 2d6f 6e6c 7960 2028 6f72  ss-csv-only` (or
-00013030: 2060 2d70 6029 206f 7074 696f 6e20 6361   `-p`) option ca
-00013040: 6e20 6265 2075 7365 6420 7769 7468 2060  n be used with `
-00013050: 7964 2d73 7562 6d69 7460 2074 6f20 6f75  yd-submit` to ou
-00013060: 7470 7574 2074 6865 204a 534f 4e20 576f  tput the JSON Wo
-00013070: 726b 2052 6571 7569 7265 6d65 6e74 2061  rk Requirement a
-00013080: 6674 6572 2043 5356 2076 6172 6961 626c  fter CSV variabl
-00013090: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
-000130a0: 6f6e 6c79 2c20 7072 696f 7220 746f 2061  only, prior to a
-000130b0: 6c6c 206f 7468 6572 2073 7562 7374 6974  ll other substit
-000130c0: 7574 696f 6e73 2061 6e64 2070 726f 7065  utions and prope
-000130d0: 7274 7920 696e 6865 7269 7461 6e63 6520  rty inheritance 
-000130e0: 6170 706c 6965 6420 6279 2060 7964 2d73  applied by `yd-s
-000130f0: 7562 6d69 7460 2e0a 0a23 2057 6f72 6b65  ubmit`...# Worke
-00013100: 7220 506f 6f6c 2050 726f 7065 7274 6965  r Pool Propertie
-00013110: 730a 0a54 6865 2060 776f 726b 6572 506f  s..The `workerPo
-00013120: 6f6c 6020 7365 6374 696f 6e20 6f66 2074  ol` section of t
-00013130: 6865 2054 4f4d 4c20 6669 6c65 2064 6566  he TOML file def
-00013140: 696e 6573 2074 6865 2070 726f 7065 7274  ines the propert
-00013150: 6965 7320 6f66 2074 6865 2057 6f72 6b65  ies of the Worke
-00013160: 7220 506f 6f6c 2074 6f20 6265 2063 7265  r Pool to be cre
-00013170: 6174 6564 2c20 616e 6420 6973 2075 7365  ated, and is use
-00013180: 6420 6279 2074 6865 2060 7964 2d70 726f  d by the `yd-pro
-00013190: 7669 7369 6f6e 6020 636f 6d6d 616e 642e  vision` command.
-000131a0: 2041 2073 7562 7365 7420 6f66 2074 6865   A subset of the
-000131b0: 2070 726f 7065 7274 6965 7320 6973 2061   properties is a
-000131c0: 6c73 6f20 7573 6564 2062 7920 7468 6520  lso used by the 
-000131d0: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
-000131e0: 2063 6f6d 6d61 6e64 2c20 666f 7220 6372   command, for cr
-000131f0: 6561 7469 6e67 2073 7461 6e64 616c 6f6e  eating standalon
-00013200: 6520 436f 6d70 7574 6520 5265 7175 6972  e Compute Requir
-00013210: 656d 656e 7473 2074 6861 7420 6172 6520  ements that are 
-00013220: 6e6f 7420 6173 736f 6369 6174 6564 2077  not associated w
-00013230: 6974 6820 576f 726b 6572 2050 6f6f 6c73  ith Worker Pools
-00013240: 2e0a 0a54 6865 206f 6e6c 7920 6d61 6e64  ...The only mand
-00013250: 6174 6f72 7920 7072 6f70 6572 7479 2069  atory property i
-00013260: 7320 6074 656d 706c 6174 6549 6460 2e20  s `templateId`. 
-00013270: 416c 6c20 6f74 6865 7220 7072 6f70 6572  All other proper
-00013280: 7469 6573 2068 6176 6520 6465 6661 756c  ties have defaul
-00013290: 7473 2028 6f72 2061 7265 206e 6f74 2072  ts (or are not r
-000132a0: 6571 7569 7265 6429 2e0a 0a54 6865 2066  equired)...The f
-000132b0: 6f6c 6c6f 7769 6e67 2070 726f 7065 7274  ollowing propert
-000132c0: 6965 7320 6172 6520 6176 6169 6c61 626c  ies are availabl
-000132d0: 653a 0a0a 7c20 5072 6f70 6572 7479 2020  e:..| Property  
-000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132f0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+0000bde0: 7c20 5965 7320 207c 2059 6573 2020 2020  | Yes  | Yes    
+0000bdf0: 2020 2020 7c0a 7c20 607b 7b74 6173 6b5f      |.| `{{task_
+0000be00: 6772 6f75 705f 636f 756e 747d 7d60 2020  group_count}}`  
+0000be10: 7c20 5468 6520 6e75 6d62 6572 206f 6620  | The number of 
+0000be20: 5461 736b 2047 726f 7570 7320 696e 2074  Task Groups in t
+0000be30: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+0000be40: 656e 7420 7c20 5965 7320 207c 2059 6573  ent | Yes  | Yes
+0000be50: 2020 2020 2020 2020 7c0a 0a49 6e20 6164          |..In ad
+0000be60: 6469 7469 6f6e 2c20 2a2a 5461 736b 732a  dition, **Tasks*
+0000be70: 2a20 6465 6669 6e65 6420 696e 204a 534f  * defined in JSO
+0000be80: 4e20 646f 6375 6d65 6e74 7320 6361 6e20  N documents can 
+0000be90: 7573 6520 616e 7920 6f66 2074 6865 2073  use any of the s
+0000bea0: 7562 7374 6974 7574 696f 6e73 2061 626f  ubstitutions abo
+0000beb0: 7665 2069 6e20 616e 7920 6f66 2074 6865  ve in any of the
+0000bec0: 6972 2070 726f 7065 7274 6965 732c 206e  ir properties, n
+0000bed0: 6f74 206a 7573 7420 606e 616d 6560 2e0a  ot just `name`..
+0000bee0: 0a4e 756d 6265 7273 2061 7265 207a 6572  .Numbers are zer
+0000bef0: 6f2d 7061 6464 6564 2066 6f72 206e 6561  o-padded for nea
+0000bf00: 7420 666f 726d 6174 7469 6e67 2061 6e64  t formatting and
+0000bf10: 2073 6f72 7469 6e67 2c20 652e 672e 2c20   sorting, e.g., 
+0000bf20: 5461 736b 206e 756d 6265 7220 6033 3760  Task number `37`
+0000bf30: 206f 6620 6031 3030 3060 2054 6173 6b73   of `1000` Tasks
+0000bf40: 2077 6f75 6c64 2062 6520 7375 6273 7469   would be substi
+0000bf50: 7475 7465 6420 6173 2060 3030 3337 602e  tuted as `0037`.
+0000bf60: 0a0a 4173 2061 6e20 6578 616d 706c 652c  ..As an example,
+0000bf70: 2074 6865 2066 6f6c 6c6f 7769 6e67 204a   the following J
+0000bf80: 534f 4e20 576f 726b 2052 6571 7569 7265  SON Work Require
+0000bf90: 6d65 6e74 3a0a 0a60 6060 6a73 6f6e 0a7b  ment:..```json.{
+0000bfa0: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+0000bfb0: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+0000bfc0: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
+0000bfd0: 6772 6f75 705f 7b7b 7461 736b 5f67 726f  group_{{task_gro
+0000bfe0: 7570 5f6e 756d 6265 727d 7d5f 6131 222c  up_number}}_a1",
+0000bff0: 0a20 2020 2020 2022 6578 6563 7574 6162  .      "executab
+0000c000: 6c65 223a 2022 6578 312e 7368 222c 0a20  le": "ex1.sh",. 
+0000c010: 2020 2020 2022 7461 736b 436f 756e 7422       "taskCount"
+0000c020: 3a20 322c 0a20 2020 2020 2022 7461 736b  : 2,.      "task
+0000c030: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
+0000c040: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+0000c050: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
+0000c060: 6b5f 6e75 6d62 6572 7d7d 2d6f 662d 7b7b  k_number}}-of-{{
+0000c070: 7461 736b 5f63 6f75 6e74 7d7d 222c 0a20  task_count}}",. 
+0000c080: 2020 2020 2020 2020 2022 656e 7669 726f           "enviro
+0000c090: 6e6d 656e 7422 3a20 7b22 5441 534b 5f4e  nment": {"TASK_N
+0000c0a0: 554d 4245 5222 3a20 227b 7b74 6173 6b5f  UMBER": "{{task_
+0000c0b0: 6e75 6d62 6572 7d7d 227d 0a20 2020 2020  number}}"}.     
+0000c0c0: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+0000c0d0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+0000c0e0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
+0000c0f0: 5f67 726f 7570 5f7b 7b74 6173 6b5f 6772  _group_{{task_gr
+0000c100: 6f75 705f 6e75 6d62 6572 7d7d 5f62 3122  oup_number}}_b1"
+0000c110: 2c0a 2020 2020 2020 2265 7865 6375 7461  ,.      "executa
+0000c120: 626c 6522 3a20 2265 7832 2e73 6822 2c0a  ble": "ex2.sh",.
+0000c130: 2020 2020 2020 2274 6173 6b43 6f75 6e74        "taskCount
+0000c140: 223a 2032 2c0a 2020 2020 2020 2274 6173  ": 2,.      "tas
+0000c150: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
+0000c160: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
+0000c170: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
+0000c180: 736b 5f6e 756d 6265 727d 7d2d 6f66 2d7b  sk_number}}-of-{
+0000c190: 7b74 6173 6b5f 636f 756e 747d 7d22 0a20  {task_count}}". 
+0000c1a0: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+0000c1b0: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
+0000c1c0: 0a0a 2e2e 2e20 776f 756c 6420 6372 6561  ..... would crea
+0000c1d0: 7465 2054 6173 6b20 4772 6f75 7073 206e  te Task Groups n
+0000c1e0: 616d 6564 2060 6d79 5f74 6173 6b5f 6772  amed `my_task_gr
+0000c1f0: 6f75 705f 315f 6131 6020 616e 6420 606d  oup_1_a1` and `m
+0000c200: 795f 7461 736b 5f67 726f 7570 5f32 5f62  y_task_group_2_b
+0000c210: 3160 2c20 6561 6368 2063 6f6e 7461 696e  1`, each contain
+0000c220: 696e 6720 5461 736b 7320 6e61 6d65 6420  ing Tasks named 
+0000c230: 606d 795f 7461 736b 5f31 2d6f 662d 3260  `my_task_1-of-2`
+0000c240: 2c20 606d 795f 7461 736b 5f32 2d6f 662d  , `my_task_2-of-
+0000c250: 3260 2e0a 0a23 2323 2057 6f72 6b20 5265  2`...### Work Re
+0000c260: 7175 6972 656d 656e 7420 4e61 6d65 2053  quirement Name S
+0000c270: 7562 7374 6974 7574 696f 6e0a 0a54 6865  ubstitution..The
+0000c280: 206e 616d 6520 6f66 2074 6865 2057 6f72   name of the Wor
+0000c290: 6b20 5265 7175 6972 656d 656e 7420 6974  k Requirement it
+0000c2a0: 7365 6c66 2063 616e 2062 6520 7573 6564  self can be used
+0000c2b0: 2076 6961 2074 6865 2076 6172 6961 626c   via the variabl
+0000c2c0: 6520 7375 6273 7469 7475 7469 6f6e 2060  e substitution `
+0000c2d0: 7b7b 7772 5f6e 616d 657d 7d60 2e20 5468  {{wr_name}}`. Th
+0000c2e0: 6973 2063 616e 2062 6520 7573 6564 2061  is can be used a
+0000c2f0: 6e79 7768 6572 6520 696e 2061 2054 4f4d  nywhere in a TOM
+0000c300: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
+0000c310: 6669 6c65 206f 7220 696e 2061 204a 534f  file or in a JSO
+0000c320: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
+0000c330: 6e74 2e0a 0a23 2320 4472 792d 5275 6e6e  nt...## Dry-Runn
+0000c340: 696e 6720 576f 726b 2052 6571 7569 7265  ing Work Require
+0000c350: 6d65 6e74 2053 7562 6d69 7373 696f 6e73  ment Submissions
+0000c360: 0a0a 546f 2065 7861 6d69 6e65 2074 6865  ..To examine the
+0000c370: 204a 534f 4e20 7468 6174 2077 696c 6c20   JSON that will 
+0000c380: 6163 7475 616c 6c79 2062 6520 7365 6e74  actually be sent
+0000c390: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
+0000c3a0: 6720 4150 4920 6166 7465 7220 616c 6c20  g API after all 
+0000c3b0: 7072 6f63 6573 7369 6e67 2c20 7573 6520  processing, use 
+0000c3c0: 7468 6520 602d 2d64 7279 2d72 756e 6020  the `--dry-run` 
+0000c3d0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
+0000c3e0: 696f 6e20 7768 656e 2072 756e 6e69 6e67  ion when running
+0000c3f0: 2060 7964 2d73 7562 6d69 7460 2e20 5468   `yd-submit`. Th
+0000c400: 6973 2077 696c 6c20 7072 696e 7420 7468  is will print th
+0000c410: 6520 6675 6c6c 7920 7072 6f63 6573 7365  e fully processe
+0000c420: 6420 4a53 4f4e 2066 6f72 2074 6865 2057  d JSON for the W
+0000c430: 6f72 6b20 5265 7175 6972 656d 656e 742e  ork Requirement.
+0000c440: 204e 6f74 6869 6e67 2077 696c 6c20 6265   Nothing will be
+0000c450: 2073 7562 6d69 7474 6564 2074 6f20 7468   submitted to th
+0000c460: 6520 506c 6174 666f 726d 2e0a 0a54 6865  e Platform...The
+0000c470: 2064 7279 2d72 756e 2069 7320 7573 6566   dry-run is usef
+0000c480: 756c 2066 6f72 2069 6e73 7065 6374 696e  ul for inspectin
+0000c490: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
+0000c4a0: 2061 6c6c 2074 6865 2070 726f 6365 7373   all the process
+0000c4b0: 696e 6720 7468 6174 2773 2062 6565 6e20  ing that's been 
+0000c4c0: 7065 7266 6f72 6d65 642e 2054 6f20 7375  performed. To su
+0000c4d0: 7070 7265 7373 2061 6c6c 206f 7574 7075  ppress all outpu
+0000c4e0: 7420 6578 6365 7074 2066 6f72 2074 6865  t except for the
+0000c4f0: 204a 534f 4e20 6974 7365 6c66 2c20 7573   JSON itself, us
+0000c500: 6520 7468 6520 602d 2d71 7569 6574 6020  e the `--quiet` 
+0000c510: 2860 2d71 6029 2063 6f6d 6d61 6e64 206c  (`-q`) command l
+0000c520: 696e 6520 6f70 7469 6f6e 2e0a 0a4e 6f74  ine option...Not
+0000c530: 6520 7468 6174 2074 6865 2067 656e 6572  e that the gener
+0000c540: 6174 6564 204a 534f 4e20 6973 2061 2063  ated JSON is a c
+0000c550: 6f6e 736f 6c69 6461 7465 6420 666f 726d  onsolidated form
+0000c560: 206f 6620 7768 6174 2077 6f75 6c64 2062   of what would b
+0000c570: 6520 7375 626d 6974 7465 6420 746f 2074  e submitted to t
+0000c580: 6865 2059 656c 6c6f 7744 6f67 2041 5049  he YellowDog API
+0000c590: 2c20 616e 6420 5461 736b 7320 6172 6520  , and Tasks are 
+0000c5a0: 6465 6669 6e65 6420 6469 7265 6374 6c79  defined directly
+0000c5b0: 2077 6974 6869 6e20 7468 6569 7220 5461   within their Ta
+0000c5c0: 736b 2047 726f 7570 7320 666f 7220 6561  sk Groups for ea
+0000c5d0: 7365 206f 6620 636f 6d70 7265 6865 6e73  se of comprehens
+0000c5e0: 696f 6e2e 2049 6e20 6163 7475 616c 2041  ion. In actual A
+0000c5f0: 5049 2073 7562 6d69 7373 696f 6e73 2c20  PI submissions, 
+0000c600: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+0000c610: 6d65 6e74 2077 6974 6820 6974 7320 5461  ment with its Ta
+0000c620: 736b 2047 726f 7570 7320 6973 2073 7562  sk Groups is sub
+0000c630: 6d69 7474 6564 2066 6972 7374 2c20 616e  mitted first, an
+0000c640: 6420 5461 736b 7320 6172 6520 7468 656e  d Tasks are then
+0000c650: 2061 6464 6564 2074 6f20 5461 736b 2047   added to Task G
+0000c660: 726f 7570 7320 7365 7061 7261 7465 6c79  roups separately
+0000c670: 2069 6e20 7375 6273 6571 7565 6e74 2041   in subsequent A
+0000c680: 5049 2063 616c 6c73 2e0a 0a41 2073 696d  PI calls...A sim
+0000c690: 706c 6520 6578 616d 706c 6520 6f66 2074  ple example of t
+0000c6a0: 6865 204a 534f 4e20 6f75 7470 7574 2069  he JSON output i
+0000c6b0: 7320 7368 6f77 6e20 6265 6c6f 772c 2073  s shown below, s
+0000c6c0: 686f 7769 6e67 2061 2057 6f72 6b20 5265  howing a Work Re
+0000c6d0: 7175 6972 656d 656e 7420 7769 7468 2061  quirement with a
+0000c6e0: 2073 696e 676c 6520 5461 736b 2047 726f   single Task Gro
+0000c6f0: 7570 2c20 636f 6e74 6169 6e69 6e67 2061  up, containing a
+0000c700: 2073 696e 676c 6520 5461 736b 2e0a 0a60   single Task...`
+0000c710: 2520 7964 2d73 7562 6d69 7420 2d2d 6472  % yd-submit --dr
+0000c720: 792d 7275 6e20 2d2d 7175 6965 7460 0a60  y-run --quiet`.`
+0000c730: 6060 6a73 6f6e 0a7b 0a20 2022 6675 6c66  ``json.{.  "fulf
+0000c740: 696c 4f6e 5375 626d 6974 223a 2066 616c  ilOnSubmit": fal
+0000c750: 7365 2c0a 2020 226e 616d 6522 3a20 2270  se,.  "name": "p
+0000c760: 7965 782d 6261 7368 5f32 3330 3131 342d  yex-bash_230114-
+0000c770: 3039 3535 3034 2d35 3361 222c 0a20 2022  095504-53a",.  "
+0000c780: 6e61 6d65 7370 6163 6522 3a20 2270 7965  namespace": "pye
+0000c790: 7861 6d70 6c65 7322 2c0a 2020 2270 7269  xamples",.  "pri
+0000c7a0: 6f72 6974 7922 3a20 302c 0a20 2022 7461  ority": 0,.  "ta
+0000c7b0: 6722 3a20 2270 7965 782d 6261 7368 222c  g": "pyex-bash",
+0000c7c0: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+0000c7d0: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+0000c7e0: 6669 6e69 7368 4966 416c 6c54 6173 6b73  finishIfAllTasks
+0000c7f0: 4669 6e69 7368 6564 223a 2074 7275 652c  Finished": true,
+0000c800: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
+0000c810: 416e 7954 6173 6b46 6169 6c65 6422 3a20  AnyTaskFailed": 
+0000c820: 6661 6c73 652c 0a20 2020 2020 2022 6e61  false,.      "na
+0000c830: 6d65 223a 2022 7461 736b 5f67 726f 7570  me": "task_group
+0000c840: 5f31 222c 0a20 2020 2020 2022 7072 696f  _1",.      "prio
+0000c850: 7269 7479 223a 2030 2c0a 2020 2020 2020  rity": 0,.      
+0000c860: 2272 756e 5370 6563 6966 6963 6174 696f  "runSpecificatio
+0000c870: 6e22 3a20 7b0a 2020 2020 2020 2020 226d  n": {.        "m
+0000c880: 6178 696d 756d 5461 736b 5265 7472 6965  aximumTaskRetrie
+0000c890: 7322 3a20 302c 0a20 2020 2020 2020 2022  s": 0,.        "
+0000c8a0: 7461 736b 5479 7065 7322 3a20 5b22 6261  taskTypes": ["ba
+0000c8b0: 7368 225d 2c0a 2020 2020 2020 2020 2277  sh"],.        "w
+0000c8c0: 6f72 6b65 7254 6167 7322 3a20 5b22 7079  orkerTags": ["py
+0000c8d0: 6578 2d62 6173 6822 5d0a 2020 2020 2020  ex-bash"].      
+0000c8e0: 7d2c 0a20 2020 2020 2022 7461 736b 7322  },.      "tasks"
+0000c8f0: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+0000c900: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+0000c910: 7473 223a 205b 2270 7965 782d 6261 7368  ts": ["pyex-bash
+0000c920: 5f32 3330 3131 342d 3039 3535 3034 2d35  _230114-095504-5
+0000c930: 3361 2f73 6c65 6570 5f73 6372 6970 742e  3a/sleep_script.
+0000c940: 7368 225d 2c0a 2020 2020 2020 2020 2020  sh"],.          
+0000c950: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+0000c960: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
+0000c970: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+0000c980: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+0000c990: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
+0000c9a0: 5061 7474 6572 6e22 3a20 2270 7965 782d  Pattern": "pyex-
+0000c9b0: 6261 7368 5f32 3330 3131 342d 3039 3535  bash_230114-0955
+0000c9c0: 3034 2d35 3361 2f73 6c65 6570 5f73 6372  04-53a/sleep_scr
+0000c9d0: 6970 742e 7368 222c 0a20 2020 2020 2020  ipt.sh",.       
+0000c9e0: 2020 2020 2020 2022 736f 7572 6365 223a         "source":
+0000c9f0: 2022 5441 534b 5f4e 414d 4553 5041 4345   "TASK_NAMESPACE
+0000ca00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000ca10: 2022 7665 7269 6669 6361 7469 6f6e 223a   "verification":
+0000ca20: 2022 5645 5249 4659 5f57 4149 5422 0a20   "VERIFY_WAIT". 
+0000ca30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+0000ca40: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0000ca50: 2020 2020 226e 616d 6522 3a20 2274 6173      "name": "tas
+0000ca60: 6b5f 3031 222c 0a20 2020 2020 2020 2020  k_01",.         
+0000ca70: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
+0000ca80: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
+0000ca90: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
+0000caa0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+0000cab0: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
+0000cac0: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
+0000cad0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+0000cae0: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+0000caf0: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
+0000cb00: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+0000cb10: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2323  }.  ].}.```..###
+0000cb20: 2053 7562 6d69 7474 696e 6720 2752 6177   Submitting 'Raw
+0000cb30: 2720 4a53 4f4e 2057 6f72 6b20 5265 7175  ' JSON Work Requ
+0000cb40: 6972 656d 656e 7420 5370 6563 6966 6963  irement Specific
+0000cb50: 6174 696f 6e73 0a0a 4974 2773 2070 6f73  ations..It's pos
+0000cb60: 7369 626c 6520 746f 2075 7365 2074 6865  sible to use the
+0000cb70: 204a 534f 4e20 6f75 7470 7574 206f 6620   JSON output of 
+0000cb80: 6079 642d 7375 626d 6974 202d 2d64 7279  `yd-submit --dry
+0000cb90: 2d72 756e 6020 2873 7563 6820 6173 2074  -run` (such as t
+0000cba0: 6865 2065 7861 6d70 6c65 2061 626f 7665  he example above
+0000cbb0: 2920 6173 2061 2073 656c 662d 636f 6e74  ) as a self-cont
+0000cbc0: 6169 6e65 642c 2066 756c 6c79 2d73 7065  ained, fully-spe
+0000cbd0: 6369 6669 6564 2057 6f72 6b20 5265 7175  cified Work Requ
+0000cbe0: 6972 656d 656e 7420 7370 6563 6966 6963  irement specific
+0000cbf0: 6174 696f 6e2c 2075 7369 6e67 2074 6865  ation, using the
+0000cc00: 2060 2d2d 6a73 6f6e 2d72 6177 6020 286f   `--json-raw` (o
+0000cc10: 7220 602d 6a60 2920 636f 6d6d 616e 6420  r `-j`) command 
+0000cc20: 6c69 6e65 206f 7074 696f 6e2c 2069 2e65  line option, i.e
+0000cc30: 2e3a 2060 7964 2d73 7562 6d69 7420 2d2d  .: `yd-submit --
+0000cc40: 6a73 6f6e 2d72 6177 203c 6669 6c65 6e61  json-raw <filena
+0000cc50: 6d65 2e6a 736f 6e3e 602e 0a0a 5468 6973  me.json>`...This
+0000cc60: 2077 696c 6c20 7375 626d 6974 2074 6865   will submit the
+0000cc70: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000cc80: 742c 2074 6865 6e20 6164 6420 616c 6c20  t, then add all 
+0000cc90: 7468 6520 7370 6563 6966 6965 6420 5461  the specified Ta
+0000cca0: 736b 732e 0a0a 4e6f 7465 2074 6861 7420  sks...Note that 
+0000ccb0: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+0000ccc0: 7574 696f 6e73 202a 2a63 616e 2a2a 2062  utions **can** b
+0000ccd0: 6520 7573 6564 2069 6e20 7468 6520 7261  e used in the ra
+0000cce0: 7720 4a53 4f4e 2066 696c 652c 206a 7573  w JSON file, jus
+0000ccf0: 7420 6173 2069 6e20 7468 6520 6f74 6865  t as in the othe
+0000cd00: 7220 576f 726b 2052 6571 7569 7265 6d65  r Work Requireme
+0000cd10: 6e74 204a 534f 4e20 6578 616d 706c 6573  nt JSON examples
+0000cd20: 2c20 6275 7420 7468 6572 6520 6973 206e  , but there is n
+0000cd30: 6f20 7072 6f70 6572 7479 2069 6e68 6572  o property inher
+0000cd40: 6974 616e 6365 2c20 696e 636c 7564 696e  itance, includin
+0000cd50: 6720 6672 6f6d 2074 6865 2060 5b77 6f72  g from the `[wor
+0000cd60: 6b52 6571 7569 7265 6d65 6e74 5d60 2073  kRequirement]` s
+0000cd70: 6563 7469 6f6e 206f 6620 7468 6520 544f  ection of the TO
+0000cd80: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+0000cd90: 206f 7220 6672 6f6d 2057 6f72 6b20 5265   or from Work Re
+0000cda0: 7175 6972 656d 656e 7420 7072 6f70 6572  quirement proper
+0000cdb0: 7469 6573 2073 7570 706c 6965 6420 6f6e  ties supplied on
+0000cdc0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+0000cdd0: 652e 0a0a 4e6f 7465 2074 6861 7420 7468  e...Note that th
+0000cde0: 6572 6520 6973 206e 6f20 6175 746f 6d61  ere is no automa
+0000cdf0: 7469 6320 6669 6c65 2075 706c 6f61 6420  tic file upload 
+0000ce00: 7768 656e 2075 7369 6e67 2074 6869 7320  when using this 
+0000ce10: 6f70 7469 6f6e 2c20 736f 2061 6e79 2066  option, so any f
+0000ce20: 696c 6573 2072 6571 7569 7265 6420 6174  iles required at
+0000ce30: 2074 6865 2073 7461 7274 206f 6620 7468   the start of th
+0000ce40: 6520 7461 736b 2028 7370 6563 6966 6965  e task (specifie
+0000ce50: 6420 7573 696e 6720 6056 4552 4946 595f  d using `VERIFY_
+0000ce60: 4154 5f53 5441 5254 6029 206d 7573 7420  AT_START`) must 
+0000ce70: 6265 2070 7265 7365 6e74 2062 6566 6f72  be present befor
+0000ce80: 6520 7468 6520 5461 736b 7320 6172 6520  e the Tasks are 
+0000ce90: 7570 6c6f 6164 6564 2c20 6f72 2074 6865  uploaded, or the
+0000cea0: 2054 6173 6b73 2077 696c 6c20 6661 696c   Tasks will fail
+0000ceb0: 2069 6d6d 6564 6961 7465 6c79 2e20 5468   immediately. Th
+0000cec0: 6520 6079 642d 7570 6c6f 6164 6020 636f  e `yd-upload` co
+0000ced0: 6d6d 616e 6420 6361 6e20 6265 2075 7365  mmand can be use
+0000cee0: 6420 746f 2075 706c 6f61 6420 7468 6573  d to upload thes
+0000cef0: 6520 6669 6c65 732c 2061 6e64 2060 7964  e files, and `yd
+0000cf00: 2d73 7562 6d69 7460 2077 696c 6c20 7061  -submit` will pa
+0000cf10: 7573 6520 746f 2061 6c6c 6f77 2074 6869  use to allow thi
+0000cf20: 7320 746f 2068 6170 7065 6e2e 0a0a 2323  s to happen...##
+0000cf30: 2046 696c 6520 5374 6f72 6167 6520 4c6f   File Storage Lo
+0000cf40: 6361 7469 6f6e 7320 616e 6420 4669 6c65  cations and File
+0000cf50: 2055 7361 6765 0a0a 5468 6973 2073 6563   Usage..This sec
+0000cf60: 7469 6f6e 2064 6973 6375 7373 6573 2068  tion discusses h
+0000cf70: 6f77 2074 6f20 7570 6c6f 6164 2066 696c  ow to upload fil
+0000cf80: 6573 2066 726f 6d20 6c6f 6361 6c20 7374  es from local st
+0000cf90: 6f72 6167 6520 746f 2074 6865 2059 656c  orage to the Yel
+0000cfa0: 6c6f 7744 6f67 204f 626a 6563 7420 5374  lowDog Object St
+0000cfb0: 6f72 652c 2068 6f77 2074 686f 7365 2066  ore, how those f
+0000cfc0: 696c 6573 2061 7265 2074 7261 6e73 6665  iles are transfe
+0000cfd0: 7272 6564 2074 6f20 576f 726b 6572 204e  rred to Worker N
+0000cfe0: 6f64 6573 2066 6f72 2054 6173 6b20 7072  odes for Task pr
+0000cff0: 6f63 6573 7369 6e67 2c20 686f 7720 7468  ocessing, how th
+0000d000: 6520 7265 7375 6c74 7320 6f66 2054 6173  e results of Tas
+0000d010: 6b20 7072 6f63 6573 7369 6e67 2061 7265  k processing are
+0000d020: 2072 6574 7572 6e65 6420 6279 2057 6f72   returned by Wor
+0000d030: 6b65 7220 4e6f 6465 732c 2061 6e64 2068  ker Nodes, and h
+0000d040: 6f77 2066 696c 6573 2061 7265 2074 7261  ow files are tra
+0000d050: 6e73 6665 7272 6564 2062 6163 6b20 6672  nsferred back fr
+0000d060: 6f6d 2074 6865 2059 656c 6c6f 7744 6f67  om the YellowDog
+0000d070: 204f 626a 6563 7420 5374 6f72 6520 746f   Object Store to
+0000d080: 206c 6f63 616c 2073 746f 7261 6765 2e0a   local storage..
+0000d090: 0a23 2323 2046 696c 6573 2055 706c 6f61  .### Files Uploa
+0000d0a0: 6465 6420 746f 2074 6865 204f 626a 6563  ded to the Objec
+0000d0b0: 7420 5374 6f72 6520 6672 6f6d 204c 6f63  t Store from Loc
+0000d0c0: 616c 2053 746f 7261 6765 0a0a 2323 2323  al Storage..####
+0000d0d0: 2046 696c 6573 2069 6e20 7468 6520 6069   Files in the `i
+0000d0e0: 6e70 7574 7360 204c 6973 740a 0a57 6865  nputs` List..Whe
+0000d0f0: 6e20 6120 576f 726b 2052 6571 7569 7265  n a Work Require
+0000d100: 6d65 6e74 2069 7320 7375 626d 6974 7465  ment is submitte
+0000d110: 6420 7573 696e 6720 6079 642d 7375 626d  d using `yd-subm
+0000d120: 6974 602c 2066 696c 6573 2061 7265 2075  it`, files are u
+0000d130: 706c 6f61 6465 6420 746f 2074 6865 2059  ploaded to the Y
+0000d140: 656c 6c6f 7744 6f67 204f 626a 6563 7420  ellowDog Object 
+0000d150: 5374 6f72 6520 6966 2074 6865 7927 7265  Store if they're
+0000d160: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
+0000d170: 206c 6973 7420 6f66 2066 696c 6573 2069   list of files i
+0000d180: 6e20 7468 6520 6069 6e70 7574 7360 2070  n the `inputs` p
+0000d190: 726f 7065 7274 792e 2028 466f 7220 7468  roperty. (For th
+0000d1a0: 6520 6361 7365 206f 6620 7468 6520 6062  e case of the `b
+0000d1b0: 6173 6860 2054 6173 6b20 5479 7065 2c20  ash` Task Type, 
+0000d1c0: 7468 6520 7363 7269 7074 2073 7065 6369  the script speci
+0000d1d0: 6669 6564 2069 6e20 7468 6520 6065 7865  fied in the `exe
+0000d1e0: 6375 7461 626c 6560 2070 726f 7065 7274  cutable` propert
+0000d1f0: 7920 6973 2061 6c73 6f20 6175 746f 6d61  y is also automa
+0000d200: 7469 6361 6c6c 7920 7570 6c6f 6164 6564  tically uploaded
+0000d210: 2061 7320 6120 636f 6e76 656e 6965 6e63   as a convenienc
+0000d220: 652c 2065 7665 6e20 6966 206e 6f74 2069  e, even if not i
+0000d230: 6e63 6c75 6465 6420 696e 2074 6865 2060  ncluded in the `
+0000d240: 696e 7075 7473 6020 6c69 7374 2e29 0a0a  inputs` list.)..
+0000d250: 4669 6c65 7320 6172 6520 7570 6c6f 6164  Files are upload
+0000d260: 6564 2074 6f20 7468 6520 4e61 6d65 7370  ed to the Namesp
+0000d270: 6163 6520 7370 6563 6966 6965 6420 696e  ace specified in
+0000d280: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+0000d290: 6f6e 2e20 5769 7468 696e 2074 6865 204e  on. Within the N
+0000d2a0: 616d 6573 7061 6365 2c20 6561 6368 2057  amespace, each W
+0000d2b0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000d2c0: 6861 7320 6120 7365 7061 7261 7465 2066  has a separate f
+0000d2d0: 6f6c 6465 7220 7468 6174 2073 6861 7265  older that share
+0000d2e0: 7320 7468 6520 6e61 6d65 206f 6620 7468  s the name of th
+0000d2f0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000d300: 6e74 2c20 616e 6420 696e 2077 6869 6368  nt, and in which
+0000d310: 2061 6c6c 2066 696c 6573 2072 656c 6174   all files relat
+0000d320: 6564 2074 6f20 7468 6520 576f 726b 2052  ed to the Work R
+0000d330: 6571 7569 7265 6d65 6e74 2061 7265 2073  equirement are s
+0000d340: 746f 7265 642e 0a0a 312e 2046 696c 6573  tored...1. Files
+0000d350: 2074 6f20 6265 2075 706c 6f61 6465 6420   to be uploaded 
+0000d360: 7468 6174 2061 7265 2069 6e20 7468 6520  that are in the 
+0000d370: 2a2a 7361 6d65 2064 6972 6563 746f 7279  **same directory
+0000d380: 2061 7320 7468 6520 576f 726b 2052 6571   as the Work Req
+0000d390: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
+0000d3a0: 6361 7469 6f6e 2a2a 2028 7468 6520 544f  cation** (the TO
+0000d3b0: 4d4c 206f 7220 4a53 4f4e 2066 696c 6529  ML or JSON file)
+0000d3c0: 2061 7265 2075 706c 6f61 6465 6420 746f   are uploaded to
+0000d3d0: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+0000d3e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000d3f0: 7420 666f 6c64 6572 2e0a 0a0a 322e 2046  t folder....2. F
+0000d400: 696c 6573 2074 6f20 6265 2075 706c 6f61  iles to be uploa
+0000d410: 6465 6420 7468 6174 2061 7265 2069 6e20  ded that are in 
+0000d420: 2a2a 7375 6264 6972 6563 746f 7269 6573  **subdirectories
+0000d430: 2062 656c 6f77 2074 6865 2057 6f72 6b20   below the Work 
+0000d440: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
+0000d450: 6966 6963 6174 696f 6e2c 206f 7220 7768  ification, or wh
+0000d460: 6572 6520 6162 736f 6c75 7465 2070 6174  ere absolute pat
+0000d470: 686e 616d 6573 2061 7265 2073 7570 706c  hnames are suppl
+0000d480: 6965 642a 2a20 6172 6520 706c 6163 6564  ied** are placed
+0000d490: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
+0000d4a0: 746f 7265 2069 6e20 6469 7265 6374 6f72  tore in director
+0000d4b0: 6965 7320 7468 6174 206d 6972 726f 7220  ies that mirror 
+0000d4c0: 7468 6569 7220 6c6f 6361 6c20 7374 6f72  their local stor
+0000d4d0: 6167 6520 6c6f 6361 7469 6f6e 732e 0a0a  age locations...
+0000d4e0: 0a33 2e20 4669 6c65 7320 746f 2062 6520  .3. Files to be 
+0000d4f0: 7570 6c6f 6164 6564 2074 6861 7420 6172  uploaded that ar
+0000d500: 6520 696e 202a 2a64 6972 6563 746f 7269  e in **directori
+0000d510: 6573 2072 656c 6174 6976 6520 746f 2074  es relative to t
+0000d520: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+0000d530: 656e 7420 7370 6563 6966 6963 6174 696f  ent specificatio
+0000d540: 6e2c 2075 7369 6e67 2060 2e2e 6020 7265  n, using `..` re
+0000d550: 6c61 7469 7665 2070 6174 6873 2a2a 2061  lative paths** a
+0000d560: 7265 2070 6c61 6365 6420 696e 204f 626a  re placed in Obj
+0000d570: 6563 7420 5374 6f72 6520 6469 7265 6374  ect Store direct
+0000d580: 6f72 6965 7320 696e 2077 6869 6368 2074  ories in which t
+0000d590: 6865 2060 2e2e 6020 7061 7274 7320 6f66  he `..` parts of
+0000d5a0: 2074 6865 2070 6174 686e 616d 6520 6172   the pathname ar
+0000d5b0: 6520 7265 706c 6163 6564 2077 6974 6820  e replaced with 
+0000d5c0: 616e 2069 6e74 6567 6572 2063 6f75 6e74  an integer count
+0000d5d0: 206f 6620 7468 6520 6e75 6d62 6572 206f   of the number o
+0000d5e0: 6620 602e 2e60 2065 6e74 7269 6573 2028  f `..` entries (
+0000d5f0: 6265 6361 7573 6520 7765 2063 616e 2774  because we can't
+0000d600: 2075 7365 2074 6865 2060 2e2e 6020 7265   use the `..` re
+0000d610: 6c61 7469 7665 2066 6f72 6d20 696e 2074  lative form in t
+0000d620: 6865 204f 626a 6563 7420 5374 6f72 6529  he Object Store)
+0000d630: 2e0a 0a41 7373 756d 696e 6720 6120 4e61  ...Assuming a Na
+0000d640: 6d65 7370 6163 6520 6361 6c6c 6564 2060  mespace called `
+0000d650: 6465 7665 6c6f 706d 656e 7460 2061 6e64  development` and
+0000d660: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
+0000d670: 656e 7420 6e61 6d65 6420 6074 6573 7472  ent named `testr
+0000d680: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000d690: 2d37 6432 602c 2074 6865 2066 6f6c 6c6f  -7d2`, the follo
+0000d6a0: 7769 6e67 206c 6f63 6174 696f 6e73 2061  wing locations a
+0000d6b0: 7265 2075 7365 6420 7768 656e 2075 706c  re used when upl
+0000d6c0: 6f61 6469 6e67 2066 696c 6573 2066 6f6c  oading files fol
+0000d6d0: 6c6f 7769 6e67 2074 6865 2070 6174 7465  lowing the patte
+0000d6e0: 726e 7320 6162 6f76 653a 0a0a 6060 6073  rns above:..```s
+0000d6f0: 6865 6c6c 0a22 696e 7075 7473 2220 3a20  hell."inputs" : 
+0000d700: 5b22 6669 6c65 5f31 2e74 7874 225d 202d  ["file_1.txt"] -
+0000d710: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
+0000d720: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
+0000d730: 3034 3034 2d37 6432 2f66 696c 655f 312e  0404-7d2/file_1.
+0000d740: 7478 740a 2269 6e70 7574 7322 203a 205b  txt."inputs" : [
+0000d750: 2264 6576 2f66 696c 655f 312e 7478 7422  "dev/file_1.txt"
+0000d760: 5d20 2d3e 2064 6576 656c 6f70 6d65 6e74  ] -> development
+0000d770: 3a3a 7465 7374 7275 6e5f 3232 3131 3038  ::testrun_221108
+0000d780: 2d31 3230 3430 342d 3764 322f 6465 762f  -120404-7d2/dev/
+0000d790: 6669 6c65 5f31 2e74 7874 0a22 696e 7075  file_1.txt."inpu
+0000d7a0: 7473 2220 3a20 5b22 2f68 6f6d 652f 6465  ts" : ["/home/de
+0000d7b0: 762f 6669 6c65 5f31 2e74 7874 225d 202d  v/file_1.txt"] -
+0000d7c0: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
+0000d7d0: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
+0000d7e0: 3034 3034 2d37 6432 2f68 6f6d 652f 6465  0404-7d2/home/de
+0000d7f0: 762f 6669 6c65 5f31 2e74 7874 0a22 696e  v/file_1.txt."in
+0000d800: 7075 7473 2220 3a20 5b22 2e2e 2f64 6576  puts" : ["../dev
+0000d810: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
+0000d820: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
+0000d830: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
+0000d840: 3430 342d 3764 322f 312f 6465 762f 6669  404-7d2/1/dev/fi
+0000d850: 6c65 5f31 2e74 7874 0a22 696e 7075 7473  le_1.txt."inputs
+0000d860: 2220 3a20 5b22 2e2e 2f2e 2e2f 6465 762f  " : ["../../dev/
+0000d870: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
+0000d880: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
+0000d890: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
+0000d8a0: 3034 2d37 6432 2f32 2f64 6576 2f66 696c  04-7d2/2/dev/fil
+0000d8b0: 655f 312e 7478 740a 6060 600a 0a2a 2a55  e_1.txt.```..**U
+0000d8c0: 7369 6e67 2060 666c 6174 7465 6e55 706c  sing `flattenUpl
+0000d8d0: 6f61 6450 6174 6873 602a 2a0a 0a54 6865  oadPaths`**..The
+0000d8e0: 2060 666c 6174 7465 6e55 706c 6f61 6450   `flattenUploadP
+0000d8f0: 6174 6873 6020 7072 6f70 6572 7479 2063  aths` property c
+0000d900: 616e 2062 6520 7573 6564 2074 6f20 7375  an be used to su
+0000d910: 7070 7265 7373 2074 6865 206d 6972 726f  ppress the mirro
+0000d920: 7269 6e67 206f 6620 616e 7920 6c6f 6361  ring of any loca
+0000d930: 6c20 6469 7265 6374 6f72 7920 7374 7275  l directory stru
+0000d940: 6374 7572 6520 7768 656e 2075 706c 6f61  cture when uploa
+0000d950: 6469 6e67 2066 696c 6573 2074 6f20 7468  ding files to th
+0000d960: 6520 4f62 6a65 6374 2053 746f 7265 2e20  e Object Store. 
+0000d970: 4966 2073 6574 2074 6f20 6074 7275 6560  If set to `true`
+0000d980: 2c20 616c 6c20 6669 6c65 7320 7769 6c6c  , all files will
+0000d990: 2062 6520 7570 6c6f 6164 6564 2074 6f20   be uploaded to 
+0000d9a0: 7468 6520 726f 6f74 206f 6620 7468 6520  the root of the 
+0000d9b0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000d9c0: 2066 6f6c 6465 722e 2046 6f72 2065 7861   folder. For exa
+0000d9d0: 6d70 6c65 3a0a 0a60 6060 7368 656c 6c0a  mple:..```shell.
+0000d9e0: 2269 6e70 7574 7322 203a 205b 2266 696c  "inputs" : ["fil
+0000d9f0: 655f 312e 7478 7422 5d20 2d3e 2064 6576  e_1.txt"] -> dev
+0000da00: 656c 6f70 6d65 6e74 3a3a 7465 7374 7275  elopment::testru
+0000da10: 6e5f 3232 3131 3038 2d31 3230 3430 342d  n_221108-120404-
+0000da20: 3764 322f 6669 6c65 5f31 2e74 7874 0a22  7d2/file_1.txt."
+0000da30: 696e 7075 7473 2220 3a20 5b22 6465 762f  inputs" : ["dev/
+0000da40: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
+0000da50: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
+0000da60: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
+0000da70: 3034 2d37 6432 2f66 696c 655f 312e 7478  04-7d2/file_1.tx
+0000da80: 740a 2269 6e70 7574 7322 203a 205b 222f  t."inputs" : ["/
+0000da90: 686f 6d65 2f64 6576 2f66 696c 655f 312e  home/dev/file_1.
+0000daa0: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
+0000dab0: 6d65 6e74 3a3a 7465 7374 7275 6e5f 3232  ment::testrun_22
+0000dac0: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
+0000dad0: 6669 6c65 5f31 2e74 7874 0a22 696e 7075  file_1.txt."inpu
+0000dae0: 7473 2220 3a20 5b22 2e2e 2f64 6576 2f66  ts" : ["../dev/f
+0000daf0: 696c 655f 312e 7478 7422 5d20 2d3e 2064  ile_1.txt"] -> d
+0000db00: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
+0000db10: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
+0000db20: 342d 3764 322f 6669 6c65 5f31 2e74 7874  4-7d2/file_1.txt
+0000db30: 0a22 696e 7075 7473 2220 3a20 5b22 2e2e  ."inputs" : ["..
+0000db40: 2f2e 2e2f 6465 762f 6669 6c65 5f31 2e74  /../dev/file_1.t
+0000db50: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
+0000db60: 656e 743a 3a74 6573 7472 756e 5f32 3231  ent::testrun_221
+0000db70: 3130 382d 3132 3034 3034 2d37 6432 2f66  108-120404-7d2/f
+0000db80: 696c 655f 312e 7478 740a 6060 600a 0a54  ile_1.txt.```..T
+0000db90: 6865 2070 726f 7065 7274 7920 6465 6661  he property defa
+0000dba0: 756c 7420 6973 2060 6661 6c73 6560 2e20  ult is `false`. 
+0000dbb0: 5468 6973 2070 726f 7065 7274 7920 2a2a  This property **
+0000dbc0: 6361 6e20 6f6e 6c79 2062 6520 7365 7420  can only be set 
+0000dbd0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
+0000dbe0: 6972 656d 656e 7420 6c65 7665 6c2a 2a20  irement level** 
+0000dbf0: 616e 6420 7769 6c6c 2074 6865 7265 666f  and will therefo
+0000dc00: 7265 2061 7070 6c79 2074 6f20 616c 6c20  re apply to all 
+0000dc10: 5461 736b 2047 726f 7570 7320 616e 6420  Task Groups and 
+0000dc20: 5461 736b 7320 7769 7468 696e 2061 2057  Tasks within a W
+0000dc30: 6f72 6b20 5265 7175 6972 656d 656e 742e  ork Requirement.
+0000dc40: 0a0a 5768 656e 2066 696c 6573 2061 7070  ..When files app
+0000dc50: 6561 7220 696e 2074 6865 2060 696e 7075  ear in the `inpu
+0000dc60: 7473 6020 6c69 7374 2c20 7468 6579 2061  ts` list, they a
+0000dc70: 7265 2061 6c73 6f20 6175 746f 6d61 7469  re also automati
+0000dc80: 6361 6c6c 7920 6164 6465 6420 746f 2074  cally added to t
+0000dc90: 6865 206c 6973 7420 6f66 2066 696c 6573  he list of files
+0000dca0: 2072 6571 7569 7265 6420 6279 2074 6865   required by the
+0000dcb0: 2072 656c 6576 616e 7420 5461 736b 2873   relevant Task(s
+0000dcc0: 2920 6173 2060 5665 7269 6679 4174 5374  ) as `VerifyAtSt
+0000dcd0: 6172 7460 2064 6570 656e 6465 6e63 6965  art` dependencie
+0000dce0: 732e 0a0a 2323 2323 2046 696c 6573 2069  s...#### Files i
+0000dcf0: 6e20 7468 6520 6075 706c 6f61 6446 696c  n the `uploadFil
+0000dd00: 6573 6020 4c69 7374 0a0a 5468 6520 6075  es` List..The `u
+0000dd10: 706c 6f61 6446 696c 6573 6020 7072 6f70  ploadFiles` prop
+0000dd20: 6572 7479 2061 6c6c 6f77 7320 6d6f 7265  erty allows more
+0000dd30: 2066 6c65 7869 626c 6520 636f 6e74 726f   flexible contro
+0000dd40: 6c20 6f76 6572 2074 6865 2066 696c 6573  l over the files
+0000dd50: 2074 6f20 6265 2075 706c 6f61 6465 6420   to be uploaded 
+0000dd60: 6672 6f6d 206c 6f63 616c 2073 746f 7261  from local stora
+0000dd70: 6765 2074 6f20 7468 6520 4f62 6a65 6374  ge to the Object
+0000dd80: 2053 746f 7265 2077 6865 6e20 6079 642d   Store when `yd-
+0000dd90: 7375 626d 6974 6020 6973 2072 756e 2e20  submit` is run. 
+0000dda0: 5468 6520 7072 6f70 6572 7479 2063 616e  The property can
+0000ddb0: 2062 6520 7573 6564 2061 7420 616c 6c20   be used at all 
+0000ddc0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000ddd0: 206c 6576 656c 732c 2066 726f 6d20 7468   levels, from th
+0000dde0: 6520 544f 4d4c 2066 696c 6520 7468 726f  e TOML file thro
+0000ddf0: 7567 6820 746f 2069 6e64 6976 6964 7561  ugh to individua
+0000de00: 6c20 5461 736b 2073 7065 6369 6669 6361  l Task specifica
+0000de10: 7469 6f6e 732e 0a0a 5468 6520 7072 6f70  tions...The prop
+0000de20: 6572 7479 2069 7320 7375 7070 6c69 6564  erty is supplied
+0000de30: 2061 7320 6120 6c69 7374 206f 6620 6469   as a list of di
+0000de40: 6374 696f 6e61 7279 2069 7465 6d73 2c20  ctionary items, 
+0000de50: 6561 6368 206f 6620 7768 6963 6820 6d75  each of which mu
+0000de60: 7374 2069 6e63 6c75 6465 2074 6865 2070  st include the p
+0000de70: 726f 7065 7274 6965 7320 606c 6f63 616c  roperties `local
+0000de80: 5061 7468 6020 616e 6420 6075 706c 6f61  Path` and `uploa
+0000de90: 6450 6174 6860 2e20 0a0a 2d20 606c 6f63  dPath`. ..- `loc
+0000dea0: 616c 5061 7468 6020 7370 6563 6966 6965  alPath` specifie
+0000deb0: 7320 7468 6520 7061 7468 6e61 6d65 206f  s the pathname o
+0000dec0: 6620 7468 6520 6669 6c65 206f 6e20 6c6f  f the file on lo
+0000ded0: 6361 6c20 7374 6f72 6167 650a 2d20 6075  cal storage.- `u
+0000dee0: 706c 6f61 6450 6174 6860 2073 7065 6369  ploadPath` speci
+0000def0: 6669 6573 2074 6865 206e 616d 6520 616e  fies the name an
+0000df00: 6420 6c6f 6361 7469 6f6e 206f 6620 7468  d location of th
+0000df10: 6520 6669 6c65 2773 2064 6573 7469 6e61  e file's destina
+0000df20: 7469 6f6e 2069 6e20 7468 6520 4f62 6a65  tion in the Obje
+0000df30: 6374 2053 746f 7265 0a0a 466f 7220 6578  ct Store..For ex
+0000df40: 616d 706c 652c 2069 6e20 544f 4d4c 3a0a  ample, in TOML:.
+0000df50: 6060 6074 6f6d 6c0a 7570 6c6f 6164 4669  ```toml.uploadFi
+0000df60: 6c65 7320 3d20 5b0a 2020 2020 7b6c 6f63  les = [.    {loc
+0000df70: 616c 5061 7468 203d 2022 6669 6c65 5f31  alPath = "file_1
+0000df80: 2e74 7874 222c 2075 706c 6f61 6450 6174  .txt", uploadPat
+0000df90: 6820 3d20 2266 696c 655f 312e 7478 7422  h = "file_1.txt"
+0000dfa0: 7d2c 0a20 2020 207b 6c6f 6361 6c50 6174  },.    {localPat
+0000dfb0: 6820 3d20 2264 6972 5f32 2f66 696c 655f  h = "dir_2/file_
+0000dfc0: 322e 7478 7422 2c20 7570 6c6f 6164 5061  2.txt", uploadPa
+0000dfd0: 7468 203d 2022 3a3a 6669 6c65 5f32 2e74  th = "::file_2.t
+0000dfe0: 7874 227d 2c0a 2020 2020 7b6c 6f63 616c  xt"},.    {local
+0000dff0: 5061 7468 203d 2022 6669 6c65 5f33 2e74  Path = "file_3.t
+0000e000: 7874 222c 2075 706c 6f61 6450 6174 6820  xt", uploadPath 
+0000e010: 3d20 226f 7468 6572 5f6e 616d 6573 7061  = "other_namespa
+0000e020: 6365 3a3a 6669 6c65 5f33 2e74 7874 227d  ce::file_3.txt"}
+0000e030: 0a5d 0a60 6060 0a41 6e64 2069 6e20 4a53  .].```.And in JS
+0000e040: 4f4e 2c20 7769 7468 2074 6865 2070 726f  ON, with the pro
+0000e050: 7065 7274 7920 7365 7420 6174 2074 6865  perty set at the
+0000e060: 2054 6173 6b20 6c65 7665 6c2c 2074 6865   Task level, the
+0000e070: 2073 616d 6520 7370 6563 6966 6963 6174   same specificat
+0000e080: 696f 6e20 776f 756c 6420 6265 3a0a 6060  ion would be:.``
+0000e090: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
+0000e0a0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+0000e0b0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+0000e0c0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+0000e0d0: 2020 2020 2022 7570 6c6f 6164 4669 6c65       "uploadFile
+0000e0e0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+0000e0f0: 2020 7b22 6c6f 6361 6c50 6174 6822 3a20    {"localPath": 
+0000e100: 2266 696c 655f 312e 7478 7422 2c20 2275  "file_1.txt", "u
+0000e110: 706c 6f61 6450 6174 6822 3a20 2266 696c  ploadPath": "fil
+0000e120: 655f 312e 7478 7422 7d2c 0a20 2020 2020  e_1.txt"},.     
+0000e130: 2020 2020 2020 207b 226c 6f63 616c 5061         {"localPa
+0000e140: 7468 223a 2022 6469 725f 322f 6669 6c65  th": "dir_2/file
+0000e150: 5f32 2e74 7874 222c 2022 7570 6c6f 6164  _2.txt", "upload
+0000e160: 5061 7468 223a 2022 3a3a 6669 6c65 5f32  Path": "::file_2
+0000e170: 2e74 7874 227d 2c0a 2020 2020 2020 2020  .txt"},.        
+0000e180: 2020 2020 7b22 6c6f 6361 6c50 6174 6822      {"localPath"
+0000e190: 3a20 2266 696c 655f 332e 7478 7422 2c20  : "file_3.txt", 
+0000e1a0: 2275 706c 6f61 6450 6174 6822 3a20 226f  "uploadPath": "o
+0000e1b0: 7468 6572 5f6e 616d 6573 7061 6365 3a3a  ther_namespace::
+0000e1c0: 6669 6c65 5f33 2e74 7874 227d 0a20 2020  file_3.txt"}.   
+0000e1d0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0000e1e0: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
+0000e1f0: 0a20 205d 0a7d 0a60 6060 0a0a 5768 656e  .  ].}.```..When
+0000e200: 2072 756e 6e69 6e67 2074 6865 2050 7974   running the Pyt
+0000e210: 686f 6e20 4578 616d 706c 6573 2063 6f6d  hon Examples com
+0000e220: 6d61 6e64 7320 6f6e 202a 2a57 696e 646f  mands on **Windo
+0000e230: 7773 2a2a 2068 6f73 7473 2c20 6e6f 7465  ws** hosts, note
+0000e240: 2074 6861 7420 6569 7468 6572 2057 696e   that either Win
+0000e250: 646f 7773 206f 7220 556e 6978 2064 6972  dows or Unix dir
+0000e260: 6563 746f 7279 2073 6570 6172 6174 6f72  ectory separator
+0000e270: 7320 6361 6e20 6265 2075 7365 6420 666f  s can be used fo
+0000e280: 7220 7468 6520 606c 6f63 616c 5061 7468  r the `localPath
+0000e290: 6020 7061 7468 6e61 6d65 7320 286f 7220  ` pathnames (or 
+0000e2a0: 7468 6520 7061 7468 6e61 6d65 7320 696e  the pathnames in
+0000e2b0: 2060 696e 7075 7473 6029 2c20 6275 7420   `inputs`), but 
+0000e2c0: 7468 6520 556e 6978 2063 6f6e 7665 6e74  the Unix convent
+0000e2d0: 696f 6e20 6d75 7374 2062 6520 7573 6564  ion must be used
+0000e2e0: 2066 6f72 2074 6865 2060 7570 6c6f 6164   for the `upload
+0000e2f0: 5061 7468 6020 6e61 6d65 732c 2065 2e67  Path` names, e.g
+0000e300: 2e3a 0a0a 6060 6074 6f6d 6c0a 7570 6c6f  .:..```toml.uplo
+0000e310: 6164 4669 6c65 7320 3d20 5b0a 2020 2020  adFiles = [.    
+0000e320: 7b6c 6f63 616c 5061 7468 203d 2022 6469  {localPath = "di
+0000e330: 725f 325c 5c66 696c 655f 322e 7478 7422  r_2\\file_2.txt"
+0000e340: 2c20 7570 6c6f 6164 5061 7468 203d 2022  , uploadPath = "
+0000e350: 3a3a 6d79 5f64 6972 6563 746f 7279 2f66  ::my_directory/f
+0000e360: 696c 655f 322e 7478 7422 7d2c 0a5d 0a60  ile_2.txt"},.].`
+0000e370: 6060 0a0a 5468 6520 6075 706c 6f61 6446  ``..The `uploadF
+0000e380: 696c 6573 6020 7072 6f70 6572 7479 2063  iles` property c
+0000e390: 616e 2061 6c73 6f20 6265 2073 6574 2061  an also be set a
+0000e3a0: 7420 7468 6520 576f 726b 2052 6571 7569  t the Work Requi
+0000e3b0: 7265 6d65 6e74 2061 6e64 2054 6173 6b20  rement and Task 
+0000e3c0: 4772 6f75 7020 6c65 7665 6c73 2c20 616e  Group levels, an
+0000e3d0: 6420 7072 6f70 6572 7479 2069 6e68 6572  d property inher
+0000e3e0: 6974 616e 6365 206f 7065 7261 7465 7320  itance operates 
+0000e3f0: 6173 206e 6f72 6d61 6c2e 0a0a 466f 7220  as normal...For 
+0000e400: 6075 706c 6f61 6450 6174 6860 2c20 7468  `uploadPath`, th
+0000e410: 6520 7361 6d65 2060 3a3a 6020 6e61 6d69  e same `::` nami
+0000e420: 6e67 2063 6f6e 7665 6e74 696f 6e20 6973  ng convention is
+0000e430: 2061 7661 696c 6162 6c65 2061 7320 6973   available as is
+0000e440: 2075 7365 6420 696e 2074 6865 2060 7665   used in the `ve
+0000e450: 7269 6679 4174 5374 6172 7460 2c20 6076  rifyAtStart`, `v
+0000e460: 6572 6966 7957 6169 7460 2061 6e64 2060  erifyWait` and `
+0000e470: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
+0000e480: 7072 6f70 6572 7469 6573 2064 6973 6375  properties discu
+0000e490: 7373 6564 2062 656c 6f77 3a0a 0a2d 2049  ssed below:..- I
+0000e4a0: 6620 603a 3a60 2069 7320 6e6f 7420 7573  f `::` is not us
+0000e4b0: 6564 2c20 7468 656e 2074 6865 2066 696c  ed, then the fil
+0000e4c0: 6520 6973 2075 706c 6f61 6465 6420 7265  e is uploaded re
+0000e4d0: 6c61 7469 7665 2074 6f20 7468 6520 6375  lative to the cu
+0000e4e0: 7272 656e 7420 6e61 6d65 7370 6163 6520  rrent namespace 
+0000e4f0: 696e 2061 2064 6972 6563 746f 7279 206e  in a directory n
+0000e500: 616d 6564 2061 6674 6572 2074 6865 206e  amed after the n
+0000e510: 616d 6520 6f66 2074 6865 2057 6f72 6b20  ame of the Work 
+0000e520: 5265 7175 6972 656d 656e 740a 2d20 4966  Requirement.- If
+0000e530: 2060 3a3a 6020 6973 2075 7365 6420 6174   `::` is used at
+0000e540: 2074 6865 2073 7461 7274 206f 6620 7468   the start of th
+0000e550: 6520 6075 706c 6f61 6450 6174 6860 2c20  e `uploadPath`, 
+0000e560: 7468 6520 6669 6c65 2069 7320 7570 6c6f  the file is uplo
+0000e570: 6164 6564 2072 656c 6174 6976 6520 746f  aded relative to
+0000e580: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+0000e590: 2063 7572 7265 6e74 206e 616d 6573 7061   current namespa
+0000e5a0: 6365 0a2d 2049 6620 603c 6e61 6d65 7370  ce.- If `<namesp
+0000e5b0: 6163 653e 3a3a 6020 6973 2075 7365 6420  ace>::` is used 
+0000e5c0: 6174 2074 6865 2073 7461 7274 206f 6620  at the start of 
+0000e5d0: 6075 706c 6f61 6450 6174 6860 2c20 7468  `uploadPath`, th
+0000e5e0: 6520 6669 6c65 2069 7320 7570 6c6f 6164  e file is upload
+0000e5f0: 6564 2072 656c 6174 6976 6520 746f 2074  ed relative to t
+0000e600: 6865 2072 6f6f 7420 6f66 2060 3c6e 616d  he root of `<nam
+0000e610: 6573 7061 6365 3e60 0a0a 4561 6368 2066  espace>`..Each f
+0000e620: 696c 6520 7370 6563 6966 6965 6420 696e  ile specified in
+0000e630: 2074 6865 2060 7570 6c6f 6164 4669 6c65   the `uploadFile
+0000e640: 7360 206c 6973 7473 2077 696c 6c20 6f6e  s` lists will on
+0000e650: 6c79 2062 6520 7570 6c6f 6164 6564 206f  ly be uploaded o
+0000e660: 6e63 6520 746f 2065 6163 6820 756e 6971  nce to each uniq
+0000e670: 7565 2075 706c 6f61 6420 6c6f 6361 7469  ue upload locati
+0000e680: 6f6e 2066 6f72 2061 6e79 2067 6976 656e  on for any given
+0000e690: 2069 6e76 6f63 6174 696f 6e20 6f66 2060   invocation of `
+0000e6a0: 7964 2d73 7562 6d69 7460 2e0a 0a49 6620  yd-submit`...If 
+0000e6b0: 6120 6669 6c65 2069 6e20 7468 6520 6075  a file in the `u
+0000e6c0: 706c 6f61 6446 696c 6573 6020 6c69 7374  ploadFiles` list
+0000e6d0: 2069 7320 7265 7175 6972 6564 2062 7920   is required by 
+0000e6e0: 6120 5461 736b 2c20 6974 206d 7573 7420  a Task, it must 
+0000e6f0: 7365 7061 7261 7465 6c79 2062 6520 6164  separately be ad
+0000e700: 6465 6420 746f 2074 6865 2060 7665 7269  ded to the `veri
+0000e710: 6679 4174 5374 6172 7460 206f 7220 6076  fyAtStart` or `v
+0000e720: 6572 6966 7957 6169 7460 206c 6973 7473  erifyWait` lists
+0000e730: 2064 6973 6375 7373 6564 2062 656c 6f77   discussed below
+0000e740: 2e20 5468 6973 2069 7320 6e6f 7420 646f  . This is not do
+0000e750: 6e65 2061 7574 6f6d 6174 6963 616c 6c79  ne automatically
+0000e760: 2e20 4e6f 7465 2061 6c73 6f20 7468 6174  . Note also that
+0000e770: 2074 6865 2060 666c 6174 7465 6e55 706c   the `flattenUpl
+0000e780: 6f61 6450 6174 6873 6020 7072 6f70 6572  oadPaths` proper
+0000e790: 7479 2069 7320 6967 6e6f 7265 6420 666f  ty is ignored fo
+0000e7a0: 7220 6669 6c65 7320 696e 2074 6865 2060  r files in the `
+0000e7b0: 7570 6c6f 6164 4669 6c65 7360 206c 6973  uploadFiles` lis
+0000e7c0: 742e 0a0a 2323 2320 4669 6c65 2044 6570  t...### File Dep
+0000e7d0: 656e 6465 6e63 6965 7320 5573 696e 6720  endencies Using 
+0000e7e0: 6076 6572 6966 7941 7453 7461 7274 6020  `verifyAtStart` 
+0000e7f0: 616e 6420 6076 6572 6966 7957 6169 7460  and `verifyWait`
+0000e800: 0a0a 4974 2773 2070 6f73 7369 626c 6520  ..It's possible 
+0000e810: 746f 206d 616b 6520 5461 736b 7320 6465  to make Tasks de
+0000e820: 7065 6e64 656e 7420 6f6e 2074 6865 2070  pendent on the p
+0000e830: 7265 7365 6e63 6520 6f66 2066 696c 6573  resence of files
+0000e840: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
+0000e850: 746f 7265 2062 7920 7573 696e 6720 7468  tore by using th
+0000e860: 6520 6076 6572 6966 7941 7453 7461 7274  e `verifyAtStart
+0000e870: 6020 616e 6420 6076 6572 6966 7957 6169  ` and `verifyWai
+0000e880: 7460 206c 6973 7473 2e20 5468 6573 6520  t` lists. These 
+0000e890: 6669 6c65 7320 6172 6520 6e6f 7420 6175  files are not au
+0000e8a0: 746f 6d61 7469 6361 6c6c 7920 7570 6c6f  tomatically uplo
+0000e8b0: 6164 6564 2077 6865 6e20 7573 696e 6720  aded when using 
+0000e8c0: 6079 642d 7375 626d 6974 6020 736f 2061  `yd-submit` so a
+0000e8d0: 7265 2065 6974 6865 7220 7570 6c6f 6164  re either upload
+0000e8e0: 6564 206d 616e 7561 6c6c 7920 2865 2e67  ed manually (e.g
+0000e8f0: 2e2c 2062 7920 7573 696e 6720 6079 642d  ., by using `yd-
+0000e900: 7570 6c6f 6164 6029 2c20 6f72 2061 7265  upload`), or are
+0000e910: 2063 7265 6174 6564 2061 7320 6120 7265   created as a re
+0000e920: 7375 6c74 206f 6620 7468 6520 6578 6563  sult of the exec
+0000e930: 7574 696f 6e20 6f66 206f 7468 6572 2054  ution of other T
+0000e940: 6173 6b73 2e0a 0a4e 6f74 6520 7468 6174  asks...Note that
+0000e950: 2061 2067 6976 656e 2066 696c 6520 6361   a given file ca
+0000e960: 6e20 6f6e 6c79 2061 7070 6561 7220 696e  n only appear in
+0000e970: 202a 6f6e 652a 206f 6620 7468 6520 6069   *one* of the `i
+0000e980: 6e70 7574 7360 2c20 6076 6572 6966 7941  nputs`, `verifyA
+0000e990: 7453 7461 7274 6020 6f72 2060 7665 7269  tStart` or `veri
+0000e9a0: 6679 5761 6974 6020 6c69 7374 732e 0a0a  fyWait` lists...
+0000e9b0: 5461 736b 7320 7769 7468 2060 7665 7269  Tasks with `veri
+0000e9c0: 6679 4174 5374 6172 7460 2064 6570 656e  fyAtStart` depen
+0000e9d0: 6465 6e63 6965 7320 7769 6c6c 2066 6169  dencies will fai
+0000e9e0: 6c20 696d 6d65 6469 6174 656c 7920 6966  l immediately if
+0000e9f0: 2074 6865 2072 6571 7569 7265 6420 6669   the required fi
+0000ea00: 6c65 7320 6172 6520 6e6f 7420 7072 6573  les are not pres
+0000ea10: 656e 7420 7768 656e 2074 6865 2054 6173  ent when the Tas
+0000ea20: 6b20 6973 2073 7562 6d69 7474 6564 2e20  k is submitted. 
+0000ea30: 5461 736b 7320 7769 7468 2060 7665 7269  Tasks with `veri
+0000ea40: 6679 5761 6974 6020 6465 7065 6e64 656e  fyWait` dependen
+0000ea50: 6369 6573 2077 696c 6c20 6e6f 7420 6265  cies will not be
+0000ea60: 636f 6d65 2060 5245 4144 5960 2074 6f20  come `READY` to 
+0000ea70: 6265 2073 6368 6564 756c 6564 2074 6f20  be scheduled to 
+0000ea80: 576f 726b 6572 7320 756e 7469 6c20 7468  Workers until th
+0000ea90: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
+0000eaa0: 7265 2073 6174 6973 6669 6564 2e0a 0a57  re satisfied...W
+0000eab0: 6865 6e20 7370 6563 6966 7969 6e67 2066  hen specifying f
+0000eac0: 696c 6573 2069 6e20 7468 6520 6076 6572  iles in the `ver
+0000ead0: 6966 7941 7453 7461 7274 6020 616e 6420  ifyAtStart` and 
+0000eae0: 6076 6572 6966 7957 6169 7460 206c 6973  `verifyWait` lis
+0000eaf0: 7473 2c20 6173 2077 6974 6820 7468 6520  ts, as with the 
+0000eb00: 6075 706c 6f61 6450 6174 6860 2070 726f  `uploadPath` pro
+0000eb10: 7065 7274 7920 6469 7363 7573 7365 6420  perty discussed 
+0000eb20: 6162 6f76 652c 2074 6865 2066 696c 6520  above, the file 
+0000eb30: 6c6f 6361 7469 6f6e 7320 6361 6e20 6265  locations can be
+0000eb40: 2028 3129 2072 656c 6174 6976 6520 746f   (1) relative to
+0000eb50: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+0000eb60: 656d 656e 7420 6e61 6d65 2069 6e20 7468  ement name in th
+0000eb70: 6520 6375 7272 656e 7420 6e61 6d65 7370  e current namesp
+0000eb80: 6163 6520 2874 6865 2064 6566 6175 6c74  ace (the default
+0000eb90: 292c 2028 3229 2072 656c 6174 6976 6520  ), (2) relative 
+0000eba0: 746f 2074 6865 2072 6f6f 7420 6f66 2074  to the root of t
+0000ebb0: 6865 2063 7572 7265 6e74 206e 616d 6573  he current names
+0000ebc0: 7061 6365 2c20 6f72 2028 3329 2072 656c  pace, or (3) rel
+0000ebd0: 6174 6976 6520 746f 2074 6865 2072 6f6f  ative to the roo
+0000ebe0: 7420 6f66 2061 2064 6966 6665 7265 6e74  t of a different
+0000ebf0: 206e 616d 6573 7061 6365 2069 6e20 7468   namespace in th
+0000ec00: 6520 7573 6572 2773 2041 6363 6f75 6e74  e user's Account
+0000ec10: 2e0a 0a31 2e20 466f 7220 6669 6c65 7320  ...1. For files 
+0000ec20: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
+0000ec30: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000ec40: 206e 616d 6520 696e 2074 6865 2063 7572   name in the cur
+0000ec50: 7265 6e74 206e 616d 6573 7061 6365 2c20  rent namespace, 
+0000ec60: 6a75 7374 2075 7365 2074 6865 2066 696c  just use the fil
+0000ec70: 6520 7061 7468 2c20 652e 672e 0a60 6060  e path, e.g..```
+0000ec80: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
+0000ec90: 7422 3a20 5b22 6669 6c65 5f31 2e74 7874  t": ["file_1.txt
+0000eca0: 225d 202d 3e20 6465 7665 6c6f 706d 656e  "] -> developmen
+0000ecb0: 743a 7465 7374 7275 6e5f 3232 3131 3038  t:testrun_221108
+0000ecc0: 2d31 3230 3430 342d 3764 322f 6669 6c65  -120404-7d2/file
+0000ecd0: 5f31 2e74 7874 0a60 6060 0a0a 322e 2046  _1.txt.```..2. F
+0000ece0: 6f72 2066 696c 6573 2072 656c 6174 6976  or files relativ
+0000ecf0: 6520 746f 2074 6865 2072 6f6f 7420 6f66  e to the root of
+0000ed00: 2074 6865 2063 7572 7265 6e74 206e 616d   the current nam
+0000ed10: 6573 7061 6365 2c20 7072 6566 6978 2074  espace, prefix t
+0000ed20: 6865 2066 696c 6520 7061 7468 2077 6974  he file path wit
+0000ed30: 6820 603a 3a60 2c20 652e 672e 0a60 6060  h `::`, e.g..```
+0000ed40: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
+0000ed50: 7422 3a20 5b22 3a3a 6669 6c65 5f31 2e74  t": ["::file_1.t
+0000ed60: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
+0000ed70: 656e 743a 6669 6c65 5f31 2e74 7874 0a60  ent:file_1.txt.`
+0000ed80: 6060 0a0a 332e 2046 6f72 2066 696c 6573  ``..3. For files
+0000ed90: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+0000eda0: 2072 6f6f 7420 6f66 2061 2064 6966 6665   root of a diffe
+0000edb0: 7265 6e74 206e 616d 6573 7061 6365 2c20  rent namespace, 
+0000edc0: 7072 6566 6978 2074 6865 2066 696c 6520  prefix the file 
+0000edd0: 7061 7468 2077 6974 6820 7468 6520 6e61  path with the na
+0000ede0: 6d65 7370 6163 6520 6e61 6d65 2061 6e64  mespace name and
+0000edf0: 2060 3a3a 602c 2065 2e67 2e0a 6060 6073   `::`, e.g..```s
+0000ee00: 6865 6c6c 0a22 7665 7269 6679 5761 6974  hell."verifyWait
+0000ee10: 223a 205b 226f 7468 6572 5f6e 616d 6573  ": ["other_names
+0000ee20: 7061 6365 3a3a 6669 6c65 5f31 2e74 7874  pace::file_1.txt
+0000ee30: 225d 202d 3e20 6f74 6865 725f 6e61 6d65  "] -> other_name
+0000ee40: 7370 6163 653a 6669 6c65 5f31 2e74 7874  space:file_1.txt
+0000ee50: 0a60 6060 0a0a 5468 6520 7573 6520 6f66  .```..The use of
+0000ee60: 2074 6865 2074 6872 6565 2064 6966 6665   the three diffe
+0000ee70: 7265 6e74 2066 6f72 6d73 2063 616e 2062  rent forms can b
+0000ee80: 6520 6d69 7865 6420 7769 7468 696e 2061  e mixed within a
+0000ee90: 2073 696e 676c 6520 6c69 7374 2c20 652e   single list, e.
+0000eea0: 672e 3a0a 6060 6073 6865 6c6c 0a22 7665  g.:.```shell."ve
+0000eeb0: 7269 6679 4174 5374 6172 7422 3a20 5b22  rifyAtStart": ["
+0000eec0: 6669 6c65 5f31 2e74 7874 222c 2022 3a3a  file_1.txt", "::
+0000eed0: 6469 725f 322f 6669 6c65 5f32 2e74 7874  dir_2/file_2.txt
+0000eee0: 222c 2022 6f74 6865 725f 6e61 6d65 7370  ", "other_namesp
+0000eef0: 6163 653a 3a64 6972 5f33 2f66 696c 655f  ace::dir_3/file_
+0000ef00: 332e 7478 7422 5d0a 6060 600a 0a23 2323  3.txt"].```..###
+0000ef10: 2046 696c 6573 2044 6f77 6e6c 6f61 6465   Files Downloade
+0000ef20: 6420 5573 696e 6720 6069 6e70 7574 734f  d Using `inputsO
+0000ef30: 7074 696f 6e61 6c60 0a0a 5468 6520 6069  ptional`..The `i
+0000ef40: 6e70 7574 734f 7074 696f 6e61 6c60 2070  nputsOptional` p
+0000ef50: 726f 7065 7274 7920 776f 726b 7320 696e  roperty works in
+0000ef60: 2061 2073 696d 696c 6172 2066 6173 6869   a similar fashi
+0000ef70: 6f6e 2074 6f20 7468 6520 6076 6572 6966  on to the `verif
+0000ef80: 792a 6020 7072 6f70 6572 7469 6573 2061  y*` properties a
+0000ef90: 626f 7665 2c20 6275 7420 7468 6520 6669  bove, but the fi
+0000efa0: 6c65 7320 7370 6563 6966 6965 6420 696e  les specified in
+0000efb0: 2074 6869 7320 6c69 7374 2061 7265 206f   this list are o
+0000efc0: 7074 696f 6e61 6c2e 2054 6869 7320 7072  ptional. This pr
+0000efd0: 6f70 6572 7479 2061 6c73 6f20 616c 6c6f  operty also allo
+0000efe0: 7773 2066 6f72 2074 6865 2075 7365 206f  ws for the use o
+0000eff0: 6620 7769 6c64 6361 7264 7320 602a 6020  f wildcards `*` 
+0000f000: 616e 6420 602a 2a60 2074 6f20 636f 6c6c  and `**` to coll
+0000f010: 6563 7420 6669 6c65 7320 7573 696e 6720  ect files using 
+0000f020: 7769 6c64 6361 7264 2070 6174 6873 2e20  wildcard paths. 
+0000f030: 5468 6520 2a2a 616e 742a 2a20 636f 6e76  The **ant** conv
+0000f040: 656e 7469 6f6e 7320 6172 6520 7573 6564  entions are used
+0000f050: 2066 6f72 2074 6865 7365 2077 696c 6463   for these wildc
+0000f060: 6172 6473 2e0a 0a23 2323 2046 696c 6573  ards...### Files
+0000f070: 2044 6f77 6e6c 6f61 6465 6420 746f 2061   Downloaded to a
+0000f080: 204e 6f64 6520 666f 7220 7573 6520 696e   Node for use in
+0000f090: 2054 6173 6b20 4578 6563 7574 696f 6e0a   Task Execution.
+0000f0a0: 0a57 6865 6e20 6120 5461 736b 2069 7320  .When a Task is 
+0000f0b0: 6578 6563 7574 6564 2062 7920 6120 576f  executed by a Wo
+0000f0c0: 726b 6572 206f 6e20 6120 4e6f 6465 2c20  rker on a Node, 
+0000f0d0: 6974 7320 7265 7175 6972 6564 2066 696c  its required fil
+0000f0e0: 6573 2061 7265 2064 6f77 6e6c 6f61 6465  es are downloade
+0000f0f0: 6420 6672 6f6d 2074 6865 204f 626a 6563  d from the Objec
+0000f100: 7420 5374 6f72 6520 7072 696f 7220 746f  t Store prior to
+0000f110: 2054 6173 6b20 6578 6563 7574 696f 6e2e   Task execution.
+0000f120: 2041 6e79 2066 696c 6520 6c69 7374 6564   Any file listed
+0000f130: 2069 6e20 7468 6520 6069 6e70 7574 7360   in the `inputs`
+0000f140: 2066 6f72 2061 2054 6173 6b20 6973 2061   for a Task is a
+0000f150: 7373 756d 6564 2074 6f20 6265 2072 6571  ssumed to be req
+0000f160: 7569 7265 642c 2061 6c6f 6e67 2077 6974  uired, along wit
+0000f170: 6820 616e 7920 6164 6469 7469 6f6e 616c  h any additional
+0000f180: 2066 696c 6573 2073 7065 6369 6669 6564   files specified
+0000f190: 2069 6e20 7468 6520 6076 6572 6966 7941   in the `verifyA
+0000f1a0: 7453 7461 7274 6020 616e 6420 6076 6572  tStart` and `ver
+0000f1b0: 6966 7957 6169 7460 206c 6973 7473 2e20  ifyWait` lists. 
+0000f1c0: 4669 6c65 7320 7370 6563 6966 6965 6420  Files specified 
+0000f1d0: 7573 696e 6720 7468 6520 6069 6e70 7574  using the `input
+0000f1e0: 734f 7074 696f 6e61 6c60 2070 726f 7065  sOptional` prope
+0000f1f0: 7274 7920 6172 6520 6f70 7469 6f6e 616c  rty are optional
+0000f200: 6c79 2064 6f77 6e6c 6f61 6465 6420 6672  ly downloaded fr
+0000f210: 6f6d 2074 6865 204f 626a 6563 7420 5374  om the Object St
+0000f220: 6f72 652e 2028 4e6f 7465 2074 6861 7420  ore. (Note that 
+0000f230: 6120 6669 6c65 2073 686f 756c 6420 6f6e  a file should on
+0000f240: 6c79 2061 7070 6561 7220 696e 206f 6e65  ly appear in one
+0000f250: 206f 6620 7468 6573 6520 666f 7572 206c   of these four l
+0000f260: 6973 7473 2c20 6f74 6865 7277 6973 6520  ists, otherwise 
+0000f270: 6079 642d 7375 626d 6974 6020 7769 6c6c  `yd-submit` will
+0000f280: 2072 6574 7572 6e20 616e 2065 7272 6f72   return an error
+0000f290: 2e29 0a0a 5768 656e 2061 2054 6173 6b20  .)..When a Task 
+0000f2a0: 6973 2073 7461 7274 6564 2062 7920 7468  is started by th
+0000f2b0: 6520 4167 656e 742c 2069 7473 2077 6f72  e Agent, its wor
+0000f2c0: 6b69 6e67 2064 6972 6563 746f 7279 2068  king directory h
+0000f2d0: 6173 2061 2070 6174 7465 726e 2073 6f6d  as a pattern som
+0000f2e0: 6574 6869 6e67 206c 696b 653a 0a0a 602f  ething like:..`/
+0000f2f0: 7661 722f 6f70 742f 7965 6c6c 6f77 646f  var/opt/yellowdo
+0000f300: 672f 7964 2d61 6765 6e74 2d34 2f64 6174  g/yd-agent-4/dat
+0000f310: 612f 776f 726b 6572 732f 312f 7964 6964  a/workers/1/ydid
+0000f320: 5f74 6173 6b5f 4430 4430 4430 5f36 3866  _task_D0D0D0_68f
+0000f330: 3565 3562 652d 6463 3933 2d34 3965 622d  5e5be-dc93-49eb-
+0000f340: 6138 3234 2d31 6663 6462 3532 6639 3139  a824-1fcdb52f919
+0000f350: 355f 315f 3160 0a0a 2860 7964 6964 5f74  5_1_1`..(`ydid_t
+0000f360: 6173 6b5f 4430 4430 4430 5f36 3866 3565  ask_D0D0D0_68f5e
+0000f370: 3562 652d 6463 3933 2d34 3965 622d 6138  5be-dc93-49eb-a8
+0000f380: 3234 2d31 6663 6462 3532 6639 3139 355f  24-1fcdb52f9195_
+0000f390: 315f 3160 2069 7320 616e 2065 7068 656d  1_1` is an ephem
+0000f3a0: 6572 616c 2064 6972 6563 746f 7279 2074  eral directory t
+0000f3b0: 6861 7420 6973 2072 656d 6f76 6564 2061  hat is removed a
+0000f3c0: 6674 6572 2074 6865 2054 6173 6b20 6669  fter the Task fi
+0000f3d0: 6e69 7368 6573 2061 6e64 2061 6e79 206f  nishes and any o
+0000f3e0: 7574 7075 7473 2068 6176 6520 6265 656e  utputs have been
+0000f3f0: 2075 706c 6f61 6465 642e 290a 0a46 696c   uploaded.)..Fil
+0000f400: 6573 2074 6861 7420 6172 6520 646f 776e  es that are down
+0000f410: 6c6f 6164 6564 2062 7920 7468 6520 4167  loaded by the Ag
+0000f420: 656e 7420 7072 696f 7220 746f 2054 6173  ent prior to Tas
+0000f430: 6b20 6578 6563 7574 696f 6e20 6172 6520  k execution are 
+0000f440: 6c6f 6361 7465 6420 6173 2066 6f6c 6c6f  located as follo
+0000f450: 7773 3a0a 0a31 2e20 4966 2074 6865 2060  ws:..1. If the `
+0000f460: 666c 6174 7465 6e49 6e70 7574 5061 7468  flattenInputPath
+0000f470: 7360 2070 726f 7065 7274 7920 6973 2073  s` property is s
+0000f480: 6574 2074 6f20 7468 6520 6465 6661 756c  et to the defaul
+0000f490: 7420 6f66 2060 6661 6c73 6560 2066 6f72  t of `false` for
+0000f4a0: 2074 6865 2054 6173 6b2c 2074 6865 2064   the Task, the d
+0000f4b0: 6f77 6e6c 6f61 6465 6420 6f62 6a65 6374  ownloaded object
+0000f4c0: 7320 6172 6520 706c 6163 6564 2069 6e20  s are placed in 
+0000f4d0: 7375 6264 6972 6563 746f 7269 6573 2074  subdirectories t
+0000f4e0: 6861 7420 6d69 7272 6f72 2074 686f 7365  hat mirror those
+0000f4f0: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
+0000f500: 746f 7265 2c20 696e 636c 7564 696e 6720  tore, including 
+0000f510: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+0000f520: 6d65 6e74 206e 616d 652c 2073 6974 7561  ment name, situa
+0000f530: 7465 6420 6265 6e65 6174 6820 7468 6520  ted beneath the 
+0000f540: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+0000f550: 792e 0a0a 0a32 2e20 4966 2074 6865 2060  y....2. If the `
+0000f560: 666c 6174 7465 6e49 6e70 7574 5061 7468  flattenInputPath
+0000f570: 7360 2070 726f 7065 7274 7920 6973 2073  s` property is s
+0000f580: 6574 2074 6f20 6074 7275 6560 2066 6f72  et to `true` for
+0000f590: 2074 6865 2054 6173 6b2c 2074 6865 2064   the Task, the d
+0000f5a0: 6f77 6e6c 6f61 6465 6420 6f62 6a65 6374  ownloaded object
+0000f5b0: 7320 6172 6520 616c 6c20 706c 6163 6564  s are all placed
+0000f5c0: 2064 6972 6563 746c 7920 696e 2072 6f6f   directly in roo
+0000f5d0: 7420 6f66 2074 6865 2054 6173 6b27 7320  t of the Task's 
+0000f5e0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+0000f5f0: 792e 0a0a 466f 7220 6578 616d 706c 653a  y...For example:
+0000f600: 0a0a 6060 6073 6865 6c6c 0a49 6620 7468  ..```shell.If th
+0000f610: 6520 7265 7175 6972 6564 206f 626a 6563  e required objec
+0000f620: 7420 6973 3a20 6465 7665 6c6f 706d 656e  t is: developmen
+0000f630: 743a 3a74 6573 7472 756e 5f32 3231 3130  t::testrun_22110
+0000f640: 382d 3132 3034 3034 2d37 6432 2f64 6576  8-120404-7d2/dev
+0000f650: 2f66 696c 655f 312e 7478 740a 0a74 6865  /file_1.txt..the
+0000f660: 6e2c 2069 6620 666c 6174 7465 6e49 6e70  n, if flattenInp
+0000f670: 7574 5061 7468 7320 6973 2066 616c 7365  utPaths is false
+0000f680: 2c20 7468 6520 6669 6c65 2077 696c 6c20  , the file will 
+0000f690: 6265 2066 6f75 6e64 2061 743a 0a20 2d3e  be found at:. ->
+0000f6a0: 203c 776f 726b 696e 675f 6469 7265 6374   <working_direct
+0000f6b0: 6f72 793e 2f74 6573 7472 756e 5f32 3231  ory>/testrun_221
+0000f6c0: 3130 382d 3132 3034 3034 2d37 6432 2f64  108-120404-7d2/d
+0000f6d0: 6576 2f66 696c 655f 312e 7478 740a 200a  ev/file_1.txt. .
+0000f6e0: 656c 7365 2c20 6966 2066 6c61 7474 656e  else, if flatten
+0000f6f0: 496e 7075 7450 6174 6873 2069 7320 7472  InputPaths is tr
+0000f700: 7565 2c20 7468 6520 6669 6c65 2077 696c  ue, the file wil
+0000f710: 6c20 6265 2066 6f75 6e64 2061 743a 0a20  l be found at:. 
+0000f720: 2d3e 203c 776f 726b 696e 675f 6469 7265  -> <working_dire
+0000f730: 6374 6f72 793e 2f66 696c 655f 312e 7478  ctory>/file_1.tx
+0000f740: 7420 0a20 0a77 6865 7265 203c 776f 726b  t . .where <work
+0000f750: 696e 675f 6469 7265 6374 6f72 793e 2069  ing_directory> i
+0000f760: 733a 0a20 202f 7661 722f 6f70 742f 7965  s:.  /var/opt/ye
+0000f770: 6c6c 6f77 646f 672f 7964 2d61 6765 6e74  llowdog/yd-agent
+0000f780: 2d34 2f64 6174 612f 776f 726b 6572 732f  -4/data/workers/
+0000f790: 312f 7964 6964 5f74 6173 6b5f 4430 4430  1/ydid_task_D0D0
+0000f7a0: 4430 5f36 3866 3565 3562 652d 6463 3933  D0_68f5e5be-dc93
+0000f7b0: 2d34 3965 622d 6138 3234 2d31 6663 6462  -49eb-a824-1fcdb
+0000f7c0: 3532 6639 3139 355f 315f 312f 0a60 6060  52f9195_1_1/.```
+0000f7d0: 0a0a 4e6f 7465 2074 6861 7420 576f 726b  ..Note that Work
+0000f7e0: 2052 6571 7569 7265 6d65 6e74 206e 616d   Requirement nam
+0000f7f0: 6520 2865 2e67 2e2c 2060 7465 7374 7275  e (e.g., `testru
+0000f800: 6e5f 3232 3131 3038 2d31 3230 3430 342d  n_221108-120404-
+0000f810: 3764 3260 2920 6973 2061 7661 696c 6162  7d2`) is availab
+0000f820: 6c65 2076 6961 2074 6865 2076 6172 6961  le via the varia
+0000f830: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
+0000f840: 2060 7772 5f6e 616d 6560 2c20 736f 2074   `wr_name`, so t
+0000f850: 6869 7320 636f 756c 6420 6265 2073 7570  his could be sup
+0000f860: 706c 6965 6420 746f 2074 6865 2054 6173  plied to the Tas
+0000f870: 6b20 746f 2068 656c 7020 6974 206c 6f63  k to help it loc
+0000f880: 6174 6520 6974 7320 646f 776e 6c6f 6164  ate its download
+0000f890: 6564 2066 696c 6573 2e20 466f 7220 6578  ed files. For ex
+0000f8a0: 616d 706c 652c 2069 6e20 7468 6520 6077  ample, in the `w
+0000f8b0: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
+0000f8c0: 7365 6374 696f 6e20 6f66 2074 6865 2060  section of the `
+0000f8d0: 636f 6e66 6967 2e74 6f6d 6c60 2066 696c  config.toml` fil
+0000f8e0: 652c 2049 2063 6f75 6c64 2073 7065 6369  e, I could speci
+0000f8f0: 6679 3a0a 0a60 6060 746f 6d6c 0a65 6e76  fy:..```toml.env
+0000f900: 6972 6f6e 6d65 6e74 203d 207b 5752 5f44  ironment = {WR_D
+0000f910: 4952 4543 544f 5259 203d 2022 7b7b 7772  IRECTORY = "{{wr
+0000f920: 5f6e 616d 657d 7d22 7d0a 6060 600a 0a54  _name}}"}.```..T
+0000f930: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+0000f940: 656e 7420 6e61 6d65 2077 6f75 6c64 2074  ent name would t
+0000f950: 6865 6e20 6265 2061 7661 696c 6162 6c65  hen be available
+0000f960: 2074 6f20 7468 6520 5461 736b 2069 6e20   to the Task in 
+0000f970: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+0000f980: 7661 7269 6162 6c65 2060 2457 525f 4449  variable `$WR_DI
+0000f990: 5245 4354 4f52 5960 2e0a 0a23 2323 2046  RECTORY`...### F
+0000f9a0: 696c 6573 2055 706c 6f61 6465 6420 6672  iles Uploaded fr
+0000f9b0: 6f6d 2061 204e 6f64 6520 746f 2074 6865  om a Node to the
+0000f9c0: 204f 626a 6563 7420 5374 6f72 6520 6166   Object Store af
+0000f9d0: 7465 7220 5461 736b 2045 7865 6375 7469  ter Task Executi
+0000f9e0: 6f6e 0a0a 4166 7465 7220 5461 736b 2063  on..After Task c
+0000f9f0: 6f6d 706c 6574 696f 6e2c 2074 6865 2041  ompletion, the A
+0000fa00: 6765 6e74 2077 696c 6c20 7570 6c6f 6164  gent will upload
+0000fa10: 2073 7065 6369 6669 6564 206f 7574 7075   specified outpu
+0000fa20: 7420 6669 6c65 7320 746f 2074 6865 204f  t files to the O
+0000fa30: 626a 6563 7420 5374 6f72 652e 2054 6865  bject Store. The
+0000fa40: 2066 696c 6573 2074 6f20 6265 2075 706c   files to be upl
+0000fa50: 6f61 6465 6420 6172 6520 7468 6f73 6520  oaded are those 
+0000fa60: 6c69 7374 6564 2069 6e20 7468 6520 606f  listed in the `o
+0000fa70: 7574 7075 7473 6020 616e 6420 606f 7574  utputs` and `out
+0000fa80: 7075 7473 5265 7175 6972 6564 6020 7072  putsRequired` pr
+0000fa90: 6f70 6572 7469 6573 2066 6f72 2074 6865  operties for the
+0000faa0: 2054 6173 6b2e 0a0a 496e 2061 6464 6974   Task...In addit
+0000fab0: 696f 6e2c 2074 6865 2063 6f6e 736f 6c65  ion, the console
+0000fac0: 206f 7574 7075 7420 6f66 2074 6865 2054   output of the T
+0000fad0: 6173 6b20 6973 2063 6170 7475 7265 6420  ask is captured 
+0000fae0: 696e 2061 2066 696c 6520 6361 6c6c 6564  in a file called
+0000faf0: 2060 7461 736b 6f75 7470 7574 2e74 7874   `taskoutput.txt
+0000fb00: 6020 696e 2074 6865 2072 6f6f 7420 6f66  ` in the root of
+0000fb10: 2074 6865 2054 6173 6b27 7320 776f 726b   the Task's work
+0000fb20: 696e 6720 6469 7265 6374 6f72 792e 2057  ing directory. W
+0000fb30: 6865 7468 6572 2074 6865 2060 7461 736b  hether the `task
+0000fb40: 6f75 7470 7574 2e74 7874 6020 6669 6c65  output.txt` file
+0000fb50: 2069 7320 7570 6c6f 6164 6564 2074 6f20   is uploaded to 
+0000fb60: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+0000fb70: 2069 7320 6465 7465 726d 696e 6564 2062   is determined b
+0000fb80: 7920 7468 6520 6063 6170 7475 7265 5461  y the `captureTa
+0000fb90: 736b 4f75 7470 7574 6020 7072 6f70 6572  skOutput` proper
+0000fba0: 7479 2066 6f72 2074 6865 2054 6173 6b2c  ty for the Task,
+0000fbb0: 2061 6e64 2074 6869 7320 6973 2073 6574   and this is set
+0000fbc0: 2074 6f20 2774 7275 6527 2062 7920 6465   to 'true' by de
+0000fbd0: 6661 756c 742e 0a0a 4966 2054 6173 6b20  fault...If Task 
+0000fbe0: 6f75 7470 7574 7320 6172 6520 6372 6561  outputs are crea
+0000fbf0: 7465 6420 696e 2073 7562 6469 7265 6374  ted in subdirect
+0000fc00: 6f72 6965 7320 6265 6c6f 7720 7468 6520  ories below the 
+0000fc10: 5461 736b 2773 2077 6f72 6b69 6e67 2064  Task's working d
+0000fc20: 6972 6563 746f 7279 2c20 696e 636c 7564  irectory, includ
+0000fc30: 6520 7468 6520 6469 7265 6374 6f72 6965  e the directorie
+0000fc40: 7320 666f 7220 6669 6c65 7320 696e 2074  s for files in t
+0000fc50: 6865 2060 6f75 7470 7574 7360 2070 726f  he `outputs` pro
+0000fc60: 7065 7274 792e 2045 2e67 2e2c 2069 6620  perty. E.g., if 
+0000fc70: 6120 5461 736b 2063 7265 6174 6573 2066  a Task creates f
+0000fc80: 696c 6573 2060 7265 7375 6c74 732f 6f70  iles `results/op
+0000fc90: 656e 666f 616d 2e74 6172 2e67 7a60 2061  enfoam.tar.gz` a
+0000fca0: 6e64 2060 7265 7375 6c74 732f 6f70 656e  nd `results/open
+0000fcb0: 666f 616d 2e6c 6f67 602c 2074 6865 6e20  foam.log`, then 
+0000fcc0: 7370 6563 6966 7920 7468 6573 6520 666f  specify these fo
+0000fcd0: 7220 7570 6c6f 6164 2069 6e20 7468 6520  r upload in the 
+0000fce0: 606f 7574 7075 7473 6020 7072 6f70 6572  `outputs` proper
+0000fcf0: 7479 2061 7320 666f 6c6c 6f77 733a 0a0a  ty as follows:..
+0000fd00: 6022 6f75 7470 7574 7322 3a20 5b22 7265  `"outputs": ["re
+0000fd10: 7375 6c74 732f 6f70 656e 666f 616d 2e74  sults/openfoam.t
+0000fd20: 6172 2e67 7a22 2c20 2272 6573 756c 7473  ar.gz", "results
+0000fd30: 2f6f 7065 6e66 6f61 6d2e 6c6f 6722 5d60  /openfoam.log"]`
+0000fd40: 0a0a 5768 656e 206f 7574 7075 7420 6669  ..When output fi
+0000fd50: 6c65 7320 6172 6520 7570 6c6f 6164 6564  les are uploaded
+0000fd60: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
+0000fd70: 746f 7265 2c20 7468 6579 2061 7265 2070  tore, they are p
+0000fd80: 6c61 6365 6420 696e 2061 2054 6173 6b20  laced in a Task 
+0000fd90: 4772 6f75 7020 616e 6420 5461 736b 2073  Group and Task s
+0000fda0: 7065 6369 6669 6320 6469 7265 6374 6f72  pecific director
+0000fdb0: 792e 2053 6f2c 2069 6620 7468 6520 4e61  y. So, if the Na
+0000fdc0: 6d65 7370 6163 6520 6973 2060 6465 7665  mespace is `deve
+0000fdd0: 6c6f 706d 656e 7460 2c20 7468 6520 576f  lopment`, the Wo
+0000fde0: 726b 2052 6571 7569 7265 6d65 6e74 2069  rk Requirement i
+0000fdf0: 7320 6074 6573 7472 756e 5f32 3231 3130  s `testrun_22110
+0000fe00: 382d 3132 3034 3034 2d37 6432 602c 2074  8-120404-7d2`, t
+0000fe10: 6865 2054 6173 6b20 4772 6f75 7020 6973  he Task Group is
+0000fe20: 2060 7461 736b 5f67 726f 7570 5f31 6020   `task_group_1` 
+0000fe30: 616e 6420 7468 6520 5461 736b 2069 7320  and the Task is 
+0000fe40: 6074 6173 6b5f 3160 2c20 7468 656e 2074  `task_1`, then t
+0000fe50: 6865 2066 696c 6573 2061 626f 7665 2077  he files above w
+0000fe60: 6f75 6c64 2062 6520 7570 6c6f 6164 6564  ould be uploaded
+0000fe70: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
+0000fe80: 746f 7265 2061 7320 666f 6c6c 6f77 733a  tore as follows:
+0000fe90: 0a0a 6060 6073 6865 6c6c 0a64 6576 656c  ..```shell.devel
+0000fea0: 6f70 6d65 6e74 3a3a 7465 7374 7275 6e5f  opment::testrun_
+0000feb0: 3232 3131 3038 2d31 3230 3430 342d 3764  221108-120404-7d
+0000fec0: 322f 7461 736b 5f67 726f 7570 5f31 2f74  2/task_group_1/t
+0000fed0: 6173 6b5f 312f 7265 7375 6c74 732f 6f70  ask_1/results/op
+0000fee0: 656e 666f 616d 2e74 6172 2e67 7a0a 6465  enfoam.tar.gz.de
+0000fef0: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
+0000ff00: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000ff10: 2d37 6432 2f74 6173 6b5f 6772 6f75 705f  -7d2/task_group_
+0000ff20: 312f 7461 736b 5f31 2f72 6573 756c 7473  1/task_1/results
+0000ff30: 2f6f 7065 6e66 6f61 6d2e 6c6f 670a 6465  /openfoam.log.de
+0000ff40: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
+0000ff50: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000ff60: 2d37 6432 2f74 6173 6b5f 6772 6f75 705f  -7d2/task_group_
+0000ff70: 312f 7461 736b 5f31 2f74 6173 6b6f 7574  1/task_1/taskout
+0000ff80: 7075 742e 7478 740a 6060 600a 0a54 6865  put.txt.```..The
+0000ff90: 202a 2a60 6f75 7470 7574 7352 6571 7569   **`outputsRequi
+0000ffa0: 7265 6460 2a2a 2070 726f 7065 7274 7920  red`** property 
+0000ffb0: 6361 6e20 6265 2075 7365 6420 696e 7374  can be used inst
+0000ffc0: 6561 6420 6f66 2028 6f72 2069 6e20 6164  ead of (or in ad
+0000ffd0: 6469 7469 6f6e 2074 6f29 2074 6865 2060  dition to) the `
+0000ffe0: 6f75 7470 7574 7360 2070 726f 7065 7274  outputs` propert
+0000fff0: 792c 2069 6620 7468 6520 6f75 7470 7574  y, if the output
+00010000: 2066 696c 6528 7329 202a 2a6d 7573 742a   file(s) **must*
+00010010: 2a20 6265 2061 7661 696c 6162 6c65 2066  * be available f
+00010020: 6f72 2075 706c 6f61 6420 746f 2074 6865  or upload to the
+00010030: 204f 626a 6563 7420 5374 6f72 6520 6174   Object Store at
+00010040: 2074 6865 2063 6f6e 636c 7573 696f 6e20   the conclusion 
+00010050: 6f66 2074 6865 2054 6173 6b20 6f72 2074  of the Task or t
+00010060: 6865 2054 6173 6b20 7769 6c6c 2062 6520  he Task will be 
+00010070: 6d61 726b 6564 2061 7320 6046 6169 6c65  marked as `Faile
+00010080: 6460 2c20 652e 672e 3a0a 0a60 226f 7574  d`, e.g.:..`"out
+00010090: 7075 7473 5265 7175 6972 6564 223a 205b  putsRequired": [
+000100a0: 2272 6573 756c 7473 2f70 726f 6365 7373  "results/process
+000100b0: 5f6f 7574 7075 742e 7478 7422 5d60 0a0a  _output.txt"]`..
+000100c0: 2323 2320 4669 6c65 7320 446f 776e 6c6f  ### Files Downlo
+000100d0: 6164 6564 2066 726f 6d20 7468 6520 4f62  aded from the Ob
+000100e0: 6a65 6374 2053 746f 7265 2074 6f20 4c6f  ject Store to Lo
+000100f0: 6361 6c20 5374 6f72 6167 650a 0a54 6865  cal Storage..The
+00010100: 2060 7964 2d64 6f77 6e6c 6f61 6460 2063   `yd-download` c
+00010110: 6f6d 6d61 6e64 2077 696c 6c20 646f 776e  ommand will down
+00010120: 6c6f 6164 2061 6c6c 206f 626a 6563 7473  load all objects
+00010130: 2066 726f 6d20 7468 6520 4f62 6a65 6374   from the Object
+00010140: 2053 746f 7265 2074 6f20 6120 6c6f 6361   Store to a loca
+00010150: 6c20 6469 7265 6374 6f72 792c 206f 6e20  l directory, on 
+00010160: 6120 7065 7220 576f 726b 2052 6571 7569  a per Work Requi
+00010170: 7265 6d65 6e74 2062 6173 6973 2028 696e  rement basis (in
+00010180: 636c 7564 696e 6720 616e 7920 6669 6c65  cluding any file
+00010190: 7320 7468 6174 2068 6176 6520 6265 656e  s that have been
+000101a0: 2075 706c 6f61 6465 6429 2e20 4120 6c6f   uploaded). A lo
+000101b0: 6361 6c20 6469 7265 6374 6f72 7920 6973  cal directory is
+000101c0: 2063 7265 6174 6564 2077 6974 6820 7468   created with th
+000101d0: 6520 7361 6d65 206e 616d 6520 6173 2074  e same name as t
+000101e0: 6865 204e 616d 6573 7061 6365 2061 6e64  he Namespace and
+000101f0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00010200: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00010210: 2064 6972 6563 746f 7269 6573 2e0a 0a55   directories...U
+00010220: 7365 2074 6865 2060 2d2d 696e 7465 7261  se the `--intera
+00010230: 6374 6976 6560 206f 7074 696f 6e20 7769  ctive` option wi
+00010240: 7468 2060 7964 2d64 6f77 6e6c 6f61 6460  th `yd-download`
+00010250: 2074 6f20 7365 6c65 6374 2077 6869 6368   to select which
+00010260: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00010270: 7428 7329 2074 6f20 646f 776e 6c6f 6164  t(s) to download
+00010280: 2e0a 0a46 6f72 2074 6865 2065 7861 6d70  ...For the examp
+00010290: 6c65 2061 626f 7665 2c20 6079 642d 646f  le above, `yd-do
+000102a0: 776e 6c6f 6164 6020 776f 756c 6420 6372  wnload` would cr
+000102b0: 6561 7465 2061 2064 6972 6563 746f 7279  eate a directory
+000102c0: 2063 616c 6c65 6420 6064 6576 656c 6f70   called `develop
+000102d0: 6d65 6e74 6020 696e 2074 6865 2063 7572  ment` in the cur
+000102e0: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
+000102f0: 6563 746f 7279 2c20 636f 6e74 6169 6e69  ectory, containi
+00010300: 6e67 2073 6f6d 6574 6869 6e67 206c 696b  ng something lik
+00010310: 653a 0a0a 6060 6073 6865 6c6c 0a64 6576  e:..```shell.dev
+00010320: 656c 6f70 6d65 6e74 0ae2 9494 e294 80e2  elopment........
+00010330: 9480 2074 6573 7472 756e 5f32 3231 3130  .. testrun_22110
+00010340: 382d 3132 3034 3034 2d37 6432 0a20 2020  8-120404-7d2.   
+00010350: 20e2 949c e294 80e2 9480 2062 6173 685f   ......... bash_
+00010360: 7363 7269 7074 2e73 680a 2020 2020 e294  script.sh.    ..
+00010370: 9ce2 9480 e294 8020 6669 6c65 5f31 2e74  ....... file_1.t
+00010380: 7874 0a20 2020 20e2 9494 e294 80e2 9480  xt.    .........
+00010390: 2074 6173 6b5f 6772 6f75 705f 310a 2020   task_group_1.  
+000103a0: 2020 2020 2020 e294 94e2 9480 e294 8020        ......... 
+000103b0: 7461 736b 5f31 0a20 2020 2020 2020 2020  task_1.         
+000103c0: 2020 20e2 949c e294 80e2 9480 2072 6573     ......... res
+000103d0: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
+000103e0: 20e2 9482 c2a0 c2a0 20e2 949c e294 80e2   ....... .......
+000103f0: 9480 206f 7065 6e66 6f61 6d2e 6c6f 670a  .. openfoam.log.
+00010400: 2020 2020 2020 2020 2020 2020 e294 82c2              ....
+00010410: a0c2 a020 e294 94e2 9480 e294 8020 6f70  ... ......... op
+00010420: 656e 666f 616d 2e74 6172 2e67 7a0a 2020  enfoam.tar.gz.  
+00010430: 2020 2020 2020 2020 2020 e294 94e2 9480            ......
+00010440: e294 8020 7461 736b 6f75 7470 7574 2e74  ... taskoutput.t
+00010450: 7874 0a60 6060 0a0a 4e6f 7465 2074 6861  xt.```..Note tha
+00010460: 7420 6576 6572 7974 6869 6e67 2077 6974  t everything wit
+00010470: 6869 6e20 7468 6520 606e 616d 6573 7061  hin the `namespa
+00010480: 6365 3a3a 776f 726b 2d72 6571 7569 7265  ce::work-require
+00010490: 6d65 6e74 6020 6469 7265 6374 6f72 7920  ment` directory 
+000104a0: 696e 2074 6865 204f 626a 6563 7420 5374  in the Object St
+000104b0: 6f72 6520 6973 2064 6f77 6e6c 6f61 6465  ore is downloade
+000104c0: 642c 2069 6e63 6c75 6469 6e67 2061 6e79  d, including any
+000104d0: 2066 696c 6573 2074 6861 7420 7765 7265   files that were
+000104e0: 2073 7065 6369 6669 6564 2069 6e20 6069   specified in `i
+000104f0: 6e70 7574 7360 2061 6e64 2075 706c 6f61  nputs` and uploa
+00010500: 6465 6420 6173 2070 6172 7420 6f66 2074  ded as part of t
+00010510: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+00010520: 656e 7420 7375 626d 6973 7369 6f6e 2e20  ent submission. 
+00010530: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
+00010540: 6f75 7073 2c20 616e 6420 6d75 6c74 6970  oups, and multip
+00010550: 6c65 2054 6173 6b73 2077 696c 6c20 616c  le Tasks will al
+00010560: 6c20 6170 7065 6172 2069 6e20 7468 6520  l appear in the 
+00010570: 6469 7265 6374 6f72 7920 7374 7275 6374  directory struct
+00010580: 7572 652e 0a0a 4966 2074 6865 2060 6465  ure...If the `de
+00010590: 7665 6c6f 706d 656e 7460 2064 6972 6563  velopment` direc
+000105a0: 746f 7279 2061 6c72 6561 6479 2065 7869  tory already exi
+000105b0: 7374 732c 2060 7964 2d64 6f77 6e6c 6f61  sts, `yd-downloa
+000105c0: 6460 2077 696c 6c20 7472 7920 6064 6576  d` will try `dev
+000105d0: 656c 6f70 6d65 6e74 2e30 3160 2c20 6574  elopment.01`, et
+000105e0: 632e 2c20 746f 2061 766f 6964 206f 7665  c., to avoid ove
+000105f0: 7277 7269 7469 6e67 2070 7265 7669 6f75  rwriting previou
+00010600: 7320 646f 776e 6c6f 6164 732e 0a0a 2323  s downloads...##
+00010610: 2054 6173 6b20 4578 6563 7574 696f 6e20   Task Execution 
+00010620: 436f 6e74 6578 740a 0a54 6869 7320 7365  Context..This se
+00010630: 6374 696f 6e20 6469 7363 7573 7365 7320  ction discusses 
+00010640: 7468 6520 636f 6e74 6578 7420 7769 7468  the context with
+00010650: 696e 2077 6869 6368 2061 2054 6173 6b20  in which a Task 
+00010660: 6f70 6572 6174 6573 2077 6865 6e20 6974  operates when it
+00010670: 2773 2065 7865 6375 7465 6420 6279 2061  's executed by a
+00010680: 2057 6f72 6b65 7220 6f6e 2061 206e 6f64   Worker on a nod
+00010690: 652e 2049 7420 6170 706c 6965 7320 7370  e. It applies sp
+000106a0: 6563 6966 6963 616c 6c79 2074 6f20 7468  ecifically to th
+000106b0: 6520 5965 6c6c 6f77 446f 6720 4167 656e  e YellowDog Agen
+000106c0: 7420 7275 6e6e 696e 6720 6f6e 2061 204c  t running on a L
+000106d0: 696e 7578 206e 6f64 652c 2061 6e64 2063  inux node, and c
+000106e0: 6f6e 6669 6775 7265 6420 7573 696e 6720  onfigured using 
+000106f0: 7468 6520 6465 6661 756c 7420 7573 6572  the default user
+00010700: 6e61 6d65 2c20 6469 7265 6374 6f72 6965  name, directorie
+00010710: 732c 2065 7463 2e20 436f 6e66 6967 7572  s, etc. Configur
+00010720: 6174 696f 6e73 2063 616e 2076 6172 792e  ations can vary.
+00010730: 0a0a 2323 2320 5461 736b 2045 7865 6375  ..### Task Execu
+00010740: 7469 6f6e 2053 7465 7073 0a0a 5768 656e  tion Steps..When
+00010750: 2061 2054 6173 6b20 6973 2061 6c6c 6f63   a Task is alloc
+00010760: 6174 6564 2074 6f20 6120 576f 726b 6572  ated to a Worker
+00010770: 206f 6e20 6120 6e6f 6465 2062 7920 7468   on a node by th
+00010780: 6520 5965 6c6c 6f77 446f 6720 5363 6865  e YellowDog Sche
+00010790: 6475 6c65 722c 2074 6865 2066 6f6c 6c6f  duler, the follo
+000107a0: 7769 6e67 2073 7465 7073 2061 7265 2066  wing steps are f
+000107b0: 6f6c 6c6f 7765 643a 0a0a 312e 2054 6865  ollowed:..1. The
+000107c0: 2041 6765 6e74 2072 756e 6e69 6e67 206f   Agent running o
+000107d0: 6e20 7468 6520 6e6f 6465 2064 6f77 6e6c  n the node downl
+000107e0: 6f61 6473 2074 6865 2054 6173 6b27 7320  oads the Task's 
+000107f0: 7072 6f70 6572 7469 6573 3a20 6974 7320  properties: its 
+00010800: 6074 6173 6b54 7970 6560 2c20 2060 6172  `taskType`,  `ar
+00010810: 6775 6d65 6e74 7360 2c20 6065 6e76 6972  guments`, `envir
+00010820: 6f6e 6d65 6e74 602c 2060 7461 736b 6461  onment`, `taskda
+00010830: 7461 602c 2061 6e64 2028 6672 6f6d 2074  ta`, and (from t
+00010840: 6865 204f 626a 6563 7420 5374 6f72 6529  he Object Store)
+00010850: 2061 6e79 2066 696c 6573 2069 6e20 7468   any files in th
+00010860: 6520 6069 6e70 7574 7360 206c 6973 7420  e `inputs` list 
+00010870: 616e 6420 616e 7920 6176 6169 6c61 626c  and any availabl
+00010880: 6520 6669 6c65 7320 696e 2074 6865 2060  e files in the `
+00010890: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
+000108a0: 6c69 7374 2e0a 322e 2054 6865 7365 2066  list..2. These f
+000108b0: 696c 6573 2061 7265 2070 6c61 6365 6420  iles are placed 
+000108c0: 696e 2061 6e20 6570 6865 6d65 7261 6c20  in an ephemeral 
+000108d0: 6469 7265 6374 6f72 7920 6372 6561 7465  directory create
+000108e0: 6420 666f 7220 7468 6973 2054 6173 6b27  d for this Task'
+000108f0: 7320 6578 6563 7574 696f 6e2c 2061 6e64  s execution, and
+00010900: 2069 6e74 6f20 7768 6963 6820 616e 7920   into which any 
+00010910: 6f75 7470 7574 2066 696c 6573 2061 7265  output files are
+00010920: 2061 6c73 6f20 706c 6163 6564 2062 7920   also placed by 
+00010930: 6465 6661 756c 742e 0a32 2e20 5468 6520  default..2. The 
+00010940: 4167 656e 7420 7275 6e73 2074 6865 2063  Agent runs the c
+00010950: 6f6d 6d61 6e64 2073 7065 6369 6669 6564  ommand specified
+00010960: 2066 6f72 2074 6865 2060 7461 736b 5479   for the `taskTy
+00010970: 7065 6020 696e 2074 6865 2041 6765 6e74  pe` in the Agent
+00010980: 2773 2060 6170 706c 6963 6174 696f 6e2e  's `application.
+00010990: 7961 6d6c 6020 636f 6e66 6967 7572 6174  yaml` configurat
+000109a0: 696f 6e20 6669 6c65 2e20 5468 6973 2064  ion file. This d
+000109b0: 6f6e 6520 6173 2061 2073 696d 706c 6520  one as a simple 
+000109c0: 6065 7865 6360 206f 6620 6120 7375 6270  `exec` of a subp
+000109d0: 726f 6365 7373 2e0a 332e 2057 6865 6e20  rocess..3. When 
+000109e0: 7468 6520 5461 736b 2063 6f6e 636c 7564  the Task conclud
+000109f0: 6573 2c20 7468 6520 4167 656e 7420 7573  es, the Agent us
+00010a00: 6573 2074 6865 2065 7869 7420 636f 6465  es the exit code
+00010a10: 206f 6620 7468 6520 7375 6270 726f 6365   of the subproce
+00010a20: 7373 2074 6f20 7265 706f 7274 2073 7563  ss to report suc
+00010a30: 6365 7373 2028 7a65 726f 2920 6f72 2066  cess (zero) or f
+00010a40: 6169 6c75 7265 2028 6e6f 6e2d 7a65 726f  ailure (non-zero
+00010a50: 292e 0a34 2e20 5468 6520 4167 656e 7420  )..4. The Agent 
+00010a60: 7468 656e 2067 6174 6865 7273 2061 6e79  then gathers any
+00010a70: 2066 696c 6573 2069 6e20 7468 6520 606f   files in the `o
+00010a80: 7574 7075 7473 6020 616e 6420 606f 7574  utputs` and `out
+00010a90: 7075 7473 5265 7175 6972 6564 6020 6c69  putsRequired` li
+00010aa0: 7374 7320 616e 6420 7570 6c6f 6164 7320  sts and uploads 
+00010ab0: 7468 656d 2074 6f20 7468 6520 4f62 6a65  them to the Obje
+00010ac0: 6374 2053 746f 7265 2e20 4966 2061 2066  ct Store. If a f
+00010ad0: 696c 6520 696e 2074 6865 2060 6f75 7470  ile in the `outp
+00010ae0: 7574 7352 6571 7569 7265 6460 206c 6973  utsRequired` lis
+00010af0: 7420 6973 206e 6f74 2066 6f75 6e64 2c20  t is not found, 
+00010b00: 7468 6520 5461 736b 2077 696c 6c20 6265  the Task will be
+00010b10: 2072 6570 6f72 7465 6420 6173 2066 6169   reported as fai
+00010b20: 6c65 642e 2054 6865 2041 6765 6e74 2077  led. The Agent w
+00010b30: 696c 6c20 616c 736f 206f 7074 696f 6e61  ill also optiona
+00010b40: 6c6c 7920 7570 6c6f 6164 2074 6865 2063  lly upload the c
+00010b50: 6f6e 736f 6c65 206f 7574 7075 7420 2869  onsole output (i
+00010b60: 6e63 6c75 6469 6e67 2062 6f74 6820 6073  ncluding both `s
+00010b70: 7464 6f75 7460 2061 6e64 2060 7374 6465  tdout` and `stde
+00010b80: 7272 6029 206f 6620 7468 6520 5461 736b  rr`) of the Task
+00010b90: 2c20 636f 6e74 6169 6e65 6420 696e 2074  , contained in t
+00010ba0: 6865 2060 7461 736b 6f75 7470 7574 2e74  he `taskoutput.t
+00010bb0: 7874 6020 6669 6c65 2e0a 352e 2054 6865  xt` file..5. The
+00010bc0: 2065 7068 656d 6572 616c 2054 6173 6b20   ephemeral Task 
+00010bd0: 6469 7265 6374 6f72 7920 6973 2074 6865  directory is the
+00010be0: 6e20 6465 6c65 7465 642e 0a0a 4e6f 7465  n deleted...Note
+00010bf0: 2074 6861 7420 6966 2061 2054 6173 6b20   that if a Task 
+00010c00: 6973 2061 626f 7274 6564 2064 7572 696e  is aborted durin
+00010c10: 6720 6578 6563 7574 696f 6e2c 2074 6865  g execution, the
+00010c20: 2054 6173 6b27 7320 7375 6270 726f 6365   Task's subproce
+00010c30: 7373 2069 7320 7365 6e74 2061 2060 5349  ss is sent a `SI
+00010c40: 4749 4e54 602c 2061 6c6c 6f77 696e 6720  GINT`, allowing 
+00010c50: 7468 6520 5461 736b 2061 6e20 6f70 706f  the Task an oppo
+00010c60: 7274 756e 6974 7920 746f 2074 6572 6d69  rtunity to termi
+00010c70: 6e61 7465 2061 6e79 2063 6869 6c64 2070  nate any child p
+00010c80: 726f 6365 7373 6573 206f 7220 6f74 6865  rocesses or othe
+00010c90: 7220 7265 736f 7572 6365 7320 2865 2e67  r resources (e.g
+00010ca0: 2e2c 2063 6f6e 7461 696e 6572 7329 2074  ., containers) t
+00010cb0: 6861 7420 6d61 7920 6861 7665 2062 6565  hat may have bee
+00010cc0: 6e20 7374 6172 7465 6420 6173 2070 6172  n started as par
+00010cd0: 7420 6f66 2054 6173 6b20 6578 6563 7574  t of Task execut
+00010ce0: 696f 6e2e 0a0a 4f6e 6365 2074 6865 2073  ion...Once the s
+00010cf0: 7465 7073 2061 626f 7665 2068 6176 6520  teps above have 
+00010d00: 6265 656e 2063 6f6d 706c 6574 6564 2c20  been completed, 
+00010d10: 7468 6520 576f 726b 6572 2069 7320 7265  the Worker is re
+00010d20: 6164 7920 746f 2061 6363 6570 7420 6974  ady to accept it
+00010d30: 7320 6e65 7874 2054 6173 6b20 6672 6f6d  s next Task from
+00010d40: 2074 6865 2059 656c 6c6f 7744 6f67 2073   the YellowDog s
+00010d50: 6368 6564 756c 6572 2e0a 0a4e 6f74 6520  cheduler...Note 
+00010d60: 7468 6174 2069 6620 7468 6520 4167 656e  that if the Agen
+00010d70: 7420 6f6e 2061 206e 6f64 6520 6861 7320  t on a node has 
+00010d80: 6d75 6c74 6970 6c65 2057 6f72 6b65 7273  multiple Workers
+00010d90: 2c20 7468 656e 2054 6173 6b73 2061 7265  , then Tasks are
+00010da0: 2065 7865 6375 7465 6420 696e 2070 6172   executed in par
+00010db0: 616c 6c65 6c20 6f6e 2074 6865 206e 6f64  allel on the nod
+00010dc0: 6520 616e 6420 6361 6e20 7374 6172 7420  e and can start 
+00010dd0: 616e 6420 7374 6f70 2069 6e64 6570 656e  and stop indepen
+00010de0: 6465 6e74 6c79 2e0a 0a23 2323 2054 6865  dently...### The
+00010df0: 2055 7365 7220 616e 6420 4772 6f75 7020   User and Group 
+00010e00: 7573 6564 2066 6f72 2054 6173 6b73 0a0a  used for Tasks..
+00010e10: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
+00010e20: 4167 656e 7420 7275 6e73 2061 7320 7573  Agent runs as us
+00010e30: 6572 2061 6e64 2067 726f 7570 2060 7964  er and group `yd
+00010e40: 2d61 6765 6e74 602c 2061 6e64 2068 656e  -agent`, and hen
+00010e50: 6365 2054 6173 6b73 2061 6c73 6f20 6578  ce Tasks also ex
+00010e60: 6563 7574 6520 756e 6465 7220 7468 6973  ecute under this
+00010e70: 2075 7365 722e 0a0a 6079 642d 6167 656e   user...`yd-agen
+00010e80: 7460 2064 6f65 7320 6e6f 7420 6861 7665  t` does not have
+00010e90: 2060 7375 646f 6020 7072 6976 696c 6567   `sudo` privileg
+00010ea0: 6573 2061 7320 7374 616e 6461 7264 2c20  es as standard, 
+00010eb0: 6275 7420 7468 6973 2063 616e 2062 6520  but this can be 
+00010ec0: 6164 6465 6420 6966 2072 6571 7569 7265  added if require
+00010ed0: 6420 6174 2069 6e73 7461 6e63 6520 626f  d at instance bo
+00010ee0: 6f74 2074 696d 6520 7669 6120 7468 6520  ot time via the 
+00010ef0: 6075 7365 7244 6174 6160 2070 726f 7065  `userData` prope
+00010f00: 7274 7920 6f66 2061 2070 726f 7669 7369  rty of a provisi
+00010f10: 6f6e 696e 6720 7265 7175 6573 742e 2045  oning request. E
+00010f20: 2e67 2e20 2866 6f72 2055 6275 6e74 7529  .g. (for Ubuntu)
+00010f30: 3a0a 0a60 6060 7368 656c 6c0a 7573 6572  :..```shell.user
+00010f40: 6d6f 6420 2d61 4720 7768 6565 6c20 7964  mod -aG wheel yd
+00010f50: 2d61 6765 6e74 0a65 6368 6f20 2d65 2022  -agent.echo -e "
+00010f60: 7964 2d61 6765 6e74 5c74 414c 4c3d 2841  yd-agent\tALL=(A
+00010f70: 4c4c 295c 744e 4f50 4153 5357 443a 2041  LL)\tNOPASSWD: A
+00010f80: 4c4c 2220 3e20 2f65 7463 2f73 7564 6f65  LL" > /etc/sudoe
+00010f90: 7273 2e64 2f30 3230 2d79 642d 6167 656e  rs.d/020-yd-agen
+00010fa0: 740a 6060 600a 0a23 2323 2048 6f6d 6520  t.```..### Home 
+00010fb0: 4469 7265 6374 6f72 7920 666f 7220 6079  Directory for `y
+00010fc0: 642d 6167 656e 7460 0a0a 4279 2064 6566  d-agent`..By def
+00010fd0: 6175 6c74 2c20 7468 6520 686f 6d65 2064  ault, the home d
+00010fe0: 6972 6563 746f 7279 206f 6620 7468 6520  irectory of the 
+00010ff0: 6079 642d 6167 656e 7460 2075 7365 7220  `yd-agent` user 
+00011000: 6973 2060 2f6f 7074 2f79 656c 6c6f 7764  is `/opt/yellowd
+00011010: 6f67 2f61 6765 6e74 602e 2054 6869 7320  og/agent`. This 
+00011020: 6469 7265 6374 6f72 7920 7479 7069 6361  directory typica
+00011030: 6c6c 7920 636f 6e74 6169 6e73 2074 6865  lly contains the
+00011040: 2060 6170 706c 6963 6174 696f 6e2e 7961   `application.ya
+00011050: 6d6c 6020 6669 6c65 2075 7365 6420 746f  ml` file used to
+00011060: 2063 6f6e 6669 6775 7265 2074 6865 2041   configure the A
+00011070: 6765 6e74 2c20 6173 2077 656c 6c20 6173  gent, as well as
+00011080: 2061 6e79 2073 6372 6970 7473 2074 6861   any scripts tha
+00011090: 7420 6172 6520 7573 6564 2074 6f20 6578  t are used to ex
+000110a0: 6563 7574 6520 7468 6520 5461 736b 2054  ecute the Task T
+000110b0: 7970 6573 2074 6861 7420 7468 6520 6e6f  ypes that the no
+000110c0: 6465 2073 7570 706f 7274 732e 0a0a 4966  de supports...If
+000110d0: 206f 6e65 2077 616e 7473 2074 6f20 5353   one wants to SS
+000110e0: 4820 746f 2061 6e20 696e 7374 616e 6365  H to an instance
+000110f0: 2061 7320 7573 6572 2060 7964 2d61 6765   as user `yd-age
+00011100: 6e74 602c 2070 6572 6861 7073 2066 6f72  nt`, perhaps for
+00011110: 2064 6562 7567 6769 6e67 2070 7572 706f   debugging purpo
+00011120: 7365 732c 2053 5348 206b 6579 7320 6361  ses, SSH keys ca
+00011130: 6e20 6265 2069 6e73 6572 7465 6420 7669  n be inserted vi
+00011140: 6120 696e 7374 616e 6365 2060 7573 6572  a instance `user
+00011150: 4461 7461 602c 2065 2e67 2e3a 0a0a 6060  Data`, e.g.:..``
+00011160: 6073 6865 6c6c 0a59 4441 5f48 4f4d 453d  `shell.YDA_HOME=
+00011170: 2f6f 7074 2f79 656c 6c6f 7764 6f67 2f61  /opt/yellowdog/a
+00011180: 6765 6e74 0a6d 6b64 6972 202d 7020 2459  gent.mkdir -p $Y
+00011190: 4441 5f48 4f4d 452f 2e73 7368 0a63 686d  DA_HOME/.ssh.chm
+000111a0: 6f64 206f 672d 7277 7820 2459 4441 5f48  od og-rwx $YDA_H
+000111b0: 4f4d 452f 2e73 7368 0a63 6174 203e 3e20  OME/.ssh.cat >> 
+000111c0: 2459 4441 5f48 4f4d 452f 2e73 7368 2f61  $YDA_HOME/.ssh/a
+000111d0: 7574 686f 7269 7a65 645f 6b65 7973 203c  uthorized_keys <
+000111e0: 3c20 454f 460a 3c3c 496e 7365 7274 5f50  < EOF.<<Insert_P
+000111f0: 7562 6c69 635f 6b65 795f 4865 7265 3e3e  ublic_key_Here>>
+00011200: 0a45 4f46 0a63 686d 6f64 206f 672d 7277  .EOF.chmod og-rw
+00011210: 2024 5944 415f 484f 4d45 2f2e 7373 682f   $YDA_HOME/.ssh/
+00011220: 6175 7468 6f72 697a 6564 5f6b 6579 730a  authorized_keys.
+00011230: 6368 6f77 6e20 2d52 2079 642d 6167 656e  chown -R yd-agen
+00011240: 743a 7964 2d61 6765 6e74 2024 5944 415f  t:yd-agent $YDA_
+00011250: 484f 4d45 2f2e 7373 680a 6060 600a 0a23  HOME/.ssh.```..#
+00011260: 2323 2054 6173 6b20 4578 6563 7574 696f  ## Task Executio
+00011270: 6e20 4469 7265 6374 6f72 790a 0a45 7068  n Directory..Eph
+00011280: 656d 6572 616c 2054 6173 6b20 6469 7265  emeral Task dire
+00011290: 6374 6f72 6965 7320 6172 6520 6279 2064  ctories are by d
+000112a0: 6566 6175 6c74 2063 7265 6174 6564 2075  efault created u
+000112b0: 6e64 6572 2060 2f76 6172 2f6f 7074 2f79  nder `/var/opt/y
+000112c0: 656c 6c6f 7764 6f67 2f61 6765 6e74 2f64  ellowdog/agent/d
+000112d0: 6174 612f 776f 726b 6572 7360 2e20 5468  ata/workers`. Th
+000112e0: 6973 2064 6972 6563 746f 7279 2063 6f6e  is directory con
+000112f0: 7461 696e 7320 6f6e 6520 6f72 206d 6f72  tains one or mor
+00011300: 6520 6e75 6d62 6572 6564 2073 7562 6469  e numbered subdi
+00011310: 7265 6374 6f72 6965 7320 7768 6572 6520  rectories where 
+00011320: 6561 6368 206e 756d 6265 7265 6420 6469  each numbered di
+00011330: 7265 6374 6f72 7920 636f 7272 6573 706f  rectory correspo
+00011340: 6e64 7320 746f 2061 2057 6f72 6b65 7220  nds to a Worker 
+00011350: 6f6e 2074 6865 206e 6f64 652e 0a0a 284f  on the node...(O
+00011360: 6e20 5769 6e64 6f77 7320 686f 7374 732c  n Windows hosts,
+00011370: 2074 6865 2054 6173 6b20 6469 7265 6374   the Task direct
+00011380: 6f72 6965 7320 6172 6520 666f 756e 6420  ories are found 
+00011390: 756e 6465 7220 6025 4170 7044 6174 6125  under `%AppData%
+000113a0: 5c79 656c 6c6f 7764 6f67 5c61 6765 6e74  \yellowdog\agent
+000113b0: 5c64 6174 615c 776f 726b 6572 7360 2e29  \data\workers`.)
+000113c0: 0a0a 5768 656e 2061 2054 6173 6b20 6973  ..When a Task is
+000113d0: 2061 6c6c 6f63 6174 6564 2074 6f20 6120   allocated to a 
+000113e0: 6e6f 6465 2c20 616e 2065 7068 656d 6572  node, an ephemer
+000113f0: 616c 2064 6972 6563 746f 7279 2069 7320  al directory is 
+00011400: 6372 6561 7465 6420 756e 6465 7220 7468  created under th
+00011410: 6520 6170 706c 6963 6162 6c65 2057 6f72  e applicable Wor
+00011420: 6b65 7220 6469 7265 6374 6f72 792c 2077  ker directory, w
+00011430: 6974 6820 6120 6e61 6d65 2063 6f72 7265  ith a name corre
+00011440: 7370 6f6e 6469 6e67 2074 6865 2059 656c  sponding the Yel
+00011450: 6c6f 7744 6f67 2049 4420 666f 7220 7468  lowDog ID for th
+00011460: 6520 5461 736b 2e20 466f 7220 6578 616d  e Task. For exam
+00011470: 706c 652c 2074 6869 7320 6973 2061 6e20  ple, this is an 
+00011480: 6570 6865 6d65 7261 6c20 6469 7265 6374  ephemeral direct
+00011490: 6f72 7920 6265 696e 6720 7573 6564 2062  ory being used b
+000114a0: 7920 576f 726b 6572 206e 756d 6265 7220  y Worker number 
+000114b0: 6031 603a 0a0a 602f 7661 722f 6f70 742f  `1`:..`/var/opt/
+000114c0: 7965 6c6c 6f77 646f 672f 6167 656e 742f  yellowdog/agent/
+000114d0: 6461 7461 2f77 6f72 6b65 7273 2f31 2f79  data/workers/1/y
+000114e0: 6469 645f 7461 736b 5f35 3539 4542 455f  did_task_559EBE_
+000114f0: 3734 3934 3933 3336 2d61 6332 622d 3438  74949336-ac2b-48
+00011500: 3131 2d61 3764 352d 6633 6563 6439 3733  11-a7d5-f3ecd973
+00011510: 3939 3038 5f31 5f31 600a 0a54 6869 7320  9908_1_1`..This 
+00011520: 6973 2074 6865 2064 6972 6563 746f 7279  is the directory
+00011530: 2069 6e74 6f20 7768 6963 6820 646f 776e   into which down
+00011540: 6c6f 6164 6564 206f 626a 6563 7473 2061  loaded objects a
+00011550: 7265 2070 6c61 6365 642c 2061 6e64 2069  re placed, and i
+00011560: 6e20 7768 6963 6820 6f75 7470 7574 2066  n which output f
+00011570: 696c 6573 2061 7265 2063 7265 6174 6564  iles are created
+00011580: 2062 7920 6465 6661 756c 742e 2054 6865   by default. The
+00011590: 2063 6f6e 736f 6c65 206f 7574 7075 7420   console output 
+000115a0: 6074 6173 6b6f 7574 7075 742e 7478 7460  `taskoutput.txt`
+000115b0: 2066 696c 6520 7769 6c6c 2061 6c73 6f20   file will also 
+000115c0: 6265 2063 7265 6174 6564 2069 6e20 7468  be created in th
+000115d0: 6973 2064 6972 6563 746f 7279 2e0a 0a53  is directory...S
+000115e0: 6565 2074 6865 205b 4669 6c65 7320 446f  ee the [Files Do
+000115f0: 776e 6c6f 6164 6564 2074 6f20 6120 4e6f  wnloaded to a No
+00011600: 6465 5d28 2366 696c 6573 2d64 6f77 6e6c  de](#files-downl
+00011610: 6f61 6465 642d 746f 2d61 2d6e 6f64 652d  oaded-to-a-node-
+00011620: 666f 722d 7573 652d 696e 2d74 6173 6b2d  for-use-in-task-
+00011630: 6578 6563 7574 696f 6e29 2073 6563 7469  execution) secti
+00011640: 6f6e 2061 626f 7665 2066 6f72 206d 6f72  on above for mor
+00011650: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
+00011660: 2066 696c 6573 2069 6e20 7468 6973 2064   files in this d
+00011670: 6972 6563 746f 7279 2061 7265 2068 616e  irectory are han
+00011680: 646c 6564 2e0a 0a41 7420 7468 6520 636f  dled...At the co
+00011690: 6e63 6c75 7369 6f6e 206f 6620 7468 6520  nclusion of the 
+000116a0: 5461 736b 2c20 6166 7465 7220 616e 7920  Task, after any 
+000116b0: 6669 6c65 7320 7265 7175 6573 7465 6420  files requested 
+000116c0: 666f 7220 7570 6c6f 6164 2068 6176 6520  for upload have 
+000116d0: 6265 656e 2075 706c 6f61 6465 6420 746f  been uploaded to
+000116e0: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
+000116f0: 6520 2873 6565 2074 6865 205b 4669 6c65  e (see the [File
+00011700: 7320 5570 6c6f 6164 6564 2066 726f 6d20  s Uploaded from 
+00011710: 6120 4e6f 6465 5d28 2366 696c 6573 2d75  a Node](#files-u
+00011720: 706c 6f61 6465 642d 6672 6f6d 2d61 2d6e  ploaded-from-a-n
+00011730: 6f64 652d 746f 2d74 6865 2d6f 626a 6563  ode-to-the-objec
+00011740: 742d 7374 6f72 652d 6166 7465 722d 7461  t-store-after-ta
+00011750: 736b 2d65 7865 6375 7469 6f6e 2920 7365  sk-execution) se
+00011760: 6374 696f 6e20 666f 7220 6d6f 7265 2069  ction for more i
+00011770: 6e66 6f72 6d61 7469 6f6e 292c 2074 6865  nformation), the
+00011780: 2060 7964 6964 5f74 6173 6b5f 3535 3945   `ydid_task_559E
+00011790: 4245 5f37 3439 3439 3333 362d 6163 3262  BE_74949336-ac2b
+000117a0: 2d34 3831 312d 6137 6435 2d66 3365 6364  -4811-a7d5-f3ecd
+000117b0: 3937 3339 3930 385f 315f 3160 2077 696c  9739908_1_1` wil
+000117c0: 6c20 6265 2072 656d 6f76 6564 2e0a 0a23  l be removed...#
+000117d0: 2320 5370 6563 6966 7969 6e67 2057 6f72  # Specifying Wor
+000117e0: 6b20 5265 7175 6972 656d 656e 7473 2075  k Requirements u
+000117f0: 7369 6e67 2043 5356 2044 6174 610a 0a43  sing CSV Data..C
+00011800: 5356 2064 6174 6120 6669 6c65 7320 6361  SV data files ca
+00011810: 6e20 6265 2075 7365 6420 746f 2064 7269  n be used to dri
+00011820: 7665 2074 6865 2067 656e 6572 6174 696f  ve the generatio
+00011830: 6e20 6f66 206c 6973 7473 206f 6620 5461  n of lists of Ta
+00011840: 736b 732c 2061 7320 666f 6c6c 6f77 733a  sks, as follows:
+00011850: 0a0a 2d20 4120 2a2a 7072 6f74 6f74 7970  ..- A **prototyp
+00011860: 652a 2a20 5461 736b 2073 7065 6369 6669  e** Task specifi
+00011870: 6361 7469 6f6e 2069 7320 6372 6561 7465  cation is create
+00011880: 6420 7769 7468 696e 2061 204a 534f 4e20  d within a JSON 
+00011890: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+000118a0: 2073 7065 6369 6669 6361 7469 6f6e 206f   specification o
+000118b0: 7220 696e 2074 6865 2060 776f 726b 5265  r in the `workRe
+000118c0: 7175 6972 656d 656e 7460 2073 6563 7469  quirement` secti
+000118d0: 6f6e 206f 6620 7468 6520 544f 4d4c 2063  on of the TOML c
+000118e0: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+000118f0: 650a 2d20 5468 6520 7072 6f74 6f74 7970  e.- The prototyp
+00011900: 6520 7461 736b 2069 6e63 6c75 6465 7320  e task includes 
+00011910: 6f6e 6520 6f72 206d 6f72 6520 7661 7269  one or more vari
+00011920: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
+00011930: 6e73 0a2d 2041 2043 5356 2066 696c 6520  ns.- A CSV file 
+00011940: 6973 2063 7265 6174 6564 2c20 7769 7468  is created, with
+00011950: 2074 6865 202a 2a68 6561 6465 7273 2a2a   the **headers**
+00011960: 2028 6669 7273 7420 726f 7729 206d 6174   (first row) mat
+00011970: 6368 696e 6720 7468 6520 6e61 6d65 7320  ching the names 
+00011980: 6f66 2074 6865 2076 6172 6961 626c 6520  of the variable 
+00011990: 7375 6273 7469 7475 7469 6f6e 7320 696e  substitutions in
+000119a0: 2074 6865 2054 6173 6b20 7072 6f74 6f74   the Task protot
+000119b0: 7970 650a 2d20 4561 6368 2073 7562 7365  ype.- Each subse
+000119c0: 7175 656e 7420 726f 7720 6f66 2074 6865  quent row of the
+000119d0: 2043 5356 2066 696c 6520 7265 7072 6573   CSV file repres
+000119e0: 656e 7473 2061 206e 6577 2054 6173 6b20  ents a new Task 
+000119f0: 6275 696c 7420 7573 696e 6720 7468 6520  built using the 
+00011a00: 7072 6f74 6f74 7970 652c 2077 6974 6820  prototype, with 
+00011a10: 7468 6520 7661 7269 6162 6c65 7320 7375  the variables su
+00011a20: 6273 7469 7475 7465 6420 6279 2074 6865  bstituted by the
+00011a30: 2076 616c 7565 7320 696e 2074 6865 2072   values in the r
+00011a40: 6f77 0a2d 2041 2054 6173 6b20 7769 6c6c  ow.- A Task will
+00011a50: 2062 6520 6372 6561 7465 6420 666f 7220   be created for 
+00011a60: 6561 6368 2064 6174 6120 726f 770a 0a23  each data row..#
+00011a70: 2323 2057 6f72 6b20 5265 7175 6972 656d  ## Work Requirem
+00011a80: 656e 7420 4353 5620 4461 7461 2045 7861  ent CSV Data Exa
+00011a90: 6d70 6c65 0a0a 4173 2061 6e20 6578 616d  mple..As an exam
+00011aa0: 706c 652c 2063 6f6e 7369 6465 7220 7468  ple, consider th
+00011ab0: 6520 666f 6c6c 6f77 696e 6720 4a53 4f4e  e following JSON
+00011ac0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00011ad0: 7420 6077 722e 6a73 6f6e 603a 0a0a 6060  t `wr.json`:..``
+00011ae0: 606a 736f 6e0a 7b0a 2020 2274 6173 6b47  `json.{.  "taskG
+00011af0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+00011b00: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+00011b10: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00011b20: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+00011b30: 3a20 5b22 7b7b 6172 675f 317d 7d22 2c20  : ["{{arg_1}}", 
+00011b40: 227b 7b61 7267 5f32 7d7d 222c 2022 7b7b  "{{arg_2}}", "{{
+00011b50: 6172 675f 337d 7d22 5d2c 0a20 2020 2020  arg_3}}"],.     
+00011b60: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+00011b70: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
+00011b80: 3a20 227b 7b65 6e76 5f31 7d7d 227d 0a20  : "{{env_1}}"}. 
+00011b90: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00011ba0: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
+00011bb0: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
+00011bc0: 5461 736b 2047 726f 7570 206d 7573 7420  Task Group must 
+00011bd0: 636f 6e74 6169 6e20 6f6e 6c79 2061 2073  contain only a s
+00011be0: 696e 676c 6520 5461 736b 2c20 6163 7469  ingle Task, acti
+00011bf0: 6e67 2061 7320 7468 6520 7072 6f74 6f74  ng as the protot
+00011c00: 7970 652e 0a0a 4e6f 7720 636f 6e73 6964  ype...Now consid
+00011c10: 6572 2061 2043 5356 2066 696c 6520 6077  er a CSV file `w
+00011c20: 725f 6461 7461 2e63 7376 6020 7769 7468  r_data.csv` with
+00011c30: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00011c40: 6f6e 7465 6e74 733a 0a0a 6060 6074 6578  ontents:..```tex
+00011c50: 740a 6172 675f 312c 2061 7267 5f32 2c20  t.arg_1, arg_2, 
+00011c60: 6172 675f 332c 2065 6e76 5f31 0a41 2c20  arg_3, env_1.A, 
+00011c70: 2020 2020 422c 2020 2020 2043 2c20 2020      B,     C,   
+00011c80: 2020 452d 310a 442c 2020 2020 2045 2c20    E-1.D,     E, 
+00011c90: 2020 2020 462c 2020 2020 2045 2d32 0a47      F,     E-2.G
+00011ca0: 2c20 2020 2020 482c 2020 2020 2049 2c20  ,     H,     I, 
+00011cb0: 2020 2020 452d 330a 6060 600a 0a4e 6f74      E-3.```..Not
+00011cc0: 6520 7468 6174 2074 6865 2028 6f70 7469  e that the (opti
+00011cd0: 6f6e 616c 2920 6c65 6164 696e 6720 7370  onal) leading sp
+00011ce0: 6163 6573 2061 6674 6572 2065 6163 6820  aces after each 
+00011cf0: 636f 6d6d 6120 6172 6520 6967 6e6f 7265  comma are ignore
+00011d00: 642c 2062 7574 2074 7261 696c 696e 6720  d, but trailing 
+00011d10: 7370 6163 6573 2061 7265 206e 6f74 2061  spaces are not a
+00011d20: 6e64 2077 696c 6c20 666f 726d 2070 6172  nd will form par
+00011d30: 7420 6f66 2074 6865 2069 6d70 6f72 7465  t of the importe
+00011d40: 6420 6461 7461 2e0a 0a49 6620 7468 6573  d data...If thes
+00011d50: 6520 6669 6c65 7320 6172 6520 7072 6f63  e files are proc
+00011d60: 6573 7365 6420 7573 696e 6720 6079 642d  essed using `yd-
+00011d70: 7375 626d 6974 202d 7220 7772 2e6a 736f  submit -r wr.jso
+00011d80: 6e20 2d56 2077 725f 6461 7461 2e63 7376  n -V wr_data.csv
+00011d90: 602c 2074 6865 2066 6f6c 6c6f 7769 6e67  `, the following
+00011da0: 2065 7870 616e 6465 6420 6c69 7374 206f   expanded list o
+00011db0: 6620 7468 7265 6520 5461 736b 7320 7769  f three Tasks wi
+00011dc0: 6c6c 2062 6520 6372 6561 7465 6420 7072  ll be created pr
+00011dd0: 696f 7220 746f 2066 7572 7468 6572 2070  ior to further p
+00011de0: 726f 6365 7373 696e 6720 6279 2074 6865  rocessing by the
+00011df0: 2060 7964 2d73 7562 6d69 7460 2073 6372   `yd-submit` scr
+00011e00: 6970 743a 0a0a 6060 606a 736f 6e0a 7b0a  ipt:..```json.{.
+00011e10: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
+00011e20: 5b0a 2020 2020 7b0a 2020 2020 2020 2274  [.    {.      "t
+00011e30: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
+00011e40: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+00011e50: 6775 6d65 6e74 7322 3a20 5b22 4122 2c20  guments": ["A", 
+00011e60: 2242 222c 2022 4322 5d2c 0a20 2020 2020  "B", "C"],.     
+00011e70: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+00011e80: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
+00011e90: 3a20 2245 2d31 227d 0a20 2020 2020 2020  : "E-1"}.       
+00011ea0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00011eb0: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00011ec0: 7473 223a 205b 2244 222c 2022 4522 2c20  ts": ["D", "E", 
+00011ed0: 2246 225d 2c0a 2020 2020 2020 2020 2020  "F"],.          
+00011ee0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00011ef0: 2245 4e56 5f56 4152 5f31 223a 2022 452d  "ENV_VAR_1": "E-
+00011f00: 3222 7d0a 2020 2020 2020 2020 7d2c 0a20  2"}.        },. 
+00011f10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00011f20: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
+00011f30: 5b22 4722 2c20 2248 222c 2022 4922 5d2c  ["G", "H", "I"],
+00011f40: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
+00011f50: 726f 6e6d 656e 7422 3a20 7b22 454e 565f  ronment": {"ENV_
+00011f60: 5641 525f 3122 3a20 2245 2d33 227d 0a20  VAR_1": "E-3"}. 
+00011f70: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00011f80: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
+00011f90: 0a0a 2323 2320 4353 5620 5661 7269 6162  ..### CSV Variab
+00011fa0: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
+00011fb0: 0a0a 5768 656e 2074 6865 2043 5356 2066  ..When the CSV f
+00011fc0: 696c 6520 6461 7461 2069 7320 7072 6f63  ile data is proc
+00011fd0: 6573 7365 642c 2074 6865 206f 6e6c 7920  essed, the only 
+00011fe0: 7375 6273 7469 7475 7469 6f6e 7320 6d61  substitutions ma
+00011ff0: 6465 2061 7265 2074 686f 7365 2077 6869  de are those whi
+00012000: 6368 206d 6174 6368 2074 6865 2076 6172  ch match the var
+00012010: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00012020: 6f6e 7320 696e 2074 6865 2070 726f 746f  ons in the proto
+00012030: 7479 7065 2054 6173 6b2e 2054 6865 2043  type Task. The C
+00012040: 5356 2066 696c 6520 6973 2074 6865 202a  SV file is the *
+00012050: 2a6f 6e6c 792a 2a20 736f 7572 6365 206f  *only** source o
+00012060: 6620 7375 6273 7469 7475 7469 6f6e 7320  f substitutions 
+00012070: 7573 6564 2066 6f72 2074 6869 7320 7072  used for this pr
+00012080: 6f63 6573 7369 6e67 2070 6861 7365 3b20  ocessing phase; 
+00012090: 616c 6c20 6f74 6865 7220 7661 7269 6162  all other variab
+000120a0: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
+000120b0: 2028 7375 7070 6c69 6564 206f 6e20 7468   (supplied on th
+000120c0: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
+000120d0: 696e 2074 6865 2054 4f4d 4c20 636f 6e66  in the TOML conf
+000120e0: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
+000120f0: 6f72 2066 726f 6d20 656e 7669 726f 6e6d  or from environm
+00012100: 656e 7420 7661 7269 6162 6c65 7329 2061  ent variables) a
+00012110: 7265 2069 676e 6f72 6564 202d 2d20 692e  re ignored -- i.
+00012120: 652e 2c20 7468 6579 2064 6f20 6e6f 7420  e., they do not 
+00012130: 6f76 6572 7269 6465 2074 6865 2063 6f6e  override the con
+00012140: 7465 6e74 7320 6f66 2074 6865 2043 5356  tents of the CSV
+00012150: 2066 696c 652e 0a0a 416c 6c20 7661 7269   file...All vari
+00012160: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
+00012170: 6e73 2075 6e72 656c 6174 6564 2074 6f20  ns unrelated to 
+00012180: 7468 6520 4353 5620 6669 6c65 2064 6174  the CSV file dat
+00012190: 6120 6172 6520 6c65 6674 2075 6e63 6861  a are left uncha
+000121a0: 6e67 6564 2c20 666f 7220 7375 6273 6571  nged, for subseq
+000121b0: 7565 6e74 2070 726f 6365 7373 696e 6720  uent processing 
+000121c0: 6279 2060 7964 2d73 7562 6d69 7460 2e0a  by `yd-submit`..
+000121d0: 0a49 6620 7468 6520 7661 6c75 6520 746f  .If the value to
+000121e0: 2062 6520 696e 7365 7274 6564 2069 7320   be inserted is 
+000121f0: 6120 6e75 6d62 6572 2028 616e 2069 6e74  a number (an int
+00012200: 6567 6572 206f 7220 666c 6f61 7469 6e67  eger or floating
+00012210: 2070 6f69 6e74 2076 616c 7565 2920 6f72   point value) or
+00012220: 2042 6f6f 6c65 616e 2c20 7468 6520 607b   Boolean, the `{
+00012230: 7b6e 756d 3a6d 795f 6e75 6d62 6572 5f76  {num:my_number_v
+00012240: 6172 7d7d 6020 616e 6420 607b 7b62 6f6f  ar}}` and `{{boo
+00012250: 6c3a 6d79 5f62 6f6f 6c65 616e 5f76 6172  l:my_boolean_var
+00012260: 7d7d 6020 666f 726d 7320 6361 6e20 6265  }}` forms can be
+00012270: 2075 7365 6420 696e 2074 6865 204a 534f   used in the JSO
+00012280: 4e20 6669 6c65 2c20 6173 2077 6974 6820  N file, as with 
+00012290: 7468 6569 7220 7573 6520 696e 206f 7468  their use in oth
+000122a0: 6572 2070 6172 7473 206f 6620 7468 6520  er parts of the 
+000122b0: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
+000122c0: 656d 656e 7420 7370 6563 6966 6963 6174  ement specificat
+000122d0: 696f 6e2e 2054 6865 2073 7562 7374 6974  ion. The substit
+000122e0: 7574 6564 2076 616c 7565 2077 696c 6c20  uted value will 
+000122f0: 6173 7375 6d65 2074 6865 206e 6f6d 696e  assume the nomin
+00012300: 6174 6564 2074 7970 6520 7261 7468 6572  ated type rather
+00012310: 2074 6861 6e20 6265 696e 6720 6120 7374   than being a st
+00012320: 7269 6e67 2e0a 0a23 2323 2050 726f 7065  ring...### Prope
+00012330: 7274 7920 496e 6865 7269 7461 6e63 650a  rty Inheritance.
+00012340: 0a41 6c6c 2074 6865 2075 7375 616c 2070  .All the usual p
+00012350: 726f 7065 7274 7920 696e 6865 7269 7461  roperty inherita
+00012360: 6e63 6520 6665 6174 7572 6573 206f 7065  nce features ope
+00012370: 7261 7465 2061 7320 6e6f 726d 616c 2e20  rate as normal. 
+00012380: 5072 6f70 6572 7469 6573 2061 7265 2069  Properties are i
+00012390: 6e68 6572 6974 6564 2066 726f 6d20 7468  nherited from th
+000123a0: 6520 6063 6f6e 6669 672e 746f 6d6c 6020  e `config.toml` 
+000123b0: 6669 6c65 2c20 616e 6420 6672 6f6d 2074  file, and from t
+000123c0: 6865 2072 656c 6576 616e 7420 7365 6374  he relevant sect
+000123d0: 696f 6e73 206f 6620 7468 6520 4a53 4f4e  ions of the JSON
+000123e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000123f0: 7420 6669 6c65 2e20 416e 7920 7072 6f70  t file. Any prop
+00012400: 6572 7469 6573 2073 6574 2077 6974 6869  erties set withi
+00012410: 6e20 6120 5461 736b 2070 726f 746f 7479  n a Task prototy
+00012420: 7065 2061 7265 2063 6f70 6965 6420 746f  pe are copied to
+00012430: 2061 6c6c 2074 6865 2067 656e 6572 6174   all the generat
+00012440: 6564 2054 6173 6b73 2e0a 0a23 2323 204d  ed Tasks...### M
+00012450: 756c 7469 706c 6520 5461 736b 2047 726f  ultiple Task Gro
+00012460: 7570 7320 7573 696e 6720 4d75 6c74 6970  ups using Multip
+00012470: 6c65 2043 5356 2046 696c 6573 0a0a 5468  le CSV Files..Th
+00012480: 6520 7573 6520 6f66 206d 756c 7469 706c  e use of multipl
+00012490: 6520 5461 736b 2047 726f 7570 7320 6973  e Task Groups is
+000124a0: 2061 6c73 6f20 7375 7070 6f72 7465 642c   also supported,
+000124b0: 2062 7920 7573 696e 6720 6f6e 6520 4353   by using one CS
+000124c0: 5620 6669 6c65 2070 6572 2054 6173 6b20  V file per Task 
+000124d0: 4772 6f75 702e 2045 6163 6820 5461 736b  Group. Each Task
+000124e0: 2047 726f 7570 206d 7573 7420 636f 6e74   Group must cont
+000124f0: 6169 6e20 6f6e 6c79 2061 2073 696e 676c  ain only a singl
+00012500: 6520 7072 6f74 6f74 7970 6520 5461 736b  e prototype Task
+00012510: 2e0a 0a54 6865 2043 5356 2066 696c 6573  ...The CSV files
+00012520: 2061 7265 2073 7570 706c 6965 6420 6f6e   are supplied on
+00012530: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00012540: 6520 696e 2074 6865 206f 7264 6572 206f  e in the order o
+00012550: 6620 7468 6520 5461 736b 2047 726f 7570  f the Task Group
+00012560: 7320 746f 2077 6869 6368 2074 6865 7920  s to which they 
+00012570: 6170 706c 792e 2046 6f72 2065 7861 6d70  apply. For examp
+00012580: 6c65 2c20 6966 2060 7772 5f6a 736f 6e60  le, if `wr_json`
+00012590: 2063 6f6e 7461 696e 7320 7477 6f20 5461   contains two Ta
+000125a0: 736b 2047 726f 7570 732c 2061 7320 666f  sk Groups, as fo
+000125b0: 6c6c 6f77 733a 0a0a 6060 606a 736f 6e0a  llows:..```json.
+000125c0: 7b0a 2020 2274 6173 6b47 726f 7570 7322  {.  "taskGroups"
+000125d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+000125e0: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
+000125f0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00012600: 6172 6775 6d65 6e74 7322 3a20 5b22 7b7b  arguments": ["{{
+00012610: 6172 675f 317d 7d22 2c20 227b 7b61 7267  arg_1}}", "{{arg
+00012620: 5f32 7d7d 222c 2022 7b7b 6172 675f 337d  _2}}", "{{arg_3}
+00012630: 7d22 5d2c 0a20 2020 2020 2020 2020 2022  }"],.          "
+00012640: 656e 7669 726f 6e6d 656e 7422 3a20 7b22  environment": {"
+00012650: 454e 565f 5641 525f 3122 3a20 227b 7b65  ENV_VAR_1": "{{e
+00012660: 6e76 5f31 7d7d 227d 0a20 2020 2020 2020  nv_1}}"}.       
+00012670: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
+00012680: 2c0a 2020 2020 7b0a 2020 2020 2020 2274  ,.    {.      "t
+00012690: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
+000126a0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+000126b0: 6775 6d65 6e74 7322 3a20 5b22 7b7b 6172  guments": ["{{ar
+000126c0: 675f 317d 7d22 2c20 227b 7b61 7267 5f32  g_1}}", "{{arg_2
+000126d0: 7d7d 225d 2c0a 2020 2020 2020 2020 2020  }}"],.          
+000126e0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+000126f0: 2245 4e56 5f56 4152 5f31 223a 2022 7b7b  "ENV_VAR_1": "{{
+00012700: 656e 765f 317d 7d22 2c20 2245 4e56 5f56  env_1}}", "ENV_V
+00012710: 4152 5f32 223a 2022 7b7b 656e 765f 327d  AR_2": "{{env_2}
+00012720: 7d22 7d0a 2020 2020 2020 2020 7d0a 2020  }"}.        }.  
+00012730: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
+00012740: 7d0a 6060 600a 0a54 6865 2060 7964 2d73  }.```..The `yd-s
+00012750: 7562 6d69 7460 2063 6f6d 6d61 6e64 2077  ubmit` command w
+00012760: 6f75 6c64 2074 6865 6e20 6265 2069 6e76  ould then be inv
+00012770: 6f6b 6564 2077 6974 6820 6120 7365 7061  oked with a sepa
+00012780: 7261 7465 2043 5356 2066 696c 6520 666f  rate CSV file fo
+00012790: 7220 6561 6368 2054 6173 6b20 4772 6f75  r each Task Grou
+000127a0: 702c 2065 2e67 2e3a 0a0a 6060 6073 6865  p, e.g.:..```she
+000127b0: 6c6c 0a79 642d 7375 626d 6974 202d 7220  ll.yd-submit -r 
+000127c0: 7772 2e6a 736f 6e20 2d56 2077 725f 6461  wr.json -V wr_da
+000127d0: 7461 5f74 6173 6b5f 6772 6f75 705f 312e  ta_task_group_1.
+000127e0: 6373 7620 2d56 2077 725f 6461 7461 5f74  csv -V wr_data_t
+000127f0: 6173 6b5f 6772 6f75 705f 322e 6373 760a  ask_group_2.csv.
+00012800: 6060 600a 0a49 6620 7468 6572 6520 6172  ```..If there ar
+00012810: 6520 2a2a 6665 7765 722a 2a20 4353 5620  e **fewer** CSV 
+00012820: 6669 6c65 7320 7468 616e 2054 6173 6b20  files than Task 
+00012830: 4772 6f75 7073 2061 2077 6172 6e69 6e67  Groups a warning
+00012840: 2077 696c 6c20 6265 2070 7269 6e74 6564   will be printed
+00012850: 2061 6e64 2c20 6966 2074 6865 7265 2061   and, if there a
+00012860: 7265 2027 6e27 2043 5356 2066 696c 6573  re 'n' CSV files
+00012870: 2c20 4353 5620 6461 7461 2070 726f 6365  , CSV data proce
+00012880: 7373 696e 6720 7769 6c6c 2062 6520 6170  ssing will be ap
+00012890: 706c 6965 6420 746f 2074 6865 2066 6972  plied to the fir
+000128a0: 7374 2027 6e27 2054 6173 6b20 4772 6f75  st 'n' Task Grou
+000128b0: 7073 2069 6e20 7468 6520 576f 726b 2052  ps in the Work R
+000128c0: 6571 7569 7265 6d65 6e74 2062 7920 6465  equirement by de
+000128d0: 6661 756c 742c 2069 6e20 7468 6520 6f72  fault, in the or
+000128e0: 6465 7220 696e 2077 6869 6368 2074 6865  der in which the
+000128f0: 2043 5356 2066 696c 6573 2077 6572 6520   CSV files were 
+00012900: 7375 7070 6c69 6564 2e20 4966 2074 6865  supplied. If the
+00012910: 7265 2061 7265 202a 2a6d 6f72 652a 2a20  re are **more** 
+00012920: 4353 5620 6669 6c65 7320 7468 616e 2054  CSV files than T
+00012930: 6173 6b20 4772 6f75 7073 2c20 616e 2065  ask Groups, an e
+00012940: 7272 6f72 2077 696c 6c20 6265 2072 6169  rror will be rai
+00012950: 7365 6420 616e 6420 7072 6f63 6573 7369  sed and processi
+00012960: 6e67 2077 696c 6c20 7374 6f70 2e0a 0a49  ng will stop...I
+00012970: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
+00012980: 2061 7070 6c79 2043 5356 2066 696c 6573   apply CSV files
+00012990: 2065 7870 6c69 6369 746c 7920 746f 2073   explicitly to s
+000129a0: 7065 6369 6669 6320 5461 736b 2047 726f  pecific Task Gro
+000129b0: 7570 732c 2062 7920 7573 696e 6720 616e  ups, by using an
+000129c0: 206f 7074 696f 6e61 6c20 2a2a 696e 6465   optional **inde
+000129d0: 7820 706f 7374 6669 782a 2a20 2865 2e67  x postfix** (e.g
+000129e0: 2e2c 2060 3a32 6029 2061 7420 7468 6520  ., `:2`) at the 
+000129f0: 656e 6420 6f66 2065 6163 6820 4353 5620  end of each CSV 
+00012a00: 6669 6c65 6e61 6d65 2e20 466f 7220 6578  filename. For ex
+00012a10: 616d 706c 652c 2069 6620 7468 6572 6520  ample, if there 
+00012a20: 6172 6520 7477 6f20 4353 5620 6669 6c65  are two CSV file
+00012a30: 7320 746f 2062 6520 6170 706c 6965 6420  s to be applied 
+00012a40: 746f 2074 6865 2073 6563 6f6e 6420 616e  to the second an
+00012a50: 6420 666f 7572 7468 2054 6173 6b20 4772  d fourth Task Gr
+00012a60: 6f75 7073 2069 6e20 6120 4a53 4f4e 2057  oups in a JSON W
+00012a70: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
+00012a80: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
+00012a90: 6e67 2073 796e 7461 783a 0a0a 6060 6073  ng syntax:..```s
+00012aa0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
+00012ab0: 7220 7772 2e6a 736f 6e20 2d56 2077 725f  r wr.json -V wr_
+00012ac0: 6461 7461 5f74 6173 6b5f 6772 6f75 705f  data_task_group_
+00012ad0: 322e 6373 763a 3220 2d56 2077 725f 6461  2.csv:2 -V wr_da
+00012ae0: 7461 5f74 6173 6b5f 6772 6f75 705f 342e  ta_task_group_4.
+00012af0: 6373 763a 340a 6060 600a 0a41 6c74 6572  csv:4.```..Alter
+00012b00: 6e61 7469 7665 6c79 2c20 7468 6520 2a2a  natively, the **
+00012b10: 5461 736b 2047 726f 7570 206e 616d 652a  Task Group name*
+00012b20: 2a20 2869 6620 7375 7070 6c69 6564 2069  * (if supplied i
+00012b30: 6e20 7468 6520 4a53 4f4e 2066 696c 6529  n the JSON file)
+00012b40: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
+00012b50: 7468 6520 706f 7374 6669 782e 2046 6f72  the postfix. For
+00012b60: 2065 7861 6d70 6c65 2c20 6966 2074 6865   example, if the
+00012b70: 2054 6173 6b20 4772 6f75 7073 2061 626f   Task Groups abo
+00012b80: 7665 2061 7265 206e 616d 6564 2060 7467  ve are named `tg
+00012b90: 5f74 776f 6020 616e 6420 6074 675f 666f  _two` and `tg_fo
+00012ba0: 7572 602c 2074 6865 2060 7964 2d73 7562  ur`, the `yd-sub
+00012bb0: 6d69 7460 2063 6f6d 6d61 6e64 2077 6f75  mit` command wou
+00012bc0: 6c64 2062 6563 6f6d 653a 0a0a 6060 6073  ld become:..```s
+00012bd0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
+00012be0: 7220 7772 2e6a 736f 6e20 2d56 2077 725f  r wr.json -V wr_
+00012bf0: 6461 7461 5f74 6173 6b5f 6772 6f75 705f  data_task_group_
+00012c00: 322e 6373 763a 7467 5f74 776f 202d 5620  2.csv:tg_two -V 
+00012c10: 7772 5f64 6174 615f 7461 736b 5f67 726f  wr_data_task_gro
+00012c20: 7570 5f34 2e63 7376 3a74 675f 666f 7572  up_4.csv:tg_four
+00012c30: 0a60 6060 0a0a 4e6f 7465 2074 6861 7420  .```..Note that 
+00012c40: 6f6e 6c79 206f 6e65 2043 5356 2066 696c  only one CSV fil
+00012c50: 6520 6361 6e20 6265 2061 7070 6c69 6564  e can be applied
+00012c60: 2074 6f20 616e 7920 6769 7665 6e20 5461   to any given Ta
+00012c70: 736b 2047 726f 7570 2e20 4120 7369 6e67  sk Group. A sing
+00012c80: 6c65 2043 5356 2066 696c 6520 6361 6e2c  le CSV file can,
+00012c90: 2068 6f77 6576 6572 2c20 6265 2072 6575   however, be reu
+00012ca0: 7365 6420 666f 7220 6d75 6c74 6970 6c65  sed for multiple
+00012cb0: 2054 6173 6b20 4772 6f75 7073 2e0a 0a23   Task Groups...#
+00012cc0: 2323 2055 7369 6e67 2043 5356 2044 6174  ## Using CSV Dat
+00012cd0: 6120 7769 7468 2053 696d 706c 652c 2054  a with Simple, T
+00012ce0: 4f4d 4c2d 4f6e 6c79 2057 6f72 6b20 5265  OML-Only Work Re
+00012cf0: 7175 6972 656d 656e 7420 5370 6563 6966  quirement Specif
+00012d00: 6963 6174 696f 6e73 0a0a 4974 2773 2070  ications..It's p
+00012d10: 6f73 7369 626c 6520 746f 2075 7365 2054  ossible to use T
+00012d20: 4f4d 4c20 6578 636c 7573 6976 656c 7920  OML exclusively 
+00012d30: 746f 2064 6572 6976 6520 6120 6c69 7374  to derive a list
+00012d40: 206f 6620 5461 736b 7320 6672 6f6d 2043   of Tasks from C
+00012d50: 5356 2064 6174 6120 2d2d 2069 2e65 2e2c  SV data -- i.e.,
+00012d60: 2061 204a 534f 4e20 576f 726b 2052 6571   a JSON Work Req
+00012d70: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
+00012d80: 6361 7469 6f6e 2069 7320 6e6f 7420 7265  cation is not re
+00012d90: 7175 6972 6564 2e0a 0a54 6f20 6d61 6b65  quired...To make
+00012da0: 2075 7365 206f 6620 7468 6973 3a0a 0a31   use of this:..1
+00012db0: 2e20 456e 7375 7265 2074 6861 7420 6e6f  . Ensure that no
+00012dc0: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
+00012dd0: 7265 6d65 6e74 2064 6f63 756d 656e 7420  rement document 
+00012de0: 6973 2073 7065 6369 6669 6564 2028 6e6f  is specified (no
+00012df0: 2060 776f 726b 5265 7175 6972 656d 656e   `workRequiremen
+00012e00: 7444 6174 6160 2069 6e20 7468 6520 544f  tData` in the TO
+00012e10: 4d4c 2066 696c 652c 206f 7220 602d 2d77  ML file, or `--w
+00012e20: 6f72 6b2d 7265 7175 6972 656d 656e 7460  ork-requirement`
+00012e30: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
+00012e40: 6c69 6e65 290a 322e 2049 6e73 6572 7420  line).2. Insert 
+00012e50: 7468 6520 7265 7175 6972 6564 2043 5356  the required CSV
+00012e60: 2d73 7570 706c 6965 6420 7661 7269 6162  -supplied variab
+00012e70: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
+00012e80: 2064 6972 6563 746c 7920 696e 746f 2074   directly into t
+00012e90: 6865 2054 4f4d 4c20 7072 6f70 6572 7469  he TOML properti
+00012ea0: 6573 2c20 652e 672e 2060 6172 6775 6d65  es, e.g. `argume
+00012eb0: 6e74 7320 3d20 5b22 7b7b 6172 675f 317d  nts = ["{{arg_1}
+00012ec0: 7d22 2c20 227b 7b61 7267 5f32 7d7d 225d  }", "{{arg_2}}"]
+00012ed0: 600a 332e 2053 7065 6369 6679 2061 2073  `.3. Specify a s
+00012ee0: 696e 676c 6520 4353 5620 6669 6c65 2069  ingle CSV file i
+00012ef0: 6e20 7468 6520 6063 7376 4669 6c65 7360  n the `csvFiles`
+00012f00: 2054 4f4d 4c20 7072 6f70 6572 7479 2c20   TOML property, 
+00012f10: 652e 672e 2060 6373 7646 696c 6573 203d  e.g. `csvFiles =
+00012f20: 205b 2277 725f 6461 7461 2e63 7376 225d   ["wr_data.csv"]
+00012f30: 602c 206f 7220 7072 6f76 6964 6520 7468  `, or provide th
+00012f40: 6520 4353 5620 6669 6c65 206f 6e20 7468  e CSV file on th
+00012f50: 6520 636f 6d6d 616e 6420 6c69 6e65 2060  e command line `
+00012f60: 2d56 2077 725f 6461 7461 2e63 7376 600a  -V wr_data.csv`.
+00012f70: 0a57 6865 6e20 6079 642d 7375 626d 6974  .When `yd-submit
+00012f80: 6020 6973 2072 756e 2c20 6974 2077 696c  ` is run, it wil
+00012f90: 6c20 6578 7061 6e64 2074 6865 2054 6173  l expand the Tas
+00012fa0: 6b20 6c69 7374 2074 6f20 6d61 7463 6820  k list to match 
+00012fb0: 7468 6520 6e75 6d62 6572 206f 6620 6461  the number of da
+00012fc0: 7461 2072 6f77 7320 696e 2074 6865 2043  ta rows in the C
+00012fd0: 5356 2066 696c 652e 0a0a 2323 2320 496e  SV file...### In
+00012fe0: 7370 6563 7469 6e67 2074 6865 2052 6573  specting the Res
+00012ff0: 756c 7473 206f 6620 4353 5620 5661 7269  ults of CSV Vari
+00013000: 6162 6c65 2053 7562 7374 6974 7574 696f  able Substitutio
+00013010: 6e0a 0a54 6865 2060 2d2d 7072 6f63 6573  n..The `--proces
+00013020: 732d 6373 762d 6f6e 6c79 6020 286f 7220  s-csv-only` (or 
+00013030: 602d 7060 2920 6f70 7469 6f6e 2063 616e  `-p`) option can
+00013040: 2062 6520 7573 6564 2077 6974 6820 6079   be used with `y
+00013050: 642d 7375 626d 6974 6020 746f 206f 7574  d-submit` to out
+00013060: 7075 7420 7468 6520 4a53 4f4e 2057 6f72  put the JSON Wor
+00013070: 6b20 5265 7175 6972 656d 656e 7420 6166  k Requirement af
+00013080: 7465 7220 4353 5620 7661 7269 6162 6c65  ter CSV variable
+00013090: 2073 7562 7374 6974 7574 696f 6e73 206f   substitutions o
+000130a0: 6e6c 792c 2070 7269 6f72 2074 6f20 616c  nly, prior to al
+000130b0: 6c20 6f74 6865 7220 7375 6273 7469 7475  l other substitu
+000130c0: 7469 6f6e 7320 616e 6420 7072 6f70 6572  tions and proper
+000130d0: 7479 2069 6e68 6572 6974 616e 6365 2061  ty inheritance a
+000130e0: 7070 6c69 6564 2062 7920 6079 642d 7375  pplied by `yd-su
+000130f0: 626d 6974 602e 0a0a 2320 576f 726b 6572  bmit`...# Worker
+00013100: 2050 6f6f 6c20 5072 6f70 6572 7469 6573   Pool Properties
+00013110: 0a0a 5468 6520 6077 6f72 6b65 7250 6f6f  ..The `workerPoo
+00013120: 6c60 2073 6563 7469 6f6e 206f 6620 7468  l` section of th
+00013130: 6520 544f 4d4c 2066 696c 6520 6465 6669  e TOML file defi
+00013140: 6e65 7320 7468 6520 7072 6f70 6572 7469  nes the properti
+00013150: 6573 206f 6620 7468 6520 576f 726b 6572  es of the Worker
+00013160: 2050 6f6f 6c20 746f 2062 6520 6372 6561   Pool to be crea
+00013170: 7465 642c 2061 6e64 2069 7320 7573 6564  ted, and is used
+00013180: 2062 7920 7468 6520 6079 642d 7072 6f76   by the `yd-prov
+00013190: 6973 696f 6e60 2063 6f6d 6d61 6e64 2e20  ision` command. 
+000131a0: 4120 7375 6273 6574 206f 6620 7468 6520  A subset of the 
+000131b0: 7072 6f70 6572 7469 6573 2069 7320 616c  properties is al
+000131c0: 736f 2075 7365 6420 6279 2074 6865 2060  so used by the `
+000131d0: 7964 2d69 6e73 7461 6e74 6961 7465 6020  yd-instantiate` 
+000131e0: 636f 6d6d 616e 642c 2066 6f72 2063 7265  command, for cre
+000131f0: 6174 696e 6720 7374 616e 6461 6c6f 6e65  ating standalone
+00013200: 2043 6f6d 7075 7465 2052 6571 7569 7265   Compute Require
+00013210: 6d65 6e74 7320 7468 6174 2061 7265 206e  ments that are n
+00013220: 6f74 2061 7373 6f63 6961 7465 6420 7769  ot associated wi
+00013230: 7468 2057 6f72 6b65 7220 506f 6f6c 732e  th Worker Pools.
+00013240: 0a0a 5468 6520 6f6e 6c79 206d 616e 6461  ..The only manda
+00013250: 746f 7279 2070 726f 7065 7274 7920 6973  tory property is
+00013260: 2060 7465 6d70 6c61 7465 4964 602e 2041   `templateId`. A
+00013270: 6c6c 206f 7468 6572 2070 726f 7065 7274  ll other propert
+00013280: 6965 7320 6861 7665 2064 6566 6175 6c74  ies have default
+00013290: 7320 286f 7220 6172 6520 6e6f 7420 7265  s (or are not re
+000132a0: 7175 6972 6564 292e 0a0a 5468 6520 666f  quired)...The fo
+000132b0: 6c6c 6f77 696e 6720 7072 6f70 6572 7469  llowing properti
+000132c0: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
+000132d0: 3a0a 0a7c 2050 726f 7065 7274 7920 2020  :..| Property   
+000132e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000132f0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
 00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 2020 2020 2020 2020 2020 7c20 4465 6661            | Defa
-00013370: 756c 7420 2020 2020 2020 2020 2020 2020  ult             
-00013380: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
+00013360: 2020 2020 2020 2020 207c 2044 6566 6175           | Defau
+00013370: 6c74 2020 2020 2020 2020 2020 2020 2020  lt              
+00013380: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
 00013390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000133a0: 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|:------------
+000133a0: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
 000133b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000133c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000133d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000133e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000133f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
+00013410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
 00013420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013430: 2d2d 2d2d 2d2d 7c0a 7c20 6069 646c 654e  ------|.| `idleN
-00013440: 6f64 6553 6875 7464 6f77 6e45 6e61 626c  odeShutdownEnabl
-00013450: 6564 6020 7c20 5768 6574 6865 7220 746f  ed` | Whether to
-00013460: 2073 6875 7420 646f 776e 206e 6f64 6573   shut down nodes
-00013470: 2074 6861 7420 6861 7665 2062 6565 6e20   that have been 
-00013480: 6964 6c65 2066 6f72 2060 6964 6c65 4e6f  idle for `idleNo
-00013490: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
-000134a0: 7460 206d 696e 7574 6573 2e20 2020 2020  t` minutes.     
+00013430: 2d2d 2d2d 2d7c 0a7c 2060 6964 6c65 4e6f  -----|.| `idleNo
+00013440: 6465 5368 7574 646f 776e 456e 6162 6c65  deShutdownEnable
+00013450: 6460 207c 2057 6865 7468 6572 2074 6f20  d` | Whether to 
+00013460: 7368 7574 2064 6f77 6e20 6e6f 6465 7320  shut down nodes 
+00013470: 7468 6174 2068 6176 6520 6265 656e 2069  that have been i
+00013480: 646c 6520 666f 7220 6069 646c 654e 6f64  dle for `idleNod
+00013490: 6553 6875 7464 6f77 6e54 696d 656f 7574  eShutdownTimeout
+000134a0: 6020 6d69 6e75 7465 732e 2020 2020 2020  ` minutes.      
 000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000134d0: 6054 7275 6560 2020 2020 2020 2020 2020  `True`          
-000134e0: 2020 2020 2020 2020 7c0a 7c20 6069 646c          |.| `idl
-000134f0: 654e 6f64 6553 6875 7464 6f77 6e54 696d  eNodeShutdownTim
-00013500: 656f 7574 6020 7c20 5468 6520 7469 6d65  eout` | The time
-00013510: 6f75 7420 696e 206d 696e 7574 6573 2061  out in minutes a
-00013520: 6674 6572 2077 6869 6368 2061 6e20 6964  fter which an id
-00013530: 6c65 206e 6f64 6520 7769 6c6c 2062 6520  le node will be 
-00013540: 7368 7574 2064 6f77 6e20 6966 2060 6964  shut down if `id
-00013550: 6c65 4e6f 6465 5368 7574 646f 776e 456e  leNodeShutdownEn
-00013560: 6162 6c65 6460 2069 7320 7365 7420 746f  abled` is set to
-00013570: 2060 5472 7565 602e 2020 2020 2020 2020   `True`.        
-00013580: 7c20 6035 2e30 6020 2020 2020 2020 2020  | `5.0`         
-00013590: 2020 2020 2020 2020 2020 7c0a 7c20 6069            |.| `i
-000135a0: 646c 6550 6f6f 6c53 6875 7464 6f77 6e45  dlePoolShutdownE
-000135b0: 6e61 626c 6564 6020 7c20 5768 6574 6865  nabled` | Whethe
-000135c0: 7220 746f 2073 6875 7420 646f 776e 2074  r to shut down t
-000135d0: 6865 2057 6f72 6b65 7220 506f 6f6c 2077  he Worker Pool w
-000135e0: 6865 6e20 6974 2068 6173 2062 6565 6e20  hen it has been 
-000135f0: 6964 6c65 2066 6f72 2060 6964 6c65 506f  idle for `idlePo
-00013600: 6f6c 5368 7574 646f 776e 5469 6d65 6f75  olShutdownTimeou
-00013610: 7460 206d 696e 7574 6573 2e20 2020 2020  t` minutes.     
+000134c0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+000134d0: 5472 7565 6020 2020 2020 2020 2020 2020  True`           
+000134e0: 2020 2020 2020 207c 0a7c 2060 6964 6c65         |.| `idle
+000134f0: 4e6f 6465 5368 7574 646f 776e 5469 6d65  NodeShutdownTime
+00013500: 6f75 7460 207c 2054 6865 2074 696d 656f  out` | The timeo
+00013510: 7574 2069 6e20 6d69 6e75 7465 7320 6166  ut in minutes af
+00013520: 7465 7220 7768 6963 6820 616e 2069 646c  ter which an idl
+00013530: 6520 6e6f 6465 2077 696c 6c20 6265 2073  e node will be s
+00013540: 6875 7420 646f 776e 2069 6620 6069 646c  hut down if `idl
+00013550: 654e 6f64 6553 6875 7464 6f77 6e45 6e61  eNodeShutdownEna
+00013560: 626c 6564 6020 6973 2073 6574 2074 6f20  bled` is set to 
+00013570: 6054 7275 6560 2e20 2020 2020 2020 207c  `True`.        |
+00013580: 2060 352e 3060 2020 2020 2020 2020 2020   `5.0`          
+00013590: 2020 2020 2020 2020 207c 0a7c 2060 6964           |.| `id
+000135a0: 6c65 506f 6f6c 5368 7574 646f 776e 456e  lePoolShutdownEn
+000135b0: 6162 6c65 6460 207c 2057 6865 7468 6572  abled` | Whether
+000135c0: 2074 6f20 7368 7574 2064 6f77 6e20 7468   to shut down th
+000135d0: 6520 576f 726b 6572 2050 6f6f 6c20 7768  e Worker Pool wh
+000135e0: 656e 2069 7420 6861 7320 6265 656e 2069  en it has been i
+000135f0: 646c 6520 666f 7220 6069 646c 6550 6f6f  dle for `idlePoo
+00013600: 6c53 6875 7464 6f77 6e54 696d 656f 7574  lShutdownTimeout
+00013610: 6020 6d69 6e75 7465 732e 2020 2020 2020  ` minutes.      
 00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 2020 7c20 6054 7275 6560 2020 2020 2020    | `True`      
-00013640: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00013650: 6069 646c 6550 6f6f 6c53 6875 7464 6f77  `idlePoolShutdow
-00013660: 6e54 696d 656f 7574 6020 7c20 5468 6520  nTimeout` | The 
-00013670: 7469 6d65 6f75 7420 696e 206d 696e 7574  timeout in minut
-00013680: 6573 2061 6674 6572 2077 6869 6368 2061  es after which a
-00013690: 6e20 6964 6c65 2057 6f72 6b65 7220 506f  n idle Worker Po
-000136a0: 6f6c 2077 696c 6c20 6265 2073 6875 7420  ol will be shut 
-000136b0: 646f 776e 2069 6620 6069 646c 6550 6f6f  down if `idlePoo
-000136c0: 6c53 6875 7464 6f77 6e45 6e61 626c 6564  lShutdownEnabled
-000136d0: 6020 6973 2073 6574 2074 6f20 6054 7275  ` is set to `Tru
-000136e0: 6560 2e20 7c20 6033 302e 3060 2020 2020  e`. | `30.0`    
-000136f0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00013700: 7c20 6069 6d61 6765 7349 6460 2020 2020  | `imagesId`    
-00013710: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-00013720: 6520 696d 6167 6573 2049 4420 746f 2075  e images ID to u
-00013730: 7365 2077 6865 6e20 626f 6f74 696e 6720  se when booting 
-00013740: 696e 7374 616e 6365 732e 2020 2020 2020  instances.      
+00013630: 207c 2060 5472 7565 6020 2020 2020 2020   | `True`       
+00013640: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00013650: 6964 6c65 506f 6f6c 5368 7574 646f 776e  idlePoolShutdown
+00013660: 5469 6d65 6f75 7460 207c 2054 6865 2074  Timeout` | The t
+00013670: 696d 656f 7574 2069 6e20 6d69 6e75 7465  imeout in minute
+00013680: 7320 6166 7465 7220 7768 6963 6820 616e  s after which an
+00013690: 2069 646c 6520 576f 726b 6572 2050 6f6f   idle Worker Poo
+000136a0: 6c20 7769 6c6c 2062 6520 7368 7574 2064  l will be shut d
+000136b0: 6f77 6e20 6966 2060 6964 6c65 506f 6f6c  own if `idlePool
+000136c0: 5368 7574 646f 776e 456e 6162 6c65 6460  ShutdownEnabled`
+000136d0: 2069 7320 7365 7420 746f 2060 5472 7565   is set to `True
+000136e0: 602e 207c 2060 3330 2e30 6020 2020 2020  `. | `30.0`     
+000136f0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00013700: 2060 696d 6167 6573 4964 6020 2020 2020   `imagesId`     
+00013710: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+00013720: 2069 6d61 6765 7320 4944 2074 6f20 7573   images ID to us
+00013730: 6520 7768 656e 2062 6f6f 7469 6e67 2069  e when booting i
+00013740: 6e73 7461 6e63 6573 2e20 2020 2020 2020  nstances.       
 00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013790: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137b0: 7c0a 7c20 6069 6e73 7461 6e63 6554 6167  |.| `instanceTag
-000137c0: 7360 2020 2020 2020 2020 2020 2020 7c20  s`            | 
-000137d0: 5468 6520 6469 6374 696f 6e61 7279 206f  The dictionary o
-000137e0: 6620 696e 7374 616e 6365 2074 6167 7320  f instance tags 
-000137f0: 746f 2061 7070 6c79 2074 6f20 7468 6520  to apply to the 
-00013800: 696e 7374 616e 6365 732e 2020 2020 2020  instances.      
+00013790: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000137a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000137b0: 0a7c 2060 696e 7374 616e 6365 5461 6773  .| `instanceTags
+000137c0: 6020 2020 2020 2020 2020 2020 207c 2054  `            | T
+000137d0: 6865 2064 6963 7469 6f6e 6172 7920 6f66  he dictionary of
+000137e0: 2069 6e73 7461 6e63 6520 7461 6773 2074   instance tags t
+000137f0: 6f20 6170 706c 7920 746f 2074 6865 2069  o apply to the i
+00013800: 6e73 7461 6e63 6573 2e20 2020 2020 2020  nstances.       
 00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00013840: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013860: 2020 7c0a 7c20 606d 696e 4e6f 6465 7360    |.| `minNodes`
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 7c20 5468 6520 6d69 6e69 6d75 6d20 6e75  | The minimum nu
-00013890: 6d62 6572 206f 6620 6e6f 6465 7320 746f  mber of nodes to
-000138a0: 2077 6869 6368 2074 6865 2057 6f72 6b65   which the Worke
-000138b0: 7220 506f 6f6c 2063 616e 2062 6520 7363  r Pool can be sc
-000138c0: 616c 6564 2064 6f77 6e2e 2020 2020 2020  aled down.      
+00013860: 207c 0a7c 2060 6d69 6e4e 6f64 6573 6020   |.| `minNodes` 
+00013870: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013880: 2054 6865 206d 696e 696d 756d 206e 756d   The minimum num
+00013890: 6265 7220 6f66 206e 6f64 6573 2074 6f20  ber of nodes to 
+000138a0: 7768 6963 6820 7468 6520 576f 726b 6572  which the Worker
+000138b0: 2050 6f6f 6c20 6361 6e20 6265 2073 6361   Pool can be sca
+000138c0: 6c65 6420 646f 776e 2e20 2020 2020 2020  led down.       
 000138d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 2020 2020 2020 2020 7c20 6030 6020            | `0` 
+000138f0: 2020 2020 2020 2020 207c 2060 3060 2020           | `0`  
 00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013910: 2020 2020 7c0a 7c20 606d 6178 4e6f 6465      |.| `maxNode
-00013920: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
-00013930: 2020 7c20 5468 6520 6d61 7869 6d75 6d20    | The maximum 
-00013940: 6e75 6d62 6572 206f 6620 6e6f 6465 7320  number of nodes 
-00013950: 746f 2077 6869 6368 2074 6865 2057 6f72  to which the Wor
-00013960: 6b65 7220 506f 6f6c 2063 616e 2062 6520  ker Pool can be 
-00013970: 7363 616c 6564 2075 702e 2020 2020 2020  scaled up.      
+00013910: 2020 207c 0a7c 2060 6d61 784e 6f64 6573     |.| `maxNodes
+00013920: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00013930: 207c 2054 6865 206d 6178 696d 756d 206e   | The maximum n
+00013940: 756d 6265 7220 6f66 206e 6f64 6573 2074  umber of nodes t
+00013950: 6f20 7768 6963 6820 7468 6520 576f 726b  o which the Work
+00013960: 6572 2050 6f6f 6c20 6361 6e20 6265 2073  er Pool can be s
+00013970: 6361 6c65 6420 7570 2e20 2020 2020 2020  caled up.       
 00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 2020 2020 2020 2020 2020 7c20 6031              | `1
-000139b0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-000139c0: 2020 2020 2020 7c0a 7c20 606e 616d 6560        |.| `name`
+000139a0: 2020 2020 2020 2020 2020 207c 2060 3160             | `1`
+000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139c0: 2020 2020 207c 0a7c 2060 6e61 6d65 6020       |.| `name` 
 000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 2020 2020 7c20 5468 6520 6e61 6d65 206f      | The name o
-000139f0: 6620 7468 6520 576f 726b 6572 2050 6f6f  f the Worker Poo
-00013a00: 6c2e 2020 2020 2020 2020 2020 2020 2020  l.              
+000139e0: 2020 207c 2054 6865 206e 616d 6520 6f66     | The name of
+000139f0: 2074 6865 2057 6f72 6b65 7220 506f 6f6c   the Worker Pool
+00013a00: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00013a60: 4175 746f 6d61 7469 6361 6c6c 7920 4765  Automatically Ge
-00013a70: 6e65 7261 7465 6420 7c0a 7c20 606e 6f64  nerated |.| `nod
-00013a80: 6542 6f6f 7454 696d 656f 7574 6020 2020  eBootTimeout`   
-00013a90: 2020 2020 2020 7c20 5468 6520 7469 6d65        | The time
-00013aa0: 2069 6e20 6d69 6e75 7465 7320 616c 6c6f   in minutes allo
-00013ab0: 7765 6420 666f 7220 6120 6e6f 6465 2074  wed for a node t
-00013ac0: 6f20 626f 6f74 2061 6e64 2072 6567 6973  o boot and regis
-00013ad0: 7465 7220 7769 7468 2074 6865 2070 6c61  ter with the pla
-00013ae0: 7466 6f72 6d2c 206f 7468 6572 7769 7365  tform, otherwise
-00013af0: 2069 7420 7769 6c6c 2062 6520 7465 726d   it will be term
-00013b00: 696e 6174 6564 2e20 2020 2020 2020 2020  inated.         
-00013b10: 7c20 6031 302e 3060 2020 2020 2020 2020  | `10.0`        
-00013b20: 2020 2020 2020 2020 2020 7c0a 7c20 6074            |.| `t
-00013b30: 6172 6765 7449 6e73 7461 6e63 6543 6f75  argetInstanceCou
-00013b40: 6e74 6020 2020 2020 7c20 5468 6520 696e  nt`     | The in
-00013b50: 6974 6961 6c20 6e75 6d62 6572 206f 6620  itial number of 
-00013b60: 6e6f 6465 7320 746f 2063 7265 6174 6520  nodes to create 
-00013b70: 666f 7220 7468 6520 576f 726b 6572 2050  for the Worker P
-00013b80: 6f6f 6c2e 2020 2020 2020 2020 2020 2020  ool.            
+00013a50: 2020 2020 2020 2020 2020 2020 207c 2041               | A
+00013a60: 7574 6f6d 6174 6963 616c 6c79 2047 656e  utomatically Gen
+00013a70: 6572 6174 6564 207c 0a7c 2060 6e6f 6465  erated |.| `node
+00013a80: 426f 6f74 5469 6d65 6f75 7460 2020 2020  BootTimeout`    
+00013a90: 2020 2020 207c 2054 6865 2074 696d 6520       | The time 
+00013aa0: 696e 206d 696e 7574 6573 2061 6c6c 6f77  in minutes allow
+00013ab0: 6564 2066 6f72 2061 206e 6f64 6520 746f  ed for a node to
+00013ac0: 2062 6f6f 7420 616e 6420 7265 6769 7374   boot and regist
+00013ad0: 6572 2077 6974 6820 7468 6520 706c 6174  er with the plat
+00013ae0: 666f 726d 2c20 6f74 6865 7277 6973 6520  form, otherwise 
+00013af0: 6974 2077 696c 6c20 6265 2074 6572 6d69  it will be termi
+00013b00: 6e61 7465 642e 2020 2020 2020 2020 207c  nated.         |
+00013b10: 2060 3130 2e30 6020 2020 2020 2020 2020   `10.0`         
+00013b20: 2020 2020 2020 2020 207c 0a7c 2060 7461           |.| `ta
+00013b30: 7267 6574 496e 7374 616e 6365 436f 756e  rgetInstanceCoun
+00013b40: 7460 2020 2020 207c 2054 6865 2069 6e69  t`     | The ini
+00013b50: 7469 616c 206e 756d 6265 7220 6f66 206e  tial number of n
+00013b60: 6f64 6573 2074 6f20 6372 6561 7465 2066  odes to create f
+00013b70: 6f72 2074 6865 2057 6f72 6b65 7220 506f  or the Worker Po
+00013b80: 6f6c 2e20 2020 2020 2020 2020 2020 2020  ol.             
 00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 2020 7c20 6031 6020 2020 2020 2020 2020    | `1`         
-00013bd0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00013be0: 6074 656d 706c 6174 6549 6460 2020 2020  `templateId`    
-00013bf0: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
-00013c00: 5965 6c6c 6f77 446f 6720 436f 6d70 7574  YellowDog Comput
-00013c10: 6520 5465 6d70 6c61 7465 2049 4420 746f  e Template ID to
-00013c20: 2075 7365 2066 6f72 2070 726f 7669 7369   use for provisi
-00013c30: 6f6e 696e 672e 2028 2a2a 5265 7175 6972  oning. (**Requir
-00013c40: 6564 2a2a 2c20 6e6f 2064 6566 6175 6c74  ed**, no default
-00013c50: 2070 726f 7669 6465 642e 2920 2020 2020   provided.)     
+00013bc0: 207c 2060 3160 2020 2020 2020 2020 2020   | `1`          
+00013bd0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00013be0: 7465 6d70 6c61 7465 4964 6020 2020 2020  templateId`     
+00013bf0: 2020 2020 2020 2020 207c 2054 6865 2059           | The Y
+00013c00: 656c 6c6f 7744 6f67 2043 6f6d 7075 7465  ellowDog Compute
+00013c10: 2054 656d 706c 6174 6520 4944 2074 6f20   Template ID to 
+00013c20: 7573 6520 666f 7220 7072 6f76 6973 696f  use for provisio
+00013c30: 6e69 6e67 2e20 282a 2a52 6571 7569 7265  ning. (**Require
+00013c40: 642a 2a2c 206e 6f20 6465 6661 756c 7420  d**, no default 
+00013c50: 7072 6f76 6964 6564 2e29 2020 2020 2020  provided.)      
 00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00013c80: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00013c90: 7c20 6075 7365 7244 6174 6160 2020 2020  | `userData`    
-00013ca0: 2020 2020 2020 2020 2020 2020 7c20 5573              | Us
-00013cb0: 6572 2044 6174 6120 746f 2062 6520 7375  er Data to be su
-00013cc0: 7070 6c69 6564 2074 6f20 696e 7374 616e  pplied to instan
-00013cd0: 6365 7320 6f6e 2062 6f6f 742e 2020 2020  ces on boot.    
+00013c70: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00013c80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00013c90: 2060 7573 6572 4461 7461 6020 2020 2020   `userData`     
+00013ca0: 2020 2020 2020 2020 2020 207c 2055 7365             | Use
+00013cb0: 7220 4461 7461 2074 6f20 6265 2073 7570  r Data to be sup
+00013cc0: 706c 6965 6420 746f 2069 6e73 7461 6e63  plied to instanc
+00013cd0: 6573 206f 6e20 626f 6f74 2e20 2020 2020  es on boot.     
 00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d20: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 7c0a 7c20 6075 7365 7244 6174 6146 696c  |.| `userDataFil
-00013d50: 6560 2020 2020 2020 2020 2020 2020 7c20  e`            | 
-00013d60: 4173 2061 626f 7665 2c20 6275 7420 7265  As above, but re
-00013d70: 6164 2074 6865 2055 7365 7220 4461 7461  ad the User Data
-00013d80: 2066 726f 6d20 7468 6520 6669 6c65 6e61   from the filena
-00013d90: 6d65 2073 7570 706c 6965 6420 696e 2074  me supplied in t
-00013da0: 6869 7320 7072 6f70 6572 7479 2e20 2020  his property.   
+00013d20: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00013d30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013d40: 0a7c 2060 7573 6572 4461 7461 4669 6c65  .| `userDataFile
+00013d50: 6020 2020 2020 2020 2020 2020 207c 2041  `            | A
+00013d60: 7320 6162 6f76 652c 2062 7574 2072 6561  s above, but rea
+00013d70: 6420 7468 6520 5573 6572 2044 6174 6120  d the User Data 
+00013d80: 6672 6f6d 2074 6865 2066 696c 656e 616d  from the filenam
+00013d90: 6520 7375 7070 6c69 6564 2069 6e20 7468  e supplied in th
+00013da0: 6973 2070 726f 7065 7274 792e 2020 2020  is property.    
 00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00013dd0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 7c0a 7c20 6075 7365 7244 6174 6146    |.| `userDataF
-00013e00: 696c 6573 6020 2020 2020 2020 2020 2020  iles`           
-00013e10: 7c20 4173 2061 626f 7665 2c20 6275 7420  | As above, but 
-00013e20: 6372 6561 7465 2074 6865 2055 7365 7220  create the User 
-00013e30: 4461 7461 2062 7920 636f 6e63 6174 656e  Data by concaten
-00013e40: 6174 696e 6720 7468 6520 636f 6e74 656e  ating the conten
-00013e50: 7473 206f 6620 7468 6520 6c69 7374 206f  ts of the list o
-00013e60: 6620 6669 6c65 6e61 6d65 7320 7375 7070  f filenames supp
-00013e70: 6c69 6564 2069 6e20 7468 6973 2070 726f  lied in this pro
-00013e80: 7065 7274 792e 2020 2020 7c20 2020 2020  perty.    |     
+00013df0: 207c 0a7c 2060 7573 6572 4461 7461 4669   |.| `userDataFi
+00013e00: 6c65 7360 2020 2020 2020 2020 2020 207c  les`           |
+00013e10: 2041 7320 6162 6f76 652c 2062 7574 2063   As above, but c
+00013e20: 7265 6174 6520 7468 6520 5573 6572 2044  reate the User D
+00013e30: 6174 6120 6279 2063 6f6e 6361 7465 6e61  ata by concatena
+00013e40: 7469 6e67 2074 6865 2063 6f6e 7465 6e74  ting the content
+00013e50: 7320 6f66 2074 6865 206c 6973 7420 6f66  s of the list of
+00013e60: 2066 696c 656e 616d 6573 2073 7570 706c   filenames suppl
+00013e70: 6965 6420 696e 2074 6869 7320 7072 6f70  ied in this prop
+00013e80: 6572 7479 2e20 2020 207c 2020 2020 2020  erty.    |      
 00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 2020 7c0a 7c20 6077 6f72 6b65 7273      |.| `workers
-00013eb0: 5065 7256 4350 5560 2020 2020 2020 2020  PerVCPU`        
-00013ec0: 2020 7c20 5468 6520 6e75 6d62 6572 206f    | The number o
-00013ed0: 6620 576f 726b 6572 7320 746f 2065 7374  f Workers to est
-00013ee0: 6162 6c69 7368 2070 6572 2076 4350 5520  ablish per vCPU 
-00013ef0: 6f6e 2065 6163 6820 6e6f 6465 2069 6e20  on each node in 
-00013f00: 7468 6520 576f 726b 6572 2050 6f6f 6c2e  the Worker Pool.
-00013f10: 2028 4f76 6572 7269 6465 7320 6077 6f72   (Overrides `wor
-00013f20: 6b65 7273 5065 724e 6f64 6560 2e29 2020  kersPerNode`.)  
-00013f30: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00013ea0: 2020 207c 0a7c 2060 776f 726b 6572 7350     |.| `workersP
+00013eb0: 6572 5643 5055 6020 2020 2020 2020 2020  erVCPU`         
+00013ec0: 207c 2054 6865 206e 756d 6265 7220 6f66   | The number of
+00013ed0: 2057 6f72 6b65 7273 2074 6f20 6573 7461   Workers to esta
+00013ee0: 626c 6973 6820 7065 7220 7643 5055 206f  blish per vCPU o
+00013ef0: 6e20 6561 6368 206e 6f64 6520 696e 2074  n each node in t
+00013f00: 6865 2057 6f72 6b65 7220 506f 6f6c 2e20  he Worker Pool. 
+00013f10: 284f 7665 7272 6964 6573 2060 776f 726b  (Overrides `work
+00013f20: 6572 7350 6572 4e6f 6465 602e 2920 2020  ersPerNode`.)   
+00013f30: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00013f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f50: 2020 2020 2020 7c0a 7c20 6077 6f72 6b65        |.| `worke
-00013f60: 7273 5065 724e 6f64 6560 2020 2020 2020  rsPerNode`      
-00013f70: 2020 2020 7c20 5468 6520 6e75 6d62 6572      | The number
-00013f80: 206f 6620 576f 726b 6572 7320 746f 2065   of Workers to e
-00013f90: 7374 6162 6c69 7368 206f 6e20 6561 6368  stablish on each
-00013fa0: 206e 6f64 6520 696e 2074 6865 2057 6f72   node in the Wor
-00013fb0: 6b65 7220 506f 6f6c 2e20 2020 2020 2020  ker Pool.       
+00013f50: 2020 2020 207c 0a7c 2060 776f 726b 6572       |.| `worker
+00013f60: 7350 6572 4e6f 6465 6020 2020 2020 2020  sPerNode`       
+00013f70: 2020 207c 2054 6865 206e 756d 6265 7220     | The number 
+00013f80: 6f66 2057 6f72 6b65 7273 2074 6f20 6573  of Workers to es
+00013f90: 7461 626c 6973 6820 6f6e 2065 6163 6820  tablish on each 
+00013fa0: 6e6f 6465 2069 6e20 7468 6520 576f 726b  node in the Work
+00013fb0: 6572 2050 6f6f 6c2e 2020 2020 2020 2020  er Pool.        
 00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00013ff0: 6031 6020 2020 2020 2020 2020 2020 2020  `1`             
-00014000: 2020 2020 2020 2020 7c0a 7c20 6077 6f72          |.| `wor
-00014010: 6b65 7250 6f6f 6c44 6174 6160 2020 2020  kerPoolData`    
-00014020: 2020 2020 2020 7c20 5468 6520 6e61 6d65        | The name
-00014030: 206f 6620 6120 6669 6c65 2063 6f6e 7461   of a file conta
-00014040: 696e 696e 6720 6120 4a53 4f4e 2064 6f63  ining a JSON doc
-00014050: 756d 656e 7420 6465 6669 6e69 6e67 2061  ument defining a
-00014060: 2057 6f72 6b65 7220 506f 6f6c 2e20 2020   Worker Pool.   
+00013fe0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00013ff0: 3160 2020 2020 2020 2020 2020 2020 2020  1`              
+00014000: 2020 2020 2020 207c 0a7c 2060 776f 726b         |.| `work
+00014010: 6572 506f 6f6c 4461 7461 6020 2020 2020  erPoolData`     
+00014020: 2020 2020 207c 2054 6865 206e 616d 6520       | The name 
+00014030: 6f66 2061 2066 696c 6520 636f 6e74 6169  of a file contai
+00014040: 6e69 6e67 2061 204a 534f 4e20 646f 6375  ning a JSON docu
+00014050: 6d65 6e74 2064 6566 696e 696e 6720 6120  ment defining a 
+00014060: 576f 726b 6572 2050 6f6f 6c2e 2020 2020  Worker Pool.    
 00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000140b0: 2020 2020 2020 2020 2020 7c0a 7c20 6077            |.| `w
-000140c0: 6f72 6b65 7254 6167 6020 2020 2020 2020  orkerTag`       
-000140d0: 2020 2020 2020 2020 7c20 5468 6520 576f          | The Wo
-000140e0: 726b 6572 2054 6167 2074 6f20 7075 626c  rker Tag to publ
-000140f0: 6973 6820 666f 7220 7468 6520 616c 6c20  ish for the all 
-00014100: 6f66 2074 6865 2057 6f72 6b65 7273 206f  of the Workers o
-00014110: 6e20 7468 6520 6e6f 6465 2e20 2020 2020  n the node.     
+00014090: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140b0: 2020 2020 2020 2020 207c 0a7c 2060 776f           |.| `wo
+000140c0: 726b 6572 5461 6760 2020 2020 2020 2020  rkerTag`        
+000140d0: 2020 2020 2020 207c 2054 6865 2057 6f72         | The Wor
+000140e0: 6b65 7220 5461 6720 746f 2070 7562 6c69  ker Tag to publi
+000140f0: 7368 2066 6f72 2074 6865 2061 6c6c 206f  sh for the all o
+00014100: 6620 7468 6520 576f 726b 6572 7320 6f6e  f the Workers on
+00014110: 2074 6865 206e 6f64 652e 2020 2020 2020   the node.      
 00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014150: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00014160: 2020 2020 2020 2020 2020 2020 7c0a 0a23              |..#
-00014170: 2320 4175 746f 6d61 7469 6320 5072 6f70  # Automatic Prop
-00014180: 6572 7469 6573 0a0a 5468 6520 6e61 6d65  erties..The name
-00014190: 206f 6620 7468 6520 576f 726b 6572 2050   of the Worker P
-000141a0: 6f6f 6c2c 2069 6620 6e6f 7420 7375 7070  ool, if not supp
-000141b0: 6c69 6564 2c20 6973 2061 7574 6f6d 6174  lied, is automat
-000141c0: 6963 616c 6c79 2067 656e 6572 6174 6564  ically generated
-000141d0: 2075 7369 6e67 2061 2063 6f6e 6361 7465   using a concate
-000141e0: 6e61 7469 6f6e 206f 6620 6077 705f 602c  nation of `wp_`,
-000141f0: 2074 6865 2060 7461 6760 2070 726f 7065   the `tag` prope
-00014200: 7274 792c 2061 2055 5443 2074 696d 6573  rty, a UTC times
-00014210: 7461 6d70 2c20 616e 6420 7468 7265 6520  tamp, and three 
-00014220: 7261 6e64 6f6d 2068 6578 2063 6861 7261  random hex chara
-00014230: 6374 6572 733a 2065 2c67 2c2e 2060 7770  cters: e,g,. `wp
-00014240: 5f6d 7974 6167 5f32 3231 3032 342d 3135  _mytag_221024-15
-00014250: 3535 3234 2d62 3061 602e 0a0a 2323 2054  5524-b0a`...## T
-00014260: 4f4d 4c20 5072 6f70 6572 7469 6573 2069  OML Properties i
-00014270: 6e20 7468 6520 6077 6f72 6b65 7250 6f6f  n the `workerPoo
-00014280: 6c60 2053 6563 7469 6f6e 0a0a 4865 7265  l` Section..Here
-00014290: 2773 2061 6e20 6578 616d 706c 6520 6f66  's an example of
-000142a0: 2074 6865 2060 776f 726b 6572 506f 6f6c   the `workerPool
-000142b0: 6020 7365 6374 696f 6e20 6f66 2061 2054  ` section of a T
-000142c0: 4f4d 4c20 636f 6e66 6967 7572 6174 696f  OML configuratio
-000142d0: 6e20 6669 6c65 2c20 7368 6f77 696e 6720  n file, showing 
-000142e0: 616c 6c20 7468 6520 706f 7373 6962 6c65  all the possible
-000142f0: 2070 726f 7065 7274 6965 7320 7468 6174   properties that
-00014300: 2063 616e 2062 6520 7365 743a 0a0a 6060   can be set:..``
-00014310: 6074 6f6d 6c0a 5b77 6f72 6b65 7250 6f6f  `toml.[workerPoo
-00014320: 6c5d 0a20 2020 2069 646c 654e 6f64 6553  l].    idleNodeS
-00014330: 6875 7464 6f77 6e45 6e61 626c 6564 203d  hutdownEnabled =
-00014340: 2074 7275 650a 2020 2020 6964 6c65 4e6f   true.    idleNo
-00014350: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
-00014360: 7420 3d20 3130 2e30 0a20 2020 2069 646c  t = 10.0.    idl
-00014370: 6550 6f6f 6c53 6875 7464 6f77 6e45 6e61  ePoolShutdownEna
-00014380: 626c 6564 203d 2074 7275 650a 2020 2020  bled = true.    
-00014390: 6964 6c65 506f 6f6c 5368 7574 646f 776e  idlePoolShutdown
-000143a0: 5469 6d65 6f75 7420 3d20 3630 2e30 0a20  Timeout = 60.0. 
-000143b0: 2020 2069 6d61 6765 7349 6420 3d20 2279     imagesId = "y
-000143c0: 6469 643a 696d 6766 616d 3a30 3030 3030  did:imgfam:00000
-000143d0: 303a 3431 3936 3235 3932 2d35 3737 632d  0:41962592-577c-
-000143e0: 3466 6465 2d61 6230 332d 6438 3532 3436  4fde-ab03-d85246
-000143f0: 3565 3766 3862 220a 2020 2020 696e 7374  5e7f8b".    inst
-00014400: 616e 6365 5461 6773 203d 207b 7d0a 2020  anceTags = {}.  
-00014410: 2020 6d61 784e 6f64 6573 203d 2031 0a20    maxNodes = 1. 
-00014420: 2020 206d 696e 4e6f 6465 7320 3d20 310a     minNodes = 1.
-00014430: 2020 2020 6e61 6d65 203d 2022 6d79 2d77      name = "my-w
-00014440: 6f72 6b65 722d 706f 6f6c 220a 2020 2020  orker-pool".    
-00014450: 6e6f 6465 426f 6f74 5469 6d65 6f75 7420  nodeBootTimeout 
-00014460: 3d20 350a 2020 2020 7461 7267 6574 496e  = 5.    targetIn
-00014470: 7374 616e 6365 436f 756e 7420 3d20 310a  stanceCount = 1.
-00014480: 2020 2020 7465 6d70 6c61 7465 4964 203d      templateId =
-00014490: 2022 7964 6964 3a63 7274 3a44 3943 3534   "ydid:crt:D9C54
-000144a0: 383a 3436 3561 3130 3763 2d37 6365 612d  8:465a107c-7cea-
-000144b0: 3436 6533 2d39 6664 642d 3135 3131 3663  46e3-9fdd-15116c
-000144c0: 6239 3263 3430 220a 2020 2020 2320 4e6f  b92c40".    # No
-000144d0: 7465 3a20 6f6e 6c79 206f 6e65 206f 6620  te: only one of 
-000144e0: 2775 7365 7244 6174 6127 2f27 7573 6572  'userData'/'user
-000144f0: 4461 7461 4669 6c65 272f 2775 7365 7244  DataFile'/'userD
-00014500: 6174 6146 696c 6573 2720 7368 6f75 6c64  ataFiles' should
-00014510: 2062 6520 7365 740a 2020 2020 7573 6572   be set.    user
-00014520: 4461 7461 203d 2022 220a 2020 2020 7573  Data = "".    us
-00014530: 6572 4461 7461 4669 6c65 203d 2022 6d79  erDataFile = "my
-00014540: 7573 6572 6461 7461 2e74 7874 220a 2020  userdata.txt".  
-00014550: 2020 7573 6572 4461 7461 4669 6c65 7320    userDataFiles 
-00014560: 3d20 5b22 6d79 7573 6572 6461 7461 312e  = ["myuserdata1.
-00014570: 7478 7422 2c20 226d 7975 7365 7264 6174  txt", "myuserdat
-00014580: 6132 2e74 7874 225d 0a20 2020 2077 6f72  a2.txt"].    wor
-00014590: 6b65 7254 6167 203d 2022 7461 672d 7b7b  kerTag = "tag-{{
-000145a0: 7573 6572 6e61 6d65 7d7d 220a 2020 2020  username}}".    
-000145b0: 2320 5370 6563 6966 7920 6569 7468 6572  # Specify either
-000145c0: 2077 6f72 6b65 7273 5065 724e 6f64 6520   workersPerNode 
-000145d0: 6f72 2077 6f72 6b65 7273 5065 7256 4350  or workersPerVCP
-000145e0: 550a 2020 2020 776f 726b 6572 7350 6572  U.    workersPer
-000145f0: 4e6f 6465 203d 2031 0a20 2020 2077 6f72  Node = 1.    wor
-00014600: 6b65 7273 5065 7256 4350 5520 3d20 310a  kersPerVCPU = 1.
-00014610: 2320 2020 776f 726b 6572 506f 6f6c 4461  #   workerPoolDa
-00014620: 7461 203d 2022 776f 726b 6572 5f70 6f6f  ta = "worker_poo
-00014630: 6c2e 6a73 6f6e 220a 6060 600a 0a23 2320  l.json".```..## 
-00014640: 576f 726b 6572 2050 6f6f 6c20 5370 6563  Worker Pool Spec
-00014650: 6966 6963 6174 696f 6e20 5573 696e 6720  ification Using 
-00014660: 4a53 4f4e 2044 6f63 756d 656e 7473 0a0a  JSON Documents..
-00014670: 4974 2773 2061 6c73 6f20 706f 7373 6962  It's also possib
-00014680: 6c65 2074 6f20 6361 7074 7572 6520 6120  le to capture a 
-00014690: 576f 726b 6572 2050 6f6f 6c20 6465 6669  Worker Pool defi
-000146a0: 6e69 7469 6f6e 2061 7320 6120 4a53 4f4e  nition as a JSON
-000146b0: 2064 6f63 756d 656e 742e 2054 6865 204a   document. The J
-000146c0: 534f 4e20 6669 6c65 6e61 6d65 2063 616e  SON filename can
-000146d0: 2062 6520 7375 7070 6c69 6564 2065 6974   be supplied eit
-000146e0: 6865 7220 7573 696e 6720 7468 6520 636f  her using the co
-000146f0: 6d6d 616e 6420 6c69 6e65 2077 6974 6820  mmand line with 
-00014700: 7468 6520 602d 2d77 6f72 6b65 722d 706f  the `--worker-po
-00014710: 6f6c 6020 6f72 2060 2d70 6020 7061 7261  ol` or `-p` para
-00014720: 6d65 7465 7220 7769 7468 2060 7964 2d70  meter with `yd-p
-00014730: 726f 7669 7369 6f6e 602c 206f 7220 6279  rovision`, or by
-00014740: 2070 6f70 756c 6174 696e 6720 7468 6520   populating the 
-00014750: 6077 6f72 6b65 7250 6f6f 6c44 6174 6160  `workerPoolData`
-00014760: 2070 726f 7065 7274 7920 696e 2074 6865   property in the
-00014770: 2054 4f4d 4c20 636f 6e66 6967 7572 6174   TOML configurat
-00014780: 696f 6e20 6669 6c65 2077 6974 6820 7468  ion file with th
-00014790: 6520 4a53 4f4e 2066 696c 656e 616d 652e  e JSON filename.
-000147a0: 2043 6f6d 6d61 6e64 206c 696e 6520 7370   Command line sp
-000147b0: 6563 6966 6963 6174 696f 6e20 7461 6b65  ecification take
-000147c0: 7320 7072 696f 7269 7479 206f 7665 7220  s priority over 
-000147d0: 544f 4d4c 2073 7065 6369 6669 6361 7469  TOML specificati
-000147e0: 6f6e 2e0a 0a54 6865 204a 534f 4e20 7370  on...The JSON sp
-000147f0: 6563 6966 6963 6174 696f 6e20 616c 6c6f  ecification allo
-00014800: 7773 2074 6865 2063 7265 6174 696f 6e20  ws the creation 
-00014810: 6f66 202a 2a41 6476 616e 6365 6420 576f  of **Advanced Wo
-00014820: 726b 6572 2050 6f6f 6c73 2a2a 2c20 7769  rker Pools**, wi
-00014830: 7468 2064 6966 6665 7265 6e74 206e 6f64  th different nod
-00014840: 6520 7479 7065 7320 616e 6420 7468 6520  e types and the 
-00014850: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
-00014860: 6679 204e 6f64 6520 4163 7469 6f6e 732e  fy Node Actions.
-00014870: 0a0a 5768 656e 2075 7369 6e67 2061 204a  ..When using a J
-00014880: 534f 4e20 646f 6375 6d65 6e74 2074 6f20  SON document to 
-00014890: 7370 6563 6966 7920 7468 6520 576f 726b  specify the Work
-000148a0: 6572 2050 6f6f 6c2c 2074 6865 2073 6368  er Pool, the sch
-000148b0: 656d 6120 6f66 2074 6865 2064 6f63 756d  ema of the docum
-000148c0: 656e 7420 6973 2069 6465 6e74 6963 616c  ent is identical
-000148d0: 2074 6f20 7468 6174 2065 7870 6563 7465   to that expecte
-000148e0: 6420 6279 2074 6865 2059 656c 6c6f 7744  d by the YellowD
-000148f0: 6f67 2052 4553 5420 4150 4920 666f 7220  og REST API for 
-00014900: 576f 726b 6572 2050 6f6f 6c20 5072 6f76  Worker Pool Prov
-00014910: 6973 696f 6e69 6e67 2e0a 0a23 2323 2057  isioning...### W
-00014920: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
-00014930: 4578 616d 706c 6573 0a0a 5468 6520 6578  Examples..The ex
-00014940: 616d 706c 6520 6265 6c6f 7720 6973 206f  ample below is o
-00014950: 6620 6120 7369 6d70 6c65 204a 534f 4e20  f a simple JSON 
-00014960: 7370 6563 6966 6963 6174 696f 6e20 6f66  specification of
-00014970: 2061 2057 6f72 6b65 7220 506f 6f6c 2077   a Worker Pool w
-00014980: 6974 6820 6f6e 6520 696e 6974 6961 6c20  ith one initial 
-00014990: 6e6f 6465 2c20 576f 726b 6572 2050 6f6f  node, Worker Poo
-000149a0: 6c20 7368 7574 646f 776e 2c20 6574 632e  l shutdown, etc.
-000149b0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2272  ..```json.{.  "r
-000149c0: 6571 7569 7265 6d65 6e74 5465 6d70 6c61  equirementTempla
-000149d0: 7465 5573 6167 6522 3a20 7b0a 2020 2020  teUsage": {.    
-000149e0: 226d 6169 6e74 6169 6e49 6e73 7461 6e63  "maintainInstanc
-000149f0: 6543 6f75 6e74 223a 2066 616c 7365 2c0a  eCount": false,.
-00014a00: 2020 2020 2272 6571 7569 7265 6d65 6e74      "requirement
-00014a10: 4e61 6d65 223a 2022 7770 5f70 7965 782d  Name": "wp_pyex-
-00014a20: 7072 696d 6573 5f32 3330 3131 332d 3136  primes_230113-16
-00014a30: 3135 3238 2d64 6130 222c 0a20 2020 2022  1528-da0",.    "
-00014a40: 7265 7175 6972 656d 656e 744e 616d 6573  requirementNames
-00014a50: 7061 6365 223a 2022 7079 6578 616d 706c  pace": "pyexampl
-00014a60: 6573 222c 0a20 2020 2022 7265 7175 6972  es",.    "requir
-00014a70: 656d 656e 7454 6167 223a 2022 7079 6578  ementTag": "pyex
-00014a80: 2d70 7269 6d65 7322 2c0a 2020 2020 2274  -primes",.    "t
-00014a90: 6172 6765 7449 6e73 7461 6e63 6543 6f75  argetInstanceCou
-00014aa0: 6e74 223a 2031 2c0a 2020 2020 2274 656d  nt": 1,.    "tem
-00014ab0: 706c 6174 6549 6422 3a20 2279 6469 643a  plateId": "ydid:
-00014ac0: 6372 743a 4439 4335 3438 3a34 3635 6131  crt:D9C548:465a1
-00014ad0: 3037 632d 3763 6561 2d34 3665 332d 3966  07c-7cea-46e3-9f
-00014ae0: 6464 2d31 3531 3136 6362 3932 6334 3022  dd-15116cb92c40"
-00014af0: 0a20 207d 2c0a 2020 2270 726f 7669 7369  .  },.  "provisi
-00014b00: 6f6e 6564 5072 6f70 6572 7469 6573 223a  onedProperties":
-00014b10: 207b 0a20 2020 2022 6964 6c65 4e6f 6465   {.    "idleNode
-00014b20: 5368 7574 646f 776e 223a 207b 2265 6e61  Shutdown": {"ena
-00014b30: 626c 6564 223a 2074 7275 652c 2022 7469  bled": true, "ti
-00014b40: 6d65 6f75 7422 3a20 2250 5431 304d 227d  meout": "PT10M"}
-00014b50: 2c0a 2020 2020 2269 646c 6550 6f6f 6c53  ,.    "idlePoolS
-00014b60: 6875 7464 6f77 6e22 3a20 7b22 656e 6162  hutdown": {"enab
-00014b70: 6c65 6422 3a20 7472 7565 2c20 2274 696d  led": true, "tim
-00014b80: 656f 7574 223a 2022 5054 3148 227d 2c0a  eout": "PT1H"},.
-00014b90: 2020 2020 2263 7265 6174 654e 6f64 6557      "createNodeW
-00014ba0: 6f72 6b65 7273 223a 207b 2274 6172 6765  orkers": {"targe
-00014bb0: 7443 6f75 6e74 223a 2031 2c20 2274 6172  tCount": 1, "tar
-00014bc0: 6765 7454 7970 6522 3a20 2250 4552 5f56  getType": "PER_V
-00014bd0: 4350 5522 7d2c 0a20 2020 2022 6d61 784e  CPU"},.    "maxN
-00014be0: 6f64 6573 223a 2035 2c0a 2020 2020 226d  odes": 5,.    "m
-00014bf0: 696e 4e6f 6465 7322 3a20 302c 0a20 2020  inNodes": 0,.   
-00014c00: 2022 6e6f 6465 426f 6f74 5469 6d65 6f75   "nodeBootTimeou
-00014c10: 7422 3a20 2250 5435 4d22 2c0a 2020 2020  t": "PT5M",.    
-00014c20: 226e 6f64 6549 646c 6547 7261 6365 5065  "nodeIdleGracePe
-00014c30: 7269 6f64 223a 2022 5054 334d 222c 0a20  riod": "PT3M",. 
-00014c40: 2020 2022 6e6f 6465 4964 6c65 5469 6d65     "nodeIdleTime
-00014c50: 4c69 6d69 7422 3a20 2250 5433 4d22 2c0a  Limit": "PT3M",.
-00014c60: 2020 2020 2277 6f72 6b65 7254 6167 223a      "workerTag":
-00014c70: 2022 7079 6578 2d62 6173 682d 646f 636b   "pyex-bash-dock
-00014c80: 6572 220a 2020 7d0a 7d0a 6060 600a 0a54  er".  }.}.```..T
-00014c90: 6865 206e 6578 7420 6578 616d 706c 6520  he next example 
-00014ca0: 6973 206f 6620 6120 7265 6c61 7469 7665  is of a relative
-00014cb0: 6c79 2072 6963 6820 4a53 4f4e 2073 7065  ly rich JSON spe
-00014cc0: 6369 6669 6361 7469 6f6e 206f 6620 616e  cification of an
-00014cd0: 2041 6476 616e 6365 6420 576f 726b 6572   Advanced Worker
-00014ce0: 2050 6f6f 6c2c 2066 726f 6d20 6f6e 6520   Pool, from one 
-00014cf0: 6f66 2074 6865 2059 656c 6c6f 7744 6f67  of the YellowDog
-00014d00: 2064 656d 6f73 2e20 4974 2069 6e63 6c75   demos. It inclu
-00014d10: 6465 7320 6e6f 6465 2073 7065 6369 616c  des node special
-00014d20: 6973 6174 696f 6e2c 2061 6e64 2061 6374  isation, and act
-00014d30: 696f 6e20 6772 6f75 7073 2074 6861 7420  ion groups that 
-00014d40: 7265 7370 6f6e 6420 746f 2074 6865 2060  respond to the `
-00014d50: 5354 4152 5455 505f 4e4f 4445 535f 4144  STARTUP_NODES_AD
-00014d60: 4445 4460 2061 6e64 2060 4e4f 4445 535f  DED` and `NODES_
-00014d70: 4144 4445 4460 2065 7665 6e74 7320 746f  ADDED` events to
-00014d80: 2064 7269 7665 202a 2a4e 6f64 6520 4163   drive **Node Ac
-00014d90: 7469 6f6e 732a 2a2e 0a0a 6060 606a 736f  tions**...```jso
-00014da0: 6e0a 7b0a 2020 2272 6571 7569 7265 6d65  n.{.  "requireme
-00014db0: 6e74 5465 6d70 6c61 7465 5573 6167 6522  ntTemplateUsage"
-00014dc0: 3a20 7b0a 2020 2020 226d 6169 6e74 6169  : {.    "maintai
-00014dd0: 6e49 6e73 7461 6e63 6543 6f75 6e74 223a  nInstanceCount":
-00014de0: 2066 616c 7365 2c0a 2020 2020 2274 6172   false,.    "tar
-00014df0: 6765 7449 6e73 7461 6e63 6543 6f75 6e74  getInstanceCount
-00014e00: 223a 2036 2c0a 2020 2020 2274 656d 706c  ": 6,.    "templ
-00014e10: 6174 6549 6422 3a20 2279 6469 643a 6372  ateId": "ydid:cr
-00014e20: 743a 4439 4335 3438 3a61 3765 6461 3238  t:D9C548:a7eda28
-00014e30: 372d 6639 6436 2d34 6263 382d 6232 6463  7-f9d6-4bc8-b2dc
-00014e40: 2d34 3535 3334 3430 3537 3235 3722 2c0a  -455344057257",.
-00014e50: 2020 2020 2272 6571 7569 7265 6d65 6e74      "requirement
-00014e60: 4e61 6d65 223a 2022 7770 5f70 7965 782d  Name": "wp_pyex-
-00014e70: 736c 7572 6d5f 3233 3031 3133 2d31 3635  slurm_230113-165
-00014e80: 3631 352d 3262 3722 2c0a 2020 2020 2272  615-2b7",.    "r
-00014e90: 6571 7569 7265 6d65 6e74 4e61 6d65 7370  equirementNamesp
-00014ea0: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
-00014eb0: 7322 2c0a 2020 2020 2272 6571 7569 7265  s",.    "require
-00014ec0: 6d65 6e74 5461 6722 3a20 2270 7965 782d  mentTag": "pyex-
-00014ed0: 736c 7572 6d22 0a20 207d 2c0a 2020 2270  slurm".  },.  "p
-00014ee0: 726f 7669 7369 6f6e 6564 5072 6f70 6572  rovisionedProper
-00014ef0: 7469 6573 223a 207b 0a20 2020 2022 6372  ties": {.    "cr
-00014f00: 6561 7465 4e6f 6465 576f 726b 6572 7322  eateNodeWorkers"
-00014f10: 3a20 7b22 7461 7267 6574 436f 756e 7422  : {"targetCount"
-00014f20: 3a20 302c 2022 7461 7267 6574 5479 7065  : 0, "targetType
-00014f30: 223a 2022 5045 525f 4e4f 4445 227d 2c0a  ": "PER_NODE"},.
-00014f40: 2020 2020 226e 6f64 6543 6f6e 6669 6775      "nodeConfigu
-00014f50: 7261 7469 6f6e 223a 207b 0a20 2020 2020  ration": {.     
-00014f60: 2022 6e6f 6465 5479 7065 7322 3a20 5b0a   "nodeTypes": [.
-00014f70: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00014f80: 2022 736c 7572 6d63 746c 6422 2c20 2263   "slurmctld", "c
-00014f90: 6f75 6e74 223a 2031 7d2c 0a20 2020 2020  ount": 1},.     
-00014fa0: 2020 207b 226e 616d 6522 3a20 2273 6c75     {"name": "slu
-00014fb0: 726d 6422 2c20 226d 696e 223a 2035 2c20  rmd", "min": 5, 
-00014fc0: 2273 6c6f 744e 756d 6265 7269 6e67 223a  "slotNumbering":
-00014fd0: 2022 5245 5553 4142 4c45 227d 0a20 2020   "REUSABLE"}.   
-00014fe0: 2020 205d 2c0a 2020 2020 2020 226e 6f64     ],.      "nod
-00014ff0: 6545 7665 6e74 7322 3a20 7b0a 2020 2020  eEvents": {.    
-00015000: 2020 2020 2253 5441 5254 5550 5f4e 4f44      "STARTUP_NOD
-00015010: 4553 5f41 4444 4544 223a 205b 0a20 2020  ES_ADDED": [.   
-00015020: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00015030: 2020 2020 2022 6163 7469 6f6e 7322 3a20       "actions": 
-00015040: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00015050: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00015060: 2020 2261 6374 696f 6e22 3a20 2257 5249    "action": "WRI
-00015070: 5445 5f46 494c 4522 2c0a 2020 2020 2020  TE_FILE",.      
-00015080: 2020 2020 2020 2020 2020 2270 6174 6822            "path"
-00015090: 3a20 226e 6f64 6573 2e6a 736f 6e22 2c0a  : "nodes.json",.
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2263 6f6e 7465 6e74 223a 2022 7b5c 6e20  "content": "{\n 
-000150c0: 205c 226e 6f64 6573 5c22 3a20 5b5c 6e7b   \"nodes\": [\n{
-000150d0: 7b23 6f74 6865 724e 6f64 6573 7d7d 5c6e  {#otherNodes}}\n
-000150e0: 2020 2020 7b5c 6e20 2020 2020 205c 226e      {\n      \"n
-000150f0: 616d 655c 223a 205c 2273 6c75 726d 647b  ame\": \"slurmd{
-00015100: 7b64 6574 6169 6c73 2e6e 6f64 6553 6c6f  {details.nodeSlo
-00015110: 747d 7d5c 222c 5c6e 2020 2020 2020 5c22  t}}\",\n      \"
-00015120: 6970 5c22 3a20 5c22 7b7b 6465 7461 696c  ip\": \"{{detail
-00015130: 732e 7072 6976 6174 6549 7041 6464 7265  s.privateIpAddre
-00015140: 7373 7d7d 5c22 5c6e 2020 2020 7d7b 7b5e  ss}}\"\n    }{{^
-00015150: 2d6c 6173 747d 7d2c 7b7b 2f2d 6c61 7374  -last}},{{/-last
-00015160: 7d7d 5c6e 7b7b 2f6f 7468 6572 4e6f 6465  }}\n{{/otherNode
-00015170: 737d 7d5c 6e20 205d 5c6e 7d22 2c0a 2020  s}}\n  ]\n}",.  
-00015180: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00015190: 6f64 6554 7970 6573 223a 205b 2273 6c75  odeTypes": ["slu
-000151a0: 726d 6374 6c64 225d 0a20 2020 2020 2020  rmctld"].       
-000151b0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000151c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000151d0: 2020 2020 2020 2020 2020 2261 6374 696f            "actio
-000151e0: 6e22 3a20 2252 554e 5f43 4f4d 4d41 4e44  n": "RUN_COMMAND
-000151f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00015200: 2020 2022 7061 7468 223a 2022 7374 6172     "path": "star
-00015210: 745f 7369 6d70 6c65 5f73 6c75 726d 6374  t_simple_slurmct
-00015220: 6c64 222c 0a20 2020 2020 2020 2020 2020  ld",.           
-00015230: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
-00015240: 3a20 5b22 6e6f 6465 732e 6a73 6f6e 225d  : ["nodes.json"]
-00015250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015260: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
-00015270: 207b 2245 5841 4d50 4c45 223a 2022 464f   {"EXAMPLE": "FO
-00015280: 4f22 7d2c 0a20 2020 2020 2020 2020 2020  O"},.           
-00015290: 2020 2020 2022 6e6f 6465 5479 7065 7322       "nodeTypes"
-000152a0: 3a20 5b22 736c 7572 6d63 746c 6422 5d0a  : ["slurmctld"].
-000152b0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-000152c0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-000152d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000152e0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-000152f0: 2020 2022 6163 7469 6f6e 7322 3a20 5b0a     "actions": [.
-00015300: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015320: 2261 6374 696f 6e22 3a20 2252 554e 5f43  "action": "RUN_C
-00015330: 4f4d 4d41 4e44 222c 0a20 2020 2020 2020  OMMAND",.       
-00015340: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
-00015350: 2022 7374 6172 745f 7369 6d70 6c65 5f73   "start_simple_s
-00015360: 6c75 726d 6422 2c0a 2020 2020 2020 2020  lurmd",.        
-00015370: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00015380: 7473 223a 205b 227b 7b6e 6f64 6573 4279  ts": ["{{nodesBy
-00015390: 5479 7065 2e73 6c75 726d 6374 6c64 2e30  Type.slurmctld.0
-000153a0: 2e64 6574 6169 6c73 2e70 7269 7661 7465  .details.private
-000153b0: 4970 4164 6472 6573 737d 7d22 2c20 227b  IpAddress}}", "{
-000153c0: 7b6e 6f64 652e 6465 7461 696c 732e 6e6f  {node.details.no
-000153d0: 6465 536c 6f74 7d7d 225d 2c0a 2020 2020  deSlot}}"],.    
-000153e0: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
-000153f0: 6554 7970 6573 223a 205b 2273 6c75 726d  eTypes": ["slurm
-00015400: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-00015410: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00015420: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
-00015430: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00015440: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
-00015450: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00015460: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00015470: 2020 2020 2261 6374 696f 6e22 3a20 2243      "action": "C
-00015480: 5245 4154 455f 574f 524b 4552 5322 2c0a  REATE_WORKERS",.
-00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154a0: 2274 6f74 616c 576f 726b 6572 7322 3a20  "totalWorkers": 
-000154b0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000154c0: 2020 2022 6e6f 6465 5479 7065 7322 3a20     "nodeTypes": 
-000154d0: 5b22 736c 7572 6d63 746c 6422 5d0a 2020  ["slurmctld"].  
-000154e0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000154f0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00015500: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00015510: 5d2c 0a20 2020 2020 2020 2022 4e4f 4445  ],.        "NODE
-00015520: 535f 4144 4445 4422 3a20 5b0a 2020 2020  S_ADDED": [.    
-00015530: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00015540: 2020 2020 2261 6374 696f 6e73 223a 205b      "actions": [
-00015550: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00015560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015570: 2022 6163 7469 6f6e 223a 2022 5752 4954   "action": "WRIT
-00015580: 455f 4649 4c45 222c 0a20 2020 2020 2020  E_FILE",.       
-00015590: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
-000155a0: 2022 6e6f 6465 732e 6a73 6f6e 222c 0a20   "nodes.json",. 
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000155c0: 636f 6e74 656e 7422 3a20 227b 5c6e 2020  content": "{\n  
-000155d0: 5c22 6e6f 6465 735c 223a 205b 5c6e 7b7b  \"nodes\": [\n{{
-000155e0: 2366 696c 7465 7265 644e 6f64 6573 7d7d  #filteredNodes}}
-000155f0: 5c6e 2020 2020 7b5c 6e20 2020 2020 205c  \n    {\n      \
-00015600: 226e 616d 655c 223a 205c 2273 6c75 726d  "name\": \"slurm
-00015610: 647b 7b64 6574 6169 6c73 2e6e 6f64 6553  d{{details.nodeS
-00015620: 6c6f 747d 7d5c 222c 5c6e 2020 2020 2020  lot}}\",\n      
-00015630: 5c22 6970 5c22 3a20 5c22 7b7b 6465 7461  \"ip\": \"{{deta
-00015640: 696c 732e 7072 6976 6174 6549 7041 6464  ils.privateIpAdd
-00015650: 7265 7373 7d7d 5c22 5c6e 2020 2020 7d7b  ress}}\"\n    }{
-00015660: 7b5e 2d6c 6173 747d 7d2c 7b7b 2f2d 6c61  {^-last}},{{/-la
-00015670: 7374 7d7d 5c6e 7b7b 2f66 696c 7465 7265  st}}\n{{/filtere
-00015680: 644e 6f64 6573 7d7d 5c6e 2020 5d5c 6e7d  dNodes}}\n  ]\n}
-00015690: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000156a0: 2020 2022 6e6f 6465 5479 7065 7322 3a20     "nodeTypes": 
-000156b0: 5b22 736c 7572 6d63 746c 6422 5d0a 2020  ["slurmctld"].  
-000156c0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000156d0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-000156e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000156f0: 6163 7469 6f6e 223a 2022 5255 4e5f 434f  action": "RUN_CO
-00015700: 4d4d 414e 4422 2c0a 2020 2020 2020 2020  MMAND",.        
-00015710: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
-00015720: 2261 6464 5f6e 6f64 6573 222c 0a20 2020  "add_nodes",.   
-00015730: 2020 2020 2020 2020 2020 2020 2022 6172               "ar
-00015740: 6775 6d65 6e74 7322 3a20 5b22 6e6f 6465  guments": ["node
-00015750: 732e 6a73 6f6e 225d 2c0a 2020 2020 2020  s.json"],.      
-00015760: 2020 2020 2020 2020 2020 226e 6f64 6554            "nodeT
-00015770: 7970 6573 223a 205b 2273 6c75 726d 6374  ypes": ["slurmct
-00015780: 6c64 225d 0a20 2020 2020 2020 2020 2020  ld"].           
-00015790: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-000157a0: 205d 0a20 2020 2020 2020 2020 207d 2c0a   ].          },.
-000157b0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-000157c0: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
-000157d0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
-000157e0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-000157f0: 2020 2020 2022 6163 7469 6f6e 223a 2022       "action": "
-00015800: 5255 4e5f 434f 4d4d 414e 4422 2c0a 2020  RUN_COMMAND",.  
-00015810: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00015820: 6174 6822 3a20 2273 7461 7274 5f73 696d  ath": "start_sim
-00015830: 706c 655f 736c 7572 6d64 222c 0a20 2020  ple_slurmd",.   
-00015840: 2020 2020 2020 2020 2020 2020 2022 6172               "ar
-00015850: 6775 6d65 6e74 7322 3a20 5b22 7b7b 6e6f  guments": ["{{no
-00015860: 6465 7342 7954 7970 652e 736c 7572 6d63  desByType.slurmc
-00015870: 746c 642e 302e 6465 7461 696c 732e 7072  tld.0.details.pr
-00015880: 6976 6174 6549 7041 6464 7265 7373 7d7d  ivateIpAddress}}
-00015890: 222c 2022 7b7b 6e6f 6465 2e64 6574 6169  ", "{{node.detai
-000158a0: 6c73 2e6e 6f64 6553 6c6f 747d 7d22 5d2c  ls.nodeSlot}}"],
-000158b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000158c0: 2022 6e6f 6465 4964 4669 6c74 6572 223a   "nodeIdFilter":
-000158d0: 2022 4556 454e 5422 2c0a 2020 2020 2020   "EVENT",.      
-000158e0: 2020 2020 2020 2020 2020 226e 6f64 6554            "nodeT
-000158f0: 7970 6573 223a 205b 2273 6c75 726d 6422  ypes": ["slurmd"
-00015900: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015910: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
-00015920: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00015930: 2020 2020 5d0a 2020 2020 2020 7d0a 2020      ].      }.  
-00015940: 2020 7d2c 0a20 2020 2022 776f 726b 6572    },.    "worker
-00015950: 5461 6722 3a20 2270 7965 782d 736c 7572  Tag": "pyex-slur
-00015960: 6d2d 636c 7573 7465 7222 0a20 207d 0a7d  m-cluster".  }.}
-00015970: 0a60 6060 0a0a 2323 2320 544f 4d4c 2050  .```..### TOML P
-00015980: 726f 7065 7274 6965 7320 496e 6865 7269  roperties Inheri
-00015990: 7465 6420 6279 2057 6f72 6b65 7220 506f  ted by Worker Po
-000159a0: 6f6c 204a 534f 4e20 5370 6563 6966 6963  ol JSON Specific
-000159b0: 6174 696f 6e73 0a0a 5768 656e 2061 204a  ations..When a J
-000159c0: 534f 4e20 576f 726b 6572 2050 6f6f 6c20  SON Worker Pool 
-000159d0: 7370 6563 6966 6963 6174 696f 6e20 6973  specification is
-000159e0: 2075 7365 642c 2074 6865 2066 6f6c 6c6f   used, the follo
-000159f0: 7769 6e67 2070 726f 7065 7274 6965 7320  wing properties 
-00015a00: 6672 6f6d 2074 6865 2060 636f 6e66 6967  from the `config
-00015a10: 2e74 6f6d 6c60 2066 696c 6520 7769 6c6c  .toml` file will
-00015a20: 2062 6520 696e 6865 7269 7465 6420 6966   be inherited if
-00015a30: 2074 6865 2076 616c 7565 2069 7320 6162   the value is ab
-00015a40: 7365 6e74 2069 6e20 7468 6520 4a53 4f4e  sent in the JSON
-00015a50: 2066 696c 653a 0a0a 2a2a 5072 6f70 6572   file:..**Proper
-00015a60: 7469 6573 2049 6e68 6572 6974 6564 2077  ties Inherited w
-00015a70: 6974 6869 6e20 7468 6520 6072 6571 7569  ithin the `requi
-00015a80: 7265 6d65 6e74 5465 6d70 6c61 7465 5573  rementTemplateUs
-00015a90: 6167 6560 2070 726f 7065 7274 792a 2a0a  age` property**.
-00015aa0: 0a2d 2060 696d 6167 6573 4964 600a 2d20  .- `imagesId`.- 
-00015ab0: 6069 6e73 7461 6e63 6554 6167 7360 0a2d  `instanceTags`.-
-00015ac0: 2060 7265 7175 6972 656d 656e 744e 616d   `requirementNam
-00015ad0: 6560 3a20 6465 7269 7665 6420 6672 6f6d  e`: derived from
-00015ae0: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
-00015af0: 6572 7479 2069 6e20 7468 6520 6054 4f4d  erty in the `TOM
-00015b00: 4c60 2063 6f6e 6669 6775 7261 7469 6f6e  L` configuration
-00015b10: 2e20 2854 6865 206e 616d 6520 7769 6c6c  . (The name will
-00015b20: 2062 6520 6765 6e65 7261 7465 6420 6175   be generated au
-00015b30: 746f 6d61 7469 6361 6c6c 7920 6966 206e  tomatically if n
-00015b40: 6f74 2073 7570 706c 6965 6420 696e 2065  ot supplied in e
-00015b50: 6974 6865 7220 7468 6520 544f 4d4c 2066  ither the TOML f
-00015b60: 696c 6520 6f72 2074 6865 204a 534f 4e20  ile or the JSON 
-00015b70: 7370 6563 6966 6963 6174 696f 6e2e 290a  specification.).
-00015b80: 2d20 6072 6571 7569 7265 6d65 6e74 4e61  - `requirementNa
-00015b90: 6d65 7370 6163 6560 3a20 6465 7269 7665  mespace`: derive
-00015ba0: 6420 6672 6f6d 2074 6865 2060 6e61 6d65  d from the `name
-00015bb0: 7370 6163 6560 2070 726f 7065 7274 7920  space` property 
-00015bc0: 696e 2074 6865 2060 544f 4d4c 6020 636f  in the `TOML` co
-00015bd0: 6e66 6967 7572 6174 696f 6e0a 2d20 6072  nfiguration.- `r
-00015be0: 6571 7569 7265 6d65 6e74 5461 6760 3a20  equirementTag`: 
-00015bf0: 3a20 6465 7269 7665 6420 6672 6f6d 2074  : derived from t
-00015c00: 6865 2060 7461 6760 2070 726f 7065 7274  he `tag` propert
-00015c10: 7920 696e 2074 6865 2060 544f 4d4c 6020  y in the `TOML` 
-00015c20: 636f 6e66 6967 7572 6174 696f 6e0a 2d20  configuration.- 
-00015c30: 6074 6172 6765 7449 6e73 7461 6e63 6543  `targetInstanceC
-00015c40: 6f75 6e74 600a 2d20 6074 656d 706c 6174  ount`.- `templat
-00015c50: 6549 6460 0a2d 2060 7573 6572 4461 7461  eId`.- `userData
-00015c60: 600a 2d20 6075 7365 7244 6174 6146 696c  `.- `userDataFil
-00015c70: 6560 0a2d 2060 7573 6572 4461 7461 4669  e`.- `userDataFi
-00015c80: 6c65 7360 0a0a 2a2a 5072 6f70 6572 7469  les`..**Properti
-00015c90: 6573 2049 6e68 6572 6974 6564 2077 6974  es Inherited wit
-00015ca0: 6869 6e20 7468 6520 6070 726f 7669 7369  hin the `provisi
-00015cb0: 6f6e 6564 5072 6f70 6572 7469 6573 6020  onedProperties` 
-00015cc0: 5072 6f70 6572 7479 2a2a 0a0a 2d20 6069  Property**..- `i
-00015cd0: 646c 654e 6f64 6553 6875 7464 6f77 6e45  dleNodeShutdownE
-00015ce0: 6e61 626c 6564 600a 2d20 6069 646c 654e  nabled`.- `idleN
-00015cf0: 6f64 6553 6875 7464 6f77 6e54 696d 656f  odeShutdownTimeo
-00015d00: 7574 600a 2d20 6069 646c 6550 6f6f 6c53  ut`.- `idlePoolS
-00015d10: 6875 7464 6f77 6e45 6e61 626c 6564 600a  hutdownEnabled`.
-00015d20: 2d20 6069 646c 6550 6f6f 6c53 6875 7464  - `idlePoolShutd
-00015d30: 6f77 6e54 696d 656f 7574 600a 2d20 606e  ownTimeout`.- `n
-00015d40: 6f64 6542 6f6f 7454 696d 656f 7574 600a  odeBootTimeout`.
-00015d50: 2d20 6077 6f72 6b65 7254 6167 600a 0a23  - `workerTag`..#
-00015d60: 2320 5661 7269 6162 6c65 2053 7562 7374  # Variable Subst
-00015d70: 6974 7574 696f 6e73 2069 6e20 576f 726b  itutions in Work
-00015d80: 6572 2050 6f6f 6c20 5072 6f70 6572 7469  er Pool Properti
-00015d90: 6573 0a0a 5661 7269 6162 6c65 2073 7562  es..Variable sub
-00015da0: 7374 6974 7574 696f 6e73 2063 616e 2062  stitutions can b
-00015db0: 6520 7573 6564 2077 6974 6869 6e20 616e  e used within an
-00015dc0: 7920 7072 6f70 6572 7479 2076 616c 7565  y property value
-00015dd0: 2069 6e20 544f 4d4c 2063 6f6e 6669 6775   in TOML configu
-00015de0: 7261 7469 6f6e 2066 696c 6573 206f 7220  ration files or 
-00015df0: 576f 726b 6572 2050 6f6f 6c20 4a53 4f4e  Worker Pool JSON
-00015e00: 2066 696c 6573 2e20 5365 6520 7468 6520   files. See the 
-00015e10: 6465 7363 7269 7074 696f 6e20 5b61 626f  description [abo
-00015e20: 7665 5d28 2376 6172 6961 626c 652d 7375  ve](#variable-su
-00015e30: 6273 7469 7475 7469 6f6e 7329 2066 6f72  bstitutions) for
-00015e40: 206d 6f72 6520 6465 7461 696c 7320 6f6e   more details on
-00015e50: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-00015e60: 7475 7469 6f6e 732e 2054 6869 7320 6973  tutions. This is
-00015e70: 2061 2070 6f77 6572 6675 6c20 6665 6174   a powerful feat
-00015e80: 7572 6520 7468 6174 2061 6c6c 6f77 7320  ure that allows 
-00015e90: 576f 726b 6572 2050 6f6f 6c73 2074 6f20  Worker Pools to 
-00015ea0: 6265 2070 6172 616d 6574 6572 6973 6564  be parameterised
-00015eb0: 2062 7920 7375 7070 6c79 696e 6720 7661   by supplying va
-00015ec0: 6c75 6573 206f 6e20 7468 6520 636f 6d6d  lues on the comm
-00015ed0: 616e 6420 6c69 6e65 2c20 7669 6120 656e  and line, via en
-00015ee0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00015ef0: 6c65 732c 206f 7220 7669 6120 7468 6520  les, or via the 
-00015f00: 544f 4d4c 2066 696c 652e 0a0a 416e 2069  TOML file...An i
-00015f10: 6d70 6f72 7461 6e74 2064 6973 7469 6e63  mportant distinc
-00015f20: 7469 6f6e 202a 2a6f 6e6c 792a 2a20 7768  tion **only** wh
-00015f30: 656e 2075 7369 6e67 2076 6172 6961 626c  en using variabl
-00015f40: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
-00015f50: 7769 7468 696e 2057 6f72 6b65 7220 506f  within Worker Po
-00015f60: 6f6c 204a 534f 4e20 646f 6375 6d65 6e74  ol JSON document
-00015f70: 7320 6973 2074 6861 7420 6561 6368 2064  s is that each d
-00015f80: 6972 6563 7469 7665 202a 2a6d 7573 7420  irective **must 
-00015f90: 6265 2070 7265 6365 6465 6420 6279 2061  be preceded by a
-00015fa0: 2060 5f5f 6020 2864 6f75 626c 6520 756e   `__` (double un
-00015fb0: 6465 7273 636f 7265 292a 2a20 746f 2064  derscore)** to d
-00015fc0: 6973 616d 6269 6775 6174 6520 6974 2066  isambiguate it f
-00015fd0: 726f 6d20 7661 7269 6162 6c65 2073 7562  rom variable sub
-00015fe0: 7374 6974 7574 696f 6e73 2074 6861 7420  stitutions that 
-00015ff0: 6172 6520 746f 2062 6520 7061 7373 6564  are to be passed
-00016000: 2064 6972 6563 746c 7920 746f 2074 6865   directly to the
-00016010: 2041 5049 2e20 466f 7220 6578 616d 706c   API. For exampl
-00016020: 652c 2075 7365 3a20 605f 5f7b 7b75 7365  e, use: `__{{use
-00016030: 726e 616d 657d 7d60 2074 6f20 6170 706c  rname}}` to appl
-00016040: 7920 6120 7375 6273 7469 7475 7469 6f6e  y a substitution
-00016050: 2066 6f72 2074 6865 2060 7573 6572 6e61   for the `userna
-00016060: 6d65 6020 6465 6661 756c 7420 7375 6273  me` default subs
-00016070: 7469 7475 7469 6f6e 2e0a 0a23 2320 4472  titution...## Dr
-00016080: 792d 5275 6e6e 696e 6720 576f 726b 6572  y-Running Worker
-00016090: 2050 6f6f 6c20 5072 6f76 6973 696f 6e69   Pool Provisioni
-000160a0: 6e67 0a0a 546f 2065 7861 6d69 6e65 2074  ng..To examine t
-000160b0: 6865 204a 534f 4e20 7468 6174 2077 696c  he JSON that wil
-000160c0: 6c20 6163 7475 616c 6c79 2062 6520 7365  l actually be se
-000160d0: 6e74 2074 6f20 7468 6520 5965 6c6c 6f77  nt to the Yellow
-000160e0: 446f 6720 4150 4920 6166 7465 7220 616c  Dog API after al
-000160f0: 6c20 7072 6f63 6573 7369 6e67 2c20 7573  l processing, us
-00016100: 6520 7468 6520 602d 2d64 7279 2d72 756e  e the `--dry-run
-00016110: 6020 636f 6d6d 616e 6420 6c69 6e65 206f  ` command line o
-00016120: 7074 696f 6e20 7768 656e 2072 756e 6e69  ption when runni
-00016130: 6e67 2060 7964 2d70 726f 7669 7369 6f6e  ng `yd-provision
-00016140: 602e 2054 6869 7320 7769 6c6c 2070 7269  `. This will pri
-00016150: 6e74 2074 6865 204a 534f 4e20 7370 6563  nt the JSON spec
-00016160: 6966 6963 6174 696f 6e20 666f 7220 7468  ification for th
-00016170: 6520 576f 726b 6572 2050 6f6f 6c2e 204e  e Worker Pool. N
-00016180: 6f74 6869 6e67 2077 696c 6c20 6265 2073  othing will be s
-00016190: 7562 6d69 7474 6564 2074 6f20 7468 6520  ubmitted to the 
-000161a0: 706c 6174 666f 726d 2e0a 0a54 6865 2067  platform...The g
-000161b0: 656e 6572 6174 6564 204a 534f 4e20 6973  enerated JSON is
-000161c0: 2070 726f 6475 6365 6420 6166 7465 7220   produced after 
-000161d0: 616c 6c20 7072 6f63 6573 7369 6e67 2028  all processing (
-000161e0: 696e 636f 7270 6f72 6174 696e 6720 6063  incorporating `c
-000161f0: 6f6e 6669 672e 746f 6d6c 6020 7072 6f70  onfig.toml` prop
-00016200: 6572 7469 6573 2c20 7661 7269 6162 6c65  erties, variable
-00016210: 2073 7562 7374 6974 7574 696f 6e73 2c20   substitutions, 
-00016220: 6574 632e 2920 6861 7320 6265 656e 2063  etc.) has been c
-00016230: 6f6e 636c 7564 6564 2c20 736f 2074 6865  oncluded, so the
-00016240: 2064 7279 2d72 756e 2069 7320 7573 6566   dry-run is usef
-00016250: 756c 2066 6f72 2069 6e73 7065 6374 696e  ul for inspectin
-00016260: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
-00016270: 2061 6c6c 2074 6865 2070 726f 6365 7373   all the process
-00016280: 696e 6720 7468 6174 2773 2062 6565 6e20  ing that's been 
-00016290: 7065 7266 6f72 6d65 642e 0a0a 546f 2073  performed...To s
-000162a0: 7570 7072 6573 7320 616c 6c20 6f75 7470  uppress all outp
-000162b0: 7574 2065 7863 6570 7420 666f 7220 7468  ut except for th
-000162c0: 6520 4a53 4f4e 2069 7473 656c 662c 2075  e JSON itself, u
-000162d0: 7365 2074 6865 2060 2d2d 7175 6965 7460  se the `--quiet`
-000162e0: 2028 602d 7160 2920 636f 6d6d 616e 6420   (`-q`) command 
-000162f0: 6c69 6e65 206f 7074 696f 6e2e 0a0a 5468  line option...Th
-00016300: 6520 4a53 4f4e 2064 7279 2d72 756e 206f  e JSON dry-run o
-00016310: 7574 7075 7420 636f 756c 6420 6974 7365  utput could itse
-00016320: 6c66 2062 6520 7573 6564 2062 7920 6079  lf be used by `y
-00016330: 642d 7072 6f76 6973 696f 6e60 2c20 6966  d-provision`, if
-00016340: 2063 6170 7475 7265 6420 696e 2061 2066   captured in a f
-00016350: 696c 652c 2065 2e67 2e3a 0a0a 6060 6073  ile, e.g.:..```s
-00016360: 6865 6c6c 0a79 642d 7072 6f76 6973 696f  hell.yd-provisio
-00016370: 6e20 2d2d 6472 792d 7275 6e20 2d71 203e  n --dry-run -q >
-00016380: 206d 795f 776f 726b 6572 5f70 6f6f 6c2e   my_worker_pool.
-00016390: 6a73 6f6e 0a79 642d 7072 6f76 6973 696f  json.yd-provisio
-000163a0: 6e20 2d70 206d 795f 776f 726b 6572 5f70  n -p my_worker_p
-000163b0: 6f6f 6c2e 6a73 6f6e 0a60 6060 0a0a 2320  ool.json.```..# 
-000163c0: 4a73 6f6e 6e65 7420 5375 7070 6f72 740a  Jsonnet Support.
-000163d0: 0a49 6e20 616c 6c20 6369 7263 756d 7374  .In all circumst
-000163e0: 616e 6365 7320 7768 6572 6520 4a53 4f4e  ances where JSON
-000163f0: 2066 696c 6573 2061 7265 2075 7365 6420   files are used 
-00016400: 6279 2074 6865 2050 7974 686f 6e20 4578  by the Python Ex
-00016410: 616d 706c 6573 2073 6372 6970 7473 2c20  amples scripts, 
-00016420: 202a 2a5b 4a73 6f6e 6e65 745d 2868 7474   **[Jsonnet](htt
-00016430: 7073 3a2f 2f6a 736f 6e6e 6574 2e6f 7267  ps://jsonnet.org
-00016440: 292a 2a20 6669 6c65 7320 6361 6e20 6265  )** files can be
-00016450: 2075 7365 6420 696e 7374 6561 642e 2054   used instead. T
-00016460: 6869 7320 616c 6c6f 7773 2074 6865 2075  his allows the u
-00016470: 7365 206f 6620 4a73 6f6e 6e65 7427 7320  se of Jsonnet's 
-00016480: 706f 7765 7266 756c 204a 534f 4e20 6578  powerful JSON ex
-00016490: 7465 6e73 696f 6e73 2c20 696e 636c 7564  tensions, includ
-000164a0: 696e 6720 636f 6d6d 656e 7473 2c20 7661  ing comments, va
-000164b0: 7269 6162 6c65 732c 2066 756e 6374 696f  riables, functio
-000164c0: 6e73 2c20 6574 632e 0a0a 4120 7369 6d70  ns, etc...A simp
-000164d0: 6c65 2075 7361 6765 2065 7861 6d70 6c65  le usage example
-000164e0: 206d 6967 6874 2062 653a 0a0a 6060 6073   might be:..```s
-000164f0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
-00016500: 2d77 6f72 6b2d 7265 7175 6972 656d 656e  -work-requiremen
-00016510: 7420 6d79 5f77 6f72 6b5f 7265 712e 6a73  t my_work_req.js
-00016520: 6f6e 6e65 740a 6060 600a 0a54 6865 2075  onnet.```..The u
-00016530: 7365 206f 6620 7468 6520 6669 6c65 6e61  se of the filena
-00016540: 6d65 2065 7874 656e 7369 6f6e 2060 2e6a  me extension `.j
-00016550: 736f 6e6e 6574 6020 7769 6c6c 2069 6e76  sonnet` will inv
-00016560: 6f6b 6520 4a73 6f6e 6e65 7420 6576 616c  oke Jsonnet eval
-00016570: 7561 7469 6f6e 2e20 284e 6f74 6520 7468  uation. (Note th
-00016580: 6174 2061 2074 656d 706f 7261 7279 204a  at a temporary J
-00016590: 534f 4e20 6669 6c65 2069 7320 6372 6561  SON file is crea
-000165a0: 7465 6420 6173 2070 6172 7420 6f66 204a  ted as part of J
-000165b0: 736f 6e6e 6574 2070 726f 6365 7373 696e  sonnet processin
-000165c0: 672c 2077 6869 6368 2079 6f75 206d 6179  g, which you may
-000165d0: 2073 6565 2072 6566 6572 7265 6420 746f   see referred to
-000165e0: 2069 6e20 6572 726f 7220 6d65 7373 6167   in error messag
-000165f0: 6573 3a20 7468 6973 2066 696c 6520 7769  es: this file wi
-00016600: 6c6c 2068 6176 6520 6265 656e 2064 656c  ll have been del
-00016610: 6574 6564 2062 6566 6f72 6520 7468 6520  eted before the 
-00016620: 7363 7269 7074 2073 746f 7073 2e29 0a0a  script stops.)..
-00016630: 2323 204a 736f 6e6e 6574 2049 6e73 7461  ## Jsonnet Insta
-00016640: 6c6c 6174 696f 6e0a 0a4a 736f 6e6e 6574  llation..Jsonnet
-00016650: 2069 7320 2a2a 6e6f 742a 2a20 696e 7374   is **not** inst
-00016660: 616c 6c65 6420 6279 2064 6566 6175 6c74  alled by default
-00016670: 2077 6865 6e20 6079 656c 6c6f 7764 6f67   when `yellowdog
-00016680: 2d70 7974 686f 6e2d 6578 616d 706c 6573  -python-examples
-00016690: 6020 6973 2069 6e73 7461 6c6c 6564 2c20  ` is installed, 
-000166a0: 6265 6361 7573 6520 7468 6520 7061 636b  because the pack
-000166b0: 6167 6520 6861 7320 6269 6e61 7279 2063  age has binary c
-000166c0: 6f6d 706f 6e65 6e74 7320 7768 6963 6820  omponents which 
-000166d0: 6172 6520 6e6f 7420 6176 6169 6c61 626c  are not availabl
-000166e0: 6520 6f6e 2050 7950 4920 666f 7220 616c  e on PyPI for al
-000166f0: 6c20 706c 6174 666f 726d 732e 2049 6620  l platforms. If 
-00016700: 796f 7520 7472 7920 746f 2075 7365 2061  you try to use a
-00016710: 204a 736f 6e6e 6574 2066 696c 6520 696e   Jsonnet file in
-00016720: 2074 6865 2061 6273 656e 6365 206f 6620   the absence of 
-00016730: 4a73 6f6e 6e65 742c 2074 6865 2073 6372  Jsonnet, the scr
-00016740: 6970 7473 2077 696c 6c20 7072 696e 7420  ipts will print 
-00016750: 616e 2065 7272 6f72 206d 6573 7361 6765  an error message
-00016760: 2c20 616e 6420 7375 6767 6573 7420 616e  , and suggest an
-00016770: 2069 6e73 7461 6c6c 6174 696f 6e20 6d65   installation me
-00016780: 6368 616e 6973 6d2e 0a0a 546f 2069 6e73  chanism...To ins
-00016790: 7461 6c6c 204a 736f 6e6e 6574 2061 7420  tall Jsonnet at 
-000167a0: 7468 6520 7361 6d65 2074 696d 6520 6173  the same time as
-000167b0: 2069 6e73 7461 6c6c 696e 6720 6f72 2075   installing or u
-000167c0: 7064 6174 696e 6720 7468 6520 5079 7468  pdating the Pyth
-000167d0: 6f6e 2045 7861 6d70 6c65 7320 7363 7269  on Examples scri
-000167e0: 7074 732c 206d 6f64 6966 7920 7468 6520  pts, modify the 
-000167f0: 696e 7374 616c 6c61 7469 6f6e 2061 7320  installation as 
-00016800: 666f 6c6c 6f77 7320 746f 2069 6e63 6c75  follows to inclu
-00016810: 6465 2074 6865 2060 6a73 6f6e 6e65 7460  de the `jsonnet`
-00016820: 206f 7074 696f 6e3a 0a0a 6060 600a 7069   option:..```.pi
-00016830: 7020 696e 7374 616c 6c20 2d55 2022 7965  p install -U "ye
-00016840: 6c6c 6f77 646f 672d 7079 7468 6f6e 2d65  llowdog-python-e
-00016850: 7861 6d70 6c65 735b 6a73 6f6e 6e65 745d  xamples[jsonnet]
-00016860: 220a 6060 600a 0a54 6f20 696e 7374 616c  ".```..To instal
-00016870: 6c20 4a73 6f6e 6e65 7420 7365 7061 7261  l Jsonnet separa
-00016880: 7465 6c79 2066 726f 6d20 6079 656c 6c6f  tely from `yello
-00016890: 7764 6f67 2d70 7974 686f 6e2d 6578 616d  wdog-python-exam
-000168a0: 706c 6573 602c 2074 7279 3a0a 0a60 6060  ples`, try:..```
-000168b0: 7368 656c 6c0a 7069 7020 696e 7374 616c  shell.pip instal
-000168c0: 6c20 2d55 206a 736f 6e6e 6574 0a60 6060  l -U jsonnet.```
-000168d0: 0a0a 4966 2074 6869 7320 6661 696c 732c  ..If this fails,
-000168e0: 2074 7279 3a0a 0a60 6060 7368 656c 6c0a   try:..```shell.
-000168f0: 7069 7020 696e 7374 616c 6c20 2d55 206a  pip install -U j
-00016900: 736f 6e6e 6574 2d62 696e 6172 790a 6060  sonnet-binary.``
-00016910: 600a 0a49 6620 626f 7468 206f 6620 7468  `..If both of th
-00016920: 6573 6520 6d65 7468 6f64 7320 6661 696c  ese methods fail
-00016930: 2c20 796f 7527 6c6c 206e 6565 6420 746f  , you'll need to
-00016940: 2065 6e73 7572 6520 7468 6174 2074 6865   ensure that the
-00016950: 2070 6c61 7466 6f72 6d20 6f6e 2077 6869   platform on whi
-00016960: 6368 2079 6f75 2772 6520 7275 6e6e 696e  ch you're runnin
-00016970: 6720 6861 7320 7468 6520 7265 7175 6972  g has the requir
-00016980: 6564 2062 7569 6c64 2074 6f6f 6c73 2061  ed build tools a
-00016990: 7661 696c 6162 6c65 2c20 736f 2074 6861  vailable, so tha
-000169a0: 7420 7468 6520 4a73 6f6e 6e65 7420 6269  t the Jsonnet bi
-000169b0: 6e61 7279 2063 6f6d 706f 6e65 6e74 7320  nary components 
-000169c0: 6361 6e20 6265 2062 7569 6c74 206c 6f63  can be built loc
-000169d0: 616c 6c79 2e20 5468 6520 7265 7175 6972  ally. The requir
-000169e0: 6564 2062 7569 6c64 2070 6163 6b61 6765  ed build package
-000169f0: 7320 7661 7279 2062 7920 706c 6174 666f  s vary by platfo
-00016a00: 726d 2062 7574 2075 7375 616c 6c79 2069  rm but usually i
-00016a10: 6e63 6c75 6465 2067 656e 6572 616c 2064  nclude general d
-00016a20: 6576 656c 6f70 6d65 6e74 2074 6f6f 6c73  evelopment tools
-00016a30: 2069 6e63 6c75 6469 6e67 2061 2043 2b2b   including a C++
-00016a40: 2063 6f6d 7069 6c65 722c 2061 6e64 2050   compiler, and P
-00016a50: 7974 686f 6e20 6465 7665 6c6f 706d 656e  ython developmen
-00016a60: 7420 746f 6f6c 7320 696e 636c 7564 696e  t tools includin
-00016a70: 6720 7468 6520 5079 7468 6f6e 2068 6561  g the Python hea
-00016a80: 6465 7273 2e0a 0a50 6c65 6173 6520 6765  ders...Please ge
-00016a90: 7420 696e 2074 6f75 6368 2077 6974 6820  t in touch with 
-00016aa0: 5965 6c6c 6f77 446f 6720 6966 2079 6f75  YellowDog if you
-00016ab0: 2067 6574 2073 7475 636b 2e0a 0a23 2320   get stuck...## 
-00016ac0: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
-00016ad0: 7574 696f 6e73 2069 6e20 4a73 6f6e 6e65  utions in Jsonne
-00016ae0: 7420 4669 6c65 730a 0a54 6865 2073 6372  t Files..The scr
-00016af0: 6970 7473 2070 726f 7669 6465 2066 756c  ipts provide ful
-00016b00: 6c20 7375 7070 6f72 7420 666f 7220 7661  l support for va
-00016b10: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-00016b20: 696f 6e73 2069 6e20 4a73 6f6e 6e65 7420  ions in Jsonnet 
-00016b30: 6669 6c65 732c 2075 7369 6e67 2074 6865  files, using the
-00016b40: 2073 616d 6520 7275 6c65 7320 6173 2066   same rules as f
-00016b50: 6f72 2074 6865 204a 534f 4e20 7370 6563  or the JSON spec
-00016b60: 6966 6963 6174 696f 6e73 2e20 5265 6d65  ifications. Reme
-00016b70: 6d62 6572 2074 6861 7420 666f 7220 2a2a  mber that for **
-00016b80: 576f 726b 6572 2050 6f6f 6c2a 2a20 7370  Worker Pool** sp
-00016b90: 6563 6966 6963 6174 696f 6e73 2c20 7661  ecifications, va
-00016ba0: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-00016bb0: 696f 6e73 206d 7573 7420 6265 2070 7265  ions must be pre
-00016bc0: 6669 7865 6420 6279 2060 5f5f 602c 2065  fixed by `__`, e
-00016bd0: 2e67 2e20 6022 5f5f 7b7b 7573 6572 6e61  .g. `"__{{userna
-00016be0: 6d65 7d7d 7d22 602e 0a0a 5661 7269 6162  me}}}"`...Variab
-00016bf0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
-00016c00: 6973 2070 6572 666f 726d 6564 2062 6566  is performed bef
-00016c10: 6f72 6520 4a73 6f6e 6e65 7420 6578 7061  ore Jsonnet expa
-00016c20: 6e73 696f 6e20 696e 746f 204a 534f 4e2c  nsion into JSON,
-00016c30: 2061 6e64 2061 6761 696e 2061 6674 6572   and again after
-00016c40: 2074 6865 2065 7870 616e 7369 6f6e 2e0a   the expansion..
-00016c50: 0a23 2320 4368 6563 6b69 6e67 204a 736f  .## Checking Jso
-00016c60: 6e6e 6574 2050 726f 6365 7373 696e 670a  nnet Processing.
-00016c70: 0a54 6865 7265 2061 7265 2074 6872 6565  .There are three
-00016c80: 2070 6f73 7369 6269 6c69 7469 6573 2066   possibilities f
-00016c90: 6f72 2076 6572 6966 7969 6e67 2074 6861  or verifying tha
-00016ca0: 7420 6120 4a73 6f6e 6e65 7420 7370 6563  t a Jsonnet spec
-00016cb0: 6966 6963 6174 696f 6e20 6973 2064 6f69  ification is doi
-00016cc0: 6e67 2077 6861 7420 6973 2069 6e74 656e  ng what is inten
-00016cd0: 6465 643a 0a0a 312e 2054 6f20 696e 7370  ded:..1. To insp
-00016ce0: 6563 7420 7468 6520 6261 7369 6320 636f  ect the basic co
-00016cf0: 6e76 6572 7369 6f6e 206f 6620 4a73 6f6e  nversion of Json
-00016d00: 6e65 7420 696e 746f 204a 534f 4e2c 2077  net into JSON, w
-00016d10: 6974 686f 7574 2061 6e79 2061 6464 6974  ithout any addit
-00016d20: 696f 6e61 6c20 7072 6f63 6573 7369 6e67  ional processing
-00016d30: 2062 7920 7468 6520 5079 7468 6f6e 2045   by the Python E
-00016d40: 7861 6d70 6c65 7320 7363 7269 7074 732c  xamples scripts,
-00016d50: 2074 6865 2060 7964 2d6a 736f 6e6e 6574   the `yd-jsonnet
-00016d60: 326a 736f 6e60 2063 6f6d 6d61 6e64 2063  2json` command c
-00016d70: 616e 2062 6520 7573 6564 2e20 5468 6973  an be used. This
-00016d80: 2074 616b 6573 2061 2073 696e 676c 6520   takes a single 
-00016d90: 636f 6d6d 616e 6420 6c69 6e65 2061 7267  command line arg
-00016da0: 756d 656e 7420 7768 6963 6820 6973 2074  ument which is t
-00016db0: 6865 206e 616d 6520 6f66 2074 6865 206a  he name of the j
-00016dc0: 736f 6e6e 6574 2066 696c 6520 746f 2062  sonnet file to b
-00016dd0: 6520 7072 6f63 6573 7365 643a 0a0a 6060  e processed:..``
-00016de0: 6073 6865 6c6c 0a79 642d 6a73 6f6e 6e65  `shell.yd-jsonne
-00016df0: 7432 6a73 6f6e 206d 795f 6669 6c65 2e6a  t2json my_file.j
-00016e00: 736f 6e6e 6574 0a60 6060 0a0a 0a32 2e20  sonnet.```...2. 
-00016e10: 5468 6520 606a 736f 6e6e 6574 2d64 7279  The `jsonnet-dry
-00016e20: 2d72 756e 6020 2860 2d4a 6029 206f 7074  -run` (`-J`) opt
-00016e30: 696f 6e20 6f66 2074 6865 2060 7964 2d73  ion of the `yd-s
-00016e40: 7562 6d69 7460 2c20 6079 642d 7072 6f76  ubmit`, `yd-prov
-00016e50: 6973 696f 6e60 2061 6e64 2060 7964 2d69  ision` and `yd-i
-00016e60: 6e73 7461 6e74 6961 7465 6020 636f 6d6d  nstantiate` comm
-00016e70: 616e 6473 2077 696c 6c20 6765 6e65 7261  ands will genera
-00016e80: 7465 204a 534f 4e20 6f75 7470 7574 2072  te JSON output r
-00016e90: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00016ea0: 4a73 6f6e 6e65 7420 746f 204a 534f 4e20  Jsonnet to JSON 
-00016eb0: 7072 6f63 6573 7369 6e67 206f 6e6c 792c  processing only,
-00016ec0: 2069 6e63 6c75 6469 6e67 2061 7070 6c69   including appli
-00016ed0: 6361 626c 6520 7661 7269 6162 6c65 2073  cable variable s
-00016ee0: 7562 7374 6974 7574 696f 6e73 2c20 6275  ubstitutions, bu
-00016ef0: 7420 6265 666f 7265 2066 756c 6c20 7072  t before full pr
-00016f00: 6f70 6572 7479 2065 7870 616e 7369 6f6e  operty expansion
-00016f10: 2069 6e74 6f20 7468 6520 4a53 4f4e 2074   into the JSON t
-00016f20: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
-00016f30: 6974 7465 6420 746f 2074 6865 2050 6c61  itted to the Pla
-00016f40: 7466 6f72 6d2e 0a0a 0a33 2e20 5468 6520  tform....3. The 
-00016f50: 6064 7279 2d72 756e 6020 2860 2d44 6029  `dry-run` (`-D`)
-00016f60: 206f 7074 696f 6e20 7769 6c6c 2067 656e   option will gen
-00016f70: 6572 6174 6520 4a53 4f4e 206f 7574 7075  erate JSON outpu
-00016f80: 7420 7265 7072 6573 656e 7469 6e67 2074  t representing t
-00016f90: 6865 2066 756c 6c20 7072 6f63 6573 7369  he full processi
-00016fa0: 6e67 206f 6620 7468 6520 4a73 6f6e 6e65  ng of the Jsonne
-00016fb0: 7420 6669 6c65 2069 6e74 6f20 7768 6174  t file into what
-00016fc0: 2077 696c 6c20 6265 2073 7562 6d69 7474   will be submitt
-00016fd0: 6564 2074 6f20 7468 6520 4150 492e 2054  ed to the API. T
-00016fe0: 6869 7320 616c 6c6f 7773 2069 6e73 7065  his allows inspe
-00016ff0: 6374 696f 6e20 746f 2063 6865 636b 2074  ction to check t
-00017000: 6861 7420 7468 6520 6f75 7470 7574 206d  hat the output m
-00017010: 6174 6368 6573 2065 7870 6563 7461 7469  atches expectati
-00017020: 6f6e 732c 2070 7269 6f72 2074 6f20 7375  ons, prior to su
-00017030: 626d 6974 7469 6e67 2074 6f20 7468 6520  bmitting to the 
-00017040: 506c 6174 666f 726d 2e0a 0a23 2320 4a73  Platform...## Js
-00017050: 6f6e 6e65 7420 4578 616d 706c 650a 0a48  onnet Example..H
-00017060: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
-00017070: 206f 6620 6120 4a73 6f6e 6e65 7420 6669   of a Jsonnet fi
-00017080: 6c65 2074 6861 7420 6765 6e65 7261 7465  le that generate
-00017090: 7320 6120 576f 726b 2052 6571 7569 7265  s a Work Require
-000170a0: 6d65 6e74 2077 6974 6820 666f 7572 2054  ment with four T
-000170b0: 6173 6b73 3a0a 0a60 6060 6a73 6f6e 6e65  asks:..```jsonne
-000170c0: 740a 2320 4675 6e63 7469 6f6e 2066 6f72  t.# Function for
-000170d0: 2073 796e 7468 6573 6973 696e 6720 5461   synthesising Ta
-000170e0: 736b 730a 6c6f 6361 6c20 5461 736b 2861  sks.local Task(a
-000170f0: 7267 756d 656e 7473 3d5b 5d2c 2065 6e76  rguments=[], env
-00017100: 6972 6f6e 6d65 6e74 3d7b 7d29 203d 207b  ironment={}) = {
-00017110: 0a20 2020 2061 7267 756d 656e 7473 3a20  .    arguments: 
-00017120: 6172 6775 6d65 6e74 732c 0a20 2020 2065  arguments,.    e
-00017130: 6e76 6972 6f6e 6d65 6e74 3a20 656e 7669  nvironment: envi
-00017140: 726f 6e6d 656e 742c 0a20 2020 206e 616d  ronment,.    nam
-00017150: 653a 2022 6d79 5f74 6173 6b5f 7b7b 7461  e: "my_task_{{ta
-00017160: 736b 5f6e 756d 6265 727d 7d22 0a7d 3b0a  sk_number}}".};.
-00017170: 0a23 2057 6f72 6b20 5265 7175 6972 656d  .# Work Requirem
-00017180: 656e 740a 7b0a 2020 226e 616d 6522 3a20  ent.{.  "name": 
-00017190: 2277 6f72 6b72 6571 5f7b 7b64 6174 6574  "workreq_{{datet
-000171a0: 696d 657d 7d22 2c0a 2020 2274 6173 6b47  ime}}",.  "taskG
-000171b0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
-000171c0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
-000171d0: 0a20 2020 2020 2020 2054 6173 6b28 5b22  .        Task(["
-000171e0: 3122 5d2c 207b 413a 2022 415f 3122 7d29  1"], {A: "A_1"})
-000171f0: 2c20 2023 2061 7267 756d 656e 7473 2061  ,  # arguments a
-00017200: 6e64 2065 6e76 6972 6f6e 6d65 6e74 0a20  nd environment. 
-00017210: 2020 2020 2020 2054 6173 6b28 5b22 3222         Task(["2"
-00017220: 2c20 2233 225d 2c20 7b7d 292c 2020 2020  , "3"], {}),    
-00017230: 2023 2061 7267 756d 656e 7473 2061 6e64   # arguments and
-00017240: 2065 6d70 7479 2065 6e76 6972 6f6e 6d65   empty environme
-00017250: 6e74 0a20 2020 2020 2020 2054 6173 6b28  nt.        Task(
-00017260: 5b22 3422 5d29 2c20 2020 2020 2020 2020  ["4"]),         
-00017270: 2020 2020 2023 2061 7267 756d 656e 7473       # arguments
-00017280: 2061 6e64 2064 6566 6175 6c74 2065 6e76   and default env
-00017290: 6972 6f6e 6d65 6e74 0a20 2020 2020 2020  ironment.       
-000172a0: 2054 6173 6b28 2920 2020 2020 2020 2020   Task()         
-000172b0: 2020 2020 2020 2020 2020 2023 2064 6566             # def
-000172c0: 6175 6c74 2061 7267 756d 656e 7473 2061  ault arguments a
-000172d0: 6e64 2065 6e76 6972 6f6e 6d65 6e74 0a20  nd environment. 
-000172e0: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
-000172f0: 0a7d 0a60 6060 0a0a 5768 656e 2074 6869  .}.```..When thi
-00017300: 7320 6973 2069 6e73 7065 6374 6564 2075  s is inspected u
-00017310: 7369 6e67 2074 6865 2060 6a73 6f6e 6e65  sing the `jsonne
-00017320: 742d 6472 792d 7275 6e60 206f 7074 696f  t-dry-run` optio
-00017330: 6e20 2860 7964 2d73 7562 6d69 7420 2d4a  n (`yd-submit -J
-00017340: 7120 2d72 206d 795f 776f 726b 5f72 6571  q -r my_work_req
-00017350: 2e6a 736f 6e6e 6574 6029 2c20 7468 6973  .jsonnet`), this
-00017360: 2069 7320 7468 6520 7072 6f63 6573 7365   is the processe
-00017370: 6420 6f75 7470 7574 3a0a 0a60 6060 6a73  d output:..```js
-00017380: 6f6e 0a7b 0a20 2022 6e61 6d65 223a 2022  on.{.  "name": "
-00017390: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
-000173a0: 3430 3634 3522 2c0a 2020 2274 6173 6b47  40645",.  "taskG
-000173b0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
-000173c0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
-000173d0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-000173e0: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
-000173f0: 3a20 5b22 3122 5d2c 0a20 2020 2020 2020  : ["1"],.       
-00017400: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
-00017410: 3a20 7b22 4122 3a20 2241 5f31 227d 2c0a  : {"A": "A_1"},.
-00017420: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00017430: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
-00017440: 6b5f 6e75 6d62 6572 7d7d 220a 2020 2020  k_number}}".    
-00017450: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
-00017460: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
-00017470: 6d65 6e74 7322 3a20 5b22 3222 2c20 2233  ments": ["2", "3
-00017480: 225d 2c0a 2020 2020 2020 2020 2020 2265  "],.          "e
-00017490: 6e76 6972 6f6e 6d65 6e74 223a 207b 7d2c  nvironment": {},
-000174a0: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
-000174b0: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
-000174c0: 736b 5f6e 756d 6265 727d 7d22 0a20 2020  sk_number}}".   
-000174d0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000174e0: 7b0a 2020 2020 2020 2020 2020 2261 7267  {.          "arg
-000174f0: 756d 656e 7473 223a 205b 2234 225d 2c0a  uments": ["4"],.
-00017500: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
-00017510: 6f6e 6d65 6e74 223a 207b 7d2c 0a20 2020  onment": {},.   
-00017520: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-00017530: 6d79 5f74 6173 6b5f 7b7b 7461 736b 5f6e  my_task_{{task_n
-00017540: 756d 6265 727d 7d22 0a20 2020 2020 2020  umber}}".       
-00017550: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00017560: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00017570: 7473 223a 205b 5d2c 0a20 2020 2020 2020  ts": [],.       
-00017580: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
-00017590: 3a20 7b7d 2c0a 2020 2020 2020 2020 2020  : {},.          
-000175a0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
-000175b0: 5f7b 7b74 6173 6b5f 6e75 6d62 6572 7d7d  _{{task_number}}
-000175c0: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-000175d0: 2020 5d0a 2020 2020 7d0a 2020 5d0a 7d0a    ].    }.  ].}.
-000175e0: 6060 600a 0a57 6865 6e20 7468 6973 2069  ```..When this i
-000175f0: 7320 696e 7370 6563 7465 6420 7573 696e  s inspected usin
-00017600: 6720 7468 6520 6064 7279 2d72 756e 6020  g the `dry-run` 
-00017610: 6f70 7469 6f6e 2028 6079 642d 7375 626d  option (`yd-subm
-00017620: 6974 202d 4471 202d 7220 6d79 5f77 6f72  it -Dq -r my_wor
-00017630: 6b5f 7265 712e 6a73 6f6e 6e65 7460 292c  k_req.jsonnet`),
-00017640: 2074 6869 7320 6973 2074 6865 2070 726f   this is the pro
-00017650: 6365 7373 6564 206f 7574 7075 743a 0a0a  cessed output:..
-00017660: 6060 606a 736f 6e0a 7b0a 2020 2266 756c  ```json.{.  "ful
-00017670: 6669 6c4f 6e53 7562 6d69 7422 3a20 6661  filOnSubmit": fa
-00017680: 6c73 652c 0a20 2022 6e61 6d65 223a 2022  lse,.  "name": "
-00017690: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
-000176a0: 3430 3634 3522 2c0a 2020 226e 616d 6573  40645",.  "names
-000176b0: 7061 6365 223a 2022 7079 6578 616d 706c  pace": "pyexampl
-000176c0: 6573 222c 0a20 2022 7072 696f 7269 7479  es",.  "priority
-000176d0: 223a 2030 2c0a 2020 2274 6167 223a 2022  ": 0,.  "tag": "
-000176e0: 7079 6578 2d62 6173 6822 2c0a 2020 2274  pyex-bash",.  "t
-000176f0: 6173 6b47 726f 7570 7322 3a20 5b0a 2020  askGroups": [.  
-00017700: 2020 7b0a 2020 2020 2020 2266 696e 6973    {.      "finis
-00017710: 6849 6641 6c6c 5461 736b 7346 696e 6973  hIfAllTasksFinis
-00017720: 6865 6422 3a20 7472 7565 2c0a 2020 2020  hed": true,.    
-00017730: 2020 2266 696e 6973 6849 6641 6e79 5461    "finishIfAnyTa
-00017740: 736b 4661 696c 6564 223a 2066 616c 7365  skFailed": false
-00017750: 2c0a 2020 2020 2020 226e 616d 6522 3a20  ,.      "name": 
-00017760: 2274 6173 6b5f 6772 6f75 705f 3122 2c0a  "task_group_1",.
-00017770: 2020 2020 2020 2270 7269 6f72 6974 7922        "priority"
-00017780: 3a20 302c 0a20 2020 2020 2022 7275 6e53  : 0,.      "runS
-00017790: 7065 6369 6669 6361 7469 6f6e 223a 207b  pecification": {
-000177a0: 0a20 2020 2020 2020 2022 6d61 7869 6d75  .        "maximu
-000177b0: 6d54 6173 6b52 6574 7269 6573 223a 2030  mTaskRetries": 0
-000177c0: 2c0a 2020 2020 2020 2020 2274 6173 6b54  ,.        "taskT
-000177d0: 7970 6573 223a 205b 2262 6173 6822 5d2c  ypes": ["bash"],
-000177e0: 0a20 2020 2020 2020 2022 776f 726b 6572  .        "worker
-000177f0: 5461 6773 223a 205b 2270 7965 782d 6261  Tags": ["pyex-ba
-00017800: 7368 2d64 6f63 6b65 7222 5d0a 2020 2020  sh-docker"].    
-00017810: 2020 7d2c 0a20 2020 2020 2022 7461 736b    },.      "task
-00017820: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
-00017830: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
-00017840: 656e 7473 223a 205b 2277 6f72 6b72 6571  ents": ["workreq
-00017850: 5f32 3330 3131 342d 3134 3036 3435 2f73  _230114-140645/s
-00017860: 6c65 6570 5f73 6372 6970 742e 7368 222c  leep_script.sh",
-00017870: 2022 3122 5d2c 0a20 2020 2020 2020 2020   "1"],.         
-00017880: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
-00017890: 7b22 4122 3a20 2241 5f31 227d 2c0a 2020  {"A": "A_1"},.  
-000178a0: 2020 2020 2020 2020 2269 6e70 7574 7322          "inputs"
-000178b0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-000178c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000178d0: 226f 626a 6563 744e 616d 6550 6174 7465  "objectNamePatte
-000178e0: 726e 223a 2022 776f 726b 7265 715f 3233  rn": "workreq_23
-000178f0: 3031 3134 2d31 3430 3634 352f 736c 6565  0114-140645/slee
-00017900: 705f 7363 7269 7074 2e73 6822 2c0a 2020  p_script.sh",.  
-00017910: 2020 2020 2020 2020 2020 2020 2273 6f75              "sou
-00017920: 7263 6522 3a20 2254 4153 4b5f 4e41 4d45  rce": "TASK_NAME
-00017930: 5350 4143 4522 2c0a 2020 2020 2020 2020  SPACE",.        
-00017940: 2020 2020 2020 2276 6572 6966 6963 6174        "verificat
-00017950: 696f 6e22 3a20 2256 4552 4946 595f 4154  ion": "VERIFY_AT
-00017960: 5f53 5441 5254 220a 2020 2020 2020 2020  _START".        
-00017970: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00017980: 5d2c 0a20 2020 2020 2020 2020 2022 6e61  ],.          "na
-00017990: 6d65 223a 2022 6d79 5f74 6173 6b5f 3122  me": "my_task_1"
-000179a0: 2c0a 2020 2020 2020 2020 2020 226f 7574  ,.          "out
-000179b0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
-000179c0: 2020 2020 207b 2261 6c77 6179 7355 706c       {"alwaysUpl
-000179d0: 6f61 6422 3a20 7472 7565 2c20 2272 6571  oad": true, "req
-000179e0: 7569 7265 6422 3a20 6661 6c73 652c 2022  uired": false, "
-000179f0: 736f 7572 6365 223a 2022 5052 4f43 4553  source": "PROCES
-00017a00: 535f 4f55 5450 5554 227d 0a20 2020 2020  S_OUTPUT"}.     
-00017a10: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00017a20: 2020 2274 6173 6b54 7970 6522 3a20 2262    "taskType": "b
-00017a30: 6173 6822 0a20 2020 2020 2020 207d 2c0a  ash".        },.
-00017a40: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00017a50: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
-00017a60: 205b 2277 6f72 6b72 6571 5f32 3330 3131   ["workreq_23011
-00017a70: 342d 3134 3036 3435 2f73 6c65 6570 5f73  4-140645/sleep_s
-00017a80: 6372 6970 742e 7368 222c 2022 3222 2c20  cript.sh", "2", 
-00017a90: 2233 225d 2c0a 2020 2020 2020 2020 2020  "3"],.          
-00017aa0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-00017ab0: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
-00017ac0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
-00017ad0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00017ae0: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
-00017af0: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
-00017b00: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
-00017b10: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
-00017b20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017b30: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
-00017b40: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
-00017b50: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
-00017b60: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
-00017b70: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
-00017b80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00017b90: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00017ba0: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
-00017bb0: 736b 5f32 222c 0a20 2020 2020 2020 2020  sk_2",.         
-00017bc0: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
-00017bd0: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
-00017be0: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
-00017bf0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-00017c00: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
-00017c10: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
-00017c20: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00017c30: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
-00017c40: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
-00017c50: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00017c60: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00017c70: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
-00017c80: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
-00017c90: 6565 705f 7363 7269 7074 2e73 6822 2c20  eep_script.sh", 
-00017ca0: 2234 225d 2c0a 2020 2020 2020 2020 2020  "4"],.          
-00017cb0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-00017cc0: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
-00017cd0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
-00017ce0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00017cf0: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
-00017d00: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
-00017d10: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
-00017d20: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
-00017d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017d40: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
-00017d50: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
-00017d60: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
-00017d70: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
-00017d80: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
-00017d90: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00017da0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00017db0: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
-00017dc0: 736b 5f33 222c 0a20 2020 2020 2020 2020  sk_3",.         
-00017dd0: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
-00017de0: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
-00017df0: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
-00017e00: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-00017e10: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
-00017e20: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
-00017e30: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00017e40: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
-00017e50: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
-00017e60: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00017e70: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00017e80: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
-00017e90: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
-00017ea0: 6565 705f 7363 7269 7074 2e73 6822 5d2c  eep_script.sh"],
-00017eb0: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
-00017ec0: 726f 6e6d 656e 7422 3a20 7b7d 2c0a 2020  ronment": {},.  
-00017ed0: 2020 2020 2020 2020 2269 6e70 7574 7322          "inputs"
-00017ee0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00017ef0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00017f00: 226f 626a 6563 744e 616d 6550 6174 7465  "objectNamePatte
-00017f10: 726e 223a 2022 776f 726b 7265 715f 3233  rn": "workreq_23
-00017f20: 3031 3134 2d31 3430 3634 352f 736c 6565  0114-140645/slee
-00017f30: 705f 7363 7269 7074 2e73 6822 2c0a 2020  p_script.sh",.  
-00017f40: 2020 2020 2020 2020 2020 2020 2273 6f75              "sou
-00017f50: 7263 6522 3a20 2254 4153 4b5f 4e41 4d45  rce": "TASK_NAME
-00017f60: 5350 4143 4522 2c0a 2020 2020 2020 2020  SPACE",.        
-00017f70: 2020 2020 2020 2276 6572 6966 6963 6174        "verificat
-00017f80: 696f 6e22 3a20 2256 4552 4946 595f 4154  ion": "VERIFY_AT
-00017f90: 5f53 5441 5254 220a 2020 2020 2020 2020  _START".        
-00017fa0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00017fb0: 5d2c 0a20 2020 2020 2020 2020 2022 6e61  ],.          "na
-00017fc0: 6d65 223a 2022 6d79 5f74 6173 6b5f 3422  me": "my_task_4"
-00017fd0: 2c0a 2020 2020 2020 2020 2020 226f 7574  ,.          "out
-00017fe0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
-00017ff0: 2020 2020 207b 2261 6c77 6179 7355 706c       {"alwaysUpl
-00018000: 6f61 6422 3a20 7472 7565 2c20 2272 6571  oad": true, "req
-00018010: 7569 7265 6422 3a20 6661 6c73 652c 2022  uired": false, "
-00018020: 736f 7572 6365 223a 2022 5052 4f43 4553  source": "PROCES
-00018030: 535f 4f55 5450 5554 227d 0a20 2020 2020  S_OUTPUT"}.     
-00018040: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00018050: 2020 2274 6173 6b54 7970 6522 3a20 2262    "taskType": "b
-00018060: 6173 6822 0a20 2020 2020 2020 207d 0a20  ash".        }. 
-00018070: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
-00018080: 0a7d 0a60 6060 0a0a 2320 436f 6d6d 616e  .}.```..# Comman
-00018090: 6420 4c69 7374 0a0a 4865 6c70 2069 7320  d List..Help is 
-000180a0: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
-000180b0: 6c20 636f 6d6d 616e 6473 2062 7920 696e  l commands by in
-000180c0: 766f 6b69 6e67 2061 2063 6f6d 6d61 6e64  voking a command
-000180d0: 2077 6974 6820 7468 6520 602d 2d68 656c   with the `--hel
-000180e0: 7060 206f 7220 602d 6860 206f 7074 696f  p` or `-h` optio
-000180f0: 6e2e 2053 6f6d 6520 636f 6d6d 616e 6420  n. Some command 
-00018100: 6c69 6e65 2070 6172 616d 6574 6572 7320  line parameters 
-00018110: 6172 6520 636f 6d6d 6f6e 2074 6f20 616c  are common to al
-00018120: 6c20 636f 6d6d 616e 6473 2c20 7768 696c  l commands, whil
-00018130: 6520 6f74 6865 7273 2061 7265 2063 6f6d  e others are com
-00018140: 6d61 6e64 2d73 7065 6369 6669 632e 0a0a  mand-specific...
-00018150: 416c 6c20 6465 7374 7275 6374 6976 6520  All destructive 
-00018160: 636f 6d6d 616e 6473 2072 6571 7569 7265  commands require
-00018170: 2075 7365 7220 636f 6e66 6972 6d61 7469   user confirmati
-00018180: 6f6e 2062 6566 6f72 6520 7461 6b69 6e67  on before taking
-00018190: 2065 6666 6563 742e 2054 6869 7320 6361   effect. This ca
-000181a0: 6e20 6265 2073 7570 7072 6573 7365 6420  n be suppressed 
-000181b0: 7573 696e 6720 7468 6520 602d 2d79 6573  using the `--yes
-000181c0: 6020 6f72 2060 2d79 6020 6f70 7469 6f6e  ` or `-y` option
-000181d0: 2c20 696e 2077 6869 6368 2063 6173 6520  , in which case 
-000181e0: 7468 6520 636f 6d6d 616e 6420 7769 6c6c  the command will
-000181f0: 2070 726f 6365 6564 2077 6974 686f 7574   proceed without
-00018200: 2063 6f6e 6669 726d 6174 696f 6e2e 0a0a   confirmation...
-00018210: 536f 6d65 2063 6f6d 6d61 6e64 7320 7375  Some commands su
-00018220: 7070 6f72 7420 7468 6520 602d 2d69 6e74  pport the `--int
-00018230: 6572 6163 7469 7665 6020 6f72 2060 2d69  eractive` or `-i
-00018240: 6020 6f70 7469 6f6e 2c20 616c 6c6f 7769  ` option, allowi
-00018250: 6e67 2075 7365 7220 7365 6c65 6374 696f  ng user selectio
-00018260: 6e73 2074 6f20 6265 206d 6164 652e 2045  ns to be made. E
-00018270: 2e67 2e2c 2074 6869 7320 6361 6e20 6265  .g., this can be
-00018280: 2075 7365 6420 746f 2073 656c 6563 7420   used to select 
-00018290: 7768 6963 6820 6f62 6a65 6374 2070 6174  which object pat
-000182a0: 6873 2074 6f20 6465 6c65 7465 2e0a 0a54  hs to delete...T
-000182b0: 6865 2060 2d2d 7175 6965 7460 206f 7220  he `--quiet` or 
-000182c0: 602d 7160 206f 7074 696f 6e20 7265 6475  `-q` option redu
-000182d0: 6365 7320 7468 6520 636f 6d6d 616e 6420  ces the command 
-000182e0: 6f75 7470 7574 2064 6f77 6e20 746f 2065  output down to e
-000182f0: 7373 656e 7469 616c 206d 6573 7361 6765  ssential message
-00018300: 7320 6f6e 6c79 2e20 536f 2c20 666f 7220  s only. So, for 
-00018310: 6578 616d 706c 652c 2060 7964 2d64 656c  example, `yd-del
-00018320: 6574 6520 2d79 7160 2077 6f75 6c64 2064  ete -yq` would d
-00018330: 656c 6574 6520 616c 6c20 6d61 7463 6869  elete all matchi
-00018340: 6e67 206f 626a 6563 7420 7061 7468 7320  ng object paths 
-00018350: 7369 6c65 6e74 6c79 2e0a 0a49 6620 796f  silently...If yo
-00018360: 7520 656e 636f 756e 7465 7220 616e 2065  u encounter an e
-00018370: 7272 6f72 2069 7420 6361 6e20 6265 2075  rror it can be u
-00018380: 7365 6675 6c20 666f 7220 7375 7070 6f72  seful for suppor
-00018390: 7420 7075 7270 6f73 6573 2074 6f20 7365  t purposes to se
-000183a0: 6520 7468 6520 6675 6c6c 2050 7974 686f  e the full Pytho
-000183b0: 6e20 7374 6163 6b20 7472 6163 652e 2054  n stack trace. T
-000183c0: 6869 7320 6361 6e20 6265 2065 6e61 626c  his can be enabl
-000183d0: 6564 2062 7920 7275 6e6e 696e 6720 7468  ed by running th
-000183e0: 6520 636f 6d6d 616e 6420 7573 696e 6720  e command using 
-000183f0: 7468 6520 602d 2d64 6562 7567 6020 6f70  the `--debug` op
-00018400: 7469 6f6e 2e0a 0a23 2320 7964 2d73 7562  tion...## yd-sub
-00018410: 6d69 740a 0a54 6865 2060 7964 2d73 7562  mit..The `yd-sub
-00018420: 6d69 7460 2063 6f6d 6d61 6e64 2073 7562  mit` command sub
-00018430: 6d69 7473 2061 206e 6577 2057 6f72 6b20  mits a new Work 
-00018440: 5265 7175 6972 656d 656e 742c 2061 6363  Requirement, acc
-00018450: 6f72 6469 6e67 2074 6f20 7468 6520 576f  ording to the Wo
-00018460: 726b 2052 6571 7569 7265 6d65 6e74 2064  rk Requirement d
-00018470: 6566 696e 6974 696f 6e20 666f 756e 6420  efinition found 
-00018480: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
-00018490: 6972 656d 656e 7460 2073 6563 7469 6f6e  irement` section
-000184a0: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
-000184b0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-000184c0: 616e 642f 6f72 2074 6865 2073 7065 6369  and/or the speci
-000184d0: 6669 6361 7469 6f6e 2066 6f75 6e64 2069  fication found i
-000184e0: 6e20 6120 576f 726b 2052 6571 7569 7265  n a Work Require
-000184f0: 6d65 6e74 204a 534f 4e20 646f 6375 6d65  ment JSON docume
-00018500: 6e74 2073 7570 706c 6965 6420 7573 696e  nt supplied usin
-00018510: 6720 7468 6520 602d 2d77 6f72 6b2d 7265  g the `--work-re
-00018520: 7175 6972 656d 656e 7460 206f 7074 696f  quirement` optio
-00018530: 6e2e 0a0a 5573 6520 7468 6520 602d 2d64  n...Use the `--d
-00018540: 7279 2d72 756e 6020 6f70 7469 6f6e 2074  ry-run` option t
-00018550: 6f20 696e 7370 6563 7420 7468 6520 6465  o inspect the de
-00018560: 7461 696c 7320 6f66 2074 6865 2057 6f72  tails of the Wor
-00018570: 6b20 5265 7175 6972 656d 656e 742c 2054  k Requirement, T
-00018580: 6173 6b20 4772 6f75 7073 2c20 616e 6420  ask Groups, and 
-00018590: 5461 736b 7320 7468 6174 2077 696c 6c20  Tasks that will 
-000185a0: 6265 2073 7562 6d69 7474 6564 2c20 696e  be submitted, in
-000185b0: 204a 534f 4e20 666f 726d 6174 2e0a 0a4f   JSON format...O
-000185c0: 6e63 6520 7375 626d 6974 7465 642c 2074  nce submitted, t
-000185d0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-000185e0: 656e 7420 7769 6c6c 2061 7070 6561 7220  ent will appear 
-000185f0: 696e 2074 6865 202a 2a57 6f72 6b2a 2a20  in the **Work** 
-00018600: 7461 6220 696e 2074 6865 2059 656c 6c6f  tab in the Yello
-00018610: 7744 6f67 2050 6f72 7461 6c2e 0a0a 5468  wDog Portal...Th
-00018620: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-00018630: 6e74 2773 2070 726f 6772 6573 7320 6361  nt's progress ca
-00018640: 6e20 6265 2074 7261 636b 6564 2074 6f20  n be tracked to 
-00018650: 636f 6d70 6c65 7469 6f6e 2062 7920 7573  completion by us
-00018660: 696e 6720 7468 6520 602d 2d66 6f6c 6c6f  ing the `--follo
-00018670: 7760 2028 6f72 2060 2d66 6029 206f 7074  w` (or `-f`) opt
-00018680: 696f 6e20 7768 656e 2069 6e76 6f6b 696e  ion when invokin
-00018690: 6720 6079 642d 7375 626d 6974 603a 2074  g `yd-submit`: t
-000186a0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
-000186b0: 7265 706f 7274 206f 6e20 5461 736b 7320  report on Tasks 
-000186c0: 6173 2074 6865 7920 636f 6e63 6c75 6465  as they conclude
-000186d0: 2061 6e64 2077 6f6e 2774 2072 6574 7572   and won't retur
-000186e0: 6e20 756e 7469 6c20 7468 6520 576f 726b  n until the Work
-000186f0: 2052 6571 7569 7265 6d65 6e74 2068 6173   Requirement has
-00018700: 2066 696e 6973 6865 642e 0a0a 2323 2079   finished...## y
-00018710: 642d 7072 6f76 6973 696f 6e0a 0a54 6865  d-provision..The
-00018720: 2060 7964 2d70 726f 7669 7369 6f6e 6020   `yd-provision` 
-00018730: 636f 6d6d 616e 6420 7072 6f76 6973 696f  command provisio
-00018740: 6e73 2061 206e 6577 2057 6f72 6b65 7220  ns a new Worker 
-00018750: 506f 6f6c 2061 6363 6f72 6469 6e67 2074  Pool according t
-00018760: 6f20 7468 6520 7370 6563 6966 6963 6174  o the specificat
-00018770: 696f 6e73 2069 6e20 7468 6520 6077 6f72  ions in the `wor
-00018780: 6b65 7250 6f6f 6c60 2073 6563 7469 6f6e  kerPool` section
-00018790: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
-000187a0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-000187b0: 616e 642f 6f72 2069 6e20 7468 6520 7370  and/or in the sp
-000187c0: 6563 6966 6963 6174 696f 6e20 666f 756e  ecification foun
-000187d0: 6420 696e 2061 2057 6f72 6b65 7220 506f  d in a Worker Po
-000187e0: 6f6c 204a 534f 4e20 646f 6375 6d65 6e74  ol JSON document
-000187f0: 2073 7570 706c 6965 6420 7573 696e 6720   supplied using 
-00018800: 7468 6520 602d 2d77 6f72 6b65 722d 706f  the `--worker-po
-00018810: 6f6c 6020 6f70 7469 6f6e 2e0a 0a55 7365  ol` option...Use
-00018820: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
-00018830: 206f 7074 696f 6e20 746f 2069 6e73 7065   option to inspe
-00018840: 6374 2074 6865 2064 6574 6169 6c73 206f  ct the details o
-00018850: 6620 7468 6520 576f 726b 6572 2050 6f6f  f the Worker Poo
-00018860: 6c20 7370 6563 6966 6963 6174 696f 6e20  l specification 
-00018870: 7468 6174 2077 696c 6c20 6265 2073 7562  that will be sub
-00018880: 6d69 7474 6564 2c20 696e 204a 534f 4e20  mitted, in JSON 
-00018890: 666f 726d 6174 2e0a 0a4f 6e63 6520 7072  format...Once pr
-000188a0: 6f76 6973 696f 6e65 642c 2074 6865 2057  ovisioned, the W
-000188b0: 6f72 6b65 7220 506f 6f6c 2077 696c 6c20  orker Pool will 
-000188c0: 6170 7065 6172 2069 6e20 7468 6520 2a2a  appear in the **
-000188d0: 576f 726b 6572 732a 2a20 7461 6220 696e  Workers** tab in
-000188e0: 2074 6865 2059 656c 6c6f 7744 6f67 2050   the YellowDog P
-000188f0: 6f72 7461 6c2c 2061 6e64 2069 7473 2061  ortal, and its a
-00018900: 7373 6f63 6961 7465 6420 436f 6d70 7574  ssociated Comput
-00018910: 6520 5265 7175 6972 656d 656e 7420 7769  e Requirement wi
-00018920: 6c6c 2061 7070 6561 7220 696e 2074 6865  ll appear in the
-00018930: 202a 2a43 6f6d 7075 7465 2a2a 2074 6162   **Compute** tab
-00018940: 2e0a 0a23 2320 7964 2d63 616e 6365 6c0a  ...## yd-cancel.
-00018950: 0a54 6865 2060 7964 2d63 616e 6365 6c60  .The `yd-cancel`
-00018960: 2063 6f6d 6d61 6e64 2063 616e 6365 6c73   command cancels
-00018970: 2061 6e79 2061 6374 6976 6520 576f 726b   any active Work
-00018980: 2052 6571 7569 7265 6d65 6e74 732c 2069   Requirements, i
-00018990: 6e63 6c75 6469 6e67 2061 6e79 2070 656e  ncluding any pen
-000189a0: 6469 6e67 2054 6173 6b20 4772 6f75 7073  ding Task Groups
-000189b0: 2061 6e64 2074 6865 2054 6173 6b73 2074   and the Tasks t
-000189c0: 6865 7920 636f 6e74 6169 6e2e 200a 0a54  hey contain. ..T
-000189d0: 6865 2060 6e61 6d65 7370 6163 6560 2061  he `namespace` a
-000189e0: 6e64 2060 7461 6760 2076 616c 7565 7320  nd `tag` values 
-000189f0: 696e 2074 6865 2060 636f 6e66 6967 2e74  in the `config.t
-00018a00: 6f6d 6c60 2066 696c 6520 6172 6520 7573  oml` file are us
-00018a10: 6564 2074 6f20 6964 656e 7469 6679 2077  ed to identify w
-00018a20: 6869 6368 2057 6f72 6b20 5265 7175 6972  hich Work Requir
-00018a30: 656d 656e 7473 2074 6f20 6361 6e63 656c  ements to cancel
-00018a40: 2e0a 0a42 7920 6465 6661 756c 742c 2061  ...By default, a
-00018a50: 6e79 2054 6173 6b73 2074 6861 7420 6172  ny Tasks that ar
-00018a60: 6520 6375 7272 656e 746c 7920 7275 6e6e  e currently runn
-00018a70: 696e 6720 6f6e 2057 6f72 6b65 7273 2077  ing on Workers w
-00018a80: 696c 6c20 636f 6e74 696e 7565 2074 6f20  ill continue to 
-00018a90: 7275 6e20 746f 2063 6f6d 706c 6574 696f  run to completio
-00018aa0: 6e20 6f72 2075 6e74 696c 2074 6865 7920  n or until they 
-00018ab0: 6661 696c 2e20 5461 736b 7320 6361 6e20  fail. Tasks can 
-00018ac0: 6265 2069 6e73 7472 7563 7465 6420 746f  be instructed to
-00018ad0: 2061 626f 7274 2069 6d6d 6564 6961 7465   abort immediate
-00018ae0: 6c79 2062 7920 7375 7070 6c79 696e 6720  ly by supplying 
-00018af0: 7468 6520 602d 2d61 626f 7274 6020 6f72  the `--abort` or
-00018b00: 2060 2d61 6020 6f70 7469 6f6e 2074 6f20   `-a` option to 
-00018b10: 6079 642d 6361 6e63 656c 602e 0a0a 2323  `yd-cancel`...##
-00018b20: 2079 642d 6162 6f72 740a 0a54 6865 2060   yd-abort..The `
-00018b30: 7964 2d61 626f 7274 6020 636f 6d6d 616e  yd-abort` comman
-00018b40: 6420 6973 2075 7365 6420 746f 2061 626f  d is used to abo
-00018b50: 7274 2054 6173 6b73 2074 6861 7420 6172  rt Tasks that ar
-00018b60: 6520 6375 7272 656e 746c 7920 7275 6e6e  e currently runn
-00018b70: 696e 672e 2054 6865 2075 7365 7220 696e  ing. The user in
-00018b80: 7465 7261 6374 6976 656c 7920 7365 6c65  teractively sele
-00018b90: 6374 7320 7468 6520 576f 726b 2052 6571  cts the Work Req
-00018ba0: 7569 7265 6d65 6e74 7320 746f 2074 6172  uirements to tar
-00018bb0: 6765 742c 2061 6e64 2074 6865 6e20 7768  get, and then wh
-00018bc0: 6963 6820 5461 736b 7320 7769 7468 696e  ich Tasks within
-00018bd0: 2074 686f 7365 2057 6f72 6b20 5265 7175   those Work Requ
-00018be0: 6972 656d 656e 7473 2074 6f20 6162 6f72  irements to abor
-00018bf0: 742e 2054 6865 2057 6f72 6b20 5265 7175  t. The Work Requ
-00018c00: 6972 656d 656e 7473 2061 7265 206e 6f74  irements are not
-00018c10: 2063 616e 6365 6c6c 6564 2061 7320 7061   cancelled as pa
-00018c20: 7274 206f 6620 7468 6973 2070 726f 6365  rt of this proce
-00018c30: 7373 2e0a 0a54 6865 2060 6e61 6d65 7370  ss...The `namesp
-00018c40: 6163 6560 2061 6e64 2060 7461 6760 2076  ace` and `tag` v
-00018c50: 616c 7565 7320 696e 2074 6865 2060 636f  alues in the `co
-00018c60: 6e66 6967 2e74 6f6d 6c60 2066 696c 6520  nfig.toml` file 
-00018c70: 6172 6520 7573 6564 2074 6f20 6964 656e  are used to iden
-00018c80: 7469 6679 2077 6869 6368 2057 6f72 6b20  tify which Work 
-00018c90: 5265 7175 6972 656d 656e 7473 2074 6f20  Requirements to 
-00018ca0: 6c69 7374 2066 6f72 2073 656c 6563 7469  list for selecti
-00018cb0: 6f6e 2e0a 0a23 2320 7964 2d64 6f77 6e6c  on...## yd-downl
-00018cc0: 6f61 640a 0a54 6865 2060 7964 2d64 6f77  oad..The `yd-dow
-00018cd0: 6e6c 6f61 6460 2063 6f6d 6d61 6e64 2064  nload` command d
-00018ce0: 6f77 6e6c 6f61 6473 2061 6e79 206f 626a  ownloads any obj
-00018cf0: 6563 7473 2063 7265 6174 6564 2069 6e20  ects created in 
-00018d00: 7468 6520 5965 6c6c 6f77 446f 6720 4f62  the YellowDog Ob
-00018d10: 6a65 6374 2053 746f 7265 2e0a 0a54 6865  ject Store...The
-00018d20: 2060 6e61 6d65 7370 6163 6560 2061 6e64   `namespace` and
-00018d30: 2060 7461 6760 2076 616c 7565 7320 6172   `tag` values ar
-00018d40: 6520 7573 6564 2074 6f20 6465 7465 726d  e used to determ
-00018d50: 696e 6520 7768 6963 6820 6f62 6a65 6374  ine which object
-00018d60: 7320 746f 2064 6f77 6e6c 6f61 642e 204f  s to download. O
-00018d70: 626a 6563 7473 2077 696c 6c20 6265 2064  bjects will be d
-00018d80: 6f77 6e6c 6f61 6465 6420 746f 2061 2064  ownloaded to a d
-00018d90: 6972 6563 746f 7279 2077 6974 6820 7468  irectory with th
-00018da0: 6520 7361 6d65 206e 616d 6520 6173 2060  e same name as `
-00018db0: 6e61 6d65 7370 6163 6560 2e20 4966 2061  namespace`. If a
-00018dc0: 2064 6972 6563 746f 7279 2061 6c72 6561   directory alrea
-00018dd0: 6479 2065 7869 7374 732c 2061 206e 6577  dy exists, a new
-00018de0: 2064 6972 6563 746f 7279 2077 6974 6820   directory with 
-00018df0: 6e61 6d65 2060 3c6e 616d 6573 7061 6365  name `<namespace
-00018e00: 3e2e 3031 6020 2865 7463 2e29 2077 696c  >.01` (etc.) wil
-00018e10: 6c20 6265 2063 7265 6174 6564 2e0a 0a23  l be created...#
-00018e20: 2320 7964 2d64 656c 6574 650a 0a54 6865  # yd-delete..The
-00018e30: 2060 7964 2d64 656c 6574 6560 2063 6f6d   `yd-delete` com
-00018e40: 6d61 6e64 2064 656c 6574 6573 2061 6e79  mand deletes any
-00018e50: 206f 626a 6563 7473 2063 7265 6174 6564   objects created
-00018e60: 2069 6e20 7468 6520 5965 6c6c 6f77 446f   in the YellowDo
-00018e70: 6720 4f62 6a65 6374 2053 746f 7265 2e0a  g Object Store..
-00018e80: 0a54 6865 2060 6e61 6d65 7370 6163 6560  .The `namespace`
-00018e90: 2061 6e64 2060 7461 6760 2076 616c 7565   and `tag` value
-00018ea0: 7320 696e 2074 6865 2060 636f 6e66 6967  s in the `config
-00018eb0: 2e74 6f6d 6c60 2066 696c 6520 6172 6520  .toml` file are 
-00018ec0: 7573 6564 2074 6f20 6964 656e 7469 6679  used to identify
-00018ed0: 2077 6869 6368 206f 626a 6563 7473 2074   which objects t
-00018ee0: 6f20 6465 6c65 7465 2e20 4e6f 7465 2074  o delete. Note t
-00018ef0: 6861 7420 6974 2773 2065 6173 7920 746f  hat it's easy to
-00018f00: 2075 7365 2060 7964 2d64 656c 6574 6560   use `yd-delete`
-00018f10: 2074 6f20 636c 6561 7220 7468 6520 636f   to clear the co
-00018f20: 6e74 656e 7473 206f 6620 6120 6e61 6d65  ntents of a name
-00018f30: 7370 6163 6520 6279 2075 7369 6e67 2061  space by using a
-00018f40: 6e20 656d 7074 7920 6074 6167 602c 2061  n empty `tag`, a
-00018f50: 7320 666f 6c6c 6f77 733a 0a0a 6060 6073  s follows:..```s
-00018f60: 6865 6c6c 0a79 642d 6465 6c65 7465 202d  hell.yd-delete -
-00018f70: 7420 2222 0a60 6060 0a0a 5468 6973 2063  t "".```..This c
-00018f80: 616e 2062 6520 6578 7465 6e64 6564 2074  an be extended t
-00018f90: 6f20 616e 7920 6f74 6865 7220 6e61 6d65  o any other name
-00018fa0: 7370 6163 6520 6279 2075 7369 6e67 2074  space by using t
-00018fb0: 6865 2060 2d2d 6e61 6d65 7370 6163 6560  he `--namespace`
-00018fc0: 2f60 2d6e 6020 6f70 7469 6f6e 2e0a 0a23  /`-n` option...#
-00018fd0: 2320 7964 2d75 706c 6f61 640a 0a54 6865  # yd-upload..The
-00018fe0: 2060 7964 2d75 706c 6f61 6460 2063 6f6d   `yd-upload` com
-00018ff0: 6d61 6e64 2075 706c 6f61 6473 2066 696c  mand uploads fil
-00019000: 6573 2066 726f 6d20 7468 6520 6c6f 6361  es from the loca
-00019010: 6c20 6669 6c65 7379 7374 656d 2074 6f20  l filesystem to 
-00019020: 7468 6520 5965 6c6c 6f77 446f 6720 4f62  the YellowDog Ob
-00019030: 6a65 6374 2073 746f 7265 2e20 4669 6c65  ject store. File
-00019040: 7320 6172 6520 706c 6163 6564 2069 6e20  s are placed in 
-00019050: 7468 6520 636f 6e66 6967 7572 6564 2060  the configured `
-00019060: 6e61 6d65 7370 6163 6560 2077 6974 6869  namespace` withi
-00019070: 6e20 6120 6469 7265 6374 6f72 7920 7375  n a directory su
-00019080: 7070 6c69 6564 2075 7369 6e67 2074 6865  pplied using the
-00019090: 2028 7265 7175 6972 6564 2920 602d 2d64   (required) `--d
-000190a0: 6972 6563 746f 7279 6020 6f70 7469 6f6e  irectory` option
-000190b0: 2c20 652e 672e 3a0a 0a60 6060 7368 656c  , e.g.:..```shel
-000190c0: 6c0a 7964 2d75 706c 6f61 6420 2d2d 6469  l.yd-upload --di
-000190d0: 7265 6374 6f72 7920 6d79 5f77 6f72 6b5f  rectory my_work_
-000190e0: 7265 7175 6972 656d 656e 7420 6669 6c65  requirement file
-000190f0: 5f31 2066 696c 655f 3220 6d6f 7265 6669  _1 file_2 morefi
-00019100: 6c65 732f 6669 6c65 330a 6060 600a 546f  les/file3.```.To
-00019110: 2073 7570 7072 6573 7320 7468 6520 6d69   suppress the mi
-00019120: 7272 6f72 696e 6720 6f66 2074 6865 206c  rroring of the l
-00019130: 6f63 616c 2064 6972 6563 746f 7279 2073  ocal directory s
-00019140: 7472 7563 7475 7265 2077 6974 6869 6e20  tructure within 
-00019150: 7468 6520 6f62 6a65 6374 2073 746f 7265  the object store
-00019160: 2c20 7573 6520 7468 6520 602d 2d66 6c61  , use the `--fla
-00019170: 7474 656e 2d75 706c 6f61 642d 7061 7468  tten-upload-path
-00019180: 7360 206f 7220 602d 6660 206f 7074 696f  s` or `-f` optio
-00019190: 6e2e 204e 6f74 6520 7468 6174 2069 6620  n. Note that if 
-000191a0: 7468 6973 2063 7265 6174 6573 206d 756c  this creates mul
-000191b0: 7469 706c 6520 7570 6c6f 6164 6564 2066  tiple uploaded f
-000191c0: 696c 6573 2077 6974 6820 7468 6520 7361  iles with the sa
-000191d0: 6d65 2070 6174 6820 696e 2074 6865 204f  me path in the O
-000191e0: 626a 6563 7420 5374 6f72 6520 666f 6c64  bject Store fold
-000191f0: 6572 2c20 6669 6c65 7320 7769 6c6c 2062  er, files will b
-00019200: 6520 6f76 6572 7772 6974 7465 6e2e 0a0a  e overwritten...
-00019210: 4669 6c65 7320 696e 2064 6972 6563 746f  Files in directo
-00019220: 7269 6573 206d 6179 2062 6520 7265 6375  ries may be recu
-00019230: 7273 6976 656c 7920 7570 6c6f 6164 6564  rsively uploaded
-00019240: 2075 7369 6e67 2074 6865 2060 2d2d 7265   using the `--re
-00019250: 6375 7273 6976 6560 206f 7220 602d 7260  cursive` or `-r`
-00019260: 206f 7074 696f 6e2c 2065 2e67 2e3a 0a0a   option, e.g.:..
-00019270: 6060 6073 6865 6c6c 0a79 642d 7570 6c6f  ```shell.yd-uplo
-00019280: 6164 202d 2d64 6972 6563 746f 7279 206d  ad --directory m
-00019290: 795f 776f 726b 5f72 6571 7569 7265 6d65  y_work_requireme
-000192a0: 6e74 202d 7220 6d79 6469 7220 6d79 6f74  nt -r mydir myot
-000192b0: 6865 7264 6972 0a60 6060 0a0a 546f 2075  herdir.```..To u
-000192c0: 706c 6f61 6420 746f 206f 7468 6572 206e  pload to other n
-000192d0: 616d 6573 7061 6365 732c 2075 7365 2074  amespaces, use t
-000192e0: 6865 2060 2d2d 6e61 6d65 7370 6163 6560  he `--namespace`
-000192f0: 2f60 2d6e 6020 6f70 7469 6f6e 2e0a 0a23  /`-n` option...#
-00019300: 2320 7964 2d73 6875 7464 6f77 6e0a 0a54  # yd-shutdown..T
-00019310: 6865 2060 7964 2d73 6875 7464 6f77 6e60  he `yd-shutdown`
-00019320: 2063 6f6d 6d61 6e64 2073 6875 7473 2064   command shuts d
-00019330: 6f77 6e20 576f 726b 6572 2050 6f6f 6c73  own Worker Pools
-00019340: 2074 6861 7420 6d61 7463 6820 7468 6520   that match the 
-00019350: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
-00019360: 6074 6167 6020 666f 756e 6420 696e 2074  `tag` found in t
-00019370: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-00019380: 2066 696c 652e 2041 6c6c 2072 656d 6169   file. All remai
-00019390: 6e69 6e67 2077 6f72 6b20 7769 6c6c 2062  ning work will b
-000193a0: 6520 6361 6e63 656c 6c65 642c 2062 7574  e cancelled, but
-000193b0: 2063 7572 7265 6e74 6c79 2065 7865 6375   currently execu
-000193c0: 7469 6e67 2054 6173 6b73 2077 696c 6c20  ting Tasks will 
-000193d0: 6265 2061 6c6c 6f77 6564 2074 6f20 636f  be allowed to co
-000193e0: 6d70 6c65 7465 2c20 6166 7465 7220 7768  mplete, after wh
-000193f0: 6963 6820 7468 6520 436f 6d70 7574 6520  ich the Compute 
-00019400: 5265 7175 6972 656d 656e 7420 7769 6c6c  Requirement will
-00019410: 2062 6520 7465 726d 696e 6174 6564 2e0a   be terminated..
-00019420: 0a23 2320 7964 2d69 6e73 7461 6e74 6961  .## yd-instantia
-00019430: 7465 0a0a 5468 6520 6079 642d 696e 7374  te..The `yd-inst
-00019440: 616e 7469 6174 6560 2063 6f6d 6d61 6e64  antiate` command
-00019450: 2069 6e73 7461 6e74 6961 7465 7320 6120   instantiates a 
-00019460: 436f 6d70 7574 6520 5265 7175 6972 656d  Compute Requirem
-00019470: 656e 7420 2869 2e65 2e2c 2061 2073 6574  ent (i.e., a set
-00019480: 206f 6620 696e 7374 616e 6365 7320 7468   of instances th
-00019490: 6174 2061 7265 206d 616e 6167 6564 2062  at are managed b
-000194a0: 7920 7468 6569 7220 6372 6561 746f 7220  y their creator 
-000194b0: 616e 6420 646f 206e 6f74 2061 7574 6f6d  and do not autom
-000194c0: 6174 6963 616c 6c79 2062 6563 6f6d 6520  atically become 
-000194d0: 7061 7274 206f 6620 6120 5965 6c6c 6f77  part of a Yellow
-000194e0: 446f 6720 576f 726b 6572 2050 6f6f 6c29  Dog Worker Pool)
-000194f0: 2e0a 0a54 6869 7320 636f 6d6d 616e 6420  ...This command 
-00019500: 7573 6573 2074 6865 2064 6174 6120 6672  uses the data fr
-00019510: 6f6d 2074 6865 2060 776f 726b 6572 506f  om the `workerPo
-00019520: 6f6c 6020 636f 6e66 6967 7572 6174 696f  ol` configuratio
-00019530: 6e20 7365 6374 696f 6e2c 2062 7574 206f  n section, but o
-00019540: 6e6c 7920 7573 6573 2074 6865 2060 6e61  nly uses the `na
-00019550: 6d65 602c 2060 7465 6d70 6c61 7465 4964  me`, `templateId
-00019560: 602c 2060 7461 7267 6574 496e 7374 616e  `, `targetInstan
-00019570: 6365 436f 756e 7460 2c20 6069 6e73 7461  ceCount`, `insta
-00019580: 6e63 6554 6167 7360 2c20 6075 7365 7244  nceTags`, `userD
-00019590: 6174 6160 2c20 616e 6420 6069 6d61 6765  ata`, and `image
-000195a0: 7349 6460 2070 726f 7065 7274 6965 732e  sId` properties.
-000195b0: 2049 6e20 6164 6469 7469 6f6e 2c20 7468   In addition, th
-000195c0: 6520 426f 6f6c 6561 6e20 7072 6f70 6572  e Boolean proper
-000195d0: 7479 2060 6d61 696e 7461 696e 496e 7374  ty `maintainInst
-000195e0: 616e 6365 436f 756e 7460 2028 6465 6661  anceCount` (defa
-000195f0: 756c 7420 3d20 6066 616c 7365 6029 2069  ult = `false`) i
-00019600: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
-00019610: 7573 6520 7769 7468 2060 7964 2d69 6e73  use with `yd-ins
-00019620: 7461 6e74 6961 7465 602e 0a0a 436f 6d70  tantiate`...Comp
-00019630: 7574 6520 5265 7175 6972 656d 656e 7473  ute Requirements
-00019640: 2063 616e 2062 6520 696e 7374 616e 7469   can be instanti
-00019650: 6174 6564 2064 6972 6563 746c 7920 6672  ated directly fr
-00019660: 6f6d 204a 534f 4e20 286f 7220 4a73 6f6e  om JSON (or Json
-00019670: 6e65 7429 2073 7065 6369 6669 6361 7469  net) specificati
-00019680: 6f6e 732c 2075 7369 6e67 2074 6865 2060  ons, using the `
-00019690: 2d2d 636f 6d70 7574 652d 7265 7175 6972  --compute-requir
-000196a0: 656d 656e 7460 2028 6f72 2060 2d43 6029  ement` (or `-C`)
-000196b0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
-000196c0: 7469 6f6e 2c20 666f 6c6c 6f77 6564 2062  tion, followed b
-000196d0: 7920 7468 6520 6669 6c65 6e61 6d65 2e20  y the filename. 
-000196e0: 5468 6520 7072 6f70 6572 7469 6573 206c  The properties l
-000196f0: 6973 7465 6420 6162 6f76 6520 7769 6c6c  isted above will
-00019700: 2062 6520 696e 6865 7269 7465 6420 6672   be inherited fr
-00019710: 6f6d 2074 6865 2063 6f6e 6669 672e 746f  om the config.to
-00019720: 6d6c 2060 776f 726b 6572 506f 6f6c 6020  ml `workerPool` 
-00019730: 7370 6563 6966 6963 6174 696f 6e20 6966  specification if
-00019740: 2074 6865 7920 6172 6520 6e6f 7420 7072   they are not pr
-00019750: 6573 656e 7420 696e 2074 6865 204a 534f  esent in the JSO
-00019760: 4e20 6669 6c65 2e20 416e 2065 7861 6d70  N file. An examp
-00019770: 6c65 204a 534f 4e20 7370 6563 6966 6963  le JSON specific
-00019780: 6174 696f 6e20 6973 2073 686f 776e 2062  ation is shown b
-00019790: 656c 6f77 3a0a 0a60 6060 6a73 6f6e 0a7b  elow:..```json.{
-000197a0: 0a20 2022 696d 6167 6573 4964 223a 2022  .  "imagesId": "
-000197b0: 7964 6964 3a69 6d67 6661 6d3a 3030 3030  ydid:imgfam:0000
-000197c0: 3030 3a34 3139 3632 3539 322d 3537 3763  00:41962592-577c
-000197d0: 2d34 6664 652d 6162 3033 2d64 3835 3234  -4fde-ab03-d8524
-000197e0: 3635 6537 6638 6222 2c0a 2020 2269 6e73  65e7f8b",.  "ins
-000197f0: 7461 6e63 6554 6167 7322 3a20 7b22 6131  tanceTags": {"a1
-00019800: 223a 2022 6f6e 6522 2c20 2261 3222 3a20  ": "one", "a2": 
-00019810: 2274 776f 227d 2c0a 2020 2272 6571 7569  "two"},.  "requi
-00019820: 7265 6d65 6e74 4e61 6d65 223a 2022 6372  rementName": "cr
-00019830: 5f74 6573 745f 7b7b 6461 7465 7469 6d65  _test_{{datetime
-00019840: 7d7d 222c 0a20 2022 7265 7175 6972 656d  }}",.  "requirem
-00019850: 656e 744e 616d 6573 7061 6365 223a 2022  entNamespace": "
-00019860: 7079 6578 616d 706c 6573 222c 0a20 2022  pyexamples",.  "
-00019870: 7265 7175 6972 656d 656e 7454 6167 223a  requirementTag":
-00019880: 2022 7079 6578 616d 706c 6573 2d74 6573   "pyexamples-tes
-00019890: 7422 2c0a 2020 2274 656d 706c 6174 6549  t",.  "templateI
-000198a0: 6422 3a20 2279 6469 643a 6372 743a 3030  d": "ydid:crt:00
-000198b0: 3030 3030 3a32 3330 6539 6134 322d 3937  0000:230e9a42-97
-000198c0: 6462 2d34 6436 392d 6161 3931 2d32 3966  db-4d69-aa91-29f
-000198d0: 6633 3039 3935 3162 3422 2c0a 2020 2275  f309951b4",.  "u
-000198e0: 7365 7244 6174 6122 3a20 2223 2f62 696e  serData": "#/bin
-000198f0: 2f62 6173 685c 6e23 4f74 6865 7220 7374  /bash\n#Other st
-00019900: 7566 662e 2e2e 222c 0a20 2022 7461 7267  uff...",.  "targ
-00019910: 6574 496e 7374 616e 6365 436f 756e 7422  etInstanceCount"
-00019920: 3a20 312c 0a20 2022 6d61 696e 7461 696e  : 1,.  "maintain
-00019930: 496e 7374 616e 6365 436f 756e 7422 3a20  InstanceCount": 
-00019940: 7472 7565 0a7d 0a60 6060 0a0a 4966 2061  true.}.```..If a
-00019950: 2057 6f72 6b65 7220 506f 6f6c 2069 7320   Worker Pool is 
-00019960: 6465 6669 6e65 642c 2075 7369 6e67 2060  defined, using `
-00019970: 776f 726b 6572 506f 6f6c 4461 7461 6020  workerPoolData` 
-00019980: 696e 2074 6865 2063 6f6e 6669 6775 7261  in the configura
-00019990: 7469 6f6e 2066 696c 6520 6f72 2062 7920  tion file or by 
-000199a0: 7573 696e 6720 7468 6520 602d 2d77 6f72  using the `--wor
-000199b0: 6b65 722d 706f 6f6c 6020 286f 7220 602d  ker-pool` (or `-
-000199c0: 7060 2920 6f70 7469 6f6e 2c20 6079 642d  p`) option, `yd-
-000199d0: 696e 7374 616e 7469 6174 6560 2077 696c  instantiate` wil
-000199e0: 6c20 6578 7472 6163 7420 7468 6520 436f  l extract the Co
-000199f0: 6d70 7574 6520 5265 7175 6972 656d 656e  mpute Requiremen
-00019a00: 7420 6672 6f6d 2074 6865 2057 6f72 6b65  t from the Worke
-00019a10: 7220 506f 6f6c 2073 7065 6369 6669 6361  r Pool specifica
-00019a20: 7469 6f6e 2028 6967 6e6f 7269 6e67 2057  tion (ignoring W
-00019a30: 6f72 6b65 722d 506f 6f6c 2d73 7065 6369  orker-Pool-speci
-00019a40: 6669 6320 6461 7461 292c 2061 6e64 2075  fic data), and u
-00019a50: 7365 2074 6861 7420 666f 7220 696e 7374  se that for inst
-00019a60: 616e 7469 6174 696e 6720 7468 6520 436f  antiating the Co
-00019a70: 6d70 7574 6520 5265 7175 6972 656d 656e  mpute Requiremen
-00019a80: 742e 0a0a 5573 6520 7468 6520 602d 2d64  t...Use the `--d
-00019a90: 7279 2d72 756e 6020 6f70 7469 6f6e 2074  ry-run` option t
-00019aa0: 6f20 696e 7370 6563 7420 7468 6520 6465  o inspect the de
-00019ab0: 7461 696c 7320 6f66 2074 6865 2043 6f6d  tails of the Com
-00019ac0: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
-00019ad0: 2073 7065 6369 6669 6361 7469 6f6e 2074   specification t
-00019ae0: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
-00019af0: 6974 7465 642c 2069 6e20 4a53 4f4e 2066  itted, in JSON f
-00019b00: 6f72 6d61 742e 2054 6865 204a 534f 4e20  ormat. The JSON 
-00019b10: 6f75 7470 7574 206f 6620 7468 6973 2063  output of this c
-00019b20: 6f6d 6d61 6e64 2063 616e 2062 6520 7573  ommand can be us
-00019b30: 6564 2077 6974 6820 7468 6520 602d 4360  ed with the `-C`
-00019b40: 206f 7074 696f 6e20 6162 6f76 6520 286f   option above (o
-00019b50: 7220 7769 7468 2060 2d70 6020 666f 7220  r with `-p` for 
-00019b60: 576f 726b 6572 2050 6f6f 6c20 7370 6563  Worker Pool spec
-00019b70: 6966 6963 6174 696f 6e73 292e 0a0a 2323  ifications)...##
-00019b80: 2320 5465 7374 2d52 756e 6e69 6e67 2061  # Test-Running a
-00019b90: 2044 796e 616d 6963 2054 656d 706c 6174   Dynamic Templat
-00019ba0: 650a 0a57 6865 6e20 6120 7468 6520 6074  e..When a the `t
-00019bb0: 656d 706c 6174 6549 6460 206f 6620 6120  emplateId` of a 
-00019bc0: 4479 6e61 6d69 6320 5265 7175 6972 656d  Dynamic Requirem
-00019bd0: 656e 7420 6973 2075 7365 642c 2074 6865  ent is used, the
-00019be0: 2060 7964 2d69 6e73 7461 6e74 6961 7465   `yd-instantiate
-00019bf0: 6020 636f 6d6d 616e 6420 6361 6e20 6265  ` command can be
-00019c00: 2075 7365 6420 746f 2072 6570 6f72 7420   used to report 
-00019c10: 6f6e 2061 2074 6573 7420 7275 6e20 6f66  on a test run of
-00019c20: 2074 6865 2054 656d 706c 6174 652c 2075   the Template, u
-00019c30: 7369 6e67 2074 6865 2060 2d2d 7265 706f  sing the `--repo
-00019c40: 7274 6020 286f 7220 602d 7260 2920 636f  rt` (or `-r`) co
-00019c50: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
-00019c60: 6e2e 2054 6869 7320 6361 6e20 6265 2075  n. This can be u
-00019c70: 7365 6420 7769 7468 2054 4f4d 4c2d 6465  sed with TOML-de
-00019c80: 6669 6e65 6420 436f 6d70 7574 6520 5265  fined Compute Re
-00019c90: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
-00019ca0: 6963 6174 696f 6e73 2c20 6275 7420 6e6f  ications, but no
-00019cb0: 7420 7468 6f73 6520 7468 6174 2061 7265  t those that are
-00019cc0: 204a 534f 4e2d 6465 6669 6e65 642e 0a0a   JSON-defined...
-00019cd0: 4e6f 2069 6e73 7461 6e63 6573 2077 696c  No instances wil
-00019ce0: 6c20 6265 2070 726f 7669 7369 6f6e 6564  l be provisioned
-00019cf0: 2064 7572 696e 6720 7468 6520 7465 7374   during the test
-00019d00: 2072 756e 2e0a 0a46 6f72 2065 7861 6d70   run...For examp
-00019d10: 6c65 3a0a 0a60 6060 7368 656c 6c0a 2520  le:..```shell.% 
-00019d20: 7964 2d69 6e73 7461 6e74 6961 7465 202d  yd-instantiate -
-00019d30: 2d72 6570 6f72 7420 2d2d 7175 6965 740a  -report --quiet.
-00019d40: 0ae2 948c e294 80e2 9480 e294 80e2 9480  ................
-00019d50: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
-00019d60: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-00019d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d90: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
-00019da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019dd0: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
-00019de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019df0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-00019e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e30: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e60: 80e2 9480 e294 80e2 9480 e294 900a e294  ................
-00019e70: 8220 2020 20e2 9482 2020 2052 616e 6b20  .    ...   Rank 
-00019e80: e294 8220 5072 6f76 6964 6572 2020 20e2  ... Provider   .
-00019e90: 9482 2054 7970 6520 2020 2020 2020 2020  .. Type         
-00019ea0: 2020 2020 2020 2020 e294 8220 5265 6769          ... Regi
-00019eb0: 6f6e 2020 2020 e294 8220 496e 7374 616e  on    ... Instan
-00019ec0: 6365 5479 7065 2020 20e2 9482 2053 6f75  ceType   ... Sou
-00019ed0: 7263 6520 4e61 6d65 2020 2020 2020 20e2  rce Name       .
-00019ee0: 9482 0ae2 949c e294 80e2 9480 e294 80e2  ................
-00019ef0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00019f00: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00019f10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019f20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f30: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00019f40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019f50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019f70: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00019f80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f90: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00019fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019fd0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-00019fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a000: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
-0001a010: e294 8220 2031 20e2 9482 2020 2020 2020  ...  1 ...      
-0001a020: 3120 e294 8220 4157 5320 2020 2020 2020  1 ... AWS       
-0001a030: 20e2 9482 2041 7773 5370 6f74 436f 6d70   ... AwsSpotComp
-0001a040: 7574 6553 6f75 7263 6520 e294 8220 6575  uteSource ... eu
-0001a050: 2d77 6573 742d 3220 e294 8220 7433 612e  -west-2 ... t3a.
-0001a060: 6e61 6e6f 2020 2020 2020 20e2 9482 2061  nano       ... a
-0001a070: 7773 7370 6f74 2d65 752d 7765 7374 2d32  wsspot-eu-west-2
-0001a080: 20e2 9482 0ae2 949c e294 80e2 9480 e294   ...............
-0001a090: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a0a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a0b0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a0c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a0d0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a0e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a0f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a100: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a110: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a140: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a170: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a1a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a1b0: a40a e294 8220 2032 20e2 9482 2020 2020  .....  2 ...    
-0001a1c0: 2020 3220 e294 8220 4157 5320 2020 2020    2 ... AWS     
-0001a1d0: 2020 20e2 9482 2041 7773 5370 6f74 436f     ... AwsSpotCo
-0001a1e0: 6d70 7574 6553 6f75 7263 6520 e294 8220  mputeSource ... 
-0001a1f0: 6575 2d77 6573 742d 3220 e294 8220 7433  eu-west-2 ... t3
-0001a200: 612e 6d69 6372 6f20 2020 2020 20e2 9482  a.micro      ...
-0001a210: 2061 7773 7370 6f74 2d65 752d 7765 7374   awsspot-eu-west
-0001a220: 2d32 20e2 9482 0ae2 949c e294 80e2 9480  -2 .............
-0001a230: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a250: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a270: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a2a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a2b0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a2c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a2d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a2e0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a2f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a310: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a330: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a340: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a350: e294 a40a e294 8220 2033 20e2 9482 2020  .......  3 ...  
-0001a360: 2020 2020 3320 e294 8220 4157 5320 2020      3 ... AWS   
-0001a370: 2020 2020 20e2 9482 2041 7773 5370 6f74       ... AwsSpot
-0001a380: 436f 6d70 7574 6553 6f75 7263 6520 e294  ComputeSource ..
-0001a390: 8220 6575 2d77 6573 742d 3220 e294 8220  . eu-west-2 ... 
-0001a3a0: 7433 612e 736d 616c 6c20 2020 2020 20e2  t3a.small      .
-0001a3b0: 9482 2061 7773 7370 6f74 2d65 752d 7765  .. awsspot-eu-we
-0001a3c0: 7374 2d32 20e2 9482 0ae2 949c e294 80e2  st-2 ...........
-0001a3d0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a3e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a3f0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a400: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a410: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001a420: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a440: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a460: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a480: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a4a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a4b0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a4c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a4d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a4e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a4f0: 9480 e294 a40a e294 8220 2034 20e2 9482  .........  4 ...
-0001a500: 2020 2020 2020 3420 e294 8220 4157 5320        4 ... AWS 
-0001a510: 2020 2020 2020 20e2 9482 2041 7773 5370         ... AwsSp
-0001a520: 6f74 436f 6d70 7574 6553 6f75 7263 6520  otComputeSource 
-0001a530: e294 8220 6575 2d77 6573 742d 3220 e294  ... eu-west-2 ..
-0001a540: 8220 6335 612e 6c61 7267 6520 2020 2020  . c5a.large     
-0001a550: 20e2 9482 2061 7773 7370 6f74 2d65 752d   ... awsspot-eu-
-0001a560: 7765 7374 2d32 20e2 9482 0ae2 949c e294  west-2 .........
-0001a570: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001a580: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a590: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a5a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a5b0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001a5c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a5d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a5e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a5f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a600: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a610: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a620: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a630: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a650: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a660: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a690: 80e2 9480 e294 a40a e294 8220 2035 20e2  ...........  5 .
-0001a6a0: 9482 2020 2020 2020 3420 e294 8220 4157  ..      4 ... AW
-0001a6b0: 5320 2020 2020 2020 20e2 9482 2041 7773  S        ... Aws
-0001a6c0: 5370 6f74 436f 6d70 7574 6553 6f75 7263  SpotComputeSourc
-0001a6d0: 6520 e294 8220 6575 2d77 6573 742d 3220  e ... eu-west-2 
-0001a6e0: e294 8220 6336 612e 6c61 7267 6520 2020  ... c6a.large   
-0001a6f0: 2020 20e2 9482 2061 7773 7370 6f74 2d65     ... awsspot-e
-0001a700: 752d 7765 7374 2d32 20e2 9482 0ae2 949c  u-west-2 .......
-0001a710: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001a720: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a730: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a740: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a750: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a760: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a770: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a780: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a7a0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a7b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a7c0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a7d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a7e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a7f0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001a800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a830: e294 80e2 9480 e294 a40a e294 8220 2036  .............  6
-0001a840: 20e2 9482 2020 2020 2020 3420 e294 8220   ...      4 ... 
-0001a850: 4157 5320 2020 2020 2020 20e2 9482 2041  AWS        ... A
-0001a860: 7773 5370 6f74 436f 6d70 7574 6553 6f75  wsSpotComputeSou
-0001a870: 7263 6520 e294 8220 6575 2d77 6573 742d  rce ... eu-west-
-0001a880: 3220 e294 8220 7433 612e 6d65 6469 756d  2 ... t3a.medium
-0001a890: 2020 2020 20e2 9482 2061 7773 7370 6f74       ... awsspot
-0001a8a0: 2d65 752d 7765 7374 2d32 20e2 9482 0ae2  -eu-west-2 .....
-0001a8b0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a8c0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a8d0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a8e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a8f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a900: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a940: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a960: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a990: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001a9a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a9b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a9c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a9d0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-0001a9e0: 2037 20e2 9482 2020 2020 2020 3520 e294   7 ...      5 ..
-0001a9f0: 8220 4157 5320 2020 2020 2020 20e2 9482  . AWS        ...
-0001aa00: 2041 7773 5370 6f74 436f 6d70 7574 6553   AwsSpotComputeS
-0001aa10: 6f75 7263 6520 e294 8220 6575 2d77 6573  ource ... eu-wes
-0001aa20: 742d 3220 e294 8220 6d35 612e 6c61 7267  t-2 ... m5a.larg
-0001aa30: 6520 2020 2020 20e2 9482 2061 7773 7370  e      ... awssp
-0001aa40: 6f74 2d65 752d 7765 7374 2d32 20e2 9482  ot-eu-west-2 ...
-0001aa50: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-0001aa60: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa70: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001aa80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aa90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aaa0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001aab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aac0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aae0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001aaf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ab00: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001ab10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ab20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ab30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ab40: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ab50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ab60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ab70: 80e2 9480 e294 80e2 9480 e294 a40a e294  ................
-0001ab80: 8220 2038 20e2 9482 2020 2020 2020 3520  .  8 ...      5 
-0001ab90: e294 8220 4157 5320 2020 2020 2020 20e2  ... AWS        .
-0001aba0: 9482 2041 7773 5370 6f74 436f 6d70 7574  .. AwsSpotComput
-0001abb0: 6553 6f75 7263 6520 e294 8220 6575 2d77  eSource ... eu-w
-0001abc0: 6573 742d 3220 e294 8220 6d35 6164 2e6c  est-2 ... m5ad.l
-0001abd0: 6172 6765 2020 2020 20e2 9482 2061 7773  arge     ... aws
-0001abe0: 7370 6f74 2d65 752d 7765 7374 2d32 20e2  spot-eu-west-2 .
-0001abf0: 9482 0ae2 949c e294 80e2 9480 e294 80e2  ................
-0001ac00: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001ac10: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001ac20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ac30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ac40: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001ac50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ac60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ac70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ac80: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001ac90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aca0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001acb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001acc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001acd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ace0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001acf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ad00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ad10: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
-0001ad20: e294 8220 2039 20e2 9482 2020 2020 2020  ...  9 ...      
-0001ad30: 3520 e294 8220 4157 5320 2020 2020 2020  5 ... AWS       
-0001ad40: 20e2 9482 2041 7773 5370 6f74 436f 6d70   ... AwsSpotComp
-0001ad50: 7574 6553 6f75 7263 6520 e294 8220 6575  uteSource ... eu
-0001ad60: 2d77 6573 742d 3220 e294 8220 6d36 612e  -west-2 ... m6a.
-0001ad70: 6c61 7267 6520 2020 2020 20e2 9482 2061  large      ... a
-0001ad80: 7773 7370 6f74 2d65 752d 7765 7374 2d32  wsspot-eu-west-2
-0001ad90: 20e2 9482 0ae2 949c e294 80e2 9480 e294   ...............
-0001ada0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001adb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001adc0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001add0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ade0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001adf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ae00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ae10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae20: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001ae30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ae40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae50: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001ae60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001ae70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001ae80: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001ae90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aeb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aec0: a40a e294 8220 3130 20e2 9482 2020 2020  ..... 10 ...    
-0001aed0: 2020 3520 e294 8220 4157 5320 2020 2020    5 ... AWS     
-0001aee0: 2020 20e2 9482 2041 7773 5370 6f74 436f     ... AwsSpotCo
-0001aef0: 6d70 7574 6553 6f75 7263 6520 e294 8220  mputeSource ... 
-0001af00: 6575 2d77 6573 742d 3220 e294 8220 7433  eu-west-2 ... t3
-0001af10: 612e 6c61 7267 6520 2020 2020 20e2 9482  a.large      ...
-0001af20: 2061 7773 7370 6f74 2d65 752d 7765 7374   awsspot-eu-west
-0001af30: 2d32 20e2 9482 0ae2 9494 e294 80e2 9480  -2 .............
-0001af40: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-0001af50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001af60: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-0001af70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001af80: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
-0001af90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001afa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001afb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001afc0: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
-0001afd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001afe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aff0: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-0001b000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001b010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001b020: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-0001b030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001b040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001b050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001b060: e294 980a 6060 600a 0a23 2320 7964 2d74  ....```..## yd-t
-0001b070: 6572 6d69 6e61 7465 0a0a 5468 6520 6079  erminate..The `y
-0001b080: 642d 7465 726d 696e 6174 6560 2063 6f6d  d-terminate` com
-0001b090: 6d61 6e64 2069 6d6d 6564 6961 7465 6c79  mand immediately
-0001b0a0: 2074 6572 6d69 6e61 7465 7320 436f 6d70   terminates Comp
-0001b0b0: 7574 6520 5265 7175 6972 656d 656e 7473  ute Requirements
-0001b0c0: 2074 6861 7420 6d61 7463 6820 7468 6520   that match the 
-0001b0d0: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
-0001b0e0: 6074 6167 6020 666f 756e 6420 696e 2074  `tag` found in t
-0001b0f0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-0001b100: 2066 696c 652e 2041 6e79 2065 7865 6375   file. Any execu
-0001b110: 7469 6e67 2054 6173 6b73 2077 696c 6c20  ting Tasks will 
-0001b120: 6265 2074 6572 6d69 6e61 7465 6420 696d  be terminated im
-0001b130: 6d65 6469 6174 656c 792c 2061 6e64 2074  mediately, and t
-0001b140: 6865 2057 6f72 6b65 7220 506f 6f6c 2077  he Worker Pool w
-0001b150: 696c 6c20 6265 2073 6875 7420 646f 776e  ill be shut down
-0001b160: 2e0a                                     ..
+00014150: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00014160: 2020 2020 2020 2020 2020 207c 0a0a 2323             |..##
+00014170: 2041 7574 6f6d 6174 6963 2050 726f 7065   Automatic Prope
+00014180: 7274 6965 730a 0a54 6865 206e 616d 6520  rties..The name 
+00014190: 6f66 2074 6865 2057 6f72 6b65 7220 506f  of the Worker Po
+000141a0: 6f6c 2c20 6966 206e 6f74 2073 7570 706c  ol, if not suppl
+000141b0: 6965 642c 2069 7320 6175 746f 6d61 7469  ied, is automati
+000141c0: 6361 6c6c 7920 6765 6e65 7261 7465 6420  cally generated 
+000141d0: 7573 696e 6720 6120 636f 6e63 6174 656e  using a concaten
+000141e0: 6174 696f 6e20 6f66 2060 7770 5f60 2c20  ation of `wp_`, 
+000141f0: 7468 6520 6074 6167 6020 7072 6f70 6572  the `tag` proper
+00014200: 7479 2c20 6120 5554 4320 7469 6d65 7374  ty, a UTC timest
+00014210: 616d 702c 2061 6e64 2074 6872 6565 2072  amp, and three r
+00014220: 616e 646f 6d20 6865 7820 6368 6172 6163  andom hex charac
+00014230: 7465 7273 3a20 652c 672c 2e20 6077 705f  ters: e,g,. `wp_
+00014240: 6d79 7461 675f 3232 3130 3234 2d31 3535  mytag_221024-155
+00014250: 3532 342d 6230 6160 2e0a 0a23 2320 544f  524-b0a`...## TO
+00014260: 4d4c 2050 726f 7065 7274 6965 7320 696e  ML Properties in
+00014270: 2074 6865 2060 776f 726b 6572 506f 6f6c   the `workerPool
+00014280: 6020 5365 6374 696f 6e0a 0a48 6572 6527  ` Section..Here'
+00014290: 7320 616e 2065 7861 6d70 6c65 206f 6620  s an example of 
+000142a0: 7468 6520 6077 6f72 6b65 7250 6f6f 6c60  the `workerPool`
+000142b0: 2073 6563 7469 6f6e 206f 6620 6120 544f   section of a TO
+000142c0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+000142d0: 2066 696c 652c 2073 686f 7769 6e67 2061   file, showing a
+000142e0: 6c6c 2074 6865 2070 6f73 7369 626c 6520  ll the possible 
+000142f0: 7072 6f70 6572 7469 6573 2074 6861 7420  properties that 
+00014300: 6361 6e20 6265 2073 6574 3a0a 0a60 6060  can be set:..```
+00014310: 746f 6d6c 0a5b 776f 726b 6572 506f 6f6c  toml.[workerPool
+00014320: 5d0a 2020 2020 6964 6c65 4e6f 6465 5368  ].    idleNodeSh
+00014330: 7574 646f 776e 456e 6162 6c65 6420 3d20  utdownEnabled = 
+00014340: 7472 7565 0a20 2020 2069 646c 654e 6f64  true.    idleNod
+00014350: 6553 6875 7464 6f77 6e54 696d 656f 7574  eShutdownTimeout
+00014360: 203d 2031 302e 300a 2020 2020 6964 6c65   = 10.0.    idle
+00014370: 506f 6f6c 5368 7574 646f 776e 456e 6162  PoolShutdownEnab
+00014380: 6c65 6420 3d20 7472 7565 0a20 2020 2069  led = true.    i
+00014390: 646c 6550 6f6f 6c53 6875 7464 6f77 6e54  dlePoolShutdownT
+000143a0: 696d 656f 7574 203d 2036 302e 300a 2020  imeout = 60.0.  
+000143b0: 2020 696d 6167 6573 4964 203d 2022 7964    imagesId = "yd
+000143c0: 6964 3a69 6d67 6661 6d3a 3030 3030 3030  id:imgfam:000000
+000143d0: 3a34 3139 3632 3539 322d 3537 3763 2d34  :41962592-577c-4
+000143e0: 6664 652d 6162 3033 2d64 3835 3234 3635  fde-ab03-d852465
+000143f0: 6537 6638 6222 0a20 2020 2069 6e73 7461  e7f8b".    insta
+00014400: 6e63 6554 6167 7320 3d20 7b7d 0a20 2020  nceTags = {}.   
+00014410: 206d 6178 4e6f 6465 7320 3d20 310a 2020   maxNodes = 1.  
+00014420: 2020 6d69 6e4e 6f64 6573 203d 2031 0a20    minNodes = 1. 
+00014430: 2020 206e 616d 6520 3d20 226d 792d 776f     name = "my-wo
+00014440: 726b 6572 2d70 6f6f 6c22 0a20 2020 206e  rker-pool".    n
+00014450: 6f64 6542 6f6f 7454 696d 656f 7574 203d  odeBootTimeout =
+00014460: 2035 0a20 2020 2074 6172 6765 7449 6e73   5.    targetIns
+00014470: 7461 6e63 6543 6f75 6e74 203d 2031 0a20  tanceCount = 1. 
+00014480: 2020 2074 656d 706c 6174 6549 6420 3d20     templateId = 
+00014490: 2279 6469 643a 6372 743a 4439 4335 3438  "ydid:crt:D9C548
+000144a0: 3a34 3635 6131 3037 632d 3763 6561 2d34  :465a107c-7cea-4
+000144b0: 3665 332d 3966 6464 2d31 3531 3136 6362  6e3-9fdd-15116cb
+000144c0: 3932 6334 3022 0a20 2020 2023 204e 6f74  92c40".    # Not
+000144d0: 653a 206f 6e6c 7920 6f6e 6520 6f66 2027  e: only one of '
+000144e0: 7573 6572 4461 7461 272f 2775 7365 7244  userData'/'userD
+000144f0: 6174 6146 696c 6527 2f27 7573 6572 4461  ataFile'/'userDa
+00014500: 7461 4669 6c65 7327 2073 686f 756c 6420  taFiles' should 
+00014510: 6265 2073 6574 0a20 2020 2075 7365 7244  be set.    userD
+00014520: 6174 6120 3d20 2222 0a20 2020 2075 7365  ata = "".    use
+00014530: 7244 6174 6146 696c 6520 3d20 226d 7975  rDataFile = "myu
+00014540: 7365 7264 6174 612e 7478 7422 0a20 2020  serdata.txt".   
+00014550: 2075 7365 7244 6174 6146 696c 6573 203d   userDataFiles =
+00014560: 205b 226d 7975 7365 7264 6174 6131 2e74   ["myuserdata1.t
+00014570: 7874 222c 2022 6d79 7573 6572 6461 7461  xt", "myuserdata
+00014580: 322e 7478 7422 5d0a 2020 2020 776f 726b  2.txt"].    work
+00014590: 6572 5461 6720 3d20 2274 6167 2d7b 7b75  erTag = "tag-{{u
+000145a0: 7365 726e 616d 657d 7d22 0a20 2020 2023  sername}}".    #
+000145b0: 2053 7065 6369 6679 2065 6974 6865 7220   Specify either 
+000145c0: 776f 726b 6572 7350 6572 4e6f 6465 206f  workersPerNode o
+000145d0: 7220 776f 726b 6572 7350 6572 5643 5055  r workersPerVCPU
+000145e0: 0a20 2020 2077 6f72 6b65 7273 5065 724e  .    workersPerN
+000145f0: 6f64 6520 3d20 310a 2020 2020 776f 726b  ode = 1.    work
+00014600: 6572 7350 6572 5643 5055 203d 2031 0a23  ersPerVCPU = 1.#
+00014610: 2020 2077 6f72 6b65 7250 6f6f 6c44 6174     workerPoolDat
+00014620: 6120 3d20 2277 6f72 6b65 725f 706f 6f6c  a = "worker_pool
+00014630: 2e6a 736f 6e22 0a60 6060 0a0a 2323 2057  .json".```..## W
+00014640: 6f72 6b65 7220 506f 6f6c 2053 7065 6369  orker Pool Speci
+00014650: 6669 6361 7469 6f6e 2055 7369 6e67 204a  fication Using J
+00014660: 534f 4e20 446f 6375 6d65 6e74 730a 0a49  SON Documents..I
+00014670: 7427 7320 616c 736f 2070 6f73 7369 626c  t's also possibl
+00014680: 6520 746f 2063 6170 7475 7265 2061 2057  e to capture a W
+00014690: 6f72 6b65 7220 506f 6f6c 2064 6566 696e  orker Pool defin
+000146a0: 6974 696f 6e20 6173 2061 204a 534f 4e20  ition as a JSON 
+000146b0: 646f 6375 6d65 6e74 2e20 5468 6520 4a53  document. The JS
+000146c0: 4f4e 2066 696c 656e 616d 6520 6361 6e20  ON filename can 
+000146d0: 6265 2073 7570 706c 6965 6420 6569 7468  be supplied eith
+000146e0: 6572 2075 7369 6e67 2074 6865 2063 6f6d  er using the com
+000146f0: 6d61 6e64 206c 696e 6520 7769 7468 2074  mand line with t
+00014700: 6865 2060 2d2d 776f 726b 6572 2d70 6f6f  he `--worker-poo
+00014710: 6c60 206f 7220 602d 7060 2070 6172 616d  l` or `-p` param
+00014720: 6574 6572 2077 6974 6820 6079 642d 7072  eter with `yd-pr
+00014730: 6f76 6973 696f 6e60 2c20 6f72 2062 7920  ovision`, or by 
+00014740: 706f 7075 6c61 7469 6e67 2074 6865 2060  populating the `
+00014750: 776f 726b 6572 506f 6f6c 4461 7461 6020  workerPoolData` 
+00014760: 7072 6f70 6572 7479 2069 6e20 7468 6520  property in the 
+00014770: 544f 4d4c 2063 6f6e 6669 6775 7261 7469  TOML configurati
+00014780: 6f6e 2066 696c 6520 7769 7468 2074 6865  on file with the
+00014790: 204a 534f 4e20 6669 6c65 6e61 6d65 2e20   JSON filename. 
+000147a0: 436f 6d6d 616e 6420 6c69 6e65 2073 7065  Command line spe
+000147b0: 6369 6669 6361 7469 6f6e 2074 616b 6573  cification takes
+000147c0: 2070 7269 6f72 6974 7920 6f76 6572 2054   priority over T
+000147d0: 4f4d 4c20 7370 6563 6966 6963 6174 696f  OML specificatio
+000147e0: 6e2e 0a0a 5468 6520 4a53 4f4e 2073 7065  n...The JSON spe
+000147f0: 6369 6669 6361 7469 6f6e 2061 6c6c 6f77  cification allow
+00014800: 7320 7468 6520 6372 6561 7469 6f6e 206f  s the creation o
+00014810: 6620 2a2a 4164 7661 6e63 6564 2057 6f72  f **Advanced Wor
+00014820: 6b65 7220 506f 6f6c 732a 2a2c 2077 6974  ker Pools**, wit
+00014830: 6820 6469 6666 6572 656e 7420 6e6f 6465  h different node
+00014840: 2074 7970 6573 2061 6e64 2074 6865 2061   types and the a
+00014850: 6269 6c69 7479 2074 6f20 7370 6563 6966  bility to specif
+00014860: 7920 4e6f 6465 2041 6374 696f 6e73 2e0a  y Node Actions..
+00014870: 0a57 6865 6e20 7573 696e 6720 6120 4a53  .When using a JS
+00014880: 4f4e 2064 6f63 756d 656e 7420 746f 2073  ON document to s
+00014890: 7065 6369 6679 2074 6865 2057 6f72 6b65  pecify the Worke
+000148a0: 7220 506f 6f6c 2c20 7468 6520 7363 6865  r Pool, the sche
+000148b0: 6d61 206f 6620 7468 6520 646f 6375 6d65  ma of the docume
+000148c0: 6e74 2069 7320 6964 656e 7469 6361 6c20  nt is identical 
+000148d0: 746f 2074 6861 7420 6578 7065 6374 6564  to that expected
+000148e0: 2062 7920 7468 6520 5965 6c6c 6f77 446f   by the YellowDo
+000148f0: 6720 5245 5354 2041 5049 2066 6f72 2057  g REST API for W
+00014900: 6f72 6b65 7220 506f 6f6c 2050 726f 7669  orker Pool Provi
+00014910: 7369 6f6e 696e 672e 0a0a 2323 2320 576f  sioning...### Wo
+00014920: 726b 6572 2050 6f6f 6c20 4a53 4f4e 2045  rker Pool JSON E
+00014930: 7861 6d70 6c65 730a 0a54 6865 2065 7861  xamples..The exa
+00014940: 6d70 6c65 2062 656c 6f77 2069 7320 6f66  mple below is of
+00014950: 2061 2073 696d 706c 6520 4a53 4f4e 2073   a simple JSON s
+00014960: 7065 6369 6669 6361 7469 6f6e 206f 6620  pecification of 
+00014970: 6120 576f 726b 6572 2050 6f6f 6c20 7769  a Worker Pool wi
+00014980: 7468 206f 6e65 2069 6e69 7469 616c 206e  th one initial n
+00014990: 6f64 652c 2057 6f72 6b65 7220 506f 6f6c  ode, Worker Pool
+000149a0: 2073 6875 7464 6f77 6e2c 2065 7463 2e0a   shutdown, etc..
+000149b0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7265  .```json.{.  "re
+000149c0: 7175 6972 656d 656e 7454 656d 706c 6174  quirementTemplat
+000149d0: 6555 7361 6765 223a 207b 0a20 2020 2022  eUsage": {.    "
+000149e0: 6d61 696e 7461 696e 496e 7374 616e 6365  maintainInstance
+000149f0: 436f 756e 7422 3a20 6661 6c73 652c 0a20  Count": false,. 
+00014a00: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
+00014a10: 616d 6522 3a20 2277 705f 7079 6578 2d70  ame": "wp_pyex-p
+00014a20: 7269 6d65 735f 3233 3031 3133 2d31 3631  rimes_230113-161
+00014a30: 3532 382d 6461 3022 2c0a 2020 2020 2272  528-da0",.    "r
+00014a40: 6571 7569 7265 6d65 6e74 4e61 6d65 7370  equirementNamesp
+00014a50: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
+00014a60: 7322 2c0a 2020 2020 2272 6571 7569 7265  s",.    "require
+00014a70: 6d65 6e74 5461 6722 3a20 2270 7965 782d  mentTag": "pyex-
+00014a80: 7072 696d 6573 222c 0a20 2020 2022 7461  primes",.    "ta
+00014a90: 7267 6574 496e 7374 616e 6365 436f 756e  rgetInstanceCoun
+00014aa0: 7422 3a20 312c 0a20 2020 2022 7465 6d70  t": 1,.    "temp
+00014ab0: 6c61 7465 4964 223a 2022 7964 6964 3a63  lateId": "ydid:c
+00014ac0: 7274 3a44 3943 3534 383a 3436 3561 3130  rt:D9C548:465a10
+00014ad0: 3763 2d37 6365 612d 3436 6533 2d39 6664  7c-7cea-46e3-9fd
+00014ae0: 642d 3135 3131 3663 6239 3263 3430 220a  d-15116cb92c40".
+00014af0: 2020 7d2c 0a20 2022 7072 6f76 6973 696f    },.  "provisio
+00014b00: 6e65 6450 726f 7065 7274 6965 7322 3a20  nedProperties": 
+00014b10: 7b0a 2020 2020 2269 646c 654e 6f64 6553  {.    "idleNodeS
+00014b20: 6875 7464 6f77 6e22 3a20 7b22 656e 6162  hutdown": {"enab
+00014b30: 6c65 6422 3a20 7472 7565 2c20 2274 696d  led": true, "tim
+00014b40: 656f 7574 223a 2022 5054 3130 4d22 7d2c  eout": "PT10M"},
+00014b50: 0a20 2020 2022 6964 6c65 506f 6f6c 5368  .    "idlePoolSh
+00014b60: 7574 646f 776e 223a 207b 2265 6e61 626c  utdown": {"enabl
+00014b70: 6564 223a 2074 7275 652c 2022 7469 6d65  ed": true, "time
+00014b80: 6f75 7422 3a20 2250 5431 4822 7d2c 0a20  out": "PT1H"},. 
+00014b90: 2020 2022 6372 6561 7465 4e6f 6465 576f     "createNodeWo
+00014ba0: 726b 6572 7322 3a20 7b22 7461 7267 6574  rkers": {"target
+00014bb0: 436f 756e 7422 3a20 312c 2022 7461 7267  Count": 1, "targ
+00014bc0: 6574 5479 7065 223a 2022 5045 525f 5643  etType": "PER_VC
+00014bd0: 5055 227d 2c0a 2020 2020 226d 6178 4e6f  PU"},.    "maxNo
+00014be0: 6465 7322 3a20 352c 0a20 2020 2022 6d69  des": 5,.    "mi
+00014bf0: 6e4e 6f64 6573 223a 2030 2c0a 2020 2020  nNodes": 0,.    
+00014c00: 226e 6f64 6542 6f6f 7454 696d 656f 7574  "nodeBootTimeout
+00014c10: 223a 2022 5054 354d 222c 0a20 2020 2022  ": "PT5M",.    "
+00014c20: 6e6f 6465 4964 6c65 4772 6163 6550 6572  nodeIdleGracePer
+00014c30: 696f 6422 3a20 2250 5433 4d22 2c0a 2020  iod": "PT3M",.  
+00014c40: 2020 226e 6f64 6549 646c 6554 696d 654c    "nodeIdleTimeL
+00014c50: 696d 6974 223a 2022 5054 334d 222c 0a20  imit": "PT3M",. 
+00014c60: 2020 2022 776f 726b 6572 5461 6722 3a20     "workerTag": 
+00014c70: 2270 7965 782d 6261 7368 2d64 6f63 6b65  "pyex-bash-docke
+00014c80: 7222 0a20 207d 0a7d 0a60 6060 0a0a 5468  r".  }.}.```..Th
+00014c90: 6520 6e65 7874 2065 7861 6d70 6c65 2069  e next example i
+00014ca0: 7320 6f66 2061 2072 656c 6174 6976 656c  s of a relativel
+00014cb0: 7920 7269 6368 204a 534f 4e20 7370 6563  y rich JSON spec
+00014cc0: 6966 6963 6174 696f 6e20 6f66 2061 6e20  ification of an 
+00014cd0: 4164 7661 6e63 6564 2057 6f72 6b65 7220  Advanced Worker 
+00014ce0: 506f 6f6c 2c20 6672 6f6d 206f 6e65 206f  Pool, from one o
+00014cf0: 6620 7468 6520 5965 6c6c 6f77 446f 6720  f the YellowDog 
+00014d00: 6465 6d6f 732e 2049 7420 696e 636c 7564  demos. It includ
+00014d10: 6573 206e 6f64 6520 7370 6563 6961 6c69  es node speciali
+00014d20: 7361 7469 6f6e 2c20 616e 6420 6163 7469  sation, and acti
+00014d30: 6f6e 2067 726f 7570 7320 7468 6174 2072  on groups that r
+00014d40: 6573 706f 6e64 2074 6f20 7468 6520 6053  espond to the `S
+00014d50: 5441 5254 5550 5f4e 4f44 4553 5f41 4444  TARTUP_NODES_ADD
+00014d60: 4544 6020 616e 6420 604e 4f44 4553 5f41  ED` and `NODES_A
+00014d70: 4444 4544 6020 6576 656e 7473 2074 6f20  DDED` events to 
+00014d80: 6472 6976 6520 2a2a 4e6f 6465 2041 6374  drive **Node Act
+00014d90: 696f 6e73 2a2a 2e0a 0a60 6060 6a73 6f6e  ions**...```json
+00014da0: 0a7b 0a20 2022 7265 7175 6972 656d 656e  .{.  "requiremen
+00014db0: 7454 656d 706c 6174 6555 7361 6765 223a  tTemplateUsage":
+00014dc0: 207b 0a20 2020 2022 6d61 696e 7461 696e   {.    "maintain
+00014dd0: 496e 7374 616e 6365 436f 756e 7422 3a20  InstanceCount": 
+00014de0: 6661 6c73 652c 0a20 2020 2022 7461 7267  false,.    "targ
+00014df0: 6574 496e 7374 616e 6365 436f 756e 7422  etInstanceCount"
+00014e00: 3a20 362c 0a20 2020 2022 7465 6d70 6c61  : 6,.    "templa
+00014e10: 7465 4964 223a 2022 7964 6964 3a63 7274  teId": "ydid:crt
+00014e20: 3a44 3943 3534 383a 6137 6564 6132 3837  :D9C548:a7eda287
+00014e30: 2d66 3964 362d 3462 6338 2d62 3264 632d  -f9d6-4bc8-b2dc-
+00014e40: 3435 3533 3434 3035 3732 3537 222c 0a20  455344057257",. 
+00014e50: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
+00014e60: 616d 6522 3a20 2277 705f 7079 6578 2d73  ame": "wp_pyex-s
+00014e70: 6c75 726d 5f32 3330 3131 332d 3136 3536  lurm_230113-1656
+00014e80: 3135 2d32 6237 222c 0a20 2020 2022 7265  15-2b7",.    "re
+00014e90: 7175 6972 656d 656e 744e 616d 6573 7061  quirementNamespa
+00014ea0: 6365 223a 2022 7079 6578 616d 706c 6573  ce": "pyexamples
+00014eb0: 222c 0a20 2020 2022 7265 7175 6972 656d  ",.    "requirem
+00014ec0: 656e 7454 6167 223a 2022 7079 6578 2d73  entTag": "pyex-s
+00014ed0: 6c75 726d 220a 2020 7d2c 0a20 2022 7072  lurm".  },.  "pr
+00014ee0: 6f76 6973 696f 6e65 6450 726f 7065 7274  ovisionedPropert
+00014ef0: 6965 7322 3a20 7b0a 2020 2020 2263 7265  ies": {.    "cre
+00014f00: 6174 654e 6f64 6557 6f72 6b65 7273 223a  ateNodeWorkers":
+00014f10: 207b 2274 6172 6765 7443 6f75 6e74 223a   {"targetCount":
+00014f20: 2030 2c20 2274 6172 6765 7454 7970 6522   0, "targetType"
+00014f30: 3a20 2250 4552 5f4e 4f44 4522 7d2c 0a20  : "PER_NODE"},. 
+00014f40: 2020 2022 6e6f 6465 436f 6e66 6967 7572     "nodeConfigur
+00014f50: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
+00014f60: 226e 6f64 6554 7970 6573 223a 205b 0a20  "nodeTypes": [. 
+00014f70: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
+00014f80: 2273 6c75 726d 6374 6c64 222c 2022 636f  "slurmctld", "co
+00014f90: 756e 7422 3a20 317d 2c0a 2020 2020 2020  unt": 1},.      
+00014fa0: 2020 7b22 6e61 6d65 223a 2022 736c 7572    {"name": "slur
+00014fb0: 6d64 222c 2022 6d69 6e22 3a20 352c 2022  md", "min": 5, "
+00014fc0: 736c 6f74 4e75 6d62 6572 696e 6722 3a20  slotNumbering": 
+00014fd0: 2252 4555 5341 424c 4522 7d0a 2020 2020  "REUSABLE"}.    
+00014fe0: 2020 5d2c 0a20 2020 2020 2022 6e6f 6465    ],.      "node
+00014ff0: 4576 656e 7473 223a 207b 0a20 2020 2020  Events": {.     
+00015000: 2020 2022 5354 4152 5455 505f 4e4f 4445     "STARTUP_NODE
+00015010: 535f 4144 4445 4422 3a20 5b0a 2020 2020  S_ADDED": [.    
+00015020: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00015030: 2020 2020 2261 6374 696f 6e73 223a 205b      "actions": [
+00015040: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00015050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015060: 2022 6163 7469 6f6e 223a 2022 5752 4954   "action": "WRIT
+00015070: 455f 4649 4c45 222c 0a20 2020 2020 2020  E_FILE",.       
+00015080: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
+00015090: 2022 6e6f 6465 732e 6a73 6f6e 222c 0a20   "nodes.json",. 
+000150a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000150b0: 636f 6e74 656e 7422 3a20 227b 5c6e 2020  content": "{\n  
+000150c0: 5c22 6e6f 6465 735c 223a 205b 5c6e 7b7b  \"nodes\": [\n{{
+000150d0: 236f 7468 6572 4e6f 6465 737d 7d5c 6e20  #otherNodes}}\n 
+000150e0: 2020 207b 5c6e 2020 2020 2020 5c22 6e61     {\n      \"na
+000150f0: 6d65 5c22 3a20 5c22 736c 7572 6d64 7b7b  me\": \"slurmd{{
+00015100: 6465 7461 696c 732e 6e6f 6465 536c 6f74  details.nodeSlot
+00015110: 7d7d 5c22 2c5c 6e20 2020 2020 205c 2269  }}\",\n      \"i
+00015120: 705c 223a 205c 227b 7b64 6574 6169 6c73  p\": \"{{details
+00015130: 2e70 7269 7661 7465 4970 4164 6472 6573  .privateIpAddres
+00015140: 737d 7d5c 225c 6e20 2020 207d 7b7b 5e2d  s}}\"\n    }{{^-
+00015150: 6c61 7374 7d7d 2c7b 7b2f 2d6c 6173 747d  last}},{{/-last}
+00015160: 7d5c 6e7b 7b2f 6f74 6865 724e 6f64 6573  }\n{{/otherNodes
+00015170: 7d7d 5c6e 2020 5d5c 6e7d 222c 0a20 2020  }}\n  ]\n}",.   
+00015180: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
+00015190: 6465 5479 7065 7322 3a20 5b22 736c 7572  deTypes": ["slur
+000151a0: 6d63 746c 6422 5d0a 2020 2020 2020 2020  mctld"].        
+000151b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000151c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000151d0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
+000151e0: 223a 2022 5255 4e5f 434f 4d4d 414e 4422  ": "RUN_COMMAND"
+000151f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015200: 2020 2270 6174 6822 3a20 2273 7461 7274    "path": "start
+00015210: 5f73 696d 706c 655f 736c 7572 6d63 746c  _simple_slurmctl
+00015220: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+00015230: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
+00015240: 205b 226e 6f64 6573 2e6a 736f 6e22 5d2c   ["nodes.json"],
+00015250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015260: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+00015270: 7b22 4558 414d 504c 4522 3a20 2246 4f4f  {"EXAMPLE": "FOO
+00015280: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00015290: 2020 2020 226e 6f64 6554 7970 6573 223a      "nodeTypes":
+000152a0: 205b 2273 6c75 726d 6374 6c64 225d 0a20   ["slurmctld"]. 
+000152b0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+000152c0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+000152d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000152e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000152f0: 2020 2261 6374 696f 6e73 223a 205b 0a20    "actions": [. 
+00015300: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00015310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015320: 6163 7469 6f6e 223a 2022 5255 4e5f 434f  action": "RUN_CO
+00015330: 4d4d 414e 4422 2c0a 2020 2020 2020 2020  MMAND",.        
+00015340: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
+00015350: 2273 7461 7274 5f73 696d 706c 655f 736c  "start_simple_sl
+00015360: 7572 6d64 222c 0a20 2020 2020 2020 2020  urmd",.         
+00015370: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
+00015380: 7322 3a20 5b22 7b7b 6e6f 6465 7342 7954  s": ["{{nodesByT
+00015390: 7970 652e 736c 7572 6d63 746c 642e 302e  ype.slurmctld.0.
+000153a0: 6465 7461 696c 732e 7072 6976 6174 6549  details.privateI
+000153b0: 7041 6464 7265 7373 7d7d 222c 2022 7b7b  pAddress}}", "{{
+000153c0: 6e6f 6465 2e64 6574 6169 6c73 2e6e 6f64  node.details.nod
+000153d0: 6553 6c6f 747d 7d22 5d2c 0a20 2020 2020  eSlot}}"],.     
+000153e0: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
+000153f0: 5479 7065 7322 3a20 5b22 736c 7572 6d64  Types": ["slurmd
+00015400: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00015410: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
+00015420: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
+00015430: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00015440: 2020 2020 2020 2261 6374 696f 6e73 223a        "actions":
+00015450: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00015460: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00015470: 2020 2022 6163 7469 6f6e 223a 2022 4352     "action": "CR
+00015480: 4541 5445 5f57 4f52 4b45 5253 222c 0a20  EATE_WORKERS",. 
+00015490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000154a0: 746f 7461 6c57 6f72 6b65 7273 223a 2031  totalWorkers": 1
+000154b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000154c0: 2020 226e 6f64 6554 7970 6573 223a 205b    "nodeTypes": [
+000154d0: 2273 6c75 726d 6374 6c64 225d 0a20 2020  "slurmctld"].   
+000154e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000154f0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00015500: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
+00015510: 2c0a 2020 2020 2020 2020 224e 4f44 4553  ,.        "NODES
+00015520: 5f41 4444 4544 223a 205b 0a20 2020 2020  _ADDED": [.     
+00015530: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00015540: 2020 2022 6163 7469 6f6e 7322 3a20 5b0a     "actions": [.
+00015550: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 2261 6374 696f 6e22 3a20 2257 5249 5445  "action": "WRITE
+00015580: 5f46 494c 4522 2c0a 2020 2020 2020 2020  _FILE",.        
+00015590: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
+000155a0: 226e 6f64 6573 2e6a 736f 6e22 2c0a 2020  "nodes.json",.  
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000155c0: 6f6e 7465 6e74 223a 2022 7b5c 6e20 205c  ontent": "{\n  \
+000155d0: 226e 6f64 6573 5c22 3a20 5b5c 6e7b 7b23  "nodes\": [\n{{#
+000155e0: 6669 6c74 6572 6564 4e6f 6465 737d 7d5c  filteredNodes}}\
+000155f0: 6e20 2020 207b 5c6e 2020 2020 2020 5c22  n    {\n      \"
+00015600: 6e61 6d65 5c22 3a20 5c22 736c 7572 6d64  name\": \"slurmd
+00015610: 7b7b 6465 7461 696c 732e 6e6f 6465 536c  {{details.nodeSl
+00015620: 6f74 7d7d 5c22 2c5c 6e20 2020 2020 205c  ot}}\",\n      \
+00015630: 2269 705c 223a 205c 227b 7b64 6574 6169  "ip\": \"{{detai
+00015640: 6c73 2e70 7269 7661 7465 4970 4164 6472  ls.privateIpAddr
+00015650: 6573 737d 7d5c 225c 6e20 2020 207d 7b7b  ess}}\"\n    }{{
+00015660: 5e2d 6c61 7374 7d7d 2c7b 7b2f 2d6c 6173  ^-last}},{{/-las
+00015670: 747d 7d5c 6e7b 7b2f 6669 6c74 6572 6564  t}}\n{{/filtered
+00015680: 4e6f 6465 737d 7d5c 6e20 205d 5c6e 7d22  Nodes}}\n  ]\n}"
+00015690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000156a0: 2020 226e 6f64 6554 7970 6573 223a 205b    "nodeTypes": [
+000156b0: 2273 6c75 726d 6374 6c64 225d 0a20 2020  "slurmctld"].   
+000156c0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000156d0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+000156f0: 6374 696f 6e22 3a20 2252 554e 5f43 4f4d  ction": "RUN_COM
+00015700: 4d41 4e44 222c 0a20 2020 2020 2020 2020  MAND",.         
+00015710: 2020 2020 2020 2022 7061 7468 223a 2022         "path": "
+00015720: 6164 645f 6e6f 6465 7322 2c0a 2020 2020  add_nodes",.    
+00015730: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
+00015740: 756d 656e 7473 223a 205b 226e 6f64 6573  uments": ["nodes
+00015750: 2e6a 736f 6e22 5d2c 0a20 2020 2020 2020  .json"],.       
+00015760: 2020 2020 2020 2020 2022 6e6f 6465 5479           "nodeTy
+00015770: 7065 7322 3a20 5b22 736c 7572 6d63 746c  pes": ["slurmctl
+00015780: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
+00015790: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+000157a0: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
+000157b0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000157c0: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
+000157d0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000157e0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000157f0: 2020 2020 2261 6374 696f 6e22 3a20 2252      "action": "R
+00015800: 554e 5f43 4f4d 4d41 4e44 222c 0a20 2020  UN_COMMAND",.   
+00015810: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+00015820: 7468 223a 2022 7374 6172 745f 7369 6d70  th": "start_simp
+00015830: 6c65 5f73 6c75 726d 6422 2c0a 2020 2020  le_slurmd",.    
+00015840: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
+00015850: 756d 656e 7473 223a 205b 227b 7b6e 6f64  uments": ["{{nod
+00015860: 6573 4279 5479 7065 2e73 6c75 726d 6374  esByType.slurmct
+00015870: 6c64 2e30 2e64 6574 6169 6c73 2e70 7269  ld.0.details.pri
+00015880: 7661 7465 4970 4164 6472 6573 737d 7d22  vateIpAddress}}"
+00015890: 2c20 227b 7b6e 6f64 652e 6465 7461 696c  , "{{node.detail
+000158a0: 732e 6e6f 6465 536c 6f74 7d7d 225d 2c0a  s.nodeSlot}}"],.
+000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158c0: 226e 6f64 6549 6446 696c 7465 7222 3a20  "nodeIdFilter": 
+000158d0: 2245 5645 4e54 222c 0a20 2020 2020 2020  "EVENT",.       
+000158e0: 2020 2020 2020 2020 2022 6e6f 6465 5479           "nodeTy
+000158f0: 7065 7322 3a20 5b22 736c 7572 6d64 225d  pes": ["slurmd"]
+00015900: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
+00015910: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00015920: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00015930: 2020 205d 0a20 2020 2020 207d 0a20 2020     ].      }.   
+00015940: 207d 2c0a 2020 2020 2277 6f72 6b65 7254   },.    "workerT
+00015950: 6167 223a 2022 7079 6578 2d73 6c75 726d  ag": "pyex-slurm
+00015960: 2d63 6c75 7374 6572 220a 2020 7d0a 7d0a  -cluster".  }.}.
+00015970: 6060 600a 0a23 2323 2054 4f4d 4c20 5072  ```..### TOML Pr
+00015980: 6f70 6572 7469 6573 2049 6e68 6572 6974  operties Inherit
+00015990: 6564 2062 7920 576f 726b 6572 2050 6f6f  ed by Worker Poo
+000159a0: 6c20 4a53 4f4e 2053 7065 6369 6669 6361  l JSON Specifica
+000159b0: 7469 6f6e 730a 0a57 6865 6e20 6120 4a53  tions..When a JS
+000159c0: 4f4e 2057 6f72 6b65 7220 506f 6f6c 2073  ON Worker Pool s
+000159d0: 7065 6369 6669 6361 7469 6f6e 2069 7320  pecification is 
+000159e0: 7573 6564 2c20 7468 6520 666f 6c6c 6f77  used, the follow
+000159f0: 696e 6720 7072 6f70 6572 7469 6573 2066  ing properties f
+00015a00: 726f 6d20 7468 6520 6063 6f6e 6669 672e  rom the `config.
+00015a10: 746f 6d6c 6020 6669 6c65 2077 696c 6c20  toml` file will 
+00015a20: 6265 2069 6e68 6572 6974 6564 2069 6620  be inherited if 
+00015a30: 7468 6520 7661 6c75 6520 6973 2061 6273  the value is abs
+00015a40: 656e 7420 696e 2074 6865 204a 534f 4e20  ent in the JSON 
+00015a50: 6669 6c65 3a0a 0a2a 2a50 726f 7065 7274  file:..**Propert
+00015a60: 6965 7320 496e 6865 7269 7465 6420 7769  ies Inherited wi
+00015a70: 7468 696e 2074 6865 2060 7265 7175 6972  thin the `requir
+00015a80: 656d 656e 7454 656d 706c 6174 6555 7361  ementTemplateUsa
+00015a90: 6765 6020 7072 6f70 6572 7479 2a2a 0a0a  ge` property**..
+00015aa0: 2d20 6069 6d61 6765 7349 6460 0a2d 2060  - `imagesId`.- `
+00015ab0: 696e 7374 616e 6365 5461 6773 600a 2d20  instanceTags`.- 
+00015ac0: 6072 6571 7569 7265 6d65 6e74 4e61 6d65  `requirementName
+00015ad0: 603a 2064 6572 6976 6564 2066 726f 6d20  `: derived from 
+00015ae0: 7468 6520 606e 616d 6560 2070 726f 7065  the `name` prope
+00015af0: 7274 7920 696e 2074 6865 2060 544f 4d4c  rty in the `TOML
+00015b00: 6020 636f 6e66 6967 7572 6174 696f 6e2e  ` configuration.
+00015b10: 2028 5468 6520 6e61 6d65 2077 696c 6c20   (The name will 
+00015b20: 6265 2067 656e 6572 6174 6564 2061 7574  be generated aut
+00015b30: 6f6d 6174 6963 616c 6c79 2069 6620 6e6f  omatically if no
+00015b40: 7420 7375 7070 6c69 6564 2069 6e20 6569  t supplied in ei
+00015b50: 7468 6572 2074 6865 2054 4f4d 4c20 6669  ther the TOML fi
+00015b60: 6c65 206f 7220 7468 6520 4a53 4f4e 2073  le or the JSON s
+00015b70: 7065 6369 6669 6361 7469 6f6e 2e29 0a2d  pecification.).-
+00015b80: 2060 7265 7175 6972 656d 656e 744e 616d   `requirementNam
+00015b90: 6573 7061 6365 603a 2064 6572 6976 6564  espace`: derived
+00015ba0: 2066 726f 6d20 7468 6520 606e 616d 6573   from the `names
+00015bb0: 7061 6365 6020 7072 6f70 6572 7479 2069  pace` property i
+00015bc0: 6e20 7468 6520 6054 4f4d 4c60 2063 6f6e  n the `TOML` con
+00015bd0: 6669 6775 7261 7469 6f6e 0a2d 2060 7265  figuration.- `re
+00015be0: 7175 6972 656d 656e 7454 6167 603a 203a  quirementTag`: :
+00015bf0: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
+00015c00: 6520 6074 6167 6020 7072 6f70 6572 7479  e `tag` property
+00015c10: 2069 6e20 7468 6520 6054 4f4d 4c60 2063   in the `TOML` c
+00015c20: 6f6e 6669 6775 7261 7469 6f6e 0a2d 2060  onfiguration.- `
+00015c30: 7461 7267 6574 496e 7374 616e 6365 436f  targetInstanceCo
+00015c40: 756e 7460 0a2d 2060 7465 6d70 6c61 7465  unt`.- `template
+00015c50: 4964 600a 2d20 6075 7365 7244 6174 6160  Id`.- `userData`
+00015c60: 0a2d 2060 7573 6572 4461 7461 4669 6c65  .- `userDataFile
+00015c70: 600a 2d20 6075 7365 7244 6174 6146 696c  `.- `userDataFil
+00015c80: 6573 600a 0a2a 2a50 726f 7065 7274 6965  es`..**Propertie
+00015c90: 7320 496e 6865 7269 7465 6420 7769 7468  s Inherited with
+00015ca0: 696e 2074 6865 2060 7072 6f76 6973 696f  in the `provisio
+00015cb0: 6e65 6450 726f 7065 7274 6965 7360 2050  nedProperties` P
+00015cc0: 726f 7065 7274 792a 2a0a 0a2d 2060 6964  roperty**..- `id
+00015cd0: 6c65 4e6f 6465 5368 7574 646f 776e 456e  leNodeShutdownEn
+00015ce0: 6162 6c65 6460 0a2d 2060 6964 6c65 4e6f  abled`.- `idleNo
+00015cf0: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
+00015d00: 7460 0a2d 2060 6964 6c65 506f 6f6c 5368  t`.- `idlePoolSh
+00015d10: 7574 646f 776e 456e 6162 6c65 6460 0a2d  utdownEnabled`.-
+00015d20: 2060 6964 6c65 506f 6f6c 5368 7574 646f   `idlePoolShutdo
+00015d30: 776e 5469 6d65 6f75 7460 0a2d 2060 6e6f  wnTimeout`.- `no
+00015d40: 6465 426f 6f74 5469 6d65 6f75 7460 0a2d  deBootTimeout`.-
+00015d50: 2060 776f 726b 6572 5461 6760 0a0a 2323   `workerTag`..##
+00015d60: 2056 6172 6961 626c 6520 5375 6273 7469   Variable Substi
+00015d70: 7475 7469 6f6e 7320 696e 2057 6f72 6b65  tutions in Worke
+00015d80: 7220 506f 6f6c 2050 726f 7065 7274 6965  r Pool Propertie
+00015d90: 730a 0a56 6172 6961 626c 6520 7375 6273  s..Variable subs
+00015da0: 7469 7475 7469 6f6e 7320 6361 6e20 6265  titutions can be
+00015db0: 2075 7365 6420 7769 7468 696e 2061 6e79   used within any
+00015dc0: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
+00015dd0: 696e 2054 4f4d 4c20 636f 6e66 6967 7572  in TOML configur
+00015de0: 6174 696f 6e20 6669 6c65 7320 6f72 2057  ation files or W
+00015df0: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
+00015e00: 6669 6c65 732e 2053 6565 2074 6865 2064  files. See the d
+00015e10: 6573 6372 6970 7469 6f6e 205b 6162 6f76  escription [abov
+00015e20: 655d 2823 7661 7269 6162 6c65 2d73 7562  e](#variable-sub
+00015e30: 7374 6974 7574 696f 6e73 2920 666f 7220  stitutions) for 
+00015e40: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
+00015e50: 7661 7269 6162 6c65 2073 7562 7374 6974  variable substit
+00015e60: 7574 696f 6e73 2e20 5468 6973 2069 7320  utions. This is 
+00015e70: 6120 706f 7765 7266 756c 2066 6561 7475  a powerful featu
+00015e80: 7265 2074 6861 7420 616c 6c6f 7773 2057  re that allows W
+00015e90: 6f72 6b65 7220 506f 6f6c 7320 746f 2062  orker Pools to b
+00015ea0: 6520 7061 7261 6d65 7465 7269 7365 6420  e parameterised 
+00015eb0: 6279 2073 7570 706c 7969 6e67 2076 616c  by supplying val
+00015ec0: 7565 7320 6f6e 2074 6865 2063 6f6d 6d61  ues on the comma
+00015ed0: 6e64 206c 696e 652c 2076 6961 2065 6e76  nd line, via env
+00015ee0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00015ef0: 6573 2c20 6f72 2076 6961 2074 6865 2054  es, or via the T
+00015f00: 4f4d 4c20 6669 6c65 2e0a 0a41 6e20 696d  OML file...An im
+00015f10: 706f 7274 616e 7420 6469 7374 696e 6374  portant distinct
+00015f20: 696f 6e20 2a2a 6f6e 6c79 2a2a 2077 6865  ion **only** whe
+00015f30: 6e20 7573 696e 6720 7661 7269 6162 6c65  n using variable
+00015f40: 2073 7562 7374 6974 7574 696f 6e73 2077   substitutions w
+00015f50: 6974 6869 6e20 576f 726b 6572 2050 6f6f  ithin Worker Poo
+00015f60: 6c20 4a53 4f4e 2064 6f63 756d 656e 7473  l JSON documents
+00015f70: 2069 7320 7468 6174 2065 6163 6820 6469   is that each di
+00015f80: 7265 6374 6976 6520 2a2a 6d75 7374 2062  rective **must b
+00015f90: 6520 7072 6563 6564 6564 2062 7920 6120  e preceded by a 
+00015fa0: 605f 5f60 2028 646f 7562 6c65 2075 6e64  `__` (double und
+00015fb0: 6572 7363 6f72 6529 2a2a 2074 6f20 6469  erscore)** to di
+00015fc0: 7361 6d62 6967 7561 7465 2069 7420 6672  sambiguate it fr
+00015fd0: 6f6d 2076 6172 6961 626c 6520 7375 6273  om variable subs
+00015fe0: 7469 7475 7469 6f6e 7320 7468 6174 2061  titutions that a
+00015ff0: 7265 2074 6f20 6265 2070 6173 7365 6420  re to be passed 
+00016000: 6469 7265 6374 6c79 2074 6f20 7468 6520  directly to the 
+00016010: 4150 492e 2046 6f72 2065 7861 6d70 6c65  API. For example
+00016020: 2c20 7573 653a 2060 5f5f 7b7b 7573 6572  , use: `__{{user
+00016030: 6e61 6d65 7d7d 6020 746f 2061 7070 6c79  name}}` to apply
+00016040: 2061 2073 7562 7374 6974 7574 696f 6e20   a substitution 
+00016050: 666f 7220 7468 6520 6075 7365 726e 616d  for the `usernam
+00016060: 6560 2064 6566 6175 6c74 2073 7562 7374  e` default subst
+00016070: 6974 7574 696f 6e2e 0a0a 2323 2044 7279  itution...## Dry
+00016080: 2d52 756e 6e69 6e67 2057 6f72 6b65 7220  -Running Worker 
+00016090: 506f 6f6c 2050 726f 7669 7369 6f6e 696e  Pool Provisionin
+000160a0: 670a 0a54 6f20 6578 616d 696e 6520 7468  g..To examine th
+000160b0: 6520 4a53 4f4e 2074 6861 7420 7769 6c6c  e JSON that will
+000160c0: 2061 6374 7561 6c6c 7920 6265 2073 656e   actually be sen
+000160d0: 7420 746f 2074 6865 2059 656c 6c6f 7744  t to the YellowD
+000160e0: 6f67 2041 5049 2061 6674 6572 2061 6c6c  og API after all
+000160f0: 2070 726f 6365 7373 696e 672c 2075 7365   processing, use
+00016100: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
+00016110: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
+00016120: 7469 6f6e 2077 6865 6e20 7275 6e6e 696e  tion when runnin
+00016130: 6720 6079 642d 7072 6f76 6973 696f 6e60  g `yd-provision`
+00016140: 2e20 5468 6973 2077 696c 6c20 7072 696e  . This will prin
+00016150: 7420 7468 6520 4a53 4f4e 2073 7065 6369  t the JSON speci
+00016160: 6669 6361 7469 6f6e 2066 6f72 2074 6865  fication for the
+00016170: 2057 6f72 6b65 7220 506f 6f6c 2e20 4e6f   Worker Pool. No
+00016180: 7468 696e 6720 7769 6c6c 2062 6520 7375  thing will be su
+00016190: 626d 6974 7465 6420 746f 2074 6865 2070  bmitted to the p
+000161a0: 6c61 7466 6f72 6d2e 0a0a 5468 6520 6765  latform...The ge
+000161b0: 6e65 7261 7465 6420 4a53 4f4e 2069 7320  nerated JSON is 
+000161c0: 7072 6f64 7563 6564 2061 6674 6572 2061  produced after a
+000161d0: 6c6c 2070 726f 6365 7373 696e 6720 2869  ll processing (i
+000161e0: 6e63 6f72 706f 7261 7469 6e67 2060 636f  ncorporating `co
+000161f0: 6e66 6967 2e74 6f6d 6c60 2070 726f 7065  nfig.toml` prope
+00016200: 7274 6965 732c 2076 6172 6961 626c 6520  rties, variable 
+00016210: 7375 6273 7469 7475 7469 6f6e 732c 2065  substitutions, e
+00016220: 7463 2e29 2068 6173 2062 6565 6e20 636f  tc.) has been co
+00016230: 6e63 6c75 6465 642c 2073 6f20 7468 6520  ncluded, so the 
+00016240: 6472 792d 7275 6e20 6973 2075 7365 6675  dry-run is usefu
+00016250: 6c20 666f 7220 696e 7370 6563 7469 6e67  l for inspecting
+00016260: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
+00016270: 616c 6c20 7468 6520 7072 6f63 6573 7369  all the processi
+00016280: 6e67 2074 6861 7427 7320 6265 656e 2070  ng that's been p
+00016290: 6572 666f 726d 6564 2e0a 0a54 6f20 7375  erformed...To su
+000162a0: 7070 7265 7373 2061 6c6c 206f 7574 7075  ppress all outpu
+000162b0: 7420 6578 6365 7074 2066 6f72 2074 6865  t except for the
+000162c0: 204a 534f 4e20 6974 7365 6c66 2c20 7573   JSON itself, us
+000162d0: 6520 7468 6520 602d 2d71 7569 6574 6020  e the `--quiet` 
+000162e0: 2860 2d71 6029 2063 6f6d 6d61 6e64 206c  (`-q`) command l
+000162f0: 696e 6520 6f70 7469 6f6e 2e0a 0a54 6865  ine option...The
+00016300: 204a 534f 4e20 6472 792d 7275 6e20 6f75   JSON dry-run ou
+00016310: 7470 7574 2063 6f75 6c64 2069 7473 656c  tput could itsel
+00016320: 6620 6265 2075 7365 6420 6279 2060 7964  f be used by `yd
+00016330: 2d70 726f 7669 7369 6f6e 602c 2069 6620  -provision`, if 
+00016340: 6361 7074 7572 6564 2069 6e20 6120 6669  captured in a fi
+00016350: 6c65 2c20 652e 672e 3a0a 0a60 6060 7368  le, e.g.:..```sh
+00016360: 656c 6c0a 7964 2d70 726f 7669 7369 6f6e  ell.yd-provision
+00016370: 202d 2d64 7279 2d72 756e 202d 7120 3e20   --dry-run -q > 
+00016380: 6d79 5f77 6f72 6b65 725f 706f 6f6c 2e6a  my_worker_pool.j
+00016390: 736f 6e0a 7964 2d70 726f 7669 7369 6f6e  son.yd-provision
+000163a0: 202d 7020 6d79 5f77 6f72 6b65 725f 706f   -p my_worker_po
+000163b0: 6f6c 2e6a 736f 6e0a 6060 600a 0a23 204a  ol.json.```..# J
+000163c0: 736f 6e6e 6574 2053 7570 706f 7274 0a0a  sonnet Support..
+000163d0: 496e 2061 6c6c 2063 6972 6375 6d73 7461  In all circumsta
+000163e0: 6e63 6573 2077 6865 7265 204a 534f 4e20  nces where JSON 
+000163f0: 6669 6c65 7320 6172 6520 7573 6564 2062  files are used b
+00016400: 7920 7468 6520 5079 7468 6f6e 2045 7861  y the Python Exa
+00016410: 6d70 6c65 7320 7363 7269 7074 732c 2020  mples scripts,  
+00016420: 2a2a 5b4a 736f 6e6e 6574 5d28 6874 7470  **[Jsonnet](http
+00016430: 733a 2f2f 6a73 6f6e 6e65 742e 6f72 6729  s://jsonnet.org)
+00016440: 2a2a 2066 696c 6573 2063 616e 2062 6520  ** files can be 
+00016450: 7573 6564 2069 6e73 7465 6164 2e20 5468  used instead. Th
+00016460: 6973 2061 6c6c 6f77 7320 7468 6520 7573  is allows the us
+00016470: 6520 6f66 204a 736f 6e6e 6574 2773 2070  e of Jsonnet's p
+00016480: 6f77 6572 6675 6c20 4a53 4f4e 2065 7874  owerful JSON ext
+00016490: 656e 7369 6f6e 732c 2069 6e63 6c75 6469  ensions, includi
+000164a0: 6e67 2063 6f6d 6d65 6e74 732c 2076 6172  ng comments, var
+000164b0: 6961 626c 6573 2c20 6675 6e63 7469 6f6e  iables, function
+000164c0: 732c 2065 7463 2e0a 0a41 2073 696d 706c  s, etc...A simpl
+000164d0: 6520 7573 6167 6520 6578 616d 706c 6520  e usage example 
+000164e0: 6d69 6768 7420 6265 3a0a 0a60 6060 7368  might be:..```sh
+000164f0: 656c 6c0a 7964 2d73 7562 6d69 7420 2d2d  ell.yd-submit --
+00016500: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
+00016510: 206d 795f 776f 726b 5f72 6571 2e6a 736f   my_work_req.jso
+00016520: 6e6e 6574 0a60 6060 0a0a 5468 6520 7573  nnet.```..The us
+00016530: 6520 6f66 2074 6865 2066 696c 656e 616d  e of the filenam
+00016540: 6520 6578 7465 6e73 696f 6e20 602e 6a73  e extension `.js
+00016550: 6f6e 6e65 7460 2077 696c 6c20 696e 766f  onnet` will invo
+00016560: 6b65 204a 736f 6e6e 6574 2065 7661 6c75  ke Jsonnet evalu
+00016570: 6174 696f 6e2e 2028 4e6f 7465 2074 6861  ation. (Note tha
+00016580: 7420 6120 7465 6d70 6f72 6172 7920 4a53  t a temporary JS
+00016590: 4f4e 2066 696c 6520 6973 2063 7265 6174  ON file is creat
+000165a0: 6564 2061 7320 7061 7274 206f 6620 4a73  ed as part of Js
+000165b0: 6f6e 6e65 7420 7072 6f63 6573 7369 6e67  onnet processing
+000165c0: 2c20 7768 6963 6820 796f 7520 6d61 7920  , which you may 
+000165d0: 7365 6520 7265 6665 7272 6564 2074 6f20  see referred to 
+000165e0: 696e 2065 7272 6f72 206d 6573 7361 6765  in error message
+000165f0: 733a 2074 6869 7320 6669 6c65 2077 696c  s: this file wil
+00016600: 6c20 6861 7665 2062 6565 6e20 6465 6c65  l have been dele
+00016610: 7465 6420 6265 666f 7265 2074 6865 2073  ted before the s
+00016620: 6372 6970 7420 7374 6f70 732e 290a 0a23  cript stops.)..#
+00016630: 2320 4a73 6f6e 6e65 7420 496e 7374 616c  # Jsonnet Instal
+00016640: 6c61 7469 6f6e 0a0a 4a73 6f6e 6e65 7420  lation..Jsonnet 
+00016650: 6973 202a 2a6e 6f74 2a2a 2069 6e73 7461  is **not** insta
+00016660: 6c6c 6564 2062 7920 6465 6661 756c 7420  lled by default 
+00016670: 7768 656e 2060 7965 6c6c 6f77 646f 672d  when `yellowdog-
+00016680: 7079 7468 6f6e 2d65 7861 6d70 6c65 7360  python-examples`
+00016690: 2069 7320 696e 7374 616c 6c65 642c 2062   is installed, b
+000166a0: 6563 6175 7365 2074 6865 2070 6163 6b61  ecause the packa
+000166b0: 6765 2068 6173 2062 696e 6172 7920 636f  ge has binary co
+000166c0: 6d70 6f6e 656e 7473 2077 6869 6368 2061  mponents which a
+000166d0: 7265 206e 6f74 2061 7661 696c 6162 6c65  re not available
+000166e0: 206f 6e20 5079 5049 2066 6f72 2061 6c6c   on PyPI for all
+000166f0: 2070 6c61 7466 6f72 6d73 2e20 4966 2079   platforms. If y
+00016700: 6f75 2074 7279 2074 6f20 7573 6520 6120  ou try to use a 
+00016710: 4a73 6f6e 6e65 7420 6669 6c65 2069 6e20  Jsonnet file in 
+00016720: 7468 6520 6162 7365 6e63 6520 6f66 204a  the absence of J
+00016730: 736f 6e6e 6574 2c20 7468 6520 7363 7269  sonnet, the scri
+00016740: 7074 7320 7769 6c6c 2070 7269 6e74 2061  pts will print a
+00016750: 6e20 6572 726f 7220 6d65 7373 6167 652c  n error message,
+00016760: 2061 6e64 2073 7567 6765 7374 2061 6e20   and suggest an 
+00016770: 696e 7374 616c 6c61 7469 6f6e 206d 6563  installation mec
+00016780: 6861 6e69 736d 2e0a 0a54 6f20 696e 7374  hanism...To inst
+00016790: 616c 6c20 4a73 6f6e 6e65 7420 6174 2074  all Jsonnet at t
+000167a0: 6865 2073 616d 6520 7469 6d65 2061 7320  he same time as 
+000167b0: 696e 7374 616c 6c69 6e67 206f 7220 7570  installing or up
+000167c0: 6461 7469 6e67 2074 6865 2050 7974 686f  dating the Pytho
+000167d0: 6e20 4578 616d 706c 6573 2073 6372 6970  n Examples scrip
+000167e0: 7473 2c20 6d6f 6469 6679 2074 6865 2069  ts, modify the i
+000167f0: 6e73 7461 6c6c 6174 696f 6e20 6173 2066  nstallation as f
+00016800: 6f6c 6c6f 7773 2074 6f20 696e 636c 7564  ollows to includ
+00016810: 6520 7468 6520 606a 736f 6e6e 6574 6020  e the `jsonnet` 
+00016820: 6f70 7469 6f6e 3a0a 0a60 6060 0a70 6970  option:..```.pip
+00016830: 2069 6e73 7461 6c6c 202d 5520 2279 656c   install -U "yel
+00016840: 6c6f 7764 6f67 2d70 7974 686f 6e2d 6578  lowdog-python-ex
+00016850: 616d 706c 6573 5b6a 736f 6e6e 6574 5d22  amples[jsonnet]"
+00016860: 0a60 6060 0a0a 546f 2069 6e73 7461 6c6c  .```..To install
+00016870: 204a 736f 6e6e 6574 2073 6570 6172 6174   Jsonnet separat
+00016880: 656c 7920 6672 6f6d 2060 7965 6c6c 6f77  ely from `yellow
+00016890: 646f 672d 7079 7468 6f6e 2d65 7861 6d70  dog-python-examp
+000168a0: 6c65 7360 2c20 7472 793a 0a0a 6060 6073  les`, try:..```s
+000168b0: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
+000168c0: 202d 5520 6a73 6f6e 6e65 740a 6060 600a   -U jsonnet.```.
+000168d0: 0a49 6620 7468 6973 2066 6169 6c73 2c20  .If this fails, 
+000168e0: 7472 793a 0a0a 6060 6073 6865 6c6c 0a70  try:..```shell.p
+000168f0: 6970 2069 6e73 7461 6c6c 202d 5520 6a73  ip install -U js
+00016900: 6f6e 6e65 742d 6269 6e61 7279 0a60 6060  onnet-binary.```
+00016910: 0a0a 4966 2062 6f74 6820 6f66 2074 6865  ..If both of the
+00016920: 7365 206d 6574 686f 6473 2066 6169 6c2c  se methods fail,
+00016930: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
+00016940: 656e 7375 7265 2074 6861 7420 7468 6520  ensure that the 
+00016950: 706c 6174 666f 726d 206f 6e20 7768 6963  platform on whic
+00016960: 6820 796f 7527 7265 2072 756e 6e69 6e67  h you're running
+00016970: 2068 6173 2074 6865 2072 6571 7569 7265   has the require
+00016980: 6420 6275 696c 6420 746f 6f6c 7320 6176  d build tools av
+00016990: 6169 6c61 626c 652c 2073 6f20 7468 6174  ailable, so that
+000169a0: 2074 6865 204a 736f 6e6e 6574 2062 696e   the Jsonnet bin
+000169b0: 6172 7920 636f 6d70 6f6e 656e 7473 2063  ary components c
+000169c0: 616e 2062 6520 6275 696c 7420 6c6f 6361  an be built loca
+000169d0: 6c6c 792e 2054 6865 2072 6571 7569 7265  lly. The require
+000169e0: 6420 6275 696c 6420 7061 636b 6167 6573  d build packages
+000169f0: 2076 6172 7920 6279 2070 6c61 7466 6f72   vary by platfor
+00016a00: 6d20 6275 7420 7573 7561 6c6c 7920 696e  m but usually in
+00016a10: 636c 7564 6520 6765 6e65 7261 6c20 6465  clude general de
+00016a20: 7665 6c6f 706d 656e 7420 746f 6f6c 7320  velopment tools 
+00016a30: 696e 636c 7564 696e 6720 6120 432b 2b20  including a C++ 
+00016a40: 636f 6d70 696c 6572 2c20 616e 6420 5079  compiler, and Py
+00016a50: 7468 6f6e 2064 6576 656c 6f70 6d65 6e74  thon development
+00016a60: 2074 6f6f 6c73 2069 6e63 6c75 6469 6e67   tools including
+00016a70: 2074 6865 2050 7974 686f 6e20 6865 6164   the Python head
+00016a80: 6572 732e 0a0a 506c 6561 7365 2067 6574  ers...Please get
+00016a90: 2069 6e20 746f 7563 6820 7769 7468 2059   in touch with Y
+00016aa0: 656c 6c6f 7744 6f67 2069 6620 796f 7520  ellowDog if you 
+00016ab0: 6765 7420 7374 7563 6b2e 0a0a 2323 2056  get stuck...## V
+00016ac0: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
+00016ad0: 7469 6f6e 7320 696e 204a 736f 6e6e 6574  tions in Jsonnet
+00016ae0: 2046 696c 6573 0a0a 5468 6520 7363 7269   Files..The scri
+00016af0: 7074 7320 7072 6f76 6964 6520 6675 6c6c  pts provide full
+00016b00: 2073 7570 706f 7274 2066 6f72 2076 6172   support for var
+00016b10: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00016b20: 6f6e 7320 696e 204a 736f 6e6e 6574 2066  ons in Jsonnet f
+00016b30: 696c 6573 2c20 7573 696e 6720 7468 6520  iles, using the 
+00016b40: 7361 6d65 2072 756c 6573 2061 7320 666f  same rules as fo
+00016b50: 7220 7468 6520 4a53 4f4e 2073 7065 6369  r the JSON speci
+00016b60: 6669 6361 7469 6f6e 732e 2052 656d 656d  fications. Remem
+00016b70: 6265 7220 7468 6174 2066 6f72 202a 2a57  ber that for **W
+00016b80: 6f72 6b65 7220 506f 6f6c 2a2a 2073 7065  orker Pool** spe
+00016b90: 6369 6669 6361 7469 6f6e 732c 2076 6172  cifications, var
+00016ba0: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00016bb0: 6f6e 7320 6d75 7374 2062 6520 7072 6566  ons must be pref
+00016bc0: 6978 6564 2062 7920 605f 5f60 2c20 652e  ixed by `__`, e.
+00016bd0: 672e 2060 225f 5f7b 7b75 7365 726e 616d  g. `"__{{usernam
+00016be0: 657d 7d7d 2260 2e0a 0a56 6172 6961 626c  e}}}"`...Variabl
+00016bf0: 6520 7375 6273 7469 7475 7469 6f6e 2069  e substitution i
+00016c00: 7320 7065 7266 6f72 6d65 6420 6265 666f  s performed befo
+00016c10: 7265 204a 736f 6e6e 6574 2065 7870 616e  re Jsonnet expan
+00016c20: 7369 6f6e 2069 6e74 6f20 4a53 4f4e 2c20  sion into JSON, 
+00016c30: 616e 6420 6167 6169 6e20 6166 7465 7220  and again after 
+00016c40: 7468 6520 6578 7061 6e73 696f 6e2e 0a0a  the expansion...
+00016c50: 2323 2043 6865 636b 696e 6720 4a73 6f6e  ## Checking Json
+00016c60: 6e65 7420 5072 6f63 6573 7369 6e67 0a0a  net Processing..
+00016c70: 5468 6572 6520 6172 6520 7468 7265 6520  There are three 
+00016c80: 706f 7373 6962 696c 6974 6965 7320 666f  possibilities fo
+00016c90: 7220 7665 7269 6679 696e 6720 7468 6174  r verifying that
+00016ca0: 2061 204a 736f 6e6e 6574 2073 7065 6369   a Jsonnet speci
+00016cb0: 6669 6361 7469 6f6e 2069 7320 646f 696e  fication is doin
+00016cc0: 6720 7768 6174 2069 7320 696e 7465 6e64  g what is intend
+00016cd0: 6564 3a0a 0a31 2e20 546f 2069 6e73 7065  ed:..1. To inspe
+00016ce0: 6374 2074 6865 2062 6173 6963 2063 6f6e  ct the basic con
+00016cf0: 7665 7273 696f 6e20 6f66 204a 736f 6e6e  version of Jsonn
+00016d00: 6574 2069 6e74 6f20 4a53 4f4e 2c20 7769  et into JSON, wi
+00016d10: 7468 6f75 7420 616e 7920 6164 6469 7469  thout any additi
+00016d20: 6f6e 616c 2070 726f 6365 7373 696e 6720  onal processing 
+00016d30: 6279 2074 6865 2050 7974 686f 6e20 4578  by the Python Ex
+00016d40: 616d 706c 6573 2073 6372 6970 7473 2c20  amples scripts, 
+00016d50: 7468 6520 6079 642d 6a73 6f6e 6e65 7432  the `yd-jsonnet2
+00016d60: 6a73 6f6e 6020 636f 6d6d 616e 6420 6361  json` command ca
+00016d70: 6e20 6265 2075 7365 642e 2054 6869 7320  n be used. This 
+00016d80: 7461 6b65 7320 6120 7369 6e67 6c65 2063  takes a single c
+00016d90: 6f6d 6d61 6e64 206c 696e 6520 6172 6775  ommand line argu
+00016da0: 6d65 6e74 2077 6869 6368 2069 7320 7468  ment which is th
+00016db0: 6520 6e61 6d65 206f 6620 7468 6520 6a73  e name of the js
+00016dc0: 6f6e 6e65 7420 6669 6c65 2074 6f20 6265  onnet file to be
+00016dd0: 2070 726f 6365 7373 6564 3a0a 0a60 6060   processed:..```
+00016de0: 7368 656c 6c0a 7964 2d6a 736f 6e6e 6574  shell.yd-jsonnet
+00016df0: 326a 736f 6e20 6d79 5f66 696c 652e 6a73  2json my_file.js
+00016e00: 6f6e 6e65 740a 6060 600a 0a0a 322e 2054  onnet.```...2. T
+00016e10: 6865 2060 6a73 6f6e 6e65 742d 6472 792d  he `jsonnet-dry-
+00016e20: 7275 6e60 2028 602d 4a60 2920 6f70 7469  run` (`-J`) opti
+00016e30: 6f6e 206f 6620 7468 6520 6079 642d 7375  on of the `yd-su
+00016e40: 626d 6974 602c 2060 7964 2d70 726f 7669  bmit`, `yd-provi
+00016e50: 7369 6f6e 6020 616e 6420 6079 642d 696e  sion` and `yd-in
+00016e60: 7374 616e 7469 6174 6560 2063 6f6d 6d61  stantiate` comma
+00016e70: 6e64 7320 7769 6c6c 2067 656e 6572 6174  nds will generat
+00016e80: 6520 4a53 4f4e 206f 7574 7075 7420 7265  e JSON output re
+00016e90: 7072 6573 656e 7469 6e67 2074 6865 204a  presenting the J
+00016ea0: 736f 6e6e 6574 2074 6f20 4a53 4f4e 2070  sonnet to JSON p
+00016eb0: 726f 6365 7373 696e 6720 6f6e 6c79 2c20  rocessing only, 
+00016ec0: 696e 636c 7564 696e 6720 6170 706c 6963  including applic
+00016ed0: 6162 6c65 2076 6172 6961 626c 6520 7375  able variable su
+00016ee0: 6273 7469 7475 7469 6f6e 732c 2062 7574  bstitutions, but
+00016ef0: 2062 6566 6f72 6520 6675 6c6c 2070 726f   before full pro
+00016f00: 7065 7274 7920 6578 7061 6e73 696f 6e20  perty expansion 
+00016f10: 696e 746f 2074 6865 204a 534f 4e20 7468  into the JSON th
+00016f20: 6174 2077 696c 6c20 6265 2073 7562 6d69  at will be submi
+00016f30: 7474 6564 2074 6f20 7468 6520 506c 6174  tted to the Plat
+00016f40: 666f 726d 2e0a 0a0a 332e 2054 6865 2060  form....3. The `
+00016f50: 6472 792d 7275 6e60 2028 602d 4460 2920  dry-run` (`-D`) 
+00016f60: 6f70 7469 6f6e 2077 696c 6c20 6765 6e65  option will gene
+00016f70: 7261 7465 204a 534f 4e20 6f75 7470 7574  rate JSON output
+00016f80: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+00016f90: 6520 6675 6c6c 2070 726f 6365 7373 696e  e full processin
+00016fa0: 6720 6f66 2074 6865 204a 736f 6e6e 6574  g of the Jsonnet
+00016fb0: 2066 696c 6520 696e 746f 2077 6861 7420   file into what 
+00016fc0: 7769 6c6c 2062 6520 7375 626d 6974 7465  will be submitte
+00016fd0: 6420 746f 2074 6865 2041 5049 2e20 5468  d to the API. Th
+00016fe0: 6973 2061 6c6c 6f77 7320 696e 7370 6563  is allows inspec
+00016ff0: 7469 6f6e 2074 6f20 6368 6563 6b20 7468  tion to check th
+00017000: 6174 2074 6865 206f 7574 7075 7420 6d61  at the output ma
+00017010: 7463 6865 7320 6578 7065 6374 6174 696f  tches expectatio
+00017020: 6e73 2c20 7072 696f 7220 746f 2073 7562  ns, prior to sub
+00017030: 6d69 7474 696e 6720 746f 2074 6865 2050  mitting to the P
+00017040: 6c61 7466 6f72 6d2e 0a0a 2323 204a 736f  latform...## Jso
+00017050: 6e6e 6574 2045 7861 6d70 6c65 0a0a 4865  nnet Example..He
+00017060: 7265 2773 2061 6e20 6578 616d 706c 6520  re's an example 
+00017070: 6f66 2061 204a 736f 6e6e 6574 2066 696c  of a Jsonnet fil
+00017080: 6520 7468 6174 2067 656e 6572 6174 6573  e that generates
+00017090: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
+000170a0: 656e 7420 7769 7468 2066 6f75 7220 5461  ent with four Ta
+000170b0: 736b 733a 0a0a 6060 606a 736f 6e6e 6574  sks:..```jsonnet
+000170c0: 0a23 2046 756e 6374 696f 6e20 666f 7220  .# Function for 
+000170d0: 7379 6e74 6865 7369 7369 6e67 2054 6173  synthesising Tas
+000170e0: 6b73 0a6c 6f63 616c 2054 6173 6b28 6172  ks.local Task(ar
+000170f0: 6775 6d65 6e74 733d 5b5d 2c20 656e 7669  guments=[], envi
+00017100: 726f 6e6d 656e 743d 7b7d 2920 3d20 7b0a  ronment={}) = {.
+00017110: 2020 2020 6172 6775 6d65 6e74 733a 2061      arguments: a
+00017120: 7267 756d 656e 7473 2c0a 2020 2020 656e  rguments,.    en
+00017130: 7669 726f 6e6d 656e 743a 2065 6e76 6972  vironment: envir
+00017140: 6f6e 6d65 6e74 2c0a 2020 2020 6e61 6d65  onment,.    name
+00017150: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
+00017160: 6b5f 6e75 6d62 6572 7d7d 220a 7d3b 0a0a  k_number}}".};..
+00017170: 2320 576f 726b 2052 6571 7569 7265 6d65  # Work Requireme
+00017180: 6e74 0a7b 0a20 2022 6e61 6d65 223a 2022  nt.{.  "name": "
+00017190: 776f 726b 7265 715f 7b7b 6461 7465 7469  workreq_{{dateti
+000171a0: 6d65 7d7d 222c 0a20 2022 7461 736b 4772  me}}",.  "taskGr
+000171b0: 6f75 7073 223a 205b 0a20 2020 207b 0a20  oups": [.    {. 
+000171c0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
+000171d0: 2020 2020 2020 2020 5461 736b 285b 2231          Task(["1
+000171e0: 225d 2c20 7b41 3a20 2241 5f31 227d 292c  "], {A: "A_1"}),
+000171f0: 2020 2320 6172 6775 6d65 6e74 7320 616e    # arguments an
+00017200: 6420 656e 7669 726f 6e6d 656e 740a 2020  d environment.  
+00017210: 2020 2020 2020 5461 736b 285b 2232 222c        Task(["2",
+00017220: 2022 3322 5d2c 207b 7d29 2c20 2020 2020   "3"], {}),     
+00017230: 2320 6172 6775 6d65 6e74 7320 616e 6420  # arguments and 
+00017240: 656d 7074 7920 656e 7669 726f 6e6d 656e  empty environmen
+00017250: 740a 2020 2020 2020 2020 5461 736b 285b  t.        Task([
+00017260: 2234 225d 292c 2020 2020 2020 2020 2020  "4"]),          
+00017270: 2020 2020 2320 6172 6775 6d65 6e74 7320      # arguments 
+00017280: 616e 6420 6465 6661 756c 7420 656e 7669  and default envi
+00017290: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
+000172a0: 5461 736b 2829 2020 2020 2020 2020 2020  Task()          
+000172b0: 2020 2020 2020 2020 2020 2320 6465 6661            # defa
+000172c0: 756c 7420 6172 6775 6d65 6e74 7320 616e  ult arguments an
+000172d0: 6420 656e 7669 726f 6e6d 656e 740a 2020  d environment.  
+000172e0: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
+000172f0: 7d0a 6060 600a 0a57 6865 6e20 7468 6973  }.```..When this
+00017300: 2069 7320 696e 7370 6563 7465 6420 7573   is inspected us
+00017310: 696e 6720 7468 6520 606a 736f 6e6e 6574  ing the `jsonnet
+00017320: 2d64 7279 2d72 756e 6020 6f70 7469 6f6e  -dry-run` option
+00017330: 2028 6079 642d 7375 626d 6974 202d 4a71   (`yd-submit -Jq
+00017340: 202d 7220 6d79 5f77 6f72 6b5f 7265 712e   -r my_work_req.
+00017350: 6a73 6f6e 6e65 7460 292c 2074 6869 7320  jsonnet`), this 
+00017360: 6973 2074 6865 2070 726f 6365 7373 6564  is the processed
+00017370: 206f 7574 7075 743a 0a0a 6060 606a 736f   output:..```jso
+00017380: 6e0a 7b0a 2020 226e 616d 6522 3a20 2277  n.{.  "name": "w
+00017390: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
+000173a0: 3036 3435 222c 0a20 2022 7461 736b 4772  0645",.  "taskGr
+000173b0: 6f75 7073 223a 205b 0a20 2020 207b 0a20  oups": [.    {. 
+000173c0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
+000173d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000173e0: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
+000173f0: 205b 2231 225d 2c0a 2020 2020 2020 2020   ["1"],.        
+00017400: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
+00017410: 207b 2241 223a 2022 415f 3122 7d2c 0a20   {"A": "A_1"},. 
+00017420: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+00017430: 2022 6d79 5f74 6173 6b5f 7b7b 7461 736b   "my_task_{{task
+00017440: 5f6e 756d 6265 727d 7d22 0a20 2020 2020  _number}}".     
+00017450: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00017460: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
+00017470: 656e 7473 223a 205b 2232 222c 2022 3322  ents": ["2", "3"
+00017480: 5d2c 0a20 2020 2020 2020 2020 2022 656e  ],.          "en
+00017490: 7669 726f 6e6d 656e 7422 3a20 7b7d 2c0a  vironment": {},.
+000174a0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+000174b0: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
+000174c0: 6b5f 6e75 6d62 6572 7d7d 220a 2020 2020  k_number}}".    
+000174d0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000174e0: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
+000174f0: 6d65 6e74 7322 3a20 5b22 3422 5d2c 0a20  ments": ["4"],. 
+00017500: 2020 2020 2020 2020 2022 656e 7669 726f           "enviro
+00017510: 6e6d 656e 7422 3a20 7b7d 2c0a 2020 2020  nment": {},.    
+00017520: 2020 2020 2020 226e 616d 6522 3a20 226d        "name": "m
+00017530: 795f 7461 736b 5f7b 7b74 6173 6b5f 6e75  y_task_{{task_nu
+00017540: 6d62 6572 7d7d 220a 2020 2020 2020 2020  mber}}".        
+00017550: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00017560: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
+00017570: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00017580: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
+00017590: 207b 7d2c 0a20 2020 2020 2020 2020 2022   {},.          "
+000175a0: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
+000175b0: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
+000175c0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+000175d0: 205d 0a20 2020 207d 0a20 205d 0a7d 0a60   ].    }.  ].}.`
+000175e0: 6060 0a0a 5768 656e 2074 6869 7320 6973  ``..When this is
+000175f0: 2069 6e73 7065 6374 6564 2075 7369 6e67   inspected using
+00017600: 2074 6865 2060 6472 792d 7275 6e60 206f   the `dry-run` o
+00017610: 7074 696f 6e20 2860 7964 2d73 7562 6d69  ption (`yd-submi
+00017620: 7420 2d44 7120 2d72 206d 795f 776f 726b  t -Dq -r my_work
+00017630: 5f72 6571 2e6a 736f 6e6e 6574 6029 2c20  _req.jsonnet`), 
+00017640: 7468 6973 2069 7320 7468 6520 7072 6f63  this is the proc
+00017650: 6573 7365 6420 6f75 7470 7574 3a0a 0a60  essed output:..`
+00017660: 6060 6a73 6f6e 0a7b 0a20 2022 6675 6c66  ``json.{.  "fulf
+00017670: 696c 4f6e 5375 626d 6974 223a 2066 616c  ilOnSubmit": fal
+00017680: 7365 2c0a 2020 226e 616d 6522 3a20 2277  se,.  "name": "w
+00017690: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
+000176a0: 3036 3435 222c 0a20 2022 6e61 6d65 7370  0645",.  "namesp
+000176b0: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
+000176c0: 7322 2c0a 2020 2270 7269 6f72 6974 7922  s",.  "priority"
+000176d0: 3a20 302c 0a20 2022 7461 6722 3a20 2270  : 0,.  "tag": "p
+000176e0: 7965 782d 6261 7368 222c 0a20 2022 7461  yex-bash",.  "ta
+000176f0: 736b 4772 6f75 7073 223a 205b 0a20 2020  skGroups": [.   
+00017700: 207b 0a20 2020 2020 2022 6669 6e69 7368   {.      "finish
+00017710: 4966 416c 6c54 6173 6b73 4669 6e69 7368  IfAllTasksFinish
+00017720: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00017730: 2022 6669 6e69 7368 4966 416e 7954 6173   "finishIfAnyTas
+00017740: 6b46 6169 6c65 6422 3a20 6661 6c73 652c  kFailed": false,
+00017750: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
+00017760: 7461 736b 5f67 726f 7570 5f31 222c 0a20  task_group_1",. 
+00017770: 2020 2020 2022 7072 696f 7269 7479 223a       "priority":
+00017780: 2030 2c0a 2020 2020 2020 2272 756e 5370   0,.      "runSp
+00017790: 6563 6966 6963 6174 696f 6e22 3a20 7b0a  ecification": {.
+000177a0: 2020 2020 2020 2020 226d 6178 696d 756d          "maximum
+000177b0: 5461 736b 5265 7472 6965 7322 3a20 302c  TaskRetries": 0,
+000177c0: 0a20 2020 2020 2020 2022 7461 736b 5479  .        "taskTy
+000177d0: 7065 7322 3a20 5b22 6261 7368 225d 2c0a  pes": ["bash"],.
+000177e0: 2020 2020 2020 2020 2277 6f72 6b65 7254          "workerT
+000177f0: 6167 7322 3a20 5b22 7079 6578 2d62 6173  ags": ["pyex-bas
+00017800: 682d 646f 636b 6572 225d 0a20 2020 2020  h-docker"].     
+00017810: 207d 2c0a 2020 2020 2020 2274 6173 6b73   },.      "tasks
+00017820: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00017830: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+00017840: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
+00017850: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
+00017860: 6565 705f 7363 7269 7074 2e73 6822 2c20  eep_script.sh", 
+00017870: 2231 225d 2c0a 2020 2020 2020 2020 2020  "1"],.          
+00017880: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00017890: 2241 223a 2022 415f 3122 7d2c 0a20 2020  "A": "A_1"},.   
+000178a0: 2020 2020 2020 2022 696e 7075 7473 223a         "inputs":
+000178b0: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
+000178c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000178d0: 6f62 6a65 6374 4e61 6d65 5061 7474 6572  objectNamePatter
+000178e0: 6e22 3a20 2277 6f72 6b72 6571 5f32 3330  n": "workreq_230
+000178f0: 3131 342d 3134 3036 3435 2f73 6c65 6570  114-140645/sleep
+00017900: 5f73 6372 6970 742e 7368 222c 0a20 2020  _script.sh",.   
+00017910: 2020 2020 2020 2020 2020 2022 736f 7572             "sour
+00017920: 6365 223a 2022 5441 534b 5f4e 414d 4553  ce": "TASK_NAMES
+00017930: 5041 4345 222c 0a20 2020 2020 2020 2020  PACE",.         
+00017940: 2020 2020 2022 7665 7269 6669 6361 7469       "verificati
+00017950: 6f6e 223a 2022 5645 5249 4659 5f41 545f  on": "VERIFY_AT_
+00017960: 5354 4152 5422 0a20 2020 2020 2020 2020  START".         
+00017970: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
+00017980: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
+00017990: 6522 3a20 226d 795f 7461 736b 5f31 222c  e": "my_task_1",
+000179a0: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
+000179b0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
+000179c0: 2020 2020 7b22 616c 7761 7973 5570 6c6f      {"alwaysUplo
+000179d0: 6164 223a 2074 7275 652c 2022 7265 7175  ad": true, "requ
+000179e0: 6972 6564 223a 2066 616c 7365 2c20 2273  ired": false, "s
+000179f0: 6f75 7263 6522 3a20 2250 524f 4345 5353  ource": "PROCESS
+00017a00: 5f4f 5554 5055 5422 7d0a 2020 2020 2020  _OUTPUT"}.      
+00017a10: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00017a20: 2022 7461 736b 5479 7065 223a 2022 6261   "taskType": "ba
+00017a30: 7368 220a 2020 2020 2020 2020 7d2c 0a20  sh".        },. 
+00017a40: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00017a50: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
+00017a60: 5b22 776f 726b 7265 715f 3233 3031 3134  ["workreq_230114
+00017a70: 2d31 3430 3634 352f 736c 6565 705f 7363  -140645/sleep_sc
+00017a80: 7269 7074 2e73 6822 2c20 2232 222c 2022  ript.sh", "2", "
+00017a90: 3322 5d2c 0a20 2020 2020 2020 2020 2022  3"],.          "
+00017aa0: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
+00017ab0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
+00017ac0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
+00017ad0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00017ae0: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
+00017af0: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
+00017b00: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
+00017b10: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
+00017b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017b30: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
+00017b40: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
+00017b50: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
+00017b60: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
+00017b70: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
+00017b80: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00017b90: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00017ba0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
+00017bb0: 6b5f 3222 2c0a 2020 2020 2020 2020 2020  k_2",.          
+00017bc0: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
+00017bd0: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
+00017be0: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
+00017bf0: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
+00017c00: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
+00017c10: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
+00017c20: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00017c30: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
+00017c40: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
+00017c50: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00017c60: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00017c70: 7473 223a 205b 2277 6f72 6b72 6571 5f32  ts": ["workreq_2
+00017c80: 3330 3131 342d 3134 3036 3435 2f73 6c65  30114-140645/sle
+00017c90: 6570 5f73 6372 6970 742e 7368 222c 2022  ep_script.sh", "
+00017ca0: 3422 5d2c 0a20 2020 2020 2020 2020 2022  4"],.          "
+00017cb0: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
+00017cc0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
+00017cd0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
+00017ce0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00017cf0: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
+00017d00: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
+00017d10: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
+00017d20: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
+00017d30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017d40: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
+00017d50: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
+00017d60: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
+00017d70: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
+00017d80: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
+00017d90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00017da0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00017db0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
+00017dc0: 6b5f 3322 2c0a 2020 2020 2020 2020 2020  k_3",.          
+00017dd0: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
+00017de0: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
+00017df0: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
+00017e00: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
+00017e10: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
+00017e20: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
+00017e30: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00017e40: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
+00017e50: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
+00017e60: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00017e70: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00017e80: 7473 223a 205b 2277 6f72 6b72 6571 5f32  ts": ["workreq_2
+00017e90: 3330 3131 342d 3134 3036 3435 2f73 6c65  30114-140645/sle
+00017ea0: 6570 5f73 6372 6970 742e 7368 225d 2c0a  ep_script.sh"],.
+00017eb0: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
+00017ec0: 6f6e 6d65 6e74 223a 207b 7d2c 0a20 2020  onment": {},.   
+00017ed0: 2020 2020 2020 2022 696e 7075 7473 223a         "inputs":
+00017ee0: 205b 0a20 2020 2020 2020 2020 2020 207b   [.            {
+00017ef0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00017f00: 6f62 6a65 6374 4e61 6d65 5061 7474 6572  objectNamePatter
+00017f10: 6e22 3a20 2277 6f72 6b72 6571 5f32 3330  n": "workreq_230
+00017f20: 3131 342d 3134 3036 3435 2f73 6c65 6570  114-140645/sleep
+00017f30: 5f73 6372 6970 742e 7368 222c 0a20 2020  _script.sh",.   
+00017f40: 2020 2020 2020 2020 2020 2022 736f 7572             "sour
+00017f50: 6365 223a 2022 5441 534b 5f4e 414d 4553  ce": "TASK_NAMES
+00017f60: 5041 4345 222c 0a20 2020 2020 2020 2020  PACE",.         
+00017f70: 2020 2020 2022 7665 7269 6669 6361 7469       "verificati
+00017f80: 6f6e 223a 2022 5645 5249 4659 5f41 545f  on": "VERIFY_AT_
+00017f90: 5354 4152 5422 0a20 2020 2020 2020 2020  START".         
+00017fa0: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
+00017fb0: 2c0a 2020 2020 2020 2020 2020 226e 616d  ,.          "nam
+00017fc0: 6522 3a20 226d 795f 7461 736b 5f34 222c  e": "my_task_4",
+00017fd0: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
+00017fe0: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
+00017ff0: 2020 2020 7b22 616c 7761 7973 5570 6c6f      {"alwaysUplo
+00018000: 6164 223a 2074 7275 652c 2022 7265 7175  ad": true, "requ
+00018010: 6972 6564 223a 2066 616c 7365 2c20 2273  ired": false, "s
+00018020: 6f75 7263 6522 3a20 2250 524f 4345 5353  ource": "PROCESS
+00018030: 5f4f 5554 5055 5422 7d0a 2020 2020 2020  _OUTPUT"}.      
+00018040: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00018050: 2022 7461 736b 5479 7065 223a 2022 6261   "taskType": "ba
+00018060: 7368 220a 2020 2020 2020 2020 7d0a 2020  sh".        }.  
+00018070: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
+00018080: 7d0a 6060 600a 0a23 2043 6f6d 6d61 6e64  }.```..# Command
+00018090: 204c 6973 740a 0a48 656c 7020 6973 2061   List..Help is a
+000180a0: 7661 696c 6162 6c65 2066 6f72 2061 6c6c  vailable for all
+000180b0: 2063 6f6d 6d61 6e64 7320 6279 2069 6e76   commands by inv
+000180c0: 6f6b 696e 6720 6120 636f 6d6d 616e 6420  oking a command 
+000180d0: 7769 7468 2074 6865 2060 2d2d 6865 6c70  with the `--help
+000180e0: 6020 6f72 2060 2d68 6020 6f70 7469 6f6e  ` or `-h` option
+000180f0: 2e20 536f 6d65 2063 6f6d 6d61 6e64 206c  . Some command l
+00018100: 696e 6520 7061 7261 6d65 7465 7273 2061  ine parameters a
+00018110: 7265 2063 6f6d 6d6f 6e20 746f 2061 6c6c  re common to all
+00018120: 2063 6f6d 6d61 6e64 732c 2077 6869 6c65   commands, while
+00018130: 206f 7468 6572 7320 6172 6520 636f 6d6d   others are comm
+00018140: 616e 642d 7370 6563 6966 6963 2e0a 0a41  and-specific...A
+00018150: 6c6c 2064 6573 7472 7563 7469 7665 2063  ll destructive c
+00018160: 6f6d 6d61 6e64 7320 7265 7175 6972 6520  ommands require 
+00018170: 7573 6572 2063 6f6e 6669 726d 6174 696f  user confirmatio
+00018180: 6e20 6265 666f 7265 2074 616b 696e 6720  n before taking 
+00018190: 6566 6665 6374 2e20 5468 6973 2063 616e  effect. This can
+000181a0: 2062 6520 7375 7070 7265 7373 6564 2075   be suppressed u
+000181b0: 7369 6e67 2074 6865 2060 2d2d 7965 7360  sing the `--yes`
+000181c0: 206f 7220 602d 7960 206f 7074 696f 6e2c   or `-y` option,
+000181d0: 2069 6e20 7768 6963 6820 6361 7365 2074   in which case t
+000181e0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
+000181f0: 7072 6f63 6565 6420 7769 7468 6f75 7420  proceed without 
+00018200: 636f 6e66 6972 6d61 7469 6f6e 2e0a 0a53  confirmation...S
+00018210: 6f6d 6520 636f 6d6d 616e 6473 2073 7570  ome commands sup
+00018220: 706f 7274 2074 6865 2060 2d2d 696e 7465  port the `--inte
+00018230: 7261 6374 6976 6560 206f 7220 602d 6960  ractive` or `-i`
+00018240: 206f 7074 696f 6e2c 2061 6c6c 6f77 696e   option, allowin
+00018250: 6720 7573 6572 2073 656c 6563 7469 6f6e  g user selection
+00018260: 7320 746f 2062 6520 6d61 6465 2e20 452e  s to be made. E.
+00018270: 672e 2c20 7468 6973 2063 616e 2062 6520  g., this can be 
+00018280: 7573 6564 2074 6f20 7365 6c65 6374 2077  used to select w
+00018290: 6869 6368 206f 626a 6563 7420 7061 7468  hich object path
+000182a0: 7320 746f 2064 656c 6574 652e 0a0a 5468  s to delete...Th
+000182b0: 6520 602d 2d71 7569 6574 6020 6f72 2060  e `--quiet` or `
+000182c0: 2d71 6020 6f70 7469 6f6e 2072 6564 7563  -q` option reduc
+000182d0: 6573 2074 6865 2063 6f6d 6d61 6e64 206f  es the command o
+000182e0: 7574 7075 7420 646f 776e 2074 6f20 6573  utput down to es
+000182f0: 7365 6e74 6961 6c20 6d65 7373 6167 6573  sential messages
+00018300: 206f 6e6c 792e 2053 6f2c 2066 6f72 2065   only. So, for e
+00018310: 7861 6d70 6c65 2c20 6079 642d 6465 6c65  xample, `yd-dele
+00018320: 7465 202d 7971 6020 776f 756c 6420 6465  te -yq` would de
+00018330: 6c65 7465 2061 6c6c 206d 6174 6368 696e  lete all matchin
+00018340: 6720 6f62 6a65 6374 2070 6174 6873 2073  g object paths s
+00018350: 696c 656e 746c 792e 0a0a 4966 2079 6f75  ilently...If you
+00018360: 2065 6e63 6f75 6e74 6572 2061 6e20 6572   encounter an er
+00018370: 726f 7220 6974 2063 616e 2062 6520 7573  ror it can be us
+00018380: 6566 756c 2066 6f72 2073 7570 706f 7274  eful for support
+00018390: 2070 7572 706f 7365 7320 746f 2073 6565   purposes to see
+000183a0: 2074 6865 2066 756c 6c20 5079 7468 6f6e   the full Python
+000183b0: 2073 7461 636b 2074 7261 6365 2e20 5468   stack trace. Th
+000183c0: 6973 2063 616e 2062 6520 656e 6162 6c65  is can be enable
+000183d0: 6420 6279 2072 756e 6e69 6e67 2074 6865  d by running the
+000183e0: 2063 6f6d 6d61 6e64 2075 7369 6e67 2074   command using t
+000183f0: 6865 2060 2d2d 6465 6275 6760 206f 7074  he `--debug` opt
+00018400: 696f 6e2e 0a0a 2323 2079 642d 7375 626d  ion...## yd-subm
+00018410: 6974 0a0a 5468 6520 6079 642d 7375 626d  it..The `yd-subm
+00018420: 6974 6020 636f 6d6d 616e 6420 7375 626d  it` command subm
+00018430: 6974 7320 6120 6e65 7720 576f 726b 2052  its a new Work R
+00018440: 6571 7569 7265 6d65 6e74 2c20 6163 636f  equirement, acco
+00018450: 7264 696e 6720 746f 2074 6865 2057 6f72  rding to the Wor
+00018460: 6b20 5265 7175 6972 656d 656e 7420 6465  k Requirement de
+00018470: 6669 6e69 7469 6f6e 2066 6f75 6e64 2069  finition found i
+00018480: 6e20 7468 6520 6077 6f72 6b52 6571 7569  n the `workRequi
+00018490: 7265 6d65 6e74 6020 7365 6374 696f 6e20  rement` section 
+000184a0: 6f66 2074 6865 2054 4f4d 4c20 636f 6e66  of the TOML conf
+000184b0: 6967 7572 6174 696f 6e20 6669 6c65 2061  iguration file a
+000184c0: 6e64 2f6f 7220 7468 6520 7370 6563 6966  nd/or the specif
+000184d0: 6963 6174 696f 6e20 666f 756e 6420 696e  ication found in
+000184e0: 2061 2057 6f72 6b20 5265 7175 6972 656d   a Work Requirem
+000184f0: 656e 7420 4a53 4f4e 2064 6f63 756d 656e  ent JSON documen
+00018500: 7420 7375 7070 6c69 6564 2075 7369 6e67  t supplied using
+00018510: 2074 6865 2060 2d2d 776f 726b 2d72 6571   the `--work-req
+00018520: 7569 7265 6d65 6e74 6020 6f70 7469 6f6e  uirement` option
+00018530: 2e0a 0a55 7365 2074 6865 2060 2d2d 6472  ...Use the `--dr
+00018540: 792d 7275 6e60 206f 7074 696f 6e20 746f  y-run` option to
+00018550: 2069 6e73 7065 6374 2074 6865 2064 6574   inspect the det
+00018560: 6169 6c73 206f 6620 7468 6520 576f 726b  ails of the Work
+00018570: 2052 6571 7569 7265 6d65 6e74 2c20 5461   Requirement, Ta
+00018580: 736b 2047 726f 7570 732c 2061 6e64 2054  sk Groups, and T
+00018590: 6173 6b73 2074 6861 7420 7769 6c6c 2062  asks that will b
+000185a0: 6520 7375 626d 6974 7465 642c 2069 6e20  e submitted, in 
+000185b0: 4a53 4f4e 2066 6f72 6d61 742e 0a0a 4f6e  JSON format...On
+000185c0: 6365 2073 7562 6d69 7474 6564 2c20 7468  ce submitted, th
+000185d0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+000185e0: 6e74 2077 696c 6c20 6170 7065 6172 2069  nt will appear i
+000185f0: 6e20 7468 6520 2a2a 576f 726b 2a2a 2074  n the **Work** t
+00018600: 6162 2069 6e20 7468 6520 5965 6c6c 6f77  ab in the Yellow
+00018610: 446f 6720 506f 7274 616c 2e0a 0a54 6865  Dog Portal...The
+00018620: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00018630: 7427 7320 7072 6f67 7265 7373 2063 616e  t's progress can
+00018640: 2062 6520 7472 6163 6b65 6420 746f 2063   be tracked to c
+00018650: 6f6d 706c 6574 696f 6e20 6279 2075 7369  ompletion by usi
+00018660: 6e67 2074 6865 2060 2d2d 666f 6c6c 6f77  ng the `--follow
+00018670: 6020 286f 7220 602d 6660 2920 6f70 7469  ` (or `-f`) opti
+00018680: 6f6e 2077 6865 6e20 696e 766f 6b69 6e67  on when invoking
+00018690: 2060 7964 2d73 7562 6d69 7460 3a20 7468   `yd-submit`: th
+000186a0: 6520 636f 6d6d 616e 6420 7769 6c6c 2072  e command will r
+000186b0: 6570 6f72 7420 6f6e 2054 6173 6b73 2061  eport on Tasks a
+000186c0: 7320 7468 6579 2063 6f6e 636c 7564 6520  s they conclude 
+000186d0: 616e 6420 776f 6e27 7420 7265 7475 726e  and won't return
+000186e0: 2075 6e74 696c 2074 6865 2057 6f72 6b20   until the Work 
+000186f0: 5265 7175 6972 656d 656e 7420 6861 7320  Requirement has 
+00018700: 6669 6e69 7368 6564 2e0a 0a23 2320 7964  finished...## yd
+00018710: 2d70 726f 7669 7369 6f6e 0a0a 5468 6520  -provision..The 
+00018720: 6079 642d 7072 6f76 6973 696f 6e60 2063  `yd-provision` c
+00018730: 6f6d 6d61 6e64 2070 726f 7669 7369 6f6e  ommand provision
+00018740: 7320 6120 6e65 7720 576f 726b 6572 2050  s a new Worker P
+00018750: 6f6f 6c20 6163 636f 7264 696e 6720 746f  ool according to
+00018760: 2074 6865 2073 7065 6369 6669 6361 7469   the specificati
+00018770: 6f6e 7320 696e 2074 6865 2060 776f 726b  ons in the `work
+00018780: 6572 506f 6f6c 6020 7365 6374 696f 6e20  erPool` section 
+00018790: 6f66 2074 6865 2054 4f4d 4c20 636f 6e66  of the TOML conf
+000187a0: 6967 7572 6174 696f 6e20 6669 6c65 2061  iguration file a
+000187b0: 6e64 2f6f 7220 696e 2074 6865 2073 7065  nd/or in the spe
+000187c0: 6369 6669 6361 7469 6f6e 2066 6f75 6e64  cification found
+000187d0: 2069 6e20 6120 576f 726b 6572 2050 6f6f   in a Worker Poo
+000187e0: 6c20 4a53 4f4e 2064 6f63 756d 656e 7420  l JSON document 
+000187f0: 7375 7070 6c69 6564 2075 7369 6e67 2074  supplied using t
+00018800: 6865 2060 2d2d 776f 726b 6572 2d70 6f6f  he `--worker-poo
+00018810: 6c60 206f 7074 696f 6e2e 0a0a 5573 6520  l` option...Use 
+00018820: 7468 6520 602d 2d64 7279 2d72 756e 6020  the `--dry-run` 
+00018830: 6f70 7469 6f6e 2074 6f20 696e 7370 6563  option to inspec
+00018840: 7420 7468 6520 6465 7461 696c 7320 6f66  t the details of
+00018850: 2074 6865 2057 6f72 6b65 7220 506f 6f6c   the Worker Pool
+00018860: 2073 7065 6369 6669 6361 7469 6f6e 2074   specification t
+00018870: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
+00018880: 6974 7465 642c 2069 6e20 4a53 4f4e 2066  itted, in JSON f
+00018890: 6f72 6d61 742e 0a0a 4f6e 6365 2070 726f  ormat...Once pro
+000188a0: 7669 7369 6f6e 6564 2c20 7468 6520 576f  visioned, the Wo
+000188b0: 726b 6572 2050 6f6f 6c20 7769 6c6c 2061  rker Pool will a
+000188c0: 7070 6561 7220 696e 2074 6865 202a 2a57  ppear in the **W
+000188d0: 6f72 6b65 7273 2a2a 2074 6162 2069 6e20  orkers** tab in 
+000188e0: 7468 6520 5965 6c6c 6f77 446f 6720 506f  the YellowDog Po
+000188f0: 7274 616c 2c20 616e 6420 6974 7320 6173  rtal, and its as
+00018900: 736f 6369 6174 6564 2043 6f6d 7075 7465  sociated Compute
+00018910: 2052 6571 7569 7265 6d65 6e74 2077 696c   Requirement wil
+00018920: 6c20 6170 7065 6172 2069 6e20 7468 6520  l appear in the 
+00018930: 2a2a 436f 6d70 7574 652a 2a20 7461 622e  **Compute** tab.
+00018940: 0a0a 2323 2079 642d 6361 6e63 656c 0a0a  ..## yd-cancel..
+00018950: 5468 6520 6079 642d 6361 6e63 656c 6020  The `yd-cancel` 
+00018960: 636f 6d6d 616e 6420 6361 6e63 656c 7320  command cancels 
+00018970: 616e 7920 6163 7469 7665 2057 6f72 6b20  any active Work 
+00018980: 5265 7175 6972 656d 656e 7473 2c20 696e  Requirements, in
+00018990: 636c 7564 696e 6720 616e 7920 7065 6e64  cluding any pend
+000189a0: 696e 6720 5461 736b 2047 726f 7570 7320  ing Task Groups 
+000189b0: 616e 6420 7468 6520 5461 736b 7320 7468  and the Tasks th
+000189c0: 6579 2063 6f6e 7461 696e 2e20 0a0a 5468  ey contain. ..Th
+000189d0: 6520 606e 616d 6573 7061 6365 6020 616e  e `namespace` an
+000189e0: 6420 6074 6167 6020 7661 6c75 6573 2069  d `tag` values i
+000189f0: 6e20 7468 6520 6063 6f6e 6669 672e 746f  n the `config.to
+00018a00: 6d6c 6020 6669 6c65 2061 7265 2075 7365  ml` file are use
+00018a10: 6420 746f 2069 6465 6e74 6966 7920 7768  d to identify wh
+00018a20: 6963 6820 576f 726b 2052 6571 7569 7265  ich Work Require
+00018a30: 6d65 6e74 7320 746f 2063 616e 6365 6c2e  ments to cancel.
+00018a40: 0a0a 4279 2064 6566 6175 6c74 2c20 616e  ..By default, an
+00018a50: 7920 5461 736b 7320 7468 6174 2061 7265  y Tasks that are
+00018a60: 2063 7572 7265 6e74 6c79 2072 756e 6e69   currently runni
+00018a70: 6e67 206f 6e20 576f 726b 6572 7320 7769  ng on Workers wi
+00018a80: 6c6c 2063 6f6e 7469 6e75 6520 746f 2072  ll continue to r
+00018a90: 756e 2074 6f20 636f 6d70 6c65 7469 6f6e  un to completion
+00018aa0: 206f 7220 756e 7469 6c20 7468 6579 2066   or until they f
+00018ab0: 6169 6c2e 2054 6173 6b73 2063 616e 2062  ail. Tasks can b
+00018ac0: 6520 696e 7374 7275 6374 6564 2074 6f20  e instructed to 
+00018ad0: 6162 6f72 7420 696d 6d65 6469 6174 656c  abort immediatel
+00018ae0: 7920 6279 2073 7570 706c 7969 6e67 2074  y by supplying t
+00018af0: 6865 2060 2d2d 6162 6f72 7460 206f 7220  he `--abort` or 
+00018b00: 602d 6160 206f 7074 696f 6e20 746f 2060  `-a` option to `
+00018b10: 7964 2d63 616e 6365 6c60 2e0a 0a23 2320  yd-cancel`...## 
+00018b20: 7964 2d61 626f 7274 0a0a 5468 6520 6079  yd-abort..The `y
+00018b30: 642d 6162 6f72 7460 2063 6f6d 6d61 6e64  d-abort` command
+00018b40: 2069 7320 7573 6564 2074 6f20 6162 6f72   is used to abor
+00018b50: 7420 5461 736b 7320 7468 6174 2061 7265  t Tasks that are
+00018b60: 2063 7572 7265 6e74 6c79 2072 756e 6e69   currently runni
+00018b70: 6e67 2e20 5468 6520 7573 6572 2069 6e74  ng. The user int
+00018b80: 6572 6163 7469 7665 6c79 2073 656c 6563  eractively selec
+00018b90: 7473 2074 6865 2057 6f72 6b20 5265 7175  ts the Work Requ
+00018ba0: 6972 656d 656e 7473 2074 6f20 7461 7267  irements to targ
+00018bb0: 6574 2c20 616e 6420 7468 656e 2077 6869  et, and then whi
+00018bc0: 6368 2054 6173 6b73 2077 6974 6869 6e20  ch Tasks within 
+00018bd0: 7468 6f73 6520 576f 726b 2052 6571 7569  those Work Requi
+00018be0: 7265 6d65 6e74 7320 746f 2061 626f 7274  rements to abort
+00018bf0: 2e20 5468 6520 576f 726b 2052 6571 7569  . The Work Requi
+00018c00: 7265 6d65 6e74 7320 6172 6520 6e6f 7420  rements are not 
+00018c10: 6361 6e63 656c 6c65 6420 6173 2070 6172  cancelled as par
+00018c20: 7420 6f66 2074 6869 7320 7072 6f63 6573  t of this proces
+00018c30: 732e 0a0a 5468 6520 606e 616d 6573 7061  s...The `namespa
+00018c40: 6365 6020 616e 6420 6074 6167 6020 7661  ce` and `tag` va
+00018c50: 6c75 6573 2069 6e20 7468 6520 6063 6f6e  lues in the `con
+00018c60: 6669 672e 746f 6d6c 6020 6669 6c65 2061  fig.toml` file a
+00018c70: 7265 2075 7365 6420 746f 2069 6465 6e74  re used to ident
+00018c80: 6966 7920 7768 6963 6820 576f 726b 2052  ify which Work R
+00018c90: 6571 7569 7265 6d65 6e74 7320 746f 206c  equirements to l
+00018ca0: 6973 7420 666f 7220 7365 6c65 6374 696f  ist for selectio
+00018cb0: 6e2e 0a0a 2323 2079 642d 646f 776e 6c6f  n...## yd-downlo
+00018cc0: 6164 0a0a 5468 6520 6079 642d 646f 776e  ad..The `yd-down
+00018cd0: 6c6f 6164 6020 636f 6d6d 616e 6420 646f  load` command do
+00018ce0: 776e 6c6f 6164 7320 616e 7920 6f62 6a65  wnloads any obje
+00018cf0: 6374 7320 6372 6561 7465 6420 696e 2074  cts created in t
+00018d00: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
+00018d10: 6563 7420 5374 6f72 652e 0a0a 5468 6520  ect Store...The 
+00018d20: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
+00018d30: 6074 6167 6020 7661 6c75 6573 2061 7265  `tag` values are
+00018d40: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
+00018d50: 6e65 2077 6869 6368 206f 626a 6563 7473  ne which objects
+00018d60: 2074 6f20 646f 776e 6c6f 6164 2e20 4f62   to download. Ob
+00018d70: 6a65 6374 7320 7769 6c6c 2062 6520 646f  jects will be do
+00018d80: 776e 6c6f 6164 6564 2074 6f20 6120 6469  wnloaded to a di
+00018d90: 7265 6374 6f72 7920 7769 7468 2074 6865  rectory with the
+00018da0: 2073 616d 6520 6e61 6d65 2061 7320 606e   same name as `n
+00018db0: 616d 6573 7061 6365 602e 2049 6620 6120  amespace`. If a 
+00018dc0: 6469 7265 6374 6f72 7920 616c 7265 6164  directory alread
+00018dd0: 7920 6578 6973 7473 2c20 6120 6e65 7720  y exists, a new 
+00018de0: 6469 7265 6374 6f72 7920 7769 7468 206e  directory with n
+00018df0: 616d 6520 603c 6e61 6d65 7370 6163 653e  ame `<namespace>
+00018e00: 2e30 3160 2028 6574 632e 2920 7769 6c6c  .01` (etc.) will
+00018e10: 2062 6520 6372 6561 7465 642e 0a0a 2323   be created...##
+00018e20: 2079 642d 6465 6c65 7465 0a0a 5468 6520   yd-delete..The 
+00018e30: 6079 642d 6465 6c65 7465 6020 636f 6d6d  `yd-delete` comm
+00018e40: 616e 6420 6465 6c65 7465 7320 616e 7920  and deletes any 
+00018e50: 6f62 6a65 6374 7320 6372 6561 7465 6420  objects created 
+00018e60: 696e 2074 6865 2059 656c 6c6f 7744 6f67  in the YellowDog
+00018e70: 204f 626a 6563 7420 5374 6f72 652e 0a0a   Object Store...
+00018e80: 5468 6520 606e 616d 6573 7061 6365 6020  The `namespace` 
+00018e90: 616e 6420 6074 6167 6020 7661 6c75 6573  and `tag` values
+00018ea0: 2069 6e20 7468 6520 6063 6f6e 6669 672e   in the `config.
+00018eb0: 746f 6d6c 6020 6669 6c65 2061 7265 2075  toml` file are u
+00018ec0: 7365 6420 746f 2069 6465 6e74 6966 7920  sed to identify 
+00018ed0: 7768 6963 6820 6f62 6a65 6374 7320 746f  which objects to
+00018ee0: 2064 656c 6574 652e 204e 6f74 6520 7468   delete. Note th
+00018ef0: 6174 2069 7427 7320 6561 7379 2074 6f20  at it's easy to 
+00018f00: 7573 6520 6079 642d 6465 6c65 7465 6020  use `yd-delete` 
+00018f10: 746f 2063 6c65 6172 2074 6865 2063 6f6e  to clear the con
+00018f20: 7465 6e74 7320 6f66 2061 206e 616d 6573  tents of a names
+00018f30: 7061 6365 2062 7920 7573 696e 6720 616e  pace by using an
+00018f40: 2065 6d70 7479 2060 7461 6760 2c20 6173   empty `tag`, as
+00018f50: 2066 6f6c 6c6f 7773 3a0a 0a60 6060 7368   follows:..```sh
+00018f60: 656c 6c0a 7964 2d64 656c 6574 6520 2d74  ell.yd-delete -t
+00018f70: 2022 220a 6060 600a 0a54 6869 7320 6361   "".```..This ca
+00018f80: 6e20 6265 2065 7874 656e 6465 6420 746f  n be extended to
+00018f90: 2061 6e79 206f 7468 6572 206e 616d 6573   any other names
+00018fa0: 7061 6365 2062 7920 7573 696e 6720 7468  pace by using th
+00018fb0: 6520 602d 2d6e 616d 6573 7061 6365 602f  e `--namespace`/
+00018fc0: 602d 6e60 206f 7074 696f 6e2e 0a0a 2323  `-n` option...##
+00018fd0: 2079 642d 7570 6c6f 6164 0a0a 5468 6520   yd-upload..The 
+00018fe0: 6079 642d 7570 6c6f 6164 6020 636f 6d6d  `yd-upload` comm
+00018ff0: 616e 6420 7570 6c6f 6164 7320 6669 6c65  and uploads file
+00019000: 7320 6672 6f6d 2074 6865 206c 6f63 616c  s from the local
+00019010: 2066 696c 6573 7973 7465 6d20 746f 2074   filesystem to t
+00019020: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
+00019030: 6563 7420 7374 6f72 652e 2046 696c 6573  ect store. Files
+00019040: 2061 7265 2070 6c61 6365 6420 696e 2074   are placed in t
+00019050: 6865 2063 6f6e 6669 6775 7265 6420 606e  he configured `n
+00019060: 616d 6573 7061 6365 6020 7769 7468 696e  amespace` within
+00019070: 2061 2064 6972 6563 746f 7279 2073 7570   a directory sup
+00019080: 706c 6965 6420 7573 696e 6720 7468 6520  plied using the 
+00019090: 2872 6571 7569 7265 6429 2060 2d2d 6469  (required) `--di
+000190a0: 7265 6374 6f72 7960 206f 7074 696f 6e2c  rectory` option,
+000190b0: 2065 2e67 2e3a 0a0a 6060 6073 6865 6c6c   e.g.:..```shell
+000190c0: 0a79 642d 7570 6c6f 6164 202d 2d64 6972  .yd-upload --dir
+000190d0: 6563 746f 7279 206d 795f 776f 726b 5f72  ectory my_work_r
+000190e0: 6571 7569 7265 6d65 6e74 2066 696c 655f  equirement file_
+000190f0: 3120 6669 6c65 5f32 206d 6f72 6566 696c  1 file_2 morefil
+00019100: 6573 2f66 696c 6533 0a60 6060 0a54 6f20  es/file3.```.To 
+00019110: 7375 7070 7265 7373 2074 6865 206d 6972  suppress the mir
+00019120: 726f 7269 6e67 206f 6620 7468 6520 6c6f  roring of the lo
+00019130: 6361 6c20 6469 7265 6374 6f72 7920 7374  cal directory st
+00019140: 7275 6374 7572 6520 7769 7468 696e 2074  ructure within t
+00019150: 6865 206f 626a 6563 7420 7374 6f72 652c  he object store,
+00019160: 2075 7365 2074 6865 2060 2d2d 666c 6174   use the `--flat
+00019170: 7465 6e2d 7570 6c6f 6164 2d70 6174 6873  ten-upload-paths
+00019180: 6020 6f72 2060 2d66 6020 6f70 7469 6f6e  ` or `-f` option
+00019190: 2e20 4e6f 7465 2074 6861 7420 6966 2074  . Note that if t
+000191a0: 6869 7320 6372 6561 7465 7320 6d75 6c74  his creates mult
+000191b0: 6970 6c65 2075 706c 6f61 6465 6420 6669  iple uploaded fi
+000191c0: 6c65 7320 7769 7468 2074 6865 2073 616d  les with the sam
+000191d0: 6520 7061 7468 2069 6e20 7468 6520 4f62  e path in the Ob
+000191e0: 6a65 6374 2053 746f 7265 2066 6f6c 6465  ject Store folde
+000191f0: 722c 2066 696c 6573 2077 696c 6c20 6265  r, files will be
+00019200: 206f 7665 7277 7269 7474 656e 2e0a 0a46   overwritten...F
+00019210: 696c 6573 2069 6e20 6469 7265 6374 6f72  iles in director
+00019220: 6965 7320 6d61 7920 6265 2072 6563 7572  ies may be recur
+00019230: 7369 7665 6c79 2075 706c 6f61 6465 6420  sively uploaded 
+00019240: 7573 696e 6720 7468 6520 602d 2d72 6563  using the `--rec
+00019250: 7572 7369 7665 6020 6f72 2060 2d72 6020  ursive` or `-r` 
+00019260: 6f70 7469 6f6e 2c20 652e 672e 3a0a 0a60  option, e.g.:..`
+00019270: 6060 7368 656c 6c0a 7964 2d75 706c 6f61  ``shell.yd-uploa
+00019280: 6420 2d2d 6469 7265 6374 6f72 7920 6d79  d --directory my
+00019290: 5f77 6f72 6b5f 7265 7175 6972 656d 656e  _work_requiremen
+000192a0: 7420 2d72 206d 7964 6972 206d 796f 7468  t -r mydir myoth
+000192b0: 6572 6469 720a 6060 600a 0a54 6f20 7570  erdir.```..To up
+000192c0: 6c6f 6164 2074 6f20 6f74 6865 7220 6e61  load to other na
+000192d0: 6d65 7370 6163 6573 2c20 7573 6520 7468  mespaces, use th
+000192e0: 6520 602d 2d6e 616d 6573 7061 6365 602f  e `--namespace`/
+000192f0: 602d 6e60 206f 7074 696f 6e2e 0a0a 2323  `-n` option...##
+00019300: 2079 642d 7368 7574 646f 776e 0a0a 5468   yd-shutdown..Th
+00019310: 6520 6079 642d 7368 7574 646f 776e 6020  e `yd-shutdown` 
+00019320: 636f 6d6d 616e 6420 7368 7574 7320 646f  command shuts do
+00019330: 776e 2057 6f72 6b65 7220 506f 6f6c 7320  wn Worker Pools 
+00019340: 7468 6174 206d 6174 6368 2074 6865 2060  that match the `
+00019350: 6e61 6d65 7370 6163 6560 2061 6e64 2060  namespace` and `
+00019360: 7461 6760 2066 6f75 6e64 2069 6e20 7468  tag` found in th
+00019370: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00019380: 6669 6c65 2e20 416c 6c20 7265 6d61 696e  file. All remain
+00019390: 696e 6720 776f 726b 2077 696c 6c20 6265  ing work will be
+000193a0: 2063 616e 6365 6c6c 6564 2c20 6275 7420   cancelled, but 
+000193b0: 6375 7272 656e 746c 7920 6578 6563 7574  currently execut
+000193c0: 696e 6720 5461 736b 7320 7769 6c6c 2062  ing Tasks will b
+000193d0: 6520 616c 6c6f 7765 6420 746f 2063 6f6d  e allowed to com
+000193e0: 706c 6574 652c 2061 6674 6572 2077 6869  plete, after whi
+000193f0: 6368 2074 6865 2043 6f6d 7075 7465 2052  ch the Compute R
+00019400: 6571 7569 7265 6d65 6e74 2077 696c 6c20  equirement will 
+00019410: 6265 2074 6572 6d69 6e61 7465 642e 0a0a  be terminated...
+00019420: 2323 2079 642d 696e 7374 616e 7469 6174  ## yd-instantiat
+00019430: 650a 0a54 6865 2060 7964 2d69 6e73 7461  e..The `yd-insta
+00019440: 6e74 6961 7465 6020 636f 6d6d 616e 6420  ntiate` command 
+00019450: 696e 7374 616e 7469 6174 6573 2061 2043  instantiates a C
+00019460: 6f6d 7075 7465 2052 6571 7569 7265 6d65  ompute Requireme
+00019470: 6e74 2028 692e 652e 2c20 6120 7365 7420  nt (i.e., a set 
+00019480: 6f66 2069 6e73 7461 6e63 6573 2074 6861  of instances tha
+00019490: 7420 6172 6520 6d61 6e61 6765 6420 6279  t are managed by
+000194a0: 2074 6865 6972 2063 7265 6174 6f72 2061   their creator a
+000194b0: 6e64 2064 6f20 6e6f 7420 6175 746f 6d61  nd do not automa
+000194c0: 7469 6361 6c6c 7920 6265 636f 6d65 2070  tically become p
+000194d0: 6172 7420 6f66 2061 2059 656c 6c6f 7744  art of a YellowD
+000194e0: 6f67 2057 6f72 6b65 7220 506f 6f6c 292e  og Worker Pool).
+000194f0: 0a0a 5468 6973 2063 6f6d 6d61 6e64 2075  ..This command u
+00019500: 7365 7320 7468 6520 6461 7461 2066 726f  ses the data fro
+00019510: 6d20 7468 6520 6077 6f72 6b65 7250 6f6f  m the `workerPoo
+00019520: 6c60 2063 6f6e 6669 6775 7261 7469 6f6e  l` configuration
+00019530: 2073 6563 7469 6f6e 2c20 6275 7420 6f6e   section, but on
+00019540: 6c79 2075 7365 7320 7468 6520 606e 616d  ly uses the `nam
+00019550: 6560 2c20 6074 656d 706c 6174 6549 6460  e`, `templateId`
+00019560: 2c20 6074 6172 6765 7449 6e73 7461 6e63  , `targetInstanc
+00019570: 6543 6f75 6e74 602c 2060 696e 7374 616e  eCount`, `instan
+00019580: 6365 5461 6773 602c 2060 7573 6572 4461  ceTags`, `userDa
+00019590: 7461 602c 2061 6e64 2060 696d 6167 6573  ta`, and `images
+000195a0: 4964 6020 7072 6f70 6572 7469 6573 2e20  Id` properties. 
+000195b0: 496e 2061 6464 6974 696f 6e2c 2074 6865  In addition, the
+000195c0: 2042 6f6f 6c65 616e 2070 726f 7065 7274   Boolean propert
+000195d0: 7920 606d 6169 6e74 6169 6e49 6e73 7461  y `maintainInsta
+000195e0: 6e63 6543 6f75 6e74 6020 2864 6566 6175  nceCount` (defau
+000195f0: 6c74 203d 2060 6661 6c73 6560 2920 6973  lt = `false`) is
+00019600: 2061 7661 696c 6162 6c65 2066 6f72 2075   available for u
+00019610: 7365 2077 6974 6820 6079 642d 696e 7374  se with `yd-inst
+00019620: 616e 7469 6174 6560 2e0a 0a43 6f6d 7075  antiate`...Compu
+00019630: 7465 2052 6571 7569 7265 6d65 6e74 7320  te Requirements 
+00019640: 6361 6e20 6265 2069 6e73 7461 6e74 6961  can be instantia
+00019650: 7465 6420 6469 7265 6374 6c79 2066 726f  ted directly fro
+00019660: 6d20 4a53 4f4e 2028 6f72 204a 736f 6e6e  m JSON (or Jsonn
+00019670: 6574 2920 7370 6563 6966 6963 6174 696f  et) specificatio
+00019680: 6e73 2c20 7573 696e 6720 7468 6520 602d  ns, using the `-
+00019690: 2d63 6f6d 7075 7465 2d72 6571 7569 7265  -compute-require
+000196a0: 6d65 6e74 6020 286f 7220 602d 4360 2920  ment` (or `-C`) 
+000196b0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
+000196c0: 696f 6e2c 2066 6f6c 6c6f 7765 6420 6279  ion, followed by
+000196d0: 2074 6865 2066 696c 656e 616d 652e 2054   the filename. T
+000196e0: 6865 2070 726f 7065 7274 6965 7320 6c69  he properties li
+000196f0: 7374 6564 2061 626f 7665 2077 696c 6c20  sted above will 
+00019700: 6265 2069 6e68 6572 6974 6564 2066 726f  be inherited fro
+00019710: 6d20 7468 6520 636f 6e66 6967 2e74 6f6d  m the config.tom
+00019720: 6c20 6077 6f72 6b65 7250 6f6f 6c60 2073  l `workerPool` s
+00019730: 7065 6369 6669 6361 7469 6f6e 2069 6620  pecification if 
+00019740: 7468 6579 2061 7265 206e 6f74 2070 7265  they are not pre
+00019750: 7365 6e74 2069 6e20 7468 6520 4a53 4f4e  sent in the JSON
+00019760: 2066 696c 652e 2041 6e20 6578 616d 706c   file. An exampl
+00019770: 6520 4a53 4f4e 2073 7065 6369 6669 6361  e JSON specifica
+00019780: 7469 6f6e 2069 7320 7368 6f77 6e20 6265  tion is shown be
+00019790: 6c6f 773a 0a0a 6060 606a 736f 6e0a 7b0a  low:..```json.{.
+000197a0: 2020 2269 6d61 6765 7349 6422 3a20 2279    "imagesId": "y
+000197b0: 6469 643a 696d 6766 616d 3a30 3030 3030  did:imgfam:00000
+000197c0: 303a 3431 3936 3235 3932 2d35 3737 632d  0:41962592-577c-
+000197d0: 3466 6465 2d61 6230 332d 6438 3532 3436  4fde-ab03-d85246
+000197e0: 3565 3766 3862 222c 0a20 2022 696e 7374  5e7f8b",.  "inst
+000197f0: 616e 6365 5461 6773 223a 207b 2261 3122  anceTags": {"a1"
+00019800: 3a20 226f 6e65 222c 2022 6132 223a 2022  : "one", "a2": "
+00019810: 7477 6f22 7d2c 0a20 2022 7265 7175 6972  two"},.  "requir
+00019820: 656d 656e 744e 616d 6522 3a20 2263 725f  ementName": "cr_
+00019830: 7465 7374 5f7b 7b64 6174 6574 696d 657d  test_{{datetime}
+00019840: 7d22 2c0a 2020 2272 6571 7569 7265 6d65  }",.  "requireme
+00019850: 6e74 4e61 6d65 7370 6163 6522 3a20 2270  ntNamespace": "p
+00019860: 7965 7861 6d70 6c65 7322 2c0a 2020 2272  yexamples",.  "r
+00019870: 6571 7569 7265 6d65 6e74 5461 6722 3a20  equirementTag": 
+00019880: 2270 7965 7861 6d70 6c65 732d 7465 7374  "pyexamples-test
+00019890: 222c 0a20 2022 7465 6d70 6c61 7465 4964  ",.  "templateId
+000198a0: 223a 2022 7964 6964 3a63 7274 3a30 3030  ": "ydid:crt:000
+000198b0: 3030 303a 3233 3065 3961 3432 2d39 3764  000:230e9a42-97d
+000198c0: 622d 3464 3639 2d61 6139 312d 3239 6666  b-4d69-aa91-29ff
+000198d0: 3330 3939 3531 6234 222c 0a20 2022 7573  309951b4",.  "us
+000198e0: 6572 4461 7461 223a 2022 232f 6269 6e2f  erData": "#/bin/
+000198f0: 6261 7368 5c6e 234f 7468 6572 2073 7475  bash\n#Other stu
+00019900: 6666 2e2e 2e22 2c0a 2020 2274 6172 6765  ff...",.  "targe
+00019910: 7449 6e73 7461 6e63 6543 6f75 6e74 223a  tInstanceCount":
+00019920: 2031 2c0a 2020 226d 6169 6e74 6169 6e49   1,.  "maintainI
+00019930: 6e73 7461 6e63 6543 6f75 6e74 223a 2074  nstanceCount": t
+00019940: 7275 650a 7d0a 6060 600a 0a49 6620 6120  rue.}.```..If a 
+00019950: 576f 726b 6572 2050 6f6f 6c20 6973 2064  Worker Pool is d
+00019960: 6566 696e 6564 2c20 7573 696e 6720 6077  efined, using `w
+00019970: 6f72 6b65 7250 6f6f 6c44 6174 6160 2069  orkerPoolData` i
+00019980: 6e20 7468 6520 636f 6e66 6967 7572 6174  n the configurat
+00019990: 696f 6e20 6669 6c65 206f 7220 6279 2075  ion file or by u
+000199a0: 7369 6e67 2074 6865 2060 2d2d 776f 726b  sing the `--work
+000199b0: 6572 2d70 6f6f 6c60 2028 6f72 2060 2d70  er-pool` (or `-p
+000199c0: 6029 206f 7074 696f 6e2c 2060 7964 2d69  `) option, `yd-i
+000199d0: 6e73 7461 6e74 6961 7465 6020 7769 6c6c  nstantiate` will
+000199e0: 2065 7874 7261 6374 2074 6865 2043 6f6d   extract the Com
+000199f0: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
+00019a00: 2066 726f 6d20 7468 6520 576f 726b 6572   from the Worker
+00019a10: 2050 6f6f 6c20 7370 6563 6966 6963 6174   Pool specificat
+00019a20: 696f 6e20 2869 676e 6f72 696e 6720 576f  ion (ignoring Wo
+00019a30: 726b 6572 2d50 6f6f 6c2d 7370 6563 6966  rker-Pool-specif
+00019a40: 6963 2064 6174 6129 2c20 616e 6420 7573  ic data), and us
+00019a50: 6520 7468 6174 2066 6f72 2069 6e73 7461  e that for insta
+00019a60: 6e74 6961 7469 6e67 2074 6865 2043 6f6d  ntiating the Com
+00019a70: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
+00019a80: 2e0a 0a55 7365 2074 6865 2060 2d2d 6472  ...Use the `--dr
+00019a90: 792d 7275 6e60 206f 7074 696f 6e20 746f  y-run` option to
+00019aa0: 2069 6e73 7065 6374 2074 6865 2064 6574   inspect the det
+00019ab0: 6169 6c73 206f 6620 7468 6520 436f 6d70  ails of the Comp
+00019ac0: 7574 6520 5265 7175 6972 656d 656e 7420  ute Requirement 
+00019ad0: 7370 6563 6966 6963 6174 696f 6e20 7468  specification th
+00019ae0: 6174 2077 696c 6c20 6265 2073 7562 6d69  at will be submi
+00019af0: 7474 6564 2c20 696e 204a 534f 4e20 666f  tted, in JSON fo
+00019b00: 726d 6174 2e20 5468 6520 4a53 4f4e 206f  rmat. The JSON o
+00019b10: 7574 7075 7420 6f66 2074 6869 7320 636f  utput of this co
+00019b20: 6d6d 616e 6420 6361 6e20 6265 2075 7365  mmand can be use
+00019b30: 6420 7769 7468 2074 6865 2060 2d43 6020  d with the `-C` 
+00019b40: 6f70 7469 6f6e 2061 626f 7665 2028 6f72  option above (or
+00019b50: 2077 6974 6820 602d 7060 2066 6f72 2057   with `-p` for W
+00019b60: 6f72 6b65 7220 506f 6f6c 2073 7065 6369  orker Pool speci
+00019b70: 6669 6361 7469 6f6e 7329 2e0a 0a23 2323  fications)...###
+00019b80: 2054 6573 742d 5275 6e6e 696e 6720 6120   Test-Running a 
+00019b90: 4479 6e61 6d69 6320 5465 6d70 6c61 7465  Dynamic Template
+00019ba0: 0a0a 5768 656e 2061 2074 6865 2060 7465  ..When a the `te
+00019bb0: 6d70 6c61 7465 4964 6020 6f66 2061 2044  mplateId` of a D
+00019bc0: 796e 616d 6963 2052 6571 7569 7265 6d65  ynamic Requireme
+00019bd0: 6e74 2069 7320 7573 6564 2c20 7468 6520  nt is used, the 
+00019be0: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
+00019bf0: 2063 6f6d 6d61 6e64 2063 616e 2062 6520   command can be 
+00019c00: 7573 6564 2074 6f20 7265 706f 7274 206f  used to report o
+00019c10: 6e20 6120 7465 7374 2072 756e 206f 6620  n a test run of 
+00019c20: 7468 6520 5465 6d70 6c61 7465 2c20 7573  the Template, us
+00019c30: 696e 6720 7468 6520 602d 2d72 6570 6f72  ing the `--repor
+00019c40: 7460 2028 6f72 2060 2d72 6029 2063 6f6d  t` (or `-r`) com
+00019c50: 6d61 6e64 206c 696e 6520 6f70 7469 6f6e  mand line option
+00019c60: 2e20 5468 6973 2063 616e 2062 6520 7573  . This can be us
+00019c70: 6564 2077 6974 6820 544f 4d4c 2d64 6566  ed with TOML-def
+00019c80: 696e 6564 2043 6f6d 7075 7465 2052 6571  ined Compute Req
+00019c90: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
+00019ca0: 6361 7469 6f6e 732c 2062 7574 206e 6f74  cations, but not
+00019cb0: 2074 686f 7365 2074 6861 7420 6172 6520   those that are 
+00019cc0: 4a53 4f4e 2d64 6566 696e 6564 2e0a 0a4e  JSON-defined...N
+00019cd0: 6f20 696e 7374 616e 6365 7320 7769 6c6c  o instances will
+00019ce0: 2062 6520 7072 6f76 6973 696f 6e65 6420   be provisioned 
+00019cf0: 6475 7269 6e67 2074 6865 2074 6573 7420  during the test 
+00019d00: 7275 6e2e 0a0a 466f 7220 6578 616d 706c  run...For exampl
+00019d10: 653a 0a0a 6060 6073 6865 6c6c 0a25 2079  e:..```shell.% y
+00019d20: 642d 696e 7374 616e 7469 6174 6520 2d2d  d-instantiate --
+00019d30: 7265 706f 7274 202d 2d71 7569 6574 0a0a  report --quiet..
+00019d40: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
+00019d50: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
+00019d60: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
+00019d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019d90: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+00019da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019dd0: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
+00019de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019df0: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
+00019e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019e20: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
+00019e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019e40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019e60: e294 80e2 9480 e294 80e2 9490 0ae2 9482  ................
+00019e70: 2020 2020 e294 8220 2020 5261 6e6b 20e2      ...   Rank .
+00019e80: 9482 2050 726f 7669 6465 7220 2020 e294  .. Provider   ..
+00019e90: 8220 5479 7065 2020 2020 2020 2020 2020  . Type          
+00019ea0: 2020 2020 2020 20e2 9482 2052 6567 696f         ... Regio
+00019eb0: 6e20 2020 20e2 9482 2049 6e73 7461 6e63  n    ... Instanc
+00019ec0: 6554 7970 6520 2020 e294 8220 536f 7572  eType   ... Sour
+00019ed0: 6365 204e 616d 6520 2020 2020 2020 e294  ce Name       ..
+00019ee0: 820a e294 9ce2 9480 e294 80e2 9480 e294  ................
+00019ef0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00019f00: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00019f10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019f20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019f30: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+00019f40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019f50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019f60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019f70: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00019f80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019f90: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00019fa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019fb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019fc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019fd0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+00019fe0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019ff0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a000: 9480 e294 80e2 9480 e294 80e2 94a4 0ae2  ................
+0001a010: 9482 2020 3120 e294 8220 2020 2020 2031  ..  1 ...      1
+0001a020: 20e2 9482 2041 5753 2020 2020 2020 2020   ... AWS        
+0001a030: e294 8220 4177 7353 706f 7443 6f6d 7075  ... AwsSpotCompu
+0001a040: 7465 536f 7572 6365 20e2 9482 2065 752d  teSource ... eu-
+0001a050: 7765 7374 2d32 20e2 9482 2074 3361 2e6e  west-2 ... t3a.n
+0001a060: 616e 6f20 2020 2020 2020 e294 8220 6177  ano       ... aw
+0001a070: 7373 706f 742d 6575 2d77 6573 742d 3220  sspot-eu-west-2 
+0001a080: e294 820a e294 9ce2 9480 e294 80e2 9480  ................
+0001a090: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001a0a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a0b0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a0c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a0d0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a0e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a0f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a100: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a110: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001a120: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a130: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a140: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a150: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a160: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a170: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001a180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a190: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a1a0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+0001a1b0: 0ae2 9482 2020 3220 e294 8220 2020 2020  ....  2 ...     
+0001a1c0: 2032 20e2 9482 2041 5753 2020 2020 2020   2 ... AWS      
+0001a1d0: 2020 e294 8220 4177 7353 706f 7443 6f6d    ... AwsSpotCom
+0001a1e0: 7075 7465 536f 7572 6365 20e2 9482 2065  puteSource ... e
+0001a1f0: 752d 7765 7374 2d32 20e2 9482 2074 3361  u-west-2 ... t3a
+0001a200: 2e6d 6963 726f 2020 2020 2020 e294 8220  .micro      ... 
+0001a210: 6177 7373 706f 742d 6575 2d77 6573 742d  awsspot-eu-west-
+0001a220: 3220 e294 820a e294 9ce2 9480 e294 80e2  2 ..............
+0001a230: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a240: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a250: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a270: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a2a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a2b0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001a2c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a2d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a2e0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a2f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a310: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001a320: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a330: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a340: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a350: 94a4 0ae2 9482 2020 3320 e294 8220 2020  ......  3 ...   
+0001a360: 2020 2033 20e2 9482 2041 5753 2020 2020     3 ... AWS    
+0001a370: 2020 2020 e294 8220 4177 7353 706f 7443      ... AwsSpotC
+0001a380: 6f6d 7075 7465 536f 7572 6365 20e2 9482  omputeSource ...
+0001a390: 2065 752d 7765 7374 2d32 20e2 9482 2074   eu-west-2 ... t
+0001a3a0: 3361 2e73 6d61 6c6c 2020 2020 2020 e294  3a.small      ..
+0001a3b0: 8220 6177 7373 706f 742d 6575 2d77 6573  . awsspot-eu-wes
+0001a3c0: 742d 3220 e294 820a e294 9ce2 9480 e294  t-2 ............
+0001a3d0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a3e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a3f0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a400: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a410: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a420: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a430: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a440: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a460: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a480: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a4a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a4b0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a4c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a4d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a4e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a4f0: 80e2 94a4 0ae2 9482 2020 3420 e294 8220  ........  4 ... 
+0001a500: 2020 2020 2034 20e2 9482 2041 5753 2020       4 ... AWS  
+0001a510: 2020 2020 2020 e294 8220 4177 7353 706f        ... AwsSpo
+0001a520: 7443 6f6d 7075 7465 536f 7572 6365 20e2  tComputeSource .
+0001a530: 9482 2065 752d 7765 7374 2d32 20e2 9482  .. eu-west-2 ...
+0001a540: 2063 3561 2e6c 6172 6765 2020 2020 2020   c5a.large      
+0001a550: e294 8220 6177 7373 706f 742d 6575 2d77  ... awsspot-eu-w
+0001a560: 6573 742d 3220 e294 820a e294 9ce2 9480  est-2 ..........
+0001a570: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a590: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a5a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a5b0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a5c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a5d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a5e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a5f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a600: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a620: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a650: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a660: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a670: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a680: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a690: e294 80e2 94a4 0ae2 9482 2020 3520 e294  ..........  5 ..
+0001a6a0: 8220 2020 2020 2034 20e2 9482 2041 5753  .      4 ... AWS
+0001a6b0: 2020 2020 2020 2020 e294 8220 4177 7353          ... AwsS
+0001a6c0: 706f 7443 6f6d 7075 7465 536f 7572 6365  potComputeSource
+0001a6d0: 20e2 9482 2065 752d 7765 7374 2d32 20e2   ... eu-west-2 .
+0001a6e0: 9482 2063 3661 2e6c 6172 6765 2020 2020  .. c6a.large    
+0001a6f0: 2020 e294 8220 6177 7373 706f 742d 6575    ... awsspot-eu
+0001a700: 2d77 6573 742d 3220 e294 820a e294 9ce2  -west-2 ........
+0001a710: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a730: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a750: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a760: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a790: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a7a0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a7b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a7c0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a7d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a7e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a7f0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a830: 9480 e294 80e2 94a4 0ae2 9482 2020 3620  ............  6 
+0001a840: e294 8220 2020 2020 2034 20e2 9482 2041  ...      4 ... A
+0001a850: 5753 2020 2020 2020 2020 e294 8220 4177  WS        ... Aw
+0001a860: 7353 706f 7443 6f6d 7075 7465 536f 7572  sSpotComputeSour
+0001a870: 6365 20e2 9482 2065 752d 7765 7374 2d32  ce ... eu-west-2
+0001a880: 20e2 9482 2074 3361 2e6d 6564 6975 6d20   ... t3a.medium 
+0001a890: 2020 2020 e294 8220 6177 7373 706f 742d      ... awsspot-
+0001a8a0: 6575 2d77 6573 742d 3220 e294 820a e294  eu-west-2 ......
+0001a8b0: 9ce2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a8c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a8d0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a8e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a8f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a900: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a910: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a920: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a930: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a940: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a960: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a990: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a9a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a9b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a9c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a9d0: 80e2 9480 e294 80e2 94a4 0ae2 9482 2020  ..............  
+0001a9e0: 3720 e294 8220 2020 2020 2035 20e2 9482  7 ...      5 ...
+0001a9f0: 2041 5753 2020 2020 2020 2020 e294 8220   AWS        ... 
+0001aa00: 4177 7353 706f 7443 6f6d 7075 7465 536f  AwsSpotComputeSo
+0001aa10: 7572 6365 20e2 9482 2065 752d 7765 7374  urce ... eu-west
+0001aa20: 2d32 20e2 9482 206d 3561 2e6c 6172 6765  -2 ... m5a.large
+0001aa30: 2020 2020 2020 e294 8220 6177 7373 706f        ... awsspo
+0001aa40: 742d 6575 2d77 6573 742d 3220 e294 820a  t-eu-west-2 ....
+0001aa50: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
+0001aa60: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aa70: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001aa80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aa90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aaa0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001aab0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aac0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aae0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001aaf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab00: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001ab10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab30: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001ab40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab70: e294 80e2 9480 e294 80e2 94a4 0ae2 9482  ................
+0001ab80: 2020 3820 e294 8220 2020 2020 2035 20e2    8 ...      5 .
+0001ab90: 9482 2041 5753 2020 2020 2020 2020 e294  .. AWS        ..
+0001aba0: 8220 4177 7353 706f 7443 6f6d 7075 7465  . AwsSpotCompute
+0001abb0: 536f 7572 6365 20e2 9482 2065 752d 7765  Source ... eu-we
+0001abc0: 7374 2d32 20e2 9482 206d 3561 642e 6c61  st-2 ... m5ad.la
+0001abd0: 7267 6520 2020 2020 e294 8220 6177 7373  rge     ... awss
+0001abe0: 706f 742d 6575 2d77 6573 742d 3220 e294  pot-eu-west-2 ..
+0001abf0: 820a e294 9ce2 9480 e294 80e2 9480 e294  ................
+0001ac00: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001ac10: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001ac20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ac30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ac40: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001ac50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ac60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ac70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ac80: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001ac90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aca0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001acb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001acc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001acd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ace0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001acf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ad00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ad10: 9480 e294 80e2 9480 e294 80e2 94a4 0ae2  ................
+0001ad20: 9482 2020 3920 e294 8220 2020 2020 2035  ..  9 ...      5
+0001ad30: 20e2 9482 2041 5753 2020 2020 2020 2020   ... AWS        
+0001ad40: e294 8220 4177 7353 706f 7443 6f6d 7075  ... AwsSpotCompu
+0001ad50: 7465 536f 7572 6365 20e2 9482 2065 752d  teSource ... eu-
+0001ad60: 7765 7374 2d32 20e2 9482 206d 3661 2e6c  west-2 ... m6a.l
+0001ad70: 6172 6765 2020 2020 2020 e294 8220 6177  arge      ... aw
+0001ad80: 7373 706f 742d 6575 2d77 6573 742d 3220  sspot-eu-west-2 
+0001ad90: e294 820a e294 9ce2 9480 e294 80e2 9480  ................
+0001ada0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001adb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001adc0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001add0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ade0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001adf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae20: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001ae30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae50: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae80: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001ae90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aea0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aeb0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
+0001aec0: 0ae2 9482 2031 3020 e294 8220 2020 2020  .... 10 ...     
+0001aed0: 2035 20e2 9482 2041 5753 2020 2020 2020   5 ... AWS      
+0001aee0: 2020 e294 8220 4177 7353 706f 7443 6f6d    ... AwsSpotCom
+0001aef0: 7075 7465 536f 7572 6365 20e2 9482 2065  puteSource ... e
+0001af00: 752d 7765 7374 2d32 20e2 9482 2074 3361  u-west-2 ... t3a
+0001af10: 2e6c 6172 6765 2020 2020 2020 e294 8220  .large      ... 
+0001af20: 6177 7373 706f 742d 6575 2d77 6573 742d  awsspot-eu-west-
+0001af30: 3220 e294 820a e294 94e2 9480 e294 80e2  2 ..............
+0001af40: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
+0001af50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001af60: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
+0001af70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001af80: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+0001af90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001afa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001afb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001afc0: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+0001afd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001afe0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aff0: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b000: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b010: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b020: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+0001b030: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b040: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b050: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b060: 9498 0a60 6060 0a0a 2323 2079 642d 7465  ...```..## yd-te
+0001b070: 726d 696e 6174 650a 0a54 6865 2060 7964  rminate..The `yd
+0001b080: 2d74 6572 6d69 6e61 7465 6020 636f 6d6d  -terminate` comm
+0001b090: 616e 6420 696d 6d65 6469 6174 656c 7920  and immediately 
+0001b0a0: 7465 726d 696e 6174 6573 2043 6f6d 7075  terminates Compu
+0001b0b0: 7465 2052 6571 7569 7265 6d65 6e74 7320  te Requirements 
+0001b0c0: 7468 6174 206d 6174 6368 2074 6865 2060  that match the `
+0001b0d0: 6e61 6d65 7370 6163 6560 2061 6e64 2060  namespace` and `
+0001b0e0: 7461 6760 2066 6f75 6e64 2069 6e20 7468  tag` found in th
+0001b0f0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+0001b100: 6669 6c65 2e20 416e 7920 6578 6563 7574  file. Any execut
+0001b110: 696e 6720 5461 736b 7320 7769 6c6c 2062  ing Tasks will b
+0001b120: 6520 7465 726d 696e 6174 6564 2069 6d6d  e terminated imm
+0001b130: 6564 6961 7465 6c79 2c20 616e 6420 7468  ediately, and th
+0001b140: 6520 576f 726b 6572 2050 6f6f 6c20 7769  e Worker Pool wi
+0001b150: 6c6c 2062 6520 7368 7574 2064 6f77 6e2e  ll be shut down.
+0001b160: 0a                                       .
```

### Comparing `yellowdog-python-examples-6.0.2/pyproject.toml` & `yellowdog-python-examples-6.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/setup.cfg` & `yellowdog-python-examples-6.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/abort.py` & `yellowdog-python-examples-6.0.3/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/admin.py` & `yellowdog-python-examples-6.0.3/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/args.py` & `yellowdog-python-examples-6.0.3/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.3/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.3/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.3/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/config.py` & `yellowdog-python-examples-6.0.3/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.3/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.3/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/delete.py` & `yellowdog-python-examples-6.0.3/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/download.py` & `yellowdog-python-examples-6.0.3/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.3/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.3/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.3/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/list.py` & `yellowdog-python-examples-6.0.3/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.3/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/printing.py` & `yellowdog-python-examples-6.0.3/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/provision.py` & `yellowdog-python-examples-6.0.3/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.3/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.3/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.3/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/submit.py` & `yellowdog-python-examples-6.0.3/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.3/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.3/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.3/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/upload.py` & `yellowdog-python-examples-6.0.3/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.3/yd_commands/upload_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Utility functions for uploading objects.
 """
 
+from os import name as os_name
 from os import stat
 from os.path import basename
 from pathlib import Path
 from typing import Optional
 
 from yellowdog_client import PlatformClient
 from yellowdog_client.object_store.model import FileTransferStatus
@@ -29,16 +30,15 @@
     """
 
     if stat(filename).st_size == 0:
         print_log(f"Not uploading zero-byte file '{filename}'")
         return False
 
     dest_filename = unique_upload_pathname(
-        # Convert Windows path naming to Unix
-        filename.replace("\\", "/").replace(":", ""),
+        filename=filename,
         id=id,
         inputs_folder_name=inputs_folder_name,
         flatten_upload_paths=flatten_upload_paths,
     )
 
     upload_file_core(
         client=client,
@@ -55,16 +55,22 @@
     id: str,
     inputs_folder_name: Optional[str],
     urlencode_forward_slash: bool = False,
     flatten_upload_paths: bool = False,
 ) -> str:
     """
     Maps the local filename into a uniquely identified upload object
-    in the YD Object Store. Optionally replaces forward slashes.
+    in the YD Object Store. Optionally replaces forward slashes for use
+    in URLs.
     """
+
+    if os_name == "nt":
+        # Convert Windows path naming to Unix style for upload
+        filename = filename.replace("/", "_").replace(":", "_").replace("\\", "/")
+
     forward_slash = "%2F" if urlencode_forward_slash else "/"
     prefix = "" if id == "" else id + forward_slash
 
     if flatten_upload_paths:
         # Use the root of the Work Requirement directory
         return prefix + basename(filename)
```

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.3/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/variables.py` & `yellowdog-python-examples-6.0.3/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/version.py` & `yellowdog-python-examples-6.0.3/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.3/yd_commands/wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,54 +50,55 @@
         for keyring_summary in keyrings:
             # This is a little brittle, obviously
             print_log(
                 f"YellowDog Account short identifier is: '{keyring_summary.id[13:19]}'"
             )
 
 
-def set_proxy_using_pac_if_enabled():
+def set_proxy():
     """
-    Set the HTTPS proxy using autoconfiguration (PAC)
+    Set the HTTPS proxy using autoconfiguration (PAC) if enabled.
     """
-    HTTPS_PROXY_VAR = "HTTPS_PROXY"
-    if CONFIG_COMMON.use_pac:
-        print_log("Using Proxy Auto-Configuration (PAC)")
-        with pac_context_for_url(CONFIG_COMMON.url):
-            https_proxy = os.getenv(HTTPS_PROXY_VAR, None)
-        if https_proxy is not None:
-            os.environ[HTTPS_PROXY_VAR] = https_proxy
+    if not dry_run():
+        proxy_var = "HTTPS_PROXY"
+        if CONFIG_COMMON.use_pac:
+            print_log("Using Proxy Auto-Configuration (PAC)")
+            with pac_context_for_url(CONFIG_COMMON.url):
+                https_proxy = os.getenv(proxy_var, None)
+            if https_proxy is not None:
+                os.environ[proxy_var] = https_proxy
+            else:
+                print_log("No PAC proxy settings found")
         else:
-            print_log("No PAC proxy settings found")
-    else:
-        https_proxy = os.getenv(HTTPS_PROXY_VAR, None)
-    if https_proxy is not None:
-        print_log(f"Using {HTTPS_PROXY_VAR}={https_proxy}")
+            https_proxy = os.getenv(proxy_var, None)
+        if https_proxy is not None:
+            print_log(f"Using {proxy_var}={https_proxy}")
 
 
 def main_wrapper(func):
     def wrapper():
         if not ARGS_PARSER.debug:
             exit_code = 0
             try:
-                set_proxy_using_pac_if_enabled()
+                set_proxy()
                 print_account()
                 func()
             except Exception as e:
                 print_error(e)
                 exit_code = 1
             except KeyboardInterrupt:
                 print_log("Cancelled")
                 exit_code = 1
             finally:
                 CLIENT.close()
                 if exit_code == 0:
                     print_log("Done")
                 exit(exit_code)
         else:
-            set_proxy_using_pac_if_enabled()
+            set_proxy()
             print_account()
             func()
             CLIENT.close()
             print_log("Done")
             exit(0)
 
     return wrapper
```

### Comparing `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.2
+Version: 6.0.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.3/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

