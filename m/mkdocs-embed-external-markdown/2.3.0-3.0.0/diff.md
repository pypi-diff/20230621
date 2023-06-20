# Comparing `tmp/mkdocs-embed-external-markdown-2.3.0.tar.gz` & `tmp/mkdocs-embed-external-markdown-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-embed-external-markdown-2.3.0.tar", max compression
+gzip compressed data, was "mkdocs-embed-external-markdown-3.0.0.tar", last modified: Tue Jun 20 22:48:37 2023, max compression
```

## Comparing `mkdocs-embed-external-markdown-2.3.0.tar` & `mkdocs-embed-external-markdown-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0     1088 2022-10-06 14:30:22.155242 mkdocs-embed-external-markdown-2.3.0/LICENSE.md
--rw-r--r--   0        0        0     6882 2022-10-06 14:30:22.155242 mkdocs-embed-external-markdown-2.3.0/README.md
--rw-r--r--   0        0        0     2953 2022-10-06 14:30:22.155242 mkdocs-embed-external-markdown-2.3.0/external_markdown/plugin.py
--rw-r--r--   0        0        0      910 2022-10-06 14:30:22.155242 mkdocs-embed-external-markdown-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 mkdocs-embed-external-markdown-2.3.0/setup.py
--rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 mkdocs-embed-external-markdown-2.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/external_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/external_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/external_markdown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/setup.cfg
```

### Comparing `mkdocs-embed-external-markdown-2.3.0/LICENSE.md` & `mkdocs-embed-external-markdown-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-embed-external-markdown-2.3.0/README.md` & `mkdocs-embed-external-markdown-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,24 +12,42 @@
 [license-url]: https://mit-license.org/
 
 ## About
 
 MkDocs Embed External Markdown plugin that allows to inject **section** or **full markdown** content from a given url.
 The goal is to embed different markdown from different sources inside your MkDocs project.
 
-## Version 2.xx
+## Version 3.xx
 
-**Braking change: Section name must include Markdown Section header like: `## Section name`**
+Version 3.0.0 (2023-06-20)
 
-Changelog:
+Added
 
-- [x] Add ability to import content from private github repositories. Thanks to @sd0408
-- [x] Added support for multi level sections such as `### Section name` and `#### Section name`
-- [x] Better Handling of parsing makrdowns wich contains `#` in the content
-- [x] Failing Mkdocs Build when Markdown content cannot be fetched
+- [x] Modularized the code into separate methods for improved readability and maintainability.
+- [x] Added type hints for better code understanding and possible performance improvements.
+- [x] Included regex pre-compilation for performance enhancement.
+- [x] Enhanced URL validation to check for the structure of a URL rather than just the presence of .md.
+- [x] Improved error logging through the use of logger.warning instead of print statements, which integrates with MkDocs' logging system.
+- [x] Added handling for relative links in the markdown, making them absolute based on the base URL.
+- [x] Introduced better error handling for Connection Errors and Status Codes through optional return types.
+
+Removed:
+
+- [x] Removed the use of sys.exit(1) on error, allowing the MkDocs build process to continue even if the plugin encounters an issue.
+- [x] Removed the strict requirement for a section level at the beginning of a section name.
+      Changed
+- [x] Switched from using re.compile for one-time regex patterns to using re.match or re.search.
+- [x] Extracted the GitHub token once at the beginning of the request method instead of multiple times.
+- [x] Replaced the check for .md at the end of the URL with a more comprehensive regular expression to validate the URL's structure.
+
+Fixed:
+
+- [x] Handling of section extraction is now more robust and less prone to errors.
+
+Please note that this is a major version update and may contain breaking changes. Carefully read the updated documentation and test the plugin thoroughly before upgrading in a production environment.
 
 ## Installation
 
 Install the package with pip:
 
 ```shell
 pip install mkdocs-embed-external-markdown
@@ -145,32 +163,23 @@
 ```
 
 {% endraw %}
 ````
 
 ## Known Issues
 
-- [ ] Embedding links without `.md` extension not working properly
+- [ ]
 
-## License
+## Version 2.xx Changelog Archive
+
+**Braking change: Section name must include Markdown Section header like: `## Section name`**
+
+Changelog:
 
