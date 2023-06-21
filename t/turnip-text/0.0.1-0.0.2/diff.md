# Comparing `tmp/turnip_text-0.0.1.tar.gz` & `tmp/turnip_text-0.0.2.tar.gz`

## Comparing `turnip_text-0.0.1.tar` & `turnip_text-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 turnip_text-0.0.1/Cargo.toml
--rw-r--r--   0     1001      123      202 2023-04-20 15:16:45.000000 turnip_text-0.0.1/.cargo/config.toml
--rw-r--r--   0     1001      123     2745 2023-04-20 15:16:45.000000 turnip_text-0.0.1/.github/workflows/CI.yaml
--rw-r--r--   0     1001      123       73 2023-04-20 15:16:45.000000 turnip_text-0.0.1/.gitignore
--rw-r--r--   0     1001      123      734 2023-04-20 15:16:45.000000 turnip_text-0.0.1/.vscode/settings.json
--rw-r--r--   0     1001      123    10847 2023-04-20 15:16:45.000000 turnip_text-0.0.1/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-04-20 15:16:45.000000 turnip_text-0.0.1/LICENSE-MIT
--rw-r--r--   0     1001      123     4391 2023-04-20 15:16:45.000000 turnip_text-0.0.1/README.md
--rw-r--r--   0     1001      123       10 2023-04-20 15:17:31.000000 turnip_text-0.0.1/dist/turnip_text-0.0.1.tar.gz
--rw-r--r--   0     1001      123      858 2023-04-20 15:16:45.000000 turnip_text-0.0.1/examples/experiment.pytext
--rw-r--r--   0     1001      123     2503 2023-04-20 15:16:45.000000 turnip_text-0.0.1/examples/phdprop.py
--rw-r--r--   0     1001      123    21583 2023-04-20 15:16:45.000000 turnip_text-0.0.1/examples/phdprop.ttxt
--rw-r--r--   0     1001      123     6171 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/analysis/asciidoctor.md
--rw-r--r--   0     1001      123        0 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/analysis/docbook.md
--rw-r--r--   0     1001      123      113 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/analysis/latex.md
--rw-r--r--   0     1001      123      135 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/analysis/restructuredtext.md
--rw-r--r--   0     1001      123       22 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/analysis/sphinx.md
--rw-r--r--   0     1001      123     9909 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/code_syntax.md
--rw-r--r--   0     1001      123    10166 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/content_v_formatting.md
--rw-r--r--   0     1001      123      188 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/goals.md
--rw-r--r--   0     1001      123     2476 2023-04-20 15:16:45.000000 turnip_text-0.0.1/notes/opinionated_text.md
--rw-r--r--   0     1001      123      734 2023-04-20 15:16:45.000000 turnip_text-0.0.1/pyproject.toml
--rw-r--r--   0     1001      123      744 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/__init__.py
--rw-r--r--   0     1001      123     2227 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/helpers.py
--rw-r--r--   0     1001      123        0 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/py.typed
--rw-r--r--   0     1001      123     9463 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/__init__.py
--rw-r--r--   0     1001      123     2921 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/dictify.py
--rw-r--r--   0     1001      123       31 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/latex/__init__.py
--rw-r--r--   0     1001      123     1432 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/latex/base.py
--rw-r--r--   0     1001      123    10610 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/latex/plugins.py
--rw-r--r--   0     1001      123       35 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/markdown/__init__.py
--rw-r--r--   0     1001      123     1431 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/markdown/base.py
--rw-r--r--   0     1001      123    15982 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/markdown/plugins.py
--rw-r--r--   0     1001      123     2794 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/renderers/std_plugins.py
--rw-r--r--   0     1001      123     1759 2023-04-20 15:16:45.000000 turnip_text-0.0.1/python/turnip_text/turnip_text.pyi
--rw-r--r--   0     1001      123    10884 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/cli.rs
--rw-r--r--   0     1001      123    19518 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/lexer.rs
--rw-r--r--   0     1001      123     1905 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/lexer_charofs_row_col.rs
--rw-r--r--   0     1001      123      102 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/lib.rs
--rw-r--r--   0     1001      123    11084 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/python/interop.rs
--rw-r--r--   0     1001      123    23148 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/python/interp/mod.rs
--rw-r--r--   0     1001      123    26566 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/python/interp/para.rs
--rw-r--r--   0     1001      123      943 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/python/mod.rs
--rw-r--r--   0     1001      123     2815 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/python/typeclass.rs
--rw-r--r--   0     1001      123      502 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/tests/mod.rs
--rw-r--r--   0     1001      123    11327 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/tests/test_lexer.rs
--rw-r--r--   0     1001      123    11008 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/tests/test_lexer_parser.rs
--rw-r--r--   0     1001      123    25784 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/tests/test_parser.rs
--rw-r--r--   0     1001      123     1287 2023-04-20 15:16:45.000000 turnip_text-0.0.1/src/util.rs
--rw-r--r--   0     1001      123     9901 2023-04-20 15:17:30.000000 turnip_text-0.0.1/Cargo.lock
--rw-r--r--   0        0        0     5120 1970-01-01 00:00:00.000000 turnip_text-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 turnip_text-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      123      202 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.cargo/config.toml
+-rw-r--r--   0     1001      123     2745 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.github/workflows/CI.yaml
+-rw-r--r--   0     1001      123       73 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.gitignore
+-rw-r--r--   0     1001      123      734 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.vscode/settings.json
+-rw-r--r--   0     1001      123    10847 2023-06-21 21:13:30.000000 turnip_text-0.0.2/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-21 21:13:30.000000 turnip_text-0.0.2/LICENSE-MIT
+-rw-r--r--   0     1001      123     4391 2023-06-21 21:13:30.000000 turnip_text-0.0.2/README.md
+-rw-r--r--   0     1001      123       10 2023-06-21 21:13:38.000000 turnip_text-0.0.2/dist/turnip_text-0.0.2.tar.gz
+-rw-r--r--   0     1001      123      858 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/experiment.pytext
+-rw-r--r--   0     1001      123     2503 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/phdprop.py
+-rw-r--r--   0     1001      123    21583 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/phdprop.ttxt
+-rw-r--r--   0     1001      123     6171 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/asciidoctor.md
+-rw-r--r--   0     1001      123        0 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/docbook.md
+-rw-r--r--   0     1001      123      113 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/latex.md
+-rw-r--r--   0     1001      123      135 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/restructuredtext.md
+-rw-r--r--   0     1001      123       22 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/sphinx.md
+-rw-r--r--   0     1001      123    10973 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/code_syntax.md
+-rw-r--r--   0     1001      123    10166 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/content_v_formatting.md
+-rw-r--r--   0     1001      123      188 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/goals.md
+-rw-r--r--   0     1001      123     2476 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/opinionated_text.md
+-rw-r--r--   0     1001      123     2151 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/pandoc.md
+-rw-r--r--   0     1001      123      768 2023-06-21 21:13:30.000000 turnip_text-0.0.2/pyproject.toml
+-rw-r--r--   0     1001      123      857 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/__init__.py
+-rw-r--r--   0     1001      123     2267 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/helpers.py
+-rw-r--r--   0     1001      123        0 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/py.typed
+-rw-r--r--   0     1001      123     9465 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/__init__.py
+-rw-r--r--   0     1001      123     2921 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/dictify.py
+-rw-r--r--   0     1001      123       31 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/__init__.py
+-rw-r--r--   0     1001      123     1432 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/base.py
+-rw-r--r--   0     1001      123    11656 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/plugins.py
+-rw-r--r--   0     1001      123       35 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/__init__.py
+-rw-r--r--   0     1001      123     1431 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/base.py
+-rw-r--r--   0     1001      123    16642 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/plugins.py
+-rw-r--r--   0     1001      123     2802 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/std_plugins.py
+-rw-r--r--   0     1001      123     1767 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/turnip_text.pyi
+-rw-r--r--   0     1001      123    11510 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/cli.rs
+-rw-r--r--   0     1001      123    19518 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lexer.rs
+-rw-r--r--   0     1001      123     1905 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lexer_charofs_row_col.rs
+-rw-r--r--   0     1001      123      102 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      123    11860 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interop.rs
+-rw-r--r--   0     1001      123     3877 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/eval_bracket.rs
+-rw-r--r--   0     1001      123    24158 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/mod.rs
+-rw-r--r--   0     1001      123    27965 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/para.rs
+-rw-r--r--   0     1001      123      943 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/mod.rs
+-rw-r--r--   0     1001      123     2815 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/typeclass.rs
+-rw-r--r--   0     1001      123      502 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/mod.rs
+-rw-r--r--   0     1001      123    11327 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_lexer.rs
+-rw-r--r--   0     1001      123    11105 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_lexer_parser.rs
+-rw-r--r--   0     1001      123    29870 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_parser.rs
+-rw-r--r--   0     1001      123     1287 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/util.rs
+-rw-r--r--   0     1001      123     9901 2023-06-21 21:13:30.000000 turnip_text-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 turnip_text-0.0.2/PKG-INFO
```

### Comparing `turnip_text-0.0.1/Cargo.toml` & `turnip_text-0.0.2/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "turnip_text"
-version = "0.0.1"
+version = "0.0.2"
 description = "Document description language that allows embedded Python to describe document structure"
 license = "MIT OR Apache-2.0"
 authors = ["Samuel Stark"]
 edition = "2021"
 
 # "cdylib" is necessary to produce a shared library for Python to import from.
 #
```

### Comparing `turnip_text-0.0.1/.github/workflows/CI.yaml` & `turnip_text-0.0.2/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/.vscode/settings.json` & `turnip_text-0.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/LICENSE-APACHE` & `turnip_text-0.0.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/LICENSE-MIT` & `turnip_text-0.0.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/README.md` & `turnip_text-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/examples/experiment.pytext` & `turnip_text-0.0.2/examples/experiment.pytext`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/examples/phdprop.py` & `turnip_text-0.0.2/examples/phdprop.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/examples/phdprop.ttxt` & `turnip_text-0.0.2/examples/phdprop.ttxt`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/notes/analysis/asciidoctor.md` & `turnip_text-0.0.2/notes/analysis/asciidoctor.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/notes/code_syntax.md` & `turnip_text-0.0.2/notes/code_syntax.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Code-in-text
 
