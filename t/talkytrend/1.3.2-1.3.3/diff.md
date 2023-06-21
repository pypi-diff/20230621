# Comparing `tmp/talkytrend-1.3.2.tar.gz` & `tmp/talkytrend-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.3.2.tar", max compression
+gzip compressed data, was "talkytrend-1.3.3.tar", max compression
```

## Comparing `talkytrend-1.3.2.tar` & `talkytrend-1.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-17 12:42:45.764912 talkytrend-1.3.2/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-17 12:42:45.764912 talkytrend-1.3.2/README.md
--rw-r--r--   0        0        0     1720 2023-06-17 12:43:03.493221 talkytrend-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-17 12:43:03.493221 talkytrend-1.3.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/config.py
--rw-r--r--   0        0        0      932 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6121 2023-06-17 12:42:45.764912 talkytrend-1.3.2/talkytrend/main.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-21 21:00:37.315259 talkytrend-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-21 21:00:37.315259 talkytrend-1.3.3/README.md
+-rw-r--r--   0        0        0     2178 2023-06-21 21:00:38.159267 talkytrend-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-21 21:00:38.159267 talkytrend-1.3.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-21 21:00:37.315259 talkytrend-1.3.3/talkytrend/config.py
+-rw-r--r--   0        0        0      932 2023-06-21 21:00:37.315259 talkytrend-1.3.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6121 2023-06-21 21:00:37.319259 talkytrend-1.3.3/talkytrend/main.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.3.3/PKG-INFO
```

### Comparing `talkytrend-1.3.2/LICENSE` & `talkytrend-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.2/README.md` & `talkytrend-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.2/pyproject.toml` & `talkytrend-1.3.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.3.2"
+version = "1.3.3"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -14,50 +14,55 @@
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/talkytrend/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/talkytrend/discussions"
 "Issues" =  "https://github.com/mraniki/talkytrend/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-asyncio = "*"
-dynaconf = "*"
-aiohttp = "*"
-tradingview_ta = "*"
-prettytable = "*"
+dynaconf = "^3.1.12"
+aiohttp = "^3.8.4"
+tradingview_ta = "^3.3.0"
+prettytable = "^3.8.0"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "*"
-pytest = "^7.0.0"
-pytest-cov = "*"
-pytest-asyncio = "*"
-pytest-mock = "*"
-coverage = "*"
+python-semantic-release = "^7.34.3"
+pytest = "^7.0"
+pytest-cov = "^4.1"
+pytest-asyncio = "^0.21.0"
+pytest-mock = "^3.11.1"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
 [tool.coverage.run]
 omit = [
     "tests/*",
     "examples/*",
+    "docs/*",
     "*/config.py"
 ]
 
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.1"
+sphinx-autoapi = "^2.1.0"
+furo = "^2023.5.20"
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","talkytrend/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-major_emoji = "💥"
-minor_emoji = "🥚,🚀,💄,✨"
-patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
+major_emoji = "BREAKING,💥,:boom:"
+minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
+patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
```

### Comparing `talkytrend-1.3.2/talkytrend/config.py` & `talkytrend-1.3.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.2/talkytrend/default_settings.toml` & `talkytrend-1.3.3/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.2/talkytrend/main.py` & `talkytrend-1.3.3/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.2/PKG-INFO` & `talkytrend-1.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.3.2
+Version: 1.3.3
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp
-Requires-Dist: asyncio
-Requires-Dist: dynaconf
-Requires-Dist: prettytable
-Requires-Dist: tradingview_ta
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: prettytable (>=3.8.0,<4.0.0)
+Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0)
 Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/talkytrend/issues
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 # TalkyTrend
```

