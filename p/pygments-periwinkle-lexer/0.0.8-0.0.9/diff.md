# Comparing `tmp/pygments-periwinkle-lexer-0.0.8.tar.gz` & `tmp/pygments-periwinkle-lexer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments-periwinkle-lexer-0.0.8.tar", last modified: Thu Mar 30 15:32:56 2023, max compression
+gzip compressed data, was "pygments-periwinkle-lexer-0.0.9.tar", last modified: Thu Mar 30 16:13:45 2023, max compression
```

## Comparing `pygments-periwinkle-lexer-0.0.8.tar` & `pygments-periwinkle-lexer-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 15:32:56.572999 pygments-periwinkle-lexer-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-03-19 16:08:19.000000 pygments-periwinkle-lexer-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      654 2023-03-30 15:32:56.572999 pygments-periwinkle-lexer-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-03-19 16:12:58.000000 pygments-periwinkle-lexer-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 15:32:56.572999 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer/
--rw-rw-rw-   0        0        0       79 2023-03-19 15:10:47.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer/__init__.py
--rw-rw-rw-   0        0        0     1975 2023-03-30 15:19:52.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer/periwinkle_lexer.py
-drwxrwxrwx   0        0        0        0 2023-03-30 15:32:56.572999 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/
--rw-rw-rw-   0        0        0      654 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-03-30 15:32:56.000000 pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 15:32:56.572999 pygments-periwinkle-lexer-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-03-30 15:07:02.000000 pygments-periwinkle-lexer-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 16:13:45.689463 pygments-periwinkle-lexer-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-03-19 16:08:19.000000 pygments-periwinkle-lexer-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      654 2023-03-30 16:13:45.689463 pygments-periwinkle-lexer-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-03-19 16:12:58.000000 pygments-periwinkle-lexer-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-30 16:13:45.689463 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer/
+-rw-rw-rw-   0        0        0       79 2023-03-19 15:10:47.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer/__init__.py
+-rw-rw-rw-   0        0        0     1974 2023-03-30 16:12:13.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer/periwinkle_lexer.py
+drwxrwxrwx   0        0        0        0 2023-03-30 16:13:45.689463 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/
+-rw-rw-rw-   0        0        0      654 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-03-30 16:13:45.000000 pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-30 16:13:45.689463 pygments-periwinkle-lexer-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-03-30 16:13:20.000000 pygments-periwinkle-lexer-0.0.9/setup.py
```

### Comparing `pygments-periwinkle-lexer-0.0.8/LICENSE` & `pygments-periwinkle-lexer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments-periwinkle-lexer-0.0.8/PKG-INFO` & `pygments-periwinkle-lexer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-periwinkle-lexer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Лексер для Барвінку.
 Home-page: https://github.com/periwinkle-lang
 Author: Федуняк Роман
 Author-email: fedynuak.roma@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer/periwinkle_lexer.py` & `pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer/periwinkle_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name = 'Periwinkle'
     aliases = ['periwinkle']
     filenames = ['*.бр', '.барвінок']
     flags = re.UNICODE
 
     tokens = {
         'root': [
-            (r'\A#!.*$', Comment.Hashbang),
+            (r'\A#!.*', Comment.Hashbang),
             (r'//.*', Comment),
             (r'/\*', Comment.Multiline, 'multilineComment'),
             (r'\b(друк|друкр|зчитати|ітератор|Число|Логічний|Стрічка|Дійсний|Масив|КінецьІтерації)\b', Name.Builtin),
             (r'(\bфункція\b)(\s*)(\b[а-яА-ЯїієґЇІЄҐ_][а-яА-ЯїієґЇІЄҐ0-9_]*\b)(?=\s*\()', bygroups(Keyword.Control, Text.Whitespace, Name.Function)),
             (r',|[.]{3}', Punctuation),
             (r'\b[а-яА-ЯїієґЇІЄҐ_][а-яА-ЯїієґЇІЄҐ0-9_]*\b(?=\()', Name.Function),
             (r'\b(якщо|або якщо|інакше|кінець|поки|завершити|продовжити|повернути|кожній|з)\b', Keyword),
```

### Comparing `pygments-periwinkle-lexer-0.0.8/pygments_periwinkle_lexer.egg-info/PKG-INFO` & `pygments-periwinkle-lexer-0.0.9/pygments_periwinkle_lexer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-periwinkle-lexer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Лексер для Барвінку.
 Home-page: https://github.com/periwinkle-lang
 Author: Федуняк Роман
 Author-email: fedynuak.roma@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygments-periwinkle-lexer-0.0.8/setup.py` & `pygments-periwinkle-lexer-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 entry_points = '''
 [pygments.lexers]
 барвінок=pygments_periwinkle_lexer:PeriwinkleLexer
 '''
 
 setup(
     name='pygments-periwinkle-lexer',
-    version='0.0.8',
+    version='0.0.9',
     description='Лексер для Барвінку.',
     long_description="Пакет для Pygments, який додає підсвічування синтаксису для мови програмування Барвінок",
     author='Федуняк Роман',
     author_email='fedynuak.roma@gmail.com',
     url='https://github.com/periwinkle-lang',
     packages=find_packages(),
     entry_points=entry_points,
```

