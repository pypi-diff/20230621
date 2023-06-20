# Comparing `tmp/sqscraper-0.3.2.tar.gz` & `tmp/sqscraper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.3.2.tar", last modified: Fri Jun 16 21:35:07 2023, max compression
+gzip compressed data, was "sqscraper-0.4.0.tar", last modified: Tue Jun 20 22:48:12 2023, max compression
```

## Comparing `sqscraper-0.3.2.tar` & `sqscraper-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.197934 sqscraper-0.3.2/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-16 21:35:07.197934 sqscraper-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.3.2/README.md
--rw-rw-rw-   0        0        0     1837 2023-06-16 21:32:57.000000 sqscraper-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 21:35:07.197934 sqscraper-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.154843 sqscraper-0.3.2/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.2/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.3.2/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.187941 sqscraper-0.3.2/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       49 2023-06-16 21:14:25.000000 sqscraper-0.3.2/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0    13195 2023-06-16 21:27:34.000000 sqscraper-0.3.2/sqscraper/cnbc/quote_page.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:07.187941 sqscraper-0.3.2/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      397 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 21:35:07.000000 sqscraper-0.3.2/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.786126 sqscraper-0.4.0/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-20 22:48:12.786126 sqscraper-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.4.0/README.md
+-rw-rw-rw-   0        0        0     2197 2023-06-20 22:47:00.000000 sqscraper-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 22:48:12.786126 sqscraper-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.765165 sqscraper-0.4.0/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.0/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.0/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.786126 sqscraper-0.4.0/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0       84 2023-06-17 17:45:03.000000 sqscraper-0.4.0/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-18 02:02:54.000000 sqscraper-0.4.0/sqscraper/cnbc/_apps.py
+-rw-rw-rw-   0        0        0    13045 2023-06-20 18:44:13.000000 sqscraper-0.4.0/sqscraper/cnbc/quote_page.py
+-rw-rw-rw-   0        0        0    11780 2023-06-20 22:32:19.000000 sqscraper-0.4.0/sqscraper/cnbc/summary.py
+-rw-rw-rw-   0        0        0      592 2023-06-20 18:30:10.000000 sqscraper-0.4.0/sqscraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.775511 sqscraper-0.4.0/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      635 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.3.2/LICENSE` & `sqscraper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.3.2/PKG-INFO` & `sqscraper-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.2
+Version: 0.4.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqscraper-0.3.2/pyproject.toml` & `sqscraper-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.3.2"
+version = "0.4.0"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
@@ -23,25 +23,34 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development"
 ]
 requires-python = ">=3.6"
 dependencies = [
+    "beautifulsoup4==4.12.2",
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'",
+    "greenlet==2.0.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+    "html5lib==1.1",
     "idna==3.4 ; python_version >= '3.5'",
+    "lxml==4.9.2",
     "numpy==1.24.3",
     "pandas==2.0.2",
+    "playwright==1.35.0",
+    "pyee==9.0.4",
     "python-dateutil==2.8.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
     "pytz==2023.3",
     "requests==2.31.0",
     "six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+    "soupsieve==2.4.1 ; python_version >= '3.7'",
+    "typing-extensions==4.6.3 ; python_version >= '3.7'",
     "tzdata==2023.3 ; python_version >= '2'",
-    "urllib3==2.0.3 ; python_version >= '3.7'"
+    "urllib3==2.0.3 ; python_version >= '3.7'",
+    "webencodings==0.5.1"
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/SQScraper"
 
 [tool.setuptools.packages.find]
 where = ["."]
```

### Comparing `sqscraper-0.3.2/sqscraper/cnbc/quote_page.py` & `sqscraper-0.4.0/sqscraper/cnbc/quote_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 """
 """
 
 import datetime
-import decimal
 import math
-import re
 import typing
 
 import numpy as np
 import pandas as pd
 import requests
 
-
-def expand_value(value: str) -> int:
-    """
-    :param value:
-    :return:
-    """
-    powers = {"K": 3, "M": 6, "B": 9, "T": 12}
-    regex = re.compile(r"^(.*)([KMBT])$")
-
-    quantity, magnitude = regex.search(value).groups()
-    return int(decimal.Decimal(quantity) * 10 ** powers[magnitude])
+from sqscraper.utils import expand_value
+from sqscraper.utils import normalize_value
 
 
 class Quote:
     """
     :param data:
     """
     def __init__(self, data: typing.Dict[str, typing.Any]):
@@ -185,21 +174,21 @@
 
     @property
     def change_pct(self) -> float:
         """
         """
         if self["change_pct"] == "UNCH":
             return np.nan
-        return float(self["change_pct"].strip("%"))
+        return float(normalize_value(self["change_pct"]))
 
     @property
     def volume(self) -> int:
         """
         """
-        return int("".join(self["volume"].split(",")))
+        return int(normalize_value(self["volume"]))
 
 
 class ExtQuoteStrip(QuoteStrip):
     """
     :param data:
     """
     @property
@@ -226,49 +215,54 @@
     def series(self) -> pd.Series:
         """
         """
         raise NotImplementedError
 
     @staticmethod
     def quote_data(
-        method: typing.Callable[["QuotePageSection"], typing.Any]
-    ) -> typing.Callable[["QuotePageSection"], typing.Any]:
+        method: typing.Callable[["QuotePageSection"], typing.Union[int, float, datetime.datetime]]
+    ) -> typing.Callable[["QuotePageSection"], typing.Union[int, float, datetime.datetime]]:
         """
         :param method:
         :return:
         """