+## TODO
+- DONE Allow scopeless eval-brackets at the starts of paragraphs to return things fitting Block and inject them directly into the document. (This behaviour already works for Inline)
+  - NOTDONE Don't allow subsequent text to start a new paragraph - e.g. `[block_expr] some extra text` shouldn't be valid
+- DONE Allow scopeless eval-brackets to return None and do no emitting
+- DONE Support assignment and recall `[x=5] \n\n [UnescapedText(x)]` -> "5"
+- DONE Better raw-scope-owning behaviour: maybe a raw-scope-owner is just something with a function that takes str? and can return either Block or Inline, and the parser adapts to this? (See above)
+- Add a context variable to all(?) plugin functions, so they can call out to other functions without knowing
+
 ## Current syntax
 
 Code exists in two contexts: block-level and inline-level.
 If an eval-bracket `[]` is opened outside of a paragraph, the contents are evaluated and two checks are performed:
   - if the result fits the `BlockScopeOwner` typeclass, it is expected that the eval brackets will be followed by a block scope (opened with squiggly brace + newline). The eval-result will be called with the contents of that scope (TODO when the block scope is closed), and *that* result will be `render()`-ed in the finalization phase.
   
   ```
@@ -13,24 +21,24 @@
     Paragraph two!
   }
 
   =>
   
   test_block_owner.render_block([Paragraph("Paragraph one!"), Paragraph("Paragraph two!")])
   ```
-  - if the result fits the `InlineScopeOwner` typeclass, it is treated as the start of a new paragraph. it is expected the eval brackets will be followed by an inline scope (opened with squiggly brace w/out newline). The eval-result will be called with the contents of that scope (TODO when the inline scope is closed), and *that* result will be `render()`-ed in the finalization phase.
+  - if the result fits the `InlineScopeOwner` typeclass, it is treated as the start of a new paragraph. it is expected the eval brackets will be followed by an inline scope (opened with squiggly brace w/out newline). The eval-result will be called with the contents of that scope when the inline scope is closed, and *that* result will be `render()`-ed in the finalization phase.
   
   ```
   [test_inline]{inline text to annotate}
 
   =>
 
   test_inline.render_inline(["inline text to annotate"])
   ```
