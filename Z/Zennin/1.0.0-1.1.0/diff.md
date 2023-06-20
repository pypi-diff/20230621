# Comparing `tmp/Zennin-1.0.0.tar.gz` & `tmp/Zennin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Zennin-1.0.0.tar", last modified: Fri Jun 16 00:57:10 2023, max compression
+gzip compressed data, was "Zennin-1.1.0.tar", last modified: Tue Jun 20 23:05:33 2023, max compression
```

## Comparing `Zennin-1.0.0.tar` & `Zennin-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-16 00:57:10.779177 Zennin-1.0.0/
--rw-rw-rw-   0 mag       (1000) users      (984)    35149 2021-12-26 20:20:37.000000 Zennin-1.0.0/LICENSE
--rw-r--r--   0 mag       (1000) users      (984)     3487 2023-06-16 00:57:10.779177 Zennin-1.0.0/PKG-INFO
--rw-r--r--   0 mag       (1000) users      (984)     2903 2023-06-16 00:54:19.000000 Zennin-1.0.0/README.md
-drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-16 00:57:10.779177 Zennin-1.0.0/Zennin.egg-info/
--rw-r--r--   0 mag       (1000) users      (984)     3487 2023-06-16 00:57:10.000000 Zennin-1.0.0/Zennin.egg-info/PKG-INFO
--rw-r--r--   0 mag       (1000) users      (984)      248 2023-06-16 00:57:10.000000 Zennin-1.0.0/Zennin.egg-info/SOURCES.txt
--rw-r--r--   0 mag       (1000) users      (984)        1 2023-06-16 00:57:10.000000 Zennin-1.0.0/Zennin.egg-info/dependency_links.txt
--rw-r--r--   0 mag       (1000) users      (984)       39 2023-06-16 00:57:10.000000 Zennin-1.0.0/Zennin.egg-info/entry_points.txt
--rw-r--r--   0 mag       (1000) users      (984)        7 2023-06-16 00:57:10.000000 Zennin-1.0.0/Zennin.egg-info/top_level.txt
--rw-r--r--   0 mag       (1000) users      (984)      687 2023-06-16 00:51:26.000000 Zennin-1.0.0/pyproject.toml
--rw-r--r--   0 mag       (1000) users      (984)       38 2023-06-16 00:57:10.779177 Zennin-1.0.0/setup.cfg
-drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-16 00:57:10.779177 Zennin-1.0.0/tests/
--rwxr-xr-x   0 mag       (1000) users      (984)     5070 2023-06-16 00:37:52.000000 Zennin-1.0.0/tests/test_quotebook.py
-drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-16 00:57:10.779177 Zennin-1.0.0/zennin/
--rwxr-xr-x   0 mag       (1000) users      (984)     2122 2023-06-16 00:37:52.000000 Zennin-1.0.0/zennin/__init__.py
--rwxr-xr-x   0 mag       (1000) users      (984)     3309 2023-06-16 00:37:52.000000 Zennin-1.0.0/zennin/quotebook.py
+drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-20 23:05:33.722753 Zennin-1.1.0/
+-rw-rw-rw-   0 mag       (1000) users      (984)    35149 2021-12-26 20:20:37.000000 Zennin-1.1.0/LICENSE
+-rw-r--r--   0 mag       (1000) users      (984)     3579 2023-06-20 23:05:33.722753 Zennin-1.1.0/PKG-INFO
+-rw-r--r--   0 mag       (1000) users      (984)     2967 2023-06-20 19:59:41.000000 Zennin-1.1.0/README.md
+drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-20 23:05:33.722753 Zennin-1.1.0/Zennin.egg-info/
+-rw-r--r--   0 mag       (1000) users      (984)     3579 2023-06-20 23:05:33.000000 Zennin-1.1.0/Zennin.egg-info/PKG-INFO
+-rw-r--r--   0 mag       (1000) users      (984)      291 2023-06-20 23:05:33.000000 Zennin-1.1.0/Zennin.egg-info/SOURCES.txt
+-rw-r--r--   0 mag       (1000) users      (984)        1 2023-06-20 23:05:33.000000 Zennin-1.1.0/Zennin.egg-info/dependency_links.txt
+-rw-r--r--   0 mag       (1000) users      (984)       39 2023-06-20 23:05:33.000000 Zennin-1.1.0/Zennin.egg-info/entry_points.txt
+-rw-r--r--   0 mag       (1000) users      (984)        7 2023-06-20 23:05:33.000000 Zennin-1.1.0/Zennin.egg-info/top_level.txt
+drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-20 23:05:33.722753 Zennin-1.1.0/doc/
+-rw-r--r--   0 mag       (1000) users      (984)     2531 2023-06-20 19:59:41.000000 Zennin-1.1.0/doc/zennin.1
+-rw-r--r--   0 mag       (1000) users      (984)      715 2023-06-20 22:54:17.000000 Zennin-1.1.0/pyproject.toml
+-rw-r--r--   0 mag       (1000) users      (984)       38 2023-06-20 23:05:33.722753 Zennin-1.1.0/setup.cfg
+-rw-r--r--   0 mag       (1000) users      (984)      222 2023-06-20 22:57:19.000000 Zennin-1.1.0/setup.py
+drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-20 23:05:33.722753 Zennin-1.1.0/tests/
+-rwxr-xr-x   0 mag       (1000) users      (984)     5102 2023-06-20 22:57:10.000000 Zennin-1.1.0/tests/test_quotebook.py
+drwxr-xr-x   0 mag       (1000) users      (984)        0 2023-06-20 23:05:33.722753 Zennin-1.1.0/zennin/
+-rwxr-xr-x   0 mag       (1000) users      (984)     2822 2023-06-20 19:59:41.000000 Zennin-1.1.0/zennin/__init__.py
+-rwxr-xr-x   0 mag       (1000) users      (984)     3309 2023-06-16 00:37:52.000000 Zennin-1.1.0/zennin/quotebook.py
+-rw-r--r--   0 mag       (1000) users      (984)     2675 2023-06-20 19:59:41.000000 Zennin-1.1.0/zennin/quotebook.txt
```

### Comparing `Zennin-1.0.0/LICENSE` & `Zennin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Zennin-1.0.0/PKG-INFO` & `Zennin-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Zennin
-Version: 1.0.0
-Summary: Knowledge
+Version: 1.1.0
+Summary: Print custom quotes on your terminal.
 Author-email: Marcelo Galván <marcelo_galvan@protonmail.com>
 Project-URL: Homepage, https://github.com/Erymer/zennin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
