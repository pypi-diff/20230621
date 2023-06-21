# Comparing `tmp/nmodl_preprocessor-1.0.6.tar.gz` & `tmp/nmodl_preprocessor-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.6.tar", last modified: Mon May  1 22:42:00 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.7.tar", last modified: Wed Jun 21 00:12:56 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.6.tar` & `nmodl_preprocessor-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.6/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.6/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.6/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1289 2023-04-20 22:05:56.000000 nmodl_preprocessor-1.0.6/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)    20861 2023-05-01 15:35:14.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/cpp_keywords.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     4533 2023-04-30 22:51:37.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     3700 2023-05-01 00:53:22.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      550 2023-05-01 00:53:17.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      479 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-05-01 22:41:13.000000 nmodl_preprocessor-1.0.6/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.7/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.7/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.7/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1899 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1158 2023-06-20 16:40:09.000000 nmodl_preprocessor-1.0.7/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     7434 2023-06-21 00:08:06.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/cpp_keywords.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4592 2023-05-16 19:37:54.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    21822 2023-06-20 15:54:47.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/optimize_nmodl.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     5722 2023-05-15 17:49:58.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      710 2023-05-10 18:26:19.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1899 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      598 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/top_level.txt
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1455 2023-06-20 23:34:46.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/diff_perf.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    10774 2023-06-20 23:28:01.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/histogram.png
+-rw-rw-r--   0 dm        (1000) dm        (1000)      489 2023-06-20 23:36:03.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/notes.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-06-20 04:56:50.000000 nmodl_preprocessor-1.0.7/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.6/DETAILS.pdf` & `nmodl_preprocessor-1.0.7/DETAILS.pdf`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.6/LICENSE.txt` & `nmodl_preprocessor-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.6/PKG-INFO` & `nmodl_preprocessor-1.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.6
+Version: 1.0.7
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -17,50 +17,49 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # nmodl_preprocessor
 
 This program optimizes NMODL files for the NEURON simulator.  
+It scans all of your project's files to perform aggressive whole program optimization.  
 It performs the following optimizations to ".mod" files:  
 * Hardcode the parameters
 * Hardcode the temperature
 * Hardcode any assigned variables with constant values
 * Inline all functions and procedures
 * Convert assigned variables into local variables
 
-These optimizations can improve run-time performance and memory usage by as much
-as 15%.
+These optimizations can improve run-time performance and memory usage by between
+5% and 15%.
 
 ## Installation
 
 #### Prerequisites
 * [Python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/)
 * [The NMODL Framework](https://bluebrain.github.io/nmodl/html/index.html)
 
 ```
 pip install nmodl_preprocessor
 ```
 
 ## Usage
 ```
-$ nmodl_preprocessor [-h] [--celsius CELSIUS] input_path output_path
+$ nmodl_preprocessor [-h] project_dir [model_dir ...]
 
 positional arguments:
-  input_path         input filename or directory of nmodl files
-  output_path        output filename or directory for nmodl files
+  project_dir  root directory of all simulation files
+  model_dir    input directory of nmodl files
 
 options:
-  -h, --help         show this help message and exit
-  --celsius CELSIUS  temperature of the simulation
+  -h, --help   show this help message and exit
 
 ```
 
 ## Tips
 
-* This program will not optimize any RANGE or GLOBAL symbols.  
-  - Remove them unless you actually need to inspect or modify
-    their value at run-time.  
-  - Add parameters to a GLOBAL statement to preserve them.  
+* Keep your projects in separate directories.  
+
+* Use unique and descriptive variable names.  
 
 * Remove unnecessary VERBATIM statements.
```

### Comparing `nmodl_preprocessor-1.0.6/nmodl_preprocessor/__main__.py` & `nmodl_preprocessor-1.0.7/nmodl_preprocessor/optimize_nmodl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-# Copyright (c) 2023 David McDougall
-# Released under the MIT License
-
-from pathlib import Path
-from sys import stderr
 from types import SimpleNamespace
-import argparse
+from pathlib import Path
 import math
 import re
 import shutil
 import textwrap
 
 import nmodl.ast
 import nmodl.dsl
@@ -16,243 +11,242 @@
 ANT = nmodl.ast.AstNodeType
 
 from nmodl_preprocessor.utils import *
 from nmodl_preprocessor.rw_patterns import RW_Visitor
 from nmodl_preprocessor.cpp_keywords import cpp_keywords
 from nmodl_preprocessor import nmodl_to_python
 