-  - otherwise the result is treated as the start of a new paragraph. The python object is placed directly into the sentence, and will be stringified in the finalization phase.
+  - otherwise the result is treated as the start of a new paragraph. The python object is placed directly into the sentence, and will be stringified in the finalization phase. (TODO this isn't the case anymore, now it's rejected because it isn't Inline. Need type coersion for this)
 
   ```
   [5+7]
 
   =>
 
   str(12)
@@ -157,14 +165,15 @@
     - `[add_float(...)]` shouldn't emit anything text immediately
 4. Document structure
     - `[section(r"The First Section")]`
     - `[section(r"The First Section", label="sec:first")]`
       - This mutates global state (a list of labels?) by adding "sec:first"
 5. DEBATE: Are there compelling use cases for assigning to variables inside eval-brackets?
     - for now, no
+       - YES FOR SIMPLE MACROS (hindsight)
     - What would `[x = 5]` emit? Python REPL doesn't emit any text
 6. Affecting eval-brackets within a sub-scope
     - e.g. inside `[math]` in Markdown/MathJax, most formatting macros should probably be disabled
     - for now, just use raw text mode
     - other example: inside `[enumerate]`, only `[item]`s can be allowed at the top level?
       - Don't try to solve this here!! Python has a type system, don't be afraid to embed text inside Python code and eval-brackets
 
@@ -183,7 +192,13 @@
 - a tree structure is very nice
   - until now I was envisioning that Rust, after processing all text, would have a list of root objects (which could be Python objects that have within them children and a tree structure)
   - Would we want rust to have a tree structure too?
 - Was previously struggling with how to restrict certain things from happening within scopes
   - i.e. inside `[math]` you can't have `[code]`, or inside `[list] [item]` you can't have `[section]`
   - enforce this by classes?
     - i.e. "`[code]` format is inline, math mode disables other inline formatting" or "`[section]` is only allowed at the top level of `[chapter]`"
+
+# Python Plugin Infrastructure
+
+Goals:
+1. Need a "context" function for composable plugins
+  - e.g. `ctx.bold @ ctx.color("red") @ "TODO: Do something"`
```

### Comparing `turnip_text-0.0.1/notes/content_v_formatting.md` & `turnip_text-0.0.2/notes/content_v_formatting.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/notes/opinionated_text.md` & `turnip_text-0.0.2/notes/opinionated_text.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/pyproject.toml` & `turnip_text-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "turnip_text"
-version = "0.0.1"
+version = "0.0.2"
 description = "Document description language that allows embedded Python to describe document structure"
 license = { text = "MIT OR Apache-2.0" }
 readme = "README.md"
 authors = [{ name = "Samuel Stark", email = "popgoestoast@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -16,15 +16,16 @@
 
 [project.optional-dependencies]
 typing = ["mypy"]
 fmt = ["black"]
 
 [tool.maturin]
 python-source = "python"
+module-name = "turnip_text._native"
 
 [tool.mypy]
 
 [tool.black]
 
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
```

### Comparing `turnip_text-0.0.1/python/turnip_text/__init__.py` & `turnip_text-0.0.2/python/turnip_text/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import Protocol, runtime_checkable
+from typing import Optional, Protocol, Union, runtime_checkable
 
-from .turnip_text import (  # type: ignore
+from ._native import (  # type: ignore
     BlockScope,
     InlineScope,
     Paragraph,
+    RawText,
     Sentence,
     UnescapedText,
 )
-from .turnip_text import parse_file as parse_file_native  # type: ignore
+from ._native import parse_file as parse_file_native  # type: ignore
+from ._native import parse_str as parse_str_native  # type: ignore
 
 
 class Inline(Protocol):
     is_inline: bool = True
 
 
 @runtime_checkable
 class Block(Protocol):
     is_block: bool = True
 
 
 @runtime_checkable
 class BlockScopeBuilder(Protocol):
-    def build_from_blocks(self, bs: BlockScope) -> Block:
+    def build_from_blocks(self, bs: BlockScope) -> Optional[Block]:
         ...
 
 
 @runtime_checkable
 class InlineScopeBuilder(Protocol):
     def build_from_inlines(self, inls: InlineScope) -> Inline:
         ...
 
 
 @runtime_checkable
 class RawScopeBuilder(Protocol):
-    def build_from_raw(self, raw: str) -> Inline:
+    def build_from_raw(self, raw: str) -> Union[Inline, Block]:
         ...
```

### Comparing `turnip_text-0.0.1/python/turnip_text/helpers.py` & `turnip_text-0.0.2/python/turnip_text/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, List
+from typing import Any, Callable, List, Optional
 
 from turnip_text import (
     Block,
     BlockScope,
     BlockScopeBuilder,
     Inline,
     InlineScope,
@@ -27,20 +27,20 @@
     ```!text
     [block(name="greg")]{
     The contents of greg
     }
     ```
     """
 
-    func: Callable[[BlockScope], Block]
+    func: Callable[[BlockScope], Optional[Block]]
 
-    def __init__(self, func: Callable[[BlockScope], Block]) -> None:
+    def __init__(self, func: Callable[[BlockScope], Optional[Block]]) -> None:
         self.func = func
 
-    def build_from_blocks(self, b: BlockScope) -> Block:
+    def build_from_blocks(self, b: BlockScope) -> Optional[Block]:
         return self.func(b)
 
 
 class inline_scope_builder(InlineScopeBuilder):
     """
     Decorator which ensures functions fit the InlineScopeBuilder typeclass
```

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/__init__.py` & `turnip_text-0.0.2/python/turnip_text/renderers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,25 @@
     Iterator,
     List,
     Tuple,
     Type,
     TypeVar,
 )
 
-from turnip_text import Block, BlockScope, Inline, parse_file_native
+from turnip_text import (
+    Block,
+    BlockScope,
+    Inline,
+    InlineScope,
+    Paragraph,
+    Sentence,
+    UnescapedText,
+    parse_file_native,
+)
 from turnip_text.renderers.dictify import dictify
-from turnip_text.turnip_text import InlineScope, Paragraph, Sentence, UnescapedText
 
 T = TypeVar("T")
 CustomRenderFunc = Tuple[Type[T], Callable[["Renderer", T], str]]
 
 
 class TypeToRenderMap(Generic[T]):
     _handlers: Dict[Type[T], Callable[["Renderer", T], str]]
```

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/dictify.py` & `turnip_text-0.0.2/python/turnip_text/renderers/dictify.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/latex/base.py` & `turnip_text-0.0.2/python/turnip_text/renderers/latex/base.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/latex/plugins.py` & `turnip_text-0.0.2/python/turnip_text/renderers/latex/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,21 @@
 @dataclass(frozen=True)
 class Citation(Inline):
     # List of (label, note?)
     labels: List[CiteKeyWithOptionNote]
 
 
 @dataclass(frozen=True)
-class Url(Inline):
+class NamedUrl(Inline, InlineScopeBuilder):
     url: str
+    name: Optional[InlineScope] = None
+
+    def build_from_inlines(self, inls: InlineScope) -> Inline:
+        assert self.name is None
+        return NamedUrl(self.url, inls)
 
 
 @dataclass(frozen=True)
 class DisplayList(Block):
     # TODO allow nested lists
     # items: List[Union[BlockNode, List]]
     items: List["DisplayListItem"]
@@ -160,28 +165,36 @@
     def footnote_text(self, label: str) -> BlockScopeBuilder:
         # Return a callable which is invoked with the contents of the following inline scope
         # Example usage:
         # [footnote_text("label")]{text}
         # equivalent to
         # [footnote_text("label")(r"text")]
         @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Block:
+        def handle_block_contents(contents: BlockScope) -> Optional[Block]:
             self._footnotes[label] = contents
             return None
 
         return handle_block_contents
 
 
 class LatexSectionPlugin(RendererPlugin, SectionPluginInterface):
+    _pagebreak_before: List[str]
+
+    def __init__(self, pagebreak_before: List[str] = []) -> None:
+        super().__init__()
+        self._pagebreak_before = pagebreak_before
+
     def _block_handlers(self) -> Iterable[CustomRenderFunc]:
         return ((HeadedBlock, self._render_headed_block),)
 
     def _render_headed_block(self, renderer: Renderer, block: HeadedBlock) -> str:
         header = f"\\{block.latex_name}"  # i.e. r"\section"
-        if block.num:
+        if block.latex_name in self._pagebreak_before:
+            header = "\\pagebreak\n" + header
+        if not block.num:
             header += "*"
         escaped_name = renderer.render_unescapedtext(block.name)
         header += f"{{{escaped_name}}}"  # i.e. r"\section*" + "{Section Name}"
         if block.label:
             header += f"\\label{{{block.label}}}"  # i.e. r"\section*{Section Name}" + r"\label{block_label}"
         return f"{header}\n\n" + renderer.render_blockscope(block.contents)
 
@@ -227,30 +240,41 @@
                 num=num,
                 contents=contents,
             )
 
         return handle_block_contents
 
 
+@inline_scope_builder
+def emph_builder(items: InlineScope) -> Inline:
+    return Formatted("emph", items)
+
+
+@inline_scope_builder
+def italic_builder(items: InlineScope) -> Inline:
+    return Formatted("textit", items)
+
+
+@inline_scope_builder
+def bold_builder(items: InlineScope) -> Inline:
+    return Formatted("textbf", items)
+
+
 class LatexFormatPlugin(RendererPlugin, FormatPluginInterface):
     def _inline_handlers(self) -> Iterable[CustomRenderFunc]:
         return ((Formatted, self._render_formatted),)
 
     def _render_formatted(self, renderer: Renderer, item: Formatted) -> str:
         data = f"\\{item.format_type}{{"
         data += renderer.render_inlinescope(item.items)
         return data + "}"
 
-    @dictify_pure_property
-    def emph(self) -> InlineScopeBuilder:
-        @inline_scope_builder
-        def emph_builder(items: InlineScope) -> Inline:
-            return Formatted("emph", items)
-
-        return emph_builder
+    emph = emph_builder
+    italic = italic_builder
+    bold = bold_builder
 
     OPEN_DQUOTE = RawLatex("``")
     CLOS_DQUOTE = RawLatex("''")
 
     @dictify_pure_property
     def enquote(self) -> InlineScopeBuilder:
         @inline_scope_builder
@@ -277,15 +301,16 @@
         data += renderer.PARAGRAPH_SEP.join(
             renderer.render_block(i) for i in list.items
         )
         return data + f"\n\\end{{{list.mode}}}"
 
     def _render_list_item(self, renderer: Renderer, list_item: DisplayListItem) -> str:
         # TODO indents!
-        return "\\item " + renderer.render_block(list_item.item)
+        # Put {} after \item so square brackets at the start of render_block don't get swallowed as arguments
+        return "\\item{} " + renderer.render_block(list_item.item)
 
     @dictify_pure_property
     def enumerate(self) -> BlockScopeBuilder:
         @block_scope_builder
         def enumerate_builder(contents: BlockScope) -> Block:
             items = list(contents)
             if any(not isinstance(x, DisplayListItem) for x in items):
@@ -320,15 +345,20 @@
         return item_builder
 
 
 class LatexUrlPlugin(RendererPlugin):
     # TODO add dependency on hyperref!!
 
     def _inline_handlers(self) -> Iterable[CustomRenderFunc]:
-        return ((Url, self._render_url),)
+        return ((NamedUrl, self._render_url),)
 
-    def _render_url(self, renderer: Renderer, url: Url) -> str:
-        escaped_url = url.url.replace("#", "\\#")
-        return f"\\url{{{escaped_url}}}"
+    def _render_url(self, renderer: Renderer, url: NamedUrl) -> str:
+        if url.name is None:
+            return f"\\url{{{url.url}}}"
+        else:
+            escaped_url_name = renderer.render_inlinescope(url.name)
+            return f"\\href{{{url.url}}}{{{escaped_url_name}}}"
 
-    def url(self, url: str) -> Inline:
-        return Url(url)
+    def url(self, url: str, name: Optional[str] = None) -> Inline:
+        return NamedUrl(
+            url, name=InlineScope([UnescapedText(name)]) if name is not None else None
+        )
```

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/markdown/base.py` & `turnip_text-0.0.2/python/turnip_text/renderers/markdown/base.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/markdown/plugins.py` & `turnip_text-0.0.2/python/turnip_text/renderers/markdown/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,21 @@
 @dataclass(frozen=True)
 class Citation(Inline):
     # List of (label, note?)
     labels: List[CiteKeyWithOptionNote]
 
 
 @dataclass(frozen=True)
-class Url(Inline):
+class NamedUrl(Inline, InlineScopeBuilder):
     url: str
+    name: Optional[InlineScope] = None
+
+    def build_from_inlines(self, inls: InlineScope) -> Inline:
+        assert self.name is None
+        return NamedUrl(self.url, inls)
 
 
 @dataclass(frozen=True)
 class DisplayList(Block):
     # TODO allow nested lists
     # items: List[Union[BlockNode, List]]
     items: List["DisplayListItem"]
@@ -249,15 +254,15 @@
     def footnote_text(self, label: str) -> BlockScopeBuilder:
         # Return a callable which is invoked with the contents of the following inline scope
         # Example usage:
         # [footnote_text("label")]{text}
         # equivalent to
         # [footnote_text("label")(r"text")]
         @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Block:
+        def handle_block_contents(contents: BlockScope) -> Optional[Block]:
             self._footnotes[label] = contents
             return None
 
         return handle_block_contents
 
 
 class MarkdownSectionPlugin(RendererPlugin, SectionPluginInterface):
@@ -355,33 +360,44 @@
                 num=section_num,
                 contents=contents,
             )
 
         return handle_block_contents
 
 
+@inline_scope_builder
+def emph_builder(items: InlineScope) -> Inline:
+    return italic_builder.build_from_inlines(items)
+
+
+@inline_scope_builder
+def italic_builder(items: InlineScope) -> Inline:
+    # Use single underscore for italics, double asterisks for bold, double underscore for underlining?
+    return Formatted("_", items)
+
+
+@inline_scope_builder
+def bold_builder(items: InlineScope) -> Inline:
+    return Formatted("**", items)
+
+
 class MarkdownFormatPlugin(RendererPlugin, FormatPluginInterface):
     def _inline_handlers(self) -> Iterable[CustomRenderFunc]:
         return ((Formatted, self._render_formatted),)
 
     def _render_formatted(self, renderer: Renderer, item: Formatted) -> str:
         return (
             item.format_type
             + renderer.render_inlinescope(item.items)
             + item.format_type
         )
 
-    @dictify_pure_property
-    def emph(self) -> InlineScopeBuilder:
-        @inline_scope_builder
-        def emph_builder(items: InlineScope) -> Inline:
-            # Use single underscore for italics, double asterisks for bold, double underscore for underlining?
-            return Formatted("_", items)
-
-        return emph_builder
+    emph = emph_builder
+    italic = italic_builder
+    bold = bold_builder
 
     DQUOTE = RawMarkdown('"')
 
     @dictify_pure_property
     def enquote(self) -> InlineScopeBuilder:
         @inline_scope_builder
         def enquote_builder(items: InlineScope) -> Inline:
@@ -390,29 +406,32 @@
                 + list(items)
                 + [MarkdownFormatPlugin.DQUOTE]
             )
 
         return enquote_builder
 
 
+def indent_item(prefix, item_rendering):
+    return prefix + item_rendering.replace("\n", "\n" + " " * len(prefix))
+
+
 class MarkdownListPlugin(RendererPlugin):
     def _block_handlers(self) -> Iterable[CustomRenderFunc]:
         return ((DisplayList, self._render_list),)
 
     def _render_list(self, renderer: Renderer, list: DisplayList) -> str:
-        # TODO indents!
-        # If list items are multiline, right now all lines after the first will NOT be indented and thus not counted as part of the list item.
+        # TODO better way of indenting
         if list.numbered:
             return renderer.SENTENCE_SEP.join(
-                f"{idx+1}. " + renderer.render_block(item.contents)
+                indent_item(f"{idx+1}. ", renderer.render_block(item.contents))
                 for idx, item in enumerate(list.items)
             )
         else:
             return renderer.SENTENCE_SEP.join(
-                f"- " + renderer.render_block(item.contents)
+                indent_item("- ", renderer.render_block(item.contents))
                 for idx, item in enumerate(list.items)
             )
 
     @dictify_pure_property
     def enumerate(self) -> BlockScopeBuilder:
         @block_scope_builder
         def enumerate_builder(contents: BlockScope) -> Block:
@@ -445,16 +464,21 @@
             return DisplayListItem(block_scope)
 
         return item_builder
 
 
 class MarkdownUrlPlugin(RendererPlugin):
     def _inline_handlers(self) -> Iterable[CustomRenderFunc]:
-        return ((Url, self._render_url),)
+        return ((NamedUrl, self._render_url),)
 
-    def _render_url(self, renderer: Renderer, url: Url) -> str:
-        # Set the "name" of the URL to the text of the URL - escaped so it can be read as normal markdown
-        escaped_url_text = renderer.render_unescapedtext(UnescapedText(url.url))
-        return f"[{escaped_url_text}]({url.url})"
+    def _render_url(self, renderer: Renderer, url: NamedUrl) -> str:
+        if url.name is None:
+            # Set the "name" of the URL to the text of the URL - escaped so it can be read as normal markdown
+            escaped_url_name = renderer.render_unescapedtext(UnescapedText(url.url))
+        else:
+            escaped_url_name = renderer.render_inlinescope(url.name)
+        return f"[{escaped_url_name}]({url.url})"
 
-    def url(self, url: str) -> Inline:
-        return Url(url)
+    def url(self, url: str, name: Optional[str] = None) -> Inline:
+        return NamedUrl(
+            url, name=InlineScope([UnescapedText(name)]) if name is not None else None
+        )
```

### Comparing `turnip_text-0.0.1/python/turnip_text/renderers/std_plugins.py` & `turnip_text-0.0.2/python/turnip_text/renderers/std_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     def subsubsection(
         self, name: str, label: Optional[str] = None, numbered: bool = False
     ) -> BlockScopeBuilder:
         ...
 
 
 class FormatPluginInterface(Protocol):
-    @dictify_pure_property
-    def emph(self) -> InlineScopeBuilder:
-        ...
+    emph: InlineScopeBuilder
+    italic: InlineScopeBuilder
+    bold: InlineScopeBuilder
 
     @dictify_pure_property
     def enquote(self) -> InlineScopeBuilder:
         ...
 
 
 class ListPluginInterface(Protocol):
```

### Comparing `turnip_text-0.0.1/python/turnip_text/turnip_text.pyi` & `turnip_text-0.0.2/python/turnip_text/turnip_text.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 from typing import Iterator, List, Optional, Protocol, runtime_checkable
 
-from turnip_text import Block, Inline
+from turnip_text._native import Block, Inline
 
 class UnescapedText(Inline):
     def __init__(self, text: str) -> None: ...
     @property
     def text(self) -> str: ...
 
 class RawText(Inline):
```

### Comparing `turnip_text-0.0.1/src/cli.rs` & `turnip_text-0.0.2/src/cli.rs`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,28 @@
             BlockOwnerCodeMidPara { code_span } => snippet_from_parse_span(
                 file_src,
                 "A `BlockScopeOwner` was returned by inline code inside a paragraph",
                 "BlockScopeOwner returned by this",
                 AnnotationType::Error,
                 code_span,
             ),
+            BlockCodeMidPara { code_span } => snippet_from_parse_span(
+                file_src,
+                "A `Block` was returned by inline code inside a paragraph",
+                "Block returned by this",
+                AnnotationType::Error,
+                code_span,
+            ),
+            BlockCodeFromRawScopeMidPara { code_span } => snippet_from_parse_span(
+                file_src,
+                "A `Block` was returned after building a raw scope inside a paragraph",
+                "RawScopeBuilder returned by this",
+                AnnotationType::Error,
+                code_span,
+            ),
             SentenceBreakInInlineScope { scope_start } => snippet_from_parse_span(
                 file_src, 
                 "Paragraph break found inside an inline scope",
                 "Inline scope opened here",
                 AnnotationType::Error,
                 scope_start
             ),
```

### Comparing `turnip_text-0.0.1/src/lexer.rs` & `turnip_text-0.0.2/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/src/lexer_charofs_row_col.rs` & `turnip_text-0.0.2/src/lexer_charofs_row_col.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/src/python/interop.rs` & `turnip_text-0.0.2/src/python/interop.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     prelude::*,
     types::{PyDict, PyIterator, PyList, PyString},
 };
 
 use super::typeclass::{PyInstanceList, PyTcRef, PyTypeclass, PyTypeclassList};
 
 #[pymodule]
+#[pyo3(name="_native")]
 pub fn turnip_text(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(parse_file, m)?)?;
     m.add_function(wrap_pyfunction!(parse_str, m)?)?;
 
     // Primitives
     m.add_class::<UnescapedText>()?;
     m.add_class::<RawText>()?;
@@ -91,14 +92,29 @@
             obj.getattr(attr_name)?.is_true()
         } else {
             Ok(false)
         }
     }
 }
 