@@ -30,15 +30,16 @@
 
 
 # Quote Book
 
 The collection of quotes used by zennin is stored in a file known as the
 `Quote Book`. By default, the program looks for the `quote book` at
 `$HOME/.config/zennin/quotebook.txt`. If this file doesn't exist, zennin
-falls back to using a default quote book located at `/etc/quotebook.txt`.
+falls back to using a default quote book located at
+`/usr/share/doc/zennin/quotebook.txt`.
 
 Feel free to use the default `quote book` as a reference to create your own
 personalized collection. The syntax of the `quote book` is similar to
 Python docstrings, with three single quotes (''') used as delimiters for the
 beginning and the end of each quote. 
 
 ```
@@ -100,14 +101,21 @@
 ``` bash
 git clone https://github.com/Erymer/zennin
 cd zennin
 sudo make install
 ```
 
 
+## From pip
+
+``` bash
+pip install zennin
+```
+
+
 # Using Zennin
 
 To use it as intended just include one of the following lines in the
 configuration file of your shell (bashrc, zshrc, etc).
 
 ``` bash
 zennin # Text in the center of the terminal
```

### Comparing `Zennin-1.0.0/README.md` & `Zennin-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 # Quote Book
 
 The collection of quotes used by zennin is stored in a file known as the
 `Quote Book`. By default, the program looks for the `quote book` at
 `$HOME/.config/zennin/quotebook.txt`. If this file doesn't exist, zennin
-falls back to using a default quote book located at `/etc/quotebook.txt`.
+falls back to using a default quote book located at
+`/usr/share/doc/zennin/quotebook.txt`.
 
 Feel free to use the default `quote book` as a reference to create your own
 personalized collection. The syntax of the `quote book` is similar to
 Python docstrings, with three single quotes (''') used as delimiters for the
 beginning and the end of each quote. 
 
 ```
@@ -84,14 +85,21 @@
 ``` bash
 git clone https://github.com/Erymer/zennin
 cd zennin
 sudo make install
 ```
 
 
+## From pip
+
+``` bash
+pip install zennin
+```
+
+
 # Using Zennin
 
 To use it as intended just include one of the following lines in the
 configuration file of your shell (bashrc, zshrc, etc).
 
 ``` bash
 zennin # Text in the center of the terminal
