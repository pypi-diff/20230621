# Comparing `tmp/hikari-miru-3.1.1.tar.gz` & `tmp/hikari-miru-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-miru-3.1.1.tar", last modified: Sun Apr 30 15:38:46 2023, max compression
+gzip compressed data, was "hikari-miru-3.1.2.tar", last modified: Wed Jun 21 11:40:00 2023, max compression
```

## Comparing `hikari-miru-3.1.1.tar` & `hikari-miru-3.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.158248 hikari-miru-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-30 15:38:46.158248 hikari-miru-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/hikari_miru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-30 15:38:46.000000 hikari-miru-3.1.1/hikari_miru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-30 15:38:46.000000 hikari-miru-3.1.1/hikari_miru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:38:46.000000 hikari-miru-3.1.1/hikari_miru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:38:45.000000 hikari-miru-3.1.1/hikari_miru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-30 15:38:46.000000 hikari-miru-3.1.1/hikari_miru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 15:38:46.000000 hikari-miru-3.1.1/hikari_miru.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/miru/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/miru/abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/abc/item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/abc/item_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/miru/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/context/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/context/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/context/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.150247 hikari-miru-3.1.1/miru/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/miru/ext/nav/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/items.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.154248 hikari-miru-3.1.1/miru/ext/nav/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/ext/nav/utils/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:38:46.158248 hikari-miru-3.1.1/miru/select/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/select/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/text_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/miru/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 15:38:46.158248 hikari-miru-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-30 15:38:37.000000 hikari-miru-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.161527 hikari-miru-3.1.2/hikari_miru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-21 11:40:00.000000 hikari-miru-3.1.2/hikari_miru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-21 11:40:00.000000 hikari-miru-3.1.2/hikari_miru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:40:00.000000 hikari-miru-3.1.2/hikari_miru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:39:59.000000 hikari-miru-3.1.2/hikari_miru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 11:40:00.000000 hikari-miru-3.1.2/hikari_miru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 11:40:00.000000 hikari-miru-3.1.2/hikari_miru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.161527 hikari-miru-3.1.2/miru/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.161527 hikari-miru-3.1.2/miru/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/abc/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/abc/item_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.161527 hikari-miru-3.1.2/miru/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/context/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/context/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/context/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.157527 hikari-miru-3.1.2/miru/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/miru/ext/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/miru/ext/nav/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/ext/nav/utils/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/miru/select/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/select/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/miru/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:40:00.165527 hikari-miru-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 11:39:50.000000 hikari-miru-3.1.2/setup.py
```

### Comparing `hikari-miru-3.1.1/LICENSE` & `hikari-miru-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/PKG-INFO` & `hikari-miru-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-miru
-Version: 3.1.1
+Version: 3.1.2
 Summary: An alternative component handler for hikari, inspired by discord.py's views.
 Home-page: https://github.com/HyperGH/hikari-miru
 Author: HyperGH
 Author-email: 46067571+HyperGH@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
```

### Comparing `hikari-miru-3.1.1/README.md` & `hikari-miru-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/hikari_miru.egg-info/PKG-INFO` & `hikari-miru-3.1.2/hikari_miru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-miru
-Version: 3.1.1
+Version: 3.1.2
 Summary: An alternative component handler for hikari, inspired by discord.py's views.
 Home-page: https://github.com/HyperGH/hikari-miru
 Author: HyperGH
 Author-email: 46067571+HyperGH@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
```

### Comparing `hikari-miru-3.1.1/hikari_miru.egg-info/SOURCES.txt` & `hikari-miru-3.1.2/hikari_miru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/__init__.py` & `hikari-miru-3.1.2/miru/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "mentionable_select",
     "TextInput",
     "MiruAware",
     "View",
     "get_view",
 )
 