+/// Typeclass used internally for things that can be emitted directly from eval-brackets:
+/// i.e. an Inline or a Block.
+/// Must be one or the other - doesn't make sense for something to be both, because it doesn't know what context it would be rendered in.
+#[derive(Debug, Clone)]
+pub struct InlineXorBlock {}
+impl PyTypeclass for InlineXorBlock {
+    const NAME: &'static str = "Inline XOR Block (not both)";
+
+    fn fits_typeclass(obj: &PyAny) -> PyResult<bool> {
+        let is_inline = Inline::fits_typeclass(obj)?;
+        let is_block = Block::fits_typeclass(obj)?;
+        Ok(is_inline ^ is_block)
+    }
+}
+
 /// Typeclass representing the "builder" of a block scope, which may modify how that scope is rendered.
 ///
 /// Requires a method
 /// ```python
 /// def build_from_blocks(self, blocks: BlockScope) -> Block: ...
 /// ```
 #[derive(Debug, Clone)]
@@ -107,20 +123,24 @@
     fn marker_func_name(py: Python<'_>) -> &PyString {
         intern!(py, "build_from_blocks")
     }
     pub fn call_build_from_blocks<'py>(
         py: Python<'py>,
         builder: PyTcRef<Self>,
         blocks: Py<BlockScope>,
