# Comparing `tmp/periodparser-1.0.0.tar.gz` & `tmp/periodparser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodparser-1.0.0.tar", max compression
+gzip compressed data, was "periodparser-1.0.2.tar", max compression
```

## Comparing `periodparser-1.0.0.tar` & `periodparser-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     4857 2023-06-21 16:01:09.710595 periodparser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      913 2023-06-21 16:43:14.865639 periodparser-1.0.0/README.md
--rw-r--r--   0        0        0       28 2023-06-21 16:31:46.228137 periodparser-1.0.0/src/periodparser/__init__.py
--rw-r--r--   0        0        0       78 2022-03-11 09:45:50.000000 periodparser-1.0.0/src/periodparser/dict/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-21 16:12:34.689771 periodparser-1.0.0/src/periodparser/dict/keywords.py
--rw-r--r--   0        0        0     2031 2023-06-21 16:12:34.684771 periodparser-1.0.0/src/periodparser/dict/morph.py
--rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.0/src/periodparser/dict/time_words.txt
--rw-r--r--   0        0        0      162 2023-06-21 16:19:06.045163 periodparser-1.0.0/src/periodparser/models/__init__.py
--rw-r--r--   0        0        0     6422 2023-06-21 16:12:34.814768 periodparser-1.0.0/src/periodparser/models/abstract_period.py
--rw-r--r--   0        0        0     2833 2023-06-21 16:12:34.775767 periodparser-1.0.0/src/periodparser/models/dates_raw_data.py
--rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.0/src/periodparser/models/i_has_edges.py
--rw-r--r--   0        0        0     2449 2023-06-21 16:15:40.201881 periodparser-1.0.0/src/periodparser/models/parse_result.py
--rw-r--r--   0        0        0     2288 2023-06-21 16:12:34.783769 periodparser-1.0.0/src/periodparser/models/parser_models.py
--rw-r--r--   0        0        0      234 2022-03-10 09:07:25.000000 periodparser-1.0.0/src/periodparser/models/text_token.py
--rw-r--r--   0        0        0     1002 2023-06-21 16:12:34.604771 periodparser-1.0.0/src/periodparser/recognizers/__init__.py
--rw-r--r--   0        0        0     1139 2023-06-21 16:12:34.624772 periodparser-1.0.0/src/periodparser/recognizers/dates_period_recognizer.py
--rw-r--r--   0        0        0     1469 2023-06-21 16:12:34.644772 periodparser-1.0.0/src/periodparser/recognizers/day_of_week_recognizer.py
--rw-r--r--   0        0        0     1727 2023-06-21 16:12:34.669771 periodparser-1.0.0/src/periodparser/recognizers/days_month_recognizer.py
--rw-r--r--   0        0        0      906 2023-06-21 16:12:34.672771 periodparser-1.0.0/src/periodparser/recognizers/holidays_recognizer.py
--rw-r--r--   0        0        0     1283 2023-06-21 16:12:34.706772 periodparser-1.0.0/src/periodparser/recognizers/month_recognizer.py
--rw-r--r--   0        0        0     1347 2023-06-21 16:12:34.704771 periodparser-1.0.0/src/periodparser/recognizers/part_of_day_recognizer.py
--rw-r--r--   0        0        0     1621 2023-06-21 16:12:34.721772 periodparser-1.0.0/src/periodparser/recognizers/recognizer.py
--rw-r--r--   0        0        0     1231 2023-06-21 16:12:34.723772 periodparser-1.0.0/src/periodparser/recognizers/relative_date_recognizer.py
--rw-r--r--   0        0        0      732 2023-06-21 16:12:34.707770 periodparser-1.0.0/src/periodparser/recognizers/relative_day_recognizer.py
--rw-r--r--   0        0        0     3137 2023-06-21 16:12:34.762771 periodparser-1.0.0/src/periodparser/recognizers/time_recognizer.py
--rw-r--r--   0        0        0     2761 2023-06-21 16:12:34.759770 periodparser-1.0.0/src/periodparser/recognizers/time_span_recognizer.py
--rw-r--r--   0        0        0      726 2023-06-21 16:12:34.727772 periodparser-1.0.0/src/periodparser/recognizers/year_recognizer.py
--rw-r--r--   0        0        0     1906 2023-06-21 16:31:46.223137 periodparser-1.0.0/src/periodparser/sugar.py
--rw-r--r--   0        0        0    11845 2023-06-21 16:15:40.193881 periodparser-1.0.0/src/periodparser/text_parser.py
--rw-r--r--   0        0        0      118 2022-03-09 12:13:37.000000 periodparser-1.0.0/src/periodparser/utils/__init__.py
--rw-r--r--   0        0        0     1043 2023-06-21 16:12:34.731771 periodparser-1.0.0/src/periodparser/utils/helpers.py
--rw-r--r--   0        0        0     4849 2023-06-21 16:12:34.811768 periodparser-1.0.0/src/periodparser/utils/parser_extractors.py
--rw-r--r--   0        0        0      668 2023-06-21 16:12:34.742772 periodparser-1.0.0/src/periodparser/utils/parser_utils.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 periodparser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4857 2023-06-21 18:23:13.042232 periodparser-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1155 2023-06-21 18:14:22.458974 periodparser-1.0.2/README.md
+-rw-r--r--   0        0        0       52 2023-06-21 18:14:22.453118 periodparser-1.0.2/src/periodparser/__init__.py
+-rw-r--r--   0        0        0       78 2022-03-11 09:45:50.000000 periodparser-1.0.2/src/periodparser/dict/__init__.py
+-rw-r--r--   0        0        0     2828 2023-06-21 18:11:19.284584 periodparser-1.0.2/src/periodparser/dict/keywords.py
+-rw-r--r--   0        0        0     2031 2023-06-21 18:11:19.274583 periodparser-1.0.2/src/periodparser/dict/morph.py
+-rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.2/src/periodparser/dict/time_words.txt
+-rw-r--r--   0        0        0      161 2023-06-21 18:14:43.124972 periodparser-1.0.2/src/periodparser/models/__init__.py
+-rw-r--r--   0        0        0     6422 2023-06-21 18:11:19.451881 periodparser-1.0.2/src/periodparser/models/abstract_period.py
+-rw-r--r--   0        0        0     2833 2023-06-21 18:11:19.386881 periodparser-1.0.2/src/periodparser/models/dates_raw_data.py
+-rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.2/src/periodparser/models/i_has_edges.py
+-rw-r--r--   0        0        0     2448 2023-06-21 18:14:43.138971 periodparser-1.0.2/src/periodparser/models/parse_result.py
+-rw-r--r--   0        0        0     2288 2023-06-21 18:11:19.380881 periodparser-1.0.2/src/periodparser/models/parser_models.py
+-rw-r--r--   0        0        0      234 2022-03-10 09:07:25.000000 periodparser-1.0.2/src/periodparser/models/text_token.py
+-rw-r--r--   0        0        0     1002 2023-06-21 18:11:19.352584 periodparser-1.0.2/src/periodparser/recognizers/__init__.py
+-rw-r--r--   0        0        0     1139 2023-06-21 18:11:19.373880 periodparser-1.0.2/src/periodparser/recognizers/dates_period_recognizer.py
+-rw-r--r--   0        0        0     1469 2023-06-21 18:11:19.410883 periodparser-1.0.2/src/periodparser/recognizers/day_of_week_recognizer.py
+-rw-r--r--   0        0        0     1727 2023-06-21 18:11:19.237211 periodparser-1.0.2/src/periodparser/recognizers/days_month_recognizer.py
+-rw-r--r--   0        0        0      906 2023-06-21 18:11:19.266584 periodparser-1.0.2/src/periodparser/recognizers/holidays_recognizer.py
+-rw-r--r--   0        0        0     1283 2023-06-21 18:11:19.311584 periodparser-1.0.2/src/periodparser/recognizers/month_recognizer.py
+-rw-r--r--   0        0        0     1347 2023-06-21 18:11:19.314583 periodparser-1.0.2/src/periodparser/recognizers/part_of_day_recognizer.py
+-rw-r--r--   0        0        0     1621 2023-06-21 18:11:19.352584 periodparser-1.0.2/src/periodparser/recognizers/recognizer.py
+-rw-r--r--   0        0        0     1231 2023-06-21 18:11:19.348583 periodparser-1.0.2/src/periodparser/recognizers/relative_date_recognizer.py
+-rw-r--r--   0        0        0      732 2023-06-21 18:11:19.339583 periodparser-1.0.2/src/periodparser/recognizers/relative_day_recognizer.py
+-rw-r--r--   0        0        0     3137 2023-06-21 18:11:19.416882 periodparser-1.0.2/src/periodparser/recognizers/time_recognizer.py
+-rw-r--r--   0        0        0     2761 2023-06-21 18:11:19.415882 periodparser-1.0.2/src/periodparser/recognizers/time_span_recognizer.py
+-rw-r--r--   0        0        0      726 2023-06-21 18:11:19.376881 periodparser-1.0.2/src/periodparser/recognizers/year_recognizer.py
+-rw-r--r--   0        0        0     2481 2023-06-21 18:16:15.025965 periodparser-1.0.2/src/periodparser/sugar.py
+-rw-r--r--   0        0        0    11842 2023-06-21 18:14:43.131971 periodparser-1.0.2/src/periodparser/text_parser.py
+-rw-r--r--   0        0        0      118 2022-03-09 12:13:37.000000 periodparser-1.0.2/src/periodparser/utils/__init__.py
+-rw-r--r--   0        0        0     1043 2023-06-21 18:11:19.376881 periodparser-1.0.2/src/periodparser/utils/helpers.py
+-rw-r--r--   0        0        0     4849 2023-06-21 18:11:19.468879 periodparser-1.0.2/src/periodparser/utils/parser_extractors.py
+-rw-r--r--   0        0        0      668 2023-06-21 18:11:19.395881 periodparser-1.0.2/src/periodparser/utils/parser_utils.py
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 periodparser-1.0.2/PKG-INFO
```

### Comparing `periodparser-1.0.0/pyproject.toml` & `periodparser-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "periodparser"
-version = "1.0.0"
+version = "1.0.2"
 description = "python parser for human readable period dates"
 authors = ["fenn_r <fenrir1121@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/fennr/periodparser"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.0"
+version = "1.0.2"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.8,<4.0"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 black = ">=23.3.0"
```

### Comparing `periodparser-1.0.0/README.md` & `periodparser-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/periodparser)
+![PyPI - Python Version](https://img.shields.io/pypi/v/periodparser)
+![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)
+
+
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=git@github.com:fennr/periodparser)
 
 # periodparser
 
 python parser for human-readable period dates
 
 ## Установка
