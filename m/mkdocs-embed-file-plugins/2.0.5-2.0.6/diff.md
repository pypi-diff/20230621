# Comparing `tmp/mkdocs_embed_file_plugins-2.0.5.tar.gz` & `tmp/mkdocs_embed_file_plugins-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_embed_file_plugins-2.0.5.tar", last modified: Sun Jan 15 00:35:17 2023, max compression
+gzip compressed data, was "mkdocs_embed_file_plugins-2.0.6.tar", last modified: Wed Jun 21 21:31:15 2023, max compression
```

## Comparing `mkdocs_embed_file_plugins-2.0.5.tar` & `mkdocs_embed_file_plugins-2.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-15 00:35:17.635281 mkdocs_embed_file_plugins-2.0.5/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3996 2023-01-15 00:35:17.635281 mkdocs_embed_file_plugins-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3131 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-15 00:35:17.631281 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9280 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-15 00:35:17.635281 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/links_correction.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/search_quote.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-01-15 00:35:14.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-15 00:35:17.631281 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3996 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      583 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-15 00:35:17.000000 mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-01-15 00:35:17.635281 mkdocs_embed_file_plugins-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1725 2023-01-15 00:35:15.000000 mkdocs_embed_file_plugins-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8930 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/links_correction.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/search_quote.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-21 21:31:12.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-21 21:31:15.000000 mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-21 21:31:15.097541 mkdocs_embed_file_plugins-2.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 21:31:13.000000 mkdocs_embed_file_plugins-2.0.6/setup.py
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/LICENSE` & `mkdocs_embed_file_plugins-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_embed_file_plugins-2.0.5/PKG-INFO` & `mkdocs_embed_file_plugins-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_embed_file_plugins
-Version: 2.0.5
+Version: 2.0.6
 Summary: A plugin to quote file from docs
 Home-page: https://github.com/Mara-Li/mkdocs_embed_file_plugins
 Author: Mara-Li
 Author-email: mara-li@icloud.com
 License: AGPL
 Keywords: obsidian,obsidian.md,mkdocs,file,embed,cite,quote
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs_embed_file_plugins Version: 2.0.5 Summary: A
+Metadata-Version: 2.1 Name: mkdocs_embed_file_plugins Version: 2.0.6 Summary: A
 plugin to quote file from docs Home-page: https://github.com/Mara-Li/
 mkdocs_embed_file_plugins Author: Mara-Li Author-email: mara-li@icloud.com
 License: AGPL Keywords: obsidian,obsidian.md,mkdocs,file,embed,cite,quote
 Classifier: Natural Language :: English Classifier: Natural Language :: French
 Classifier: Topic :: Text Processing :: Markup :: Markdown Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/README.md` & `mkdocs_embed_file_plugins-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/plugin.py` & `mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,219 +2,225 @@
 import os
 import re
 from pathlib import Path
 from urllib.parse import unquote
 import frontmatter
 import markdown
 from bs4 import BeautifulSoup
-from mdx_wikilink_plus.mdx_wikilink_plus import WikiLinkPlusExtension
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs_callouts.plugin import CalloutsPlugin
 from custom_attributes.plugin import convert_text_attributes
 import logging
 
-from mkdocs_embed_file_plugins.src.links_correction import convert_links_if_markdown, mini_ez_links
-from mkdocs_embed_file_plugins.src.search_quote import search_file_in_documentation, search_in_file
+from mkdocs_embed_file_plugins.src.links_correction import (
+    convert_links_if_markdown,
+    mini_ez_links,
+)
+from mkdocs_embed_file_plugins.src.search_quote import (
+    search_file_in_documentation,
+    search_in_file,
+)
 from mkdocs_embed_file_plugins.src.utils import create_link, strip_comments
 
 
 def cite(
-        md_link_path, link, soup, citation_part, config,
-        callouts, custom_attr, msg
-        ) -> BeautifulSoup :
+    md_link_path, link, soup, citation_part, config, callouts, custom_attr, msg
+) -> BeautifulSoup:
     """Append the content of the founded file to the original file.
 
     Args:
         md_link_path (str): Path of the file to be modified.
         link (str): Link to the file to be included.
         soup (BeautifulSoup): BeautifulSoup object of the file to be modified.
         citation_part (str): Part of the link to be included.
         config (dict): Configuration of the plugin.
         callouts (CalloutsPlugin): Callouts plugin.
         custom_attr (CustomAttributesPlugin): Custom attributes plugin.
         msg (str): Message to be displayed if the file is not found.
     Returns: updated HTML
     """
