# Comparing `tmp/pure_ocean_breeze-3.9.7.tar.gz` & `tmp/pure_ocean_breeze-3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.7.tar", last modified: Wed Jun 14 02:31:01 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.8.tar", last modified: Wed Jun 21 03:31:07 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.7.tar` & `pure_ocean_breeze-3.9.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    31004 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    67375 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   228266 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:31:01.353446 pure_ocean_breeze-3.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.673502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31316 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68253 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228535 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.673502 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/setup.py
```

### Comparing `pure_ocean_breeze-3.9.7/LICENSE` & `pure_ocean_breeze-3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/PKG-INFO` & `pure_ocean_breeze-3.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.7
+Version: 3.9.8
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.7/README.md` & `pure_ocean_breeze-3.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-06-10 21:02:21"
-__version__ = "3.9.7"
+__updated__ = "2023-06-14 16:01:53"
+__version__ = "3.9.8"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/read_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,82 +165,82 @@
 
     if not unadjust:
         if path:
             return pd.read_parquet(homeplace.daily_data_file + path)
         elif open:
             opens = pd.read_parquet(
                 homeplace.daily_data_file + "opens.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = opens
         elif close:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = closes
         elif high:
             highs = pd.read_parquet(
                 homeplace.daily_data_file + "highs.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = highs
         elif low:
             lows = pd.read_parquet(
                 homeplace.daily_data_file + "lows.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = lows
         elif vwap:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "vwaps.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1)
+                * read_daily(state=1,start=start)
             )
         elif tr:
             trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet").replace(
                 0, np.nan
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = trs
         elif sharenum:
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             df = sharenums
         elif total_sharenum:
             df = pd.read_parquet(homeplace.daily_data_file + "total_sharenums.parquet")
         elif amount:
             volumes = pd.read_parquet(
                 homeplace.daily_data_file + "amounts.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = volumes
         elif money:
             df = pd.read_parquet(
                 homeplace.factor_data_file + "日频数据-每日成交额/每日成交额.parquet"
             )
         elif age:
             age = pd.read_parquet(homeplace.daily_data_file + "ages.parquet")
             df = age
         elif flow_cap:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             flow_cap = closes * sharenums
             df = flow_cap
         elif total_cap:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             sharenums = pd.read_parquet(
                 homeplace.daily_data_file + "total_sharenums.parquet"
             )
             flow_cap = closes * sharenums
             df = flow_cap
         elif adjfactor:
             # df=pd.read_parquet(homeplace.daily_data_file+'adjfactors.parquet')
             df = (
                 read_daily(close=1, start=start)
-                * read_daily(state=1)
+                * read_daily(state=1,start=start)
                 / read_daily(close=1, start=start, unadjust=1)
-                * read_daily(state=1)
+                * read_daily(state=1,start=start)
             )
         elif st:
             st = pd.read_parquet(homeplace.daily_data_file + "sts.parquet")
             df = st
         elif state:
             state = pd.read_parquet(homeplace.daily_data_file + "states.parquet")
             state = state.where(state == 1, np.nan)
@@ -271,50 +271,50 @@
             df = df.rolling(20, min_periods=10).std()
         elif swing:
             df = (
                 read_daily(high=1, start=start) - read_daily(low=1, start=start)
             ) / read_daily(close=1, start=start)
         elif pb:
             df = pd.read_parquet(homeplace.daily_data_file + "pb.parquet") * read_daily(
-                state=1
+                state=1,start=start
             )
         elif pe:
             df = pd.read_parquet(homeplace.daily_data_file + "pe.parquet") * read_daily(
-                state=1
+                state=1,start=start
             )
         elif iret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "idiosyncratic_ret.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif ivol:
             df = read_daily(iret=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif illiquidity:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "illiquidity.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif swindustry_ret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "股票对应申万一级行业每日收益率.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif zxindustry_ret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "股票对应中信一级行业每日收益率.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif stop_up:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "stop_ups.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1)
+                * read_daily(state=1,start=start)
             )
         elif stop_down:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "stop_downs.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1)
+                * read_daily(state=1,start=start)
             )
         elif zxindustry_dummy_code:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量代码版.parquet")
         elif zxindustry_dummy_name:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量名称版.parquet")
         elif swindustry_dummy:
             df = pd.read_parquet(homeplace.daily_data_file + "申万行业2021版哑变量.parquet")
@@ -338,43 +338,43 @@
             )
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     else:
         if open:
             opens = pd.read_parquet(
                 homeplace.daily_data_file + "opens_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = opens
         elif close:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = closes
         elif high:
             highs = pd.read_parquet(
                 homeplace.daily_data_file + "highs_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = highs
         elif low:
             lows = pd.read_parquet(
                 homeplace.daily_data_file + "lows_unadj.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
             df = lows
         elif vwap:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "vwaps.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif stop_up:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "stop_ups.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         elif stop_down:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "stop_downs.parquet"
-            ) * read_daily(state=1)
+            ) * read_daily(state=1,start=start)
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     if "date" not in df.columns:
         df = df[df.index >= pd.Timestamp(str(start))]
     return df.dropna(how="all")
```

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-06-14 00:08:18"
+__updated__ = "2023-06-20 22:25:36"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
@@ -70,16 +70,22 @@
     """
     res = {}
     import h5py
 
     a = h5py.File(path)
     for k, v in tqdm.tqdm(list(a.items()), desc="数据加载中……"):
         value = list(v.values())[-1]
-        col = [i.decode("utf-8") for i in list(list(v.values())[0])]
-        ind = [i.decode("utf-8") for i in list(list(v.values())[1])]
+        try:
+            col = [i.decode("utf-8") for i in list(list(v.values())[0])]
+        except Exception:
+            col=list(list(v.values())[0])
+        try:
+            ind = [i.decode("utf-8") for i in list(list(v.values())[1])]
+        except Exception:
+            ind=list(list(v.values())[1])
         res[k] = pd.DataFrame(value, columns=col, index=ind)
     return res
 
 
 @do_on_dfs
 @deprecation.deprecated(
     deprecated_in="3.0",
@@ -156,14 +162,41 @@
         kind = "stock"
     else:
         kind = "index"
     return x, kind
 
 
 @do_on_dfs
+def add_suffix(code:str)->str:
+    """给股票代码加上后缀
+
+    Parameters
+    ----------
+    code : str
+        纯数字组成的字符串类型的股票代码，如000001
+
+    Returns
+    -------
+    str
+        添加完后缀后的股票代码，如000001.SZ
+    """    
+    if not isinstance(code, str):
+        code = str(code)
+    if len(code) < 6:
+        code = "0" * (6 - len(code)) + code
+    if code.startswith("0") or code.startswith("3"):
+        code = ".".join([code, "SZ"])
+    elif code.startswith("6"):
+        code = ".".join([code, "SH"])
+    elif code.startswith("8"):
+        code = ".".join([code, "BJ"])
+    return code
+
+
+@do_on_dfs
 def get_value(df: pd.DataFrame, n: int) -> pd.DataFrame:
     """很多因子计算时，会一次性生成很多值，使用时只取出一个值
 
     Parameters
     ----------
     df : pd.DataFrame
         每个value是一个列表或元组的pd.DataFrame
@@ -320,14 +353,16 @@
     elif code.startswith("8"):
         code = code + ".BJ"
     else:
         code = code + ".UN"
     return code
 
 
+
+
 @do_on_dfs
 def 生成每日分类表(
     df: pd.DataFrame, code: str, entry: str, exit: str, kind: str
 ) -> pd.DataFrame:
     """
     ```
     df是要包含任意多列的表格，为dataframe格式，主要内容为，每一行是
@@ -1913,15 +1948,15 @@
             return x
 
         df = df.groupby(["date"]).apply(lambda x: clip_sing(x, n))
         try:
             df = df.reset_index()
         except Exception:
             ...
-        df = df.pivot(index="date", columns="code", values="fac")
+        df = df.drop_duplicates(subset=['date','code']).pivot(index="date", columns="code", values="fac")
         return df
     elif replace:
 
         def clip_sing(x: pd.Series, n: float = 3):
             median = x.quantile(0.5)
             diff_median = ((x - median).abs()).quantile(0.5)
             max_range = median + n * diff_median
```

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-06-14 09:29:34"
+__updated__ = "2023-06-21 11:11:30"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -926,15 +926,18 @@
 
     Returns
     -------
     `pd.DataFrame`
         修改为交易日标注后的pd.DataFrame
     """
     """"""
-    trs = read_daily(tr=1)
+    start=df.index.min()
+    start=start-pd.tseries.offsets.MonthBegin()
+    start=datetime.datetime.strftime(start,'%Y%m%d')
+    trs = read_daily(tr=1,start=start)
     trs = trs.assign(tradeends=list(trs.index))
     trs = trs[["tradeends"]]
     trs = trs.resample("M").last()
     df = pd.concat([trs, df], axis=1)
     df = df.set_index(["tradeends"])
     return df
 
@@ -3332,22 +3335,23 @@
             df = df.sort_values(["date", "num"])
         df = df.groupby(self.groupby_target).apply(the_func)
         if self.groupby_target == ["date", "code"]:
             df = df.to_frame("fac").reset_index()
             df.columns = ["date", "code", "fac"]
         else:
             df = df.reset_index()
-        df = df.pivot(columns="code", index="date", values="fac")
-        df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-        to_save = df.stack().reset_index()
-        to_save.columns = ["date", "code", "fac"]
-        self.factor_steps.write_via_df(
-            to_save, self.factor_file_pinyin, tuple_col="fac"
-        )
-        return df
+        if (df is not None) and (df.shape[0]>0):
+            df = df.pivot(columns="code", index="date", values="fac")
+            df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+            to_save = df.stack().reset_index()
+            to_save.columns = ["date", "code", "fac"]
+            self.factor_steps.write_via_df(
+                to_save, self.factor_file_pinyin, tuple_col="fac"
+            )
+            return df
 
     def select_many_calculate(
         self,
         dates: List[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
@@ -3542,14 +3546,16 @@
                 return res
             elif isinstance(res, pd.DataFrame):
                 res.columns = [f"fac{i}" for i in range(len(res.columns))]
                 res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
                 res = res[["fac"]].reset_index()
                 res.columns = ["code", "fac"]
                 return res
+            elif res is None:
+                ...
             else:
                 res = pd.concat(res, axis=1)
                 res.columns = [f"fac{i}" for i in range(len(res.columns))]
                 res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
                 res = res[["fac"]].reset_index()
                 res.columns = ["code", "fac"]
                 return res
```

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.7
+Version: 3.9.8
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.7/setup.py` & `pure_ocean_breeze-3.9.8/setup.py`

 * *Files identical despite different names*

