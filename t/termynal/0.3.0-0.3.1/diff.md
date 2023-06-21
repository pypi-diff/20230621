# Comparing `tmp/termynal-0.3.0.tar.gz` & `tmp/termynal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.3.0.tar", max compression
+gzip compressed data, was "termynal-0.3.1.tar", max compression
```

## Comparing `termynal-0.3.0.tar` & `termynal-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1092 2023-05-09 07:28:18.968331 termynal-0.3.0/LICENSE
--rw-r--r--   0        0        0      725 2023-05-09 07:28:18.968331 termynal-0.3.0/README.md
--rw-r--r--   0        0        0     2390 2023-05-09 07:28:18.968331 termynal-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     3251 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/plugin.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 termynal-0.3.0/setup.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 termynal-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-21 13:00:32.572570 termynal-0.3.1/LICENSE
+-rw-r--r--   0        0        0      725 2023-06-21 13:00:32.576570 termynal-0.3.1/README.md
+-rw-r--r--   0        0        0     2390 2023-06-21 13:00:32.576570 termynal-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     3355 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/plugin.py
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 termynal-0.3.1/setup.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 termynal-0.3.1/PKG-INFO
```

### Comparing `termynal-0.3.0/LICENSE` & `termynal-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.3.0/README.md` & `termynal-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.3.0/pyproject.toml` & `termynal-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0"
+version = "0.3.1"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
```

### Comparing `termynal-0.3.0/termynal/assets/termynal.css` & `termynal-0.3.1/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.3.0/termynal/assets/termynal.js` & `termynal-0.3.1/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.3.0/termynal/markdown.py` & `termynal-0.3.1/termynal/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import List
+from typing import Dict, List
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 
 class Termynal:
     progress_literal_start = "---&gt; 100%"
@@ -32,15 +32,15 @@
 
 
 class TermynalPreprocessor(Preprocessor):
     rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
     comment = "<!-- termynal -->"
     language_class = 'class="language-console"'
 
-    def run(self, lines):
+    def run(self, lines: List):
         content_by_placeholder = {}
         for i in range(self.md.htmlStash.html_counter):
             placeholder = self.md.htmlStash.get_placeholder(i)
             content = self.md.htmlStash.rawHtmlBlocks[i]
             content_by_placeholder[placeholder] = (content, i)
 
         lines_by_placeholder = self._get_lines(lines, content_by_placeholder)
@@ -51,22 +51,26 @@
             if line in lines_by_placeholder:
                 new_lines.extend(lines_by_placeholder[line])
 
         return new_lines
 
     def _get_lines(
         self,
-        lines,
-        content_by_placeholder,
+        lines: List,
+        content_by_placeholder: Dict,
     ):  # pylint:disable=too-many-nested-blocks
         lines_by_placeholder = {}
         is_termynal_code = False
         for line in lines:
             if line in content_by_placeholder:
                 (content, i) = content_by_placeholder[line]
+
+                if not isinstance(content, str):
+                    continue
+
                 if content.startswith(self.comment):
                     is_termynal_code = True
                     continue
 
                 matches = self.rexep.search(content)
                 if not matches:
                     continue
```

### Comparing `termynal-0.3.0/termynal/plugin.py` & `termynal-0.3.1/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.3.0/setup.py` & `termynal-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'markdown.extensions': ['termynal = termynal.markdown:TermynalExtension'],
  'mkdocs.plugins': ['termynal = termynal.plugin:TermynalPlugin']}
 
 setup_kwargs = {
     'name': 'termynal',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': '',
     'long_description': '# Termynal\n\nA lightweight and modern animated terminal window.\nBuilt for [mkdocs](https://www.mkdocs.org/).\n\n## Installation\n\n<!-- termynal -->\n\n```\n$ pip install termynal\n---> 100%\nInstalled\n```\n\n[Example](https://daxartio.github.io/termynal/)\n\n## Usage\n\nUse `<!-- termynal -->` before code block\n\n````\n<!-- termynal -->\n\n```\n// code\n```\n````\n\nor `console` in code block\n\n````\n```console\n// code\n```\n````\n\nprogress, prompt `---> 100%`\n\n````\n```console\n$ show progress\n---> 100%\nDone!\n```\n````\n\ncommand, start with `$`\n\n````\n```console\n$ command\n```\n````\n\ncomment, start with `#`\n\n````\n```console\n# comment\n```\n````\n\n`mkdocs` plugin\n\n```yaml\n...\nplugins:\n  - termynal\n...\n```\n\nThanks [ines](https://github.com/ines/termynal)\n',
     'author': 'Danil Akhtarov',
     'author_email': 'daxartio@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/termynal',
```

### Comparing `termynal-0.3.0/PKG-INFO` & `termynal-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