```

### Comparing `Zennin-1.0.0/Zennin.egg-info/PKG-INFO` & `Zennin-1.1.0/Zennin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Zennin
-Version: 1.0.0
-Summary: Knowledge
+Version: 1.1.0
+Summary: Print custom quotes on your terminal.
 Author-email: Marcelo Galván <marcelo_galvan@protonmail.com>
 Project-URL: Homepage, https://github.com/Erymer/zennin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
@@ -30,15 +30,16 @@
 
 
 # Quote Book
 
 The collection of quotes used by zennin is stored in a file known as the
 `Quote Book`. By default, the program looks for the `quote book` at
 `$HOME/.config/zennin/quotebook.txt`. If this file doesn't exist, zennin
-falls back to using a default quote book located at `/etc/quotebook.txt`.
+falls back to using a default quote book located at
+`/usr/share/doc/zennin/quotebook.txt`.
 
 Feel free to use the default `quote book` as a reference to create your own
 personalized collection. The syntax of the `quote book` is similar to
 Python docstrings, with three single quotes (''') used as delimiters for the
 beginning and the end of each quote. 
 
 ```
@@ -100,14 +101,21 @@
 ``` bash
 git clone https://github.com/Erymer/zennin
 cd zennin
 sudo make install
 ```
 
 
+## From pip
+
+``` bash
+pip install zennin
+```
+
+
 # Using Zennin
 
 To use it as intended just include one of the following lines in the
 configuration file of your shell (bashrc, zshrc, etc).
 
 ``` bash
 zennin # Text in the center of the terminal
```

### Comparing `Zennin-1.0.0/tests/test_quotebook.py` & `Zennin-1.1.0/tests/test_quotebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
 from zennin import QuoteBook
+import zennin
 import tempfile
 import os
 import random
+import subprocess
 
 
 QUOTES = [
 '''Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
 incididunt ut labore et dolore magna aliqua. Tincidunt ornare massa eget
 egestas purus. Posuere sollicitudin aliquam ultrices sagittis orci a
 scelerisque purus semper. Sit amet tellus cras adipiscing enim eu turpis
@@ -53,22 +55,23 @@
 NUM_OF_QUOTES_IN_TEST_FILE = 100
 
 random_quotes = random.choices(QUOTES, k=NUM_OF_QUOTES_IN_TEST_FILE)
 
 DEFAULT_SEPARATOR = "'''"
 RANDOM_SEPARATOR = "***"
 
-DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT = ""
 
+DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT = ""
 for quote in random_quotes:
     DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT += f"{DEFAULT_SEPARATOR}\n"
     DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT += quote
     DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT += f"\n{DEFAULT_SEPARATOR}\n"
     DEFAULT_SEPARATOR_QUOTE_BOOK_CONTENT += f"\n\n"
 
+
 RANDOM_SEPARATOR_QUOTE_BOOK_CONTENT = ""
 for quote in random_quotes:
     RANDOM_SEPARATOR_QUOTE_BOOK_CONTENT += f"{RANDOM_SEPARATOR}\n"
     RANDOM_SEPARATOR_QUOTE_BOOK_CONTENT += quote
     RANDOM_SEPARATOR_QUOTE_BOOK_CONTENT += f"\n{RANDOM_SEPARATOR}\n"
     RANDOM_SEPARATOR_QUOTE_BOOK_CONTENT += f"\n\n"
 
@@ -113,10 +116,9 @@
         print('NEXT QUOTES MUST BE ON THE RIGHT')
         self.default_separator_book.print_quote(1, "right")
         self.random_separator_book.print_quote(1, "right")
         print('NEXT QUOTES MUST BE ON THE CENTER')
         self.default_separator_book.print_quote(1, "center")
         self.random_separator_book.print_quote(1, "center")
 
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Zennin-1.0.0/zennin/quotebook.py` & `Zennin-1.1.0/zennin/quotebook.py`

 * *Files identical despite different names*

