# Comparing `tmp/citation_docket-0.1.3.tar.gz` & `tmp/citation_docket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_docket-0.1.3.tar", max compression
+gzip compressed data, was "citation_docket-0.1.4.tar", max compression
```

## Comparing `citation_docket-0.1.3.tar` & `citation_docket-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      681 2023-05-15 16:29:06.515132 citation_docket-0.1.3/citation_docket/__init__.py
--rw-r--r--   0        0        0     2428 2023-02-25 08:47:01.299013 citation_docket-0.1.3/citation_docket/main.py
--rw-r--r--   0        0        0      813 2023-02-25 08:31:23.194919 citation_docket-0.1.3/citation_docket/regexes/__init__.py
--rw-r--r--   0        0        0     3123 2023-02-25 08:29:02.278789 citation_docket-0.1.3/citation_docket/regexes/constructed_ac.py
--rw-r--r--   0        0        0     3164 2023-02-25 08:28:27.409030 citation_docket-0.1.3/citation_docket/regexes/constructed_am.py
--rw-r--r--   0        0        0     2485 2023-02-25 08:28:13.070495 citation_docket-0.1.3/citation_docket/regexes/constructed_bm.py
--rw-r--r--   0        0        0     2858 2023-02-25 08:28:39.943312 citation_docket-0.1.3/citation_docket/regexes/constructed_gr.py
--rw-r--r--   0        0        0     2436 2023-05-15 16:29:12.052715 citation_docket-0.1.3/citation_docket/regexes/constructed_oca.py
--rw-r--r--   0        0        0     1647 2023-02-25 08:31:23.194872 citation_docket-0.1.3/citation_docket/regexes/constructed_pet.py
--rw-r--r--   0        0        0      318 2023-01-22 05:43:38.806076 citation_docket-0.1.3/citation_docket/regexes/models/__init__.py
--rw-r--r--   0        0        0     4824 2023-02-25 08:00:22.655943 citation_docket-0.1.3/citation_docket/regexes/models/constructor.py
--rw-r--r--   0        0        0     1233 2023-02-25 06:10:48.723073 citation_docket-0.1.3/citation_docket/regexes/models/docket_category.py
--rw-r--r--   0        0        0      806 2023-01-23 14:56:36.287341 citation_docket-0.1.3/citation_docket/regexes/models/docket_citation.py
--rw-r--r--   0        0        0     3615 2023-02-25 06:04:26.946543 citation_docket-0.1.3/citation_docket/regexes/models/docket_model.py
--rw-r--r--   0        0        0     2911 2023-01-22 07:02:08.786981 citation_docket-0.1.3/citation_docket/regexes/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-02-25 07:24:24.112930 citation_docket-0.1.3/citation_docket/regexes/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2022-12-30 05:16:22.648456 citation_docket-0.1.3/citation_docket/regexes/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2022-12-30 05:27:34.939026 citation_docket-0.1.3/citation_docket/regexes/models/misc/num.py
--rw-r--r--   0        0        0      242 2022-11-20 04:25:09.137225 citation_docket-0.1.3/citation_docket/regexes/models/misc/x.py
--rw-r--r--   0        0        0     2607 2023-02-25 08:51:06.796290 citation_docket-0.1.3/citation_docket/sc_website_2023.py
--rw-r--r--   0        0        0     7002 2023-01-22 06:56:13.992705 citation_docket-0.1.3/citation_docket/simple_matcher.py
--rw-r--r--   0        0        0      489 2022-11-20 04:19:09.072188 citation_docket-0.1.3/citation_docket/specials.py
--rw-r--r--   0        0        0     1466 2023-05-15 16:27:39.511078 citation_docket-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 citation_docket-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:24:36.706225 citation_docket-0.1.4/LICENSE
+-rw-r--r--   0        0        0      765 2023-06-21 16:51:59.539672 citation_docket-0.1.4/citation_docket/__init__.py
+-rw-r--r--   0        0        0     2657 2023-06-21 16:50:14.915233 citation_docket-0.1.4/citation_docket/main.py
+-rw-r--r--   0        0        0     1015 2023-06-21 16:31:23.228996 citation_docket-0.1.4/citation_docket/regexes/__init__.py
+-rw-r--r--   0        0        0     3227 2023-06-21 15:55:09.436575 citation_docket-0.1.4/citation_docket/regexes/constructed_ac.py
+-rw-r--r--   0        0        0     3268 2023-06-21 15:56:18.843853 citation_docket-0.1.4/citation_docket/regexes/constructed_am.py
+-rw-r--r--   0        0        0     2520 2023-06-21 15:57:44.929109 citation_docket-0.1.4/citation_docket/regexes/constructed_bm.py
+-rw-r--r--   0        0        0     2962 2023-06-21 15:59:25.169084 citation_docket-0.1.4/citation_docket/regexes/constructed_gr.py
+-rw-r--r--   0        0        0     2173 2023-06-21 16:28:57.847377 citation_docket-0.1.4/citation_docket/regexes/constructed_jib.py
+-rw-r--r--   0        0        0     2473 2023-06-21 16:03:45.556847 citation_docket-0.1.4/citation_docket/regexes/constructed_oca.py
+-rw-r--r--   0        0        0     1683 2023-06-21 16:04:34.509830 citation_docket-0.1.4/citation_docket/regexes/constructed_pet.py
+-rw-r--r--   0        0        0     1832 2023-06-21 16:30:20.655709 citation_docket-0.1.4/citation_docket/regexes/constructed_udk.py
+-rw-r--r--   0        0        0      318 2023-06-21 15:24:10.209775 citation_docket-0.1.4/citation_docket/regexes/models/__init__.py
+-rw-r--r--   0        0        0     4864 2023-06-21 16:32:36.479915 citation_docket-0.1.4/citation_docket/regexes/models/constructor.py
+-rw-r--r--   0        0        0     1335 2023-06-21 16:18:04.452929 citation_docket-0.1.4/citation_docket/regexes/models/docket_category.py
+-rw-r--r--   0        0        0      806 2023-06-21 15:24:10.210056 citation_docket-0.1.4/citation_docket/regexes/models/docket_citation.py
+-rw-r--r--   0        0        0     3553 2023-06-21 16:03:10.920090 citation_docket-0.1.4/citation_docket/regexes/models/docket_model.py
+-rw-r--r--   0        0        0     2911 2023-06-21 15:24:10.210259 citation_docket-0.1.4/citation_docket/regexes/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-21 15:27:47.288680 citation_docket-0.1.4/citation_docket/regexes/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-21 15:24:10.210504 citation_docket-0.1.4/citation_docket/regexes/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-21 15:24:10.210588 citation_docket-0.1.4/citation_docket/regexes/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-21 15:24:10.210659 citation_docket-0.1.4/citation_docket/regexes/models/misc/x.py
+-rw-r--r--   0        0        0      189 2023-06-21 16:50:09.229278 citation_docket-0.1.4/citation_docket/utils/__init__.py
+-rw-r--r--   0        0        0     2717 2023-06-21 16:51:04.316239 citation_docket-0.1.4/citation_docket/utils/sc_website_2023.py
+-rw-r--r--   0        0        0     6997 2023-06-21 16:50:29.098899 citation_docket-0.1.4/citation_docket/utils/simple_matcher.py
+-rw-r--r--   0        0        0      489 2023-06-21 15:24:10.210955 citation_docket-0.1.4/citation_docket/utils/specials.py
+-rw-r--r--   0        0        0     1354 2023-06-21 15:47:07.932002 citation_docket-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 citation_docket-0.1.4/PKG-INFO
```

### Comparing `citation_docket-0.1.3/citation_docket/__init__.py` & `citation_docket-0.1.4/citation_docket/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-__version__ = "0.1.3"
-from .sc_website_2023 import extract_docket_meta
 from .main import (
     CITATIONS,
     DocketReportCitationType,
     extract_docket_from_data,
     extract_dockets,
 )
 from .regexes import (
     DOCKET_DATE_FORMAT,
     CitationAC,
     CitationAM,
     CitationBM,
     CitationGR,
+    CitationJIB,
     CitationOCA,
     CitationPET,
+    CitationUDK,
     Docket,
     DocketCategory,
     Num,
     ShortDocketCategory,
     ac_key,
     ac_phrases,
     am_key,
     am_phrases,
     bm_key,
     bm_phrases,
-    oca_key,
-    oca_phrases,
-    pet_key,
-    pet_phrases,
     cull_extra,
     formerly,
     gr_key,
     gr_phrases,
+    jib_key,
+    jib_phrases,
     l_key,
+    oca_key,
+    oca_phrases,
+    pet_key,
+    pet_phrases,
     pp,
+    udk_key,
+    udk_phrases,
 )
