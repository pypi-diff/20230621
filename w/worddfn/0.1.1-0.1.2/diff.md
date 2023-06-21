# Comparing `tmp/worddfn-0.1.1.tar.gz` & `tmp/worddfn-0.1.2.tar.gz`

## Comparing `worddfn-0.1.1.tar` & `worddfn-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/__init__.py
--rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/__main__.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/dictionaryAPI.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/setting.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.1/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.1/LICENSE
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 worddfn-0.1.1/README.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 worddfn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 worddfn-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0   137387 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Black_logo-no_background.png
+-rwxr-xr-x   0        0        0   198761 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Color_logo-no_background.png
+-rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/Color_logo-no_background_RM.png
+-rwxr-xr-x   0        0        0   151331 2020-02-02 00:00:00.000000 worddfn-0.1.2/images/logo/White_logo-no_background.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/__init__.py
+-rw-r--r--   0        0        0    23496 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/__main__.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/dictionaryAPI.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.2/worddfn/setting.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 worddfn-0.1.2/README.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 worddfn-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 worddfn-0.1.2/PKG-INFO
```

### Comparing `worddfn-0.1.1/worddfn/__main__.py` & `worddfn-0.1.2/worddfn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import pyperclip as _pclp
 from requests import Request, Session, codes
 from requests.exceptions import ConnectionError, HTTPError, Timeout, TooManyRedirects
 
 from worddfn import dictionaryAPI as _da
 from worddfn.setting import setting_handler as _sh
+from worddfn import __version__ as _v
 
 # Manage user setting from .json file.
 GET_SETTINGS = _sh()
 
 API_KEY = GET_SETTINGS["api_key"]
 CLIP = GET_SETTINGS["handler"]
 
@@ -187,14 +188,17 @@
     parser = _ap.ArgumentParser()
 
     # Specify the individual argument use on the CLI.
     parser.add_argument("word", nargs="?")
     parser.add_argument("-f", "--verb", nargs="?")
     parser.add_argument("-s", "--syn", nargs="?")
     parser.add_argument("-o", "--ant", nargs="?")
+    parser.add_argument(
+        "-v", "--version", action="version", version=f"wordDFN version {_v}"
+    )
 
     # Run the parser object and place the extended data in args variable as an argpaser.Namespace object.
     arg = parser.parse_args()
 
     # Convert the object to a dictionary.
     args = vars(arg)
 
@@ -359,15 +363,15 @@
 
 
 def menu(word: str) -> str:
     """Creat a menu for the user to interact with.
     Take the word to search for and return a key that is use to lookup the word."""
 
     key = input(
-        f"{'*'*(55+(len(word)))}\nWhat part would you like to extract from the word {word}?\nOption:\nSelect/type a leter to chose your option:\nDefinition:[d/D]\nVerb:[f/F]\nSynonym:[s/S]\nAntonym:[o/O]\nExit:[q/Q]\nTo clear the clip board press [c/C]\n{'*'*(55+(len(word)))}\n> "
+        f"{'*'*(55+(len(word)))}\nWhat part would you like to extract from the word {word}?\nOption:\nSelect/type a leter to chose your option:\nDefinition:[d/D]\nVerb:[f/F]\nSynonym:[s/S]\nAntonym:[o/O]\nVersion:[v/V]\nExit:[q/Q]\nTo clear the clip board press [c/C]\n{'*'*(55+(len(word)))}\n> "
     )
     key = key.lower()
     while key:
         if key == "d":
             key = "def"
             break
         elif key == "f":
@@ -375,24 +379,26 @@
             break
         elif key == "s":
             key = "syn"
             break
         elif key == "o":
             key = "ant"
             break
+        elif key == "v":
+            _sys.exit(print(f"wordDFN version {_v}"))
         elif key == "c":
             # clear the clipboard and exit.
             _pclp.copy("")
             _sys.exit()
         elif key == "q":
             _sys.exit()
         else:
             print(f"Option invalid , try again")
             key = input(
-                f"{'*'*(55+(len(word)))}\nWhat part would you like to extract from the word {word}?\nOption:\nSelect/type a leter to chose your option:\nDefinition:[d/D]\nVerb:[f/F]\nSynonym:[s/S]\nAntonym:[o/O]\nExit:[q/Q]\nTo clear the clip board press [c/C]\n{'*'*(55+(len(word)))}\n> "
+                f"{'*'*(55+(len(word)))}\nWhat part would you like to extract from the word {word}?\nOption:\nSelect/type a leter to chose your option:\nDefinition:[d/D]\nVerb:[f/F]\nSynonym:[s/S]\nAntonym:[o/O]\nVersion:[v/V]\nExit:[q/Q]\nTo clear the clip board press [c/C]\n{'*'*(55+(len(word)))}\n> "
             )
             key = key.lower()
     return key
 
 
 def main() -> None:
     filePath = _Path.home() / _Path(".Worddfn/data/wordDnf.json")
@@ -505,15 +511,15 @@
 
                     else:
                         # save data to cache:
                         _cache_data(filePath, ant_result, word, key)
                         # word = _pclp.copy("")
 
     elif word == "":
-        print(f"Using cli argument\nrun word -h to view how to run commands")
+        print(f"Using cli argument\nrun word -h to view how to run commands\n")
 
         # Args return from args_handler function.
         words = args_handler()
 
         for k, w in words.items():
             if w != None:
                 key = k
