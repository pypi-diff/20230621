# Comparing `tmp/consoleiotools-4.2.1.tar.gz` & `tmp/consoleiotools-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleiotools-4.2.1.tar", last modified: Sun Feb 12 08:56:11 2023, max compression
+gzip compressed data, was "consoleiotools-4.2.2.tar", last modified: Wed Jun 21 03:35:34 2023, max compression
```

## Comparing `consoleiotools-4.2.1.tar` & `consoleiotools-4.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-02-12 08:56:11.909505 consoleiotools-4.2.1/
--rw-r--r--   0 kyan001    (501) staff       (20)     1071 2017-01-21 01:51:03.000000 consoleiotools-4.2.1/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)     6771 2023-02-12 08:56:11.907609 consoleiotools-4.2.1/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)     4690 2023-02-11 07:08:58.000000 consoleiotools-4.2.1/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-02-12 08:56:11.882182 consoleiotools-4.2.1/consoleiotools/
--rw-r--r--   0 kyan001    (501) staff       (20)     9646 2023-02-12 08:55:00.000000 consoleiotools-4.2.1/consoleiotools/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2462 2022-12-25 09:57:18.000000 consoleiotools-4.2.1/consoleiotools/__main__.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-02-12 08:56:11.904809 consoleiotools-4.2.1/consoleiotools.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)     6771 2023-02-12 08:56:11.000000 consoleiotools-4.2.1/consoleiotools.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      304 2023-02-12 08:56:11.000000 consoleiotools-4.2.1/consoleiotools.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2023-02-12 08:56:11.000000 consoleiotools-4.2.1/consoleiotools.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       36 2023-02-12 08:56:11.000000 consoleiotools-4.2.1/consoleiotools.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       20 2023-02-12 08:56:11.000000 consoleiotools-4.2.1/consoleiotools.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1220 2022-12-25 09:57:18.000000 consoleiotools-4.2.1/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2023-02-12 08:56:11.909657 consoleiotools-4.2.1/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-02-12 08:56:11.906294 consoleiotools-4.2.1/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)    10806 2023-02-11 07:00:37.000000 consoleiotools-4.2.1/tests/test_consoleiotools.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:35:34.973026 consoleiotools-4.2.2/
+-rw-rw-rw-   0        0        0     1092 2021-03-17 11:22:04.000000 consoleiotools-4.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7041 2023-06-21 03:35:34.972032 consoleiotools-4.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4918 2023-02-11 09:48:53.000000 consoleiotools-4.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 03:35:34.959619 consoleiotools-4.2.2/consoleiotools/
+-rw-rw-rw-   0        0        0     9978 2023-06-21 03:15:07.000000 consoleiotools-4.2.2/consoleiotools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-06-21 03:15:10.000000 consoleiotools-4.2.2/consoleiotools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:35:34.970020 consoleiotools-4.2.2/consoleiotools.egg-info/
+-rw-rw-rw-   0        0        0     7041 2023-06-21 03:35:34.000000 consoleiotools-4.2.2/consoleiotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-21 03:35:34.000000 consoleiotools-4.2.2/consoleiotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:35:34.000000 consoleiotools-4.2.2/consoleiotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-21 03:35:34.000000 consoleiotools-4.2.2/consoleiotools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 03:35:34.000000 consoleiotools-4.2.2/consoleiotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1262 2022-12-15 10:59:59.000000 consoleiotools-4.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:35:34.973026 consoleiotools-4.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 03:35:34.971035 consoleiotools-4.2.2/tests/
+-rw-rw-rw-   0        0        0    11083 2023-02-11 09:48:53.000000 consoleiotools-4.2.2/tests/test_consoleiotools.py
```

### Comparing `consoleiotools-4.2.1/LICENSE` & `consoleiotools-4.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2016 Kyan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2016 Kyan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `consoleiotools-4.2.1/PKG-INFO` & `consoleiotools-4.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,270 +1,270 @@
-Metadata-Version: 2.1
-Name: consoleiotools
-Version: 4.2.1
-Summary: Console tools for inputs and outputs in Python
-Author-email: Kyan <kai@kyan001.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2016 Kyan
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/kyan001/PyConsoleIOTools
-Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleIOTools/issues
-Project-URL: Source Code, https://github.com/kyan001/PyConsoleIOTools
-Keywords: python,console,input,output,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# PyConsoleIOTools
-![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
-![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
-
-## Installation
-
-```sh
-pip install consoleiotools  # install
-pip install --upgrade consoleiotools  # update
-python -m consoleiotools  # examples
-```
-
-## Get Started
-
-```python
-import consoleiotools as cit
-print(cit.__version__)
-```
-
-## Prints on Screen
-
-```python
->>> cit.start()
-# blank line
-
->>> cit.title('Session Name')
-+--------------+
-| SESSION NAME |
-+--------------+
-
->>> cit.echo('Hello World')
-| Hello World
-
->>> cit.echo('Hello World', pre='say', bar='!')
-! (Say) Hello World
-
->>> cit.ask('Hello World')
-| (?) Hello World
-
->>> cit.info('Hello World')
-| (Info) Hello World
-
->>> cit.warn('Hello World')
-| (Warning) Hello World
-
->>> cit.err('Hello World')
-| (Error) Hello World
-
->>> cit.mute('Hello World')
-| Hello World  # muted by dim
-
->>> cit.print(var)  # print variable
-...
-
->>> cit.markdown("# Header")  # print markdown
-+--------------+
-|    Header    |
-+--------------+
-
->>> cit.rule()  # print horizontal rule
-----------------------------------------
-
->>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
----------------- Title ----------------
-
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
-+---------- Panel Title ----------+
-| Panel                           |  # full width
-+-------- Panel Subtitle ---------+
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
-+- Panel Title -+  # blue
-| Panel         |
-+- Panel Subtit-+
-
->>> cit.end()
-`
-
->>> cit.br()
-# blank line
-
->>> cit.br(2)
-# blank line
-# blank line
-
->>> for var in cit.track(iterables, "Progress"): pass
-| : Progress ---------------------===================  52% 0:00:52 - 52/100
-
->>> cit.__ascii__ = True  # use ascii chars only.
-```
-
-## Get User Input
-
-```python
->>> cit.get_input()  # Get user input from stdin
-> Hello World
-'Hello World'
-
->>> cit.get_input("Question?")  # With a question
-| (?) Question?
-> Yes
-'Yes'
-
->>> cit.get_input(prompt="Answer:")  # With a customized prompt.
-Answer: Apple
-'Apple'
-
->>> cit.get_input("Continue?", default="yes")  # With a default answer.
-| (?) Continue?
-> (yes)  # Entered nothing
-'yes'
-
->>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
->       # Whitespaces
-'    '
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
-|  1) Apple
-|  2) Google
-> 2
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
-|  1) Apple
-|  2) Google
-> Google
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) Apple
-|  2) Google
-|  0) ** EXIT **
-> 0
-None
-
->>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
-|  1) [ ] Apple
-|  2) [ ] Google
-> 1  # Enter number to check or uncheck selections
-|  1) [+] Apple
-|  2) [ ] Google
-|  0) ** DONE **
-> Google  # Enter string is ok too.
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0  # Enter 0 when done.
-['Apple', 'Google']  # return [] is no selections.
-
->>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
-|  a) ** ALL **
-|  1) [ ] Apple
-|  2) [ ] Google
-> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
-|  a) ** ALL **
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0
-['Apple', 'Google']
-
->>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) [ ] Apple
-|  2) [ ] Google
-|  0) ** EXIT **
-> 0
-[]  # Empty list returned.
-```
-
-## File IO
-
-```python
->>> cit.read_file('/path/to/file')
-'File contents'
-
->>> cit.read_file('/path/to/file', with_encoding=True)
-('File contents', 'utf-8')
-
->>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
-8  # writed bytes
-
->>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
-8  # writed bytes
-```
-
-## Controls
-
-```python
->>> cit.pause()
-| Press [Enter] to Continue...
-
->>> cit.bye()
-# exit
-
->>> cit.bye(0)
-# exit with code 0
-
->>> cit.bye('Seeya')
-Seeya
-# exit
-```
-
-## Decorators
-
-```python
-@cit.as_session('Hello')
-def my_func():
-    cit.echo('World')
-
->>> my_func()
-+---------+
-| HELLO() |
-+---------+
-| World
-`
-
-@cit.as_session
-def underscore_orCamel():
-    pass
-
->>> underscore_orCamel()
-+-----------------------+
-| UNDERSCORE OR CAMEL() |
-+-----------------------+
-`
-```
+Metadata-Version: 2.1
+Name: consoleiotools
+Version: 4.2.2
+Summary: Console tools for inputs and outputs in Python
+Author-email: Kyan <kai@kyan001.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016 Kyan
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/kyan001/PyConsoleIOTools
+Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleIOTools/issues
+Project-URL: Source Code, https://github.com/kyan001/PyConsoleIOTools
+Keywords: python,console,input,output,tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# PyConsoleIOTools
+![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
+![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
+
+## Installation
+
+```sh
+pip install consoleiotools  # install
+pip install --upgrade consoleiotools  # update
+python -m consoleiotools  # examples
+```
+
+## Get Started
+
+```python
+import consoleiotools as cit
+print(cit.__version__)
+```
+
+## Prints on Screen
+
+```python
+>>> cit.start()
+# blank line
+
+>>> cit.title('Session Name')
++--------------+
+| SESSION NAME |
++--------------+
+
+>>> cit.echo('Hello World')
+| Hello World
+
+>>> cit.echo('Hello World', pre='say', bar='!')
+! (Say) Hello World
+
+>>> cit.ask('Hello World')
+| (?) Hello World
+
+>>> cit.info('Hello World')
+| (Info) Hello World
+
+>>> cit.warn('Hello World')
+| (Warning) Hello World
+
+>>> cit.err('Hello World')
+| (Error) Hello World
+
+>>> cit.mute('Hello World')
+| Hello World  # muted by dim
+
+>>> cit.print(var)  # print variable
+...
+
+>>> cit.markdown("# Header")  # print markdown
++--------------+
+|    Header    |
++--------------+
+
+>>> cit.rule()  # print horizontal rule
+----------------------------------------
+
+>>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
+---------------- Title ----------------
+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
++---------- Panel Title ----------+
+| Panel                           |  # full width
++-------- Panel Subtitle ---------+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
++- Panel Title -+  # blue
+| Panel         |
++- Panel Subtit-+
+
+>>> cit.end()
+`
+
+>>> cit.br()
+# blank line
+
+>>> cit.br(2)
+# blank line
+# blank line
+
+>>> for var in cit.track(iterables, "Progress"): pass
+| : Progress ---------------------===================  52% 0:00:52 - 52/100
+
+>>> cit.__ascii__ = True  # use ascii chars only.
+```
+
+## Get User Input
+
+```python
+>>> cit.get_input()  # Get user input from stdin
+> Hello World
+'Hello World'
+
+>>> cit.get_input("Question?")  # With a question
+| (?) Question?
+> Yes
+'Yes'
+
+>>> cit.get_input(prompt="Answer:")  # With a customized prompt.
+Answer: Apple
+'Apple'
+
+>>> cit.get_input("Continue?", default="yes")  # With a default answer.
+| (?) Continue?
+> (yes)  # Entered nothing
+'yes'
+
+>>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
+>       # Whitespaces
+'    '
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
+|  1) Apple
+|  2) Google
+> 2
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
+|  1) Apple
+|  2) Google
+> Google
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) Apple
+|  2) Google
+|  0) ** EXIT **
+> 0
+None
+
+>>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
+|  1) [ ] Apple
+|  2) [ ] Google
+> 1  # Enter number to check or uncheck selections
+|  1) [+] Apple
+|  2) [ ] Google
+|  0) ** DONE **
+> Google  # Enter string is ok too.
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0  # Enter 0 when done.
+['Apple', 'Google']  # return [] is no selections.
+
+>>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
+|  a) ** ALL **
+|  1) [ ] Apple
+|  2) [ ] Google
+> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
+|  a) ** ALL **
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0
+['Apple', 'Google']
+
+>>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) [ ] Apple
+|  2) [ ] Google
+|  0) ** EXIT **
+> 0
+[]  # Empty list returned.
+```
+
+## File IO
+
+```python
+>>> cit.read_file('/path/to/file')
+'File contents'
+
+>>> cit.read_file('/path/to/file', with_encoding=True)
+('File contents', 'utf-8')
+
+>>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
+8  # writed bytes
+
+>>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
+8  # writed bytes
+```
+
+## Controls
+
+```python
+>>> cit.pause()
+| Press [Enter] to Continue...
+
+>>> cit.bye()
+# exit
+
+>>> cit.bye(0)
+# exit with code 0
+
+>>> cit.bye('Seeya')
+Seeya
+# exit
+```
+
+## Decorators
+
+```python
+@cit.as_session('Hello')
+def my_func():
+    cit.echo('World')
+
+>>> my_func()
++---------+
+| HELLO() |
++---------+
+| World
+`
+
+@cit.as_session
+def underscore_orCamel():
+    pass
+
+>>> underscore_orCamel()
++-----------------------+
+| UNDERSCORE OR CAMEL() |
++-----------------------+
+`
+```
```