-    docs = config['docs_dir']
-    url = config['site_url']
+    docs = config["docs_dir"]
+    url = config["site_url"]
 
     md_config = {
-        'mdx_wikilink_plus' : {
-            'base_url' : (docs, url, md_link_path),
-            'build_url' : mini_ez_links,
-            'image_class' : 'wikilink',
-            }
+        "mdx_wikilink_plus": {
+            "base_url": (docs, url, md_link_path),
+            "build_url": mini_ez_links,
+            "image_class": "wikilink",
         }
+    }
     new_uri = str(md_link_path).replace(str(docs), str(url))
-    new_uri = new_uri.replace('\\', '/')
-    new_uri = new_uri.replace('.md', '/')
-    new_uri = new_uri.replace('//', '/')
-    new_uri = re.sub('https?:\\/', '\\g<0>/', new_uri)
-    new_uri = new_uri.replace('/index/', '/')
-    input_file = codecs.open(str(md_link_path), mode = 'r', encoding = 'utf-8')
+    new_uri = new_uri.replace("\\", "/")
+    new_uri = new_uri.replace(".md", "/")
+    new_uri = new_uri.replace("//", "/")
+    new_uri = re.sub("https?:\\/", "\\g<0>/", new_uri)
+    new_uri = new_uri.replace("/index/", "/")
+    input_file = codecs.open(str(md_link_path), mode="r", encoding="utf-8")
     text = input_file.read()
 
     contents = frontmatter.loads(text).content
     quote = search_in_file(citation_part, contents)
     tooltip_template = (
-            "<div class='citation'> <a href='"
-            + str(link['src'])
-            + "' class='link_citation'><i class='fas fa-link'></i> </a>"
-            + str(link['alt']) + ' not exists.'
-            + '</div>'
+        "<div class='citation'> <a href='"
+        + str(link["src"])
+        + "' class='link_citation'><i class='fas fa-link'></i> </a>"
+        + str(link["alt"])
+        + " not exists."
+        + "</div>"
     )
-    if len(quote) > 0 :
-        if callouts :
+    if len(quote) > 0:
+        if callouts:
             quote = CalloutsPlugin().on_page_markdown(quote, None, None, None)
-        if len(custom_attr) > 0 :
-            config_attr = {
-                'file' : custom_attr,
-                'docs_dir' : docs
-                }
+        if len(custom_attr) > 0:
+            config_attr = {"file": custom_attr, "docs_dir": docs}
             quote = convert_text_attributes(quote, config_attr)
         quote = convert_links_if_markdown(quote, (docs, url, md_link_path))
         quote = strip_comments(quote)
-        md_extensions = config['markdown_extensions']
-        md_extensions.append('mdx_wikilink_plus')
+        md_extensions = config["markdown_extensions"]
+        md_extensions.append("mdx_wikilink_plus")
         html = markdown.markdown(
-                quote,
-                extensions = md_extensions,
-                extension_configs = md_config
-                )
-        link_soup = BeautifulSoup(html, 'html.parser')
-        if link_soup :
+            quote, extensions=md_extensions, extension_configs=md_config
+        )
+        link_soup = BeautifulSoup(html, "html.parser")
+        if link_soup:
             tooltip_template = (
-                    "<div class='citation'> <a href='"
-                    + str(new_uri)
-                    + "' class='link_citation'><i class='fas fa-link'></i> </a>"
-                    + str(link_soup).replace(
+                "<div class='citation'> <a href='"
+                + str(new_uri)
+                + "' class='link_citation'><i class='fas fa-link'></i> </a>"
+                + str(link_soup).replace(
                     '!<img class="wikilink', '<img class="wikilink'
-                    )
-                    + '</div>'
+                )
+                + "</div>"
             )
             new_soup = str(soup).replace(str(link), str(tooltip_template))
-            soup = BeautifulSoup(new_soup, 'html.parser')
+            soup = BeautifulSoup(new_soup, "html.parser")
             return soup
