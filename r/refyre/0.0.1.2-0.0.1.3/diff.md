# Comparing `tmp/refyre-0.0.1.2.tar.gz` & `tmp/refyre-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refyre-0.0.1.2.tar", max compression
+gzip compressed data, was "refyre-0.0.1.3.tar", max compression
```

## Comparing `refyre-0.0.1.2.tar` & `refyre-0.0.1.3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0      355 2023-05-28 21:01:39.742013 refyre-0.0.1.2/README.md
--rw-r--r--   0        0        0      821 2023-05-28 21:01:39.742013 refyre-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0    18563 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/Refyre.py
--rw-r--r--   0        0        0      115 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/__init__.py
--rw-r--r--   0        0        0      580 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/cli.py
--rw-r--r--   0        0        0      441 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/core/AliasManager.py
--rw-r--r--   0        0        0      641 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/core/CodeManager.py
--rw-r--r--   0        0        0     2595 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/core/RecipePreprocessor.py
--rw-r--r--   0        0        0      126 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/core/__init__.py
--rw-r--r--   0        0        0     1532 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/datastack/DataStack.py
--rw-r--r--   0        0        0       34 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/datastack/__init__.py
--rw-r--r--   0        0        0     8380 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fcluster/AutoRefresher.py
--rw-r--r--   0        0        0    11904 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fcluster/FileCluster.py
--rw-r--r--   0        0        0      355 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fcluster/FileClusterIterator.py
--rw-r--r--   0        0        0       77 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fcluster/__init__.py
--rw-r--r--   0        0        0      802 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fgraph/FileGraph.py
--rw-r--r--   0        0        0     2012 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fgraph/FileGraphNode.py
--rw-r--r--   0        0        0       73 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/fgraph/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/ExpressionGenerator.py
--rw-r--r--   0        0        0     5585 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/Lexer.py
--rw-r--r--   0        0        0     2776 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/Parser.py
--rw-r--r--   0        0        0     1411 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/PatternGenerator.py
--rw-r--r--   0        0        0      270 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/__init__.py
--rw-r--r--   0        0        0      760 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/cogs/LexerToken.py
--rw-r--r--   0        0        0     2719 2023-05-28 21:01:39.742013 refyre-0.0.1.2/refyre/reader/cogs/VariableParser.py
--rw-r--r--   0        0        0      618 2023-05-28 21:01:39.746013 refyre-0.0.1.2/refyre/reader/cogs/lexer_utils.py
--rw-r--r--   0        0        0      136 2023-05-28 21:01:39.746013 refyre-0.0.1.2/refyre/utils/__init__.py
--rw-r--r--   0        0        0      617 2023-05-28 21:01:39.746013 refyre-0.0.1.2/refyre/utils/clone.py
--rw-r--r--   0        0        0      413 2023-05-28 21:01:39.746013 refyre-0.0.1.2/refyre/utils/optional_imports.py
--rw-r--r--   0        0        0      589 2023-05-28 21:01:39.746013 refyre-0.0.1.2/refyre/utils/regex.py
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 refyre-0.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10009 2023-06-21 04:06:36.387076 refyre-0.0.1.3/README.md
+-rw-r--r--   0        0        0      921 2023-06-21 04:06:36.387076 refyre-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    23166 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/Refyre.py
+-rw-r--r--   0        0        0      135 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cli.py
+-rw-r--r--   0        0        0     3427 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/Broadcast.py
+-rw-r--r--   0        0        0    18513 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/Cluster.py
+-rw-r--r--   0        0        0      718 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/FileClusterIterator.py
+-rw-r--r--   0        0        0      164 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/__init__.py
+-rw-r--r--   0        0        0     3637 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/cogs/VariableAction.py
+-rw-r--r--   0        0        0     2767 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/cluster/cogs/VariableParser.py
+-rw-r--r--   0        0        0       23 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/config/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/config/log.py
+-rw-r--r--   0        0        0      499 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/core/AliasManager.py
+-rw-r--r--   0        0        0      375 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/core/CodeManager.py
+-rw-r--r--   0        0        0     3882 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/core/RecipePreprocessor.py
+-rw-r--r--   0        0        0      126 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/core/__init__.py
+-rw-r--r--   0        0        0     1658 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/datastack/DataStack.py
+-rw-r--r--   0        0        0       34 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/datastack/__init__.py
+-rw-r--r--   0        0        0      802 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/graph/FileGraph.py
+-rw-r--r--   0        0        0     2051 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/graph/FileGraphNode.py
+-rw-r--r--   0        0        0       73 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/graph/__init__.py
+-rw-r--r--   0        0        0     2262 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/ExpressionGenerator.py
+-rw-r--r--   0        0        0     6066 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/Lexer.py
+-rw-r--r--   0        0        0     3287 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/Parser.py
+-rw-r--r--   0        0        0     2662 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/PatternGenerator.py
+-rw-r--r--   0        0        0      221 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/cogs/LexerToken.py
+-rw-r--r--   0        0        0      618 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/reader/cogs/lexer_utils.py
+-rw-r--r--   0        0        0      153 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/utils/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/utils/clone.py
+-rw-r--r--   0        0        0      453 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/utils/optional_imports.py
+-rw-r--r--   0        0        0      903 2023-06-21 04:06:36.387076 refyre-0.0.1.3/refyre/utils/regex.py
+-rw-r--r--   0        0        0    10868 1970-01-01 00:00:00.000000 refyre-0.0.1.3/PKG-INFO
```

### Comparing `refyre-0.0.1.2/pyproject.toml` & `refyre-0.0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refyre"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "Filesystem dominance is all you need."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/refyre"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
@@ -16,19 +16,23 @@
             "License :: OSI Approved :: MIT License",
 ]
 include = [
     "LICENSE.md",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7"
-
+python = ">=3.8"
+tqdm = ">=4.64.0"
+requests = ">=2.29.0"
+pandas = ">=2.0.0"
+gitpython = ">=3.1.30"
 
 [tool.poetry.dev-dependencies]
 pytest = {version="^7.0.1", python = ">=3.7,<4.0"}
+pillow = ">=9.4.0"
 
 [tool.poetry.scripts]
 refyre = "refyre.cli:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `refyre-0.0.1.2/refyre/cli.py` & `refyre-0.0.1.3/refyre/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 import argparse 
+import sys
 from refyre import Refyre
+from refyre.core import RecipePreprocessor
 
 #Instantiate an argument parser
-def cli():
+def main(argv = None):
     parser = argparse.ArgumentParser(
         prog = "cli",
         description = "refyre v.0.0.1 CLI",
     )
 
     #Add positional arguments for input specs
     parser.add_argument("-i", '--input', help = "filepaths to the input specs, seperated by spaces", nargs='+')
     parser.add_argument("-o", '--output', help = "filepaths to the output specs, seperated by spaces", nargs='+')
+    parser.add_argument("-r", '--recipe', help = "path to recipe / workflow file you want refyre to execute")
 
-    args = parser.parse_args()
+    #Add positional arguments for saving refyre state
+    parser.add_argument("-s", '--save', help = "save the refyre state locally")
+
+    args = parser.parse_args(argv)
+
+    if args.recipe != None:
+        RecipePreprocessor(args.recipe)
 
     ref = Refyre(input_specs = args.input, output_specs = args.output)
 
-cli()
+    if args.save:
+        ref.save()
+
+if __name__ == '__main__':
+    sys.exit(main(sys.argv[1:]))
```

### Comparing `refyre-0.0.1.2/refyre/core/RecipePreprocessor.py` & `refyre-0.0.1.3/refyre/core/RecipePreprocessor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from pathlib import Path
 import sys
 import venv
 import site
+
 from refyre.utils import optional_dependencies
 from refyre import Refyre
+from refyre.config import logger
+
 from pip._internal import main as pip_main
 import subprocess
+import shutil
 
 def create_virtualenv_and_install_requirements(venv_path, requirements_file):
     # Create the virtual environment
     venv_builder = venv.EnvBuilder(with_pip=True)
     venv_builder.create(venv_path)
 
     # Activate the virtual environment
     activate_script = (
         Path(venv_path) / "Scripts" / "activate" if sys.platform == "win32"
         else Path(venv_path) / "bin" / "activate"
     )
     activate_cmd = f"source {activate_script} && python -m pip"
     
     # Install the requirements using pip within the virtual environment
-    print("installing reqs")
+    logger.debug("installing reqs")
     pip_install_cmd = f"{activate_cmd} install -r {requirements_file}"
     subprocess.run(pip_install_cmd, shell=True, check=True)
 
 class RecipePreprocessor:
     def __new__(self, recipe_path):
         '''
             Performs all the recipe path preprocessing, and then 
@@ -37,35 +41,62 @@
             import yaml 
 
             assert Path(recipe_path).exists(), f"The input file you were trying to access - {recipe_path} - does NOT exist"
 
             recipe_dict = None
             with open(recipe_path, 'r') as f:
                 recipe_dict = yaml.safe_load(f)
+                logger.debug(recipe_dict)
             
             '''
             Currently, a recipe consists of attributes:
 
                 input-spec: a filepath to the input spec
                 base-dir: filepath to the base directory / entry point you want your program to see
                 env: a description of the environment you want to setup, with two attributes
                     - name: name of the environment
                     - requirements: requirements file
 
             '''
 
-            print(recipe_dict)
-            print(recipe_dict['env']['name'])
+            logger.debug(recipe_dict)
+            logger.debug(recipe_dict['env']['name'])
 
             #Setup the base directories based on an input spec
-            #ref = Refyre.Refyre(input_specs = [recipe_dict["input-spec"]])
+            logger.debug(f'Sending to: {recipe_dict["input-spec"]}')
 
-            #Create the env if it doesn't exist already:
+
+            #Current base directory is assumed to be CWD
+            '''
+            if 'base-dir' and Path(recipe_dict['base-dir']) != Path.cwd():
+                current_base_dir = Path.cwd()
+
+                logger.debug(f'{sys.path}, {current_base_dir.resolve()}')
+                sys.path.remove(str(current_base_dir.resolve()))
+
+                sys.path.append(str(Path(recipe_dict['base-dir'].resolve())))
+                logger.debug()
+            '''
+
+            ref = Refyre.Refyre(input_specs = [recipe_dict["input-spec"]])
+
+            #Create the env if it doesn't exist already or needs to be refreshed
+            venv_path = recipe_dict['env']['name']
             if 'env' in recipe_dict and recipe_dict['env']:
                 if 'name' in recipe_dict['env']:
                     if not Path(recipe_dict['env']['name']).exists():
+                        create_virtualenv_and_install_requirements(venv_path, recipe_dict['env']['requirements'])
+                    elif 'refresh' in recipe_dict['env'] and recipe_dict['env']['refresh']:
+                        shutil.rmtree(recipe_dict['env']['name'])
                         create_virtualenv_and_install_requirements(recipe_dict['env']['name'], recipe_dict['env']['requirements'])
 
-            
-            #Setup the base dir
+            #Activate the env 
+            activate_script = (
+                Path(venv_path) / "Scripts" / "activate" if sys.platform == "win32"
+                else Path(venv_path) / "bin" / "activate"
+            )
+            activate_cmd = f"source {activate_script}"
+            subprocess.run(activate_cmd, shell=True, check=True)
+
             return ref
-            
+            
+
```

### Comparing `refyre-0.0.1.2/refyre/datastack/DataStack.py` & `refyre-0.0.1.3/refyre/datastack/DataStack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from refyre.utils import optional_dependencies 
 
 with optional_dependencies("warn"):
     import numpy as np 
     import pandas as pd
     import matplotlib.pyplot as plt
 
+# The PandasStack class is a Python class that creates a Pandas dataframe from a list of variables
+# using a mapper function.
 class PandasStack:
 
     def __init__(self, variables_array):
         self.variables_array = variables_array
     
     def create_dataframe(self, col_names, mapper_func):
         '''
```

### Comparing `refyre-0.0.1.2/refyre/fgraph/FileGraph.py` & `refyre-0.0.1.3/refyre/graph/FileGraph.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.2/refyre/fgraph/FileGraphNode.py` & `refyre-0.0.1.3/refyre/graph/FileGraphNode.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,29 @@
         Problem: There may be multiple root "entry" directories the user many want to be 
         able to target.
 
         Solution: We abstract that away in the graph.
 
         We will have one virtual "root" node stringing together all the other entry points.
     '''
-    def __init__(self, children = [], pattern = "", directory = "", type = "", name = "", is_root = False, flags = "", serialize = "", imports="", mode = "", link="", alias=""):
+    def __init__(self, children = [], pattern = "", directory = "", type = "", name = "", is_root = False, flags = "", serialize = "", imports="", mode = "", link="", alias="", limit = ""):
         self.children = children
 
         self.pattern = pattern #fnmatch.translate(pattern) #Add this attribute to handle glob pattern recognition
         self.directory = directory
         self.type = type
         self.name = name
         self.is_root = is_root
         self.flags = flags
         self.serialize = serialize
         self.imports = imports
         self.mode = mode
         self.link = link
         self.alias = alias
+        self.limit = limit
 
 
     def add_child(self, child):
         assert isinstance(child, FileGraphNode), "Children of FileGraphNode should only be FileGraphNodes"
         
         self.children.append(child)
```

### Comparing `refyre-0.0.1.2/refyre/reader/Lexer.py` & `refyre-0.0.1.3/refyre/reader/Lexer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from pathlib import Path
 from .cogs.lexer_utils import split_string_ignore_quotes, find_missing_separator
 from .cogs.LexerToken import Token
 import fnmatch
+from refyre.config import logger
 
 class Lexer:
     '''
         refyre's static lexer 
 
         Fundamental assumptions:
              - There are 4 spaces / tab. On some systems, there are 8, hence I've made a SPACES_PER_TAB variable that can be adjusted
@@ -21,24 +22,34 @@
         get rid of the unnecessary clutter.
         '''
 
         #Remove any multiline comments
         multiline_removal_pattern = r"'''[\s\S]*?'''"
         updated_content = re.sub(multiline_removal_pattern, '', input_str)
 
+
+        split_lines = updated_content.split('\n')
+
         #Remove any single line comments
         singleline_removal_pattern = r'#.*$'
-        updated_content = re.sub(singleline_removal_pattern, '', updated_content)
+        
+        updated_content = [re.sub(singleline_removal_pattern, '', l) for l in split_lines] 
 
         #Remove any purely whitespace lines
         whitespace_pattern = r'^\s*$'
-        updated_content = re.sub(whitespace_pattern, '', updated_content).strip()
+
+        updated_content = [re.sub(whitespace_pattern, '', l) for l in updated_content]
+        updated_content = [l for l in updated_content if l != '']
+        updated_content = '\n'.join(updated_content)
+
 
         #Remove any stay newlines
         updated_content = re.sub(r'\n+', '\n', updated_content)
+
+
         return updated_content
 
     def extract_line_data(line):
         '''
             Packages all the important line data into a Token()
             object
         '''
@@ -55,23 +66,23 @@
             print(f"ERROR: The lexer has found that some of the attributes don't have a '|' between them. This is a necessary, and will directly alter Lexer output if not fixed. Here's the attributes to check for:\n\n ")
             for w in p:
                 print(w)
 
             print(f"\nHere's the line we detected the error on: {line.strip()}")
             print('Make sure that there\'s a bar between all parts. For example, dir="a"name="k" is incorrect, while dir="a"|name="k" is.')
             print('Aborting ...')
-            exit(1)
+            raise Exception("Error in bracketing.")
 
 
         try:
             matches = re.search(inside_bracket_pattern, line).group(1)
         except AttributeError as e:
             print(f"ERROR: The lexer attempted to parse line {line} but couldn't find a match. Can you make sure that you have opening and closing brackets? ('[',']')")
             print('Aborting ...')
-            exit(1)
+            raise Exception("Error in parsing lines.")
 
 
         match = split_string_ignore_quotes(matches)
         dict_of_args = {}
 
 
         #Extract the key and value of each item, while accounting for potential spaces
@@ -83,23 +94,23 @@
 
             try:
                 key = matches.group(1)
             except AttributeError as e:
                 print("ERROR: it looks like you're missing a key attribute. Check to make sure each attribute and value have an '=' sign between them, and are in \"\".")
                 print(f"The error happened on line: {line.strip()}, when we tried to handle match {arg}")
                 print('Aborting ...')
-                exit(1)
+                raise Exception("Missing a key attribute")
 
             try:
                 val = matches.group(2)
             except AttributeError as e:
                 print("ERROR: it looks like you're missing a val attribute. Check to make sure each attribute and value have an '=' sign between them, and are in \"\".")
                 print(f"The error happened on line: {line.strip()}, when we tried to handle match {arg}")
                 print('Aborting ...')
-                exit(1)
+                raise Exception("Missing a val attribute")
 
             dict_of_args[key] = val
 
         #Grab the tab counts - we grab spaces, and count total
         space_pattern = r'^(\s*)\[.*\]'
 
         num_spaces = len(re.match(space_pattern, line).group(1))
@@ -109,15 +120,15 @@
 
         try:
             t = Token(num_spaces // Lexer.SPACES_PER_TAB, **dict_of_args)
         except TypeError as e:
             print(f"ERROR: The lexer failed to read one of the attributes. It's most likely because you typed one of the attributes wrong. Here's the full error message below.")
             print(e)
             print('Aborting ...')
-            exit(1)
+            raise Exception("Lexer failed to read attribute")
 
         return t
 
     def lex(input_file):
         '''
             Performs "lexical analysis", a.k.a grabs all the important information 
             from each line
@@ -126,15 +137,18 @@
             raise Exception(f"The input file path to the spec at {input_file} doesn't exist or is a directory!")
 
         with open(input_file, "r") as f:
             txt = f.read()
             cleaned_lines = Lexer.preprocess(txt)
             cleaned_lines = cleaned_lines.split('\n')
 
+            logger.debug(cleaned_lines)
         tokens = []
         for line in cleaned_lines:
             tokens.append(Lexer.extract_line_data(line))
+
             
+        logger.debug(tokens)
         return tokens
 
     def __new__(self, input_file):
         return Lexer.lex(input_file)
```

### Comparing `refyre-0.0.1.2/refyre/reader/Parser.py` & `refyre-0.0.1.3/refyre/reader/Parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from .Lexer import Lexer
 from .cogs.LexerToken import Token
 
-from refyre.fgraph import FileGraphNode
+from refyre.graph import FileGraphNode
 from pathlib import Path
+from refyre.config import logger
+from tqdm import tqdm
 
 
 #Utility stack (LIFO) data stucture methods
 def push(stack, item):
     stack.append(item)
 
 def pop(stack):
@@ -18,21 +20,27 @@
     '''
     def parse(tokens, INF = -10, ):
         '''
         Things to note: 
             - Floor for tab depth is set to be -10. If it goes beyond this, ...
             the circus would really love to hire their new rising clown.
         '''
+
+        #Ensure that the tokens spacing is proper, i.e no crazy tabs to the front
+        assert tokens[0].tab_level == 0, "There should be no tabs for the first line"
+        for i in range(1, len(tokens)):
+            assert tokens[i].tab_level - tokens[i - 1].tab_level <= 1, f"Tab difference {i} {tokens[i].tab_level} and {i - 1} {tokens[i - 1].tab_level} is too high."
+
         stack = []
 
         #Push our virtual top
         push(stack, (FileGraphNode(is_root = True, children = []), INF))
 
         
-        for tok in tokens:
+        for tok in tqdm(tokens, desc = "Generating token stack", ncols = 100):
             cur = []
 
             #Resolve all the nodes with tab_level lower
             while tok.tab_level < stack[-1][1]:
                 top = pop(stack)
 
                 #Grab all the nodes with the same level
@@ -45,16 +53,16 @@
                 
                 #Now, we know that the next node, whatever it is, must have a lower level
                 stack[-1][0].add_children(cur)
 
                 #Clear the list
                 cur.clear()
 
-            print('imports', tok.imports, tok.link)
-            push(stack, (FileGraphNode(children = list([]), pattern = tok.pattern, directory = tok.directory, type = tok.dirtype, name = tok.name, is_root = Path(tok.directory).exists(), flags = tok.flags, serialize = tok.serialize, imports = tok.imports, mode = tok.mode, link = tok.link, alias = tok.alias) , tok.tab_level))
+            logger.debug(f'imports {tok.imports} {tok.link}')
+            push(stack, (FileGraphNode(children = list([]), pattern = tok.pattern, directory = tok.directory, type = tok.dirtype, name = tok.name, is_root = Path(tok.directory).exists(), flags = tok.flags, serialize = tok.serialize, imports = tok.imports, mode = tok.mode, link = tok.link, alias = tok.alias, limit = tok.limit) , tok.tab_level))
 
         #Compress the remainder of the stack
         while len(stack) > 1: 
 
             top = pop(stack)
             cur = []
```

### Comparing `refyre-0.0.1.2/refyre/reader/PatternGenerator.py` & `refyre-0.0.1.3/refyre/reader/PatternGenerator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import fnmatch
 import re
+from .ExpressionGenerator import ExpressionGenerator
+from refyre.config import logger
 
 class PatternGenerator:
     '''
         The pattern generator is designed to parse all pattern based 
         strings and return regex versions of them that can be used to 
         pattern match.
 
@@ -13,32 +15,64 @@
 
         A glob string will come in the normal form. A regex string will start with an r before the actual pattern.
 
         ex: "a?.txt" is a glob pattern. "ra?.txt" is regex.
 
     '''
     def is_valid_regex(pattern_string):
+        logger.debug(pattern_string)
         if pattern_string.startswith('r'):
             try:
                 re.compile(pattern_string[1:])
-            except re.error:
+            except re.error as e:
+                logger.error(e)
                 return False
-        else:
+        elif pattern_string.startswith('g'):
             try:
-                re.compile(fnmatch.translate(pattern_string))
-            except re.error:
+                re.compile(fnmatch.translate(pattern_string[1:]))
+            except re.error as e:
+                logger.error(e)
+                return False
+        else:
+            if not PatternGenerator.is_valid_genexp(pattern_string):
                 return False
-
         return True
 
+    def is_valid_genexp(expression):
+        return ExpressionGenerator.is_valid_genexp(expression)
+    
+    def convert_generator_expression(expression):
+        return ExpressionGenerator.convert_generator_expression(expression)
+
+    def get_pattern_type(pattern_string):
+        if pattern_string.startswith('r'):
+            return "regex"
+
+        if pattern_string.startswith('g'):
+            return "glob"
+        
+        #Handle generator expressions
+        if not ExpressionGenerator.is_null_generator(pattern_string):
+            return "generator_expression"
+
+        #Else, the string is a normal string
+        return "normal_string" 
+
     def __new__(self, pattern_string):
         '''
             Takes in an input pattern string and returns the appropriate regex pattern.
 
         '''
         if pattern_string.startswith('r'):
-            print('regex')
+            logger.debug('regex')
             return pattern_string[1:]
 
-        #Clear out any leading / trailing spaces 
-        print('glob')
-        return '' if pattern_string == '' else fnmatch.translate(pattern_string.strip())
+        if pattern_string.startswith('g'):
+            logger.debug('glob')
+            return fnmatch.translate(pattern_string[1:])
+        
+        #Handle generator expressions
+        if not ExpressionGenerator.is_null_generator(pattern_string):
+            return ExpressionGenerator.convert_generator_expression(pattern_string)
+
+        #Else, the string is a normal string
+        return pattern_string
```

### Comparing `refyre-0.0.1.2/refyre/reader/cogs/LexerToken.py` & `refyre-0.0.1.3/refyre/reader/cogs/LexerToken.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import fnmatch
 
 class Token:
     '''
         A single Lexer token
     '''
-    def __init__(self, tab_level, pattern = "", dir = "",  type = "", name = "", flags = "", serialize="", imports="", mode = "", link = "", alias = ""):
+    def __init__(self, tab_level, pattern = "", dir = "",  type = "", name = "", flags = "", serialize="", imports="", mode = "", link = "", alias = "", limit = ""):
         self.tab_level = tab_level
         self.pattern = pattern
         self.directory = dir
         self.dirtype = type
         self.name = name
         self.flags = flags
         self.serialize = serialize
         self.imports = imports
         self.mode = mode
         self.link = link
         self.alias = alias
+        self.limit = limit
 
 
     def __repr__(self):
         return f"Token(tab_level={self.tab_level},pattern={self.pattern},directory={self.directory},dirtype={self.dirtype},name={self.name},flags={self.flags},serialize={self.serialize})"
```

### Comparing `refyre-0.0.1.2/refyre/reader/cogs/VariableParser.py` & `refyre-0.0.1.3/refyre/cluster/cogs/VariableParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import re 
-from refyre.fcluster import FileCluster
+from refyre.cluster import FileCluster
+from refyre.config import logger
 
 class VariableParser:
     '''
     A static class parser designed specifically to identify and evaluate expressions
     relating to variables. This class is the most relevant to the
     node.name attribute, and will normally be used to parse it.
     '''
     def extract_variable_data(expression):
         pattern1 = r'^([\w-]+)(?:\[(\d+)?:(\d+)?(?:\:(\d+))?\])?$'
         pattern2 = r'^([\w-]+)\[(\d+)\]$'
 
         match1 = re.match(pattern1, expression)
         match2 = re.match(pattern2, expression)
 
-        print(match1, match2)
+        logger.debug(f'{match1}, {match2}')
 
         if match1:
-            print('match1')
+            logger.debug('match1')
             name = match1.group(1)
             start = match1.group(2)
             stop = match1.group(3)
             step = match1.group(4)
 
             return name, start, stop, step
 
         elif match2:
-            print('match2')
+            logger.debug('match2')
             name = match2.group(1)
             start = match2.group(2)
             stop = str(int(start) + 1)
             step = None
 
             return name, start, stop, step
 
@@ -43,15 +44,15 @@
             - Var: the FileCluster variable we seek to obtain a slice from
             - Start: the start of the slice, 0 if nothing specified
             - Stop: the stop of the slice, length if nothing specified
             - Step: the step of the slice, 1 if nothing specified 
         
         Returns a slice object involving the three indices
         '''
-        assert type(var) == FileCluster.FileCluster
+        assert type(var) == FileCluster
 
         start, stop, step = 0 if start is None else int(start), len(var) if stop is None else int(stop), 1 if step is None else int(step)
         return slice(start, stop, step), start, stop, step
     
     def __new__(self, expression, variable_dict):
         '''
             Hijack the '__new__' method (usually used in constructors)
```

### Comparing `refyre-0.0.1.2/refyre/reader/cogs/lexer_utils.py` & `refyre-0.0.1.3/refyre/reader/cogs/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.2/refyre/utils/clone.py` & `refyre-0.0.1.3/refyre/utils/clone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from refyre.utils import optional_dependencies 
-from refyre.fcluster import FileCluster #Time to use the power of our variables :)
+from refyre.cluster import FileCluster #Time to use the power of our variables :)
 from pathlib import Path
+from refyre.config import logger
 import random
 import shutil
 
 def clone_node(url, fp):
     import git 
 
-    print("GEET", git)
+    logger.debug(f"GEET {git}")
 
 
     #Ensure no file conflicts
     rand_num = ''.join(["{}".format(random.randint(0, 9)) for num in range(0, 20)])
     tmp_empty = fp / f'tmp{rand_num}'
 
 
-    print('Cloning to ', tmp_empty)
+    logger.debug(f'Cloning to {tmp_empty}')
     git.Repo.clone_from(url, tmp_empty)
 
-    mv_var = FileCluster(input_paths = [tmp_empty], input_patterns = ['*'])
+    mv_var = FileCluster(input_paths = [tmp_empty], input_patterns = ['g*'])
 
     mv_var.move(tmp_empty.parent)
 
     tmp_empty.rmdir()
```