-website = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"
-
-parser = argparse.ArgumentParser(prog='nmodl_preprocessor',
-    description="This program optimizes NMODL files for the NEURON simulator.",
-    epilog=f"For more information or to report a problem go to:\n{website}",
-    formatter_class=argparse.RawDescriptionHelpFormatter)
-
-parser.add_argument('input_path', type=str,
-        help="input filename or directory of nmodl files")
-
-parser.add_argument('output_path', type=str,
-        help="output filename or directory for nmodl files")
-
-parser.add_argument('--celsius', type=float, default=None,
-        help="temperature of the simulation")
-
-args = parser.parse_args()
-
-# Find and sanity check all files to be processed.
-input_path  = Path(args.input_path).resolve()
-output_path = Path(args.output_path).resolve()
-process_files   = [] # List of pairs of (source, destination)
-copy_files      = [] # List of pairs of (source, destination)
-assert input_path.exists()
-if input_path.is_file(): # Process a single file.
-    assert input_path.suffix == ".mod", "input file is not an NMODL file (expected \".mod\" file)"
-    if output_path.exists():
-        if output_path.is_file(): # Overwrite the output file.
-            assert output_path.suffix == ".mod", "output file is not an NMODL file (expected \".mod\" file)"
-        elif output_path.is_dir(): # Put the output in this directory.
-            output_path = output_path.joinpath(input_path.name)
-    else:
-        if output_path.suffix: # Write the output to a new file.
-            assert output_path.suffix == ".mod", "output file is not an NMODL file (expected \".mod\" file)"
-        else: # Put the output in a new directory.
-            assert output_path.parent.is_dir(), "output directory does not exist" # Refuse to make multiple nested directories.
-            output_path.mkdir()
-            output_path = output_path.joinpath(input_path.name)
-    process_files.append((input_path, output_path))
-elif input_path.is_dir(): # Process multiple files.
-    if not output_path.exists(): # Make a new directory for the output.
-        assert output_path.parent.is_dir(), "output directory does not exist" # Refuse to make multiple nested directories.
-        output_path.mkdir()
-    assert output_path.is_dir(), "if the input is a directory then the output must also be a directory"
-    for input_file in input_path.iterdir():
-        output_file = output_path.joinpath(input_file.name)
-        if input_file.suffix == ".mod":
-            process_files.append((input_file, output_file))
-        else:
-            copy_files.append((input_file, output_file))
-else:
-    raise RuntimeError('Unreachable')
-
-for input_file, output_file in process_files:
-    assert input_file != output_file, "operation would overwrite input file"
-
 # Don't remove parameters with these names, because of unexpected name conflicts
 # caused by auto-generated initial values.
 parameter_name_conflicts = {'y0', 'j0'}
 
-# Check for known problematic files.
-for input_file, output_file in list(process_files):
-    if input_file.name in {'vecst.mod'}:
-        process_files.remove((input_file, output_file))
-        copy_files.append((input_file, output_file))
-
-# Main Loop.
-for input_file, output_file in process_files:
+def optimize_nmodl(input_file, output_file, external_refs, other_nmodl_refs, celsius=None) -> bool:
     # 
-    def print_verbose(*strings, **kwargs):
-        print(input_file.name+':', *strings, **kwargs, file=stderr)
-    def print_exception(exception):
-        print_verbose(f"{type(exception).__name__}: {str(exception)}")
-    # First read the file as binary and discard as much of it as possible.
-    print_verbose(f'read file: "{input_file}"')
+    def print(*strings, **kwargs):
+        __builtins__['print'](input_file.name+':', *strings, **kwargs)
+
+    # First read the file as binary and discard as much of it as possible, in
+    # case it contains invalid utf-8.
     with open(input_file, 'rb') as f:
         nmodl_text = f.read()
 
-    # Remove comments because they might contain invalid utf-8 text.
-    nmodl_text = re.sub(rb'(?s)\bCOMMENT\b.*?\bENDCOMMENT\b', b'', nmodl_text)
+    def clean_nmodl(nmodl_text):
+        # Remove comments.
+        nmodl_text = re.sub(rb'(?s)\bCOMMENT\b.*?\bENDCOMMENT\b', b'', nmodl_text)
+        # Remove INDEPENDENT statements because they're unnecessary and the nmodl library does not like them.
+        nmodl_text = re.sub(rb'\bINDEPENDENT\b\s*{[^{}]*}', b'', nmodl_text)
+        return nmodl_text
+
+    nmodl_text = clean_nmodl(nmodl_text)
+
+    # Substitute INCLUDE statements with the file that they point to.
+    include_regex = re.compile(br'\bINCLUDE\s*"(.*)"')
+    def include_file(match):
+        file = match.groups()[0].decode()
+        # TODO: This is supposed to search the environment variable "MODL_INCLUDES".
+        for path in (Path.cwd(), input_file.parent,):
+            include_file = path.joinpath(file)
+            if include_file.exists():
+                with open(include_file, 'rb') as f:
+                    return f.read()
+        raise ValueError(f'file not found {file}')
+    nmodl_text = re.sub(include_regex, include_file, nmodl_text)
 