-    else :
-        log = logging.getLogger('mkdocs.plugins.' + __name__)
+    else:
+        log = logging.getLogger("mkdocs.plugins." + __name__)
         log.info(
-                '[EMBED FILE PLUGIN] CITATION NOT FOUND : ' +
-                unquote(citation_part) +
-                'for : ' +
-                str(md_link_path) +
-                ' with link: ' +
-                str(link) +
-                ' and new_uri: ' +
-                str(new_uri) +
-                ' and quote: ' +
-                str(quote)
-                )
+            "[EMBED FILE PLUGIN] CITATION NOT FOUND : "
+            + unquote(citation_part)
+            + "for : "
+            + str(md_link_path)
+            + " with link: "
+            + str(link)
+            + " and new_uri: "
+            + str(new_uri)
+            + " and quote: "
+            + str(quote)
+        )
         return tooltip_not_found(link, soup, msg)
 
 
-def tooltip_not_found(link, soup, msg) -> BeautifulSoup :
+def tooltip_not_found(link, soup, msg) -> BeautifulSoup:
     tooltip_template = (
-            "<div class='citation'> <a class='link_citation'><i class='fas fa-link'></i> </a>"
-            + '<p style="text-align: center; display: block"><i class="not_found">' +
-            str(link['alt']) + f'</i> {msg}</p>'
-            + '</div>'
+        "<div class='citation'> <a class='link_citation'><i class='fas fa-link'></i> </a>"
+        + '<p style="text-align: center; display: block"><i class="not_found">'
+        + str(link["alt"])
+        + f"</i> {msg}</p>"
+        + "</div>"
     )
     new_soup = str(soup).replace(str(link), str(tooltip_template))
-    soup = BeautifulSoup(new_soup, 'html.parser')
+    soup = BeautifulSoup(new_soup, "html.parser")
     return soup
 
 
-class EmbedFile(BasePlugin) :
+class EmbedFile(BasePlugin):
     config_scheme = (
-        ('callouts', config_options.Type(bool, default = False)),
-        ('custom-attributes', config_options.Type(str, default = '')),
-        ('language_message', config_options.Type(str, default = 'file not exists')),
-        )
+        ("callouts", config_options.Type(bool, default=False)),
+        ("custom-attributes", config_options.Type(str, default="")),
+        ("language_message", config_options.Type(str, default="file not exists")),
+    )
 
-    def __init__(self) :
+    def __init__(self):
         self.enabled = True
         self.total_time = 0
 
-    def on_post_page(self, output_content, page, config) -> str :
-        soup = BeautifulSoup(output_content, 'html.parser')
-        docs = Path(config['docs_dir'])
-        md_link_path = ''
-        callout = self.config['callouts']
-        language_message = self.config['language_message']
+    def on_post_page(self, output_content, page, config) -> str:
+        soup = BeautifulSoup(output_content, "html.parser")
+        docs = Path(config["docs_dir"])
+        md_link_path = ""
+        callout = self.config["callouts"]
+        language_message = self.config["language_message"]
         for link in soup.findAll(
-                'img',
-                src = lambda src : src is not None
-                                   and 'favicon' not in src
-                                   and not src.endswith(('png', 'jpg', 'jpeg', 'gif', 'svg'))
-                                   and not 'www' in src
-                                   and not 'http' in src
-                                   and not '://' in src,
-                ) :
-            if len(link['src']) > 0 :
-                if link['src'].startswith('./') :
+            "img",
+            src=lambda src: src is not None
+            and "favicon" not in src
+            and not src.endswith(("png", "jpg", "jpeg", "gif", "svg"))
+            and "www" not in src
+            and "http" not in src
+            and "://" not in src,
+        ):
+            if len(link["src"]) > 0:
+                if link["src"].startswith("./"):
                     md_link_path = page.file.abs_src_path
-                elif link['src'][0] == '.' :  # relative links
-                    md_src = create_link(unquote(link['src']))
+                elif link["src"][0] == ".":  # relative links
+                    md_src = create_link(unquote(link["src"]))
                     md_link_path = Path(
-                            os.path.dirname(page.file.abs_src_path), md_src
-                            ).resolve()
-                    md_link_path = re.sub(
-                            r'[\/\\]?#(.*)$', '', str(md_link_path)
-                            )
-                    if not os.path.isfile(md_link_path) :
+                        os.path.dirname(page.file.abs_src_path), md_src
+                    ).resolve()
+                    md_link_path = re.sub(r"[\/\\]?#(.*)$", "", str(md_link_path))
+                    if not os.path.isfile(md_link_path):
                         md_link_path = search_file_in_documentation(
-                                md_link_path, docs
-                                )
+                            md_link_path, docs, docs
+                        )
 
