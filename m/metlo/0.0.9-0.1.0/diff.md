# Comparing `tmp/metlo-0.0.9.tar.gz` & `tmp/metlo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metlo-0.0.9.tar", last modified: Fri Oct  1 04:50:35 2021, max compression
+gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-umkol9th/metlo-0.1.0.tar", last modified: Wed Jun 21 02:58:52 2023, max compression
```

## Comparing `metlo-0.0.9.tar` & `metlo-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.694925 metlo-0.0.9/
--rw-r--r--   0 akshay     (501) staff       (20)      638 2021-10-01 04:50:35.694662 metlo-0.0.9/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)       79 2021-09-16 23:45:35.000000 metlo-0.0.9/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.690190 metlo-0.0.9/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)      159 2021-10-01 04:29:39.000000 metlo-0.0.9/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     2554 2021-10-01 02:57:00.000000 metlo-0.0.9/metlo/api.py
--rw-r--r--   0 akshay     (501) staff       (20)     1591 2021-09-19 00:42:54.000000 metlo-0.0.9/metlo/command_line.py
--rw-r--r--   0 akshay     (501) staff       (20)     1346 2021-09-19 06:20:48.000000 metlo-0.0.9/metlo/config.py
--rw-r--r--   0 akshay     (501) staff       (20)      544 2021-09-19 00:21:50.000000 metlo-0.0.9/metlo/load_definitions.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.692829 metlo-0.0.9/metlo/types/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2021-09-18 22:57:57.000000 metlo-0.0.9/metlo/types/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     1771 2021-09-20 01:05:19.000000 metlo-0.0.9/metlo/types/definition.py
--rw-r--r--   0 akshay     (501) staff       (20)      938 2021-09-18 22:57:41.000000 metlo-0.0.9/metlo/types/enums.py
--rw-r--r--   0 akshay     (501) staff       (20)      444 2021-09-18 22:58:23.000000 metlo-0.0.9/metlo/types/query.py
--rw-r--r--   0 akshay     (501) staff       (20)      243 2021-09-17 00:36:52.000000 metlo-0.0.9/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.694324 metlo-0.0.9/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)      638 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      416 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       51 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/entry_points.txt
--rw-r--r--   0 akshay     (501) staff       (20)      109 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       38 2021-10-01 04:50:35.695007 metlo-0.0.9/setup.cfg
--rw-r--r--   0 akshay     (501) staff       (20)     1120 2021-10-01 04:29:34.000000 metlo-0.0.9/setup.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 02:58:52.000000 metlo-0.1.0/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.0/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.0/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/django.py
+-rw-r--r--   0 akshay     (501) staff       (20)    21150 2023-06-21 02:34:12.000000 metlo-0.1.0/metlo/fastapi.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/flask.py
+-rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-20 06:00:51.000000 metlo-0.1.0/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 02:58:52.000000 metlo-0.1.0/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.0/pyproject.toml
+-rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 02:58:52.000000 metlo-0.1.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