-### MIT License
+- [x] Add ability to import content from private github repositories. Thanks to @sd0408
+- [x] Added support for multi level sections such as `### Section name` and `#### Section name`
+- [x] Better Handling of parsing makrdowns wich contains `#` in the content
+- [x] Failing Mkdocs Build when Markdown content cannot be fetched
 
-Copyright© 3os.org @ 2022
+## License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+This project is licensed under the terms of the [MIT License](LICENSE.md).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mkdocs-embed-external-markdown-2.3.0/PKG-INFO` & `mkdocs-embed-external-markdown-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: mkdocs-embed-external-markdown
-Version: 2.3.0
+Version: 3.0.0
 Summary: Mkdocs plugin that allow to inject external markdown or markdown section from given url
-Home-page: https://3os.org/guides/markdown-cheatsheet/external-markdown/
+Author-email: Stas Yakobov <dev@3os.org>
 License: MIT
+Project-URL: Source, https://github.com/fire1ce/pypi-test
 Keywords: mkdocs,plugin,markdown,external-markdown,embed,external,markdown-section
-Author: fire1ce
-Author-email: dev@3os.org
-Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Project-URL: Repository, https://github.com/fire1ce/mkdocs-embed-external-markdown
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # MkDocs Embed External Markdown Plugin
 
 [![PyPI - Downloads][pypi-image]][pypi-url]
 [![contributions welcome][contributions-image]][contributions-url]
 [![MIT license][license-image]][license-url]
 
@@ -33,24 +26,42 @@
 [license-url]: https://mit-license.org/
 
 ## About
 
 MkDocs Embed External Markdown plugin that allows to inject **section** or **full markdown** content from a given url.
 The goal is to embed different markdown from different sources inside your MkDocs project.
 
-## Version 2.xx
+## Version 3.xx
 
-**Braking change: Section name must include Markdown Section header like: `## Section name`**
+Version 3.0.0 (2023-06-20)
 
-Changelog:
+Added
 
-- [x] Add ability to import content from private github repositories. Thanks to @sd0408
-- [x] Added support for multi level sections such as `### Section name` and `#### Section name`
-- [x] Better Handling of parsing makrdowns wich contains `#` in the content
-- [x] Failing Mkdocs Build when Markdown content cannot be fetched
+- [x] Modularized the code into separate methods for improved readability and maintainability.
+- [x] Added type hints for better code understanding and possible performance improvements.
+- [x] Included regex pre-compilation for performance enhancement.
+- [x] Enhanced URL validation to check for the structure of a URL rather than just the presence of .md.
+- [x] Improved error logging through the use of logger.warning instead of print statements, which integrates with MkDocs' logging system.
+- [x] Added handling for relative links in the markdown, making them absolute based on the base URL.
+- [x] Introduced better error handling for Connection Errors and Status Codes through optional return types.
+
+Removed:
+
+- [x] Removed the use of sys.exit(1) on error, allowing the MkDocs build process to continue even if the plugin encounters an issue.
+- [x] Removed the strict requirement for a section level at the beginning of a section name.
+      Changed
+- [x] Switched from using re.compile for one-time regex patterns to using re.match or re.search.
+- [x] Extracted the GitHub token once at the beginning of the request method instead of multiple times.
+- [x] Replaced the check for .md at the end of the URL with a more comprehensive regular expression to validate the URL's structure.
+
+Fixed:
+
+- [x] Handling of section extraction is now more robust and less prone to errors.
+
+Please note that this is a major version update and may contain breaking changes. Carefully read the updated documentation and test the plugin thoroughly before upgrading in a production environment.
 
 ## Installation
 
 Install the package with pip:
 
 ```shell
 pip install mkdocs-embed-external-markdown
@@ -166,33 +177,23 @@
 ```
 
 {% endraw %}
 ````
 
 ## Known Issues
 
-- [ ] Embedding links without `.md` extension not working properly
+- [ ]
 
-## License
+## Version 2.xx Changelog Archive
 
-### MIT License
+**Braking change: Section name must include Markdown Section header like: `## Section name`**
+
+Changelog:
 
-Copyright© 3os.org @ 2022
+- [x] Add ability to import content from private github repositories. Thanks to @sd0408
+- [x] Added support for multi level sections such as `### Section name` and `#### Section name`
+- [x] Better Handling of parsing makrdowns wich contains `#` in the content
+- [x] Failing Mkdocs Build when Markdown content cannot be fetched
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+## License
 
+This project is licensed under the terms of the [MIT License](LICENSE.md).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