-    # Remove INDEPENDENT statements because they're unnecessary and the nmodl library does not like them.
-    nmodl_text = re.sub(rb'\bINDEPENDENT\b\s*{[^{}]*}', b'', nmodl_text)
+    nmodl_text = clean_nmodl(nmodl_text)
+    nmodl_text = nmodl_text.decode()
+    nmodl_text = ''.join(filter((lambda x: x.isprintable() or x.isspace()), nmodl_text))
 
     # Parse the nmodl file into an AST.
-    nmodl_text = nmodl_text.decode()
     try:
         AST = nmodl.NmodlDriver().parse_string(nmodl_text)
+    except RuntimeError as error:
+        print("warning: could not parse file:", str(error))
+        shutil.copy(input_file, output_file.parent.joinpath(input_file.name))
+        return
+    try:
         nmodl.symtab.SymtabVisitor().visit_program(AST)
     except RuntimeError as error:
-        print_exception(error)
-        print_verbose("warning: could not parse and build symbol table")
-        copy_files.append((input_file, output_file))
-        continue
-
-    # nmodl.ast.view(AST)             # Useful for debugging.
-    # print(AST.get_symbol_table())   # Useful for debugging.
-
-    # Check for INCLUDE statements. It is unreasonable to find the included file.
-    # The file is located in one of the following places (searched in this order):
-    #     1) The current working directory,
-    #     2) The directory of this nmodl file,
-    #     3) The directories specified by the "MODL_INCLUDES" environment variable.
-    # INCLUDE statements prevent all optimizations because they all rely on
-    # having the complete NMODL source code.
+        print("warning: could not build symbol table:", str(error))
+        shutil.copy(input_file, output_file.parent.joinpath(input_file.name))
+        return
+
     visitor = nmodl.dsl.visitor.AstLookupVisitor()
     lookup  = lambda ast_node_type: visitor.lookup(AST, ast_node_type)
-    if lookup(ANT.INCLUDE):
-        print_verbose('warning: INCLUDE prevent optimization')
-        copy_files.append((input_file, output_file))
-        continue
+    includes = list(lookup(ANT.INCLUDE))
+
+
+
+    # Useful for debugging.
+    # nmodl.ast.view(AST)
+    # print(AST.get_symbol_table())
+
+
 
     # Find all symbols that are referenced in VERBATIM blocks.
     verbatim_vars = set()
+    verbatim_length = 0
     for stmt in lookup(ANT.VERBATIM):
-        for symbol in re.finditer(r'\b\w+\b', nmodl.to_nmodl(stmt)):
+        verbatim_text = nmodl.to_nmodl(stmt)
+        verbatim_length += len(verbatim_text)
+        for symbol in re.finditer(r'[a-zA-Z]\w*', verbatim_text):
             verbatim_vars.add(symbol.group())
     verbatim_vars -= cpp_keywords
+    if verbatim_length / len(nmodl_text) > .50:
+        print('warning: too much VERBATIM, will not optimize')
+        shutil.copy(input_file, output_file.parent.joinpath(input_file.name))
+        return
     # Let's get this warning out of the way. As chunks of arbitrary C/C++ code,
     # VERBATIM blocks can not be analysed. Assume that all symbols in VERBATIM
     # blocks are publicly visible and are both read from and written to.
     # Do not attempt to alter the source code inside of VERBATIM blocks.
     if verbatim_vars:
-        print_verbose('warning: VERBATIM may prevent optimization')
+        print('warning: VERBATIM may prevent optimization')
 
     # Inline all of the functions and procedures
     if not verbatim_vars: # The NMODL library fails to correctly analyze VERBATIM blocks.
         try:
             nmodl.dsl.visitor.InlineVisitor().visit_program(AST)
         except RuntimeError as error:
-            print_exception(error)
-            print_verbose("warning: could not inline all functions and procedures")
+            print("warning: could not inline all functions and procedures:", str(error))
         else:
             nmodl_text = nmodl.to_nmodl(AST)
         # Reload the modified AST so that the NMODL library starts from a clean state.
         AST    = nmodl.NmodlDriver().parse_string(nmodl_text)
         lookup = lambda ast_node_type: visitor.lookup(AST, ast_node_type)
         nmodl.symtab.SymtabVisitor().visit_program(AST)
 
