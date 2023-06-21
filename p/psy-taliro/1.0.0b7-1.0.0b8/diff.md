# Comparing `tmp/PSY-TaLiRo-1.0.0b7.tar.gz` & `tmp/psy_taliro-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSY-TaLiRo-1.0.0b7.tar", max compression
+gzip compressed data, was "psy_taliro-1.0.0b8.tar", max compression
```

## Comparing `PSY-TaLiRo-1.0.0b7.tar` & `psy_taliro-1.0.0b8.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1520 2021-11-08 18:51:51.678033 PSY-TaLiRo-1.0.0b7/LICENSE
--rw-r--r--   0        0        0     1601 2022-09-16 16:43:54.451013 PSY-TaLiRo-1.0.0b7/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-08 18:51:51.686034 PSY-TaLiRo-1.0.0b7/src/staliro/__init__.py
--rw-r--r--   0        0        0      786 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/__init__.py
--rw-r--r--   0        0        0     7484 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/cost.py
--rw-r--r--   0        0        0     1508 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/core/interval.py
--rw-r--r--   0        0        0     1602 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/layout.py
--rw-r--r--   0        0        0     3215 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/model.py
--rw-r--r--   0        0        0     2087 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/optimizer.py
--rw-r--r--   0        0        0     5087 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/result.py
--rw-r--r--   0        0        0     1733 2022-05-17 20:52:27.240725 PSY-TaLiRo-1.0.0b7/src/staliro/core/sample.py
--rw-r--r--   0        0        0     8058 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/scenario.py
--rw-r--r--   0        0        0      763 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/core/signal.py
--rw-r--r--   0        0        0     1222 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/core/specification.py
--rw-r--r--   0        0        0     5133 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/models.py
--rw-r--r--   0        0        0     5430 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/optimizers.py
--rw-r--r--   0        0        0     5180 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/options.py
--rw-r--r--   0        0        0      155 2022-09-12 20:44:09.130089 PSY-TaLiRo-1.0.0b7/src/staliro/parser/__init__.py
--rw-r--r--   0        0        0     1317 2021-11-08 18:51:51.686034 PSY-TaLiRo-1.0.0b7/src/staliro/parser/grammar/stlLexer.g4
--rw-r--r--   0        0        0      791 2021-11-08 18:51:51.686034 PSY-TaLiRo-1.0.0b7/src/staliro/parser/grammar/stlParser.g4
--rw-r--r--   0        0        0     3431 2022-09-12 20:44:09.130089 PSY-TaLiRo-1.0.0b7/src/staliro/parser/parser.py
--rw-r--r--   0        0        0    12212 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlLexer.py
--rw-r--r--   0        0        0    32028 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParser.py
--rw-r--r--   0        0        0     3986 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParserListener.py
--rw-r--r--   0        0        0     6496 2022-08-16 15:47:49.143132 PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParserVisitor.py
--rw-r--r--   0        0        0     8586 2022-09-12 20:44:09.130089 PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlTptlParserVisitorTranslator.py
--rw-r--r--   0        0        0        0 2021-11-08 18:51:51.686034 PSY-TaLiRo-1.0.0b7/src/staliro/py.typed
--rw-r--r--   0        0        0     4547 2022-08-16 15:47:49.147132 PSY-TaLiRo-1.0.0b7/src/staliro/signals.py
--rw-r--r--   0        0        0    10272 2022-09-13 12:48:41.295908 PSY-TaLiRo-1.0.0b7/src/staliro/specifications.py
--rw-r--r--   0        0        0     4168 2022-09-06 02:20:07.063027 PSY-TaLiRo-1.0.0b7/src/staliro/staliro.py
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 PSY-TaLiRo-1.0.0b7/setup.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 PSY-TaLiRo-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-05-09 16:22:40.594155 psy_taliro-1.0.0b8/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-21 00:24:23.401552 psy_taliro-1.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 23:38:32.004447 psy_taliro-1.0.0b8/src/staliro/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-12 23:38:32.004833 psy_taliro-1.0.0b8/src/staliro/core/__init__.py
+-rw-r--r--   0        0        0     7484 2023-06-12 23:38:32.004952 psy_taliro-1.0.0b8/src/staliro/core/cost.py
+-rw-r--r--   0        0        0     1508 2023-06-12 23:38:32.005305 psy_taliro-1.0.0b8/src/staliro/core/interval.py
+-rw-r--r--   0        0        0     1602 2023-06-12 23:38:32.005461 psy_taliro-1.0.0b8/src/staliro/core/layout.py
+-rw-r--r--   0        0        0     3215 2023-06-12 23:38:32.005576 psy_taliro-1.0.0b8/src/staliro/core/model.py
+-rw-r--r--   0        0        0     2087 2023-06-12 23:38:32.005727 psy_taliro-1.0.0b8/src/staliro/core/optimizer.py
+-rw-r--r--   0        0        0     5087 2023-06-12 23:38:32.005906 psy_taliro-1.0.0b8/src/staliro/core/result.py
+-rw-r--r--   0        0        0     1733 2023-06-12 23:38:32.006035 psy_taliro-1.0.0b8/src/staliro/core/sample.py
+-rw-r--r--   0        0        0     8058 2023-06-12 23:38:32.006184 psy_taliro-1.0.0b8/src/staliro/core/scenario.py
+-rw-r--r--   0        0        0      763 2023-06-12 23:38:32.006343 psy_taliro-1.0.0b8/src/staliro/core/signal.py
+-rw-r--r--   0        0        0     1222 2023-06-12 23:38:32.006459 psy_taliro-1.0.0b8/src/staliro/core/specification.py
+-rw-r--r--   0        0        0     5133 2023-06-12 23:38:32.006577 psy_taliro-1.0.0b8/src/staliro/models.py
+-rw-r--r--   0        0        0     5430 2023-06-12 23:38:32.006693 psy_taliro-1.0.0b8/src/staliro/optimizers.py
+-rw-r--r--   0        0        0     5180 2023-06-12 23:38:32.006871 psy_taliro-1.0.0b8/src/staliro/options.py
+-rw-r--r--   0        0        0      155 2023-05-09 16:22:40.597460 psy_taliro-1.0.0b8/src/staliro/parser/__init__.py
+-rw-r--r--   0        0        0     1317 2023-05-09 16:22:40.597538 psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlLexer.g4
+-rw-r--r--   0        0        0      791 2023-05-09 16:22:40.597591 psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlParser.g4
+-rw-r--r--   0        0        0     3431 2023-05-16 00:14:46.061497 psy_taliro-1.0.0b8/src/staliro/parser/parser.py
+-rw-r--r--   0        0        0    12212 2023-05-09 16:22:40.597746 psy_taliro-1.0.0b8/src/staliro/parser/stlLexer.py
+-rw-r--r--   0        0        0    32028 2023-05-09 16:22:40.597877 psy_taliro-1.0.0b8/src/staliro/parser/stlParser.py
+-rw-r--r--   0        0        0     3986 2023-05-09 16:22:40.597963 psy_taliro-1.0.0b8/src/staliro/parser/stlParserListener.py
+-rw-r--r--   0        0        0     6496 2023-05-09 16:22:40.598018 psy_taliro-1.0.0b8/src/staliro/parser/stlParserVisitor.py
+-rw-r--r--   0        0        0     8586 2023-05-09 16:22:40.598105 psy_taliro-1.0.0b8/src/staliro/parser/stlTptlParserVisitorTranslator.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:22:40.598128 psy_taliro-1.0.0b8/src/staliro/py.typed
+-rw-r--r--   0        0        0     4547 2023-06-12 23:38:32.007007 psy_taliro-1.0.0b8/src/staliro/signals.py
+-rw-r--r--   0        0        0    10272 2023-06-12 23:38:32.007174 psy_taliro-1.0.0b8/src/staliro/specifications.py
+-rw-r--r--   0        0        0     4168 2023-06-12 23:38:32.007310 psy_taliro-1.0.0b8/src/staliro/staliro.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 psy_taliro-1.0.0b8/PKG-INFO
```

### Comparing `PSY-TaLiRo-1.0.0b7/LICENSE` & `psy_taliro-1.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/pyproject.toml` & `psy_taliro-1.0.0b8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PSY-TaLiRo"
-version = "1.0.0b7"
+version = "1.0.0b8"
 description = "System-level verification library using STL"
 authors = ["Quinn Thibeault <qthibeau@asu.edu>", "Jacob Anderson <jwande18@asu.edu>"]
 license = "BSD-3-Clause"
 packages = [
     {include = "staliro", from = "src"}
 ]
 
