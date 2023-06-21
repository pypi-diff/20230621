# Comparing `tmp/proto_schema_parser-0.1.0.tar.gz` & `tmp/proto_schema_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto_schema_parser-0.1.0.tar", last modified: Mon Jun 19 21:10:42 2023, max compression
+gzip compressed data, was "proto_schema_parser-0.2.0.tar", last modified: Wed Jun 21 16:07:59 2023, max compression
```

## Comparing `proto_schema_parser-0.1.0.tar` & `proto_schema_parser-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-06-19 20:44:40.014912 proto_schema_parser-0.1.0/LICENSE
--rw-r--r--   0        0        0     1915 2023-06-19 21:04:50.958983 proto_schema_parser-0.1.0/README.md
--rw-r--r--   0        0        0      159 2023-06-19 20:44:40.029432 proto_schema_parser-0.1.0/proto_schema_parser/__init__.py
--rw-r--r--   0        0        0    22913 2023-06-19 21:04:04.807667 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.interp
--rw-r--r--   0        0        0    22385 2023-06-19 21:04:04.944494 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.py
--rw-r--r--   0        0        0     1285 2023-06-19 21:04:04.975510 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.tokens
--rw-r--r--   0        0        0    29665 2023-06-19 21:04:05.119927 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.interp
--rw-r--r--   0        0        0   268632 2023-06-19 21:04:05.365103 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.py
--rw-r--r--   0        0        0     1285 2023-06-19 21:04:05.401645 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.tokens
--rw-r--r--   0        0        0    30623 2023-06-19 21:04:05.374046 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParserListener.py
--rw-r--r--   0        0        0    18134 2023-06-19 21:04:05.376325 proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParserVisitor.py
--rw-r--r--   0        0        0        0 2023-06-19 20:44:40.029511 proto_schema_parser-0.1.0/proto_schema_parser/antlr/__init__.py
--rw-r--r--   0        0        0      502 2023-06-19 20:44:40.029588 proto_schema_parser-0.1.0/proto_schema_parser/model.py
--rw-r--r--   0        0        0     3549 2023-06-19 21:07:44.319834 proto_schema_parser-0.1.0/proto_schema_parser/parser.py
--rw-r--r--   0        0        0     1237 2023-06-19 21:10:42.940854 proto_schema_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4921 2023-06-19 20:47:16.111081 proto_schema_parser-0.1.0/tests/test_parser.py
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 proto_schema_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-19 20:44:40.014912 proto_schema_parser-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2405 2023-06-21 16:07:40.720467 proto_schema_parser-0.2.0/README.md
+-rw-r--r--   0        0        0      157 2023-06-21 15:58:39.952033 proto_schema_parser-0.2.0/proto_schema_parser/__init__.py
+-rw-r--r--   0        0        0    22913 2023-06-21 15:58:03.887400 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.interp
+-rw-r--r--   0        0        0    22385 2023-06-21 15:58:03.887777 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.py
+-rw-r--r--   0        0        0     1285 2023-06-21 15:58:03.888019 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.tokens
+-rw-r--r--   0        0        0    29665 2023-06-21 15:58:03.888363 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.interp
+-rw-r--r--   0        0        0   268632 2023-06-21 15:58:03.889387 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.py
+-rw-r--r--   0        0        0     1285 2023-06-21 15:58:03.889520 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.tokens
+-rw-r--r--   0        0        0    30623 2023-06-21 15:58:03.889721 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserListener.py
+-rw-r--r--   0        0        0    18134 2023-06-21 15:58:03.889910 proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserVisitor.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:58:03.889952 proto_schema_parser-0.2.0/proto_schema_parser/antlr/__init__.py
+-rw-r--r--   0        0        0     4469 2023-06-21 16:07:40.720880 proto_schema_parser-0.2.0/proto_schema_parser/ast.py
+-rw-r--r--   0        0        0     8977 2023-06-21 16:07:40.721184 proto_schema_parser-0.2.0/proto_schema_parser/parser.py
+-rw-r--r--   0        0        0     1237 2023-06-21 16:07:59.283537 proto_schema_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    20338 2023-06-21 16:07:40.721458 proto_schema_parser-0.2.0/tests/test_parser.py
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 proto_schema_parser-0.2.0/PKG-INFO
```

### Comparing `proto_schema_parser-0.1.0/LICENSE` & `proto_schema_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.interp` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.py` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufLexer.tokens` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufLexer.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.interp` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.py` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParser.tokens` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParser.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParserListener.py` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserListener.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/proto_schema_parser/antlr/ProtobufParserVisitor.py` & `proto_schema_parser-0.2.0/proto_schema_parser/antlr/ProtobufParserVisitor.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-0.1.0/pyproject.toml` & `proto_schema_parser-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proto-schema-parser"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Pure Python Protobuf 3 .proto Parser"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
 ]
 dependencies = [
     "antlr4-python3-runtime>=4.13.0",
 ]
```