+    # Find all external references to this mechanism.
+    try:
+        suffix = '_' + STR(next(iter(lookup(ANT.SUFFIX))).get_node_name())
+    except StopIteration:
+        suffix = ''
+    external_refs = set(external_refs) # Will mutate, don't alter the original version.
+    for x in list(external_refs) + list(other_nmodl_refs):
+        if x.endswith(suffix):
+            external_refs.add(x[:-len(suffix)])
+
     # Extract important data from the symbol table.
     sym_table           = AST.get_symbol_table()
     sym_type            = nmodl.symtab.NmodlType
     get_vars_with_prop  = lambda prop: set(STR(x.get_name()) for x in sym_table.get_variables_with_properties(prop))
     neuron_vars         = get_vars_with_prop(sym_type.extern_neuron_variable)
     read_ion_vars       = get_vars_with_prop(sym_type.read_ion_var)
     write_ion_vars      = get_vars_with_prop(sym_type.write_ion_var)
     nonspecific_vars    = get_vars_with_prop(sym_type.nonspecific_cur_var)
     electrode_cur_vars  = get_vars_with_prop(sym_type.electrode_cur_var)
     range_vars          = get_vars_with_prop(sym_type.range_var)
     global_vars         = get_vars_with_prop(sym_type.global_var)
+    constant_vars       = get_vars_with_prop(sym_type.constant_var)
     parameter_vars      = get_vars_with_prop(sym_type.param_assign)
     assigned_vars       = get_vars_with_prop(sym_type.assigned_definition)
     state_vars          = get_vars_with_prop(sym_type.state_var)
     pointer_vars        = get_vars_with_prop(sym_type.pointer_var) | get_vars_with_prop(sym_type.bbcore_pointer_var)
-    functions           = get_vars_with_prop(sym_type.function_block)
-    procedures          = get_vars_with_prop(sym_type.procedure_block)
+    function_vars       = get_vars_with_prop(sym_type.function_block)
+    procedure_vars      = get_vars_with_prop(sym_type.procedure_block)
     reaction_vars       = set(STR(x.get_node_name()) for x in lookup(ANT.REACT_VAR_NAME))
     compartment_vars    = set()
     for c in lookup(ANT.COMPARTMENT):
         compartment_vars.update(STR(x.get_node_name()) for x in c.names)
     diffusion_vars = set()
     for d in lookup(ANT.LON_DIFUSE):
         diffusion_vars.update(STR(x.get_node_name()) for x in d.names)
     state_vars = state_vars | reaction_vars | compartment_vars | diffusion_vars
-    # Check for array variables and ignore them. They should have already been
-    # unrolled into individual variables by now.
+    # Find all array variables.
+    array_vars = {}
     for x in sym_table.get_variables_with_properties(sym_type.assigned_definition):
-        node = x.get_node()
-        if '[' in str(node):
-            assigned_vars.discard(STR(x.get_name()))
+        for decl in x.get_nodes():
+            if length := getattr(decl, 'length', None):
+                array_vars[STR(x.get_name())] = nmodl.to_nmodl(length)
     # Find all symbols which are provided by or are visible to the larger NEURON simulation.
     external_vars = (
             neuron_vars |
             read_ion_vars |
             write_ion_vars |
             nonspecific_vars |
             electrode_cur_vars |
-            range_vars |
-            global_vars |
             state_vars |
             pointer_vars |
-            functions |
-            procedures |
+            ((function_vars | procedure_vars | range_vars | global_vars | parameter_vars) & external_refs) |
             verbatim_vars)
     # Find the units associated with each assigned variable.
     assigned_units = {name: '' for name in assigned_vars}
     for stmt in lookup(ANT.ASSIGNED_DEFINITION):
         if stmt.unit:
             assigned_units[STR(stmt.name)] = STR(stmt.unit)
     # Code analysis: determine the read/write usage patterns for each variable.
     rw = RW_Visitor()
     rw.visit_program(AST)
     # Split the document into its top-level blocks for easier manipulation.
     blocks_list = [SimpleNamespace(node=x, text=nmodl.to_nmodl(x)) for x in AST.blocks]
     blocks      = {get_block_name(x.node): x for x in blocks_list}