-from .simple_matcher import is_docket, setup_docket_field
+from .utils.sc_website_2023 import extract_docket_meta
+from .utils.simple_matcher import is_docket, setup_docket_field
```

### Comparing `citation_docket-0.1.3/citation_docket/main.py` & `citation_docket-0.1.4/citation_docket/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 from collections.abc import Iterator
 
 from .regexes import (
     CitationAC,
     CitationAM,
     CitationBM,
     CitationGR,
+    CitationJIB,
     CitationOCA,
     CitationPET,
+    CitationUDK,
 )
-from .simple_matcher import setup_docket_field
+from .utils.simple_matcher import setup_docket_field
 
 DocketReportCitationType = (
     CitationAC
     | CitationAM
     | CitationOCA
     | CitationBM
     | CitationGR
     | CitationPET
+    | CitationJIB
+    | CitationUDK
 )  # noqa: E501
 
 CITATIONS = [
     CitationAC,
     CitationAM,
     CitationOCA,
     CitationBM,
     CitationGR,
     CitationPET,
+    CitationUDK,
+    CitationJIB,
 ]
 
 
-def extract_dockets(
-    raw: str,
-) -> Iterator[DocketReportCitationType]:
+def extract_dockets(raw: str) -> Iterator[DocketReportCitationType]:
     """Extract from `raw` text all raw citations which
     should include their `Docket` and `Report` component parts.
 
     Examples:
-        >>> next(extract_dockets("Bagong Alyansang Makabayan v. Zamora, G.R. Nos. 138570, 138572, 138587, 138680, 138698, October 10, 2000, 342 SCRA 449"))
-        CitationGR(publisher='SCRA', volume='342', page='449', volpubpage='342 SCRA 449', report_date=None, context='G.R. Nos. 138570, 138572, 138587, 138680, 138698', short_category='GR', category='General Register', ids='138570, 138572, 138587, 138680, 138698', docket_date=datetime.date(2000, 10, 10))
+        >>> cite = next(extract_dockets("Bagong Alyansang Makabayan v. Zamora, G.R. Nos. 138570, 138572, 138587, 138680, 138698, October 10, 2000, 342 SCRA 449"))
+        >>> cite.model_dump(exclude_none=True)
+        {'publisher': 'SCRA', 'volume': '342', 'page': '449', 'volpubpage': '342 SCRA 449', 'context': 'G.R. Nos. 138570, 138572, 138587, 138680, 138698', 'short_category': <ShortDocketCategory.GR: 'GR'>, 'category': <DocketCategory.GR: 'General Register'>, 'ids': '138570, 138572, 138587, 138680, 138698', 'docket_date': datetime.date(2000, 10, 10)}
 
     Args:
         raw (str): Text to look for `Dockets` and `Reports`
 
     Yields:
         Iterator[DocketReportCitationType]: Any of custom `Docket` with `Report` types, e.g. `CitationAC`, etc.
     """  # noqa: E501
     for citation in CITATIONS:
         yield from citation.search(raw)
 
 
 def extract_docket_from_data(data: dict) -> DocketReportCitationType | None:
-    """
-    Return a DocketReportCitationType based on contents of a `data` dict.
+    """Return a DocketReportCitationType based on contents of a `data` dict.
 
     Examples:
         >>> data = {"date_prom": "1985-04-24", "docket": "General Register L-63915, April 24, 1985", "orig_idx": "GR No. L-63915", "phil": "220 Phil. 422", "scra": "136 SCRA 27", "offg": None} # assume transformation from /details.yaml file
-        >>> extract_docket_from_data(data)
-        CitationGR(publisher=None, volume=None, page=None, volpubpage=None, report_date=None, context='G.R. No. L-63915', short_category='GR', category='General Register', ids='L-63915', docket_date=datetime.date(1985, 4, 24))
+        >>> cite = extract_docket_from_data(data)
+        >>> cite.model_dump(exclude_none=True)
+        {'context': 'G.R. No. L-63915', 'short_category': <ShortDocketCategory.GR: 'GR'>, 'category': <DocketCategory.GR: 'General Register'>, 'ids': 'L-63915', 'docket_date': datetime.date(1985, 4, 24)}
 
     Args:
         data (dict): Should contain relevant keys.
 
     Returns:
         DocketReportCitationType: Any of custom `Docket` with `Report` types, e.g. `CitationAC`
     """  # noqa: E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/__init__.py` & `citation_docket-0.1.4/citation_docket/regexes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,26 +19,38 @@
 from .constructed_gr import (
     CitationGR,
     constructed_gr,
     gr_key,
     gr_phrases,
     l_key,
 )
-from .constructed_pet import (
-    CitationPET,
-    constructed_pet,
-    pet_key,
-    pet_phrases,
+from .constructed_jib import (
+    CitationJIB,
+    constructed_jib,
+    jib_key,
+    jib_phrases,
 )
 from .constructed_oca import (
     CitationOCA,
     constructed_oca,
     oca_key,
     oca_phrases,
 )
+from .constructed_pet import (
+    CitationPET,
+    constructed_pet,
+    pet_key,
+    pet_phrases,
+)
+from .constructed_udk import (
+    CitationUDK,
+    constructed_udk,
+    udk_key,
+    udk_phrases,
+)
 from .models import (
     DOCKET_DATE_FORMAT,
     Constructor,
     Docket,
     DocketCategory,
     DocketReportCitation,
     Num,
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_ac.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_ac.py`

 * *Files 11% similar despite different names*

```diff
@@ -127,16 +127,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `AC` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "A.C. No. P-88-198, February 25, 1992, 206 SCRA 491."
-            >>> next(CitationAC.search(text))
-            CitationAC(publisher='SCRA', volume='206', page='491', volpubpage='206 SCRA 491', report_date=None, context='A.C. No. P-88-198', short_category='AC', category='Administrative Case', ids='P-88-198', docket_date=datetime.date(1992, 2, 25))
+            >>> cite = next(CitationAC.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'publisher': 'SCRA', 'volume': '206', 'page': '491', 'volpubpage': '206 SCRA 491', 'context': 'A.C. No. P-88-198', 'short_category': <ShortDocketCategory.AC: 'AC'>, 'category': <DocketCategory.AC: 'Administrative Case'>, 'ids': 'P-88-198', 'docket_date': datetime.date(1992, 2, 25)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_am.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_am.py`

 * *Files 22% similar despite different names*

```diff
@@ -153,16 +153,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `AM` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "A.M. No. P-88-198, February 25, 1992, 206 SCRA 491."
-            >>> next(CitationAM.search(text))
-            CitationAM(publisher='SCRA', volume='206', page='491', volpubpage='206 SCRA 491', report_date=None, context='A.M. No. P-88-198', short_category='AM', category='Administrative Matter', ids='P-88-198', docket_date=datetime.date(1992, 2, 25))
+            >>> cite = next(CitationAM.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'publisher': 'SCRA', 'volume': '206', 'page': '491', 'volpubpage': '206 SCRA 491', 'context': 'A.M. No. P-88-198', 'short_category': <ShortDocketCategory.AM: 'AM'>, 'category': <DocketCategory.AM: 'Administrative Matter'>, 'ids': 'P-88-198', 'docket_date': datetime.date(1992, 2, 25)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_bm.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_bm.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,16 +110,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `BM` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "B.M. No. 1678, December 17, 2007"
-            >>> next(CitationBM.search(text))
-            CitationBM(publisher=None, volume=None, page=None, volpubpage=None, report_date=None, context='B.M. No. 1678', short_category='BM', category='Bar Matter', ids='1678', docket_date=datetime.date(2007, 12, 17))
+            >>> cite = next(CitationBM.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'context': 'B.M. No. 1678', 'short_category': <ShortDocketCategory.BM: 'BM'>, 'category': <DocketCategory.BM: 'Bar Matter'>, 'ids': '1678', 'docket_date': datetime.date(2007, 12, 17)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_gr.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_gr.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `GR` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "Bagong Alyansang Makabayan v. Zamora, G.R. Nos. 138570, 138572, 138587, 138680, 138698, October 10, 2000, 342 SCRA 449"
-            >>> next(CitationGR.search(text))
-            CitationGR(publisher='SCRA', volume='342', page='449', volpubpage='342 SCRA 449', report_date=None, context='G.R. Nos. 138570, 138572, 138587, 138680, 138698', short_category='GR', category='General Register', ids='138570, 138572, 138587, 138680, 138698', docket_date=datetime.date(2000, 10, 10))
+            >>> cite = next(CitationGR.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'publisher': 'SCRA', 'volume': '342', 'page': '449', 'volpubpage': '342 SCRA 449', 'context': 'G.R. Nos. 138570, 138572, 138587, 138680, 138698', 'short_category': <ShortDocketCategory.GR: 'GR'>, 'category': <DocketCategory.GR: 'General Register'>, 'ids': '138570, 138572, 138587, 138680, 138698', 'docket_date': datetime.date(2000, 10, 10)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_oca.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_oca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Self
 from collections.abc import Iterator
+from typing import Self
+
 from .models import Constructor, DocketCategory, DocketReportCitation
 from .models.misc import NUMBER_KEYWORD
 
 separator = r"[\.\s]*"
 digit = r"(\d{2}|P)[\d-]*"  # e.g. 323-23, 343-34
 
 end_digit = r"""
