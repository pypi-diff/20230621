# Comparing `tmp/openoligo-0.1.0.tar.gz` & `tmp/openoligo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.0.tar", max compression
+gzip compressed data, was "openoligo-0.1.1.tar", max compression
```

## Comparing `openoligo-0.1.0.tar` & `openoligo-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-06-20 14:00:57.577233 openoligo-0.1.0/LICENSE
--rw-r--r--   0        0        0       11 2023-06-20 14:00:57.577343 openoligo-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-20 14:20:30.850020 openoligo-0.1.0/openoligo/main.py
--rw-r--r--   0        0        0      722 2023-06-20 14:17:18.166770 openoligo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 openoligo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 15:02:43.473844 openoligo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1917 2023-06-20 20:46:11.014057 openoligo-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 14:31:11.021160 openoligo-0.1.1/openoligo/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:58:07.198168 openoligo-0.1.1/openoligo/container/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-21 07:30:08.808691 openoligo-0.1.1/openoligo/container/cartridge.py
+-rw-r--r--   0        0        0     1464 2023-06-21 07:11:10.738482 openoligo-0.1.1/openoligo/container/types.py
+-rw-r--r--   0        0        0        0 2023-06-20 17:48:38.907388 openoligo-0.1.1/openoligo/driver/__init__.py
+-rw-r--r--   0        0        0     1905 2023-06-21 05:08:40.538815 openoligo-0.1.1/openoligo/driver/manifold.py
+-rw-r--r--   0        0        0     2184 2023-06-21 02:39:37.013644 openoligo-0.1.1/openoligo/driver/switch.py
+-rw-r--r--   0        0        0      958 2023-06-21 03:42:34.120363 openoligo-0.1.1/openoligo/driver/types.py
+-rw-r--r--   0        0        0      931 2023-06-21 04:56:42.236811 openoligo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 openoligo-0.1.1/PKG-INFO
```

