# Comparing `tmp/mkdocs-embed-external-markdown-3.0.0.tar.gz` & `tmp/mkdocs-embed-external-markdown-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-embed-external-markdown-3.0.0.tar", last modified: Tue Jun 20 22:48:37 2023, max compression
+gzip compressed data, was "mkdocs-embed-external-markdown-3.0.1.tar", last modified: Wed Jun 21 00:02:57 2023, max compression
```

## Comparing `mkdocs-embed-external-markdown-3.0.0.tar` & `mkdocs-embed-external-markdown-3.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/external_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/external_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/external_markdown/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 22:48:37.000000 mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-20 22:48:20.000000 mkdocs-embed-external-markdown-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:48:37.209379 mkdocs-embed-external-markdown-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:02:57.728361 mkdocs-embed-external-markdown-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-21 00:02:39.000000 mkdocs-embed-external-markdown-3.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-21 00:02:57.728361 mkdocs-embed-external-markdown-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-21 00:02:39.000000 mkdocs-embed-external-markdown-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:02:57.728361 mkdocs-embed-external-markdown-3.0.1/external_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:02:39.000000 mkdocs-embed-external-markdown-3.0.1/external_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-21 00:02:39.000000 mkdocs-embed-external-markdown-3.0.1/external_markdown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:02:57.728361 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 00:02:57.000000 mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 00:02:39.000000 mkdocs-embed-external-markdown-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:02:57.728361 mkdocs-embed-external-markdown-3.0.1/setup.cfg
```

### Comparing `mkdocs-embed-external-markdown-3.0.0/LICENSE.md` & `mkdocs-embed-external-markdown-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-embed-external-markdown-3.0.0/PKG-INFO` & `mkdocs-embed-external-markdown-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-embed-external-markdown
-Version: 3.0.0
+Version: 3.0.1
 Summary: Mkdocs plugin that allow to inject external markdown or markdown section from given url
 Author-email: Stas Yakobov <dev@3os.org>
 License: MIT
 Project-URL: Source, https://github.com/fire1ce/pypi-test
 Keywords: mkdocs,plugin,markdown,external-markdown,embed,external,markdown-section
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -28,14 +28,20 @@
 ## About
 
 MkDocs Embed External Markdown plugin that allows to inject **section** or **full markdown** content from a given url.
 The goal is to embed different markdown from different sources inside your MkDocs project.
 
 ## Version 3.xx
 
+Version 3.0.1 (2023-06-21)
+
+Fixed:
+
+- [x] Crash caused by conflict with Jinja2 render engine expects `config` parameter from other 3rd party plugins.
+
 Version 3.0.0 (2023-06-20)
 
 Added
 
 - [x] Modularized the code into separate methods for improved readability and maintainability.
 - [x] Added type hints for better code understanding and possible performance improvements.
 - [x] Included regex pre-compilation for performance enhancement.
```

### Comparing `mkdocs-embed-external-markdown-3.0.0/README.md` & `mkdocs-embed-external-markdown-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 ## About
 
 MkDocs Embed External Markdown plugin that allows to inject **section** or **full markdown** content from a given url.
 The goal is to embed different markdown from different sources inside your MkDocs project.
 
 ## Version 3.xx
 
+Version 3.0.1 (2023-06-21)
+
+Fixed:
+
+- [x] Crash caused by conflict with Jinja2 render engine expects `config` parameter from other 3rd party plugins.
+
 Version 3.0.0 (2023-06-20)
 
 Added
 
 - [x] Modularized the code into separate methods for improved readability and maintainability.
 - [x] Added type hints for better code understanding and possible performance improvements.
 - [x] Included regex pre-compilation for performance enhancement.
```

### Comparing `mkdocs-embed-external-markdown-3.0.0/external_markdown/plugin.py` & `mkdocs-embed-external-markdown-3.0.1/external_markdown/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,12 +134,12 @@
             if section_level is not None:
                 markdown = self.extract_section_from_markdown(markdown, section_name, section_level, url) or ""
             else:
                 markdown = ""
 
         return markdown
 
-    def on_page_markdown(self, markdown: str, **kwargs) -> str:
+    def on_page_markdown(self, markdown: str, config, **kwargs) -> str:
         """
         Render the markdown content using the Jinja2 template engine.
         """
-        return Template(markdown).render(external_markdown=self.external_markdown)
+        return Template(markdown).render(external_markdown=self.external_markdown, config=config)
```

### Comparing `mkdocs-embed-external-markdown-3.0.0/mkdocs_embed_external_markdown.egg-info/PKG-INFO` & `mkdocs-embed-external-markdown-3.0.1/mkdocs_embed_external_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-embed-external-markdown
-Version: 3.0.0
+Version: 3.0.1
 Summary: Mkdocs plugin that allow to inject external markdown or markdown section from given url
 Author-email: Stas Yakobov <dev@3os.org>
 License: MIT
 Project-URL: Source, https://github.com/fire1ce/pypi-test
 Keywords: mkdocs,plugin,markdown,external-markdown,embed,external,markdown-section
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -28,14 +28,20 @@
 ## About
 
 MkDocs Embed External Markdown plugin that allows to inject **section** or **full markdown** content from a given url.
 The goal is to embed different markdown from different sources inside your MkDocs project.
 
 ## Version 3.xx
 
+Version 3.0.1 (2023-06-21)
+
+Fixed:
+
+- [x] Crash caused by conflict with Jinja2 render engine expects `config` parameter from other 3rd party plugins.
+
 Version 3.0.0 (2023-06-20)
 
 Added
 
 - [x] Modularized the code into separate methods for improved readability and maintainability.
 - [x] Added type hints for better code understanding and possible performance improvements.
 - [x] Included regex pre-compilation for performance enhancement.
```

### Comparing `mkdocs-embed-external-markdown-3.0.0/pyproject.toml` & `mkdocs-embed-external-markdown-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mkdocs-embed-external-markdown"
-version = "3.0.0"
+version = "3.0.1"
 description = "Mkdocs plugin that allow to inject external markdown or markdown section from given url"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{name = "Stas Yakobov", email = "dev@3os.org"}]
 license = {text = "MIT"}
 keywords = [
   "mkdocs",
   "plugin",
```

