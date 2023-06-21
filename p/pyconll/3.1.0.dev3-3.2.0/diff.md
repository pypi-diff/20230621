# Comparing `tmp/pyconll-3.1.0.dev3.tar.gz` & `tmp/pyconll-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconll-3.1.0.dev3.tar", last modified: Mon Oct 25 19:59:42 2021, max compression
+gzip compressed data, was "pyconll-3.2.0.tar", last modified: Wed Jun 21 03:30:31 2023, max compression
```

## Comparing `pyconll-3.1.0.dev3.tar` & `pyconll-3.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:59:42.342703 pyconll-3.1.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9477 2021-10-25 19:59:42.342703 pyconll-3.1.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6081 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/README
--rw-r--r--   0 runner    (1001) docker     (121)     7015 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     7345 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:59:42.338703 pyconll-3.1.0.dev3/pyconll/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/conllable.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/load.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:59:42.338703 pyconll-3.1.0.dev3/pyconll/tree/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6773 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/tree/_treebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/tree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:59:42.338703 pyconll-3.1.0.dev3/pyconll/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5384 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/unit/conll.py
--rw-r--r--   0 runner    (1001) docker     (121)    12239 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/unit/sentence.py
--rw-r--r--   0 runner    (1001) docker     (121)    26467 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/unit/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     8229 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/pyconll/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 19:59:42.338703 pyconll-3.1.0.dev3/pyconll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9477 2021-10-25 19:59:42.000000 pyconll-3.1.0.dev3/pyconll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-10-25 19:59:42.000000 pyconll-3.1.0.dev3/pyconll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-25 19:59:42.000000 pyconll-3.1.0.dev3/pyconll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-25 19:59:42.000000 pyconll-3.1.0.dev3/pyconll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-25 19:59:42.342703 pyconll-3.1.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2021-10-25 19:59:37.000000 pyconll-3.1.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:31.701292 pyconll-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-06-21 03:30:26.000000 pyconll-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-21 03:30:26.000000 pyconll-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9339 2023-06-21 03:30:31.701292 pyconll-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6000 2023-06-21 03:30:26.000000 pyconll-3.2.0/README
+-rw-r--r--   0 runner    (1001) docker     (122)     6938 2023-06-21 03:30:26.000000 pyconll-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7228 2023-06-21 03:30:26.000000 pyconll-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:31.697292 pyconll-3.2.0/pyconll/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/conllable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:31.701292 pyconll-3.2.0/pyconll/tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/tree/_treebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/tree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:31.701292 pyconll-3.2.0/pyconll/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/unit/conll.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12810 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/unit/sentence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26836 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/unit/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8229 2023-06-21 03:30:26.000000 pyconll-3.2.0/pyconll/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:30:31.697292 pyconll-3.2.0/pyconll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9339 2023-06-21 03:30:31.000000 pyconll-3.2.0/pyconll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-21 03:30:31.000000 pyconll-3.2.0/pyconll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 03:30:31.000000 pyconll-3.2.0/pyconll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-21 03:30:31.000000 pyconll-3.2.0/pyconll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 03:30:31.701292 pyconll-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-21 03:30:26.000000 pyconll-3.2.0/setup.py
```

### Comparing `pyconll-3.1.0.dev3/LICENSE` & `pyconll-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconll-3.1.0.dev3/PKG-INFO` & `pyconll-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 1.2
 Name: pyconll
-Version: 3.1.0.dev3
+Version: 3.2.0
 Summary: Read and manipulate CoNLL files
 Home-page: https://github.com/pyconll/pyconll
 Author: Matias Grioni
 Author-email: matgrioni@gmail.com
 License: MIT
 Description: |Build Status| |Coverage Status| |Documentation Status| |Version|
         |gitter|
         
         pyconll
         -------
         