+    # 
+    if block := blocks.get('NET_RECEIVE', None):
+        for x in visitor.lookup(block.node, ANT.INITIAL_BLOCK):
+            blocks['NET_RECEIVE INITIAL'] = SimpleNamespace(node=x, text=nmodl.to_nmodl(x))
+
+
+    # Useful for debugging.
+    if False:
+        symbols = {k:v for k,v in locals().items() if k.endswith('_vars')}
+        for name, symbols in sorted(symbols.items()):
+            if name == 'external_vars': continue
+            if symbols: print((name + ':').ljust(20), ', '.join(sorted(symbols)))
+        for block in blocks:
+            print("Top Level Block:", block)
+            reads  = rw.reads.get(block, set())
+            writes = rw.writes.get(block, set())
+            maybes = rw.maybes.get(block, set()) - writes
+            if reads:  print("Read Variables:",  ', '.join(sorted(reads)))
+            if writes: print("Always Write Variables:", ', '.join(sorted(writes)))
+            if maybes: print("Maybe Write Variables:", ', '.join(sorted(maybes)))
+
+
+
+    ############################################################################
+    # Determine what to optimize.
+
 
     # Inline the parameters.
     parameters = {}
-    for name in (parameter_vars - external_vars - rw.all_writes - parameter_name_conflicts):
+    for name in ((parameter_vars | constant_vars) - external_vars - rw.all_writes - parameter_name_conflicts):
         for node in sym_table.lookup(name).get_nodes():
-            if node.is_param_assign() and node.value is not None:
+            if (node.is_param_assign() or node.is_constant_var()) and node.value is not None:
                 value = float(STR(node.value))
                 units = ('('+STR(node.unit.name)+')') if node.unit else ''
                 parameters[name] = (value, units)
-                print_verbose(f'inline PARAMETER: {name} = {value} {units}')
+                if node.is_param_assign():
+                    print(f'hardcode PARAMETER: {name} = {value} {units}')
+                elif node.is_constant_var():
+                    print(f'hardcode CONSTANT: {name} = {value} {units}')
+                else:
+                    raise RuntimeError(type(node))
 
     # Inline celsius if it's given and if this nmodl file uses it.
-    if args.celsius is not None and 'celsius' in parameter_vars:
+    if celsius is not None and 'celsius' in parameter_vars:
         if 'celsius' in verbatim_vars:
             pass # Can not inline into VERBATIM blocks.
         else:
             # Overwrite any existing default value with the given value.
-            parameters['celsius'] = (args.celsius, '(degC)')
-            print_verbose(f'inline PARAMETER: celsius = {args.celsius} (degC)')
+            parameters['celsius'] = (celsius, '(degC)')
+            print(f'hardcode TEMPERATURE: celsius = {celsius} (degC)')
 
     # Inline Q10. Detect and inline assigned variables with known constant
     # values that are set in the initial block.
     assigned_const_value = {}
     if initial_block := blocks.get('INITIAL', None):
         # Convert the INITIAL block into python.
         x = nmodl_to_python.PyGenerator()
         try:
             x.visit_initial_block(initial_block.node)
             can_exec = True
         except nmodl_to_python.VerbatimError:
             can_exec = False
-        except nmodl_to_python.ComplexityError:
+        except nmodl_to_python.ComplexityError as error:
             can_exec = False
-            print_verbose('warning: complex INITIAL block may prevent optimization')
+            print('warning: complex INITIAL block may prevent optimization:', error.args[0])
         # 
         global_scope  = dict(nmodl_to_python.nmodl_builtins)
         initial_scope = {}
         # Represent unknown external input values as NaN's.
         for name in external_vars | parameter_vars:
             global_scope[name] = math.nan
         # Only use the parameters which we've committed to hard-coding.
@@ -263,47 +257,80 @@
             global_scope[name] = 0.0
         # 
         if can_exec:
             try:
                 exec(x.pycode, global_scope, initial_scope)
             except Exception as error:
                 pycode = prepend_line_numbers(x.pycode.rstrip())
-                print_exception(error)
-                print_verbose("warning: could not execute INITIAL block:\n" + pycode)
+                print("warning: could not execute INITIAL block:\n" + pycode)
+                print("exception:", str(error))
                 initial_scope = {}
-        # Find all of the variables which are written to durring the runtime.
+        # Find all of the variables which are written to during the runtime.
         # These variables obviously do not have a constant value.
         runtime_writes_to = set()
-        for block_name, variables in rw.writes.items():
+        for block_name, variables in rw.maybes.items():
             if block_name != 'INITIAL':
                 runtime_writes_to.update(variables)
         # Search the local scope of the INITIAL block for variables which can be optimized away.
         for name, value in initial_scope.items():
             if name in assigned_vars:
                 if name in external_vars: continue
                 if name in runtime_writes_to: continue
                 # Filter out values that can not be computed ahead of time
                 # because they depends on unknown external values (like the
                 # voltage or the cell diameter).
                 if math.isnan(value): continue
                 # 
                 units = assigned_units[name]
                 assigned_const_value[name] = (value, units)