@@ -13,10 +18,11 @@
 Библиотека для парсинга дат и времени в естественной речи на русском языке.
 
 ## Пример
 
 ```python
 import periodparser as pp
 
-result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
-print(result.dates[0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
+result = pp.exctract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
+print(result.dates[
+          0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
 ```
```

### Comparing `periodparser-1.0.0/src/periodparser/dict/keywords.py` & `periodparser-1.0.2/src/periodparser/dict/keywords.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/dict/morph.py` & `periodparser-1.0.2/src/periodparser/dict/morph.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/dict/time_words.txt` & `periodparser-1.0.2/src/periodparser/dict/time_words.txt`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/models/abstract_period.py` & `periodparser-1.0.2/src/periodparser/models/abstract_period.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/models/dates_raw_data.py` & `periodparser-1.0.2/src/periodparser/models/dates_raw_data.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/models/parse_result.py` & `periodparser-1.0.2/src/periodparser/models/parse_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict, Set, Any
 from re import sub
 
 from ..utils import Helpers
 from .parser_models import DateTimeToken
 
 
-class PeriodResult:
+class ParseResult:
     source_text: str
     tokens: List[str]
     text: str
     dates: List[DateTimeToken]
 
     __full_dates: List[DateTimeToken]
     __tokens_to_remove: Set[str] = set()
```

