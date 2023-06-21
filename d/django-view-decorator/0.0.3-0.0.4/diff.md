# Comparing `tmp/django_view_decorator-0.0.3.tar.gz` & `tmp/django_view_decorator-0.0.4.tar.gz`

## Comparing `django_view_decorator-0.0.3.tar` & `django_view_decorator-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/__about__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/apps.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/conf.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/decorators.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/urls.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/urls_utils.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/management/commands/list_views.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/README.md
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/__about__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/app_config.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/apps.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/conf.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/decorators.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/urls.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/urls_utils.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/django_view_decorator/management/commands/list_views.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/README.md
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 django_view_decorator-0.0.4/PKG-INFO
```

### Comparing `django_view_decorator-0.0.3/django_view_decorator/apps.py` & `django_view_decorator-0.0.4/django_view_decorator/apps.py`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.3/django_view_decorator/decorators.py` & `django_view_decorator-0.0.4/django_view_decorator/decorators.py`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.3/django_view_decorator/urls_utils.py` & `django_view_decorator-0.0.4/django_view_decorator/urls_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from django.urls import include
 from django.urls import URLPattern
 from django.urls import URLResolver
 
 
 def include_view_urls(
     *,
-    modules: list[str] | None = None,
+    extra_modules: list[str] | None = None,
 ) -> tuple[Sequence[URLResolver | URLPattern], str | None, str | None]:
     """
     Include the view urls from the registry discovered by django_view_decorator, and
     optionally from the given modules.
-    :param modules: A list of modules to import before including the view urls.
+    :param extra_modules: A list of modules to import before including the view urls.
     :return: A tuple of (urlpatterns, app_name, namespace) (result from calling
         include())
     """
-    if modules:
-        for module in modules:
+    if extra_modules:
+        for module in extra_modules:
             import_module(f"{module}")
 
     return include("django_view_decorator.urls")
```

### Comparing `django_view_decorator-0.0.3/django_view_decorator/management/commands/list_views.py` & `django_view_decorator-0.0.4/django_view_decorator/management/commands/list_views.py`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.3/LICENSE.txt` & `django_view_decorator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.3/README.md` & `django_view_decorator-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Django View Decorator
 
 [![Tests](https://github.com/valberg/django-view-decorator/actions/workflows/test.yml/badge.svg)](https://github.com/valberg/django-view-decorator/actions/workflows/test.yml)
 [![Documentation](https://readthedocs.org/projects/django-view-decorator/badge/?version=latest)](https://django-view-decorator.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/valberg/django-view-decorator/main.svg)](https://results.pre-commit.ci/latest/github/valberg/django-view-decorator/main)
 [![PyPI - Version](https://img.shields.io/pypi/v/django-view-decorator.svg)](https://pypi.org/project/django-view-decorator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-view-decorator.svg)](https://pypi.org/project/django-view-decorator)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/valberg/django-view-decorator/main.svg)](https://results.pre-commit.ci/latest/github/valberg/django-view-decorator/main)
 
 -----
 
 **django-view-decorator** is decorator aimed at bringing locality of behaviour to the connection between a URL and a view in Django.
```

### Comparing `django_view_decorator-0.0.3/pyproject.toml` & `django_view_decorator-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Víðir Valberg Guðmundsson", email = "valberg@orn.li" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 3 - Alpha",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
```

### Comparing `django_view_decorator-0.0.3/PKG-INFO` & `django_view_decorator-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-view-decorator
-Version: 0.0.3
+Version: 0.0.4
 Summary: django-view-decorator is decorator aimed at bringing locality of behaviour to the connection between a URL and a view in Django.
 Project-URL: Documentation, https://django-view-decorator.readthedocs.io/
 Project-URL: Issues, https://github.com/valberg/django-view-decorator/issues
 Project-URL: Source, https://github.com/valberg/django-view-decorator
 Author-email: Víðir Valberg Guðmundsson <valberg@orn.li>
 License-Expression: MIT
 License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: django>=3.2
 Description-Content-Type: text/markdown
 
 # Django View Decorator
 
 [![Tests](https://github.com/valberg/django-view-decorator/actions/workflows/test.yml/badge.svg)](https://github.com/valberg/django-view-decorator/actions/workflows/test.yml)
 [![Documentation](https://readthedocs.org/projects/django-view-decorator/badge/?version=latest)](https://django-view-decorator.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/valberg/django-view-decorator/main.svg)](https://results.pre-commit.ci/latest/github/valberg/django-view-decorator/main)
 [![PyPI - Version](https://img.shields.io/pypi/v/django-view-decorator.svg)](https://pypi.org/project/django-view-decorator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-view-decorator.svg)](https://pypi.org/project/django-view-decorator)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/valberg/django-view-decorator/main.svg)](https://results.pre-commit.ci/latest/github/valberg/django-view-decorator/main)
 
 -----
 
 **django-view-decorator** is decorator aimed at bringing locality of behaviour to the connection between a URL and a view in Django.
```

