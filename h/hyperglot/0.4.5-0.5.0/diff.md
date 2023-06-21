# Comparing `tmp/hyperglot-0.4.5.tar.gz` & `tmp/hyperglot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperglot-0.4.5.tar", last modified: Tue Mar 28 10:07:22 2023, max compression
+gzip compressed data, was "hyperglot-0.5.0.tar", last modified: Wed Jun 21 08:27:20 2023, max compression
```

## Comparing `hyperglot-0.4.5.tar` & `hyperglot-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-03-28 10:07:22.386044 hyperglot-0.4.5/
--rw-r--r--   0 johannes   (501) staff       (20)    35145 2022-06-21 08:09:24.000000 hyperglot-0.4.5/LICENSE.txt
--rw-r--r--   0 johannes   (501) staff       (20)    11768 2023-03-28 10:07:22.385793 hyperglot-0.4.5/PKG-INFO
--rw-r--r--   0 johannes   (501) staff       (20)    10977 2022-12-18 19:22:02.000000 hyperglot-0.4.5/README.md
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-03-28 10:07:22.381384 hyperglot-0.4.5/lib/
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-03-28 10:07:22.383906 hyperglot-0.4.5/lib/hyperglot/
--rw-r--r--   0 johannes   (501) staff       (20)     1079 2023-03-28 10:05:03.000000 hyperglot-0.4.5/lib/hyperglot/__init__.py
--rw-r--r--   0 johannes   (501) staff       (20)   507998 2023-03-28 10:05:03.000000 hyperglot-0.4.5/lib/hyperglot/hyperglot.yaml
--rw-r--r--   0 johannes   (501) staff       (20)    19309 2023-03-27 15:56:35.000000 hyperglot-0.4.5/lib/hyperglot/language.py
--rw-r--r--   0 johannes   (501) staff       (20)    13356 2022-12-18 19:22:02.000000 hyperglot-0.4.5/lib/hyperglot/languages.py
--rw-r--r--   0 johannes   (501) staff       (20)    18268 2023-03-27 15:47:00.000000 hyperglot-0.4.5/lib/hyperglot/main.py
--rw-r--r--   0 johannes   (501) staff       (20)     7948 2022-06-21 08:09:24.000000 hyperglot-0.4.5/lib/hyperglot/parse.py
--rw-r--r--   0 johannes   (501) staff       (20)    13316 2022-12-18 19:22:02.000000 hyperglot-0.4.5/lib/hyperglot/validate.py
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-03-28 10:07:22.385043 hyperglot-0.4.5/lib/hyperglot.egg-info/
--rw-r--r--   0 johannes   (501) staff       (20)    11768 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/PKG-INFO
--rw-r--r--   0 johannes   (501) staff       (20)      519 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/SOURCES.txt
--rw-r--r--   0 johannes   (501) staff       (20)        1 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/dependency_links.txt
--rw-r--r--   0 johannes   (501) staff       (20)      224 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/entry_points.txt
--rw-r--r--   0 johannes   (501) staff       (20)       77 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/requires.txt
--rw-r--r--   0 johannes   (501) staff       (20)       10 2023-03-28 10:07:22.000000 hyperglot-0.4.5/lib/hyperglot.egg-info/top_level.txt
--rw-r--r--   0 johannes   (501) staff       (20)       38 2023-03-28 10:07:22.386083 hyperglot-0.4.5/setup.cfg
--rw-r--r--   0 johannes   (501) staff       (20)     2591 2022-12-18 19:22:02.000000 hyperglot-0.4.5/setup.py
-drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-03-28 10:07:22.385568 hyperglot-0.4.5/tests/
--rw-r--r--   0 johannes   (501) staff       (20)    15951 2023-03-27 15:55:32.000000 hyperglot-0.4.5/tests/test_language.py
--rw-r--r--   0 johannes   (501) staff       (20)     2084 2022-06-21 08:09:24.000000 hyperglot-0.4.5/tests/test_languages.py
--rw-r--r--   0 johannes   (501) staff       (20)     9816 2022-06-21 08:09:24.000000 hyperglot-0.4.5/tests/test_main.py
--rw-r--r--   0 johannes   (501) staff       (20)     5140 2022-06-21 08:09:24.000000 hyperglot-0.4.5/tests/test_parse.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-06-21 08:27:20.785843 hyperglot-0.5.0/
+-rw-r--r--   0 johannes   (501) staff       (20)    35145 2022-06-21 08:09:24.000000 hyperglot-0.5.0/LICENSE.txt
+-rw-r--r--   0 johannes   (501) staff       (20)    11768 2023-06-21 08:27:20.785567 hyperglot-0.5.0/PKG-INFO
+-rw-r--r--   0 johannes   (501) staff       (20)    10977 2023-06-08 09:12:01.000000 hyperglot-0.5.0/README.md
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-06-21 08:27:20.781570 hyperglot-0.5.0/lib/
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-06-21 08:27:20.783675 hyperglot-0.5.0/lib/hyperglot/
+-rw-r--r--   0 johannes   (501) staff       (20)     1069 2023-06-21 08:22:36.000000 hyperglot-0.5.0/lib/hyperglot/__init__.py
+-rw-r--r--   0 johannes   (501) staff       (20)    21371 2023-03-28 13:25:53.000000 hyperglot-0.5.0/lib/hyperglot/language.py
+-rw-r--r--   0 johannes   (501) staff       (20)    14930 2023-06-21 08:22:36.000000 hyperglot-0.5.0/lib/hyperglot/languages.py
+-rw-r--r--   0 johannes   (501) staff       (20)    17982 2023-06-21 08:22:36.000000 hyperglot-0.5.0/lib/hyperglot/main.py
+-rw-r--r--   0 johannes   (501) staff       (20)     7948 2022-06-21 08:09:24.000000 hyperglot-0.5.0/lib/hyperglot/parse.py
+-rw-r--r--   0 johannes   (501) staff       (20)    13316 2022-12-18 19:22:02.000000 hyperglot-0.5.0/lib/hyperglot/validate.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-06-21 08:27:20.784889 hyperglot-0.5.0/lib/hyperglot.egg-info/
+-rw-r--r--   0 johannes   (501) staff       (20)    11768 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/PKG-INFO
+-rw-r--r--   0 johannes   (501) staff       (20)      490 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes   (501) staff       (20)        1 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes   (501) staff       (20)      224 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/entry_points.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       77 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/requires.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       10 2023-06-21 08:27:20.000000 hyperglot-0.5.0/lib/hyperglot.egg-info/top_level.txt
+-rw-r--r--   0 johannes   (501) staff       (20)       38 2023-06-21 08:27:20.785882 hyperglot-0.5.0/setup.cfg
+-rw-r--r--   0 johannes   (501) staff       (20)     2591 2022-12-18 19:22:02.000000 hyperglot-0.5.0/setup.py
+drwxr-xr-x   0 johannes   (501) staff       (20)        0 2023-06-21 08:27:20.785385 hyperglot-0.5.0/tests/
+-rw-r--r--   0 johannes   (501) staff       (20)    15951 2023-03-27 15:55:32.000000 hyperglot-0.5.0/tests/test_language.py
+-rw-r--r--   0 johannes   (501) staff       (20)     2084 2022-06-21 08:09:24.000000 hyperglot-0.5.0/tests/test_languages.py
+-rw-r--r--   0 johannes   (501) staff       (20)     9816 2022-06-21 08:09:24.000000 hyperglot-0.5.0/tests/test_main.py
+-rw-r--r--   0 johannes   (501) staff       (20)     5140 2022-06-21 08:09:24.000000 hyperglot-0.5.0/tests/test_parse.py
```

### Comparing `hyperglot-0.4.5/LICENSE.txt` & `hyperglot-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/PKG-INFO` & `hyperglot-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperglot
-Version: 0.4.5
+Version: 0.5.0
 Summary: Detect language support for font binaries
 Home-page: https://github.com/rosettatype/hyperglot
 Author: Johannes Neumeier - Rosetta
 Author-email: johannes@rosettatype.com
 License: GNU GPLv3
 Project-URL: Hyperglot web interface, https://hyperglot.rosettatype.com
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hyperglot-0.4.5/README.md` & `hyperglot-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/lib/hyperglot/__init__.py` & `hyperglot-0.5.0/lib/hyperglot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Gather a few package wide constants
 """
 from os import path
-__version__ = "0.4.5"
+__version__ = "0.5.0"
 
-DB = path.abspath(path.join(path.dirname(__file__), "hyperglot.yaml"))
+DB = path.abspath(path.join(path.dirname(__file__), "data"))
 
 SUPPORTLEVELS = {
     "base": "base",
     "aux": "auxiliary"
 }
```

### Comparing `hyperglot-0.4.5/lib/hyperglot/language.py` & `hyperglot-0.5.0/lib/hyperglot/language.py`

 * *Files 16% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                              if "status" not in o or
                              o["status"] != "deprecated"]
         else:
             orthographies = [o for o in self["orthographies"]
                              if "status" in o and o["status"] == "primary"]
 
         if not checkAllOrthographies:
-            # Note the .copy() here since we manipulate the attribute ll.256
+            # Note the .copy() here since we manipulate the attribute
             # and do not want to alter the original
             as_group = [o.copy() for o in orthographies
                         if "preferred_as_group" in o]
 
             as_individual = [o.copy() for o in orthographies
                              if "preferred_as_group" not in o]
 
@@ -384,23 +384,59 @@
 base characters: {base_chars}
 base marks: {base_marks}
 auxiliary characters: {aux_chars}
 auxiliary marks: {aux_marks}
 script: {script}
 status: {status}
 note: {note}"""
