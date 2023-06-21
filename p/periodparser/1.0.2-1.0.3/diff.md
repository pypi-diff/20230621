# Comparing `tmp/periodparser-1.0.2.tar.gz` & `tmp/periodparser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodparser-1.0.2.tar", max compression
+gzip compressed data, was "periodparser-1.0.3.tar", max compression
```

## Comparing `periodparser-1.0.2.tar` & `periodparser-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     4857 2023-06-21 18:23:13.042232 periodparser-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1155 2023-06-21 18:14:22.458974 periodparser-1.0.2/README.md
--rw-r--r--   0        0        0       52 2023-06-21 18:14:22.453118 periodparser-1.0.2/src/periodparser/__init__.py
--rw-r--r--   0        0        0       78 2022-03-11 09:45:50.000000 periodparser-1.0.2/src/periodparser/dict/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-21 18:11:19.284584 periodparser-1.0.2/src/periodparser/dict/keywords.py
--rw-r--r--   0        0        0     2031 2023-06-21 18:11:19.274583 periodparser-1.0.2/src/periodparser/dict/morph.py
--rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.2/src/periodparser/dict/time_words.txt
--rw-r--r--   0        0        0      161 2023-06-21 18:14:43.124972 periodparser-1.0.2/src/periodparser/models/__init__.py
--rw-r--r--   0        0        0     6422 2023-06-21 18:11:19.451881 periodparser-1.0.2/src/periodparser/models/abstract_period.py
--rw-r--r--   0        0        0     2833 2023-06-21 18:11:19.386881 periodparser-1.0.2/src/periodparser/models/dates_raw_data.py
--rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.2/src/periodparser/models/i_has_edges.py
--rw-r--r--   0        0        0     2448 2023-06-21 18:14:43.138971 periodparser-1.0.2/src/periodparser/models/parse_result.py
--rw-r--r--   0        0        0     2288 2023-06-21 18:11:19.380881 periodparser-1.0.2/src/periodparser/models/parser_models.py
--rw-r--r--   0        0        0      234 2022-03-10 09:07:25.000000 periodparser-1.0.2/src/periodparser/models/text_token.py
--rw-r--r--   0        0        0     1002 2023-06-21 18:11:19.352584 periodparser-1.0.2/src/periodparser/recognizers/__init__.py
--rw-r--r--   0        0        0     1139 2023-06-21 18:11:19.373880 periodparser-1.0.2/src/periodparser/recognizers/dates_period_recognizer.py
--rw-r--r--   0        0        0     1469 2023-06-21 18:11:19.410883 periodparser-1.0.2/src/periodparser/recognizers/day_of_week_recognizer.py
--rw-r--r--   0        0        0     1727 2023-06-21 18:11:19.237211 periodparser-1.0.2/src/periodparser/recognizers/days_month_recognizer.py
--rw-r--r--   0        0        0      906 2023-06-21 18:11:19.266584 periodparser-1.0.2/src/periodparser/recognizers/holidays_recognizer.py
--rw-r--r--   0        0        0     1283 2023-06-21 18:11:19.311584 periodparser-1.0.2/src/periodparser/recognizers/month_recognizer.py
--rw-r--r--   0        0        0     1347 2023-06-21 18:11:19.314583 periodparser-1.0.2/src/periodparser/recognizers/part_of_day_recognizer.py
--rw-r--r--   0        0        0     1621 2023-06-21 18:11:19.352584 periodparser-1.0.2/src/periodparser/recognizers/recognizer.py
--rw-r--r--   0        0        0     1231 2023-06-21 18:11:19.348583 periodparser-1.0.2/src/periodparser/recognizers/relative_date_recognizer.py
--rw-r--r--   0        0        0      732 2023-06-21 18:11:19.339583 periodparser-1.0.2/src/periodparser/recognizers/relative_day_recognizer.py
--rw-r--r--   0        0        0     3137 2023-06-21 18:11:19.416882 periodparser-1.0.2/src/periodparser/recognizers/time_recognizer.py
--rw-r--r--   0        0        0     2761 2023-06-21 18:11:19.415882 periodparser-1.0.2/src/periodparser/recognizers/time_span_recognizer.py
--rw-r--r--   0        0        0      726 2023-06-21 18:11:19.376881 periodparser-1.0.2/src/periodparser/recognizers/year_recognizer.py
--rw-r--r--   0        0        0     2481 2023-06-21 18:16:15.025965 periodparser-1.0.2/src/periodparser/sugar.py
--rw-r--r--   0        0        0    11842 2023-06-21 18:14:43.131971 periodparser-1.0.2/src/periodparser/text_parser.py
--rw-r--r--   0        0        0      118 2022-03-09 12:13:37.000000 periodparser-1.0.2/src/periodparser/utils/__init__.py
--rw-r--r--   0        0        0     1043 2023-06-21 18:11:19.376881 periodparser-1.0.2/src/periodparser/utils/helpers.py
--rw-r--r--   0        0        0     4849 2023-06-21 18:11:19.468879 periodparser-1.0.2/src/periodparser/utils/parser_extractors.py
--rw-r--r--   0        0        0      668 2023-06-21 18:11:19.395881 periodparser-1.0.2/src/periodparser/utils/parser_utils.py
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 periodparser-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4857 2023-06-21 18:31:00.723311 periodparser-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1154 2023-06-21 18:31:00.722309 periodparser-1.0.3/README.md
+-rw-r--r--   0        0        0       28 2023-06-21 18:31:00.724310 periodparser-1.0.3/src/periodparser/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-21 18:31:00.724310 periodparser-1.0.3/src/periodparser/dict/__init__.py
+-rw-r--r--   0        0        0     2828 2023-06-21 18:31:00.725311 periodparser-1.0.3/src/periodparser/dict/keywords.py
+-rw-r--r--   0        0        0     2031 2023-06-21 18:31:00.726310 periodparser-1.0.3/src/periodparser/dict/morph.py
+-rw-r--r--   0        0        0    13223 2020-03-04 13:43:34.000000 periodparser-1.0.3/src/periodparser/dict/time_words.txt
+-rw-r--r--   0        0        0      161 2023-06-21 18:31:00.727310 periodparser-1.0.3/src/periodparser/models/__init__.py
+-rw-r--r--   0        0        0     6422 2023-06-21 18:31:00.728311 periodparser-1.0.3/src/periodparser/models/abstract_period.py
+-rw-r--r--   0        0        0     2833 2023-06-21 18:31:00.728311 periodparser-1.0.3/src/periodparser/models/dates_raw_data.py
+-rw-r--r--   0        0        0      158 2022-03-10 14:47:55.000000 periodparser-1.0.3/src/periodparser/models/i_has_edges.py
+-rw-r--r--   0        0        0     2448 2023-06-21 18:31:00.729312 periodparser-1.0.3/src/periodparser/models/parse_result.py
+-rw-r--r--   0        0        0     2288 2023-06-21 18:31:00.730309 periodparser-1.0.3/src/periodparser/models/parser_models.py
+-rw-r--r--   0        0        0      234 2023-06-21 18:31:00.731310 periodparser-1.0.3/src/periodparser/models/text_token.py
+-rw-r--r--   0        0        0     1002 2023-06-21 18:31:00.732309 periodparser-1.0.3/src/periodparser/recognizers/__init__.py
+-rw-r--r--   0        0        0     1139 2023-06-21 18:31:00.733310 periodparser-1.0.3/src/periodparser/recognizers/dates_period_recognizer.py
+-rw-r--r--   0        0        0     1469 2023-06-21 18:31:00.733310 periodparser-1.0.3/src/periodparser/recognizers/day_of_week_recognizer.py
+-rw-r--r--   0        0        0     1727 2023-06-21 18:31:00.734312 periodparser-1.0.3/src/periodparser/recognizers/days_month_recognizer.py
+-rw-r--r--   0        0        0      906 2023-06-21 18:31:00.735312 periodparser-1.0.3/src/periodparser/recognizers/holidays_recognizer.py
+-rw-r--r--   0        0        0     1283 2023-06-21 18:31:00.735312 periodparser-1.0.3/src/periodparser/recognizers/month_recognizer.py
+-rw-r--r--   0        0        0     1347 2023-06-21 18:31:00.736309 periodparser-1.0.3/src/periodparser/recognizers/part_of_day_recognizer.py
+-rw-r--r--   0        0        0     1621 2023-06-21 18:31:00.737311 periodparser-1.0.3/src/periodparser/recognizers/recognizer.py
+-rw-r--r--   0        0        0     1231 2023-06-21 18:31:00.738309 periodparser-1.0.3/src/periodparser/recognizers/relative_date_recognizer.py
+-rw-r--r--   0        0        0      732 2023-06-21 18:31:00.739309 periodparser-1.0.3/src/periodparser/recognizers/relative_day_recognizer.py
+-rw-r--r--   0        0        0     3137 2023-06-21 18:31:00.740311 periodparser-1.0.3/src/periodparser/recognizers/time_recognizer.py
+-rw-r--r--   0        0        0     2761 2023-06-21 18:31:00.740311 periodparser-1.0.3/src/periodparser/recognizers/time_span_recognizer.py
+-rw-r--r--   0        0        0      726 2023-06-21 18:31:00.741311 periodparser-1.0.3/src/periodparser/recognizers/year_recognizer.py
+-rw-r--r--   0        0        0     2538 2023-06-21 18:31:00.742316 periodparser-1.0.3/src/periodparser/sugar.py
+-rw-r--r--   0        0        0    11842 2023-06-21 18:31:00.743310 periodparser-1.0.3/src/periodparser/text_parser.py
+-rw-r--r--   0        0        0      118 2023-06-21 18:31:00.744312 periodparser-1.0.3/src/periodparser/utils/__init__.py
+-rw-r--r--   0        0        0     1043 2023-06-21 18:31:00.745309 periodparser-1.0.3/src/periodparser/utils/helpers.py
+-rw-r--r--   0        0        0     4849 2023-06-21 18:31:00.745309 periodparser-1.0.3/src/periodparser/utils/parser_extractors.py
+-rw-r--r--   0        0        0      668 2023-06-21 18:31:00.746311 periodparser-1.0.3/src/periodparser/utils/parser_utils.py
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 periodparser-1.0.3/PKG-INFO
```

### Comparing `periodparser-1.0.2/pyproject.toml` & `periodparser-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "periodparser"
-version = "1.0.2"
+version = "1.0.3"
 description = "python parser for human readable period dates"
 authors = ["fenn_r <fenrir1121@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/fennr/periodparser"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.2"
+version = "1.0.3"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.8,<4.0"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 black = ">=23.3.0"
```

### Comparing `periodparser-1.0.2/README.md` & `periodparser-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 Библиотека для парсинга дат и времени в естественной речи на русском языке.
 
 ## Пример
 
 ```python
 import periodparser as pp
 
-result = pp.exctract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
+result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
 print(result.dates[
           0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
 ```
```

### Comparing `periodparser-1.0.2/src/periodparser/dict/keywords.py` & `periodparser-1.0.3/src/periodparser/dict/keywords.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/dict/morph.py` & `periodparser-1.0.3/src/periodparser/dict/morph.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/dict/time_words.txt` & `periodparser-1.0.3/src/periodparser/dict/time_words.txt`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/models/abstract_period.py` & `periodparser-1.0.3/src/periodparser/models/abstract_period.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/models/dates_raw_data.py` & `periodparser-1.0.3/src/periodparser/models/dates_raw_data.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/models/parse_result.py` & `periodparser-1.0.3/src/periodparser/models/parse_result.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/models/parser_models.py` & `periodparser-1.0.3/src/periodparser/models/parser_models.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/__init__.py` & `periodparser-1.0.3/src/periodparser/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/dates_period_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/dates_period_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/day_of_week_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/day_of_week_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/days_month_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/days_month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/holidays_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/holidays_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/month_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/month_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/part_of_day_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/part_of_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/relative_date_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/relative_date_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/relative_day_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/relative_day_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/time_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/time_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/time_span_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/time_span_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/recognizers/year_recognizer.py` & `periodparser-1.0.3/src/periodparser/recognizers/year_recognizer.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/sugar.py` & `periodparser-1.0.3/src/periodparser/sugar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from datetime import datetime
-from typing import Optional
-from re import sub
-
-from .models.parse_result import ParseResult
-from .text_parser import parse
-
-
-def preprocess(phrase: str) -> str:
-    # change forms
-    phrase = phrase.replace("часок", "час")
-    phrase = phrase.replace("часиков", "часов")
-    phrase = phrase.replace("минуток", "минут")
-
-    # translate times
-    phrase = phrase.replace("полчаса", "30 минут")
-    phrase = phrase.replace("полчасика", "30 минут")
-    phrase = phrase.replace("полтора часа", "1 час 30 минут")
-    phrase = phrase.replace("через пару часов", "через 2 часа")
-    phrase = phrase.replace("в обед", "в 13 часов")
-    phrase = phrase.replace("после обеда", "в 14 часов")
-
-    # swap syntax
-    phrase = sub(r"через (минут|часов|часа) (\d*)", r"через \2 \1", phrase)
-    phrase = sub(r"(минут|часов|часа) через (\d*)", r"через \2 \1", phrase)
-    phrase = sub(r"в течение (\w*а)", r"через \1", phrase)
-    phrase = phrase.replace("получас", "30 минут")
-    phrase = sub(r"(\d+) с половиной часа", r"\1 часа 30 минут", phrase)
-
-    return phrase
-
-
-def preprocess_today(phrase: str) -> str:
-    phrase = phrase.replace("вечерком", "вечером").replace("ближе к вечеру", "вечером")
-    phrase = sub(r"(вечером|днём|утром)", r"сегодня \1", phrase)
-    return phrase
-
-
-def exctract(phrase: str, now: Optional[datetime] = None) -> ParseResult:
-    """
-        Извлекает период времени из заданной фразы и возвращает объект PeriodResult
-
-        :param phrase: Строка, содержащая период времени
-        :type phrase: str
-        :param now: Опциональный параметр, представляющий текущий момент времени
-        :type now: Optional[datetime]
-        :return: PeriodResult содержащий информацию о промежутке времени
-        :rtype: PeriodResult
-        """
-    phrase = preprocess(phrase)
-    now = now or datetime.now()
-
-    hors_result = parse(phrase, now)
-    if not hors_result.dates:
-        phrase = preprocess_today(phrase)
-        hors_result = parse(phrase, now)
-
-    return hors_result
+from datetime import datetime
+from typing import Optional
+from re import sub
+
+from .models.parse_result import ParseResult
+from .text_parser import parse
+
+
+def preprocess(phrase: str) -> str:
+    # change forms
+    phrase = phrase.replace("часок", "час")
+    phrase = phrase.replace("часиков", "часов")
+    phrase = phrase.replace("минуток", "минут")
+
+    # translate times
+    phrase = phrase.replace("полчаса", "30 минут")
+    phrase = phrase.replace("полчасика", "30 минут")
+    phrase = phrase.replace("полтора часа", "1 час 30 минут")
+    phrase = phrase.replace("через пару часов", "через 2 часа")
+    phrase = phrase.replace("в обед", "в 13 часов")
+    phrase = phrase.replace("после обеда", "в 14 часов")
+
+    # swap syntax
+    phrase = sub(r"через (минут|часов|часа) (\d*)", r"через \2 \1", phrase)
+    phrase = sub(r"(минут|часов|часа) через (\d*)", r"через \2 \1", phrase)
+    phrase = sub(r"в течение (\w*а)", r"через \1", phrase)
+    phrase = phrase.replace("получас", "30 минут")
+    phrase = sub(r"(\d+) с половиной часа", r"\1 часа 30 минут", phrase)
+
+    return phrase
+
+
+def preprocess_today(phrase: str) -> str:
+    phrase = phrase.replace("вечерком", "вечером").replace("ближе к вечеру", "вечером")
+    phrase = sub(r"(вечером|днём|утром)", r"сегодня \1", phrase)
+    return phrase
+
+
+def extract(phrase: str, now: Optional[datetime] = None) -> ParseResult:
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
+    phrase = preprocess(phrase)
+    now = now or datetime.now()
+
+    hors_result = parse(phrase, now)
+    if not hors_result.dates:
+        phrase = preprocess_today(phrase)
+        hors_result = parse(phrase, now)
+
+    return hors_result
```

### Comparing `periodparser-1.0.2/src/periodparser/text_parser.py` & `periodparser-1.0.3/src/periodparser/text_parser.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/utils/helpers.py` & `periodparser-1.0.3/src/periodparser/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/utils/parser_extractors.py` & `periodparser-1.0.3/src/periodparser/utils/parser_extractors.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/src/periodparser/utils/parser_utils.py` & `periodparser-1.0.3/src/periodparser/utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `periodparser-1.0.2/PKG-INFO` & `periodparser-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodparser
-Version: 1.0.2
+Version: 1.0.3
 Summary: python parser for human readable period dates
 Home-page: https://github.com/fennr/periodparser
 Author: fenn_r
 Author-email: fenrir1121@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -34,11 +34,11 @@
 Библиотека для парсинга дат и времени в естественной речи на русском языке.
 
 ## Пример
 
 ```python
 import periodparser as pp
 
-result = pp.exctract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
+result = pp.extract('Техобслуживание пройдет с вечера следующей среды до пол 9 утра')
 print(result.dates[
           0])  # [Type=DateTimeTokenType.PERIOD, From=2023-06-28T17:00:00, To=2023-06-29T08:30:00, Span=None, HasTime=True, StartIndex=24, EndIndex=62]
 ```
```