```

### Comparing `worddfn-0.1.1/worddfn/dictionaryAPI.py` & `worddfn-0.1.2/worddfn/dictionaryAPI.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.1/worddfn/setting.py` & `worddfn-0.1.2/worddfn/setting.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.1/LICENSE` & `worddfn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.1/README.md` & `worddfn-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-# wordDFN  
-Search for definition with example, verbs, synonyms and antonyms of a given word.  
-  
+<div align="center">
+<img src= "./images/logo/Color_logo-no_background_RM.png" />  
+
+## Search for definition with example, verbs, synonyms and antonyms of a given word. 
+<br/>
+</div>  
+
+# About wordDFN 
 worddfn is a wordnik API CLI client that uses the **[wordnik](https://developer.wordnik.com/)** API to retrieve data about a single word and parse it into the cli (terminal) for the user.  
 
 ---
 
 ## Requirements  
+
+---
 ### Note  
 **worddfn has not been tested on Mac and Windows at the moment**, but should be able to function properly.  
 On **Mac**, need to assure that the *pbcopy* and *pbpaste* commands are present.  
 On **Windows**, no additional modules are needed.  
 
 1. System
     - Linux:  
@@ -32,14 +39,17 @@
 # CAUTION!  
 While this module (*client*) is release under the MIT License ([see license](#license)) the API is not, wordnik have it's own TOS, i hereby acknowledge those TOS and ask of anyone who come to use this client to do the same. In the source code of this module there are a function that is use to cache data solely for the Purpose of readability (to beter manage the parsing of the data) and nothing else.  
 For more information on the wordnik API TOS [see Wordnik API Terms of Service Agreement](https://developer.wordnik.com/terms "TOS").  
 
 ---
 
 ## How to use  
+
+---
+
 ### INSTALATION  
 before installing this module make sure you have your [API key](#requirements).  
 
 To Install run:
 
 ```
 pip3 install worddfn  
@@ -154,19 +164,25 @@
 cd /path/to/wordDFN/dist
 pip3 install worddfn-x.x.x-py3-none-any.whl
 ```
 
 ---
 
 ## Credits  
+
+---
+
 This project uses:  
 [wordnik](https://www.wordnik.com/) API.  
 [pyperclip](https://pypi.org/project/pyperclip/#description) to help manage the clipboard see [pyperclip repo](https://github.com/asweigart/pyperclip).  
 [xclip](https://github.com/astrand/xclip) as system dependency use by pyperclip.  
 
 ---
 
 ## License  
+
+---
+
 This project is licensed under the terms of the [MIT license](#LICENSE).  
   
 ### WORDNIK API  
 This project also respects and acknowledge the TOS of [wordnik API](https://developer.wordnik.com/terms).
```

### Comparing `worddfn-0.1.1/pyproject.toml` & `worddfn-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.1/PKG-INFO` & `worddfn-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worddfn
-Version: 0.1.1
+Version: 0.1.2
 Summary: worddfn, lookup word meaning and forms via the wordnik api
 Project-URL: Homepage, https://github.com/SirX7/wordDFN
 Project-URL: Bug Tracker, https://github.com/SirX7/wordDFN/issues
 Author-email: Shall Mcfield <xhall.mc@protonmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -17,22 +17,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: requests==2.30.0
 Description-Content-Type: text/markdown
 
-# wordDFN  
-Search for definition with example, verbs, synonyms and antonyms of a given word.  
-  
+<div align="center">
+<img src= "./images/logo/Color_logo-no_background_RM.png" />  
+
+## Search for definition with example, verbs, synonyms and antonyms of a given word. 
+<br/>
+</div>  
+
+# About wordDFN 
 worddfn is a wordnik API CLI client that uses the **[wordnik](https://developer.wordnik.com/)** API to retrieve data about a single word and parse it into the cli (terminal) for the user.  
 
 ---
 
 ## Requirements  
+
+---
 ### Note  
 **worddfn has not been tested on Mac and Windows at the moment**, but should be able to function properly.  
 On **Mac**, need to assure that the *pbcopy* and *pbpaste* commands are present.  
 On **Windows**, no additional modules are needed.  
 
 1. System
     - Linux:  
@@ -55,14 +62,17 @@
 # CAUTION!  
 While this module (*client*) is release under the MIT License ([see license](#license)) the API is not, wordnik have it's own TOS, i hereby acknowledge those TOS and ask of anyone who come to use this client to do the same. In the source code of this module there are a function that is use to cache data solely for the Purpose of readability (to beter manage the parsing of the data) and nothing else.  
 For more information on the wordnik API TOS [see Wordnik API Terms of Service Agreement](https://developer.wordnik.com/terms "TOS").  
 
 ---
 
 ## How to use  
+
+---
+
 ### INSTALATION  
 before installing this module make sure you have your [API key](#requirements).  
 
 To Install run:
 
 ```
 pip3 install worddfn  
@@ -177,19 +187,25 @@
 cd /path/to/wordDFN/dist
 pip3 install worddfn-x.x.x-py3-none-any.whl
 ```
 
 ---
 
 ## Credits  
+
+---
+
 This project uses:  
 [wordnik](https://www.wordnik.com/) API.  
 [pyperclip](https://pypi.org/project/pyperclip/#description) to help manage the clipboard see [pyperclip repo](https://github.com/asweigart/pyperclip).  
 [xclip](https://github.com/astrand/xclip) as system dependency use by pyperclip.  
 
 ---
 
 ## License  
+
+---
+
 This project is licensed under the terms of the [MIT license](#LICENSE).  
   
 ### WORDNIK API  
 This project also respects and acknowledge the TOS of [wordnik API](https://developer.wordnik.com/terms).
```