-    ) -> PyResult<PyTcRef<Block>> {
+    ) -> PyResult<Option<PyTcRef<Block>>> {
         let output = builder
             .as_ref(py)
             .getattr(Self::marker_func_name(py))?
             .call1((blocks,))?;
-        PyTcRef::of(output)
+        if output.is_none() {
+            Ok(None)
+        } else {
+            Ok(Some(PyTcRef::of(output)?))
+        }
     }
 }
 impl PyTypeclass for BlockScopeBuilder {
     const NAME: &'static str = "BlockScopeBuilder";
 
     fn fits_typeclass(obj: &PyAny) -> PyResult<bool> {
         obj.hasattr(Self::marker_func_name(obj.py()))
@@ -167,20 +187,20 @@
 /// ```
 #[derive(Debug, Clone)]
 pub struct RawScopeBuilder {}
 impl RawScopeBuilder {
     fn marker_func_name(py: Python<'_>) -> &PyString {
         intern!(py, "build_from_raw")
     }
-    /// Calls builder.build_from_raw(raw)  
+    /// Calls builder.build_from_raw(raw), could be inline or block 
     pub fn call_build_from_raw<'py>(
         py: Python<'py>,
-        builder: PyTcRef<Self>,
-        raw: String,
-    ) -> PyResult<PyTcRef<Inline>> {
+        builder: &PyTcRef<Self>,
+        raw: &String,
+    ) -> PyResult<PyTcRef<InlineXorBlock>> {
         let output = builder
             .as_ref(py)
             .getattr(Self::marker_func_name(py))?
             .call1((raw,))?;
         PyTcRef::of(output)
     }
 }
```

### Comparing `turnip_text-0.0.1/src/python/interp/mod.rs` & `turnip_text-0.0.2/src/python/interp/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -47,111 +47,131 @@
     ReadyForNewBlock,
     /// Building a paragraph block node, which will be added to the parent block node once complete.
     ///
     /// Transitions to [Self::ReadyForNewBlock] after finishing the paragraph
     WritingPara(InterpParaState),
     /// Building Python-code to evaluate at the block level, outside a paragraph
     ///
-    /// Transitions to [Self::AttachingBlockLevelCode] once finished
-    BuildingBlockLevelCode {
+    /// Transitions to [Self::AttachingBlockLevelCode] or [Self::ReadyForNewBlock] once finished
+    BuildingCode {
         code: String,
         code_start: ParseSpan,
         expected_close_len: usize,
     },
+    /// When building raw text initiated at the block level, owned by a RawScopeBuilder, which may return Inline or Block content
+    BuildingRawText {
+        builder: PyTcRef<RawScopeBuilder>,
+        text: String,
+        builder_span: ParseSpan,
+        expected_n_hashes: usize,
+    },
 }
 
 #[derive(Debug)]
 struct InterpCommentState {
     comment_start: ParseSpan,
 }
 
 #[derive(Debug)]
 struct InterpBlockScopeState {
     builder: Option<PyTcRef<BlockScopeBuilder>>,
     children: Py<BlockScope>,
     scope_start: ParseSpan,
 }
 impl InterpBlockScopeState {
-    fn build_to_block(self, py: Python, scope_end: ParseSpan) -> InterpResult<PyTcRef<Block>> {
+    fn build_to_block(self, py: Python, scope_end: ParseSpan) -> InterpResult<Option<PyTcRef<Block>>> {
         let scope = ParseSpan::new(self.scope_start.start, scope_end.end);
         match self.builder {
             Some(builder) => BlockScopeBuilder::call_build_from_blocks(py, builder, self.children)
                 .err_as_interp(py, scope),
-            None => Ok(PyTcRef::of(self.children.as_ref(py)).expect("Internal error: InterpBlockScopeState::children, a BlockScope, somehow doesn't fit the Block typeclass")),
+            None => Ok(Some(PyTcRef::of(self.children.as_ref(py)).expect("Internal error: InterpBlockScopeState::children, a BlockScope, somehow doesn't fit the Block typeclass"))),
         }
     }
 }
 
 #[derive(Debug)]
 pub(crate) enum InterpBlockTransition {
     /// On encountering a CodeOpen at the start of a line, start gathering block level code
     ///
-    /// - [InterpBlockState::ReadyForNewBlock] -> [InterpBlockState::BuildingBlockLevelCode]
+    /// - [InterpBlockState::ReadyForNewBlock] -> [InterpBlockState::BuildingCode]
     /// - All others invalid
     StartBlockLevelCode(ParseSpan, usize),
 
-    /// Start a paragraph, optionally executing a transition on the paragraph-level state machine
+    /// On executing code that returned None, transition back to waiting for a paragraph
+    /// 
+    /// - [InterpBlockState::BuildingCode] -> [InterpBlockState::ReadyForNewBlock]
+    EmitNone,
+
+    /// On finishing block-level code, if it intends to own a raw scope, start a raw scope.
+    /// 
+    /// - [InterpBlockState::BuildingCode] -> [InterpBlockState::BuildingRawText]
+    StartRawScope(PyTcRef<RawScopeBuilder>, ParseSpan, usize),
+
+    /// Start a paragraph, executing a transition on the paragraph-level state machine
     ///
     /// - [InterpBlockState::ReadyForNewBlock] -> [InterpBlockState::WritingPara]
-    /// - [InterpBlockState::BuildingBlockLevelCode] -> [InterpBlockState::WritingPara]
-    /// TODO dear god stop using Option here, its so verbose and actually unnecessary
-    StartParagraph(Option<InterpParaTransition>),
+    /// - [InterpBlockState::BuildingCode] -> [InterpBlockState::WritingPara]
+    /// - [InterpBlockState::BuildingRawText] -> [InterpBlockState::WritingPara]
+    StartParagraph(InterpParaTransition),
 
     /// On encountering a paragraph break (a blank line), add the paragraph to the document
     ///
     /// - [InterpBlockState::WritingPara] -> [InterpBlockState::ReadyForNewBlock]
     EndParagraph,
 
     /// On encountering a block scope close inside a paragraph,
     /// add the paragraph and close the topmost scope
     ///
     /// - [InterpBlockState::WritingPara] -> [InterpBlockState::ReadyForNewBlock]
     EndParagraphAndPopBlock(ParseSpan),
 
-    /// On encountering block content (i.e. a BlockScopeOpen optionally preceded by a Python scope owner),
+    /// On encountering a block scope owner (i.e. a BlockScopeOpen optionally preceded by a Python scope owner),
     /// push a block scope onto the current stack
     ///
     /// - [InterpBlockState::ReadyForNewBlock] -> [InterpBlockState::ReadyForNewBlock]
-    /// - [InterpBlockState::BuildingBlockLevelCode] -> [InterpBlockState::ReadyForNewBlock]
-    PushBlock(Option<PyTcRef<BlockScopeBuilder>>, ParseSpan),
+    /// - [InterpBlockState::BuildingCode] -> [InterpBlockState::ReadyForNewBlock]
+    PushBlockScope(Option<PyTcRef<BlockScopeBuilder>>, ParseSpan),
+
+    /// If an eval-bracket emits a Block directly, or a raw scope owner takes raw text and produces Block, push it onto the stack
+    /// 
+    /// - [InterpBlockState::BuildingCode] -> [InterpBlockState::ReadyForNewBlock]
+    /// - [InterpBlockState::BuildingRawText] -> [InterpBlockState::ReadyForNewBlock]
+    PushBlock(PyTcRef<Block>),
 
     /// On encountering a scope close, pop the current block from the scope
     ///
     /// - [InterpBlockState::ReadyForNewBlock] -> [InterpBlockState::ReadyForNewBlock]
-    PopBlock(ParseSpan),
+    PopBlockScope(ParseSpan),
 }
 
 #[derive(Debug)]
 pub(crate) enum InterpSpecialTransition {
     /// On encountering a comment starter, go into comment mode
     StartComment(ParseSpan),
 
     /// Leave comment mode
     EndComment,
 }
 
 #[derive(Debug)]
 pub(crate) enum InlineNodeToCreate {
     UnescapedText(String),
-    RawText(Option<PyTcRef<RawScopeBuilder>>, String),
+    RawText(String),
     PythonObject(PyTcRef<Inline>),
 }
 impl InlineNodeToCreate {
     fn to_py_intern(self, py: Python) -> PyResult<PyTcRef<Inline>> {
         match self {
             InlineNodeToCreate::UnescapedText(s) => {
                 let unescaped_text = Py::new(py, UnescapedText::new_rs(py, s.as_str()))?;
                 PyTcRef::of(unescaped_text.as_ref(py))
             }
-            InlineNodeToCreate::RawText(builder, raw) => match builder {
-                Some(builder) => RawScopeBuilder::call_build_from_raw(py, builder, raw),
-                None => {
-                    let raw_text = Py::new(py, RawText::new_rs(py, raw.as_str()))?;
-                    PyTcRef::of(raw_text.as_ref(py))
-                }
+            InlineNodeToCreate::RawText(raw) => {
+                let raw_text = Py::new(py, RawText::new_rs(py, raw.as_str()))?;
+                PyTcRef::of(raw_text.as_ref(py))
             },
             InlineNodeToCreate::PythonObject(obj) => Ok(obj),
         }
     }
     pub(crate) fn to_py(self, py: Python) -> InterpResult<PyTcRef<Inline>> {
         self.to_py_intern(py).err_as_interp_internal(py)
     }
@@ -172,14 +192,18 @@
     EndedInsideRawScope { raw_scope_start: ParseSpan },
     #[error("File ended inside scope")]
     EndedInsideScope { scope_start: ParseSpan },
     #[error("Block scope encountered mid-line")]
     BlockScopeOpenedMidPara { scope_start: ParseSpan },
     #[error("A Python `BlockScopeOwner` was returned by code inside a paragraph")]
     BlockOwnerCodeMidPara { code_span: ParseSpan },
+    #[error("A Python `Block` was returned by code inside a paragraph")]
+    BlockCodeMidPara { code_span: ParseSpan },
+    #[error("A Python `Block` was returned by a RawScopeBuilder inside a paragraph")]
+    BlockCodeFromRawScopeMidPara { code_span: ParseSpan },
     #[error("Inline scope contained sentence break")]
     SentenceBreakInInlineScope { scope_start: ParseSpan },
     #[error("Inline scope contained paragraph break")]
     ParaBreakInInlineScope {
         scope_start: ParseSpan,
         para_break: ParseSpan,
     },
@@ -245,19 +269,24 @@
         &mut self,
         py: Python<'interp>,
         globals: &'interp PyDict,
     ) -> InterpResult<()> {
         let transitions = match &mut self.block_state {
             InterpBlockState::ReadyForNewBlock => (None, None),
             InterpBlockState::WritingPara(state) => state.finalize(py)?,
-            InterpBlockState::BuildingBlockLevelCode { code_start, .. } => {
+            InterpBlockState::BuildingCode { code_start, .. } => {
                 return Err(InterpError::EndedInsideCode {
                     code_start: *code_start,
                 })
             }
+            InterpBlockState::BuildingRawText { builder_span, .. } => {
+                return Err(InterpError::EndedInsideRawScope {
+                    raw_scope_start: *builder_span, // TODO This is technically wrong but it gets the point across. Should return the raw_scope token start, not the builder start
+                })
+            }
         };
 
         match self.block_stack.pop() {
             // No open blocks on the stack => process the transition
             None => self.handle_transition(py, globals, transitions),
             Some(InterpBlockScopeState { scope_start, .. }) => {
                 return Err(InterpError::EndedInsideScope { scope_start })
@@ -294,36 +323,38 @@
                     Escaped(span, Escapable::Newline) => {
                         return Err(InterpError::EscapedNewlineOutsideParagraph { newline: span })
                     }
 
                     CodeOpen(span, n_hashes) => (Some(StartBlockLevelCode(span, n_hashes)), None),
 
                     // PushBlock with no code managing it
-                    BlockScopeOpen(span) => (Some(PushBlock(None, span)), None),
+                    BlockScopeOpen(span) => (Some(PushBlockScope(None, span)), None),
 
                     // PushInlineScope with no code managing it
                     InlineScopeOpen(span) => (
-                        Some(StartParagraph(Some(InterpParaTransition::PushInlineScope(
+                        Some(StartParagraph(InterpParaTransition::PushInlineScope(
                             None, span,
-                        )))),
+                        ))),
                         None,
                     ),
 
                     // StartRawBlock
+                    // If we start a raw scope directly, with no owner, go into Inline mode.
+                    // Raw text can only be inline content when inserted directly.
                     RawScopeOpen(span, n_hashes) => (
-                        Some(StartParagraph(Some(InterpParaTransition::StartRawScope(
+                        Some(StartParagraph(InterpParaTransition::StartRawScope(
                             None, span, n_hashes,
-                        )))),
+                        ))),
                         None,
                     ),
                     RawScopeClose(span, _) => Err(InterpError::RawScopeCloseOutsideRawScope(span))?,
 
                     // Try a scope close
                     ScopeClose(span) => match self.block_stack.last() {
-                        Some(_) => (Some(PopBlock(span)), None),
+                        Some(_) => (Some(PopBlockScope(span)), None),
                         None => Err(InterpError::ScopeCloseOutsideScope(span))?,
                     },
 
                     // Complain - not in code mode
                     CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span)),
 
                     // Do nothing - we're still ready to receive a new block
@@ -332,25 +363,25 @@
                     Whitespace(_) => (None, None),
 
                     // Enter comment mode
                     Hashes(span, _) => (None, Some(InterpSpecialTransition::StartComment(span))),
 
                     // Normal text - start a new paragraph
                     _ => (
-                        Some(StartParagraph(Some(InterpParaTransition::StartText(
+                        Some(StartParagraph(InterpParaTransition::StartText(
                             tok.stringify_escaped(self.data).into(),
-                        )))),
+                        ))),
                         None,
                     ),
                 }
             }
             InterpBlockState::WritingPara(state) => {
                 state.handle_token(py, globals, tok, self.data)?
             }
-            InterpBlockState::BuildingBlockLevelCode {
+            InterpBlockState::BuildingCode {
                 code,
                 code_start,
                 expected_close_len,
             } => {
                 match handle_code_mode(
                     self.data,
                     tok,
@@ -360,35 +391,53 @@
                     py,
                     globals,
                 )? {
                     Some((res, code_span)) => {
                         use EvalBracketResult::*;
 
                         let block_transition = match res {
-                            Block(b) => PushBlock(Some(b), code_span),
-                            Inline(i) => StartParagraph(Some(
+                            BlockBuilder(b) => PushBlockScope(Some(b), code_span),
+                            InlineBuilder(i) => StartParagraph(
                                 InterpParaTransition::PushInlineScope(Some(i), code_span),
-                            )),
-                            Raw(r, n_hashes) => StartParagraph(Some(
-                                InterpParaTransition::StartRawScope(Some(r), code_span, n_hashes),
-                            )),
-                            Other(s) => {
-                                // TODO If the object is not already Inline, check if it's Block or BlockScopeBuilder or InlineScopeBuilder or RawScopeBuilder, stringify it, then put in an Unescaped box?
-                                StartParagraph(Some(InterpParaTransition::PushInlineContent(
+                            ),
+                            RawBuilder(r, n_hashes) => StartRawScope(r, code_span, n_hashes),
+                            Block(b) => PushBlock(b),
+                            Inline(i) => {
+                                StartParagraph(InterpParaTransition::PushInlineContent(
                                     InlineNodeToCreate::PythonObject(
-                                        PyTcRef::of(s.as_ref(py)).err_as_interp(py, code_span)?,
+                                        i
                                     ),
-                                )))
+                                ))
                             }
+                            PyNone => EmitNone
                         };
                         (Some(block_transition), None)
                     }
                     None => (None, None),
                 }
             }
+            InterpBlockState::BuildingRawText { builder, text, builder_span, expected_n_hashes } => match tok {
+                RawScopeClose(_, n_hashes) if n_hashes == *expected_n_hashes => {
+                    // Make sure the RawScopeBuilder produces something that's either Inline or Block
+                    let to_emit = RawScopeBuilder::call_build_from_raw(py, builder, text).err_as_interp(py, *builder_span)?;
+                    
+                    let to_emit_as_py = to_emit.as_ref(py);
+                    if let Ok(block) = PyTcRef::of(to_emit_as_py) {
+                        (Some(PushBlock(block)), None)
+                    } else if let Ok(inl) = PyTcRef::of(to_emit_as_py) {
+                        (Some(StartParagraph(InterpParaTransition::PushInlineContent(InlineNodeToCreate::PythonObject(inl)))), None)
+                    } else {
+                        unreachable!()
+                    }
+                }
+                _ => {
+                    text.push_str(tok.stringify_raw(self.data));
+                    (None, None)
+                }
+            },
         };
 
         Ok(transition)
     }
 
     /// May recurse if StartParagraph(transition)
     fn handle_transition(
@@ -404,28 +453,28 @@
 
         if let Some(transition) = block_transition {
             use InterpBlockState as S;
             use InterpBlockTransition as T;
 
             let new_block_state = match (&self.block_state, transition) {
                 (S::ReadyForNewBlock, T::StartBlockLevelCode(code_start, expected_close_len)) => {
-                    S::BuildingBlockLevelCode {
+                    S::BuildingCode {
                         code: "".into(),
                         code_start,
                         expected_close_len,
                     }
                 }
 
                 (
-                    S::ReadyForNewBlock | S::BuildingBlockLevelCode { .. },
+                    S::ReadyForNewBlock | S::BuildingCode { .. } | S::BuildingRawText { .. },
                     T::StartParagraph(transition),
                 ) => {
                     let mut para_state = InterpParaState::new(py).err_as_interp_internal(py)?;
                     let (new_block_transition, new_special_transition) =
-                        para_state.handle_transition(py, transition)?;
+                        para_state.handle_transition(py, Some(transition))?;
                     if new_block_transition.is_some() {
                         return Err(InterpError::InternalErr(
                             "An inline transition, initiated with the start of a paragraph, tried to initiate another block transition. This is not allowed and should not be possible.".into()
                         ));
                     }
                     self.handle_transition(py, globals, (None, new_special_transition))?;
                     S::WritingPara(para_state)
@@ -437,40 +486,65 @@
                 (S::WritingPara(para_state), T::EndParagraphAndPopBlock(scope_close_span)) => {
                     // End paragraph i.e. push paragraph onto topmost block
                     self.push_to_topmost_block(py, para_state.para().as_ref(py))?;
                     // Pop block
                     let popped_scope = self.block_stack.pop();
                     match popped_scope {
                         Some(popped_scope) => {
-                            let block = popped_scope.build_to_block(py, scope_close_span)?;
-                            self.push_to_topmost_block(py, block.as_ref(py))?
+                            match popped_scope.build_to_block(py, scope_close_span)? {
+                                Some(block) => self.push_to_topmost_block(py, block.as_ref(py))?,
+                                None => {}
+                            }
                         }
                         None => return Err(InterpError::ScopeCloseOutsideScope(scope_close_span)),
                     }
                     S::ReadyForNewBlock
                 }
 
                 (
-                    S::ReadyForNewBlock | S::BuildingBlockLevelCode { .. },
-                    T::PushBlock(builder, scope_start),
+                    S::BuildingCode { .. } | S::BuildingRawText { .. },
+                    T::PushBlock(b)
+                ) => {
+                    self.push_to_topmost_block(py, b.as_ref(py))?;
+                    S::ReadyForNewBlock
+                }
+
+                (
+                    S::BuildingCode { .. },
+                    T::EmitNone
+                ) => {
+                    S::ReadyForNewBlock
+                }
+                
+                (
+                    S::BuildingCode { .. },
+                    T::StartRawScope(r, builder_span, expected_n_hashes)
+                ) => {
+                    S::BuildingRawText { builder: r, text: "".into(), builder_span, expected_n_hashes }
+                }
+                (
+                    S::ReadyForNewBlock | S::BuildingCode { .. },
+                    T::PushBlockScope(builder, scope_start),
                 ) => {
                     self.block_stack.push(InterpBlockScopeState {
                         builder,
                         children: Py::new(py, BlockScope::new_empty(py))
                             .err_as_interp_internal(py)?,
                         scope_start,
                     });
                     S::ReadyForNewBlock
                 }
-                (S::ReadyForNewBlock, T::PopBlock(scope_close_span)) => {
+                (S::ReadyForNewBlock, T::PopBlockScope(scope_close_span)) => {
                     let popped_scope = self.block_stack.pop();
                     match popped_scope {
                         Some(popped_scope) => {
-                            let block = popped_scope.build_to_block(py, scope_close_span)?;
-                            self.push_to_topmost_block(py, block.as_ref(py))?
+                            match popped_scope.build_to_block(py, scope_close_span)? {
+                                Some(block) => self.push_to_topmost_block(py, block.as_ref(py))?,
+                                None => {}
+                            }
                         }
                         None => return Err(InterpError::ScopeCloseOutsideScope(scope_close_span)),
                     }
                     S::ReadyForNewBlock
                 }
                 (_, transition) => {
                     return Err(InterpError::InternalErr(format!(
@@ -510,74 +584,9 @@
             };
             child_list_ref.borrow_mut(py).push_block(block)
         }
         .err_as_interp_internal(py)
     }
 }
 
-/// If the code is closed, evaluates the result and checks it matches the type of code close:
-/// - [TTToken::CodeCloseOwningBlock] -> [EvalBracketResult::Block]
-/// - [TTToken::CodeCloseOwningInline] -> [EvalBracketResult::Inline]
-/// - [TTToken::CodeCloseOwningRaw] -> [EvalBracketResult::Inline]
-/// - [TTToken::CodeClose] -> [EvalBracketResult::Other]
-fn handle_code_mode(
-    data: &str,
-    tok: TTToken,
-    code: &mut String,
-    code_start: &ParseSpan,
-    expected_close_len: usize,
-    py: Python,
-    globals: &PyDict,
-) -> InterpResult<Option<(EvalBracketResult, ParseSpan)>> {
-    let code_span = match tok {
-        TTToken::CodeClose(close_span, n)
-        | TTToken::CodeCloseOwningBlock(close_span, n)
-        | TTToken::CodeCloseOwningInline(close_span, n)
-        | TTToken::CodeCloseOwningRaw(close_span, n, _)
-            if n == expected_close_len =>
-        {
-            ParseSpan {
-                start: code_start.start,
-                end: close_span.end,
-            }
-        }
-        _ => {
-            // Code blocks use raw stringification to avoid confusion between text written and text entered
-            code.push_str(tok.stringify_raw(data));
-            return Ok(None);
-        }
-    };
-
-    let res = EvalBracketResult::eval_in_correct_ctx(py, globals, code, tok)
-        .err_as_interp(py, code_span)?;
-    Ok(Some((res, code_span)))
-}
-pub enum EvalBracketResult {
-    Block(PyTcRef<BlockScopeBuilder>),
-    Inline(PyTcRef<InlineScopeBuilder>),
-    Raw(PyTcRef<RawScopeBuilder>, usize),
-    Other(PyObject),
-}
-impl EvalBracketResult {
-    pub fn eval_in_correct_ctx(
-        py: Python,
-        globals: &PyDict,
-        code: &str,
-        tok: TTToken,
-    ) -> PyResult<EvalBracketResult> {
-        // Python picks up leading whitespace as an incorrect indent
-        let code = code.trim();
-        let raw_res = py.eval(code, Some(globals), None)?;
-        let res = match tok {
-            TTToken::CodeCloseOwningBlock(_, _) => EvalBracketResult::Block(PyTcRef::of(raw_res)?),
-            TTToken::CodeCloseOwningInline(_, _) => {
-                EvalBracketResult::Inline(PyTcRef::of(raw_res)?)
-            }
-            TTToken::CodeCloseOwningRaw(_, _, n_hashes) => {
-                EvalBracketResult::Raw(PyTcRef::of(raw_res)?, n_hashes)
-            }
-            TTToken::CodeClose(_, _) => EvalBracketResult::Other(raw_res.to_object(py)),
-            _ => unreachable!(),
-        };
-        Ok(res)
-    }
-}
+mod eval_bracket;
+use eval_bracket::{EvalBracketResult, handle_code_mode};
```

### Comparing `turnip_text-0.0.1/src/python/interp/para.rs` & `turnip_text-0.0.2/src/python/interp/para.rs`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,19 @@
     },
     /// When in code mode
     BuildingCode {
         code: String,
         code_start: ParseSpan,
         expected_n_hashes: usize,
     },
-    /// When building raw text, optionally attached to an InlineScopeOwner
+    /// When building raw text, optionally attached to a RawScopeBuilder
     BuildingRawText {
-        owner: Option<PyTcRef<RawScopeBuilder>>,
+        builder: Option<PyTcRef<RawScopeBuilder>>,
         text: String,
+        /// Either the token opening the raw scope, or the code for the builder
         raw_start: ParseSpan,
         expected_n_hashes: usize,
     },
 }
 
 #[derive(Debug)]
 pub(crate) enum InterpParaTransition {
@@ -81,14 +82,19 @@
     /// Break the current sentence within the paragraph.
     /// Finishes the current BuildingText if in progress, and pushes it to the topmost scope (which should be the sentence)
     /// Errors out if inline scopes are currently open - right now inline scopes must be entirely within a sentence.
     ///
     /// - [InterpSentenceState::MidSentence] -> [InterpSentenceState::SentenceStart]
     BreakSentence,
 
+    /// On running Python code and returning None, ignore the code without emitting anything
+    ///
+    /// - [InterpSentenceState::BuildingCode] -> [InterpSentenceState::MidSentence]
+    EmitNone,
+
     /// On encountering the start of an inline scope (i.e. an InlineScopeOpen optionally preceded by Python scope owner),
     /// push an inline scope onto existing paragraph state (or create a new one).
     ///
     /// Finishes the current BuildingText if in progress, pushes it to topmost scope before creating new scope.
     ///
     /// - [InterpSentenceState::SentenceStart] -> [InterpSentenceState::MidSentence]
     /// - [InterpSentenceState::MidSentence] -> [InterpSentenceState::MidSentence]
@@ -289,14 +295,21 @@
                     (
                         S::SentenceStart,
                         (None, Some(InterpSpecialTransition::StartComment(span))),
                     )
                 }
 
                 (
+                    S::BuildingCode { .. },
+                    T::EmitNone,
+                ) => {
+                    (S::MidSentence, (None, None))
+                }
+
+                (
                     S::SentenceStart
                     | S::MidSentence
                     | S::BuildingCode { .. }
                     | S::BuildingText { .. },
                     T::PushInlineScope(builder, span),
                 ) => {
                     let scope = InterpInlineScopeState {
@@ -326,18 +339,18 @@
                 }
 
                 (
                     S::SentenceStart
                     | S::MidSentence
                     | S::BuildingText { .. }
                     | S::BuildingCode { .. },
-                    T::StartRawScope(owner, raw_start, expected_n_hashes),
+                    T::StartRawScope(builder, raw_start, expected_n_hashes),
                 ) => (
                     S::BuildingRawText {
-                        owner,
+                        builder,
                         text: "".into(),
                         raw_start,
                         expected_n_hashes,
                     },
                     (None, None),
                 ),
 
@@ -539,38 +552,55 @@
                     globals,
                 )? {
                     Some((res, code_span)) => {
                         // The code ended...
                         use EvalBracketResult::*;
 
                         let inl_transition = match res {
-                            Block(_) => {
+                            BlockBuilder(_) => {
                                 return Err(InterpError::BlockOwnerCodeMidPara { code_span })
                             }
-                            Inline(i) => PushInlineScope(Some(i), code_span),
-                            Raw(r, n_hashes) => StartRawScope(Some(r), code_span, n_hashes),
+                            Block(_) => {
+                                return Err(InterpError::BlockCodeMidPara { code_span });
+                            }
+                            InlineBuilder(i) => PushInlineScope(Some(i), code_span),
+                            RawBuilder(r, n_hashes) => StartRawScope(Some(r), code_span, n_hashes),
                             // TODO If the object is not already Inline, check if it's Block or BlockScopeBuilder or InlineScopeBuilder or RawScopeBuilder, stringify it, then put in an Unescaped box?
-                            Other(s) => PushInlineContent(InlineNodeToCreate::PythonObject(
-                                PyTcRef::of(s.as_ref(py)).err_as_interp(py, code_span)?,
-                            )),
+                            Inline(i) => PushInlineContent(InlineNodeToCreate::PythonObject(i)),
+                            PyNone => EmitNone,
                         };
                         Some(inl_transition)
                     }
                     None => None,
                 }
             }
             InterpSentenceState::BuildingRawText {
-                owner,
+                builder,
                 text,
                 expected_n_hashes,
-                ..
+                raw_start,
             } => match tok {
-                RawScopeClose(_, n_hashes) if n_hashes == *expected_n_hashes => Some(
-                    PushInlineContent(InlineNodeToCreate::RawText(owner.clone(), text.clone())),
-                ),
+                RawScopeClose(_, n_hashes) if n_hashes == *expected_n_hashes => match builder {
+                    Some(builder) => {
+                        let to_emit = RawScopeBuilder::call_build_from_raw(py, builder, text).err_as_interp(py, *raw_start)?;
+                    
+                        let to_emit_as_py = to_emit.as_ref(py);
+                        if let Ok(_) = PyTcRef::<Block>::of(to_emit_as_py) {
+                            return Err(InterpError::BlockCodeFromRawScopeMidPara{ code_span: *raw_start })
+                        } else if let Ok(inl) = PyTcRef::of(to_emit_as_py) {
+                            Some(PushInlineContent(InlineNodeToCreate::PythonObject(inl)))
+                        } else {
+                            unreachable!()
+                        }
+                    },
+                    None => Some(
+                        PushInlineContent(InlineNodeToCreate::RawText(text.clone())),
+                    ),
+                }
+                    
                 _ => {
                     text.push_str(tok.stringify_raw(data));
                     None
                 }
             },
         };
         Ok(transition)
```

### Comparing `turnip_text-0.0.1/src/python/mod.rs` & `turnip_text-0.0.2/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/src/python/typeclass.rs` & `turnip_text-0.0.2/src/python/typeclass.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/src/tests/test_lexer.rs` & `turnip_text-0.0.2/src/tests/test_lexer.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/src/tests/test_lexer_parser.rs` & `turnip_text-0.0.2/src/tests/test_lexer_parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,71 +34,71 @@
 use TestTTToken::*;
 
 // These tests are condensed versions of the tests in [test_parser] that also sanity-check the tokens generated.
 
 #[test]
 pub fn test_inline_code() {
     expect_lex_parse(
-        r#"3=[len((1,2,3))]"#,
+        r#"3=[test_inline_of(len((1,2,3)))]"#,
         vec![
             OtherText("3="),
             CodeOpen(1),
-            OtherText("len((1,2,3))"),
+            OtherText("test_inline_of(len((1,2,3)))"),
             CodeClose(1),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("3="),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_extra_delimiter() {
     expect_lex_parse(
-        r#"3=[[len((1,2,3))]]"#,
+        r#"3=[[test_inline_of(len((1,2,3)))]]"#,
         vec![
             OtherText("3="),
             CodeOpen(2),
-            OtherText("len((1,2,3))"),
+            OtherText("test_inline_of(len((1,2,3)))"),
             CodeClose(2),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("3="),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_long_extra_delimiter() {
     expect_lex_parse(
-        r#"3=[[[[[len((1,2,3))]]]]]"#,
+        r#"3=[[[[[test_inline_of(len((1,2,3)))]]]]]"#,
         vec![
             OtherText("3="),
             CodeOpen(5),
-            OtherText("len((1,2,3))"),
+            OtherText("test_inline_of(len((1,2,3)))"),
             CodeClose(5),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("3="),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_escaped_extra_delimiter() {
     expect_lex_parse(
-        r#"3=\[[len((1,2,3))]\]"#,
+        r#"3=\[[test_inline_of(len((1,2,3)))]\]"#,
         vec![
             OtherText("3="),
             Escaped(Escapable::SqrOpen),
             CodeOpen(1),
-            OtherText("len((1,2,3))"),
+            OtherText("test_inline_of(len((1,2,3)))"),
             CodeClose(1),
             Escaped(Escapable::SqrClose),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("3=["),
             test_text("3"),
             test_text("]"),
@@ -125,23 +125,23 @@
         )])])),
     )
 }
 
 #[test]
 pub fn test_inline_list_with_extra_delimiter() {
     expect_lex_parse(
-        r#"3=[[len([1,2,3])]]"#,
+        r#"3=[[test_inline_of(len([1,2,3]))]]"#,
         vec![
             OtherText("3="),
             CodeOpen(2),
-            OtherText("len("),
+            OtherText("test_inline_of(len("),
             CodeOpen(1),
             OtherText("1,2,3"),
             CodeClose(1),
-            OtherText(")"),
+            OtherText("))"),
             CodeClose(2),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("3="),
             test_text("3"),
         ]])])),
     )
@@ -334,24 +334,21 @@
         ])])),
     )
 }
 
 #[test]
 pub fn test_special_with_escaped_backslash() {
     expect_lex_parse(
-        r#"\\[None]"#,
+        r#"\\#"#,
         vec![
             Escaped(Escapable::Backslash),
-            CodeOpen(1),
-            OtherText("None"),
-            CodeClose(1),
+            Hashes(1),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("\\"),
-            test_text("None"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_escaped_special_with_escaped_backslash() {
     expect_lex_parse(
@@ -396,20 +393,20 @@
         )])])),
     )
 }
 
 #[test]
 pub fn test_newline_in_code() {
     expect_lex_parse(
-        "[len((1,\r\n2))]",
+        "[test_inline_of(len((1,\r\n2)))]",
         vec![
             CodeOpen(1),
-            OtherText("len((1,"),
+            OtherText("test_inline_of(len((1,"),
             Newline,
-            OtherText("2))"),
+            OtherText("2)))"),
             CodeClose(1),
         ],
         Ok(test_doc(vec![TestBlock::Paragraph(vec![test_sentence(
             "2",
         )])])),
     )
 }