-                elif link['src'][0] == '/' :
-                    md_src_path = create_link(unquote(link['src']))
-                    md_link_path = os.path.join(
-                            config['docs_dir'], md_src_path
-                            )
+                elif link["src"][0] == "/":
+                    md_src_path = create_link(unquote(link["src"]))
+                    md_link_path = os.path.join(config["docs_dir"], md_src_path)
                     md_link_path = Path(unquote(md_link_path)).resolve()
 
-                elif link['src'][0] != '#':
-                    md_src_path = create_link(unquote(link['src']))
+                elif link["src"][0] != "#":
+                    md_src_path = create_link(unquote(link["src"]))
                     md_link_path = os.path.join(
-                            os.path.dirname(page.file.abs_src_path), md_src_path
-                            )
-                    md_link_path = re.sub(
-                            r'/#(.*).md$', '.md', str(md_link_path)
-                            )
+                        os.path.dirname(page.file.abs_src_path), md_src_path
+                    )
+                    md_link_path = re.sub(r"/#(.*).md$", ".md", str(md_link_path))
                     md_link_path = Path(unquote(md_link_path)).resolve()
 
-            else :
-                md_src_path = create_link(unquote(link['src']))
+            else:
+                md_src_path = create_link(unquote(link["src"]))
                 md_link_path = os.path.join(
-                        os.path.dirname(page.file.abs_src_path), md_src_path
-                        )
+                    os.path.dirname(page.file.abs_src_path), md_src_path
+                )
                 md_link_path = Path(unquote(md_link_path)).resolve()
-            if md_link_path == 0 :
+            if md_link_path == 0:
                 soup = tooltip_not_found(link, soup, language_message)
-            if (md_link_path != '' or md_link_path ==
-                0) and len(link['src']) > 0 :
-                if '#' in link.get('alt', '') :
+            if (md_link_path != "" or md_link_path == 0) and len(link["src"]) > 0:
+                if "#" in link.get("alt", ""):
                     # heading
-                    citation_part = re.sub('^(.*)#', '#', link['alt'])
-                elif '#' in link.get('src', '') :
-                    citation_part = re.sub('^(.*)#', '#', unquote(link['src']))
-                else :
-                    citation_part = link.get('alt', False)
-                if citation_part :
+                    citation_part = re.sub("^(.*)#", "#", link["alt"])
+                elif "#" in link.get("src", ""):
+                    citation_part = re.sub("^(.*)#", "#", unquote(link["src"]))
+                else:
+                    citation_part = link.get("alt", False)
+                if citation_part:
                     md_link_path = Path(str(md_link_path))
 
-                    if os.path.isfile(md_link_path) :
+                    if os.path.isfile(md_link_path):
                         soup = cite(
-                                md_link_path, link, soup,
-                                citation_part, config, callout, self.config['custom-attributes'], language_message
-                                )
-                    else :
+                            md_link_path,
+                            link,
+                            soup,
+                            citation_part,
+                            config,
+                            callout,
+                            self.config["custom-attributes"],
+                            language_message,
+                        )
+                    else:
                         link_found = search_file_in_documentation(
-                                md_link_path, docs
-                                )
-                        if link_found != 0 :
+                            md_link_path, docs, docs
+                        )
+                        if link_found != 0:
                             soup = cite(
-                                    link_found, link, soup,
-                                    citation_part, config, callout, self.config['custom-attributes'], language_message
-                                    )
+                                link_found,
+                                link,
+                                soup,
+                                citation_part,
+                                config,
+                                callout,
+                                self.config["custom-attributes"],
+                                language_message,
+                            )
         return str(soup)
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/links_correction.py` & `mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/links_correction.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,67 +3,75 @@
 import os
 import re
 from urllib.parse import quote
 
 from mkdocs_embed_file_plugins.src.search_quote import search_file_in_documentation
 
 
-def mini_ez_links(link, base, end, url_whitespace, url_case) :
+def mini_ez_links(link, base, end, url_whitespace, url_case):
     base_data, url_blog, md_link_path = base
-    url_blog_path = [x for x in url_blog.split('/') if len(x) > 0]
+    url_blog_path = [x for x in url_blog.split("/") if len(x) > 0]
     url_blog_path = url_blog_path[len(url_blog_path) - 1]
     internal_link = Path(md_link_path, link[2]).resolve()
     return create_url(internal_link, link[2], base, url_blog_path, True)
 
 
-def convert_links_if_markdown(quote_str, base) :
+def convert_links_if_markdown(quote_str, base):
     """Convert links if the file is a markdown file."""
     # search for links
