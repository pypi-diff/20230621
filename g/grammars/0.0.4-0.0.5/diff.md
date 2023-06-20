# Comparing `tmp/grammars-0.0.4.tar.gz` & `tmp/grammars-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grammars-0.0.4.tar", max compression
+gzip compressed data, was "grammars-0.0.5.tar", max compression
```

## Comparing `grammars-0.0.4.tar` & `grammars-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.4/LICENSE
--rw-r--r--   0        0        0     6784 2023-06-19 22:45:20.879351 grammars-0.0.4/README.md
--rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.4/grammars/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.4/grammars/decode/__init__.py
--rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.4/grammars/decode/decode.py
--rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.4/grammars/decode/generate.py
--rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.4/grammars/decode/modes.py
--rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.4/grammars/decode/rank.py
--rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.4/grammars/decode/visualize.py
--rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.4/grammars/parse/__init__.py
--rw-r--r--   0        0        0     8244 2023-06-19 22:49:43.664734 grammars-0.0.4/grammars/parse/parsers.py
--rw-r--r--   0        0        0     1427 2023-06-19 22:53:38.965258 grammars-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 grammars-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 21:58:06.150146 grammars-0.0.5/LICENSE
+-rw-r--r--   0        0        0       11 2023-06-20 22:42:10.169417 grammars-0.0.5/README.md
+-rw-r--r--   0        0        0       79 2023-06-19 16:15:08.373081 grammars-0.0.5/grammars/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:15:01.125215 grammars-0.0.5/grammars/decode/__init__.py
+-rw-r--r--   0        0        0     2008 2023-06-19 22:47:06.275395 grammars-0.0.5/grammars/decode/decode.py
+-rw-r--r--   0        0        0     3322 2023-06-19 22:47:06.288800 grammars-0.0.5/grammars/decode/generate.py
+-rw-r--r--   0        0        0     4208 2023-06-19 22:47:06.281054 grammars-0.0.5/grammars/decode/modes.py
+-rw-r--r--   0        0        0     3852 2023-06-19 22:47:06.295864 grammars-0.0.5/grammars/decode/rank.py
+-rw-r--r--   0        0        0     2669 2023-06-19 19:38:12.441884 grammars-0.0.5/grammars/decode/visualize.py
+-rw-r--r--   0        0        0       37 2023-06-19 19:38:12.224937 grammars-0.0.5/grammars/parse/__init__.py
+-rw-r--r--   0        0        0     8244 2023-06-19 22:49:43.664734 grammars-0.0.5/grammars/parse/parsers.py
+-rw-r--r--   0        0        0      526 2023-06-20 22:57:29.477235 grammars-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 grammars-0.0.5/PKG-INFO
```

### Comparing `grammars-0.0.4/LICENSE` & `grammars-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/decode/decode.py` & `grammars-0.0.5/grammars/decode/decode.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/decode/generate.py` & `grammars-0.0.5/grammars/decode/generate.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/decode/modes.py` & `grammars-0.0.5/grammars/decode/modes.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/decode/rank.py` & `grammars-0.0.5/grammars/decode/rank.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/decode/visualize.py` & `grammars-0.0.5/grammars/decode/visualize.py`

 * *Files identical despite different names*

### Comparing `grammars-0.0.4/grammars/parse/parsers.py` & `grammars-0.0.5/grammars/parse/parsers.py`

 * *Files identical despite different names*