```

### Comparing `turnip_text-0.0.1/src/tests/test_parser.rs` & `turnip_text-0.0.2/src/tests/test_parser.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use crate::python::interop::{
     BlockScope, InlineScope, Paragraph, RawText, Sentence, UnescapedText,
 };
 use crate::python::{interp_data, prepare_freethreaded_turniptext_python, InterpError};
 use crate::util::ParseSpan;
 
 use pyo3::prelude::*;
-use pyo3::types::{PyDict, PyList};
+use pyo3::types::PyDict;
 
 use std::panic;
 // We need to initialize Python the first time we test
 use std::sync::Once;
 static INIT_PYTHON: Once = Once::new();
 
 /// A type mimicking [ParserSpan] for test purposes
@@ -49,14 +49,20 @@
     },
     BlockScopeOpenedMidPara {
         scope_start: TestParserSpan,
     },
     BlockOwnerCodeMidPara {
         code_span: TestParserSpan,
     },
+    BlockCodeMidPara {
+        code_span: TestParserSpan,
+    },
+    BlockCodeFromRawScopeMidPara {
+        code_span: TestParserSpan,
+    },
     SentenceBreakInInlineScope {
         scope_start: TestParserSpan,
     },
     ParaBreakInInlineScope {
         scope_start: TestParserSpan,
     },
     BlockOwnerCodeHasNoScope {
@@ -99,14 +105,20 @@
             },
             InterpError::BlockScopeOpenedMidPara { scope_start } => Self::BlockScopeOpenedMidPara {
                 scope_start: scope_start.into(),
             },
             InterpError::BlockOwnerCodeMidPara { code_span } => Self::BlockOwnerCodeMidPara {
                 code_span: code_span.into(),
             },