-    links = re.findall(r'\[([^\]]*)\]\(([^\)]*)\)', quote_str)
+    links = re.findall(r"\[([^\]]*)\]\(([^\)]*)\)", quote_str)
     base_data, url_blog, md_link_path = base
-    url_blog_path = [x for x in url_blog.split('/') if len(x) > 0]
+    url_blog_path = [x for x in url_blog.split("/") if len(x) > 0]
     url_blog_path = url_blog_path[len(url_blog_path) - 1]
-    for link in links :
-        if not link[1].startswith('http') :
+    for link in links:
+        if not link[1].startswith("http"):
             internal_link = Path(md_link_path, link[1]).resolve()
             url = create_url(internal_link, link[1], base, url_blog_path, False)
             quote_str = quote_str.replace(link[1], url)
     return quote_str
 
 
-def create_url(internal_link, link, base, url_blog_path, wikilinks=False) :
+def create_url(internal_link, link, base, url_blog_path, wikilinks=False):
     base, url_blog, md_link_path = base
-    if os.path.isfile(internal_link) :
-        internal_link = str(internal_link).replace(base, '')
-    else :
-        if link.endswith('.md') :
-            if wikilinks :
-                internal_link = str(search_file_in_documentation(Path(link).resolve(), md_link_path.parent))
-            else :
-                internal_link = str(search_file_in_documentation(link, md_link_path.parent))
-        if not os.path.isfile(internal_link) :
-            file_name = link.replace('index', '')
-            file_name = file_name.replace('../', '')
-            file_name = file_name.replace('./', '')
-            file_name = file_name.replace('.md', '')
+    if os.path.isfile(internal_link):
+        internal_link = str(internal_link).replace(base, "")
+    else:
+        if link.endswith(".md"):
+            if wikilinks:
+                internal_link = str(
+                    search_file_in_documentation(
+                        Path(link).resolve(), md_link_path.parent, base
+                    )
+                )
+            else:
+                internal_link = str(
+                    search_file_in_documentation(link, md_link_path.parent, base)
+                )
+        if not os.path.isfile(internal_link):
+            file_name = link.replace("index", "")
+            file_name = file_name.replace("../", "")
+            file_name = file_name.replace("./", "")
+            file_name = file_name.replace(".md", "")
             all_docs = [
-                re.sub(rf"(.*)({url_blog_path})?/docs/*", '', x.replace('\\', '/')).replace(
-                        '.md', ''
-                        )
-                for x in iglob(str(base) + os.sep + '**', recursive = True)
+                re.sub(
+                    rf"(.*)({url_blog_path})?/docs/*", "", x.replace("\\", "/")
+                ).replace(".md", "")
+                for x in iglob(str(base) + os.sep + "**", recursive=True)
                 if os.path.isfile(x)
-                ]
+            ]
             file_found = [
-                '/' + x for x in all_docs if os.path.basename(x) == file_name or x == file_name
-                ]
-            if file_found :
+                "/" + x
+                for x in all_docs
+                if os.path.basename(x) == file_name or x == file_name
+            ]
+            if file_found:
                 internal_link = file_found[0]
-            else :
+            else:
                 internal_link = file_name
-    filepath = internal_link.replace(base, '')
-    url = filepath.replace('\\', '/').replace('.md', '')
-    url = re.sub(r'\/$', '', str(url_blog)) + '/' + quote(url)
-    if not url.startswith('http') :
-        url = 'https://' + url
-    if not url.endswith('/') and not re.search(r'\.(.*)$', url) :
-        url = url + '/'
+    filepath = internal_link.replace(base, "")
+    url = filepath.replace("\\", "/").replace(".md", "")
+    url = re.sub(r"\/$", "", str(url_blog)) + "/" + quote(url)
+    if not url.startswith("http"):
+        url = "https://" + url
+    if not url.endswith("/") and not re.search(r"\.(.*)$", url):
+        url = url + "/"
     return url
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins/src/search_quote.py` & `mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins/src/search_quote.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,48 +8,59 @@
     """
     Search a part in the file
     Args:
         citation_part: The part to find
         contents: The file contents
     Returns: the part found
     """
-    data = contents.split('\n')
-    if '#' not in citation_part:
+    data = contents.split("\n")
+    if "#" not in citation_part:
         # All text citation
