# Comparing `tmp/arabic2latin-1.1.3.tar.gz` & `tmp/arabic2latin-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabic2latin-1.1.3.tar", last modified: Thu May 11 10:51:16 2023, max compression
+gzip compressed data, was "arabic2latin-1.1.4.tar", last modified: Wed Jun 21 20:01:12 2023, max compression
```

## Comparing `arabic2latin-1.1.3.tar` & `arabic2latin-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/
--rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3219 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1203 2023-05-07 20:26:17.000000 arabic2latin-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.294223 arabic2latin-1.1.3/arabic2latin/
--rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.3/arabic2latin/__init__.py
--rw-rw-rw-   0        0        0     3765 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/arabic2latin/arabic2latin.py
--rw-rw-rw-   0        0        0       23 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/arabic2latin/version.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/arabic2latin.egg-info/
--rw-rw-rw-   0        0        0     3219 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-11 10:51:16.000000 arabic2latin-1.1.3/arabic2latin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-05-09 12:22:36.000000 arabic2latin-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 10:51:16.325616 arabic2latin-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:01:12.504597 arabic2latin-1.1.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3219 2023-06-21 20:01:12.504597 arabic2latin-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1203 2023-05-07 20:26:17.000000 arabic2latin-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 20:01:12.479950 arabic2latin-1.1.4/arabic2latin/
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.4/arabic2latin/__init__.py
+-rw-rw-rw-   0        0        0     4008 2023-06-21 19:58:29.000000 arabic2latin-1.1.4/arabic2latin/arabic2latin.py
+-rw-rw-rw-   0        0        0       23 2023-06-21 19:56:07.000000 arabic2latin-1.1.4/arabic2latin/version.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:01:12.502529 arabic2latin-1.1.4/arabic2latin.egg-info/
+-rw-rw-rw-   0        0        0     3219 2023-06-21 20:01:12.000000 arabic2latin-1.1.4/arabic2latin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-21 20:01:12.000000 arabic2latin-1.1.4/arabic2latin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:01:12.000000 arabic2latin-1.1.4/arabic2latin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-21 20:01:12.000000 arabic2latin-1.1.4/arabic2latin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-06-21 19:56:07.000000 arabic2latin-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 20:01:12.504597 arabic2latin-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.4/setup.py
```

### Comparing `arabic2latin-1.1.3/LICENSE` & `arabic2latin-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.1.3/PKG-INFO` & `arabic2latin-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.1.3/README.md` & `arabic2latin-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.1.3/arabic2latin/arabic2latin.py` & `arabic2latin-1.1.4/arabic2latin/arabic2latin.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,102 +3,110 @@
     'ج': 'j', 'ح': 'h', 'خ': 'kh', 'د': 'd', 'ذ': 'th', 'ر': 'r', 'ز': 'z',
     'ُژ': 'j', 'س': 's', 'ش': 'sh', 'ص': 's', 'ض': 'dh', 'ط': 't', 'ظ': 'z', 'ع': 'aa',
     'غ': 'gh', 'ف': 'f', 'ق': 'q', 'ك': 'k', 'ک': 'k', 'گ': 'g', 'ل': 'l', 'م': 'm',
     'ن': 'n', 'ه': 'h', 'ة': 'ah', 'و': 'o', 'ؤ': 'o\'', 'ي': 'y', 'ی': 'y', 'ى': 'y',
     'ٰ': 'aa', 'َ': 'a', 'ُ': 'o', 'ِ': 'e', 'ٌ': 'on', 'ً': 'an', 'ٍ': 'en', 'ء': '', 'ئ': '\'e'
 }
 
-# vowels and sokoon sign:
-VOWELS = ['a', 'e', 'i', 'o', 'u', 'ْ']
+# vowels:
+VOWELS = ['a', 'e', 'i', 'o', 'u']
 
 
-def arabic_to_latin(text, debug=False):
-    n = len(text)
+def arabic_to_latin(text: str, debug=False):
+    end_index = len(text) - 1
     result = ''
     no_vowel = False
     special_case = False
-    for c, char in enumerate(text):
+    for i, char in enumerate(text):
         if special_case:
             special_case = False
             continue
 
         if char in MAPPING:
-            if c == 0 or text[c-1] == " ":
-                if char in "اأ" and text[c+1] in "ىيی":
+            if i == 0 or text[i-1] == " ":
+                if char in "اأ" and text[i+1] in "ىيی":
                     result += "ei"
                     special_case = True
 