+            InterpError::BlockCodeMidPara { code_span } => Self::BlockCodeMidPara {
+                code_span: code_span.into(),
+            },
+            InterpError::BlockCodeFromRawScopeMidPara { code_span } => Self::BlockCodeFromRawScopeMidPara {
+                code_span: code_span.into()
+            },
             InterpError::SentenceBreakInInlineScope { scope_start, .. } => {
                 Self::SentenceBreakInInlineScope {
                     scope_start: scope_start.into(),
                 }
             }
             InterpError::ParaBreakInInlineScope { scope_start, .. } => {
                 Self::ParaBreakInInlineScope {
@@ -259,40 +271,61 @@
 /// Provides `TEST_BLOCK_BUILDER`, `TEST_INLINE_BUILDER`, `TEST_RAW_BUILDER` objects
 /// that can own block, inline, and raw scopes respectively.
 pub fn generate_globals<'interp>(py: Python<'interp>) -> Option<&'interp PyDict> {
     let globals = PyDict::new(py);
 
     let result = py.run(
         r#"
+from turnip_text import InlineScope, UnescapedText, BlockScope
+
 class FauxBlock:
     is_block = True
     def __init__(self, contents):
         self.test_block = contents
 
 class FauxInline:
     is_inline = True
     def __init__(self, contents):
         self.test_inline = contents
 
-class FauxRaw:
+class FauxInlineRaw:
     is_inline = True
-    def __init__(self, contents):
-        self.test_raw_str = str(contents)
+    def __init__(self, raw_str):
+        self.test_raw_str = str(raw_str)
 
 class TestBuilder:
     def build_from_blocks(self, contents):
         return FauxBlock(contents)
     def build_from_inlines(self, contents):
         return FauxInline(contents)
-    def build_from_raw(self, contents):
-        return FauxRaw(contents)
+
+class TestRawInlineBuilder:
+    def build_from_raw(self, raw_str):
+        return FauxInlineRaw(raw_str)
+
+TEST_BLOCK = FauxBlock(BlockScope([]))
+
+class TestRawBlockBuilder:
+    def build_from_raw(self, raw_str):
+        return TEST_BLOCK
+
+class TestBlockSwallower():
+    def build_from_blocks(self, contents):
+        return None
 
 TEST_BLOCK_BUILDER = TestBuilder()
 TEST_INLINE_BUILDER = TestBuilder()
-TEST_RAW_BUILDER = TestBuilder() 
+TEST_RAW_INLINE_BUILDER = TestRawInlineBuilder()
+TEST_RAW_BLOCK_BUILDER = TestRawBlockBuilder()
+
+TEST_BLOCK_SWALLOWER = TestBlockSwallower()
+
+def test_inline_of(x):
+    return UnescapedText(str(x))
+
 "#,
         Some(globals),
         Some(globals),
     );
 
     match result {
         Err(pyerr) => {
@@ -375,48 +408,48 @@
         )
     )
 }
 
 #[test]
 pub fn test_inline_code() {
     expect_parse(
-        r#"Number of values in (1,2,3): [len((1,2,3))]"#,
+        r#"Number of values in (1,2,3): [test_inline_of(len((1,2,3)))]"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("Number of values in (1,2,3): "),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_extra_delimiter() {
     expect_parse(
-        r#"Number of values in (1,2,3): [[ len((1,2,3)) ]]"#,
+        r#"Number of values in (1,2,3): [[ test_inline_of(len((1,2,3))) ]]"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("Number of values in (1,2,3): "),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_long_extra_delimiter() {
     expect_parse(
-        r#"Number of values in (1,2,3): [[[[[ len((1,2,3)) ]]]]]"#,
+        r#"Number of values in (1,2,3): [[[[[ test_inline_of(len((1,2,3))) ]]]]]"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("Number of values in (1,2,3): "),
             test_text("3"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_inline_code_with_escaped_extra_delimiter() {
     expect_parse(
-        r#"Number of values in (1,2,3): \[[ len((1,2,3)) ]\]"#,
+        r#"Number of values in (1,2,3): \[[ test_inline_of(len((1,2,3))) ]\]"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("Number of values in (1,2,3): ["),
             test_text("3"),
             test_text("]"),
         ]])])),
     )
 }