-        return re.sub(r'\[?\^\w+$', '', contents)
-    elif '#' in citation_part and not '^' in citation_part:
+        return re.sub(r"\[?\^\w+$", "", contents)
+    elif "#" in citation_part and "^" not in citation_part:
         # cite from title
         sub_section = []
-        citation_part = citation_part.replace(
-            '-', ' ').replace('#', '# ').upper()
+        citation_part = citation_part.replace("-", " ").replace("#", "# ").upper()
         heading = 0
 
         for i in data:
-            if citation_part in i.upper() and i.startswith('#'):
-                heading = i.count('#') * (-1)
+            if citation_part in i.upper() and i.startswith("#"):
+                heading = i.count("#") * (-1)
                 sub_section.append([i])
             elif heading != 0:
-                inverse = i.count('#') * (-1)
+                inverse = i.count("#") * (-1)
                 if inverse == 0 or heading > inverse:
                     sub_section.append([i])
                 elif inverse >= heading:
                     break
         sub_section = [x for y in sub_section for x in y]
-        sub_section = [re.sub(r'\[?\^\w+$', '', x) for x in sub_section]
-        sub_section = '\n'.join(sub_section)
+        sub_section = [re.sub(r"\[?\^\w+$", "", x) for x in sub_section]
+        sub_section = "\n".join(sub_section)
         return sub_section
-    elif '#^' in citation_part:
+    elif "#^" in citation_part:
         # cite from block
-        citation_part = citation_part.replace('#', '')
+        citation_part = citation_part.replace("#", "")
         for i in data:
-            if re.search(re.escape(citation_part) + '$', i):
-                return i.replace(citation_part, '')
-    return ''
+            if re.search(re.escape(citation_part) + "$", i):
+                print("found!", i.replace(citation_part, ""))
+                return i.replace(citation_part, "")
+    return ""
+
 
 def search_file_in_documentation(
-        link: Union[Path, str], config_dir: Path) -> Union[Path, int]:
+    link: Union[Path, str], config_dir: Path, base: any
+) -> Union[Path, int]:
     file_name = os.path.basename(link)
-    if not file_name.endswith('.md'):
-        file_name = file_name + '.md'
-    for p in config_dir.rglob(f'*{file_name}'):
-        return p
+    if not file_name.endswith(".md"):
+        file_name = file_name + ".md"
+    if not file_name.startswith("index"):
+        for p in config_dir.rglob(f"*{file_name}"):
+            return p
+    else:
+        baseParent = Path(base).parents
+        linksParent = Path(link).parents
+        # find the common parent
+        linksBaseEquals = [i for i in linksParent if i in baseParent][0]
+        relative = Path(str(link).replace(str(linksBaseEquals), ""))
+        for p in Path(base).rglob(f"**{relative}"):
+            return p
     return 0
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/PKG-INFO` & `mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-embed-file-plugins
-Version: 2.0.5
+Version: 2.0.6
 Summary: A plugin to quote file from docs
 Home-page: https://github.com/Mara-Li/mkdocs_embed_file_plugins
 Author: Mara-Li
 Author-email: mara-li@icloud.com
 License: AGPL
 Keywords: obsidian,obsidian.md,mkdocs,file,embed,cite,quote
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-embed-file-plugins Version: 2.0.5 Summary: A
+Metadata-Version: 2.1 Name: mkdocs-embed-file-plugins Version: 2.0.6 Summary: A
 plugin to quote file from docs Home-page: https://github.com/Mara-Li/
 mkdocs_embed_file_plugins Author: Mara-Li Author-email: mara-li@icloud.com
 License: AGPL Keywords: obsidian,obsidian.md,mkdocs,file,embed,cite,quote
 Classifier: Natural Language :: English Classifier: Natural Language :: French
 Classifier: Topic :: Text Processing :: Markup :: Markdown Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mkdocs_embed_file_plugins-2.0.5/mkdocs_embed_file_plugins.egg-info/SOURCES.txt` & `mkdocs_embed_file_plugins-2.0.6/mkdocs_embed_file_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_embed_file_plugins-2.0.5/setup.py` & `mkdocs_embed_file_plugins-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
-version = "2.0.5"
+version = "2.0.6"
+
 
 def classification_dependencies():
     with open("requirements.txt") as f:
-        external=[]
-        internal=[]
+        external = []
+        internal = []
         for package in f.read().splitlines():
             if package.startswith("git+"):
-                external.append(package.replace('git+', ''))
+                external.append(package.replace("git+", ""))
             else:
                 internal.append(package)
     return external, internal
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