-        def wrapper(self: "QuotePageSection") -> typing.Any:
+        def wrapper(self: "QuotePageSection") -> typing.Union[int, float, datetime.datetime]:
             """
             :param self:
             :return:
             """
             try:
                 return method(self)
             except KeyError:
-                return None
+                return np.nan
         return wrapper
 
 
 class KeyStats(QuotePageSection):
     """
     """
     @property
     def series(self) -> pd.Series:
         """
         """
         data = {
-            "Open": self.open, "Day High": self.day_high, "Day Low": self.day_low,
+            "Open": self.open,
+            "Day High": self.day_high,
+            "Day Low": self.day_low,
             "Previous Close": self.prev_close,
             "10 Day Average Volume": self.ten_day_average_volume,
             "52 Week High": self.fiftytwo_week_high,
             "52 Week High Date": self.fiftytwo_week_high_date,
             "52 Week Low": self.fiftytwo_week_low,
             "52 Week Low Date": self.fiftytwo_week_low_date,
-            "Beta": self.beta, "Shares Out": self.shares_out, "Dividend": self.dividend,
-            "Dividend Yield (%)": self.dividend_yield, "YTD % Change": self.ytd_pct_change
+            "Beta": self.beta,
+            "Shares Out": self.shares_out,
+            "Dividend": self.dividend,
+            "Dividend Yield (%)": self.dividend_yield,
+            "YTD % Change": self.ytd_pct_change
         }
         return pd.Series(data, name="Key Stats")
 
     @property
     @QuotePageSection.quote_data
     def open(self) -> float:
         """
@@ -360,15 +354,15 @@
         return float(self["dividend"])
 
     @property
     @QuotePageSection.quote_data
     def dividend_yield(self) -> float:
         """
         """
-        return float("".join(self["dividendyield"].strip("%").split(",")))
+        return float(normalize_value(self["dividendyield"]))
 
     @property
     @QuotePageSection.quote_data
     def ytd_pct_change(self) -> float:
         """
         """
         return np.nan
@@ -418,43 +412,43 @@
         return expand_value(self["revenuettm"])
 
     @property
     @QuotePageSection.quote_data
     def roe(self) -> float:
         """
         """
-        return float("".join(self["ROETTEM"].strip("%").split(",")))
+        return float(normalize_value(self["ROETTEM"]))
 
     @property
     @QuotePageSection.quote_data
     def ebitda(self) -> int:
         """
         """
         return expand_value(self["TTMEBITD"])
 
     @property
     @QuotePageSection.quote_data
     def gross_margin(self) -> float:
         """
         """
-        return float("".join(self["GROSMGNTTM"].strip("%").split(",")))
+        return float(normalize_value(self["GROSMGNTTM"]))
 
     @property
     @QuotePageSection.quote_data
     def net_margin(self) -> float:
         """
         """
-        return float("".join(self["NETPROFTTM"].strip("%").split(",")))
+        return float(normalize_value(self["NETPROFTTM"]))
 
     @property
     @QuotePageSection.quote_data
     def debt_to_equity(self) -> float:
         """
         """
-        return float("".join(self["DEBTEQTYQ"].strip("%").split(",")))
+        return float(normalize_value(self["DEBTEQTYQ"]))
 
 
 class Events(QuotePageSection):
     """
     """
     @property
     def series(self) -> pd.Series:
```

### Comparing `sqscraper-0.3.2/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.4.0/sqscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.3.2
+Version: 0.4.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

