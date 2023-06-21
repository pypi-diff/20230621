# Comparing `tmp/findmyorder-1.4.4.tar.gz` & `tmp/findmyorder-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.4.4.tar", max compression
+gzip compressed data, was "findmyorder-1.4.5.tar", max compression
```

## Comparing `findmyorder-1.4.4.tar` & `findmyorder-1.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-15 19:53:36.577196 findmyorder-1.4.4/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-15 19:53:36.577196 findmyorder-1.4.4/README.md
--rw-r--r--   0        0        0      113 2023-06-15 19:53:52.793015 findmyorder-1.4.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-06-15 19:53:36.577196 findmyorder-1.4.4/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-15 19:53:36.577196 findmyorder-1.4.4/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-15 19:53:36.577196 findmyorder-1.4.4/findmyorder/main.py
--rw-r--r--   0        0        0     1745 2023-06-15 19:53:52.793015 findmyorder-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-21 14:12:20.552563 findmyorder-1.4.5/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-21 14:12:20.552563 findmyorder-1.4.5/README.md
+-rw-r--r--   0        0        0      113 2023-06-21 14:12:39.836780 findmyorder-1.4.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/config.py
+-rw-r--r--   0        0        0     2265 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-21 14:12:20.552563 findmyorder-1.4.5/findmyorder/main.py
+-rw-r--r--   0        0        0     1921 2023-06-21 14:12:39.836780 findmyorder-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.5/PKG-INFO
```

### Comparing `findmyorder-1.4.4/LICENSE` & `findmyorder-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.4/README.md` & `findmyorder-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.4/findmyorder/config.py` & `findmyorder-1.4.5/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.4/findmyorder/default_settings.toml` & `findmyorder-1.4.5/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.4/findmyorder/main.py` & `findmyorder-1.4.5/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.4/pyproject.toml` & `findmyorder-1.4.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.4.4"
+version = "1.4.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -16,15 +16,15 @@
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 pyparsing = "^3.0.9"
-emoji = "^2.4.0"
+emoji = "^2.5.1"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "7.0.1"
 furo = "2023.5.20"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
@@ -56,10 +56,11 @@
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
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
+patch_emoji = "fix,Update,🎨,:art:,🐛,:bug:,🚑,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️|:arrow_up:,🩹,👷,📝,🔒,:lock:,👽,:alien:,💬,🥅,✅,:white_check_mark:,🐳,🙈,⚗️,🧐,🔇,🔊"
+
```

### Comparing `findmyorder-1.4.4/PKG-INFO` & `findmyorder-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.4.4
+Version: 1.4.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
-Requires-Dist: emoji (>=2.4.0,<3.0.0)
+Requires-Dist: emoji (>=2.5.1,<3.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order
```