-                print_verbose(f'inline ASSIGNED with constant value: {name} = {value} {units}')
+                print(f'hardcode ASSIGNED with constant value: {name} = {value} {units}')
 
     # Convert assigned variables into local variables as able.
     assigned_to_local = set(assigned_vars) - set(external_vars) - set(assigned_const_value)
     # Search for variables whose persistent state is ignored/overwritten.
     for block_name, read_variables in rw.reads.items():
         assigned_to_local -= read_variables
     # 
     for name in assigned_to_local:
-        print_verbose(f'convert from ASSIGNED to LOCAL: {name}')
+        print(f'convert from ASSIGNED to LOCAL: {name}')
+
+
 
     ############################################################################
+    # Apply the optimizations.
+
+
+    # Useful for debugging.
+    if False:
+        # Do not intentionally apply any optimizations.
+        parameters = {}
+        assigned_const_value = {}
+        assigned_to_local = set()
+        print("debug mode: will not apply any optimizations")
+
+
+
+    # Rewrite the NEURON block without the removed variables.
+    if block := blocks.get('NEURON', None):
+        new_block = "NEURON {\n"
+        for stmt in block.node.statement_block.statements:
+            if stmt.is_global() or stmt.is_range():
+                variables = [x.get_node_name() for x in stmt.variables]
+                variables = [x for x in variables if x not in parameters]
+                variables = [x for x in variables if x not in assigned_to_local]
+                variables = [x for x in variables if x not in assigned_const_value]
+                if not variables:
+                    continue
+                if   stmt.is_global(): new_block += '    GLOBAL '
+                elif stmt.is_range():  new_block += '    RANGE '
+                new_block += ', '.join(variables) + '\n'
+            else:
+                new_block += '    ' + nmodl.to_nmodl(stmt) + '\n'
+        new_block += "}\n"
+        block.text = new_block
 
     # Regenerate the PARAMETER block without the inlined parameters.
     if block := blocks.get('PARAMETER', None):
         new_lines = []
         for stmt in block.node.statements:
             if stmt.is_param_assign():
                 name = STR(stmt.name)
@@ -321,24 +348,46 @@
         new_lines = []
         for stmt in block.node.definitions:
             if not (stmt.is_assigned_definition() and STR(stmt.name) in remove_assigned):
                 stmt_nmodl = nmodl.to_nmodl(stmt)
                 new_lines.append(stmt_nmodl)
         block.text = 'ASSIGNED {\n' + '\n'.join('    ' + x for x in new_lines) + '\n}'
 
+    # Insert new LOCAL statements to replace the removed assigned variables.
+    new_locals = {} # Maps from block name to set of names of new local variables.
+    new_locals['INITIAL'] = set(assigned_const_value.keys())
+    for block_name, write_variables in rw.maybes.items():
+        new_locals.setdefault(block_name, set()).update(assigned_to_local & write_variables)
+    # 
+    for block_name, local_names in new_locals.items():
+        local_names = sorted(local_names)
+        if not local_names:
+            continue
+        block = blocks[block_name]
+        signature, start, body = block.text.partition('{')
+        body = textwrap.indent(body, '    ')
+        # Format the local variables for printing.
+        for idx, name in enumerate(sorted(local_names)):
+            if array_size := array_vars.get(name, None):
+                local_names[idx] = name + '[' + array_size + ']'
+        local_names = ', '.join(local_names)
+        block.text = signature + '{\n    LOCAL ' + local_names + '\n    {' + body + '\n}'
+
     # Substitute the parameters with their values.
     substitutions = dict(parameters)
     substitutions.update(assigned_const_value)
+
     # Delete any references to the substituted symbols out of TABLE statements.
     # First setup a regex to find the TABLE statements.
     list_regex  = r'\w+(\s*,\s*\w+)*'
-    table_regex = rf'\bTABLE\s+(?P<table_vars>{list_regex}\s+)?(DEPEND\s+(?P<depend_vars>{list_regex})\s+)?FROM\b'
+    table_regex = rf'\bTABLE\s+(?P<table_vars>{list_regex}\s+)?(DEPEND\s+(?P<depend_vars>{list_regex})\s+)?FROM\b(?P<tail>.*)'
     table_regex = re.compile(table_regex)
     def rewrite_table_stmt(match):
         match = match.groupdict()
