# Comparing `tmp/django-translatemessages-0.0.3.tar.gz` & `tmp/django-translatemessages-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-translatemessages-0.0.3.tar", last modified: Mon Jun 12 14:47:46 2023, max compression
+gzip compressed data, was "django-translatemessages-0.0.4.tar", last modified: Wed Jun 21 10:30:31 2023, max compression
```

## Comparing `django-translatemessages-0.0.3.tar` & `django-translatemessages-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       53 2023-06-12 08:55:29.000000 django-translatemessages-0.0.3/CHANGELOG.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.3/LICENSE
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.3/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4117 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3075 2023-06-12 14:40:26.000000 django-translatemessages-0.0.3/README.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-12 14:07:48.000000 django-translatemessages-0.0.3/django_translatemessages/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/management/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.3/django_translatemessages/management/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/management/commands/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.3/django_translatemessages/management/commands/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11506 2023-06-12 13:57:29.000000 django-translatemessages-0.0.3/django_translatemessages/management/commands/translatemessages.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4117 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.3/setup.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      125 2023-06-21 10:29:53.000000 django-translatemessages-0.0.4/CHANGELOG.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.4/LICENSE
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.4/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4191 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3077 2023-06-12 15:37:11.000000 django-translatemessages-0.0.4/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-21 10:28:43.000000 django-translatemessages-0.0.4/django_translatemessages/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/management/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.4/django_translatemessages/management/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/management/commands/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.4/django_translatemessages/management/commands/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11579 2023-06-21 10:28:43.000000 django-translatemessages-0.0.4/django_translatemessages/management/commands/translatemessages.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4191 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.4/setup.py
```

### Comparing `django-translatemessages-0.0.3/LICENSE` & `django-translatemessages-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.3/PKG-INFO` & `django-translatemessages-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.3
+Version: 0.0.4
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -47,15 +47,15 @@
 
 
 Configuration
 -------------
 
 You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters)
 
 To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
@@ -95,16 +95,17 @@
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
 **IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
-This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
-search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+This force the developer to validate manually each translation.
+
+To do so, edit each ``django.po`` file, search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
 Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
 and press ``CTRL + RETURN`` on each highlighted translation you agree.
 
 To disable auto-fuzzy feature, use this in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "auto_fuzzy": False,
@@ -123,11 +124,15 @@
 
 For more options, run ``python ./manage.py translatemessages -h``
 
 
 News
 ----
 
+0.0.4 (2023-06-21)
+------------------
+- Do not translate fuzzy strings
+
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.3/README.rst` & `django-translatemessages-0.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 Configuration
 -------------
 
 You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters)
 
 To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
@@ -67,16 +67,17 @@
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
 **IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
-This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
-search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+This force the developer to validate manually each translation.
+
+To do so, edit each ``django.po`` file, search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
 Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
 and press ``CTRL + RETURN`` on each highlighted translation you agree.
 
 To disable auto-fuzzy feature, use this in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "auto_fuzzy": False,
```

### Comparing `django-translatemessages-0.0.3/django_translatemessages/management/commands/translatemessages.py` & `django-translatemessages-0.0.4/django_translatemessages/management/commands/translatemessages.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     locations.extend(
                         (dirpath, f) for f in filenames if f.endswith(".po")
                     )
             if locations:
                 self.translate_messages(locations)
 
         if self.has_errors:
-            raise CommandError("compilemessages generated one or more errors.")
+            raise CommandError("translatemessages generated one or more errors.")
 
     def translate_messages(self, locations):
         for location in locations:
             path = Path(os.sep.join(location))
             self.translate_pofile(path)
 
     def translate_pofile(self, path):
@@ -268,15 +268,17 @@
                 self.stdout.write(
                     colorize(f"{entry.msgid}", fg="blue"),
                     ending="",
                 )
                 self.stdout.write(colorize(f"-> {translated_text}", fg="cyan"))
         else:
             for entry in po:
-                if not entry.translated() or self.options["all"]:
+                if (
+                    not entry.translated() and "fuzzy" not in entry.flags
+                ) or self.options["all"]:
                     filtered_msgid = self.filter_msgid(entry.msgid)
                     if filtered_msgid:
                         nb_translations += 1
                         self.stdout.write(
                             colorize(f"{entry.msgid}", fg="blue"),
                             ending="",
                         )
```

### Comparing `django-translatemessages-0.0.3/django_translatemessages.egg-info/PKG-INFO` & `django-translatemessages-0.0.4/django_translatemessages.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.3
+Version: 0.0.4
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -47,15 +47,15 @@
 
 
 Configuration
 -------------
 
 You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters)
 
 To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
@@ -95,16 +95,17 @@
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
 **IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
-This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
-search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+This force the developer to validate manually each translation.
+
+To do so, edit each ``django.po`` file, search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
 Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
 and press ``CTRL + RETURN`` on each highlighted translation you agree.
 
 To disable auto-fuzzy feature, use this in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "auto_fuzzy": False,
@@ -123,11 +124,15 @@
 
 For more options, run ``python ./manage.py translatemessages -h``
 
 
 News
 ----
 
+0.0.4 (2023-06-21)
+------------------
+- Do not translate fuzzy strings
+
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.3/django_translatemessages.egg-info/SOURCES.txt` & `django-translatemessages-0.0.4/django_translatemessages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.3/setup.py` & `django-translatemessages-0.0.4/setup.py`

 * *Files identical despite different names*

