# Comparing `tmp/lamin_logger-0.6.2.tar.gz` & `tmp/lamin_logger-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.6.2.tar` & `lamin_logger-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.6.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.6.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.6.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.6.2/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.6.2/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.6.2/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.6.2/docs/api.md
--rw-r--r--   0        0        0     4152 2023-06-20 17:08:07.854751 lamin_logger-0.6.2/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.6.2/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.6.2/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.6.2/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-20 17:08:01.019139 lamin_logger-0.6.2/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.6.2/lamin_logger/_core.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.6.2/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.6.2/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     6568 2023-06-20 17:06:22.547794 lamin_logger-0.6.2/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.6.2/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.6.2/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.6.2/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.6.2/tests/test_base.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.6.2/tests/test_lookup.py
--rw-r--r--   0        0        0     5300 2023-06-19 17:49:41.484125 lamin_logger-0.6.2/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.6.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.6.2/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.0/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.0/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.0/docs/api.md
+-rw-r--r--   0        0        0     4306 2023-06-21 14:29:41.424448 lamin_logger-0.7.0/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.0/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.0/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-21 14:29:33.203168 lamin_logger-0.7.0/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.0/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3442 2023-06-21 14:28:14.948996 lamin_logger-0.7.0/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.0/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.0/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     6603 2023-06-21 14:28:14.949325 lamin_logger-0.7.0/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.0/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.0/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.0/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.0/tests/test_base.py
+-rw-r--r--   0        0        0     3437 2023-06-21 14:28:14.949583 lamin_logger-0.7.0/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.0/tests/test_lookup.py
+-rw-r--r--   0        0        0     5300 2023-06-19 17:49:41.484125 lamin_logger-0.7.0/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.0/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.0/PKG-INFO
```

### Comparing `lamin_logger-0.6.2/.github/workflows/build.yml` & `lamin_logger-0.7.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/.gitignore` & `lamin_logger-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/.pre-commit-config.yaml` & `lamin_logger-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/LICENSE` & `lamin_logger-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/docs/changelog.md` & `lamin_logger-0.7.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
 🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
 ✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
 🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
 💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
 ✨ Lookup can also return sql records | [22](https://github.com/laminlabs/lamin-logger/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.5.1
```

### Comparing `lamin_logger-0.6.2/docs/quickstart.ipynb` & `lamin_logger-0.7.0/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/lamin_logger/_core.py` & `lamin_logger-0.7.0/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/lamin_logger/_logger.py` & `lamin_logger-0.7.0/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/lamin_logger/_lookup.py` & `lamin_logger-0.7.0/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.0/lamin_logger/_map_synonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     return_mapper: bool = False,
     synonyms_field: str = "synonyms",
     sep: str = "|",
     keep: Literal["first", "last", False] = "first",
 ) -> Union[Dict[str, str], List[str]]:
     """Maps input identifiers against a concatenated synonyms column.
 
+    Will also standardize casing.
+
     Args:
         df: Reference DataFrame.
         identifiers: Identifiers that will be mapped against a field.
         return_mapper: If True, returns {input synonyms : standardized field name}.
         case_sensitive: Whether the mapping is case sensitive.
         keep : {'first', 'last', False}, default 'first'
             When a synonym maps to multiple standardized values, determines
```

### Comparing `lamin_logger-0.6.2/lamin_logger/_python_version.py` & `lamin_logger-0.7.0/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/lamin_logger/_search.py` & `lamin_logger-0.7.0/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/pyproject.toml` & `lamin_logger-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/tests/test_lookup.py` & `lamin_logger-0.7.0/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/tests/test_map_synonyms.py` & `lamin_logger-0.7.0/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/tests/test_search.py` & `lamin_logger-0.7.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.2/PKG-INFO` & `lamin_logger-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.6.2
+Version: 0.7.0
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