@@ -12,15 +12,22 @@
 python = ">=3.8, <3.11"
 antlr4-python3-runtime = ">=4.7"
 attrs = "^21.0.0"
 numpy = "^1.21.5"
 scipy = "^1.6.2"
 typing-extensions = "^4.2.0"
 matplotlib = "^3.5.2"
-py-taliro = "^0.2.1"
+py-taliro = { version = "^0.2.1", optional = true }
+rtamt = { version = "^0.3.5", optional = true }
+tltk-mtl = { version = "^0.0.27", optional = true, markers = "sys_platform == 'linux'" }
+
+[tool.poetry.extras]
+rtamt = ["rtamt"]
+pytaliro = ["py-taliro"]
+tltk = ["tltk-mtl"]
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 mypy = "^0"
 flake8 = "^4.0.0"
 flake8-comprehensions = "^3.4.0"
```

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/__init__.py` & `psy_taliro-1.0.0b8/src/staliro/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/cost.py` & `psy_taliro-1.0.0b8/src/staliro/core/cost.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/interval.py` & `psy_taliro-1.0.0b8/src/staliro/core/interval.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/layout.py` & `psy_taliro-1.0.0b8/src/staliro/core/layout.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/model.py` & `psy_taliro-1.0.0b8/src/staliro/core/model.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/optimizer.py` & `psy_taliro-1.0.0b8/src/staliro/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/result.py` & `psy_taliro-1.0.0b8/src/staliro/core/result.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/sample.py` & `psy_taliro-1.0.0b8/src/staliro/core/sample.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/scenario.py` & `psy_taliro-1.0.0b8/src/staliro/core/scenario.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/signal.py` & `psy_taliro-1.0.0b8/src/staliro/core/signal.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/core/specification.py` & `psy_taliro-1.0.0b8/src/staliro/core/specification.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/models.py` & `psy_taliro-1.0.0b8/src/staliro/models.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/optimizers.py` & `psy_taliro-1.0.0b8/src/staliro/optimizers.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/options.py` & `psy_taliro-1.0.0b8/src/staliro/options.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/grammar/stlLexer.g4` & `psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlLexer.g4`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/grammar/stlParser.g4` & `psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlParser.g4`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/parser.py` & `psy_taliro-1.0.0b8/src/staliro/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlLexer.py` & `psy_taliro-1.0.0b8/src/staliro/parser/stlLexer.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParser.py` & `psy_taliro-1.0.0b8/src/staliro/parser/stlParser.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParserListener.py` & `psy_taliro-1.0.0b8/src/staliro/parser/stlParserListener.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlParserVisitor.py` & `psy_taliro-1.0.0b8/src/staliro/parser/stlParserVisitor.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/parser/stlTptlParserVisitorTranslator.py` & `psy_taliro-1.0.0b8/src/staliro/parser/stlTptlParserVisitorTranslator.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/signals.py` & `psy_taliro-1.0.0b8/src/staliro/signals.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/specifications.py` & `psy_taliro-1.0.0b8/src/staliro/specifications.py`

 * *Files identical despite different names*

### Comparing `PSY-TaLiRo-1.0.0b7/src/staliro/staliro.py` & `psy_taliro-1.0.0b8/src/staliro/staliro.py`

 * *Files identical despite different names*

