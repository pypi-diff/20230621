# Comparing `tmp/citation_docket-0.1.4.tar.gz` & `tmp/citation_docket-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_docket-0.1.4.tar", max compression
+gzip compressed data, was "citation_docket-0.1.5.tar", max compression
```

## Comparing `citation_docket-0.1.4.tar` & `citation_docket-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:24:36.706225 citation_docket-0.1.4/LICENSE
--rw-r--r--   0        0        0      765 2023-06-21 16:51:59.539672 citation_docket-0.1.4/citation_docket/__init__.py
--rw-r--r--   0        0        0     2657 2023-06-21 16:50:14.915233 citation_docket-0.1.4/citation_docket/main.py
--rw-r--r--   0        0        0     1015 2023-06-21 16:31:23.228996 citation_docket-0.1.4/citation_docket/regexes/__init__.py
--rw-r--r--   0        0        0     3227 2023-06-21 15:55:09.436575 citation_docket-0.1.4/citation_docket/regexes/constructed_ac.py
--rw-r--r--   0        0        0     3268 2023-06-21 15:56:18.843853 citation_docket-0.1.4/citation_docket/regexes/constructed_am.py
--rw-r--r--   0        0        0     2520 2023-06-21 15:57:44.929109 citation_docket-0.1.4/citation_docket/regexes/constructed_bm.py
--rw-r--r--   0        0        0     2962 2023-06-21 15:59:25.169084 citation_docket-0.1.4/citation_docket/regexes/constructed_gr.py
--rw-r--r--   0        0        0     2173 2023-06-21 16:28:57.847377 citation_docket-0.1.4/citation_docket/regexes/constructed_jib.py
--rw-r--r--   0        0        0     2473 2023-06-21 16:03:45.556847 citation_docket-0.1.4/citation_docket/regexes/constructed_oca.py
--rw-r--r--   0        0        0     1683 2023-06-21 16:04:34.509830 citation_docket-0.1.4/citation_docket/regexes/constructed_pet.py
--rw-r--r--   0        0        0     1832 2023-06-21 16:30:20.655709 citation_docket-0.1.4/citation_docket/regexes/constructed_udk.py
--rw-r--r--   0        0        0      318 2023-06-21 15:24:10.209775 citation_docket-0.1.4/citation_docket/regexes/models/__init__.py
--rw-r--r--   0        0        0     4864 2023-06-21 16:32:36.479915 citation_docket-0.1.4/citation_docket/regexes/models/constructor.py
--rw-r--r--   0        0        0     1335 2023-06-21 16:18:04.452929 citation_docket-0.1.4/citation_docket/regexes/models/docket_category.py
--rw-r--r--   0        0        0      806 2023-06-21 15:24:10.210056 citation_docket-0.1.4/citation_docket/regexes/models/docket_citation.py
--rw-r--r--   0        0        0     3553 2023-06-21 16:03:10.920090 citation_docket-0.1.4/citation_docket/regexes/models/docket_model.py
--rw-r--r--   0        0        0     2911 2023-06-21 15:24:10.210259 citation_docket-0.1.4/citation_docket/regexes/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-21 15:27:47.288680 citation_docket-0.1.4/citation_docket/regexes/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-21 15:24:10.210504 citation_docket-0.1.4/citation_docket/regexes/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-21 15:24:10.210588 citation_docket-0.1.4/citation_docket/regexes/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-21 15:24:10.210659 citation_docket-0.1.4/citation_docket/regexes/models/misc/x.py
--rw-r--r--   0        0        0      189 2023-06-21 16:50:09.229278 citation_docket-0.1.4/citation_docket/utils/__init__.py
--rw-r--r--   0        0        0     2717 2023-06-21 16:51:04.316239 citation_docket-0.1.4/citation_docket/utils/sc_website_2023.py
--rw-r--r--   0        0        0     6997 2023-06-21 16:50:29.098899 citation_docket-0.1.4/citation_docket/utils/simple_matcher.py
--rw-r--r--   0        0        0      489 2023-06-21 15:24:10.210955 citation_docket-0.1.4/citation_docket/utils/specials.py
--rw-r--r--   0        0        0     1354 2023-06-21 15:47:07.932002 citation_docket-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 citation_docket-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 16:53:42.975833 citation_docket-0.1.5/LICENSE
+-rw-r--r--   0        0        0      772 2023-06-21 17:31:08.172013 citation_docket-0.1.5/citation_docket/__init__.py
+-rw-r--r--   0        0        0     2671 2023-06-21 17:30:56.814252 citation_docket-0.1.5/citation_docket/main.py
+-rw-r--r--   0        0        0     1015 2023-06-21 16:53:42.976667 citation_docket-0.1.5/citation_docket/regexes/__init__.py
+-rw-r--r--   0        0        0     3227 2023-06-21 16:53:42.977054 citation_docket-0.1.5/citation_docket/regexes/constructed_ac.py
+-rw-r--r--   0        0        0     3268 2023-06-21 16:53:42.977569 citation_docket-0.1.5/citation_docket/regexes/constructed_am.py
+-rw-r--r--   0        0        0     2520 2023-06-21 16:53:42.977837 citation_docket-0.1.5/citation_docket/regexes/constructed_bm.py
+-rw-r--r--   0        0        0     2962 2023-06-21 16:53:42.978086 citation_docket-0.1.5/citation_docket/regexes/constructed_gr.py
+-rw-r--r--   0        0        0     2173 2023-06-21 16:53:42.978492 citation_docket-0.1.5/citation_docket/regexes/constructed_jib.py
+-rw-r--r--   0        0        0     2473 2023-06-21 16:53:42.978834 citation_docket-0.1.5/citation_docket/regexes/constructed_oca.py
+-rw-r--r--   0        0        0     1683 2023-06-21 16:53:42.979210 citation_docket-0.1.5/citation_docket/regexes/constructed_pet.py
+-rw-r--r--   0        0        0     1832 2023-06-21 16:53:42.979689 citation_docket-0.1.5/citation_docket/regexes/constructed_udk.py
+-rw-r--r--   0        0        0      318 2023-06-21 15:24:10.209775 citation_docket-0.1.5/citation_docket/regexes/models/__init__.py
+-rw-r--r--   0        0        0     4847 2023-06-21 17:32:34.395438 citation_docket-0.1.5/citation_docket/regexes/models/constructor.py
+-rw-r--r--   0        0        0     1335 2023-06-21 16:53:42.980603 citation_docket-0.1.5/citation_docket/regexes/models/docket_category.py
+-rw-r--r--   0        0        0      806 2023-06-21 15:24:10.210056 citation_docket-0.1.5/citation_docket/regexes/models/docket_citation.py
+-rw-r--r--   0        0        0     3591 2023-06-21 17:34:01.013037 citation_docket-0.1.5/citation_docket/regexes/models/docket_model.py
+-rw-r--r--   0        0        0     2911 2023-06-21 15:24:10.210259 citation_docket-0.1.5/citation_docket/regexes/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-21 16:53:42.981135 citation_docket-0.1.5/citation_docket/regexes/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-21 15:24:10.210504 citation_docket-0.1.5/citation_docket/regexes/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-21 15:24:10.210588 citation_docket-0.1.5/citation_docket/regexes/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-21 15:24:10.210659 citation_docket-0.1.5/citation_docket/regexes/models/misc/x.py
+-rw-r--r--   0        0        0      189 2023-06-21 16:53:42.981278 citation_docket-0.1.5/citation_docket/utils/__init__.py
+-rw-r--r--   0        0        0     2717 2023-06-21 16:53:42.981418 citation_docket-0.1.5/citation_docket/utils/sc_website_2023.py
+-rw-r--r--   0        0        0     6997 2023-06-21 16:53:42.981586 citation_docket-0.1.5/citation_docket/utils/simple_matcher.py
+-rw-r--r--   0        0        0      489 2023-06-21 16:53:42.981681 citation_docket-0.1.5/citation_docket/utils/specials.py
+-rw-r--r--   0        0        0     1354 2023-06-21 17:30:20.577343 citation_docket-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 citation_docket-0.1.5/PKG-INFO
```

### Comparing `citation_docket-0.1.4/LICENSE` & `citation_docket-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/__init__.py` & `citation_docket-0.1.5/citation_docket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .main import (
-    CITATIONS,
+    CITATION_OPTIONS,
     DocketReportCitationType,
     extract_docket_from_data,
     extract_dockets,
 )
 from .regexes import (
     DOCKET_DATE_FORMAT,
     CitationAC,
```

### Comparing `citation_docket-0.1.4/citation_docket/main.py` & `citation_docket-0.1.5/citation_docket/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,24 @@
     | CitationBM
     | CitationGR
     | CitationPET
     | CitationJIB
     | CitationUDK
 )  # noqa: E501
 