-__version__ = "3.1.1"
+__version__ = "3.1.2"
 
 # MIT License
 #
 # Copyright (c) 2022-present HyperGH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari-miru-3.1.1/miru/__main__.py` & `hikari-miru-3.1.2/miru/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/abc/__init__.py` & `hikari-miru-3.1.2/miru/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/abc/item.py` & `hikari-miru-3.1.2/miru/abc/item.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/abc/item_handler.py` & `hikari-miru-3.1.2/miru/abc/item_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         """
         The last context that was received by the item handler.
         """
         return self._last_context
 
     @property
     @abc.abstractmethod
-    def _builder(self) -> type[BuilderT]:
+    def _builder(self) -> t.Type[BuilderT]:
         ...
 
     def add_item(self, item: Item[BuilderT]) -> ItemHandler[BuilderT]:
         """Adds a new item to the item handler.
 
         Parameters
         ----------
```

### Comparing `hikari-miru-3.1.1/miru/bootstrap.py` & `hikari-miru-3.1.2/miru/bootstrap.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/button.py` & `hikari-miru-3.1.2/miru/button.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/context/__init__.py` & `hikari-miru-3.1.2/miru/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/context/base.py` & `hikari-miru-3.1.2/miru/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/context/modal.py` & `hikari-miru-3.1.2/miru/context/modal.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/context/raw.py` & `hikari-miru-3.1.2/miru/context/raw.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/context/view.py` & `hikari-miru-3.1.2/miru/context/view.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/events.py` & `hikari-miru-3.1.2/miru/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     _bound_handlers: t.MutableMapping[hikari.Snowflakeish, ItemHandler[t.Any]] = {}
     """A mapping of message_id to ItemHandler. This contains handlers that are bound to a message or custom_id."""
 
     _handlers: t.MutableMapping[str, ItemHandler[t.Any]] = {}
     """A mapping of custom_id to ItemHandler. This only contains handlers that are not bound to a message."""
 
-    def __new__(cls: type[EventHandler]) -> EventHandler:
+    def __new__(cls: t.Type[EventHandler]) -> EventHandler:
         if not hasattr(cls, "instance"):  # Ensure that class remains singleton
             cls.instance = super(EventHandler, cls).__new__(cls)
         return cls.instance
 
     def start(self, app: MiruAware) -> None:
         """Start all custom event listeners, this is called during miru.install()"""
         if self._app is not None:
```

### Comparing `hikari-miru-3.1.1/miru/exceptions.py` & `hikari-miru-3.1.2/miru/exceptions.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/ext/nav/README.md` & `hikari-miru-3.1.2/miru/ext/nav/README.md`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/ext/nav/__init__.py` & `hikari-miru-3.1.2/miru/ext/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/ext/nav/items.py` & `hikari-miru-3.1.2/miru/ext/nav/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     def __init__(
         self,
         *,
         custom_id: t.Optional[str] = None,
         row: t.Optional[int] = None,
         position: t.Optional[int] = None,
         disabled: bool = False,
+        width: int = 1,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row, position=position, disabled=disabled)
+        super().__init__(custom_id=custom_id, row=row, width=width, position=position, disabled=disabled)
         self._handler: t.Optional[NavigatorView] = None
 
     async def before_page_change(self) -> None:
         """
         Called when the navigator is about to transition to the next page. Also called before the first page is sent.
         """
         pass
```

### Comparing `hikari-miru-3.1.1/miru/ext/nav/navigator.py` & `hikari-miru-3.1.2/miru/ext/nav/navigator.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/ext/nav/utils/__init__.py` & `hikari-miru-3.1.2/miru/ext/nav/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/ext/nav/utils/paginator.py` & `hikari-miru-3.1.2/miru/ext/nav/utils/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         if len(self._prefix + line + self._line_separator + self._suffix) > self._max_len:
             raise ValueError(
                 f"A single line cannot be longer than the maximum length of a page ({self._max_len} characters)."
             )
 
         if not self._pages:
-            self._pages[0] = self._prefix
+            self._pages.append(self._prefix)
 
         # If content fits on page
         if not len(self._pages[-1]) + len(f"{line}{self._line_separator}{self._suffix}") >= self._max_len:
             self._pages[-1] += f"{line}{self._line_separator}"
         # If not, finish this page, start a new one, repeat
         else:
             self._pages[-1] += self._suffix