-        *Easily work with **CoNLL** files using the familiar syntax of
-        **python**.*
+        *Easily work with* **CoNLL** *files using the familiar syntax of*
+        **python**\ *.*
         
         Links
         '''''
         
         -  `Homepage <https://pyconll.github.io>`__
         -  `Documentation <https://pyconll.readthedocs.io/>`__
         
         Installation
         ~~~~~~~~~~~~
         
         As with most python packages, simply use ``pip`` to install from PyPi.
-        
         ::
         
-            pip install pyconll
+           pip install pyconll
         
         ``pyconll`` is also available as a conda package on the ``pyconll``
         channel. Only packages 2.2.0 and newer are available on conda at the
         moment.
         
         ::
         
-            conda install -c pyconll pyconll
+           conda install -c pyconll pyconll
         
-        pyconll supports Python 3.6 and greater, starting in version 3.0.0. In
-        general pyconll will focus development efforts on officially supported
-        python versions. Python 3.5 reached end of support in October 2020.
+        pyconll supports Python 3.8 and greater. In general, pyconll will focus
+        development efforts on officially supported python versions.
         
         Use
         ~~~
         
         This tool is intended to be a **minimal**, **low level**, **expressive**
         and **pragmatic** library in a widely used programming language. pyconll
         creates a thin API on top of raw CoNLL annotations that is simple and
@@ -58,38 +56,38 @@
         a smooth development workflow no matter the dataset size (performs about
         25%-35% faster than other comparable packages)
         
         See the following code example to understand the basics of the API.
         
         .. code:: python
         
-            # This snippet finds sentences where a token marked with part of speech 'AUX' are
-            # governed by a NOUN. For example, in French this is a less common construction
-            # and we may want to validate these examples because we have previously found some
-            # problematic examples of this construction.
-            import pyconll
-        
-            train = pyconll.load_from_file('./ud/train.conllu')
-        
-            review_sentences = []
-        
-            # Conll objects are iterable over their sentences, and sentences are iterable
-            # over their tokens. Sentences also de/serialize comment information.
-            for sentence in train:
-                for token in sentence:
-        
-                    # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
-                    # can be indexed by a token's id. We must check that the token is not the
-                    # root token, whose id, '0', cannot be looked up.
-                    if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
-                        review_sentences.append(sentence)
-        
-            print('Review the following sentences:')
-            for sent in review_sentences:
-                print(sent.id)
+           # This snippet finds sentences where a token marked with part of speech 'AUX' are
+           # governed by a NOUN. For example, in French this is a less common construction
+           # and we may want to validate these examples because we have previously found some
+           # problematic examples of this construction.
+           import pyconll
+        
+           train = pyconll.load_from_file('./ud/train.conllu')
+        
+           review_sentences = []
+        
+           # Conll objects are iterable over their sentences, and sentences are iterable
+           # over their tokens. Sentences also de/serialize comment information.
+           for sentence in train:
+              for token in sentence:
+        
+              # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
+              # can be indexed by a token's id. We must check that the token is not the
+              # root token, whose id, '0', cannot be looked up.
+              if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
+                 review_sentences.append(sentence)
+            
+           print('Review the following sentences:')
+           for sent in review_sentences:
+              print(sent.id)
         
         A full definition of the API can be found in the
         `documentation <https://pyconll.readthedocs.io/>`__ or use the `quick
         start <https://pyconll.readthedocs.io/en/stable/starting.html>`__ guide
         for a focused introduction.
         
         Uses and Limitations
@@ -185,8 +183,8 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
```

### Comparing `pyconll-3.1.0.dev3/README` & `pyconll-3.2.0/README`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [Build Status] [Coverage Status] [Documentation Status] [Version]
 [gitter]
 
-
 pyconll
 
-_Easily work with CONLL files using the familiar syntax of PYTHON._
+Easily work with CoNLL files using the familiar syntax of python.
 
 Links
 
 -   Homepage
 -   Documentation
 
 Installation
@@ -18,22 +17,21 @@
     pip install pyconll
 
 pyconll is also available as a conda package on the pyconll channel.
 Only packages 2.2.0 and newer are available on conda at the moment.
 
     conda install -c pyconll pyconll
 
-pyconll supports Python 3.6 and greater, starting in version 3.0.0. In
-general pyconll will focus development efforts on officially supported
-python versions. Python 3.5 reached end of support in October 2020.
+pyconll supports Python 3.8 and greater. In general, pyconll will focus
+development efforts on officially supported python versions.
 
 Use
 
-This tool is intended to be a MINIMAL, LOW LEVEL, EXPRESSIVE and
-PRAGMATIC library in a widely used programming language. pyconll creates
+This tool is intended to be a minimal, low level, expressive and
+pragmatic library in a widely used programming language. pyconll creates
 a thin API on top of raw CoNLL annotations that is simple and intuitive.
 
 It offers the following features: * Regular CI testing and validation
 against all UD v2.x versions. * A strong domain model that includes
 CoNLL sources, Sentences, Tokens, Trees, etc. * A typed API for better
 development experience and better semantics. * A focus on usability and
 simplicity in design (no dependencies) * Performance optimizations for a
@@ -133,8 +131,7 @@
     for master. After validating these results, create a tag
     corresponding to the next version number and push the tag.
 -   Create a new release from this tag from the Releases page. On
     creating this release, two workflows will start. One releases to
     pypi, and the other releases to conda.
 -   Validate these workflows pass, and the package is properly released
     on both platforms.
-
```

### Comparing `pyconll-3.1.0.dev3/README.md` & `pyconll-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 `pyconll` is also available as a conda package on the `pyconll` channel. Only packages 2.2.0 and newer are available on conda at the moment.
 
 ```
 conda install -c pyconll pyconll
 ```
 
-pyconll supports Python 3.6 and greater, starting in version 3.0.0. In general pyconll will focus development efforts on officially supported python versions. Python 3.5 reached end of support in October 2020.
+pyconll supports Python 3.8 and greater. In general, pyconll will focus development efforts on officially supported python versions.
 
 
 ### Use
 
 This tool is intended to be a **minimal**, **low level**, **expressive** and **pragmatic** library in a widely used programming language. pyconll creates a thin API on top of raw CoNLL annotations that is simple and intuitive.
 
 It offers the following features:
```

### Comparing `pyconll-3.1.0.dev3/README.rst` & `pyconll-3.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 |Build Status| |Coverage Status| |Documentation Status| |Version|
 |gitter|
 
 pyconll
 -------
 
-*Easily work with **CoNLL** files using the familiar syntax of
-**python**.*
+*Easily work with* **CoNLL** *files using the familiar syntax of*
+**python**\ *.*
 
 Links
 '''''
 
 -  `Homepage <https://pyconll.github.io>`__
 -  `Documentation <https://pyconll.readthedocs.io/>`__
 
 Installation
 ~~~~~~~~~~~~
 
 As with most python packages, simply use ``pip`` to install from PyPi.
