# Comparing `tmp/citation_report-0.1.3.tar.gz` & `tmp/citation_report-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_report-0.1.3.tar", max compression
+gzip compressed data, was "citation_report-0.1.4.tar", max compression
```

## Comparing `citation_report-0.1.3.tar` & `citation_report-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      172 2023-05-15 16:22:47.952684 citation_report-0.1.3/citation_report/__init__.py
--rw-r--r--   0        0        0     6143 2023-01-23 14:31:25.452050 citation_report-0.1.3/citation_report/__main__.py
--rw-r--r--   0        0        0     1751 2023-01-24 04:28:16.713479 citation_report-0.1.3/citation_report/published_report.py
--rw-r--r--   0        0        0     3235 2023-01-23 14:30:33.463242 citation_report-0.1.3/citation_report/publisher.py
--rw-r--r--   0        0        0     1488 2023-05-15 16:23:08.412866 citation_report-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 citation_report-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:17:10.404107 citation_report-0.1.4/LICENSE
+-rw-r--r--   0        0        0      149 2023-06-21 15:20:34.271243 citation_report-0.1.4/citation_report/__init__.py
+-rw-r--r--   0        0        0     6097 2023-06-21 15:20:17.992985 citation_report-0.1.4/citation_report/__main__.py
+-rw-r--r--   0        0        0     1751 2023-06-21 15:17:00.053497 citation_report-0.1.4/citation_report/published_report.py
+-rw-r--r--   0        0        0     3233 2023-06-21 15:20:49.835556 citation_report-0.1.4/citation_report/publisher.py
+-rw-r--r--   0        0        0     1377 2023-06-21 15:19:04.186541 citation_report-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 citation_report-0.1.4/PKG-INFO
```

### Comparing `citation_report-0.1.3/citation_report/__main__.py` & `citation_report-0.1.4/citation_report/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,15 @@
     2. `@scra`
     3. `@offg`
     """
 
     publisher: str | None = Field(
         None,
         title="Report Publisher",
-        description=(
-            "Shorthand label of the publisher involved, e.g. SCRA, Phil. Offg"
-        ),
+        description="Shorthand label of the publisher involved, e.g. SCRA, Phil. Offg",
         max_length=5,
     )
     volume: str | None = Field(
         None,
         title="Volume Number",
         description=(
             "Publisher volume number - may not be a full digit since it can"
@@ -167,10 +165,8 @@
 
         Args:
             text (str): Text to search for report patterns
 
         Returns:
             list[str]: Unique report `volpubpage` strings found in the text
         """  # noqa: E501
-        return list(
-            {r.volpubpage for r in cls.extract_report(text) if r.volpubpage}
-        )
+        return list({r.volpubpage for r in cls.extract_report(text) if r.volpubpage})
```

### Comparing `citation_report-0.1.3/citation_report/published_report.py` & `citation_report-0.1.4/citation_report/published_report.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.3/citation_report/publisher.py` & `citation_report-0.1.4/citation_report/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     """Each publisher is represented by a regex expression `regex`.
     The `group_name` should be present in the `regex`.
     """
 
     label: str = Field(
         ...,
         title="Report style",
-        description="Use for uniformity",
+        description="Use for uniformity"
     )
     group_name: str = Field(
         ...,
         title="Regex group name",
-        description="Custom regex group that identifies the publisher",
+        description="Custom regex group that identifies the publisher"
     )
     regex: str = Field(
         ...,
         title="Regular expression",
         description=(
             "The regex expression that can be used to extract the various"
             " publisher styles, e.g. 'Phil.' or 'Phil. Report', 'SCRA' or"
```

### Comparing `citation_report-0.1.3/pyproject.toml` & `citation_report-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "citation-report"
-version = "0.1.3"
+version = "0.1.4"
 description = "Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG."
-authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
+authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-report"
 documentation = "https://justmars.github.io/citation-report"
 classifiers = [
   "Topic :: Text Processing :: General",
   "Programming Language :: Python :: 3.11",
@@ -15,50 +15,34 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = "^1.10.7"
-citation-date = "^0.1.4"
+citation-date = "^0.1.5"
+pydantic = ">=2.0b3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
-pre-commit = "^2.21"
-mkdocs = "^1.4.2"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.1"
+pre-commit = "^3.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.15"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
 testpaths = ["tests", "citation_report"]
 
 [tool.ruff]
-ignore = ["F401"]
-
-[tool.black]
-line-length = 79
-include = '.pyi?$'
-exclude = '''
-/(
-    .git
-    | .hg
-    | .mypy_cache
-    | .tox
-    | .venv
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
-'''
-
+ignore = ["F401", "F403"]
+fixable = ["F", "E", "W", "I001"]
+select = ["F", "E", "W", "I001"]
 
 [build-system]
 requires = ["poetry-core>=1.1.12"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `citation_report-0.1.3/PKG-INFO` & `citation_report-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: citation-report
-Version: 0.1.3
+Version: 0.1.4
 Summary: Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
-Author-email: mars@veloso.one
+Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation-date (>=0.1.4,<0.2.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: citation-date (>=0.1.5,<0.2.0)
+Requires-Dist: pydantic (>=2.0b3)
 Project-URL: Documentation, https://justmars.github.io/citation-report
 Project-URL: Repository, https://github.com/justmars/citation-report
```