-CITATIONS = [
+CITATION_OPTIONS = (
     CitationAC,
     CitationAM,
     CitationOCA,
     CitationBM,
     CitationGR,
     CitationPET,
     CitationUDK,
     CitationJIB,
-]
+)
 
 
 def extract_dockets(raw: str) -> Iterator[DocketReportCitationType]:
     """Extract from `raw` text all raw citations which
     should include their `Docket` and `Report` component parts.
 
     Examples:
@@ -46,15 +46,15 @@
 
     Args:
         raw (str): Text to look for `Dockets` and `Reports`
 
     Yields:
         Iterator[DocketReportCitationType]: Any of custom `Docket` with `Report` types, e.g. `CitationAC`, etc.
     """  # noqa: E501
-    for citation in CITATIONS:
+    for citation in CITATION_OPTIONS:
         yield from citation.search(raw)
 
 
 def extract_docket_from_data(data: dict) -> DocketReportCitationType | None:
     """Return a DocketReportCitationType based on contents of a `data` dict.
 
     Examples:
```

### Comparing `citation_docket-0.1.4/citation_docket/regexes/__init__.py` & `citation_docket-0.1.5/citation_docket/regexes/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_ac.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_am.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_bm.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_gr.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_jib.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_oca.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_pet.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/constructed_udk.py` & `citation_docket-0.1.5/citation_docket/regexes/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/constructor.py` & `citation_docket-0.1.5/citation_docket/regexes/models/constructor.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
     label: str = Field(
         ...,
         title="Docket Label",
         description="e.g. General Register, Administrative Matter",
     )
     short_category: str = Field(
-        ...,
-        title="Docket Category Shorthand",
-        description="e.g. GR, AM",
+        ..., title="Docket Category Shorthand", description="e.g. GR, AM"
     )
     group_name: str = Field(
         ...,
         title="Regex Group Name",
         description=(
             "e.g. 'gr_test_phrase' identifies that portion of the"
             "Match object that should be associated with the label."
```

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/docket_category.py` & `citation_docket-0.1.5/citation_docket/regexes/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/docket_citation.py` & `citation_docket-0.1.5/citation_docket/regexes/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/docket_model.py` & `citation_docket-0.1.5/citation_docket/regexes/models/docket_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
         ...,
         title="Docket Date",
         description="Either in UK, US styles",
     )
 
     def __str__(self) -> str:
         if self.serial_text:
-            return f"{self.short_category} {self.serial_text}, {self.formatted_date}"
+            return (
+                f"{self.short_category.value} {self.serial_text}, {self.formatted_date}"
+            )
         return "No proper string detected."
 
     @property
     def serial_text(self) -> str:
         """From the raw `ids`, get the `cleaned_ids`, and of these `cleaned_ids`,
             extract the `@first_id` found to deal with compound ids, e.g.
             ids separated by 'and' and ','
```

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/gr_clean.py` & `citation_docket-0.1.5/citation_docket/regexes/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/misc/extra.py` & `citation_docket-0.1.5/citation_docket/regexes/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/regexes/models/misc/num.py` & `citation_docket-0.1.5/citation_docket/regexes/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/utils/sc_website_2023.py` & `citation_docket-0.1.5/citation_docket/utils/sc_website_2023.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/citation_docket/utils/simple_matcher.py` & `citation_docket-0.1.5/citation_docket/utils/simple_matcher.py`

 * *Files identical despite different names*

### Comparing `citation_docket-0.1.4/pyproject.toml` & `citation_docket-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_docket"
-version = "0.1.4"
+version = "0.1.5"
 description = "Regex formula of Philippine Supreme Court citations in docket format, i.e. GR, AM, AC, BM."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-docket"
 documentation = "https://justmars.github.io/citation-docket"
 classifiers = [
   "Topic :: Text Processing :: General",
```

### Comparing `citation_docket-0.1.4/PKG-INFO` & `citation_docket-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-docket
-Version: 0.1.4
+Version: 0.1.5
 Summary: Regex formula of Philippine Supreme Court citations in docket format, i.e. GR, AM, AC, BM.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