-                elif char in "اأ" and text[c+1] in "وؤ":
+                elif char in "اأ" and text[i+1] in "وؤ":
                     result += "ou"
                     special_case = True
 
-                elif char in "ىيی" and text[c+1] in "ؤو":
+                elif char in "ىيی" and text[i+1] in "ؤو":
                     result += "yoo"
                     special_case = True
 
                 elif char == "و":
                     result += "v"
 
                 else:
                     result += MAPPING[char]
 
-            elif char in "ىيی" and (c != n-1 and text[c+1] in MAPPING):
+            elif char in "ىيی" and (i != end_index and text[i+1] in MAPPING):
                 result += "i"
 
-            elif char == "و":
-                if (c != n-1 and text[c+1] in "اىيی") and (c == n-2 or text[c:].startswith("وا ")):
-                    if result[-1] == "o":
-                        result += "o"
-                    else:
-                        result += "oo"
-                    special_case = True
-
-                elif text[c-1] in "اىيی" or (c != n-1 and text[c+1] in "اىيی"):
-                    if result[-1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
-                        if not no_vowel:
-                            result += "a"
-                        else:
-                            no_vowel = False
-
-                    result += "v"
-
+            elif char == "و" and (i != end_index and text[i+1] == "ا") and (
+                    i == end_index - 1 or text[i:].startswith("وا ")
+            ):
+                if result[-1] == "o":
+                    result += "o"
                 else:
-                    result += MAPPING[char]
+                    result += "oo"
+                special_case = True
 
-            elif char == "ه" and (c == n-1 or (c != n-1 and text[c+1] == " ")):
+            elif char == "ه" and (i == end_index or (i != end_index and text[i+1] == " ")):
                 result += "ah"
 
+            elif (i == end_index or text[i+1] == " ") and char == "ع":
+                if result[-1] == "i":
+                    result += "'"
+
             elif result:
-                if result[-1] not in VOWELS and MAPPING[char][:1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
+                # handling special case of double ل in اللّه
+                if char == "ل" and (i != end_index and text[i+1] == "ل"):
+                    special_case = True
+
+                if (
+                        result[-1] not in VOWELS and MAPPING[char][:1] not in VOWELS
+                        and result[-3:] not in " al" and MAPPING[char] != "y"
+                ):
                     if not no_vowel:
                         result += "a"
                     else:
                         no_vowel = False
 
+                if char == "و" and (text[i - 1] in "اىيی" or (i != end_index and text[i + 1] in "ىيی")):
+                    result += "av"
+                    continue
+
                 # prevent occurrence of a letter for more than two times
                 if not result.endswith(MAPPING[char] * 2):
                     # handle two character replacements
                     if result[-1] * 2 == MAPPING[char]:
                         result += MAPPING[char][0]
                     else:
                         result += MAPPING[char]
 
         elif ord(char) < 128:
             result += char
 
         # tashdid:
         elif char == "ّ":
             # prevent occurrence of a letter for more than two times
-            if result[-2:] != MAPPING[text[c-1]] * 2:
-                result += MAPPING[text[c - 1]]
+            if result[-2:] != MAPPING[text[i-1]] * 2:
+                result += MAPPING[text[i - 1]]
 
         # sokoon:
         elif char == "ْ":
             no_vowel = True
 
         elif char == "ـْ":
             pass
 
         elif debug:
             return f"unknown character: {char}"
 
     return result
+
+
+if __name__ == '__main__':
+    print(arabic_to_latin('شفیع مهدوی', debug=True))
```

### Comparing `arabic2latin-1.1.3/arabic2latin.egg-info/PKG-INFO` & `arabic2latin-1.1.4/arabic2latin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
```

### Comparing `arabic2latin-1.1.3/pyproject.toml` & `arabic2latin-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arabic2latin"
-version = "1.1.3"
+version = "1.1.4"
 description = "Convert Arabic characters to their Latin (English) homophones."
 readme = "README.md"
 requires-python = ">=3.6"
 license= {file = "LICENSE"}
 keywords=["arabic", "homophone", "arabic to english", "arabic to latin"]
 authors = [
   {email = "rexa222@outlook.com"},
```

### Comparing `arabic2latin-1.1.3/setup.py` & `arabic2latin-1.1.4/setup.py`

 * *Files identical despite different names*