### Comparing `consoleiotools-4.2.1/README.md` & `consoleiotools-4.2.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-# PyConsoleIOTools
-![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
-![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
-
-## Installation
-
-```sh
-pip install consoleiotools  # install
-pip install --upgrade consoleiotools  # update
-python -m consoleiotools  # examples
-```
-
-## Get Started
-
-```python
-import consoleiotools as cit
-print(cit.__version__)
-```
-
-## Prints on Screen
-
-```python
->>> cit.start()
-# blank line
-
->>> cit.title('Session Name')
-+--------------+
-| SESSION NAME |
-+--------------+
-
->>> cit.echo('Hello World')
-| Hello World
-
->>> cit.echo('Hello World', pre='say', bar='!')
-! (Say) Hello World
-
->>> cit.ask('Hello World')
-| (?) Hello World
-
->>> cit.info('Hello World')
-| (Info) Hello World
-
->>> cit.warn('Hello World')
-| (Warning) Hello World
-
->>> cit.err('Hello World')
-| (Error) Hello World
-
->>> cit.mute('Hello World')
-| Hello World  # muted by dim
-
->>> cit.print(var)  # print variable
-...
-
->>> cit.markdown("# Header")  # print markdown
-+--------------+
-|    Header    |
-+--------------+
-
->>> cit.rule()  # print horizontal rule
-----------------------------------------
-
->>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
----------------- Title ----------------
-
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
-+---------- Panel Title ----------+
-| Panel                           |  # full width
-+-------- Panel Subtitle ---------+
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
-+- Panel Title -+  # blue
-| Panel         |
-+- Panel Subtit-+
-
->>> cit.end()
-`
-
->>> cit.br()
-# blank line
-
->>> cit.br(2)
-# blank line
-# blank line
-
->>> for var in cit.track(iterables, "Progress"): pass
-| : Progress ---------------------===================  52% 0:00:52 - 52/100
-
->>> cit.__ascii__ = True  # use ascii chars only.
-```
-
-## Get User Input
-
-```python
->>> cit.get_input()  # Get user input from stdin
-> Hello World
-'Hello World'
-
->>> cit.get_input("Question?")  # With a question
-| (?) Question?
-> Yes
-'Yes'
-
->>> cit.get_input(prompt="Answer:")  # With a customized prompt.
-Answer: Apple
-'Apple'
-
->>> cit.get_input("Continue?", default="yes")  # With a default answer.
-| (?) Continue?
-> (yes)  # Entered nothing
-'yes'
-
->>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
->       # Whitespaces
-'    '
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
-|  1) Apple
-|  2) Google
-> 2
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
-|  1) Apple
-|  2) Google
-> Google
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) Apple
-|  2) Google
-|  0) ** EXIT **
-> 0
-None
-
->>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
-|  1) [ ] Apple
-|  2) [ ] Google
-> 1  # Enter number to check or uncheck selections
-|  1) [+] Apple
-|  2) [ ] Google
-|  0) ** DONE **
-> Google  # Enter string is ok too.
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0  # Enter 0 when done.
-['Apple', 'Google']  # return [] is no selections.
-
->>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
-|  a) ** ALL **
-|  1) [ ] Apple
-|  2) [ ] Google
-> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
-|  a) ** ALL **
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0
-['Apple', 'Google']
-
->>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) [ ] Apple
-|  2) [ ] Google
-|  0) ** EXIT **
-> 0
-[]  # Empty list returned.
-```
-
-## File IO
-
-```python
->>> cit.read_file('/path/to/file')
-'File contents'
-
->>> cit.read_file('/path/to/file', with_encoding=True)
-('File contents', 'utf-8')
-
->>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
-8  # writed bytes
-
->>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
-8  # writed bytes
-```
-
-## Controls
-
-```python
->>> cit.pause()
-| Press [Enter] to Continue...
-
->>> cit.bye()
-# exit
-
->>> cit.bye(0)
-# exit with code 0
-
->>> cit.bye('Seeya')
-Seeya
-# exit
-```
-
-## Decorators
-
-```python
-@cit.as_session('Hello')
-def my_func():
-    cit.echo('World')
-
->>> my_func()
-+---------+
-| HELLO() |
-+---------+
-| World
-`
-
-@cit.as_session
-def underscore_orCamel():
-    pass
-
->>> underscore_orCamel()
-+-----------------------+
-| UNDERSCORE OR CAMEL() |
-+-----------------------+
-`
-```
+# PyConsoleIOTools
+![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
+![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
+
+## Installation
+
+```sh
+pip install consoleiotools  # install
+pip install --upgrade consoleiotools  # update
+python -m consoleiotools  # examples
+```
+
+## Get Started
+
+```python
+import consoleiotools as cit
+print(cit.__version__)
+```
+
+## Prints on Screen
+
+```python
+>>> cit.start()
+# blank line
+
+>>> cit.title('Session Name')
++--------------+
+| SESSION NAME |
++--------------+
+
+>>> cit.echo('Hello World')
+| Hello World
+
+>>> cit.echo('Hello World', pre='say', bar='!')
+! (Say) Hello World
+
+>>> cit.ask('Hello World')
+| (?) Hello World
+
+>>> cit.info('Hello World')
+| (Info) Hello World
+
+>>> cit.warn('Hello World')
+| (Warning) Hello World
+
+>>> cit.err('Hello World')
+| (Error) Hello World
+
+>>> cit.mute('Hello World')
+| Hello World  # muted by dim
+
+>>> cit.print(var)  # print variable
+...
+
+>>> cit.markdown("# Header")  # print markdown
++--------------+
+|    Header    |
++--------------+
+
+>>> cit.rule()  # print horizontal rule
+----------------------------------------
+
+>>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
+---------------- Title ----------------
+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
++---------- Panel Title ----------+
+| Panel                           |  # full width
++-------- Panel Subtitle ---------+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
++- Panel Title -+  # blue
+| Panel         |
++- Panel Subtit-+
+
+>>> cit.end()
+`
+
+>>> cit.br()
+# blank line
+
+>>> cit.br(2)
+# blank line
+# blank line
+
+>>> for var in cit.track(iterables, "Progress"): pass
+| : Progress ---------------------===================  52% 0:00:52 - 52/100
+
+>>> cit.__ascii__ = True  # use ascii chars only.
+```
+
+## Get User Input
+
+```python
+>>> cit.get_input()  # Get user input from stdin
+> Hello World
+'Hello World'
+
+>>> cit.get_input("Question?")  # With a question
+| (?) Question?
+> Yes
+'Yes'
+
+>>> cit.get_input(prompt="Answer:")  # With a customized prompt.
+Answer: Apple
+'Apple'
+
+>>> cit.get_input("Continue?", default="yes")  # With a default answer.
+| (?) Continue?
+> (yes)  # Entered nothing
+'yes'
+
+>>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
+>       # Whitespaces
+'    '
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
+|  1) Apple
+|  2) Google
+> 2
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
+|  1) Apple
+|  2) Google
+> Google
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) Apple
+|  2) Google
+|  0) ** EXIT **
+> 0
+None
+
+>>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
+|  1) [ ] Apple
+|  2) [ ] Google
+> 1  # Enter number to check or uncheck selections
+|  1) [+] Apple
+|  2) [ ] Google
+|  0) ** DONE **
+> Google  # Enter string is ok too.
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0  # Enter 0 when done.
+['Apple', 'Google']  # return [] is no selections.
+
+>>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
+|  a) ** ALL **
+|  1) [ ] Apple
+|  2) [ ] Google
+> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
+|  a) ** ALL **
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0
+['Apple', 'Google']
+
+>>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) [ ] Apple
+|  2) [ ] Google
+|  0) ** EXIT **
+> 0
+[]  # Empty list returned.
+```
+
+## File IO
+
+```python
+>>> cit.read_file('/path/to/file')
+'File contents'
+
+>>> cit.read_file('/path/to/file', with_encoding=True)
+('File contents', 'utf-8')
+
+>>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
+8  # writed bytes
+
+>>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
+8  # writed bytes
+```
+
+## Controls
+
+```python
+>>> cit.pause()
+| Press [Enter] to Continue...
+
+>>> cit.bye()
+# exit
+
+>>> cit.bye(0)
+# exit with code 0
+
+>>> cit.bye('Seeya')
+Seeya
+# exit
+```
+
+## Decorators
+
+```python
+@cit.as_session('Hello')
+def my_func():
+    cit.echo('World')
+
+>>> my_func()
++---------+
+| HELLO() |
++---------+
+| World
+`
+
+@cit.as_session
+def underscore_orCamel():
+    pass
+
+>>> underscore_orCamel()
++-----------------------+
+| UNDERSCORE OR CAMEL() |
++-----------------------+
+`
+```
```

### Comparing `consoleiotools-4.2.1/consoleiotools/__init__.py` & `consoleiotools-4.2.2/consoleiotools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,283 +1,286 @@
-from functools import wraps
-
-import rich.console
-import rich.theme
-import rich.panel
-import rich.text
-import rich.progress
-import rich.traceback
-import rich.markdown
-import rich.box
-
-__version__ = "4.2.1"
-__ascii__ = False
-theme = rich.theme.Theme({
-    "echo": "bright_white",
-    "echo-bar": "",
-    "echo-pre": "dim bright_white",
-    "info": "",
-    "info-bar": "",
-    "info-pre": "dim",
-    "warn": "red",
-    "warn-bar": "red",
-    "warn-pre": "dim red",
-    "err": "bright_white on red",
-    "err-bar": "bright_red",
-    "err-pre": "dim bright_red",
-    "ask": "yellow",
-    "ask-bar": "yellow",
-    "ask-pre": "dim yellow",
-    "muted": "dim bright_white",
-    "muted-bar": "dim white",
-    "muted-pre": "dim white",
-    "title": "bright_magenta",
-    "pause": "bright_yellow",
-    "choice-i": "yellow",
-    "choice-cmd": "yellow underline",
-})
-console = rich.console.Console(theme=theme)  # main output printer
-rich.traceback.install()
-
-
-def debug(show_locals: bool = True) -> None:
-    rich.traceback.install(show_locals=show_locals)
-
-
-def as_session(name_or_func):  # decorator
-    """print start/title/end info before and after the function call
-
-    Args:
-        title: title will show after the start, if has any
-    """
-    if callable(name_or_func):  # no name provided
-        func = name_or_func
-        name = func.__name__
-        name = "".join([(" " + x) if x.isupper() else x for x in name])
-        name = name.replace("_", " ")
-        return as_session(name)(func)  # deco(func) -> deco(name)(func)
-    else:
-        name = name_or_func
-
-    def get_func(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            start()
-            title(name)
-            result = func(*args, **kwargs)
-            end()
-            return result
-        return wrapper
-    return get_func
-
-
-def start():
-    br()
-
-
-def end():
-    console.print("`" if __ascii__ else "╰")
-
-
-def br(count=1):
-    """print 1 to N blank lines"""
-    print("\n" * (count - 1))
-
-
-def echo(*args, pre: str = "", bar: str = "|" if __ascii__ else "│", style: str = "echo", **options):
-    txt = rich.text.Text()
-    if bar:
-        txt.append(f"{bar}", style=f"{style}-bar" if f"{style}-bar" in theme.styles else style)
-        txt.append(" ")
-    if pre:
-        txt.append(f"({pre.capitalize()})", style=f"{style}-pre" if f"{style}-pre" in theme.styles else style)
-        txt.append(" ")
-    contents = rich.text.Text(" ").join(rich.text.Text.from_markup(f"{arg}") for arg in args)
-    contents.stylize(style)
-    txt.append(contents)
-    console.print(txt, **options)
-
-
-def title(*args, **options):
-    """print something like a title"""
-    console.print(rich.panel.Panel((" ".join([f"{arg}" for arg in args])).upper().strip(), highlight=True, expand=False, box=rich.box.ASCII if __ascii__ else rich.box.ROUNDED), **options)
-
-
-def ask(*args, **options):
-    return echo(*args, pre="?", style="ask", **options)
-
-
-def info(*args, **options):
-    return echo(*args, pre="info", style="info", **options)
-
-
-def warn(*args, **options):
-    return echo(*args, pre="warning", style="warn", **options)
-
-
-def err(*args, **options):
-    return echo(*args, pre="error", style="err", **options)
-
-
-def mute(*args, **options):
-    return echo(*args, style="muted", **options)
-
-
-def print(*args, **options):
-    console.print(*args, **options)
-
-
-def markdown(*args, **options):
-    console.print(rich.markdown.Markdown(" ".join([f"{arg}" for arg in args])))
-
-
-def rule(title: str, *args, **options):
-    console.rule(title, *args, characters="-" if __ascii__ else "─", **options)
-
-
-def panel(txt, title="", subtitle="", expand=True, highlight=True, style="", **options):
-    return console.print(
-        rich.panel.Panel(
-            txt,
-            title=title,
-            subtitle=subtitle,
-            highlight=highlight,
-            expand=expand,
-            style=style,
-            border_style=f"{style}-pre" if f"{style}-pre" in theme.styles else "",
-            box=rich.box.ASCII if __ascii__ else rich.box.ROUNDED,
-            **options
-        )
-    )
-
-
-def pause(msg="Press [Enter] to Continue..."):
-    """press to continue"""
-    with console.status(f"[pause]{rich.markup.escape(msg)}", spinner="point", spinner_style="pause"):
-        return input()
-
-
-def bye(msg=""):
-    """print msg and exit"""
-    exit(msg)
-
-
-def get_input(question: str = "", prompt: str = "> ", default: str = "", strip: bool = True) -> str:
-    """Get user input in stdin.
-
-    Args:
-        question: str. The question asked before get the answer.
-        prompt: str. The prompt shows in the same line with the input field. Always ending with a space.
-        default: str. If the answer is empty, default value returns.
-        strip: bool. Remove leading and trailing whitespaces from user input or not. Default is True.
-    """
-    if default:
-        prompt += f"[dim]({default})[/]"
-    if question:
-        ask(question)
-    if prompt:
-        console.print(prompt.strip(), end=" ")
-    answer = input()
-    if strip:
-        answer = answer.strip()
-    return answer or default
-
-
-def get_choice(choices, exitable: bool = False) -> str:
-    """Get user choice from a given list
-
-    Args:
-        choices: list. The list that user can choose from.
-        exitable: bool. Does `exit` is an option for user to select.
-    """
-    EXIT_WORD = "exit" if "0" in choices else "0"
-    DECO_WORD = "[dim]{}[/]".format("--" if __ascii__ else "──")
-    BAR_WORD = "|" if __ascii__ else "│"
-    fill = max(len(EXIT_WORD), 2)
-    for index, item in enumerate(choices, start=1):
-        console.print(f"{BAR_WORD} [choice-i]{index:>{fill}}[/][dim])[/] [white]{item}[/]")
-    if exitable:
-        console.print(f"{BAR_WORD} [choice-i]{EXIT_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]EXIT[/] {DECO_WORD}")
-    user_choice = get_input().strip()
-    if exitable and user_choice == EXIT_WORD:
-        return None
-    if user_choice in choices:
-        return user_choice
-    if user_choice.isdigit():
-        index = int(user_choice) - 1
-        if 0 <= index < len(choices):
-            return choices[index]
-    err("Please enter a valid choice.")
-    return get_choice(choices)
-
-
-def get_choices(choices, allable: bool = False, exitable: bool = False) -> list:
-    def toggle_listitem(itm, lst: list):
-        if itm in lst:
-            lst.remove(itm)
-        else:
-            lst.append(itm)
-        return lst
-
-    EXIT_WORD = "exit" if "0" in choices else "0"
-    DONE_WORD = "done" if "0" in choices else "0"
-    ALL_WORD = "all" if "a" in choices else "a"
-    DECO_WORD = "[dim]{}[/]".format("--" if __ascii__ else "──")
-    BAR_WORD = "|" if __ascii__ else "│"
-    BRACKET_WORD = "[cyan]" + rich.console.escape("[") + "{}][/]"
-    fill = max(len(EXIT_WORD), len(DONE_WORD), len(ALL_WORD), 2)
-    user_choices = []
-    while True:
-        if allable:
-            console.print(f"{BAR_WORD} [choice-i]{ALL_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]ALL[/] {DECO_WORD}")
-        for index, item in enumerate(choices, start=1):
-
-            mark = BRACKET_WORD.format(f"[bright_green]{'+' if __ascii__ else '✓'}[/]") if item in user_choices else BRACKET_WORD.format(" ")  # item is selected or not
-            console.print(f"{BAR_WORD} [choice-i]{index:>{fill}}[/][dim])[/] {mark} [white]{item}")
-        if user_choices:  # user selections > 0
-            console.print(f"{BAR_WORD} [choice-i]{DONE_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]DONE[/] {DECO_WORD}")
-        elif exitable:  # no user selection, but exitable is on.
-            console.print(f"{BAR_WORD} [choice-i]{EXIT_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]EXIT[/] {DECO_WORD}")
-        user_choice = get_input().strip()
-        if (user_choice == DONE_WORD or user_choice == EXIT_WORD):
-            if exitable or len(user_choices) > 0:  # keep looping when not exitable and no user choices.
-                return user_choices
-        if allable and user_choice == ALL_WORD:
-            if len(user_choices) == len(choices):
-                user_choices = []
-            else:
-                user_choices = choices.copy()
-        elif user_choice in choices:
-            user_choices = toggle_listitem(user_choice, user_choices)
-        elif user_choice.isdigit() and 0 < int(user_choice) <= len(choices):
-            index = int(user_choice) - 1
-            user_choices = toggle_listitem(choices[index], user_choices)
-        else:
-            err("Please enter a valid choice.")
-
-
-def track(iterable, desc="", unit="", *args, **options):
-    with rich.progress.Progress("|" if __ascii__ else "│", rich.progress.SpinnerColumn(), *rich.progress.Progress.get_default_columns(), "·", rich.progress.MofNCompleteColumn(), unit, *args, **options) as progress:
-        task = progress.add_task(desc, total=None if not iterable or not len(iterable) else len(iterable))
-        while not progress.finished:
-            for item in iterable:
-                yield item
-                progress.update(task, advance=1)
-
-
-def read_file(path: str, with_encoding: bool = False, **kwargs):
-    for enc in ("utf-8", "gbk", "cp1252", "windows-1252", "latin-1"):
-        try:
-            with open(path, mode="r", encoding=enc, **kwargs) as f:
-                return (f.read(), enc) if with_encoding else f.read()
-        except UnicodeDecodeError:
-            pass
-
-
-def write_file(path: str, content: str, overwrite: bool = False, **kwargs):
-    mode = "w" if overwrite else "a"
-    with open(path, mode=mode, encoding="utf-8", **kwargs) as fl:
-        return fl.write(content)
-
-
-if __name__ == "__main__":
-    markdown(read_file("README.md"))
+from functools import wraps
+
+import rich.console
+import rich.theme
+import rich.panel
+import rich.text
+import rich.progress
+import rich.traceback
+import rich.markdown
+import rich.box
+
+__version__ = "4.2.2"
+__ascii__ = False
+theme = rich.theme.Theme({
+    "echo": "bright_white",
+    "echo-bar": "",
+    "echo-pre": "dim bright_white",
+    "info": "",
+    "info-bar": "",
+    "info-pre": "dim",
+    "warn": "red",
+    "warn-bar": "red",
+    "warn-pre": "dim red",
+    "err": "bright_white on red",
+    "err-bar": "bright_red",
+    "err-pre": "dim bright_red",
+    "ask": "yellow",
+    "ask-bar": "yellow",
+    "ask-pre": "dim yellow",
+    "muted": "dim bright_white",
+    "muted-bar": "dim white",
+    "muted-pre": "dim white",
+    "title": "bright_magenta",
+    "pause": "bright_yellow",
+    "choice-i": "yellow",
+    "choice-cmd": "yellow underline",
+})
+console = rich.console.Console(theme=theme)  # main output printer
+rich.traceback.install()
+
+
+def debug(show_locals: bool = True) -> None:
+    rich.traceback.install(show_locals=show_locals)
+
+
+def as_session(name_or_func):  # decorator
+    """print start/title/end info before and after the function call
+
+    Args:
+        title: title will show after the start, if has any
+    """
+    if callable(name_or_func):  # no name provided
+        func = name_or_func
+        name = func.__name__
+        name = "".join([(" " + x) if x.isupper() else x for x in name])
+        name = name.replace("_", " ")
+        return as_session(name)(func)  # deco(func) -> deco(name)(func)
+    else:
+        name = name_or_func
+
+    def get_func(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            start()
+            title(name)
+            result = func(*args, **kwargs)
+            end()
+            return result
+        return wrapper
+    return get_func
+
+
+def start():
+    br()
+
+
+def end():
+    console.print("`" if __ascii__ else "╰")
+
+
+def br(count=1):
+    """print 1 to N blank lines"""
+    print("\n" * (count - 1))
+
+
+def echo(*args, pre: str = "", bar: str = "|" if __ascii__ else "│", style: str = "echo", **options):
+    txt = rich.text.Text()
+    if bar:
+        txt.append(f"{bar}", style=f"{style}-bar" if f"{style}-bar" in theme.styles else style)
+        txt.append(" ")
+    if pre:
+        txt.append(f"({pre.capitalize()})", style=f"{style}-pre" if f"{style}-pre" in theme.styles else style)
+        txt.append(" ")
+    contents = rich.text.Text(" ").join(rich.text.Text.from_markup(f"{arg}") for arg in args)
+    contents.stylize(style)
+    txt.append(contents)
+    console.print(txt, **options)
+
+
+def title(*args, **options):
+    """print something like a title"""
+    console.print(rich.panel.Panel((" ".join([f"{arg}" for arg in args])).upper().strip(), highlight=True, expand=False, box=rich.box.ASCII if __ascii__ else rich.box.ROUNDED), **options)
+
+
+def ask(*args, **options):
+    return echo(*args, pre="?", style="ask", **options)
+
+
+def info(*args, **options):
+    return echo(*args, pre="info", style="info", **options)
+
+
+def warn(*args, **options):
+    return echo(*args, pre="warning", style="warn", **options)
+
+
+def err(*args, **options):
+    return echo(*args, pre="error", style="err", **options)
+
+
+def mute(*args, **options):
+    return echo(*args, style="muted", **options)
+
+
+def print(*args, **options):
+    console.print(*args, **options)
+
+
+def markdown(*args, **options):
+    console.print(rich.markdown.Markdown(" ".join([f"{arg}" for arg in args])))
+
+
+def rule(title: str, *args, **options):
+    console.rule(title, *args, characters="-" if __ascii__ else "─", **options)
+
+
+def panel(txt, title="", subtitle="", expand=True, highlight=True, style="", **options):
+    return console.print(
+        rich.panel.Panel(
+            txt,
+            title=title,
+            subtitle=subtitle,
+            highlight=highlight,
+            expand=expand,
+            style=style,
+            border_style=f"{style}-pre" if f"{style}-pre" in theme.styles else "",
+            box=rich.box.ASCII if __ascii__ else rich.box.ROUNDED,
+            **options
+        )
+    )
+
+
+def pause(msg="Press [Enter] to Continue..."):
+    """press to continue"""
+    with console.status(f"[pause]{rich.markup.escape(msg)}", spinner="point", spinner_style="pause"):
+        return input()
+
+
+def bye(msg=""):
+    """print msg and exit"""
+    exit(msg)
+
+
+def get_input(question: str = "", prompt: str = "> ", default: str = "", strip: bool = True) -> str:
+    """Get user input in stdin.
+
+    Args:
+        question: str. The question asked before get the answer.
+        prompt: str. The prompt shows in the same line with the input field. Always ending with a space.
+        default: str. If the answer is empty, default value returns.
+        strip: bool. Remove leading and trailing whitespaces from user input or not. Default is True.
+    """
+    if default:
+        prompt += f"[dim]({default})[/]"
+    if question:
+        ask(question)
+    if prompt:
+        console.print(prompt.strip(), end=" ")
+    answer = input()
+    if strip:
+        answer = answer.strip()
+    if answer == "":
+        br()
+        return default
+    return answer
+
+
+def get_choice(choices, exitable: bool = False) -> str:
+    """Get user choice from a given list
+
+    Args:
+        choices: list. The list that user can choose from.
+        exitable: bool. Does `exit` is an option for user to select.
+    """
+    EXIT_WORD = "exit" if "0" in choices else "0"
+    DECO_WORD = "[dim]{}[/]".format("--" if __ascii__ else "──")
+    BAR_WORD = "|" if __ascii__ else "│"
+    fill = max(len(EXIT_WORD), 2)
+    for index, item in enumerate(choices, start=1):
+        console.print(f"{BAR_WORD} [choice-i]{index:>{fill}}[/][dim])[/] [white]{item}[/]")
+    if exitable:
+        console.print(f"{BAR_WORD} [choice-i]{EXIT_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]EXIT[/] {DECO_WORD}")
+    user_choice = get_input().strip()
+    if exitable and user_choice == EXIT_WORD:
+        return None
+    if user_choice in choices:
+        return user_choice
+    if user_choice.isdigit():
+        index = int(user_choice) - 1
+        if 0 <= index < len(choices):
+            return choices[index]
+    err("Please enter a valid choice.")
+    return get_choice(choices)
+
+
+def get_choices(choices, allable: bool = False, exitable: bool = False) -> list:
+    def toggle_listitem(itm, lst: list):
+        if itm in lst:
+            lst.remove(itm)
+        else:
+            lst.append(itm)
+        return lst
+
+    EXIT_WORD = "exit" if "0" in choices else "0"
+    DONE_WORD = "done" if "0" in choices else "0"
+    ALL_WORD = "all" if "a" in choices else "a"
+    DECO_WORD = "[dim]{}[/]".format("--" if __ascii__ else "──")
+    BAR_WORD = "|" if __ascii__ else "│"
+    BRACKET_WORD = "[cyan]" + rich.console.escape("[") + "{}][/]"
+    fill = max(len(EXIT_WORD), len(DONE_WORD), len(ALL_WORD), 2)
+    user_choices = []
+    while True:
+        if allable:
+            console.print(f"{BAR_WORD} [choice-i]{ALL_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]ALL[/] {DECO_WORD}")
+        for index, item in enumerate(choices, start=1):
+
+            mark = BRACKET_WORD.format(f"[bright_green]{'+' if __ascii__ else '✓'}[/]") if item in user_choices else BRACKET_WORD.format(" ")  # item is selected or not
+            console.print(f"{BAR_WORD} [choice-i]{index:>{fill}}[/][dim])[/] {mark} [white]{item}")
+        if user_choices:  # user selections > 0
+            console.print(f"{BAR_WORD} [choice-i]{DONE_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]DONE[/] {DECO_WORD}")
+        elif exitable:  # no user selection, but exitable is on.
+            console.print(f"{BAR_WORD} [choice-i]{EXIT_WORD:>{fill}}[/][dim])[/] {DECO_WORD} [choice-cmd]EXIT[/] {DECO_WORD}")
+        user_choice = get_input().strip()
+        if (user_choice == DONE_WORD or user_choice == EXIT_WORD):
+            if exitable or len(user_choices) > 0:  # keep looping when not exitable and no user choices.
+                return user_choices
+        if allable and user_choice == ALL_WORD:
+            if len(user_choices) == len(choices):
+                user_choices = []
+            else:
+                user_choices = choices.copy()
+        elif user_choice in choices:
+            user_choices = toggle_listitem(user_choice, user_choices)
+        elif user_choice.isdigit() and 0 < int(user_choice) <= len(choices):
+            index = int(user_choice) - 1
+            user_choices = toggle_listitem(choices[index], user_choices)
+        else:
+            err("Please enter a valid choice.")
+
+
+def track(iterable, desc="", unit="", *args, **options):
+    with rich.progress.Progress("|" if __ascii__ else "│", rich.progress.SpinnerColumn(), *rich.progress.Progress.get_default_columns(), "·", rich.progress.MofNCompleteColumn(), unit, *args, **options) as progress:
+        task = progress.add_task(desc, total=None if not iterable or not len(iterable) else len(iterable))
+        while not progress.finished:
+            for item in iterable:
+                yield item
+                progress.update(task, advance=1)
+
+
+def read_file(path: str, with_encoding: bool = False, **kwargs):
+    for enc in ("utf-8", "gbk", "cp1252", "windows-1252", "latin-1"):
+        try:
+            with open(path, mode="r", encoding=enc, **kwargs) as f:
+                return (f.read(), enc) if with_encoding else f.read()
+        except UnicodeDecodeError:
+            pass
+
+
+def write_file(path: str, content: str, overwrite: bool = False, **kwargs):
+    mode = "w" if overwrite else "a"
+    with open(path, mode=mode, encoding="utf-8", **kwargs) as fl:
+        return fl.write(content)
+
+
+if __name__ == "__main__":
+    markdown(read_file("README.md"))
```

### Comparing `consoleiotools-4.2.1/consoleiotools/__main__.py` & `consoleiotools-4.2.2/consoleiotools/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,92 @@
-import sys
-import io
-import time
-
-import consoleiotools as cit
-
-
-def inspect(func_name, *args, **kwargs):
-    cit.br()
-    args_txt = ""
-    if args:
-        args_txt += ", ".join(f"{('`' + a + '`') if isinstance(a, str) else str(a)}" for a in args)
-    if kwargs:
-        args_txt += ", " + ", ".join(f"{k}=" + f"{('`' + v + '`') if isinstance(v, str) else str(v)}" for k, v in kwargs.items())
-    cit.print(f"[dim bright_white]# {func_name}({args_txt})")
-    return getattr(cit, func_name)(*args, **kwargs)
-
-
-class fake_input():
-    def __init__(self, user_input: str):
-        self.user_input = user_input
-
-    def __enter__(self):
-        sys.stdin = io.StringIO(self.user_input)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.stdin = sys.__stdin__
-
-
-def examples():
-    inspect("start")
-    inspect("title", "This is a title")
-    inspect("echo", "This is a normal print.")
-    inspect("ask", "This is a question.")
-    inspect("info", "This is a info message.")
-    inspect("warn", "This is a warning message.")
-    inspect("err", "This is an error message.")
-    inspect("mute", "This is a muted message.")
-    inspect("end")
-    inspect("print", "This is a [blue]COLORFUL[/] print.")
-    inspect("markdown", "> *This* **is** a `markdown` print.")
-    inspect(
-        "panel",
-        "This is a panel.",
-        title="Title",
-        subtitle="Subtitle",
-        expand=False
-    )
-    inspect("br")
-    inspect("rule", "This is a horizontal rule.")
-    with fake_input("Apple\n"):
-        result = inspect("get_input", "Get user input:")
-        print("Apple")
-        print(repr(result))
-    with fake_input("1\n"):
-        result = inspect(
-            "get_choice",
-            [
-                "Apple",
-                "Banana",
-            ],
-            exitable=True
-        )
-        print("2")
-        print(repr(result))
-    with fake_input("0\n"):
-        result = inspect(
-            "get_choices",
-            [
-                "Apple",
-                "Banana",
-            ],
-            exitable=True,
-            allable=True
-        )
-        print("0")
-        print(result)
-    inspect("track", "range(10), desc='Progress', unit='unit'")
-    for i in cit.track(range(10), desc="Progress", unit="unit"):
-        time.sleep(0.1)
-    inspect("pause")
-
-
-if __name__ == "__main__":
-    cit.panel(f"cit.__version__ = {cit.__version__}\ncit.__ascii__ = {cit.__ascii__}", title="ConsoleIOTools Features")
-    examples()
+import sys
+import io
+import time
+
+import consoleiotools as cit
+
+
+def inspect(func_name, *args, **kwargs):
+    cit.br()
+    args_txt = ""
+    if args:
+        args_txt += ", ".join(f"{('`' + a + '`') if isinstance(a, str) else str(a)}" for a in args)
+    if kwargs:
+        args_txt += ", " + ", ".join(f"{k}=" + f"{('`' + v + '`') if isinstance(v, str) else str(v)}" for k, v in kwargs.items())
+    cit.print(f"[dim bright_white]# {func_name}({args_txt})")
+    return getattr(cit, func_name)(*args, **kwargs)
+
+
+class fake_input:
+    def __init__(self, user_input: str, double: bool = False):
+        self.double = double
+        self.user_input = user_input.strip().strip("\n") + "\n"
+        if double:
+            self.user_input += self.user_input
+
+    def __enter__(self):
+        sys.stdin = io.StringIO(self.user_input)
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.stdin = sys.__stdin__
+
+
+def examples():
+    inspect("start")
+    inspect("title", "This is a title")
+    inspect("echo", "This is a normal print.")
+    inspect("ask", "This is a question.")
+    inspect("info", "This is a info message.")
+    inspect("warn", "This is a warning message.")
+    inspect("err", "This is an error message.")
+    inspect("mute", "This is a muted message.")
+    inspect("end")
+    inspect("print", "This is a [blue]COLORFUL[/] print.")
+    inspect("markdown", "> *This* **is** a `markdown` print.")
+    inspect(
+        "panel",
+        "This is a panel.",
+        title="Title",
+        subtitle="Subtitle",
+        expand=False
+    )
+    inspect("br")
+    inspect("rule", "This is a horizontal rule.")
+    with fake_input("Apple"):
+        result = inspect("get_input", "Get user input:")
+        print("Apple")
+        print(repr(result))
+    with fake_input("1"):
+        result = inspect(
+            "get_choice",
+            [
+                "Apple",
+                "Banana",
+            ],
+            exitable=True
+        )
+        print("2")
+        print(repr(result))
+    with fake_input("0"):
+        result = inspect(
+            "get_choices",
+            [
+                "Apple",
+                "Banana",
+            ],
+            exitable=True,
+            allable=True
+        )
+        print("0")
+        print(result)
+    inspect("track", "range(10), desc='Progress', unit='unit'")
+    for i in cit.track(range(10), desc="Progress", unit="unit"):
+        time.sleep(0.1)
+    inspect("pause")
+
+
+if __name__ == "__main__":
+    cit.panel("\n".join([
+        f"cit.__version__ = {cit.__version__}",
+        f"cit.__ascii__ = {cit.__ascii__}"
+    ]), title="ConsoleIOTools Features")
+    examples()
```

### Comparing `consoleiotools-4.2.1/consoleiotools.egg-info/PKG-INFO` & `consoleiotools-4.2.2/consoleiotools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,270 +1,270 @@
-Metadata-Version: 2.1
-Name: consoleiotools
-Version: 4.2.1
-Summary: Console tools for inputs and outputs in Python
-Author-email: Kyan <kai@kyan001.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2016 Kyan
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/kyan001/PyConsoleIOTools
-Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleIOTools/issues
-Project-URL: Source Code, https://github.com/kyan001/PyConsoleIOTools
-Keywords: python,console,input,output,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# PyConsoleIOTools
-![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
-![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
-
-## Installation
-
-```sh
-pip install consoleiotools  # install
-pip install --upgrade consoleiotools  # update
-python -m consoleiotools  # examples
-```
-
-## Get Started
-
-```python
-import consoleiotools as cit
-print(cit.__version__)
-```
-
-## Prints on Screen
-
-```python
->>> cit.start()
-# blank line
-
->>> cit.title('Session Name')
-+--------------+
-| SESSION NAME |
-+--------------+
-
->>> cit.echo('Hello World')
-| Hello World
-
->>> cit.echo('Hello World', pre='say', bar='!')
-! (Say) Hello World
-
->>> cit.ask('Hello World')
-| (?) Hello World
-
->>> cit.info('Hello World')
-| (Info) Hello World
-
->>> cit.warn('Hello World')
-| (Warning) Hello World
-
->>> cit.err('Hello World')
-| (Error) Hello World
-
->>> cit.mute('Hello World')
-| Hello World  # muted by dim
-
->>> cit.print(var)  # print variable
-...
-
->>> cit.markdown("# Header")  # print markdown
-+--------------+
-|    Header    |
-+--------------+
-
->>> cit.rule()  # print horizontal rule
-----------------------------------------
-
->>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
----------------- Title ----------------
-
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
-+---------- Panel Title ----------+
-| Panel                           |  # full width
-+-------- Panel Subtitle ---------+
-
->>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
-+- Panel Title -+  # blue
-| Panel         |
-+- Panel Subtit-+
-
->>> cit.end()
-`
-
->>> cit.br()
-# blank line
-
->>> cit.br(2)
-# blank line
-# blank line
-
->>> for var in cit.track(iterables, "Progress"): pass
-| : Progress ---------------------===================  52% 0:00:52 - 52/100
-
->>> cit.__ascii__ = True  # use ascii chars only.
-```
-
-## Get User Input
-
-```python
->>> cit.get_input()  # Get user input from stdin
-> Hello World
-'Hello World'
-
->>> cit.get_input("Question?")  # With a question
-| (?) Question?
-> Yes
-'Yes'
-
->>> cit.get_input(prompt="Answer:")  # With a customized prompt.
-Answer: Apple
-'Apple'
-
->>> cit.get_input("Continue?", default="yes")  # With a default answer.
-| (?) Continue?
-> (yes)  # Entered nothing
-'yes'
-
->>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
->       # Whitespaces
-'    '
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
-|  1) Apple
-|  2) Google
-> 2
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
-|  1) Apple
-|  2) Google
-> Google
-'Google'
-
->>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) Apple
-|  2) Google
-|  0) ** EXIT **
-> 0
-None
-
->>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
-|  1) [ ] Apple
-|  2) [ ] Google
-> 1  # Enter number to check or uncheck selections
-|  1) [+] Apple
-|  2) [ ] Google
-|  0) ** DONE **
-> Google  # Enter string is ok too.
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0  # Enter 0 when done.
-['Apple', 'Google']  # return [] is no selections.
-
->>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
-|  a) ** ALL **
-|  1) [ ] Apple
-|  2) [ ] Google
-> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
-|  a) ** ALL **
-|  1) [+] Apple
-|  2) [+] Google
-|  0) ** DONE **
-> 0
-['Apple', 'Google']
-
->>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
-|  1) [ ] Apple
-|  2) [ ] Google
-|  0) ** EXIT **
-> 0
-[]  # Empty list returned.
-```
-
-## File IO
-
-```python
->>> cit.read_file('/path/to/file')
-'File contents'
-
->>> cit.read_file('/path/to/file', with_encoding=True)
-('File contents', 'utf-8')
-
->>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
-8  # writed bytes
-
->>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
-8  # writed bytes
-```
-
-## Controls
-
-```python
->>> cit.pause()
-| Press [Enter] to Continue...
-
->>> cit.bye()
-# exit
-
->>> cit.bye(0)
-# exit with code 0
-
->>> cit.bye('Seeya')
-Seeya
-# exit
-```
-
-## Decorators
-
-```python
-@cit.as_session('Hello')
-def my_func():
-    cit.echo('World')
-
->>> my_func()
-+---------+
-| HELLO() |
-+---------+
-| World
-`
-
-@cit.as_session
-def underscore_orCamel():
-    pass
-
->>> underscore_orCamel()
-+-----------------------+
-| UNDERSCORE OR CAMEL() |
-+-----------------------+
-`
-```
+Metadata-Version: 2.1
+Name: consoleiotools
+Version: 4.2.2
+Summary: Console tools for inputs and outputs in Python
+Author-email: Kyan <kai@kyan001.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016 Kyan
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/kyan001/PyConsoleIOTools
+Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleIOTools/issues
+Project-URL: Source Code, https://github.com/kyan001/PyConsoleIOTools
+Keywords: python,console,input,output,tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# PyConsoleIOTools
+![PyPI - Downloads](https://img.shields.io/pypi/dm/consoleiotools.svg)
+![GitHub release](https://img.shields.io/github/release/kyan001/PyConsoleIOTools.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleIOTools.svg)](https://github.com/kyan001/PyConsoleIOTools/blob/master/LICENSE)
+
+## Installation
+
+```sh
+pip install consoleiotools  # install
+pip install --upgrade consoleiotools  # update
+python -m consoleiotools  # examples
+```
+
+## Get Started
+
+```python
+import consoleiotools as cit
+print(cit.__version__)
+```
+
+## Prints on Screen
+
+```python
+>>> cit.start()
+# blank line
+
+>>> cit.title('Session Name')
++--------------+
+| SESSION NAME |
++--------------+
+
+>>> cit.echo('Hello World')
+| Hello World
+
+>>> cit.echo('Hello World', pre='say', bar='!')
+! (Say) Hello World
+
+>>> cit.ask('Hello World')
+| (?) Hello World
+
+>>> cit.info('Hello World')
+| (Info) Hello World
+
+>>> cit.warn('Hello World')
+| (Warning) Hello World
+
+>>> cit.err('Hello World')
+| (Error) Hello World
+
+>>> cit.mute('Hello World')
+| Hello World  # muted by dim
+
+>>> cit.print(var)  # print variable
+...
+
+>>> cit.markdown("# Header")  # print markdown
++--------------+
+|    Header    |
++--------------+
+
+>>> cit.rule()  # print horizontal rule
+----------------------------------------
+
+>>> cit.rule("Title", style="blue", align="center")  # print horizontal rule with Title. align = center|left|right
+---------------- Title ----------------
+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle")  # print text in a panel
++---------- Panel Title ----------+
+| Panel                           |  # full width
++-------- Panel Subtitle ---------+
+
+>>> cit.panel("Panel", title="Panel Title", subtitle="Panel Subtitle", expand=False, style="blue")  # fit panel to text
++- Panel Title -+  # blue
+| Panel         |
++- Panel Subtit-+
+
+>>> cit.end()
+`
+
+>>> cit.br()
+# blank line
+
+>>> cit.br(2)
+# blank line
+# blank line
+
+>>> for var in cit.track(iterables, "Progress"): pass
+| : Progress ---------------------===================  52% 0:00:52 - 52/100
+
+>>> cit.__ascii__ = True  # use ascii chars only.
+```
+
+## Get User Input
+
+```python
+>>> cit.get_input()  # Get user input from stdin
+> Hello World
+'Hello World'
+
+>>> cit.get_input("Question?")  # With a question
+| (?) Question?
+> Yes
+'Yes'
+
+>>> cit.get_input(prompt="Answer:")  # With a customized prompt.
+Answer: Apple
+'Apple'
+
+>>> cit.get_input("Continue?", default="yes")  # With a default answer.
+| (?) Continue?
+> (yes)  # Entered nothing
+'yes'
+
+>>> cit.get_input(strip=False)  # Do not remove leading and trailing whitespaces from user input.
+>       # Whitespaces
+'    '
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter number to select.
+|  1) Apple
+|  2) Google
+> 2
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'])  # Enter string is ok too.
+|  1) Apple
+|  2) Google
+> Google
+'Google'
+
+>>> cit.get_choice(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) Apple
+|  2) Google
+|  0) ** EXIT **
+> 0
+None
+
+>>> cit.get_choices(['Apple', 'Google'])  # Multiple Selection
+|  1) [ ] Apple
+|  2) [ ] Google
+> 1  # Enter number to check or uncheck selections
+|  1) [+] Apple
+|  2) [ ] Google
+|  0) ** DONE **
+> Google  # Enter string is ok too.
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0  # Enter 0 when done.
+['Apple', 'Google']  # return [] is no selections.
+
+>>> cit.get_choices(['Apple', 'Google'], allable=True)  # Add a choice of select all in menu.
+|  a) ** ALL **
+|  1) [ ] Apple
+|  2) [ ] Google
+> a  # Enter `a` to check all. If `a` is in choices, enter `all`.
+|  a) ** ALL **
+|  1) [+] Apple
+|  2) [+] Google
+|  0) ** DONE **
+> 0
+['Apple', 'Google']
+
+>>> cit.get_choices(['Apple', 'Google'], exitable=True)  # Add a choice of exit in menu.
+|  1) [ ] Apple
+|  2) [ ] Google
+|  0) ** EXIT **
+> 0
+[]  # Empty list returned.
+```
+
+## File IO
+
+```python
+>>> cit.read_file('/path/to/file')
+'File contents'
+
+>>> cit.read_file('/path/to/file', with_encoding=True)
+('File contents', 'utf-8')
+
+>>> cit.write_file('/path/to/file', 'Contents')  # Append content to file.
+8  # writed bytes
+
+>>> cit.write_file('/path/to/file', 'Contents', overwrite=True)  # Overwrite if file exists.
+8  # writed bytes
+```
+
+## Controls
+
+```python
+>>> cit.pause()
+| Press [Enter] to Continue...
+
+>>> cit.bye()
+# exit
+
+>>> cit.bye(0)
+# exit with code 0
+
+>>> cit.bye('Seeya')
+Seeya
+# exit
+```
+
+## Decorators
+
+```python
+@cit.as_session('Hello')
+def my_func():
+    cit.echo('World')
+
+>>> my_func()
++---------+
+| HELLO() |
++---------+
+| World
+`
+
+@cit.as_session
+def underscore_orCamel():
+    pass
+
+>>> underscore_orCamel()
++-----------------------+
+| UNDERSCORE OR CAMEL() |
++-----------------------+
+`
+```
```

### Comparing `consoleiotools-4.2.1/pyproject.toml` & `consoleiotools-4.2.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "consoleiotools"
-description = "Console tools for inputs and outputs in Python"
-requires-python = ">=3.6"
-readme = "README.md"
-keywords = ["python", "console", "input", "output", "tool"]
-license = {file = "LICENSE"}
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: User Interfaces",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-]
-dependencies = ["rich"]
-dynamic = ["version"]
-
-[[project.authors]]
-name = "Kyan"
-email = "kai@kyan001.com"
-
-[project.optional-dependencies]
-dev = ["build", "wheel", "pycodestyle"]
-
-[project.urls]
-Homepage = "https://github.com/kyan001/PyConsoleIOTools"
-"Issue Tracker" = "https://github.com/kyan001/PyConsoleIOTools/issues"
-"Source Code" = "https://github.com/kyan001/PyConsoleIOTools"
-
-[tool.setuptools]
-py-modules = ["consoleiotools"]
-
-[tool.setuptools.dynamic]
-version = {attr = "consoleiotools.__version__"}
-
-[tool.setuptools.packages.find]
-exclude = ["contrib", "docs", "tests"]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "consoleiotools"
+description = "Console tools for inputs and outputs in Python"
+requires-python = ">=3.6"
+readme = "README.md"
+keywords = ["python", "console", "input", "output", "tool"]
+license = {file = "LICENSE"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: User Interfaces",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+]
+dependencies = ["rich"]
+dynamic = ["version"]
+
+[[project.authors]]
+name = "Kyan"
+email = "kai@kyan001.com"
+
+[project.optional-dependencies]
+dev = ["build", "wheel", "pycodestyle"]
+
+[project.urls]
+Homepage = "https://github.com/kyan001/PyConsoleIOTools"
+"Issue Tracker" = "https://github.com/kyan001/PyConsoleIOTools/issues"
+"Source Code" = "https://github.com/kyan001/PyConsoleIOTools"
+
+[tool.setuptools]
+py-modules = ["consoleiotools"]
+
+[tool.setuptools.dynamic]
+version = {attr = "consoleiotools.__version__"}
+
+[tool.setuptools.packages.find]
+exclude = ["contrib", "docs", "tests"]
```

### Comparing `consoleiotools-4.2.1/tests/test_consoleiotools.py` & `consoleiotools-4.2.2/tests/test_consoleiotools.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,277 +1,277 @@
-from typing import List
-import unittest
-import sys
-import os
-from unittest.mock import patch
-
-from ansiesc import StringIO
-
-sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-import consoleiotools as cit  # noqa: linter (pycodestyle) should not lint this line.
-
-
-class test_consoleiotools(unittest.TestCase):
-    """For testing consoleiotools"""
-    TMP_FILE = "tmp.txt"
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        if os.path.isfile(self.TMP_FILE):
-            os.remove(self.TMP_FILE)
-
-    def test_version(self):
-        self.assertTrue(isinstance(cit.__version__, str))
-
-    def test_start(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.start()
-            self.assertEqual(fake_out.getvalue(), '\n')
-
-    def test_end(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.end()
-            self.assertEqual('╰', fake_out.getvalue().strip())
-
-    def test_ascii(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.__ascii__ = True
-            cit.end()
-            cit.__ascii__ = False
-            self.assertEqual("`", fake_out.getvalue().strip())
-
-    def test_br(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.br(2)
-            self.assertEqual(fake_out.getvalue(), '\n\n')
-
-    def test_echo(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ ABC\n")
-
-    def test_echo_pre(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC", pre="prefix")
-            self.assertEqual(fake_out.getvalue(), "│ (Prefix) ABC\n")
-
-    def test_echo_bar(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.echo("ABC", bar="BAR")
-            self.assertEqual(fake_out.getvalue(), "BAR ABC\n")
-
-    def test_markdown(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.markdown("### ABC")
-            self.assertEqual(fake_out.getvalue().strip(), "ABC")
-
-    def test_panel(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.panel("ABC", title="ABC", subtitle="ABC", expand=False, style="dim")
-            self.assertEqual(fake_out.getvalue().strip(), """
-╭─ ABC ─╮
-│ ABC   │
-╰─ ABC ─╯
-            """.strip())
-
-    def test_title(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.title("ABC")
-            self.assertEqual(fake_out.getvalue().strip(), """
-╭─────╮
-│ ABC │
-╰─────╯
-            """.strip())
-
-    def test_ask(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.ask("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ (?) ABC\n")
-
-    def test_info(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.info("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ (Info) ABC\n")
-
-    def test_warn(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.warn("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ (Warning) ABC\n")
-
-    def test_err(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.err("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ (Error) ABC\n")
-
-    def test_mute(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            cit.mute("ABC")
-            self.assertEqual(fake_out.getvalue(), "│ ABC\n")
-
-    def test_pause(self):
-        with patch("sys.stdin", new=StringIO("\n")):  # simulate press enter
-            cit.pause()
-
-    def test_track(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            for i in cit.track(range(5), disable=True):
-                print(i)
-            self.assertEqual("0\n1\n2\n3\n4\n\n", fake_out.getvalue())
-
-    def test_bye(self):
-        self.assertRaises(SystemExit, cit.bye, None)
-
-    def test_get_input(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
-            userinput = cit.get_input()
-            self.assertIn("> ", fake_out.getvalue())
-            self.assertEqual(userinput, "ABC")
-
-    def test_get_input_question(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
-            userinput = cit.get_input(question="question")
-            self.assertIn("question", fake_out.getvalue())
-            self.assertEqual(userinput, "ABC")
-
-    def test_get_input_prompt(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
-            userinput = cit.get_input(prompt=": ")
-            self.assertIn(": ", fake_out.getvalue())
-            self.assertEqual(userinput, "ABC")
-
-    def test_get_input_default(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("\n")):
-            userinput = cit.get_input(default="answer")
-            self.assertIn("> (answer) ", fake_out.getvalue())
-            self.assertEqual(userinput, "answer")
-
-    def test_get_input_strip(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("  ABC  \n")):
-            userinput = cit.get_input(strip=True)
-            self.assertEqual(userinput, "ABC")
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("  ABC  \n")):
-            userinput = cit.get_input(strip=False)
-            self.assertEqual(userinput, "  ABC  ")
-
-    def test_get_choice(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\n")):
-            self.assertEqual(cit.get_choice(["ABC", "DEF"]), "ABC")
-            self.assertIn("1) ABC", fake_out.getvalue())
-            self.assertIn("2) DEF", fake_out.getvalue())
-
-    def test_get_choice_string(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
-            self.assertEqual(cit.get_choice(["ABC", "DEF"]), "ABC")
-
-    def test_get_choices_done(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\n0\n")):
-            self.assertEqual(cit.get_choices(["ABC", "DEF"]), ["ABC", ])
-            self.assertIn("DONE", fake_out.getvalue())
-
-    def test_get_choices_done_esc(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\ndone\n")):
-            self.assertEqual(cit.get_choices(["ABC", "0"]), ["ABC", ])
-            self.assertIn("done)", fake_out.getvalue())
-
-    def test_get_choices_exitable_esc(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("exit\n")):
-            self.assertEqual(cit.get_choices(["ABC", "0"], exitable=True), [])
-            self.assertIn("exit)", fake_out.getvalue())
-
-    def test_get_choices_exitable(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("0\n")):
-            self.assertEqual(cit.get_choices(["ABC", "DEF"], exitable=True), [])
-            self.assertIn("EXIT", fake_out.getvalue())
-
-    def test_get_choices_allable_off(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\n0\n")):  # allable off
-            self.assertEqual(cit.get_choices(["ABC", "DEF"], exitable=True), [])
-            self.assertIn("Please enter a valid choice.", fake_out.getvalue())
-
-    def test_get_choices_allable_esc(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("all\n0\n")):  # allable off
-            self.assertEqual(cit.get_choices(["a", "DEF"], allable=True, exitable=True), ["a", "DEF"])
-            self.assertIn("all)", fake_out.getvalue())
-
-    def test_get_choices_allable_select(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\n0\n")):  # allable on
-            self.assertEqual(cit.get_choices(["ABC", "DEF"], allable=True), ["ABC", "DEF"])
-            expect_word = "ALL"
-            self.assertIn(expect_word, fake_out.getvalue())
-
-    def test_get_choices_allable_unselect(self):
-        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\na\n0\n")):  # allable on, unselect all.
-            self.assertEqual(cit.get_choices(["ABC", "DEF"], allable=True, exitable=True), [])
-            self.assertIn("[✓] ABC", fake_out.getvalue())
-
-    def test_as_session_1(self):
-        @cit.as_session
-        def func():
-            print('ABC')
-
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            func()
-            self.assertEqual(fake_out.getvalue().strip(), """
-╭──────╮
-│ FUNC │
-╰──────╯
-ABC
-╰
-            """.strip())
-
-    def test_as_session_2(self):
-        @cit.as_session('DEF')
-        def func():
-            print('ABC')
-
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            func()
-            self.assertEqual(fake_out.getvalue().strip(), """
-╭─────╮
-│ DEF │
-╰─────╯
-ABC
-╰
-            """.strip())
-
-    def test_as_session_3(self):
-        @cit.as_session
-        def underscore_orCamel():
-            print('ABC')
-
-        with patch("sys.stdout", new=StringIO()) as fake_out:
-            underscore_orCamel()
-            self.assertEqual(fake_out.getvalue().strip(), """
-╭─────────────────────╮
-│ UNDERSCORE OR CAMEL │
-╰─────────────────────╯
-ABC
-╰
-            """.strip())
-
-    def test_write_file(self):
-        content = "3.1415926"
-        len_write = cit.write_file(self.TMP_FILE, content)
-        self.assertEqual(len_write, len(content))
-
-    def test_write_file_overwrite(self):
-        content = "3.1415926"
-        len_write = cit.write_file(self.TMP_FILE, content, overwrite=True)
-        self.assertEqual(len_write, len(content))
-
-    def test_read_file(self):
-        content = "3.1415926"
-        len_write = cit.write_file(self.TMP_FILE, content)
-        content_read = cit.read_file(self.TMP_FILE)
-        self.assertEqual(content_read, content)
-
-    def test_read_file_with_encoding(self):
-        content = "3.1415926"
-        len_write = cit.write_file(self.TMP_FILE, content)
-        content_read, encoding = cit.read_file(self.TMP_FILE, with_encoding=True)
-        self.assertEqual(encoding, "utf-8")
-
-
-if __name__ == '__main__':
-    unittest.main(verbosity=2, exit=False)
+from typing import List
+import unittest
+import sys
+import os
+from unittest.mock import patch
+
+from ansiesc import StringIO
+
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+import consoleiotools as cit  # noqa: linter (pycodestyle) should not lint this line.
+
+
+class test_consoleiotools(unittest.TestCase):
+    """For testing consoleiotools"""
+    TMP_FILE = "tmp.txt"
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        if os.path.isfile(self.TMP_FILE):
+            os.remove(self.TMP_FILE)
+
+    def test_version(self):
+        self.assertTrue(isinstance(cit.__version__, str))
+
+    def test_start(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.start()
+            self.assertEqual(fake_out.getvalue(), '\n')
+
+    def test_end(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.end()
+            self.assertEqual('╰', fake_out.getvalue().strip())
+
+    def test_ascii(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.__ascii__ = True
+            cit.end()
+            cit.__ascii__ = False
+            self.assertEqual("`", fake_out.getvalue().strip())
+
+    def test_br(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.br(2)
+            self.assertEqual(fake_out.getvalue(), '\n\n')
+
+    def test_echo(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.echo("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ ABC\n")
+
+    def test_echo_pre(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.echo("ABC", pre="prefix")
+            self.assertEqual(fake_out.getvalue(), "│ (Prefix) ABC\n")
+
+    def test_echo_bar(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.echo("ABC", bar="BAR")
+            self.assertEqual(fake_out.getvalue(), "BAR ABC\n")
+
+    def test_markdown(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.markdown("### ABC")
+            self.assertEqual(fake_out.getvalue().strip(), "ABC")
+
+    def test_panel(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.panel("ABC", title="ABC", subtitle="ABC", expand=False, style="dim")
+            self.assertEqual(fake_out.getvalue().strip(), """
+╭─ ABC ─╮
+│ ABC   │
+╰─ ABC ─╯
+            """.strip())
+
+    def test_title(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.title("ABC")
+            self.assertEqual(fake_out.getvalue().strip(), """
+╭─────╮
+│ ABC │
+╰─────╯
+            """.strip())
+
+    def test_ask(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.ask("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ (?) ABC\n")
+
+    def test_info(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.info("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ (Info) ABC\n")
+
+    def test_warn(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.warn("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ (Warning) ABC\n")
+
+    def test_err(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.err("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ (Error) ABC\n")
+
+    def test_mute(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            cit.mute("ABC")
+            self.assertEqual(fake_out.getvalue(), "│ ABC\n")
+
+    def test_pause(self):
+        with patch("sys.stdin", new=StringIO("\n")):  # simulate press enter
+            cit.pause()
+
+    def test_track(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            for i in cit.track(range(5), disable=True):
+                print(i)
+            self.assertEqual("0\n1\n2\n3\n4\n\n", fake_out.getvalue())
+
+    def test_bye(self):
+        self.assertRaises(SystemExit, cit.bye, None)
+
+    def test_get_input(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
+            userinput = cit.get_input()
+            self.assertIn("> ", fake_out.getvalue())
+            self.assertEqual(userinput, "ABC")
+
+    def test_get_input_question(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
+            userinput = cit.get_input(question="question")
+            self.assertIn("question", fake_out.getvalue())
+            self.assertEqual(userinput, "ABC")
+
+    def test_get_input_prompt(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
+            userinput = cit.get_input(prompt=": ")
+            self.assertIn(": ", fake_out.getvalue())
+            self.assertEqual(userinput, "ABC")
+
+    def test_get_input_default(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("\n")):
+            userinput = cit.get_input(default="answer")
+            self.assertIn("> (answer) ", fake_out.getvalue())
+            self.assertEqual(userinput, "answer")
+
+    def test_get_input_strip(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("  ABC  \n")):
+            userinput = cit.get_input(strip=True)
+            self.assertEqual(userinput, "ABC")
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("  ABC  \n")):
+            userinput = cit.get_input(strip=False)
+            self.assertEqual(userinput, "  ABC  ")
+
+    def test_get_choice(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\n")):
+            self.assertEqual(cit.get_choice(["ABC", "DEF"]), "ABC")
+            self.assertIn("1) ABC", fake_out.getvalue())
+            self.assertIn("2) DEF", fake_out.getvalue())
+
+    def test_get_choice_string(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("ABC\n")):
+            self.assertEqual(cit.get_choice(["ABC", "DEF"]), "ABC")
+
+    def test_get_choices_done(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\n0\n")):
+            self.assertEqual(cit.get_choices(["ABC", "DEF"]), ["ABC", ])
+            self.assertIn("DONE", fake_out.getvalue())
+
+    def test_get_choices_done_esc(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("1\ndone\n")):
+            self.assertEqual(cit.get_choices(["ABC", "0"]), ["ABC", ])
+            self.assertIn("done)", fake_out.getvalue())
+
+    def test_get_choices_exitable_esc(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("exit\n")):
+            self.assertEqual(cit.get_choices(["ABC", "0"], exitable=True), [])
+            self.assertIn("exit)", fake_out.getvalue())
+
+    def test_get_choices_exitable(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("0\n")):
+            self.assertEqual(cit.get_choices(["ABC", "DEF"], exitable=True), [])
+            self.assertIn("EXIT", fake_out.getvalue())
+
+    def test_get_choices_allable_off(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\n0\n")):  # allable off
+            self.assertEqual(cit.get_choices(["ABC", "DEF"], exitable=True), [])
+            self.assertIn("Please enter a valid choice.", fake_out.getvalue())
+
+    def test_get_choices_allable_esc(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("all\n0\n")):  # allable off
+            self.assertEqual(cit.get_choices(["a", "DEF"], allable=True, exitable=True), ["a", "DEF"])
+            self.assertIn("all)", fake_out.getvalue())
+
+    def test_get_choices_allable_select(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\n0\n")):  # allable on
+            self.assertEqual(cit.get_choices(["ABC", "DEF"], allable=True), ["ABC", "DEF"])
+            expect_word = "ALL"
+            self.assertIn(expect_word, fake_out.getvalue())
+
+    def test_get_choices_allable_unselect(self):
+        with patch("sys.stdout", new=StringIO()) as fake_out, patch("sys.stdin", new=StringIO("a\na\n0\n")):  # allable on, unselect all.
+            self.assertEqual(cit.get_choices(["ABC", "DEF"], allable=True, exitable=True), [])
+            self.assertIn("[✓] ABC", fake_out.getvalue())
+
+    def test_as_session_1(self):
+        @cit.as_session
+        def func():
+            print('ABC')
+
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            func()
+            self.assertEqual(fake_out.getvalue().strip(), """
+╭──────╮
+│ FUNC │
+╰──────╯
+ABC
+╰
+            """.strip())
+
+    def test_as_session_2(self):
+        @cit.as_session('DEF')
+        def func():
+            print('ABC')
+
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            func()
+            self.assertEqual(fake_out.getvalue().strip(), """
+╭─────╮
+│ DEF │
+╰─────╯
+ABC
+╰
+            """.strip())
+
+    def test_as_session_3(self):
+        @cit.as_session
+        def underscore_orCamel():
+            print('ABC')
+
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            underscore_orCamel()
+            self.assertEqual(fake_out.getvalue().strip(), """
+╭─────────────────────╮
+│ UNDERSCORE OR CAMEL │
+╰─────────────────────╯
+ABC
+╰
+            """.strip())
+
+    def test_write_file(self):
+        content = "3.1415926"
+        len_write = cit.write_file(self.TMP_FILE, content)
+        self.assertEqual(len_write, len(content))
+
+    def test_write_file_overwrite(self):
+        content = "3.1415926"
+        len_write = cit.write_file(self.TMP_FILE, content, overwrite=True)
+        self.assertEqual(len_write, len(content))
+
+    def test_read_file(self):
+        content = "3.1415926"
+        len_write = cit.write_file(self.TMP_FILE, content)
+        content_read = cit.read_file(self.TMP_FILE)
+        self.assertEqual(content_read, content)
+
+    def test_read_file_with_encoding(self):
+        content = "3.1415926"
+        len_write = cit.write_file(self.TMP_FILE, content)
+        content_read, encoding = cit.read_file(self.TMP_FILE, with_encoding=True)
+        self.assertEqual(encoding, "utf-8")
+
+
+if __name__ == '__main__':
+    unittest.main(verbosity=2, exit=False)
```

