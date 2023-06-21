# Comparing `tmp/test_jrubics_poetry_publish-0.2.3.tar.gz` & `tmp/test_jrubics_poetry_publish-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_jrubics_poetry_publish-0.2.3.tar", max compression
+gzip compressed data, was "test_jrubics_poetry_publish-0.2.4.tar", max compression
```

## Comparing `test_jrubics_poetry_publish-0.2.3.tar` & `test_jrubics_poetry_publish-0.2.4.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      320 2023-06-14 11:39:37.562635 test_jrubics_poetry_publish-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-14 11:39:37.562635 test_jrubics_poetry_publish-0.2.3/test_jrubics_poetry_publish/__init__.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 test_jrubics_poetry_publish-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      320 2023-06-21 09:51:25.017743 test_jrubics_poetry_publish-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-21 09:51:25.017743 test_jrubics_poetry_publish-0.2.4/test_jrubics_poetry_publish/__init__.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 test_jrubics_poetry_publish-0.2.4/PKG-INFO
```