@@ -430,15 +463,15 @@
         )])])),
     )
 }
 
 #[test]
 pub fn test_inline_list_with_extra_delimiter() {
     expect_parse(
-        r#"Number of values in (1,2,3): [[ len([1,2,3]) ]]"#,
+        r#"Number of values in (1,2,3): [[ test_inline_of(len([1,2,3])) ]]"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text("Number of values in (1,2,3): "),
             test_text("3"),
         ]])])),
     )
 }
 
@@ -585,15 +618,15 @@
         }),
     )
 }
 
 #[test]
 pub fn test_owned_inline_raw_scope_with_newline() {
     expect_parse(
-        r#"[TEST_RAW_BUILDER]#{
+        r#"[TEST_RAW_INLINE_BUILDER]#{
 import os
 }#"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             TestInline::TestOwnedRaw(
                 r#"
 import os
 "#
@@ -651,18 +684,17 @@
         ])])),
     )
 }
 
 #[test]
 pub fn test_special_with_escaped_backslash() {
     expect_parse(
-        r#"About to see a backslash! \\[None]"#,
+        r#"About to see a backslash! \\#"#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
             test_text(r#"About to see a backslash! \"#),
-            test_text("None"),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_escaped_special_with_escaped_backslash() {
     expect_parse(
@@ -693,15 +725,15 @@
         )])])),
     )
 }
 
 #[test]
 pub fn test_newline_in_code() {
     expect_parse(
-        "[len((1,\r\n2))]",
+        "[test_inline_of(len((1,\r\n2)))]",
         Ok(test_doc(vec![TestBlock::Paragraph(vec![test_sentence(
             "2",
         )])])),
     )
 }
 #[test]
 pub fn test_code_close_in_text() {
@@ -841,7 +873,122 @@
 Whitespace is allowed after this \
 because you may need it to split up words in sentences."#,
         Ok(test_doc(vec![TestBlock::Paragraph(vec![
             test_sentence("Whitespace is allowed after this because you may need it to split up words in sentences."),
         ])])),
     )
 }
+
+#[test]
+pub fn test_emit_block_from_code() {
+    expect_parse(
+        "[TEST_BLOCK]", 
+        Ok(test_doc(vec![TestBlock::TestOwnedBlock(vec![])])),
+    )
+}
+
+#[test]
+pub fn test_cant_emit_block_from_code_inside_paragraph() {
+    expect_parse(
+        "Lorem ipsum!
+I'm in a [TEST_BLOCK]", 
+        Err(TestInterpError::BlockCodeMidPara { code_span: TestParserSpan { start: (2, 10), end: (2, 22) } }),
+    )
+}
+
+#[test]
+pub fn test_raw_scope_emitting_block_from_block_level() {
+    expect_parse(
+        "[TEST_RAW_BLOCK_BUILDER]#{some raw stuff that goes in a block!}#",
+        Ok(test_doc(vec![TestBlock::TestOwnedBlock(vec![])])),
+    )
+}
+
+#[test]
+pub fn test_raw_scope_emitting_inline_from_block_level() {
+    expect_parse(
+        "[TEST_RAW_INLINE_BUILDER]#{some raw stuff that goes in a block!}#",
+        Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
+            TestInline::TestOwnedRaw("some raw stuff that goes in a block!".into())
+        ]])])),
+    )
+}
+
+#[test]
+pub fn test_raw_scope_cant_emit_block_inside_paragraph() {
+    expect_parse(
+        "Inside a paragraph, you can't [TEST_RAW_BLOCK_BUILDER]#{some raw stuff that goes in a block!}#",
+        Err(TestInterpError::BlockCodeFromRawScopeMidPara { code_span: TestParserSpan { start: (1, 31), end: (1, 57) } })
+    )
+}
+
+#[test]
+pub fn test_raw_scope_emitting_inline_inside_paragraph() {
+    expect_parse(
+        "Inside a paragraph, you can [TEST_RAW_INLINE_BUILDER]#{insert an inline raw!}#",
+        Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
+            test_text("Inside a paragraph, you can "),
+            TestInline::TestOwnedRaw("insert an inline raw!".into())
+        ]])])),
+    )
+}
+
+#[test]
+pub fn test_emitting_none_at_block() {
+    expect_parse(
+        "
+[None]
+", 
+    Ok(test_doc(vec![]))
+    )
+}
+
+#[test]
+pub fn test_emitting_none_inline() {
+    expect_parse(
+        "Check it out, there's [None]!", 
+    Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
+        test_text("Check it out, there's "),
+        test_text("!")
+    ]])]))
+    )
+}
+
+#[test]
+pub fn test_assign_and_recall() {
+    expect_parse(
+        "[x = 5]
+
+[test_inline_of(x)]",
+    Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![test_text("5")]])]))
+    )
+}
+
+#[test]
+pub fn test_syntax_errs_passed_thru() {
+    // The assignment support depends on trying to eval() the expression, that failing with a SyntaxError, and then trying to exec() it.
+    // Make sure that something invalid as both still returns a SyntaxError
+    expect_parse(
+        "[1invalid]",
+        Err(TestInterpError::PythonErr {
+            pyerr: "SyntaxError : invalid syntax (<string>, line 1)".into(),
+            code_span: TestParserSpan { start: (1, 1), end: (1, 11) }
+        })
+    )
+}
+
+#[test]
+pub fn test_block_scope_builder_return_none() {
+    expect_parse(
+        "[TEST_BLOCK_SWALLOWER]{
+stuff that gets swallowed
+}", Ok(test_doc(vec![]))
+    )
+}
+
+#[test]
+pub fn test_block_scope_builder_return_none_with_end_inside_para() {
+    expect_parse(
+        "[TEST_BLOCK_SWALLOWER]{
+stuff that gets swallowed}", Ok(test_doc(vec![]))
+    )
+}
```

### Comparing `turnip_text-0.0.1/src/util.rs` & `turnip_text-0.0.2/src/util.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.1/Cargo.lock` & `turnip_text-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "turnip_text"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "annotate-snippets",
  "anyhow",
  "argh",
  "lexer-rs",
  "pyo3",
  "thiserror",
```

### Comparing `turnip_text-0.0.1/PKG-INFO` & `turnip_text-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: turnip_text
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Dist: mypy; extra == 'typing'
-Requires-Dist: black; extra == 'fmt'
+Requires-Dist: mypy ; extra == 'typing'
+Requires-Dist: black ; extra == 'fmt'
 Provides-Extra: typing
 Provides-Extra: fmt
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: Document description language that allows embedded Python to describe document structure
 Author: Samuel Stark
 Author-email: Samuel Stark <popgoestoast@gmail.com>
```

