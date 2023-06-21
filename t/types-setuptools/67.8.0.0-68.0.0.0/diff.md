# Comparing `tmp/types-setuptools-67.8.0.0.tar.gz` & `tmp/types-setuptools-68.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-67.8.0.0.tar", last modified: Sat May 20 09:12:52 2023, max compression
+gzip compressed data, was "types-setuptools-68.0.0.0.tar", last modified: Wed Jun 21 12:29:45 2023, max compression
```

## Comparing `types-setuptools-67.8.0.0.tar` & `types-setuptools-68.0.0.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.001527 types-setuptools-67.8.0.0/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/pkg_resources-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.005527 types-setuptools-67.8.0.0/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 09:12:50.000000 types-setuptools-67.8.0.0/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.009527 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.009527 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-20 09:12:34.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/py312compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-20 09:12:35.000000 types-setuptools-67.8.0.0/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:12:52.013527 types-setuptools-67.8.0.0/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 09:12:51.000000 types-setuptools-67.8.0.0/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.111280 types-setuptools-68.0.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-06-21 12:29:44.000000 types-setuptools-68.0.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 12:29:44.000000 types-setuptools-68.0.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 12:29:45.111280 types-setuptools-68.0.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.103280 types-setuptools-68.0.0.0/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 12:29:44.000000 types-setuptools-68.0.0.0/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/pkg_resources-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:29:45.111280 types-setuptools-68.0.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-21 12:29:44.000000 types-setuptools-68.0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.107280 types-setuptools-68.0.0.0/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 12:29:44.000000 types-setuptools-68.0.0.0/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.107280 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.107280 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.107280 types-setuptools-68.0.0.0/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.107280 types-setuptools-68.0.0.0/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.111280 types-setuptools-68.0.0.0/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/py312compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 12:29:25.000000 types-setuptools-68.0.0.0/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:29:45.111280 types-setuptools-68.0.0.0/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 12:29:45.000000 types-setuptools-68.0.0.0/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-21 12:29:45.000000 types-setuptools-68.0.0.0/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:29:45.000000 types-setuptools-68.0.0.0/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 12:29:45.000000 types-setuptools-68.0.0.0/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-67.8.0.0/CHANGELOG.md` & `types-setuptools-68.0.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## 68.0.0.0 (2023-06-21)
+
+Bump setuptools to 68.0 (#10339)
+
+* Any -> Incomplete in a few files
+* Bump setuptools to 68.0.*
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 67.8.0.0 (2023-05-20)
 
 [stubsabot] Bump setuptools to 67.8.* (#10194)
 
 Release: https://pypi.org/pypi/setuptools/67.8.0
 Homepage: https://github.com/pypa/setuptools
 Changelog: https://setuptools.pypa.io/en/stable/history.html
```

### Comparing `types-setuptools-67.8.0.0/PKG-INFO` & `types-setuptools-68.0.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.8.0.0
+Version: 68.0.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
+This package was generated from typeshed commit `06c2fb047abe52e329ff854fba2675293173bf50` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-setuptools-67.8.0.0/pkg_resources-stubs/__init__.pyi` & `types-setuptools-68.0.0.0/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setup.py` & `types-setuptools-68.0.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
+This package was generated from typeshed commit `06c2fb047abe52e329ff854fba2675293173bf50` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="67.8.0.0",
+      version="68.0.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['pkg_resources-stubs', 'setuptools-stubs'],
-      package_data={'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml'], 'setuptools-stubs': ['__init__.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'py312compat.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml']},
+      packages=['setuptools-stubs', 'pkg_resources-stubs'],
+      package_data={'setuptools-stubs': ['__init__.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'py312compat.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed'], 'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/__init__.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/archive_util.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/build_meta.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/build_py.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/develop.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/easy_install.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from _typeshed import Incomplete
-from collections.abc import Iterator
-from typing import Any
+from collections.abc import Iterable, Iterator
+from typing import ClassVar
+from typing_extensions import Self, TypedDict
 
 from pkg_resources import Environment
 
 from .. import Command, SetuptoolsDeprecationWarning
 
 __all__ = ["easy_install", "PthDistributions", "extract_wininst_cfg", "get_exe_prefixes"]
 
 class easy_install(Command):
     description: str
     command_consumes_arguments: bool
-    user_options: Any
-    boolean_options: Any
-    negative_opt: Any
-    create_index: Any
+    user_options: Incomplete
+    boolean_options: Incomplete
+    negative_opt: Incomplete
+    create_index: Incomplete
     user: int
-    zip_ok: Any
-    install_dir: Any
-    index_url: Any
-    find_links: Any
-    build_directory: Any
-    args: Any
-    optimize: Any
-    upgrade: Any
-    editable: Any
-    root: Any
-    version: Any
-    install_purelib: Any
-    install_platlib: Any
-    install_headers: Any
-    install_lib: Any
-    install_scripts: Any
-    install_data: Any
-    install_base: Any
-    install_platbase: Any
-    install_userbase: Any
-    install_usersite: Any
-    no_find_links: Any
-    package_index: Any
-    pth_file: Any
-    site_dirs: Any
-    installed_projects: Any
-    verbose: Any
+    zip_ok: Incomplete
+    install_dir: Incomplete
+    index_url: Incomplete
+    find_links: Incomplete
+    build_directory: Incomplete
+    args: Incomplete
+    optimize: Incomplete
+    upgrade: Incomplete
+    editable: Incomplete
+    root: Incomplete
+    version: Incomplete
+    install_purelib: Incomplete
+    install_platlib: Incomplete
+    install_headers: Incomplete
+    install_lib: Incomplete
+    install_scripts: Incomplete
+    install_data: Incomplete
+    install_base: Incomplete
+    install_platbase: Incomplete
+    install_userbase: Incomplete
+    install_usersite: Incomplete
+    no_find_links: Incomplete
+    package_index: Incomplete
+    pth_file: Incomplete
+    site_dirs: Incomplete
+    installed_projects: Incomplete
+    verbose: Incomplete
     def initialize_options(self) -> None: ...
     def delete_blockers(self, blockers) -> None: ...
-    config_vars: Any
-    script_dir: Any
-    all_site_dirs: Any
-    shadow_path: Any
-    local_index: Any
-    outputs: Any
+    config_vars: Incomplete
+    script_dir: Incomplete
+    all_site_dirs: Incomplete
+    shadow_path: Incomplete
+    local_index: Incomplete
+    outputs: Incomplete
     def finalize_options(self) -> None: ...
     def expand_basedirs(self) -> None: ...
     def expand_dirs(self) -> None: ...
     def run(self, show_deprecation: bool = True) -> None: ...
     def pseudo_tempname(self): ...
     def warn_deprecated_options(self) -> None: ...
     def check_site_dir(self) -> None: ...
@@ -84,71 +85,66 @@
     def run_setup(self, setup_script, setup_base, args) -> None: ...
     def build_and_install(self, setup_script, setup_base): ...
     def update_pth(self, dist) -> None: ...
     def unpack_progress(self, src, dst): ...
     def unpack_and_compile(self, egg_path, destination): ...
     def byte_compile(self, to_compile) -> None: ...
     def create_home_path(self) -> None: ...
-    INSTALL_SCHEMES: Any
-    DEFAULT_SCHEME: Any
+    INSTALL_SCHEMES: Incomplete
+    DEFAULT_SCHEME: Incomplete
 
 def extract_wininst_cfg(dist_filename): ...
 def get_exe_prefixes(exe_filename): ...
 
 class PthDistributions(Environment):
     dirty: bool
-    filename: Any
-    sitedirs: Any
-    basedir: Any
+    filename: Incomplete
+    sitedirs: Incomplete
+    basedir: Incomplete
     paths: list[str]
     def __init__(self, filename, sitedirs=()) -> None: ...
     def save(self) -> None: ...
     def add(self, dist) -> None: ...
     def remove(self, dist) -> None: ...
     def make_relative(self, path): ...
 
 class RewritePthDistributions(PthDistributions):
-    prelude: Any
-    postlude: Any
+    prelude: Incomplete
+    postlude: Incomplete
+
+class _SplitArgs(TypedDict, total=False):
+    comments: bool
+    posix: bool
 
 class CommandSpec(list[str]):
-    options: Any
-    split_args: Any
+    options: list[Incomplete]
+    split_args: ClassVar[_SplitArgs]
     @classmethod
     def best(cls) -> type[CommandSpec]: ...
     @classmethod
-    def from_param(cls, param) -> CommandSpec: ...
+    def from_param(cls, param: str | Self | Iterable[str] | None) -> Self: ...
     @classmethod
     def from_environment(cls) -> CommandSpec: ...
     @classmethod
     def from_string(cls, string: str) -> CommandSpec: ...
     def install_options(self, script_text: str) -> None: ...
     def as_header(self) -> str: ...
 
-class WindowsCommandSpec(CommandSpec):
-    split_args: Any
+class WindowsCommandSpec(CommandSpec): ...
 
 class ScriptWriter:
-    template: Any
-    command_spec_class: Any
-    @classmethod
-    def get_script_args(cls, dist, executable: Incomplete | None = None, wininst: bool = False) -> Iterator[tuple[str, str]]: ...
-    @classmethod
-    def get_script_header(cls, script_text, executable: Incomplete | None = None, wininst: bool = False) -> str: ...
+    template: ClassVar[str]
+    command_spec_class: ClassVar[type[CommandSpec]]
     @classmethod
     def get_args(cls, dist, header: Incomplete | None = None) -> Iterator[tuple[str, str]]: ...
     @classmethod
-    def get_writer(cls, force_windows: bool) -> type[ScriptWriter]: ...
-    @classmethod
     def best(cls) -> type[ScriptWriter]: ...
     @classmethod
-    def get_header(cls, script_text: str = "", executable: Incomplete | None = None) -> str: ...
+    def get_header(cls, script_text: str = "", executable: str | CommandSpec | Iterable[str] | None = None) -> str: ...
 
 class WindowsScriptWriter(ScriptWriter):
-    command_spec_class: Any
-    @classmethod
-    def get_writer(cls): ...
+    command_spec_class: ClassVar[type[WindowsCommandSpec]]
     @classmethod
-    def best(cls): ...
+    def best(cls) -> type[WindowsScriptWriter]: ...
 
 class WindowsExecutableLauncherWriter(WindowsScriptWriter): ...
 class EasyInstallDeprecationWarning(SetuptoolsDeprecationWarning): ...
```

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/editable_wheel.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/egg_info.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from typing import Any
+from _typeshed import Incomplete
 from typing_extensions import Final
 
 from .. import Command, SetuptoolsDeprecationWarning
 from .._distutils.filelist import FileList as _FileList
 from .sdist import sdist
 
 PY_MAJOR: Final[str]
 
 def translate_pattern(glob): ...
 
 class InfoCommon:
-    tag_build: Any
-    tag_date: Any
+    tag_build: Incomplete
+    tag_date: Incomplete
     @property
     def name(self): ...
     def tagged_version(self): ...
     def tags(self): ...
     @property
     def vtags(self): ...
 
 class egg_info(InfoCommon, Command):
     description: str
-    user_options: Any
-    boolean_options: Any
-    negative_opt: Any
-    egg_base: Any
-    egg_name: Any
-    egg_info: Any
-    egg_version: Any
+    user_options: Incomplete
+    boolean_options: Incomplete
+    negative_opt: Incomplete
+    egg_base: Incomplete
+    egg_name: Incomplete
+    egg_info: Incomplete
+    egg_version: Incomplete
     broken_egg_info: bool
     def initialize_options(self) -> None: ...
     @property
     def tag_svn_revision(self) -> None: ...
     @tag_svn_revision.setter
     def tag_svn_revision(self, value) -> None: ...
     def save_version_info(self, filename) -> None: ...
     def finalize_options(self) -> None: ...
     def write_or_delete_file(self, what, filename, data, force: bool = False) -> None: ...
     def write_file(self, what, filename, data) -> None: ...
     def delete_file(self, filename) -> None: ...
     def run(self) -> None: ...
-    filelist: Any
+    filelist: Incomplete
     def find_sources(self) -> None: ...
-    def check_broken_egg_info(self) -> None: ...
 
 class FileList(_FileList):
     def __init__(self, warn=None, debug_print=None, ignore_egg_info_dir: bool = False) -> None: ...
     def process_template_line(self, line) -> None: ...
     def include(self, pattern): ...
     def exclude(self, pattern): ...
     def recursive_include(self, dir, pattern): ...
@@ -62,15 +61,15 @@
     template: str
     use_defaults: int
     prune: int
     manifest_only: int
     force_manifest: int
     def initialize_options(self) -> None: ...
     def finalize_options(self) -> None: ...
-    filelist: Any
+    filelist: Incomplete
     def run(self) -> None: ...
     def write_manifest(self) -> None: ...
     def warn(self, msg) -> None: ...
     def add_defaults(self) -> None: ...
     def add_license_files(self) -> None: ...
     def prune_file_list(self) -> None: ...
 
@@ -79,10 +78,9 @@
 def warn_depends_obsolete(cmd, basename, filename) -> None: ...
 def write_requirements(cmd, basename, filename) -> None: ...
 def write_setup_requirements(cmd, basename, filename) -> None: ...
 def write_toplevel_names(cmd, basename, filename) -> None: ...
 def overwrite_arg(cmd, basename, filename) -> None: ...
 def write_arg(cmd, basename, filename, force: bool = False) -> None: ...
 def write_entries(cmd, basename, filename) -> None: ...
-def get_pkg_info_revision(): ...
 
 class EggInfoDeprecationWarning(SetuptoolsDeprecationWarning): ...
```

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/sdist.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/setopt.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/test.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/config/expand.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/depends.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/discovery.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/dist.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/errors.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/extension.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/msvc.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/package_index.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/setuptools-stubs/sandbox.pyi` & `types-setuptools-68.0.0.0/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.8.0.0/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-68.0.0.0/types_setuptools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.8.0.0
+Version: 68.0.0.0
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `35450d9c0d673fc713c3210d8c25d19425f9790e`.
+This package was generated from typeshed commit `06c2fb047abe52e329ff854fba2675293173bf50` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-setuptools-67.8.0.0/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-68.0.0.0/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