@@ -77,16 +78,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `OCA` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "AM OCA IPI No. P-07-2403, Feb. 06, 2008"
-            >>> next(CitationOCA.search(text))
-            CitationOCA(publisher=None, volume=None, page=None, volpubpage=None, report_date=None, context='AM OCA IPI No. P-07-2403', short_category='OCA', category='Office of the Court Administrator', ids='P-07-2403', docket_date=datetime.date(2008, 2, 6))
+            >>> cite = next(CitationOCA.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'context': 'AM OCA IPI No. P-07-2403', 'short_category': <ShortDocketCategory.OCA: 'OCA'>, 'category': <DocketCategory.OCA: 'Office of the Court Administrator'>, 'ids': 'P-07-2403', 'docket_date': datetime.date(2008, 2, 6)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/constructed_pet.py` & `citation_docket-0.1.4/citation_docket/regexes/constructed_pet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Self
 from collections.abc import Iterator
+from typing import Self
+
 from .models import Constructor, DocketCategory, DocketReportCitation
 from .models.misc import NUMBER_KEYWORD
 
-
 pet_key = rf"""
     (
         P
         [\.\s]*
         E
         [\.\s]*
         T
@@ -52,16 +52,17 @@
 
     @classmethod
     def search(cls, text: str) -> Iterator[Self]:
         """Get all dockets matching the `PET` docket pattern, inclusive of their optional Report object.
 
         Examples:
             >>> text = "P.E.T. Case No. 001, February 13, 1996"
-            >>> next(CitationPET.search(text))
-            CitationPET(publisher=None, volume=None, page=None, volpubpage=None, report_date=None, context='P.E.T. Case No. 001', short_category='PET', category='Presidential Electoral Tribunal', ids='001', docket_date=datetime.date(1996, 2, 13))
+            >>> cite = next(CitationPET.search(text))
+            >>> cite.model_dump(exclude_none=True)
+            {'context': 'P.E.T. Case No. 001', 'short_category': <ShortDocketCategory.PET: 'PET'>, 'category': <DocketCategory.PET: 'Presidential Electoral Tribunal'>, 'ids': '001', 'docket_date': datetime.date(1996, 2, 13)}
 
         Args:
             text (str): Text to look for citation objects
 
         Yields:
             Iterator[Self]: Combination of Docket and Report pydantic model.
         """  # noqa E501
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/constructor.py` & `citation_docket-0.1.4/citation_docket/regexes/models/constructor.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     1. General Register
     2. Administrative Matter
     3. Administrative Case
     4. Bar Matter
     5. Office of the Court Administrator
     6. Presidential Electoral Tribunal
+    7. Judicial Integrity Board
+    8. Undocketed Case
 
     The Constructor formalizes the assigned group names into
     their respective fields.
 
     Relatedly, it takes advantage of
     the `citation_date` and the `citation_report` libraries in
     generating the main `@pattern` since the regex strings above
@@ -57,16 +59,15 @@
         title="Regex Initial Group Name",
         description="e.g. gr_mid, am_init; see .regexes for other group names",
     )
     docket_regex: str = Field(
         ...,
         title="Regex Expression Proper",
         description=(
-            "The full regex expression which includes the group"
-            "names referred to above."
+            "The full regex expression which includes the groupnames referred to above."
         ),
     )
     key_regex: str = Field(
         ...,
         title="Regex Key",
         description="Regex portion to get the serial ids",
     )
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/docket_category.py` & `citation_docket-0.1.4/citation_docket/regexes/models/docket_category.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,39 +9,38 @@
     :--|:--
     `GR` | General Register
     `AM` | Administrative Matter
     `AC` | Administrative Case
     `BM` | Bar Matter
     `PET` | Presidential Electoral Tribunal
     `OCA` | Office of the Court Administrator
+    `JIB` | Judicial Integrity Board
+    `UDK` | Undocketed
 
     Complication: These categories do not always represent decisions. For instance,
     there are are `AM` and `BM` docket numbers that represent rules rather
     than decisions.
     """
 
     GR = "General Register"
     AM = "Administrative Matter"
     AC = "Administrative Case"
     BM = "Bar Matter"
     PET = "Presidential Electoral Tribunal"
     OCA = "Office of the Court Administrator"
+    JIB = "Judicial Integrity Board"
+    UDK = "Undocketed"
 
 
 class ShortDocketCategory(str, Enum):
     """For purposes of creating an enumeration for use in `sqlpyd` wherein
     the value will be stored in the database.
-
-    Name | Value
-    :--|:--
-    `GR` | GR
-    `AM` | AM
-    `AC` | AC
-    `BM` | BM
     """
 
     GR = DocketCategory.GR.name
     AM = DocketCategory.AM.name
     AC = DocketCategory.AC.name
     BM = DocketCategory.BM.name
     PET = DocketCategory.PET.name
     OCA = DocketCategory.OCA.name
+    JIB = DocketCategory.JIB.name
+    UDK = DocketCategory.UDK.name
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/docket_citation.py` & `citation_docket-0.1.4/citation_docket/regexes/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/docket_model.py` & `citation_docket-0.1.4/citation_docket/regexes/models/docket_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date
 
 from citation_date import DOCKET_DATE_FORMAT
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .docket_category import DocketCategory, ShortDocketCategory
 from .gr_clean import gr_prefix_clean
 
 
 class Docket(BaseModel):
     """
@@ -27,56 +27,49 @@
     _A.M. RTJ-12-2317 (Formerly OCA I.P.I. No. 10-3378-RTJ), Jan 1, 2000_ | AM | RTJ-12-2317 |Jan 1, 2000
     _A.C. No. 10179 (Formerly CBD 11-2985), March 04, 2014_ | AC | 10179 | Mar. 4, 2014
 
     The Docket is often paired with a Report, which is the traditional
     identifier based on volume and page numbers.
     """  # noqa: E501
 
+    model_config = ConfigDict(use_enum_values=True)
     context: str = Field(
         ...,
         title="Context",
         description="Full texted matched by the regex pattern.",
     )
     short_category: ShortDocketCategory = Field(
         ...,
         title="Docket Acronym",
         description="GR, AM, AC, BM, etc.",
         min_length=2,
-        max_length=3,
+        max_length=4,
     )
     category: DocketCategory = Field(
         ...,
         title="Docket Category",
         description=(
             "e.g. General Register, Administrative Matter,"
             " Administrative Case, Bar Matter"
         ),
     )
     ids: str = Field(
         ...,
         title="Raw Docket IDs",
-        description=(
-            "The docket can contain multiple tokens, e.g. 24141, 14234, 2342."
-        ),
+        description="The docket can contain multiple tokens, e.g. 24141, 14234, 2342.",
     )
     docket_date: date = Field(
         ...,
         title="Docket Date",
         description="Either in UK, US styles",
     )
 
-    class Config:
-        use_enum_values = True
-
     def __str__(self) -> str:
         if self.serial_text:
-            return (
-                f"{self.short_category} {self.serial_text},"
-                f" {self.formatted_date}"
-            )
+            return f"{self.short_category} {self.serial_text}, {self.formatted_date}"
         return "No proper string detected."
 
     @property
     def serial_text(self) -> str:
         """From the raw `ids`, get the `cleaned_ids`, and of these `cleaned_ids`,
             extract the `@first_id` found to deal with compound ids, e.g.
             ids separated by 'and' and ','
```

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/gr_clean.py` & `citation_docket-0.1.4/citation_docket/regexes/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/misc/extra.py` & `citation_docket-0.1.4/citation_docket/regexes/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.3/citation_docket/regexes/models/misc/num.py` & `citation_docket-0.1.4/citation_docket/regexes/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.3/citation_docket/sc_website_2023.py` & `citation_docket-0.1.4/citation_docket/utils/sc_website_2023.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dateutil.parser import parse
-from typing import Any
 import re
-from .main import extract_dockets
+from typing import Any
+
+from dateutil.parser import parse
 
 DOCKET_PATTERN = re.compile(
     r"""
     (?P<docket>.*?)
     \.
     \s+
     (?P<decision_date>[A-Z]\w+\s\d+,\s\d{4})
@@ -23,24 +23,26 @@
 
 
 def extract_docket_meta(text: str) -> dict[str, Any] | None:
     """Metadata involving the docket.
 
     Examples:
         >>> extract_docket_meta("G.R. No. 234179. December 5, 2022 [Date Uploaded: 01/26/2023]")
-        {'docket': 'G.R. No. 234179', 'decision_date': datetime.date(2022, 12, 5), 'upload_date': '01/26/2023', 'context': 'G.R. No. 234179', 'short_category': 'GR', 'category': 'General Register', 'ids': '234179', 'docket_date': datetime.date(2022, 12, 5)}
+        {'docket': 'G.R. No. 234179', 'decision_date': datetime.date(2022, 12, 5), 'upload_date': '01/26/2023', 'context': 'G.R. No. 234179', 'short_category': <ShortDocketCategory.GR: 'GR'>, 'category': <DocketCategory.GR: 'General Register'>, 'ids': '234179', 'docket_date': datetime.date(2022, 12, 5)}
         >>> extract_docket_meta("G.R. No. 180350/G.R. No. 205186/G.R. No. 222919/G.R. No. 223237. July 6, 2022 [Date Uploaded: 09/21/2022]")
-        {'docket': 'G.R. No. 180350/G.R. No. 205186/G.R. No. 222919/G.R. No. 223237', 'decision_date': datetime.date(2022, 7, 6), 'upload_date': '09/21/2022', 'context': 'G.R. No. 180350/G.R. No. 205186/G.R. No. 222919/G.R. No. 223237', 'short_category': 'GR', 'category': 'General Register', 'ids': '180350', 'docket_date': datetime.date(2022, 7, 6)}
+        {'docket': 'G.R. No. 180350/G.R. No. 205186/G.R. No. 222919/G.R. No. 223237', 'decision_date': datetime.date(2022, 7, 6), 'upload_date': '09/21/2022', 'context': 'G.R. No. 180350/G.R. No. 205186/G.R. No. 222919/G.R. No. 223237', 'short_category': <ShortDocketCategory.GR: 'GR'>, 'category': <DocketCategory.GR: 'General Register'>, 'ids': '180350', 'docket_date': datetime.date(2022, 7, 6)}
 
     Args:
         text (str): Line from Supreme Court URL sub-title heading.
 
     Returns:
         dict[str, Any] | None: Docket-based details.
     """  # noqa: E501
+    from citation_docket import extract_dockets
+
     match = DOCKET_PATTERN.search(text)
     if not match:
         return None
     res = match.groupdict()
 
     if not res.get("docket"):
         return None
```

### Comparing `citation_docket-0.1.3/citation_docket/simple_matcher.py` & `citation_docket-0.1.4/citation_docket/utils/simple_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from collections.abc import Iterator
 from datetime import date
 from re import Match, Pattern
 from typing import NoReturn
 
 from dateutil.parser import parse
 
-from .regexes import DOCKET_DATE_FORMAT, ShortDocketCategory
+from citation_docket.regexes import DOCKET_DATE_FORMAT, ShortDocketCategory
+
 from .specials import remove_prefix
 
 MAX_LENGTH_IDX = 100
 
 
 def parse_date_if_exists(text: str | None) -> date | None:
     "If the variable contains text with more than 5 characters, parse possible date."
@@ -72,15 +73,15 @@
         culled = raw.removeprefix(text_to_remove)
         separated = culled.split(",")
         return {"cat": simple_category, "idx": separated[0]}
     return None
 
 
 def updated_cat_idx(d: dict) -> dict:
-    from .regexes import ac_key, am_key, bm_key, formerly, gr_key
+    from ..regexes import ac_key, am_key, bm_key, formerly, gr_key
 
     def process_idx_further(text: str) -> str:
         pattern = re.compile(formerly, re.X)
         replaced = pattern.sub("", text)
         result = replaced.split()[0].strip()
         return result
 
@@ -98,17 +99,15 @@
             or get_cat_idx_from_orig(raw, "ac", ac_key)
             or get_cat_idx_from_orig(raw, "bm", bm_key)
             or get_cat_idx_from_orig(raw, "gr", gr_key)
         )
 
     def source_simple(raw: str) -> dict | None:
         idx = " ".join(i for i in raw.split() if re.search(r"\d+|&|(and)", i))
-        text = " ".join(
-            i for i in raw.split() if not re.search(r"\d+|&|(and)", i)
-        )
+        text = " ".join(i for i in raw.split() if not re.search(r"\d+|&|(and)", i))
         if not (cat := simple_two_letter_docket_category(text)):
             return None
 
         return {"cat": cat, "idx": idx}
 
     if d.get("orig_idx", None):
         text = d["orig_idx"]
```

