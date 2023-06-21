# Comparing `tmp/translit_ru-1.1.tar.gz` & `tmp/translit_ru-1.2.tar.gz`

## Comparing `translit_ru-1.1.tar` & `translit_ru-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 translit_ru-1.1/.gitattributes
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 translit_ru-1.1/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 translit_ru-1.1/.vscode/.gitignore
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 translit_ru-1.1/.vscode/settings.json.skel
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 translit_ru-1.1/.vscode/shell_init_script.bash.skel
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 translit_ru-1.1/ayum/translit/__init__.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 translit_ru-1.1/ayum/translit/translit.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 translit_ru-1.1/tests/test.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 translit_ru-1.1/.gitignore
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 translit_ru-1.1/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 translit_ru-1.1/pyproject.toml
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 translit_ru-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 translit_ru-1.2/.gitattributes
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 translit_ru-1.2/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 translit_ru-1.2/.vscode/.gitignore
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 translit_ru-1.2/.vscode/settings.json.skel
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 translit_ru-1.2/.vscode/shell_init_script.bash.skel
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 translit_ru-1.2/ayum/translit/__init__.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 translit_ru-1.2/ayum/translit/translit.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 translit_ru-1.2/tests/test.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 translit_ru-1.2/.gitignore
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 translit_ru-1.2/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 translit_ru-1.2/pyproject.toml
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 translit_ru-1.2/PKG-INFO
```

### Comparing `translit_ru-1.1/.gitattributes` & `translit_ru-1.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `translit_ru-1.1/ayum/translit/translit.py` & `translit_ru-1.2/ayum/translit/translit.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,20 @@
     ustring = UnicodeString(string)
     nfc = Normalizer2.getNFCInstance()
     ustring = nfc.normalize(ustring)
 
     trans = Transliterator.createFromRules("",
                                            "$wb = [^[:Letter:]] ;"
                                            # е
+                                           "$wb { е } $wb > e ;"
                                            "$wb { е > ye ;"
                                            "[ьъ] { е > ye ;"
                                            "е > e ;"
                                            # э
+                                           "$wb { э } $wb > qe ;"
                                            "$wb { э > e ;"
                                            "[жшцйjwcy] { э > е ;"
                                            "э > qe ;"
                                            # ы
                                            "[жшцйjwcy] { ы > i ;"
                                            "ы > qi ;"
                                            # ё
@@ -32,15 +34,15 @@
                                            "[уеёыаоэяиюьъiuoeaq] { ю > yu ;"
                                            "ю > hu ;"
                                            # я
                                            "$wb { я > ya ;"
                                            "[жшцйjwcy] { я > a ;"
                                            "[уеёыаоэяиюьъiuoeaq] { я > ya ;"
                                            "я > ha ;"
-                                           # Буквосочетание ьо,  только в заимствованных
+                                           # Буквосочетание ьо, только в заимствованных
                                            "ньо > nyo ;"
                                            "льо > lyo ;"
                                            "мьо > myo ;"
                                            "рьо > ryo ;"
                                            # Остальные буквы
                                            "а > a ;"
                                            "б > b ;"
```

### Comparing `translit_ru-1.1/tests/test.py` & `translit_ru-1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `translit_ru-1.1/.gitignore` & `translit_ru-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `translit_ru-1.1/README.md` & `translit_ru-1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 Латинизация русской кириллицы
 =======================
 
 Используется следующее соответствие:
 - *а* —  *a*;
 - *б* —  *b*;
 - *в* —  *v*;
@@ -66,27 +68,27 @@
 - парашют - parawut;
 - аллофон - allofon;
 - съезд - syezd;
 - метр - metr;
 - мэтр - mqetr;
 - лук - luk;
 - люк - lhuk;
-- клык - klqk;
+- клык - klqik;
 - клик - klik;
 - клён - klhon;
 - клон - klon;
 - раса - rasa;
 - ряса - rhasa;
 - пот - pot;
 - под - pod;
 - топ - top;
 - топь - toph;
 - йод - yod;
 - яд - yad;
-- подыграть - podqgrath;
+- подыграть - podqigrath;
 - вожжи - vojji;
 - жужжать - jujjath;
 - объём - obyom;
 - выемка - vqiemka;
 - гальюн - galyun;
 - веет - veet;
 - веешь - veew;
```

### Comparing `translit_ru-1.1/pyproject.toml` & `translit_ru-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `translit_ru-1.1/PKG-INFO` & `translit_ru-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translit-ru
-Version: 1.1
+Version: 1.2
 Summary: Translit russian cyrillic and slugify phrases
 Project-URL: Homepage, https://github.com/ayum/ayum.translit
 Project-URL: Bug Tracker, https://github.com/ayum/ayum.translit/issues
 Author: Aleksey Mikhaylov
 License-Expression: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -13,14 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
+
+
 Латинизация русской кириллицы
 =======================
 
 Используется следующее соответствие:
 - *а* —  *a*;
 - *б* —  *b*;
 - *в* —  *v*;
@@ -85,27 +87,27 @@
 - парашют - parawut;
 - аллофон - allofon;
 - съезд - syezd;
 - метр - metr;
 - мэтр - mqetr;
 - лук - luk;
 - люк - lhuk;
-- клык - klqk;
+- клык - klqik;
 - клик - klik;
 - клён - klhon;
 - клон - klon;
 - раса - rasa;
 - ряса - rhasa;
 - пот - pot;
 - под - pod;
 - топ - top;
 - топь - toph;
 - йод - yod;
 - яд - yad;
-- подыграть - podqgrath;
+- подыграть - podqigrath;
 - вожжи - vojji;
 - жужжать - jujjath;
 - объём - obyom;
 - выемка - vqiemka;
 - гальюн - galyun;
 - веет - veet;
 - веешь - veew;
```

