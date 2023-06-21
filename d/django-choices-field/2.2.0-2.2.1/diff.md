# Comparing `tmp/django_choices_field-2.2.0.tar.gz` & `tmp/django_choices_field-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_choices_field-2.2.0.tar", max compression
+gzip compressed data, was "django_choices_field-2.2.1.tar", max compression
```

## Comparing `django_choices_field-2.2.0.tar` & `django_choices_field-2.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/LICENSE
--rw-r--r--   0        0        0     2822 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/README.md
--rw-r--r--   0        0        0      188 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/__init__.py
--rw-r--r--   0        0        0     5249 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/fields.py
--rw-r--r--   0        0        0     7193 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/fields.pyi
--rw-r--r--   0        0        0      625 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/types.py
--rw-r--r--   0        0        0     3264 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 django_choices_field-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2822 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/README.md
+-rw-r--r--   0        0        0      188 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/__init__.py
+-rw-r--r--   0        0        0     5913 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/fields.py
+-rw-r--r--   0        0        0     7193 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/fields.pyi
+-rw-r--r--   0        0        0      625 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/django_choices_field/types.py
+-rw-r--r--   0        0        0     3264 2023-06-21 18:54:24.579867 django_choices_field-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 django_choices_field-2.2.1/PKG-INFO
```

### Comparing `django_choices_field-2.2.0/LICENSE` & `django_choices_field-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.0/README.md` & `django_choices_field-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.0/django_choices_field/fields.py` & `django_choices_field-2.2.1/django_choices_field/fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 import functools
 import itertools
-from typing import ClassVar, Dict, Optional, Type
+from typing import Callable, ClassVar, Dict, Optional, Sequence, Type, cast
 
 from django.core.exceptions import ValidationError
 from django.db import models
 
 from .types import IntegerChoicesFlag
 
 
+def _get_flag_description(descs: Sequence[str]) -> str:
+    return "|".join(str(desc) for desc in descs)
+
+
+try:
+    from django.utils.functional import Promise, lazy
+except ImportError:  # pragma: nocover
+    Promise = None
+    _get_flag_description_lazy = None
+else:
+    _get_flag_description_lazy = cast(
+        Callable[[Sequence[str]], str],
+        lazy(_get_flag_description, str),
+    )
+
+
 class TextChoicesField(models.CharField):
     description: ClassVar[str] = "TextChoices"
     default_error_messages: ClassVar[Dict[str, str]] = {
         "invalid": "“%(value)s” must be a subclass of %(enum)s.",
     }
 
     def __init__(
@@ -118,20 +134,24 @@
     ):
         self.choices_enum = choices_enum
 
         default_choices = choices_enum.choices
         kwargs["choices"] = default_choices[:]
         for i in range(1, len(default_choices)):
             for combination in itertools.combinations(default_choices, i + 1):
-                kwargs["choices"].append(
-                    (
-                        functools.reduce(lambda a, b: a | b[0], combination, 0),
-                        "|".join(c[1] for c in combination),
-                    ),
-                )
+                value = functools.reduce(lambda a, b: a | b[0], combination, 0)
+
+                descs = [c[1] for c in combination]
+                if Promise is not None and any(isinstance(desc, Promise) for desc in descs):
+                    assert _get_flag_description_lazy is not None
+                    desc = _get_flag_description_lazy(descs)
+                else:
+                    desc = _get_flag_description(descs)
+
+                kwargs["choices"].append((value, desc))
 
         super().__init__(verbose_name=verbose_name, name=name, **kwargs)
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         kwargs["choices_enum"] = self.choices_enum
         return name, path, args, kwargs
```

### Comparing `django_choices_field-2.2.0/django_choices_field/fields.pyi` & `django_choices_field-2.2.1/django_choices_field/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.0/django_choices_field/types.py` & `django_choices_field-2.2.1/django_choices_field/types.py`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.2.0/pyproject.toml` & `django_choices_field-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-choices-field"
-version = "2.2.0"
+version = "2.2.1"
 description = "Django field that set/get django's new TextChoices/IntegerChoices enum."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bellini666/django-choices-field"
 repository = "https://github.com/bellini666/django-choices-field"
 documentation = "https://django-choices-field.readthedocs.io"
```

### Comparing `django_choices_field-2.2.0/PKG-INFO` & `django_choices_field-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-choices-field
-Version: 2.2.0
+Version: 2.2.1
 Summary: Django field that set/get django's new TextChoices/IntegerChoices enum.
 Home-page: https://github.com/bellini666/django-choices-field
 License: MIT
 Keywords: django,enum
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