### Comparing `periodparser-1.0.0/src/periodparser/models/parser_models.py` & `periodparser-1.0.2/src/periodparser/models/parser_models.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/__init__.py` & `periodparser-1.0.2/src/periodparser/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/dates_period_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/dates_period_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/day_of_week_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/day_of_week_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/days_month_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/days_month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/holidays_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/holidays_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/month_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/part_of_day_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/part_of_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/relative_date_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/relative_date_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/relative_day_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/relative_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/time_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/time_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/time_span_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/time_span_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/recognizers/year_recognizer.py` & `periodparser-1.0.2/src/periodparser/recognizers/year_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/sugar.py` & `periodparser-1.0.2/src/periodparser/sugar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Optional
 from re import sub
 
-from .models.parse_result import PeriodResult
+from .models.parse_result import ParseResult
 from .text_parser import parse
 
 
 def preprocess(phrase: str) -> str:
     # change forms
     phrase = phrase.replace("часок", "час")
     phrase = phrase.replace("часиков", "часов")
@@ -32,17 +32,27 @@
 
 def preprocess_today(phrase: str) -> str:
     phrase = phrase.replace("вечерком", "вечером").replace("ближе к вечеру", "вечером")
     phrase = sub(r"(вечером|днём|утром)", r"сегодня \1", phrase)
     return phrase
 
 