-
 ::
 
-    pip install pyconll
+   pip install pyconll
 
 ``pyconll`` is also available as a conda package on the ``pyconll``
 channel. Only packages 2.2.0 and newer are available on conda at the
 moment.
 
 ::
 
-    conda install -c pyconll pyconll
+   conda install -c pyconll pyconll
 
-pyconll supports Python 3.6 and greater, starting in version 3.0.0. In
-general pyconll will focus development efforts on officially supported
-python versions. Python 3.5 reached end of support in October 2020.
+pyconll supports Python 3.8 and greater. In general, pyconll will focus
+development efforts on officially supported python versions.
 
 Use
 ~~~
 
 This tool is intended to be a **minimal**, **low level**, **expressive**
 and **pragmatic** library in a widely used programming language. pyconll
 creates a thin API on top of raw CoNLL annotations that is simple and
@@ -50,38 +48,38 @@
 a smooth development workflow no matter the dataset size (performs about
 25%-35% faster than other comparable packages)
 
 See the following code example to understand the basics of the API.
 
 .. code:: python
 
-    # This snippet finds sentences where a token marked with part of speech 'AUX' are
-    # governed by a NOUN. For example, in French this is a less common construction
-    # and we may want to validate these examples because we have previously found some
-    # problematic examples of this construction.
-    import pyconll
-
-    train = pyconll.load_from_file('./ud/train.conllu')
-
-    review_sentences = []
-
-    # Conll objects are iterable over their sentences, and sentences are iterable
-    # over their tokens. Sentences also de/serialize comment information.
-    for sentence in train:
-        for token in sentence:
-
-            # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
-            # can be indexed by a token's id. We must check that the token is not the
-            # root token, whose id, '0', cannot be looked up.
-            if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
-                review_sentences.append(sentence)
-
-    print('Review the following sentences:')
-    for sent in review_sentences:
-        print(sent.id)
+   # This snippet finds sentences where a token marked with part of speech 'AUX' are
+   # governed by a NOUN. For example, in French this is a less common construction
+   # and we may want to validate these examples because we have previously found some
+   # problematic examples of this construction.
+   import pyconll
+
+   train = pyconll.load_from_file('./ud/train.conllu')
+
+   review_sentences = []
+
+   # Conll objects are iterable over their sentences, and sentences are iterable
+   # over their tokens. Sentences also de/serialize comment information.
+   for sentence in train:
+      for token in sentence:
+
+      # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
+      # can be indexed by a token's id. We must check that the token is not the
+      # root token, whose id, '0', cannot be looked up.
+      if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
+         review_sentences.append(sentence)
+    
+   print('Review the following sentences:')
+   for sent in review_sentences:
+      print(sent.id)
 
 A full definition of the API can be found in the
 `documentation <https://pyconll.readthedocs.io/>`__ or use the `quick
 start <https://pyconll.readthedocs.io/en/stable/starting.html>`__ guide
 for a focused introduction.
 
 Uses and Limitations