+        is_function_table = bool(match['table_vars'])
         # Process each list of variables and store them back into the dict.
         for section in ('table_vars', 'depend_vars'):
             var_list = match[section]
             if var_list is None:
                 var_list = ''
             else:
                 var_list = re.split(r'\s+|,', var_list)
@@ -346,26 +395,28 @@
                 var_list = [x for x in var_list if x not in substitutions] # Filter out hardcoded parameters.
                 var_list = [x for x in var_list if x not in assigned_to_local] # Filter out local vars with no persistent state.
                 var_list = ', '.join(var_list)
             match[section] = var_list
         # Rewrite the TABLE statement using the new lists of variables.
         table_vars  = match['table_vars']
         depend_vars = match['depend_vars']
-        if depend_vars:
-            return f'TABLE {table_vars} DEPEND {depend_vars} FROM'
-        else:
-            return f'TABLE {table_vars} FROM'
+        if table_vars or not is_function_table:
+            if depend_vars:
+                return f'TABLE {table_vars} DEPEND {depend_vars} FROM' + match['tail']
+            else:
+                return f'TABLE {table_vars} FROM' + match['tail']
     # Search for the blocks which contain code.
-    for block in blocks_list:
+    for block in blocks.values():
         if block.node.is_model(): continue
         if block.node.is_block_comment(): continue
         if block.node.is_neuron_block(): continue
         if block.node.is_unit_block(): continue
         if block.node.is_unit_state(): continue
         if block.node.is_param_block(): continue
+        if block.node.is_constant_block(): continue
         if block.node.is_state_block(): continue
         if block.node.is_assigned_block(): continue
         if block.node.is_local_list_statement(): continue
         if block.node.is_define(): continue
         # 
         block.text = re.sub(table_regex, rewrite_table_stmt, block.text)
         # Don't substitute function/procedure arguments.
@@ -384,53 +435,39 @@
             if float(value) == int(value):
                 value = int(value)
             # Substitute the symbol out of general code.
             value = str(value) + units
             body  = re.sub(rf'\b{name}\b', value, body)
         block.text = declaration + brace + body
 
-    # Check the temperature in the INITIAL block.
-    if 'celsius' in parameters:
-        if block := blocks.get('INITIAL', None):
-            signature, start, body = block.text.partition('{')
-            check_temp = f"\n    VERBATIM\n    assert(celsius == {parameters['celsius'][0]});\n    ENDVERBATIM\n"
-            block.text = signature + start + check_temp + body
-
-    # Insert new LOCAL statements to replace the removed assigned variables.
-    new_locals = {} # Maps from block name to set of names of new local variables.
-    if assigned_const_value:
-        new_locals['INITIAL'] = set(assigned_const_value.keys())
-    for block_name, write_variables in rw.writes.items():
-        if converted_variables := assigned_to_local & write_variables:
-            new_locals.setdefault(block_name, set()).update(converted_variables)
-    # 
-    for block_name, local_names in new_locals.items():
-        block = blocks[block_name]
-        signature, start, body = block.text.partition('{')
-        names = ', '.join(sorted(local_names))
-        body  = textwrap.indent(body, '    ')
-        block.text = signature + '{\n    LOCAL ' + names + '\n    {' + body + '\n}'
+    # Special case for initial block inside of net receive.
+    if initial_block := blocks.get('NET_RECEIVE INITIAL', None):
+        block = blocks['NET_RECEIVE']
+        before, keyword, after = block.text.partition('INITIAL')
+        # Discard the next block of statements.
+        depth = 0
+        for match in re.finditer(r'{|}', after):
+            if match.group() == '{':
+                depth += 1
+            elif match.group() == '}':
+                depth -= 1
+                if depth == 0:
+                    break
+        assert (depth == 0) and (match.group() == '}')
+        block.text = before + initial_block.text + after[match.end():]
 
     # Find any local statements in the top level scope and move them to the top
     # of the file. Local variables must be declared before they're used, and
     # inlining functions can cause them to be used before they were originally declared.
     blocks_list.sort(key=lambda x: not (
             x.node.is_model() or x.node.is_block_comment() or
             x.node.is_local_list_statement() or x.node.is_define()))
 
     # Join the top-level blocks back into one big string and save it to the output file.
     nmodl_text = '\n\n'.join(x.text for x in blocks_list) + '\n'
 
     # Break up very long lines into multiple lines as able.
     nmodl_text = re.sub(r'.{500}\b', lambda m: m.group() + '\n', nmodl_text)
 
-    print_verbose(f'write file: "{output_file}"')
     with output_file.open('w') as f:
         f.write(nmodl_text)
 