```

### Comparing `hikari-miru-3.1.1/miru/modal.py` & `hikari-miru-3.1.2/miru/modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     def last_context(self) -> t.Optional[ModalContext]:
         """
         Context proxying the last interaction that was received by the modal.
         """
         return t.cast(ModalContext, self._last_context)
 
     @property
-    def _builder(self) -> type[hikari.impl.ModalActionRowBuilder]:
+    def _builder(self) -> t.Type[hikari.impl.ModalActionRowBuilder]:
         return hikari.impl.ModalActionRowBuilder
 
     @property
     def children(self) -> t.Sequence[ModalItem]:
         return t.cast(t.Sequence[ModalItem], super().children)
 
     def add_item(self, item: Item[hikari.impl.ModalActionRowBuilder]) -> Modal:
@@ -256,15 +256,15 @@
 
         self.stop()  # Modals can only receive one response
 
     async def _process_interactions(self, event: hikari.InteractionCreateEvent) -> None:
         if not isinstance(event.interaction, hikari.ModalInteraction):
             return
 
-        children = {item.custom_id: item for item in self.children if isinstance(item, ModalItem)}
+        children = {item.custom_id: item for item in self.children}
 
         values = {  # Check if any components match the provided custom_ids
             children[component.custom_id]: component.value
             for action_row in event.interaction.components
             for component in action_row.components
             if children.get(component.custom_id) is not None
         }
```

### Comparing `hikari-miru-3.1.1/miru/select/base.py` & `hikari-miru-3.1.2/miru/select/base.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/select/channel.py` & `hikari-miru-3.1.2/miru/select/channel.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/select/mentionable.py` & `hikari-miru-3.1.2/miru/select/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/select/role.py` & `hikari-miru-3.1.2/miru/select/role.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/select/text.py` & `hikari-miru-3.1.2/miru/select/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,18 +185,14 @@
                 emoji=option.emoji or hikari.UNDEFINED,
             )
 
     @property
     def values(self) -> t.Sequence[str]:
         return self._values
 
-    @property
-    def width(self) -> int:
-        return 5
-
     async def _refresh_state(self, context: Context[hikari.ComponentInteraction]) -> None:
         assert isinstance(context, ViewContext)
         self._values = context.interaction.values
 
 
 def text_select(
     *,
```

### Comparing `hikari-miru-3.1.1/miru/select/user.py` & `hikari-miru-3.1.2/miru/select/user.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/text_input.py` & `hikari-miru-3.1.2/miru/text_input.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/traits.py` & `hikari-miru-3.1.2/miru/traits.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/miru/view.py` & `hikari-miru-3.1.2/miru/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     def last_context(self) -> t.Optional[ViewContext]:
         """
         The last context that was received by the view.
         """
         return t.cast(ViewContext, self._last_context)
 
     @property
-    def _builder(self) -> type[hikari.impl.MessageActionRowBuilder]:
+    def _builder(self) -> t.Type[hikari.impl.MessageActionRowBuilder]:
         return hikari.impl.MessageActionRowBuilder
 
     @property
     def children(self) -> t.Sequence[ViewItem]:
         return t.cast(t.Sequence[ViewItem], super().children)
 
     @classmethod
@@ -283,14 +283,17 @@
         return cls(self, interaction)
 
     async def _handle_callback(self, item: ViewItem, context: ViewContext) -> None:
         """
         Handle the callback of a view item. Seperate task in case the view is stopped in the callback.
         """
         try:
+            if self._message_id == context.message.id:
+                self._message = context.message
+
             now = datetime.datetime.now()
             self._input_event.set()
             self._input_event.clear()
 
             await item._refresh_state(context)
             await item.callback(context)
```

### Comparing `hikari-miru-3.1.1/pyproject.toml` & `hikari-miru-3.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.1.1/setup.py` & `hikari-miru-3.1.2/setup.py`

 * *Files identical despite different names*