```

### Comparing `pyconll-3.1.0.dev3/pyconll/_parser.py` & `pyconll-3.2.0/pyconll/_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 An internal module for common parsing logic, which is currently creating
 Sentence objects from an iterator that returns CoNLL source lines. This logic
 can then be used in the Conll class or in pyconll.load.
 """
 
 from typing import Iterable, Iterator
 
+from pyconll.exception import ParseError
 from pyconll.unit.sentence import Sentence
 
 
-def _create_sentence(sent_lines: Iterable[str]) -> Sentence:
+def _create_sentence(sent_lines: Iterable[str], line_num: int) -> Sentence:
     """
     Creates a Sentence object given the current state of the source iteration.
 
     Args:
         sent_lines: An iterable of the lines that make up the source.
+        line_num: The current line number the sentence starts at, for logging
+            purposes.
 
     Returns:
         The created Sentence.
 
     Raises:
         ParseError: If the sentence source is not valid.
     """
     sent_source = '\n'.join(sent_lines)
-    sentence = Sentence(sent_source)
+    try:
+        sentence = Sentence(sent_source)
+    except ParseError as err:
+        raise ParseError(
+            f'Failed to create sentence at line {line_num}') from err
 
     return sentence
 
 
 def iter_sentences(lines_it: Iterable[str]) -> Iterator[Sentence]:
     """
     Iterate over the constructed sentences in the given lines.
@@ -40,23 +47,26 @@
     Yields:
         An iterator over the constructed Sentence objects found in the source.
 
     Raises:
         ValueError: If there is an error constructing the Sentence.
     """
     sent_lines = []
-    for line in lines_it:
+    last_empty_line = -1
+    for i, line in enumerate(lines_it):
         line = line.strip()
 
         # Collect all lines until there is a blank line. Then all the
         # collected lines were between blank lines and are a sentence.
         if line:
             sent_lines.append(line)
-        elif sent_lines:
-            sentence = _create_sentence(sent_lines)
-            sent_lines.clear()
+        else:
+            if sent_lines:
+                sentence = _create_sentence(sent_lines, last_empty_line + 2)
+                sent_lines.clear()
+                yield sentence
 
-            yield sentence
+            last_empty_line = i
 
     if sent_lines:
-        sentence = _create_sentence(sent_lines)
+        sentence = _create_sentence(sent_lines, last_empty_line)
         yield sentence
```

### Comparing `pyconll-3.1.0.dev3/pyconll/conllable.py` & `pyconll-3.2.0/pyconll/conllable.py`

 * *Files identical despite different names*

### Comparing `pyconll-3.1.0.dev3/pyconll/tree/_treebuilder.py` & `pyconll-3.2.0/pyconll/tree/_treebuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         """
         self._assert_initialization_status()
 
         try:
             self.current = self.current[i]
         except IndexError as e:
             raise IndexError(
-                '{}-th child is out of range. There are {} children on this node'
-                .format(i, len(self.current))) from e
+                f'{i}-th child is out of range. There are {len(self.current)} children on this node'
+            ) from e
 
     def move_to_root(self) -> None:
         """
         Move the internal cursor to the root of the entire tree.
 
         Raises:
             ValueError: If the TreeBuilder's root has not been initialized.
@@ -117,16 +117,16 @@
         self._assert_initialization_status()
         self._copy_if_necessary()
 
         try:
             del self.current._children[i]
         except IndexError as e:
             raise IndexError(
-                '{}-th child is out of range. There are {} children on this node'
-                .format(i, len(self.current))) from e
+                f'{i}-th child is out of range. There are {len(self.current)} children on this node'
+            ) from e
 
     def add_child(self, data: T, move: bool = False) -> None:
         """
         Adds a child to the current cursor location's node.
 
         Children indices are directly related to the order of their creation.