-        return tpl.format(autonym=self["autonym"],
+        return tpl.format(autonym=self["autonym"] if "autonym" in self else "",
                           base_chars=" ".join(self.base_chars),
                           base_marks=" ".join(self.base_marks),
                           aux_chars=" ".join(self.auxiliary_chars),
                           aux_marks=" ".join(self.auxiliary_marks),
                           script="" if "script" not in self else self["script"],  # noqa
                           status="" if "status" not in self else self["status"],  # noqa
                           note="" if "note" not in self else self["note"])
 
+    def diff(self, chars):
+        """
+        Output a presentation that highlights found and missing chars
+        """
+        tpl = """autonym: {autonym}
+supported base characters: {base_chars}
+supported base marks: {base_marks}
+supported auxiliary characters: {aux_chars}
+supported auxiliary marks: {aux_marks}
+missing base characters: {base_chars_missing}
+missing base marks: {base_marks_missing}
+missing auxiliary characters: {aux_chars_missing}
+missing auxiliary marks: {aux_marks_missing}
+script: {script}
+status: {status}
+note: {note}
+"""
+
+        # base_chars_missing = " ".join([c for c in self.base_chars if c not in chars])
+        # base_marks_missing = " ".join([c for c in self.base_marks if c not in chars])
+        # aux_chars_missing = " ".join([c for c in self.auxiliary_chars if c not in chars])
+        # aux_marks_missing = " ".join([c for c in self.auxiliary_marks if c not in chars])
+
+        return tpl.format(autonym=self["autonym"] if "autonym" in self else "",
+                          base_chars=" ".join([c for c in self.base_chars if c in chars]),
+                          base_chars_missing=" ".join([ c for c in self.base_chars if c not in chars]),
+                          base_marks=" ".join([c for c in self.base_marks if c in chars]),
+                          base_marks_missing=" ".join([ c for c in self.base_marks if c not in chars]),
+                          aux_chars=" ".join([c for c in self.auxiliary_chars if c in chars]),
+                          aux_chars_missing=" ".join([ c for c in self.auxiliary_chars if c not in chars]),
+                          aux_marks=" ".join([c for c in self.auxiliary_marks if c in chars]),
+                          aux_marks_missing=" ".join([ c for c in self.auxiliary_marks if c not in chars]),
+                          script="" if "script" not in self else self["script"],  # noqa
+                          status="" if "status" not in self else self["status"],  # noqa
+                          note="" if "note" not in self else self["note"])
+
     @property
     def script(self):
         return self["script"]
 
     @property
     def base(self):
         """
```

### Comparing `hyperglot-0.4.5/lib/hyperglot/languages.py` & `hyperglot-0.5.0/lib/hyperglot/languages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,63 @@
 """
 Helper classes to work with the rosetta.yaml data in more pythonic way
 """
+import os
 import yaml
 import logging
 from .language import Language
 from . import DB, VALIDITYLEVELS, SUPPORTLEVELS
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.WARNING)
 
 
+def find_language(search):
+    """
+    Utility method to find a language by ISO code or language name
+    """
+
+    hg = Languages(validity=VALIDITYLEVELS[0])
+
+    search = search.lower()
+
+    # Search as 3-letter iso code, return if matched
+    if search in hg.keys():
+        return [getattr(hg, search)], f"Matched from iso code {search}:"
+
+    # Search from language names and autonyms
+    # If a single match is a full 1=1 match return that
+    # If a single match is a partial match, return iso and prompt with info
+    # If more than one are found, return a list of isos as prompt
+
+    matches = {}
+    for iso in hg.keys():
+        lang = getattr(hg, iso)
+        name = lang.get_name().lower()
+        aut = lang.get_autonym()
+        autonyms = [] if not aut else [aut.lower()]
+        if "orthographies" in lang:
+            for o in lang["orthographies"]:
+                if "autonym" in o:
+                    autonyms.append(o["autonym"].lower())
+
+        if search == name or search in autonyms:
+            return [lang], f"Matched from name match for {search}:"
+
+        # For now let's not do any fancy input proximity checks, just partials
+        search_in_autonym = len([a for a in autonyms if search in a]) > 0
+        if search in name or search_in_autonym:
+            matches[iso] = lang
+
+    if len(matches) > 0:
+        return matches.values(), f"Matched for search string {search}"
+
+    return False, ""
+
+
 class Languages(dict):
     """
     A dict wrapper around the language data yaml file with additional querying
     options for convenience
     """
 
     def __init__(self, strict=False, inherit=True, validity=VALIDITYLEVELS[1]):
@@ -22,27 +66,31 @@
             or ISO definitions (True). Defaults to False.
         @param inherit (Boolean): Inherit orthographies. Defaults to True.
         @param validity (Hyperglot.VALIDITYLEVEL): Minimum level of validity
             which languages must have. One of "todo", "draft", "preliminary",
             "verified". Defaults to "draft" — all languages with basic
             information, but possibly unconfirmed.
         """
-        with open(DB, "rb") as f:
-            data = yaml.load(f, Loader=yaml.Loader)
-            self.update(data)
-
-            if inherit:
-                self.inherit_orthographies_from_macrolanguage()
-                self.inherit_orthographies()
 
-            if not strict:
-                self.lax_macrolanguages()
+        # Load raw yaml data for all languages
+        for file in os.listdir(DB):
+            iso = os.path.splitext(file)[0]
+            with open(os.path.join(DB, file), "rb") as f:
+                data = yaml.load(f, Loader=yaml.Loader)
+                self[iso] = data
+
+        if inherit:
+            self.inherit_orthographies_from_macrolanguage()
+            self.inherit_orthographies()
+
+        if not strict:
+            self.lax_macrolanguages()
 
-            self.filter_by_validity(validity)
-            self.set_defaults()
+        self.filter_by_validity(validity)
+        self.set_defaults()
 
     def __repr__(self):
         return "Languages DB dict with '%d' languages" % len(self.keys())
 
     def __getattribute__(self, iso: str) -> Language:
         """
         A convenience getter returning initialized hyperglot.language.Language
```

### Comparing `hyperglot-0.4.5/lib/hyperglot/main.py` & `hyperglot-0.5.0/lib/hyperglot/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import re
 import yaml
 import logging
 from collections import OrderedDict
 from fontTools.ttLib import TTFont
 from . import (__version__, SORTING_DIRECTIONS, DB, SUPPORTLEVELS,
                VALIDITYLEVELS, CHARACTER_ATTRIBUTES, MARK_BASE, SORTING)
-from .languages import Languages
-from .language import Language, is_mark
+from .languages import Languages, find_language
+from .language import Language, Orthography, is_mark
 from .validate import validate
 from .parse import (list_unique, parse_font_chars, parse_marks)
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.WARNING)
 
 # All YAML dumps have these same additional arguments to make sure the unicode
@@ -75,20 +75,24 @@
             items.append("%s (%s)" % (name, str(l["speakers"])))
         else:
             items.append("%s" % name)
 
     return seperator.join(items)
 
 
-def print_to_cli(font, title, autonyms, speakers, strict_iso):
+def print_title(title):
     print()
     print("=" * len(title))
     print(title)
     print("=" * len(title))
     print()
+
+
+def print_to_cli(font, title, autonyms, speakers, strict_iso):
+    print_title(title)
     total = 0
     for script in font:
         count = len(font[script])
         if count > 0:
             print()
             title = "%d %s of %s script:" % \
                 (count, "language" if count == 1 else "languages",
@@ -247,14 +251,17 @@
               type=click.Choice(MODES, case_sensitive=False),
               default=MODES[0], show_default=True,
               help="When passing in more than one file, a comparison can be "
               "generated. By default each file's support is listed "
               "individually. 'union' shows support for all languages "
               "supported by the combination of the passed in fonts. "
               "'intersection' shows the support all fonts have in common.")
+@click.option("-l", "--languages", default="", 
+              help="Pass in one or more comma-separated language names or ISO "
+              "code to output a detailed support report for this font.")
 @click.option("--include-all-orthographies", is_flag=True, default=False,
               help="Flag to show all otherwise ignored orthographies of a "
               "language.")
 @click.option("--include-historical", is_flag=True, default=False,
               help="Flag to include otherwise ignored historical languages.")
 @click.option("--include-constructed", is_flag=True, default=False,
               help="Flag to include otherwise ignored contructed languages.")
@@ -264,14 +271,15 @@
               "transforms to show preferred languages names and "
               "macrolanguage structure that deviates from ISO data.")
 @click.option("-v", "--verbose", is_flag=True, default=False)
 @click.option("-V", "--version", is_flag=True, default=False)
 def cli(fonts, support, decomposed, marks, validity, autonyms, speakers,
         sorting, sort_dir,
         output, comparison,
+        languages,
         include_all_orthographies, include_historical, include_constructed,
         strict_iso, verbose, version):
     """
     Pass in one or more fonts to check their languages support
     """
 
     if version:
@@ -344,14 +352,34 @@
         # Wrap in "single file" 'intersection' top level, which will be removed
         # when writing the data
         data = {"intersection": intersection}
 
     if output:
         write_yaml(output, data)
 
+    if languages:
+        print_title("Language check:")
+        languages = [l.strip() for l in languages.split(",") if l.strip() != ""]  # noqa
+
+        for f in fonts:
+            chars = parse_font_chars(f)
+            for s in languages:
+                res, _ = find_language(s)
+                if res is False:
+                    return
+                for r in res:
+                    res_name = r.get_name()
+                    print(f"Listing full support information for {res_name}")
+                    print()
+                    if "orthographies" not in r:
+                        continue
+                    for o in r["orthographies"]:
+                        ort = Orthography(o)
+                        print(ort.diff(chars))
+
 
 def save_sorted(Langs=None, run_validation=True):
     """
     Helper script to re-save the hyperglot.yaml sorted alphabetically,
     alternatively from the passed in Langs object (which can have been
     modified)
     """
@@ -406,20 +434,31 @@
                     # Note: Let's store marks with a dotted circle and a
                     # whitespace between them to make them more legible. When
                     # parsing the attribute back in circles and all whitespaces
                     # are removed
                     decorated = [MARK_BASE + m for m in list_unique(marks)]
                     o["marks"] = " ".join(decorated)
 
-    # Sort by keys
-    alphabetic = dict(OrderedDict(sorted(Langs.items())))
+    # Ensure db folder exists
+    if not os.path.isdir(DB):
+        os.mkdir(DB)
 
-    file = open(DB, "w")
-    yaml.dump(alphabetic, file, **DUMP_ARGS)
-    print("Saved lib/hyperglot/hyperglot.yaml")
+    for iso, data in Langs.items():
+        save_language(iso, data)
+
+    print("Saved all language data to lib/hyperglot/data")
+
+
+def save_language(iso, data):
+    """
+    Save the language data of one language by its three letter iso (mostly)
+    """
+    file = open(os.path.join(DB, iso + ".yaml"), "w")
+    yaml.dump(data, file, **DUMP_ARGS)
+    logging.info(f"Saved lib/hyperglot/data/{iso}.yaml")
 
 
 @click.command()
 @click.argument("output", type=click.Path())
 def export(output):
     """
     Helper script to export hyperglot.yaml with all inhereted orthographies
@@ -436,57 +475,16 @@
 @click.argument("search")
 def data(search):
     """
     Pass in a 3-letter iso code or language name (search term) to show
     Hyperglot data for it
     """
     print()
-    print(f"Hyperglot data for {search}:")
+    print_title(f"Hyperglot data for '{search}':")
 
     search = search.lower().strip()
 
-    hg = Languages(validity=VALIDITYLEVELS[0])
+    hits, msg = find_language(search)
 
-    # Search as 3-letter iso code, return if matched
-    if search in hg.keys():
-        print(f"Matched from iso code {search}:")
-        print()
-        print(getattr(hg, search).presentation)
-        return
-
-    # Search from language names and autonyms
-    # If a single match is a full 1=1 match return that
-    # If a single match is a partial match, return iso and prompt with info
-    # If more than one are found, return a list of isos as prompt
-
-    matches = {}
-    for iso in hg.keys():
-        lang = getattr(hg, iso)
-        name = lang.get_name().lower()
-        aut = lang.get_autonym()
-        autonyms = [] if not aut else [aut.lower()]
-        if "orthographies" in lang:
-            for o in lang["orthographies"]:
-                if "autonym" in o:
-                    autonyms.append(o["autonym"].lower())
-
-        if search == name or search in autonyms:
-            print(f"Matched from name match for {search}:")
-            print()
-            print(lang.presentation)
-            return
-
-        # For now lets not do any fancy input proximity checks, just partials
-        if search in name or (autonyms != [] and len([a for a in autonyms if search in a]) > 0):
-            matches[iso] = lang
-
-    if len(matches) == 1:
-        print(f"Matched for search string {search}")
-        print()
-        print(list(matches.values())[0].presentation)
-        return
-    elif len(matches) > 1:
-        print("Found several languages matching {search}:")
-        print()
-        print("\n".join(["%s: %s" % (iso, lang.get_name()) for iso, lang in matches.items()]))  # noqa
-        print()
-        print("Narrow your search (by iso code) for one of these results.")
+    print(msg)
+    for h in hits:
+        print(h.presentation)
```

### Comparing `hyperglot-0.4.5/lib/hyperglot/parse.py` & `hyperglot-0.5.0/lib/hyperglot/parse.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/lib/hyperglot/validate.py` & `hyperglot-0.5.0/lib/hyperglot/validate.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/lib/hyperglot.egg-info/PKG-INFO` & `hyperglot-0.5.0/lib/hyperglot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperglot
-Version: 0.4.5
+Version: 0.5.0
 Summary: Detect language support for font binaries
 Home-page: https://github.com/rosettatype/hyperglot
 Author: Johannes Neumeier - Rosetta
 Author-email: johannes@rosettatype.com
 License: GNU GPLv3
 Project-URL: Hyperglot web interface, https://hyperglot.rosettatype.com
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hyperglot-0.4.5/setup.py` & `hyperglot-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/tests/test_language.py` & `hyperglot-0.5.0/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/tests/test_languages.py` & `hyperglot-0.5.0/tests/test_languages.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/tests/test_main.py` & `hyperglot-0.5.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `hyperglot-0.4.5/tests/test_parse.py` & `hyperglot-0.5.0/tests/test_parse.py`

 * *Files identical despite different names*