-def extract(phrase: str, now: Optional[datetime] = None) -> PeriodResult:
+def exctract(phrase: str, now: Optional[datetime] = None) -> ParseResult:
+    """
+        Извлекает период времени из заданной фразы и возвращает объект PeriodResult
+
+        :param phrase: Строка, содержащая период времени
+        :type phrase: str
+        :param now: Опциональный параметр, представляющий текущий момент времени
+        :type now: Optional[datetime]
+        :return: PeriodResult содержащий информацию о промежутке времени
+        :rtype: PeriodResult
+        """
     phrase = preprocess(phrase)
     now = now or datetime.now()
 
-    period_result = parse(phrase, now)
-    if not period_result.dates:
+    hors_result = parse(phrase, now)
+    if not hors_result.dates:
         phrase = preprocess_today(phrase)
-        period_result = parse(phrase, now)
+        hors_result = parse(phrase, now)
 
-    return period_result
+    return hors_result
```

### Comparing `periodparser-1.0.0/src/periodparser/text_parser.py` & `periodparser-1.0.2/src/periodparser/text_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,23 +241,23 @@
 
             for p in overlap_periods:
                 p.start = min_index
                 p.end = max_index
                 skipped.add(p)
 
 
-def parse(text: str, now: datetime) -> PeriodResult:
+def parse(text: str, now: datetime) -> ParseResult:
     tokens = RX_SPLIT.split(text)
     split_tokens = [(m.start(), m.end() - m.start()) for m in RX_SPLIT.finditer(text)]
     return do_parse(tokens, text, split_tokens, now)
 
 
 def do_parse(
     tokens: List[str], text: str, split_tokens: ITuplesList, now: datetime
-) -> PeriodResult:
+) -> ParseResult:
     collapse_distance = 4
 
     data = DatesRawData(tokens)
     data.create_tokens(tokens)
 
     for r in recognizers:
         r.parse_tokens(data, now)
@@ -296,8 +296,8 @@
         "(([fo]?(@)t(@))|([fo]?(@)))",
         lambda m: create_date_period(m, data, now, final_periods),
     )
 
     fix_overlap(final_periods)
     fix_indexes(final_periods, split_tokens)
 
-    return PeriodResult(text, [t.value for t in data.tokens], final_periods)
+    return ParseResult(text, [t.value for t in data.tokens], final_periods)
```

### Comparing `periodparser-1.0.0/src/periodparser/utils/helpers.py` & `periodparser-1.0.2/src/periodparser/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/utils/parser_extractors.py` & `periodparser-1.0.2/src/periodparser/utils/parser_extractors.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/src/periodparser/utils/parser_utils.py` & `periodparser-1.0.2/src/periodparser/utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.0/PKG-INFO` & `periodparser-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: periodparser
-Version: 1.0.0
+Version: 1.0.2
 Summary: python parser for human readable period dates
 Home-page: https://github.com/fennr/periodparser
 Author: fenn_r
 Author-email: fenrir1121@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/fennr/periodparser
 Description-Content-Type: text/markdown
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/periodparser)
+![PyPI - Python Version](https://img.shields.io/pypi/v/periodparser)
+![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)
+
+
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=git@github.com:fennr/periodparser)
 
 # periodparser
 
 python parser for human-readable period dates
 
 ## Установка
@@ -29,10 +34,11 @@
 Библиотека для парсинга дат и времени в естественной речи на русском языке.
 
 ## Пример
 
 ```python
 import periodparser as pp
 
-result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
-print(result.dates[0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
+result = pp.exctract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
+print(result.dates[
+          0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
 ```
```

