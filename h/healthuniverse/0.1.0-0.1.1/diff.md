# Comparing `tmp/healthuniverse-0.1.0.tar.gz` & `tmp/healthuniverse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthuniverse-0.1.0.tar", max compression
+gzip compressed data, was "healthuniverse-0.1.1.tar", max compression
```

## Comparing `healthuniverse-0.1.0.tar` & `healthuniverse-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       72 2023-06-20 15:19:44.273478 healthuniverse-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-20 15:21:02.557478 healthuniverse-0.1.0/healthuniverse/__init__.py
--rw-r--r--   0        0        0      758 2023-06-20 15:30:36.225478 healthuniverse-0.1.0/healthuniverse/client.py
--rw-r--r--   0        0        0      280 2023-06-20 15:37:21.157478 healthuniverse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 healthuniverse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1735 2023-06-20 16:38:04.928133 healthuniverse-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 15:21:02.557478 healthuniverse-0.1.1/healthuniverse/__init__.py
+-rw-r--r--   0        0        0     2711 2023-06-21 12:13:24.100693 healthuniverse-0.1.1/healthuniverse/client.py
+-rw-r--r--   0        0        0      279 2023-06-21 15:46:22.442732 healthuniverse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 healthuniverse-0.1.1/PKG-INFO
```