-# Copy over any miscellaneous files from the source directory.
-for src, dst in copy_files:
-    print(f'Copy associated file: "{src.name}"')
-    shutil.copy(src, dst)
-
-_placeholder = lambda: None # Symbol for the CLI script to import and call.
-
```

### Comparing `nmodl_preprocessor-1.0.6/nmodl_preprocessor/cpp_keywords.py` & `nmodl_preprocessor-1.0.7/nmodl_preprocessor/cpp_keywords.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.6/nmodl_preprocessor/nmodl_to_python.py` & `nmodl_preprocessor-1.0.7/nmodl_preprocessor/nmodl_to_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,29 +113,29 @@
             else_node.statement_block.accept(self)
 
     def visit_function_call(self, node):
         name = node.name.get_node_name()
         if name in nmodl_builtins:
             pass
         elif name == "net_send":
-            raise ComplexityError()
+            raise ComplexityError(f'call {name}')
         else:
             # All functions and procedures should have been inlined already.
             # The exceptions mostly involve TABLE statements.
             # I could attempt to evaluate these calls, but that would be very
             # complicated, especially because python does not support ASSIGNED
             # variables, which would need to be communicated back to the caller.
-            raise ComplexityError()
+            raise ComplexityError(f'call {name}')
         # 
         self.pycode += name + "("
         for arg in node.arguments:
             arg.accept(self)
             self.pycode += ", "
         self.pycode += ")"
 
     def visit_while_statement(self, node):
         # Can not guarantee correct results BC the condition might reference unknown values.
-        raise ComplexityError()
+        raise ComplexityError('while_statement')
 
     def visit_indexed_name(self, node):
-        raise ComplexityError()
+        raise ComplexityError('indexed_name')
```

### Comparing `nmodl_preprocessor-1.0.6/nmodl_preprocessor/utils.py` & `nmodl_preprocessor-1.0.7/nmodl_preprocessor/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 STR = lambda x: str(x).strip() # nmodl sometimes leaves trailing whitespace on stuff.
 
 def get_block_name(node):
     if node.is_ba_block():
         return get_block_name(node.parent)
+    if node.is_before_block():
+        return 'BEFORE ' + STR(node.bablock.type)
+    if node.is_after_block():
+        return 'AFTER ' + STR(node.bablock.type)
     if name := getattr(node, 'name', None):
         return STR(name)
     try:
         return STR(node.get_nmodl_name())
     except RuntimeError:
         return STR(node.get_node_type_name())
```

### Comparing `nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.6
+Version: 1.0.7
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -17,50 +17,49 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # nmodl_preprocessor
 
 This program optimizes NMODL files for the NEURON simulator.  
+It scans all of your project's files to perform aggressive whole program optimization.  
 It performs the following optimizations to ".mod" files:  
 * Hardcode the parameters
 * Hardcode the temperature
 * Hardcode any assigned variables with constant values
 * Inline all functions and procedures
 * Convert assigned variables into local variables
 
-These optimizations can improve run-time performance and memory usage by as much
-as 15%.
+These optimizations can improve run-time performance and memory usage by between
+5% and 15%.
 
 ## Installation
 
 #### Prerequisites
 * [Python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/)
 * [The NMODL Framework](https://bluebrain.github.io/nmodl/html/index.html)
 
 ```
 pip install nmodl_preprocessor
 ```
 
 ## Usage
 ```
-$ nmodl_preprocessor [-h] [--celsius CELSIUS] input_path output_path
+$ nmodl_preprocessor [-h] project_dir [model_dir ...]
 
 positional arguments:
-  input_path         input filename or directory of nmodl files
-  output_path        output filename or directory for nmodl files
+  project_dir  root directory of all simulation files
+  model_dir    input directory of nmodl files
 
 options:
-  -h, --help         show this help message and exit
-  --celsius CELSIUS  temperature of the simulation
+  -h, --help   show this help message and exit
 
 ```
 
 ## Tips
 
-* This program will not optimize any RANGE or GLOBAL symbols.  
-  - Remove them unless you actually need to inspect or modify
-    their value at run-time.  
-  - Add parameters to a GLOBAL statement to preserve them.  
+* Keep your projects in separate directories.  
+
+* Use unique and descriptive variable names.  
 
 * Remove unnecessary VERBATIM statements.
```

### Comparing `nmodl_preprocessor-1.0.6/pyproject.toml` & `nmodl_preprocessor-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["nmodl_preprocessor"]
 
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.6"
+version = "1.0.7"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 urls = {Homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"}
```