```

### Comparing `pyconll-3.1.0.dev3/pyconll/tree/tree.py` & `pyconll-3.2.0/pyconll/tree/tree.py`

 * *Files identical despite different names*

### Comparing `pyconll-3.1.0.dev3/pyconll/unit/conll.py` & `pyconll-3.2.0/pyconll/unit/conll.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
     def conll(self) -> str:
         """
         Output the Conll object to a CoNLL-U formatted string.
 
         Returns:
             The CoNLL-U object as a string. This string will end in a newline.
+
+        Raises:
+            FormatError: If there are issues converting the sentences to the
+                CoNLL format.
         """
         # Add newlines along with sentence strings so that there is no need to
         # slice potentially long lists or modify strings.
         components = list(map(lambda sent: sent.conll(), self._sentences))
         components.append('')
 
         return '\n\n'.join(components)
```

### Comparing `pyconll-3.1.0.dev3/pyconll/unit/sentence.py` & `pyconll-3.2.0/pyconll/unit/sentence.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from collections import OrderedDict
 import re
 from typing import ClassVar, Dict, Iterator, List, Optional, Sequence, overload
 
 from pyconll.conllable import Conllable
+from pyconll.exception import FormatError, ParseError
 from pyconll.tree._treebuilder import TreeBuilder
 from pyconll.tree.tree import Tree
 from pyconll.unit.token import Token
 
 
 class Sentence(Sequence[Token], Conllable):
     """
@@ -60,15 +61,15 @@
         """
         lines = source.split('\n')
 
         self._meta: OrderedDict[str, Optional[str]] = OrderedDict()  # pylint: disable=E1136
         self._tokens: List[Token] = []
         self._ids_to_indexes: Dict[str, int] = {}
 
-        for line in lines:
+        for i, line in enumerate(lines):
             if line:
                 if line[0] == Sentence.COMMENT_MARKER:
                     kv_match = re.match(Sentence.KEY_VALUE_COMMENT_PATTERN,
                                         line)
 
                     if kv_match:
                         k = kv_match.group(1)
@@ -77,15 +78,21 @@
                     else:
                         singleton_match = re.match(
                             Sentence.SINGLETON_COMMENT_PATTERN, line)
                         if singleton_match:
                             k = singleton_match.group(1)
                             self._meta[k] = None
                 else:
-                    token = Token(line)
+                    try:
+                        token = Token(line)
+                    except ParseError as err:
+                        raise ParseError(
+                            f'Error creating token on line {i} for the current sentence'
+                        ) from err
+
                     self._tokens.append(token)
 
                     if token.id is not None:
                         self._ids_to_indexes[token.id] = len(self._tokens) - 1
 
     @property
     def id(self) -> Optional[str]:
@@ -159,15 +166,15 @@
 
         Args:
             key: The key for the comment.
             value: The value to associate with the key. If the comment is a
                 singleton, this field can be ignored or set to None.
         """
         if key == Sentence.TEXT_KEY:
-            raise ValueError('Key cannot be {}'.format(Sentence.TEXT_KEY))
+            raise ValueError(f'Key cannot be {Sentence.TEXT_KEY}')
 
         self._meta[key] = value
 
     def remove_meta(self, key: str) -> None:
         """
         Remove a metadata element associated with the Sentence.
 
@@ -175,15 +182,15 @@
             key: The name of the metadata / comment.
 
         Raises:
             KeyError: If the key is not present in the Sentence metadata.
             ValueError: If the text key is provided, regardless of presence.
         """
         if key == Sentence.TEXT_KEY:
-            raise ValueError('Key cannot be {}'.format(Sentence.TEXT_KEY))
+            raise ValueError(f'Key cannot be {Sentence.TEXT_KEY}')
 
         del self._meta[key]
 
     def to_tree(self) -> Tree[Token]:
         """
         Creates a Tree data structure from the current sentence.
 
@@ -211,16 +218,16 @@
             if token.head is not None:
                 try:
                     children_tokens[token.head].append(token)
                 except KeyError:
                     children_tokens[token.head] = [token]
             elif not (token.is_multiword() or token.is_empty_node()):
                 raise ValueError(
-                    'The current sentence is not fully defined as a tree and ' \
-                    'has a token with an empty head at {}'.format(token.id))
+                    'The current sentence is not fully defined as a tree and has a token with an '
+                    f'empty head at {token.id}')
 
         builder: TreeBuilder[Token] = TreeBuilder()
         if '0' in children_tokens:
             if len(children_tokens['0']) != 1:
                 raise ValueError(
                     'There should be exactly one root token in a sentence.')
 
@@ -263,27 +270,35 @@
 
     def conll(self) -> str:
         """
         Convert the sentence to a CoNLL-U representation.
 
         Returns:
             A string representing the Sentence in CoNLL-U format.
+
+        Raises:
+            FormatError: If the Sentence or underlying Tokens can not be
+                converted to the CoNLL format.
         """
         lines = []
         for meta in self._meta.items():
             if meta[1] is not None:
