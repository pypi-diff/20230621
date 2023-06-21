# Comparing `tmp/ufomerge-1.1.0.tar.gz` & `tmp/ufomerge-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufomerge-1.1.0.tar", last modified: Fri May 26 06:28:05 2023, max compression
+gzip compressed data, was "ufomerge-1.2.0.tar", last modified: Wed Jun 21 09:58:43 2023, max compression
```

## Comparing `ufomerge-1.1.0.tar` & `ufomerge-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.964199 ufomerge-1.1.0/
--rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.1.0/AUTHORS.txt
--rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.1.0/CONTRIBUTORS.txt
--rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.1.0/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.959356 ufomerge-1.1.0/Lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.961735 ufomerge-1.1.0/Lib/ufomerge/
--rw-r--r--   0 simon      (501) staff       (20)    27676 2023-05-26 06:20:31.000000 ufomerge-1.1.0/Lib/ufomerge/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.1.0/Lib/ufomerge/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)      160 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge/_version.py
--rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.1.0/Lib/ufomerge/cli.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.962921 ufomerge-1.1.0/Lib/ufomerge.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      433 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       47 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)       29 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-26 06:28:05.964027 ufomerge-1.1.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.1.0/README.md
--rw-r--r--   0 simon      (501) staff       (20)      632 2023-05-26 06:27:42.000000 ufomerge-1.1.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-26 06:28:05.964239 ufomerge-1.1.0/setup.cfg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.963658 ufomerge-1.1.0/tests/
--rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.1.0/tests/conftest.py
--rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.1.0/tests/test_basic.py
--rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.1.0/tests/test_layout.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.276602 ufomerge-1.2.0/
+-rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.2.0/AUTHORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.2.0/CONTRIBUTORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.2.0/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.272517 ufomerge-1.2.0/Lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.274703 ufomerge-1.2.0/Lib/ufomerge/
+-rw-r--r--   0 simon      (501) staff       (20)    30294 2023-06-21 09:41:06.000000 ufomerge-1.2.0/Lib/ufomerge/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.2.0/Lib/ufomerge/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)      160 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge/_version.py
+-rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.2.0/Lib/ufomerge/cli.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.275535 ufomerge-1.2.0/Lib/ufomerge.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      433 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       47 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)       18 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-06-21 09:58:43.276459 ufomerge-1.2.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.2.0/README.md
+-rw-r--r--   0 simon      (501) staff       (20)      616 2023-06-21 09:02:36.000000 ufomerge-1.2.0/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-21 09:58:43.276635 ufomerge-1.2.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.276174 ufomerge-1.2.0/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.2.0/tests/conftest.py
+-rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.2.0/tests/test_basic.py
+-rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.2.0/tests/test_layout.py
```

### Comparing `ufomerge-1.1.0/CONTRIBUTORS.txt` & `ufomerge-1.2.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/LICENSE` & `ufomerge-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/Lib/ufomerge/__init__.py` & `ufomerge-1.2.0/Lib/ufomerge/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,14 +112,15 @@
                     )
                 count = len(self.final_glyphset)
 
         if self.layout_handling != "ignore":
             self.ufo2_features.statements = self.filter_layout(
                 self.ufo2_features.statements
             )
+            self.clean_layout(self.ufo2_features)
             self.ufo1.features.text += self.ufo2_features.asFea()
             self.add_language_systems()
 
         # list() avoids "Set changed size during iteration" error
         for glyph in list(self.incoming_glyphset.keys()):
             self.close_components(glyph)
 
@@ -414,16 +415,76 @@
                 st.suffix = self.filter_sequence(st.suffix)
                 container, vr = st.pos[0]
                 st.pos = [(self.filter_glyph_container(container), vr)]
                 if not st.pos[0][0].glyphSet():
                     continue
 
             newstatements.append(st)
+
         return newstatements
 
+    def clean_layout(self, layout: ast.FeatureFile):
+        # Collect all referenced lookups
+        referenced = set()
+        for feature in layout.statements:
+            if not isinstance(feature, (ast.FeatureBlock, ast.LookupBlock)):
+                continue
+            for statement in feature.statements:
+                if isinstance(statement, ast.LookupReferenceStatement):
+                    referenced.add(statement.lookup.name)
+                if hasattr(statement, "lookups"):
+                    for lookuplist in statement.lookups:
+                        if lookuplist is None:
+                            continue
+                        if isinstance(lookuplist, (list, tuple)):
+                            for lookup in lookuplist:
+                                referenced.add(lookup.name)
+                        else:
+                            referenced.add(lookuplist.name)
+
+        newfeatures = []
+        # If there are any lookups within a feature but with no effective
+        # statements, remove them.
+        for feature in layout.statements:
+            # Remove any unreferenced lookups
+            if isinstance(feature, ast.LookupBlock) and feature.name not in referenced:
+                continue
+            if not isinstance(feature, ast.FeatureBlock):
+                newfeatures.append(feature)
+                continue
+            newstatements = []
+            for lookup in feature.statements:
+                if not isinstance(lookup, ast.LookupBlock) or lookup.name in referenced:
+                    newstatements.append(lookup)
+                    continue
+                effective = False
+                for statement in lookup.statements:
+                    if isinstance(statement, (ast.Comment, ast.LookupFlagStatement)):
+                        continue
+                    effective = True
+                    break
+                if effective:
+                    newstatements.append(lookup)
+                else:
+                    logger.warn(
+                        "Removing ineffective lookup %s in %s "
+                        % (lookup.name, feature.name)
+                    )
+            if newstatements and any(
+                [
+                    not isinstance(
+                        st, (ast.Comment, ast.ScriptStatement, ast.LanguageStatement)
+                    )
+                    for st in newstatements
+                ]
+            ):
+                feature.statements = newstatements
+                newfeatures.append(feature)
+        layout.statements = newfeatures
+
     def fix_context_and_check_applicable(self, rule) -> bool:
         # Slim context and inputs to only those glyphs we have
 
         # Horrible API decision in FontFeatures, sorry everyone
         if hasattr(rule, "input"):
             rule.input = self.filter_sequence(rule.input)
             slots = rule.input
```

### Comparing `ufomerge-1.1.0/Lib/ufomerge/cli.py` & `ufomerge-1.2.0/Lib/ufomerge/cli.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/Lib/ufomerge.egg-info/PKG-INFO` & `ufomerge-1.2.0/Lib/ufomerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.1.0
+Version: 1.2.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.1.0/PKG-INFO` & `ufomerge-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.1.0
+Version: 1.2.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.1.0/README.md` & `ufomerge-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/pyproject.toml` & `ufomerge-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   { name = "Simon Cozens", email = "simon@simon-cozens.org" }
 ]
 classifiers = [
   'Environment :: Console',
   'Topic :: Text Processing :: Fonts',
 ]
 dependencies = [
-  'setuptools',
   'fontTools',
   'ufoLib2',
 ]
 
 [project.scripts]
 ufomerge = "ufomerge.cli:main"
```

### Comparing `ufomerge-1.1.0/tests/conftest.py` & `ufomerge-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/tests/test_basic.py` & `ufomerge-1.2.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.1.0/tests/test_layout.py` & `ufomerge-1.2.0/tests/test_layout.py`

 * *Files identical despite different names*