-                line = '{} {} = {}'.format(Sentence.COMMENT_MARKER, meta[0],
-                                           meta[1])
+                line = f'{Sentence.COMMENT_MARKER} {meta[0]} = {meta[1]}'
             else:
-                line = '{} {}'.format(Sentence.COMMENT_MARKER, meta[0])
+                line = f'{Sentence.COMMENT_MARKER} {meta[0]}'
 
             lines.append(line)
 
         for token in self._tokens:
-            lines.append(token.conll())
+            try:
+                lines.append(token.conll())
+            except FormatError as err:
+                raise FormatError(
+                    f'Error serializing sentence with id {self.id} on token \'{token.id}\'.'
+                ) from err
 
         return '\n'.join(lines)
 
     def __iter__(self) -> Iterator[Token]:
         """
         Iterate through all the tokens in the Sentence including multiword
         tokens.
```

### Comparing `pyconll-3.1.0.dev3/pyconll/unit/token.py` & `pyconll-3.2.0/pyconll/unit/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Defines the Token type and parsing and output logic. A Token is the based unit
 in CoNLL-U and so the data and parsing in this module is central to the CoNLL-U
 format.
 """
 
 import functools
-import itertools
 import math
 from typing import Callable, ClassVar, Dict, Optional, Set, Tuple
 
 from pyconll.conllable import Conllable
-from pyconll.exception import ParseError, FormatError
+from pyconll.exception import FormatError, ParseError
 
 
 def _unit_empty_map(value, empty):
     """
     Map unit values for CoNLL-U columns to a string or None if empty.
 
     Args:
@@ -42,16 +41,15 @@
         ParseError: If there was an error parsing the value. This happens when
             the value is None.
     """
     if v is not None:
         vs = set(v.split(v_delimiter))
         return vs
 
-    error_msg = 'Error parsing "{}" properly. Please check against CoNLL format spec.'.format(
-        v)
+    error_msg = f'Error parsing "{v}" properly. Please check against CoNLL format spec.'
     raise ParseError(error_msg)
 
 
 def _dict_empty_map(values, empty, delim, av_separator, v_delimiter):
     """
     Map dict values for CoNLL-U columns to a dict or empty dict if empty.
 
@@ -102,27 +100,27 @@
         Returns:
             The parsed value as a tuple.
 
         Raises:
             ParseError: If there was an error parsing the value as a tuple.
         """
         if v is None:
-            error_msg = ('Error parsing "{}" as tuple properly. Please check'
-                         'against CoNLL format spec').format(v)
-            raise ParseError(error_msg)
+            raise ParseError(
+                f'Error parsing "{v}" as tuple properly. Please check against CoNLL'
+                ' format spec')
 
         components = v.split(v_delimiter)
         left = size - len(components)
 
         if not strict and 0 <= left < size:
             vs = tuple(components + [None] * left)
         else:
-            error_msg = ('Error parsing "{}" as tuple properly. Please'
-                         'check against CoNLL format spec.').format(v)
-            raise ParseError(error_msg)
+            raise ParseError(
+                f'Error parsing "{v}" as tuple properly. Please check against CoNLL'
+                ' format spec.')
 
         return vs
 
     return _dict_tupled_empty_parser
 
 
 TUPLE_PARSER_MEMOIZE: Dict[int, Callable[[str, str], Tuple[Optional[str],
@@ -656,17 +654,16 @@
                 improper column values.
         """
         if source[-1] == '\n':
             source = source[:-1]
 
         fields = source.split(Token.FIELD_DELIMITER)
 
-        if len(fields) < 10:
-            error_msg = 'The columns per token line must be at least 10. Invalid line: {}'.format(
-                source)
+        if len(fields) != 10:
+            error_msg = f'The number of columns per token line must be 10. Invalid token: {source}'
             raise ParseError(error_msg)
 
         # Assign all the field values from the line to internal equivalents.
         self.id: str = fields[0]
 
         # If we can assume the form and lemma are empty, or if either of the
         # fields are not the empty token, then we can proceed as usual.
@@ -677,26 +674,29 @@
             self.lemma: Optional[str] = _unit_empty_map(fields[2], Token.EMPTY)
         else:
             self._form = fields[1]
             self.lemma = fields[2]
 
         self.upos: Optional[str] = _unit_empty_map(fields[3], Token.EMPTY)
         self.xpos: Optional[str] = _unit_empty_map(fields[4], Token.EMPTY)
-        self.feats: Dict[str, Optional[Set[str]]] = _dict_mixed_empty_map(
-            fields[5], Token.EMPTY, Token.COMPONENT_DELIMITER,
-            Token.AV_SEPARATOR, Token.V_DELIMITER)
+        self.feats: Dict[str,
+                         Set[str]] = _dict_empty_map(fields[5], Token.EMPTY,
+                                                     Token.COMPONENT_DELIMITER,
+                                                     Token.AV_SEPARATOR,
+                                                     Token.V_DELIMITER)
         self.head: Optional[str] = _unit_empty_map(fields[6], Token.EMPTY)
         self.deprel: Optional[str] = _unit_empty_map(fields[7], Token.EMPTY)
-        self.deps: Optional[str] = _unit_empty_map(fields[8], Token.EMPTY)
+        self.deps: Dict[str,
+                        Tuple[str, str, str, str]] = _dict_tupled_empty_map(
+                            fields[8], Token.EMPTY, Token.COMPONENT_DELIMITER,
+                            Token.AV_DEPS_SEPARATOR, Token.V_DEPS_DELIMITER, 4)
         self.misc: Dict[str, Optional[Set[str]]] = _dict_mixed_empty_map(
             fields[9], Token.EMPTY, Token.COMPONENT_DELIMITER,
             Token.AV_SEPARATOR, Token.V_DELIMITER)
 
-        self.extra_cols = fields[10:]
-
     @property
     def form(self) -> Optional[str]:
         """
         Provide the word form of this Token. This property is read only.
 
         Returns:
             The Token form.
@@ -729,33 +729,37 @@
         Convert this Token to its CoNLL-U representation.
 
         A Token's CoNLL-U representation is a line. Note that this method does
         not include a newline at the end.
 
         Returns:
             A string representing the Token in CoNLL-U format.
+
+        Raises:
+            FormatError: If the Token can not be converted to the CoNLL format.
         """
         # Transform the internal CoNLL-U representations back to text and
         # combine the fields.
         token_id = self.id
         form = _unit_conll_map(self.form, Token.EMPTY)
         lemma = _unit_conll_map(self.lemma, Token.EMPTY)
         upos = _unit_conll_map(self.upos, Token.EMPTY)
         xpos = _unit_conll_map(self.xpos, Token.EMPTY)
-        feats = _dict_mixed_conll_map(self.feats, Token.EMPTY,
-                                      Token.COMPONENT_DELIMITER,
-                                      Token.AV_SEPARATOR, Token.V_DELIMITER,
-                                      Token.BY_CASE_INSENSITIVE)
+        feats = _dict_conll_map(self.feats, Token.EMPTY,
+                                Token.COMPONENT_DELIMITER, Token.AV_SEPARATOR,
+                                Token.V_DELIMITER, Token.BY_CASE_INSENSITIVE)
         head = _unit_conll_map(self.head, Token.EMPTY)
         deprel = _unit_conll_map(self.deprel, Token.EMPTY)
-        deps = _unit_conll_map(self.deps, Token.EMPTY)
+        deps = _dict_tupled_conll_map(self.deps, Token.EMPTY,
+                                      Token.COMPONENT_DELIMITER,
+                                      Token.AV_DEPS_SEPARATOR,
+                                      Token.V_DEPS_DELIMITER, Token.BY_ID)
         misc = _dict_mixed_conll_map(self.misc, Token.EMPTY,
                                      Token.COMPONENT_DELIMITER,
                                      Token.AV_SEPARATOR, Token.V_DELIMITER,
                                      Token.BY_CASE_INSENSITIVE)
 
         items = [
             token_id, form, lemma, upos, xpos, feats, head, deprel, deps, misc
         ]
-        it = itertools.chain(items, self.extra_cols)
 
-        return Token.FIELD_DELIMITER.join(it)
+        return Token.FIELD_DELIMITER.join(items)
```

### Comparing `pyconll-3.1.0.dev3/pyconll/util.py` & `pyconll-3.2.0/pyconll/util.py`

 * *Files identical despite different names*

### Comparing `pyconll-3.1.0.dev3/pyconll.egg-info/PKG-INFO` & `pyconll-3.2.0/pyconll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 Metadata-Version: 1.2
 Name: pyconll
-Version: 3.1.0.dev3
+Version: 3.2.0
 Summary: Read and manipulate CoNLL files
 Home-page: https://github.com/pyconll/pyconll
 Author: Matias Grioni
 Author-email: matgrioni@gmail.com
 License: MIT
 Description: |Build Status| |Coverage Status| |Documentation Status| |Version|
         |gitter|
         
         pyconll
         -------
         
-        *Easily work with **CoNLL** files using the familiar syntax of
-        **python**.*
+        *Easily work with* **CoNLL** *files using the familiar syntax of*
+        **python**\ *.*
         
         Links
         '''''
         
         -  `Homepage <https://pyconll.github.io>`__
         -  `Documentation <https://pyconll.readthedocs.io/>`__
         
         Installation
         ~~~~~~~~~~~~
         
         As with most python packages, simply use ``pip`` to install from PyPi.
-        
         ::
         
-            pip install pyconll
+           pip install pyconll
         
         ``pyconll`` is also available as a conda package on the ``pyconll``
         channel. Only packages 2.2.0 and newer are available on conda at the
         moment.
         
         ::
         
-            conda install -c pyconll pyconll
+           conda install -c pyconll pyconll
         
-        pyconll supports Python 3.6 and greater, starting in version 3.0.0. In
-        general pyconll will focus development efforts on officially supported
-        python versions. Python 3.5 reached end of support in October 2020.
+        pyconll supports Python 3.8 and greater. In general, pyconll will focus
+        development efforts on officially supported python versions.
         
         Use
         ~~~
         
         This tool is intended to be a **minimal**, **low level**, **expressive**
         and **pragmatic** library in a widely used programming language. pyconll
         creates a thin API on top of raw CoNLL annotations that is simple and
@@ -58,38 +56,38 @@
         a smooth development workflow no matter the dataset size (performs about
         25%-35% faster than other comparable packages)
         
         See the following code example to understand the basics of the API.
         
         .. code:: python
         
-            # This snippet finds sentences where a token marked with part of speech 'AUX' are
-            # governed by a NOUN. For example, in French this is a less common construction
-            # and we may want to validate these examples because we have previously found some
-            # problematic examples of this construction.
-            import pyconll
-        
-            train = pyconll.load_from_file('./ud/train.conllu')
-        
-            review_sentences = []
-        
-            # Conll objects are iterable over their sentences, and sentences are iterable
-            # over their tokens. Sentences also de/serialize comment information.
-            for sentence in train:
-                for token in sentence:
-        
-                    # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
-                    # can be indexed by a token's id. We must check that the token is not the
-                    # root token, whose id, '0', cannot be looked up.
-                    if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
-                        review_sentences.append(sentence)
-        
-            print('Review the following sentences:')
-            for sent in review_sentences:
-                print(sent.id)
+           # This snippet finds sentences where a token marked with part of speech 'AUX' are
+           # governed by a NOUN. For example, in French this is a less common construction
+           # and we may want to validate these examples because we have previously found some
+           # problematic examples of this construction.
+           import pyconll
+        
+           train = pyconll.load_from_file('./ud/train.conllu')
+        
+           review_sentences = []
+        
+           # Conll objects are iterable over their sentences, and sentences are iterable
+           # over their tokens. Sentences also de/serialize comment information.
+           for sentence in train:
+              for token in sentence:
+        
+              # Tokens have attributes such as upos, head, id, deprel, etc, and sentences
+              # can be indexed by a token's id. We must check that the token is not the
+              # root token, whose id, '0', cannot be looked up.
+              if token.upos == 'AUX' and (token.head != '0' and sentence[token.head].upos == 'NOUN'):
+                 review_sentences.append(sentence)
+            
+           print('Review the following sentences:')
+           for sent in review_sentences:
+              print(sent.id)
         
         A full definition of the API can be found in the
         `documentation <https://pyconll.readthedocs.io/>`__ or use the `quick
         start <https://pyconll.readthedocs.io/en/stable/starting.html>`__ guide
         for a focused introduction.
         
         Uses and Limitations
@@ -185,8 +183,8 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
```

### Comparing `pyconll-3.1.0.dev3/setup.py` & `pyconll-3.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     description = 'Read and manipulate CoNLL files',
     long_description = make_relative('README.rst').read_text(),
     author = 'Matias Grioni',
     author_email = 'matgrioni@gmail.com',
     url = 'https://github.com/pyconll/pyconll',
     license = 'MIT',
     keywords = ['nlp', 'conllu', 'conll', 'universal dependencies'],
-    python_requires = '~=3.6',
+    python_requires = '~=3.8',
+    package_data = { 'pyconll': ['py.typed'] },
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
```

