# Comparing `tmp/django_listview_filters-0.0.1b1.dev1.tar.gz` & `tmp/django_listview_filters-0.0.1b1.dev2.tar.gz`

## Comparing `django_listview_filters-0.0.1b1.dev1.tar` & `django_listview_filters-0.0.1b1.dev2.tar`

### file list

```diff
@@ -1,26 +1,13 @@
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/.readthedocs.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/requirements.txt
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/requirements_freeze.txt
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/Makefile
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/classes.rst
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/conf.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/make.bat
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/miscellaneous.rst
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/requirements.txt
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/settings.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/custom-extensions/__init__.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/docs/custom-extensions/extensions.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/_helpers.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/_settings.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/filters.py
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/mixins.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/LICENSE
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/README.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/pyproject.toml
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.readthedocs.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.vscode/settings.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/_helpers.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/_settings.py
+-rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/filters.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/mixins.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/LICENSE
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/README.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/PKG-INFO
```

### Comparing `django_listview_filters-0.0.1b1.dev1/src/django_listview_filters/filters.py` & `django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,94 @@
-# from django.conf import settings
-
 from django.contrib import messages
+from django.contrib.admin.options import IncorrectLookupParameters
 
+# get_fields_from_path,; lookup_spawns_duplicates,
 from django.contrib.admin.utils import (
     get_model_from_relation,
-    get_fields_from_path,
     prepare_lookup_value,
     reverse_field_path,
-    lookup_spawns_duplicates,
 )
-from django.contrib.admin.options import IncorrectLookupParameters
-
 from django.core.exceptions import ImproperlyConfigured, ValidationError
-
 from django.db import models
-
-from django.db.models import Count
-
 from furl import furl
 
 from ._helpers import get_setting
-from ._settings import (
-    ALL_VAR,
-    PAGE_VAR,
-    SEARCH_VAR,
-    ERROR_VAR,
-    IGNORED_PARAMS,
+from ._settings import (  # ALL_VAR,; PAGE_VAR,; SEARCH_VAR,; ERROR_VAR,
     FILTER_PREFIX,
+    IGNORED_PARAMS,
 )
 
+# from django.db.models import Count
+
 
 class ListViewFilter:
     """
-    Base class for list view filters. Must create subclasses to provide specific functionality.
+    Base class for list view filters. Must create subclasses to provide specific
+    functionality.
     """
 
     title = None  # Human-readable title to appear in the right sidebar.
     show_all = True
     show_unused_filters = True
 
     def __init__(self, request, params, model):
         self.used_parameters = {}
-        self.show_all = get_setting("{}SHOW_ALL".format(FILTER_PREFIX), self.show_all)
+        self.show_all = get_setting(f"{FILTER_PREFIX}SHOW_ALL", self.show_all)
         self.show_unused_filters = get_setting(
-            "{}SHOW_UNUSED_FILTERS".format(FILTER_PREFIX), self.show_unused_filters
+            f"{FILTER_PREFIX}SHOW_UNUSED_FILTERS",
+            self.show_unused_filters,
         )
 
         extra_ignored_params = get_setting(
-            "{}EXTRA_IGNORED_PARAMS".format(FILTER_PREFIX), None
+            f"{FILTER_PREFIX}EXTRA_IGNORED_PARAMS",
+            None,
         )
 
         self.ignored_params = IGNORED_PARAMS
 
         if extra_ignored_params:
             self.ignored_params += extra_ignored_params
 
         if self.title is None:
             raise ImproperlyConfigured(
                 "The list view filter '{}' does not specify a 'title'.".format(
-                    self.__class__.__name__
-                )
+                    self.__class__.__name__,
+                ),
             )
 
     def has_output(self):
         """Return True if some choices would be output for this filter."""
         raise NotImplementedError(
-            "Subclasses of ListViewFilter must provide a 'has_output()' method."
+            "Subclasses of ListViewFilter must provide a 'has_output()' method.",
         )
 
     def choices(self, changelist):
         """
         Return choices ready to be output in the template.
 
         'changelist' is the ChangeList to be displayed.
         """
         raise NotImplementedError(
-            "Subclasses of ListViewFilter must provide a 'choices()' method."
+            "Subclasses of ListViewFilter must provide a 'choices()' method.",
         )
 
     def queryset(self, request, queryset):
         """Return the filtered queryset."""
         raise NotImplementedError(
-            "Subclasses of ListViewFilter must provide a 'queryset()' method."
+            "Subclasses of ListViewFilter must provide a 'queryset()' method.",
         )
 
     def expected_parameters(self):
         """
         Return the list of parameter names that are expected from the
         request's query string and that will be used by this filter.
         """
         raise NotImplementedError(
-            "Subclasses of ListViewFilter must provide an 'expected_parameters()' method."
+            "Subclasses of ListViewFilter must provide an 'expected_parameters()' \
+                method.",
         )
 
     def clear_filter_string(self, view):
         expected_params = self.expected_parameters()
         query = furl(view.request.get_full_path())
         has_param = False
         for expected_p in expected_params:
@@ -106,67 +100,74 @@
             return query.url
         else:
             return None
 
 
 class FieldListViewFilter(ListViewFilter):
     """Filter for simple choice fields. Doesn't allow for multiple choice fields."""
+
     _field_list_filters = []
     _take_priority_index = 0
     list_separator = ","
 
     def __init__(self, field, request, params, model, field_path):
         self.field = field
         self.field_path = field_path
         self.title = getattr(field, "verbose_name", field_path)
         super().__init__(request, params, model)
         for p in self.expected_parameters():
             if p in params:
                 value = params.pop(p)
                 self.used_parameters[p] = prepare_lookup_value(
                     p,
-                    value,  # , self.list_separator ### added in a future version of Django as an optional parameter
+                    value,
+                    # , self.list_separator ### added in a future version of Django
                 )
 
     def has_output(self):
         return True
 
     def queryset(self, request, queryset):
         try:
             return queryset.filter(**self.used_parameters)
         except (ValueError, ValidationError) as err:
-            raise IncorrectLookupParameters(err)
+            raise IncorrectLookupParameters(err) from err
 
     @classmethod
     def register(cls, test, list_filter_class, take_priority=False):
         if take_priority:
             cls._field_list_filters.insert(
-                cls._take_priority_index, (test, list_filter_class)
+                cls._take_priority_index,
+                (test, list_filter_class),
             )
             cls._field_list_filters.append((test, list_filter_class))
 
     @classmethod
     def create(cls, field, request, params, model, field_path):
         for test, list_filter_class in cls._field_list_filters:
             if test(field):
                 return list_filter_class(
-                    field, request, params, model, field_path=field_path
+                    field,
+                    request,
+                    params,
+                    model,
+                    field_path=field_path,
                 )
 
 
 class RelatedFieldListViewFilter(FieldListViewFilter):
     """
     For model fields that use a ForeignKey relationship.
     Not for m2m fields."""
 
     empty_value_display = "--"
 
     def __init__(self, field, request, params, model, field_path):
         other_model = get_model_from_relation(field)
-        self.lookup_kwarg = "%s__%s__exact" % (field_path, field.target_field.name)
+        self.lookup_kwarg = f"{field_path}__{field.target_field.name}__exact"
         self.lookup_kwarg_isnull = "%s__isnull" % field_path
         self.lookup_val = params.get(self.lookup_kwarg)
         self.lookup_val_isnull = params.get(self.lookup_kwarg_isnull)
         super().__init__(field, request, params, model, field_path)
         self.lookup_choices = self.field_choices(field, request)
         if hasattr(field, "verbose_name"):
             self.lookup_title = field.verbose_name
@@ -180,18 +181,15 @@
         """
         Return True if a "(None)" choice should be included, which filters
         out everything except empty relationships.
         """
         return self.field.null or (self.field.is_relation and self.field.many_to_many)
 
     def has_output(self):
-        if self.include_empty_choice:
-            extra = 1
-        else:
-            extra = 0
+        extra = 1 if self.include_empty_choice else 0
         return len(self.lookup_choices) + extra > 1
 
     def expected_parameters(self):
         return [self.lookup_kwarg, self.lookup_kwarg_isnull]
 
     # def field_admin_ordering(self, field, request, model_admin):
     #     """
@@ -227,31 +225,33 @@
 
         <changelist> is a ListView.
         """
         if self.show_all:
             yield {
                 "selected": self.lookup_val is None and not self.lookup_val_isnull,
                 "query_string": changelist.get_query_string(
-                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull]
+                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull],
                 ),
                 "display": "All",
             }
         for pk_val, val in self.lookup_choices:
             yield {
                 "selected": self.lookup_val == str(pk_val),
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg: pk_val}, [self.lookup_kwarg_isnull]
+                    {self.lookup_kwarg: pk_val},
+                    [self.lookup_kwarg_isnull],
                 ),
                 "display": val,
             }
         if self.include_empty_choice:
             yield {
                 "selected": bool(self.lookup_val_isnull),
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg_isnull: "True"}, [self.lookup_kwarg]
+                    {self.lookup_kwarg_isnull: "True"},
+                    [self.lookup_kwarg],
                 ),
                 "display": self.empty_value_display,
             }
 
 
 FieldListViewFilter.register(lambda f: f.remote_field, RelatedFieldListViewFilter)
 
@@ -282,46 +282,48 @@
                 new_list = []
                 for value in qs_dict:
                     kwargs = {field.name: value}
                     valid = model.objects.filter(**kwargs).exists()
                     if valid:
                         new_list.append((value, qs_dict[value]))
                 qs = new_list
-            except Exception as err:
+            except Exception:
                 raise
                 # messages.warning(self.request, message=err)
 
         return qs
 
     def choices(self, changelist):
         if self.show_all:
             yield {
                 "selected": self.lookup_val is None,
                 "query_string": changelist.get_query_string(
-                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull]
+                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull],
                 ),
                 "display": "All",
             }
         none_title = ""
         for lookup, title in self.get_choices(self.field):
             if lookup is None:
                 none_title = title
                 continue
             yield {
                 "selected": str(lookup) == self.lookup_val,
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg: lookup}, [self.lookup_kwarg_isnull]
+                    {self.lookup_kwarg: lookup},
+                    [self.lookup_kwarg_isnull],
                 ),
                 "display": title,
             }
         if none_title:
             yield {
                 "selected": bool(self.lookup_val_isnull),
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg_isnull: "True"}, [self.lookup_kwarg]
+                    {self.lookup_kwarg_isnull: "True"},
+                    [self.lookup_kwarg],
                 ),
                 "display": none_title,
             }
 
 
 FieldListViewFilter.register(lambda f: bool(f.choices), ChoicesFieldListViewFilter)
 
@@ -351,35 +353,37 @@
         return [self.lookup_kwarg, self.lookup_kwarg_isnull]
 
     def choices(self, changelist):
         if self.get_show_all:
             yield {
                 "selected": self.lookup_val is None and self.lookup_val_isnull is None,
                 "query_string": changelist.get_query_string(
-                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull]
+                    remove=[self.lookup_kwarg, self.lookup_kwarg_isnull],
                 ),
                 "display": "All",
             }
         include_none = False
         for val in self.lookup_choices:
             if val is None:
                 include_none = True
                 continue
             val = str(val)
             yield {
                 "selected": self.lookup_val == val,
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg: val}, [self.lookup_kwarg_isnull]
+                    {self.lookup_kwarg: val},
+                    [self.lookup_kwarg_isnull],
                 ),
                 "display": val,
             }
         if include_none:
             yield {
                 "selected": bool(self.lookup_val_isnull),
                 "query_string": changelist.get_query_string(
-                    {self.lookup_kwarg_isnull: "True"}, [self.lookup_kwarg]
+                    {self.lookup_kwarg_isnull: "True"},
+                    [self.lookup_kwarg],
                 ),
                 "display": self.empty_value_display,
             }
 
 
 FieldListViewFilter.register(lambda f: True, AllValuesFieldListFilter)
```

### Comparing `django_listview_filters-0.0.1b1.dev1/.gitignore` & `django_listview_filters-0.0.1b1.dev2/.gitignore`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
```

### Comparing `django_listview_filters-0.0.1b1.dev1/LICENSE` & `django_listview_filters-0.0.1b1.dev2/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Washington State University - Tri-Cities
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
+MIT License
+
+Copyright (c) 2022 Washington State University - Tri-Cities
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

### Comparing `django_listview_filters-0.0.1b1.dev1/README.md` & `django_listview_filters-0.0.1b1.dev2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,160 @@
 00000000: 2320 446a 616e 676f 204c 6973 7456 6965  # Django ListVie
-00000010: 7720 4669 6c74 6572 730a 0a41 6464 2063  w Filters..Add c
-00000020: 6f6e 7465 7874 2074 6f20 6c69 7374 2076  ontext to list v
-00000030: 6965 7773 2066 6f72 2073 6964 6562 6172  iews for sidebar
-00000040: 206c 696e 6b73 2061 6e64 206d 6f64 6966   links and modif
-00000050: 7969 6e67 2071 7565 7279 7365 7473 2077  ying querysets w
-00000060: 6974 6820 7468 6f73 6520 6c69 6e6b 732e  ith those links.
-00000070: 0a0a 2323 2050 7572 706f 7365 0a0a 4174  ..## Purpose..At
-00000080: 7465 6d70 7469 6e67 2074 6f20 6475 706c  tempting to dupl
-00000090: 6963 6174 6520 7468 6520 6675 6e63 7469  icate the functi
-000000a0: 6f6e 616c 6974 7920 6f66 2074 6865 205b  onality of the [
-000000b0: 604d 6f64 656c 4164 6d69 6e60 204c 6973  `ModelAdmin` Lis
-000000c0: 7420 4669 6c74 6572 5d28 6874 7470 733a  t Filter](https:
-000000d0: 2f2f 646f 6373 2e64 6a61 6e67 6f70 726f  //docs.djangopro
-000000e0: 6a65 6374 2e63 6f6d 2f65 6e2f 7374 6162  ject.com/en/stab
-000000f0: 6c65 2f72 6566 2f63 6f6e 7472 6962 2f61  le/ref/contrib/a
-00000100: 646d 696e 2f66 696c 7465 7273 2f29 2063  dmin/filters/) c
-00000110: 6170 6162 696c 6974 6965 732e 0a0a 5468  apabilities...Th
-00000120: 6973 2069 7320 6c61 7267 656c 7920 6120  is is largely a 
-00000130: 636f 7079 2d70 6173 7465 206f 6620 7468  copy-paste of th
-00000140: 6520 736f 7572 6365 2063 6f64 6520 666f  e source code fo
-00000150: 7220 7468 6174 206d 6f64 6966 6965 6420  r that modified 
-00000160: 746f 2077 6f72 6b20 6f75 7473 6964 6520  to work outside 
-00000170: 6f66 2074 6865 2061 646d 696e 2069 6e74  of the admin int
-00000180: 6572 6661 6365 2e20 466f 7220 6578 616d  erface. For exam
-00000190: 706c 652c 2072 6566 6572 656e 6365 7320  ple, references 
-000001a0: 746f 2060 6d6f 6465 6c5f 6164 6d69 6e60  to `model_admin`
-000001b0: 2068 6176 6520 6265 656e 2072 656d 6f76   have been remov
-000001c0: 6564 2e0a 0a23 2320 4164 6469 7469 6f6e  ed...## Addition
-000001d0: 616c 2046 756e 6374 696f 6e61 6c69 7479  al Functionality
-000001e0: 0a0a 4120 6665 7720 6375 7374 6f6d 697a  ..A few customiz
-000001f0: 6174 696f 6e73 2061 7265 2061 6464 6564  ations are added
-00000200: 2e0a 0a23 2323 2041 6464 2027 436c 6561  ...### Add 'Clea
-00000210: 7220 4669 6c74 6572 2720 436f 6e74 6578  r Filter' Contex
-00000220: 740a 0a41 6c6c 6f77 2066 6f72 2072 6570  t..Allow for rep
-00000230: 6c61 6369 6e67 2074 6865 2027 416c 6c27  lacing the 'All'
-00000240: 206c 696e 6b20 7769 7468 2061 2062 7574   link with a but
-00000250: 746f 6e20 7468 6174 2063 6c65 6172 7320  ton that clears 
-00000260: 7468 6520 7061 7261 6d65 7465 7220 6672  the parameter fr
-00000270: 6f6d 2074 6865 2071 7565 7279 2e0a 0a23  om the query...#
-00000280: 2323 204f 6e6c 7920 4c69 7374 204c 6f6f  ## Only List Loo
-00000290: 6b75 7073 2057 6974 6820 4d61 7463 6865  kups With Matche
-000002a0: 730a 0a41 6c6c 6f77 2066 6f72 2066 696c  s..Allow for fil
-000002b0: 7465 7269 6e67 206f 6620 6c69 7374 2066  tering of list f
-000002c0: 6f72 2073 6964 6562 6172 2074 6f20 6f6e  or sidebar to on
-000002d0: 6c79 2074 686f 7365 2077 6974 6820 6d61  ly those with ma
-000002e0: 7463 6865 732e 2054 6861 7420 7761 7920  tches. That way 
-000002f0: 656d 7074 7920 6c69 6e6b 7320 6172 656e  empty links aren
-00000300: 2774 2074 616b 696e 6720 7570 2076 616c  't taking up val
-00000310: 7561 626c 6520 7370 6163 652e 0a0a 2323  uable space...##
-00000320: 2320 4164 6420 436f 756e 7420 746f 2043  # Add Count to C
-00000330: 6f6e 7465 7874 0a0a 4164 6420 7468 6520  ontext..Add the 
-00000340: 636f 756e 7420 6f66 206e 756d 6265 7220  count of number 
-00000350: 6f66 206f 626a 6563 7473 2074 6f20 6561  of objects to ea
-00000360: 6368 206c 696e 6b20 7468 6174 2063 616e  ch link that can
-00000370: 2062 6520 7368 6f77 6e20 696e 2074 6865   be shown in the
-00000380: 2074 656d 706c 6174 652e 0a0a 2323 2043   template...## C
-00000390: 6f6e 6669 6775 7261 7469 6f6e 0a0a 2323  onfiguration..##
-000003a0: 2320 4d6f 6465 6c0a 0a60 6060 7079 7468  # Model..```pyth
-000003b0: 6f6e 0a66 726f 6d20 646a 616e 676f 2e64  on.from django.d
-000003c0: 6220 696d 706f 7274 206d 6f64 656c 730a  b import models.
-000003d0: 0a63 6c61 7373 2041 7574 686f 7228 6d6f  .class Author(mo
-000003e0: 6465 6c73 2e4d 6f64 656c 293a 0a20 2020  dels.Model):.   
-000003f0: 206e 616d 6520 3d20 6d6f 6465 6c73 2e43   name = models.C
-00000400: 6861 7246 6965 6c64 2822 4175 7468 6f72  harField("Author
-00000410: 2773 204e 616d 6522 2c20 6d61 785f 6c65  's Name", max_le
-00000420: 6e67 7468 3d31 3030 290a 2020 2020 6269  ngth=100).    bi
-00000430: 7274 6864 6179 203d 206d 6f64 656c 732e  rthday = models.
-00000440: 4461 7465 4669 656c 6428 2241 7574 686f  DateField("Autho
-00000450: 7227 7320 4269 7274 6864 6179 222c 2062  r's Birthday", b
-00000460: 6c61 6e6b 3d54 7275 6529 0a0a 636c 6173  lank=True)..clas
-00000470: 7320 426f 6f6b 286d 6f64 656c 732e 4d6f  s Book(models.Mo
-00000480: 6465 6c29 3a0a 2020 2020 7469 746c 6520  del):.    title 
-00000490: 3d20 6d6f 6465 6c73 2e43 6861 7246 6965  = models.CharFie
-000004a0: 6c64 2822 426f 6f6b 2054 6974 6c65 222c  ld("Book Title",
-000004b0: 206d 6178 5f6c 656e 6774 683d 3135 3029   max_length=150)
-000004c0: 0a20 2020 2061 7574 686f 7220 3d20 6d6f  .    author = mo
-000004d0: 6465 6c73 2e46 6f72 6569 676e 4b65 7928  dels.ForeignKey(
-000004e0: 4175 7468 6f72 2c20 6f6e 5f64 656c 6574  Author, on_delet
-000004f0: 653d 6d6f 6465 6c73 2e50 524f 5445 4354  e=models.PROTECT
-00000500: 290a 6060 600a 0a23 2323 2043 6c61 7373  ).```..### Class
-00000510: 2d62 6173 6564 2056 6965 770a 0a60 6060  -based View..```
-00000520: 7079 7468 6f6e 0a66 726f 6d20 646a 616e  python.from djan
-00000530: 676f 2e76 6965 772e 6765 6e65 7269 6320  go.view.generic 
-00000540: 696d 706f 7274 204c 6973 7456 6965 770a  import ListView.
-00000550: 0a66 726f 6d20 646a 616e 676f 2d6c 6973  .from django-lis
-00000560: 7476 6965 772d 6669 6c74 6572 7320 696d  tview-filters im
-00000570: 706f 7274 2052 656c 6174 6564 4669 656c  port RelatedFiel
-00000580: 644c 6973 7456 6965 7746 696c 7465 720a  dListViewFilter.
-00000590: 0a63 6c61 7373 2041 7574 686f 724c 6973  .class AuthorLis
-000005a0: 7456 6965 7728 4c69 7374 5669 6577 293a  tView(ListView):
-000005b0: 0a20 2020 2063 6f6e 7465 7874 5f6f 626a  .    context_obj
-000005c0: 6563 745f 6e61 6d65 203d 2022 6175 7468  ect_name = "auth
-000005d0: 6f72 220a 2020 2020 7175 6572 7973 6574  or".    queryset
-000005e0: 203d 2041 7574 686f 722e 6f62 6a65 6374   = Author.object
-000005f0: 732e 6f72 6465 725f 6279 2822 6e61 6d65  s.order_by("name
-00000600: 2229 0a0a 636c 6173 7320 426f 6f6b 4c69  ")..class BookLi
-00000610: 7374 5669 6577 284c 6973 7456 6965 7729  stView(ListView)
-00000620: 3a0a 2020 2020 636f 6e74 6578 745f 6f62  :.    context_ob
-00000630: 6a65 6374 5f6e 616d 6520 3d20 2262 6f6f  ject_name = "boo
-00000640: 6b22 0a20 2020 2071 7565 7279 7365 7420  k".    queryset 
-00000650: 3d20 4175 7468 6f72 2e6f 626a 6563 7473  = Author.objects
-00000660: 2e6f 7264 6572 5f62 7928 2274 6974 6c65  .order_by("title
-00000670: 2229 0a0a 2020 2020 6c69 7374 5f66 696c  ")..    list_fil
-00000680: 7465 7220 3d20 5b0a 2020 2020 2020 2020  ter = [.        
-00000690: 2827 6175 7468 6f72 272c 2052 656c 6174  ('author', Relat
-000006a0: 6564 4669 656c 644c 6973 7456 6965 7746  edFieldListViewF
-000006b0: 696c 7465 7229 0a20 2020 205d 0a60 6060  ilter).    ].```
-000006c0: 0a0a 2323 2320 5465 6d70 6c61 7465 0a0a  ..### Template..
-000006d0: 6060 6070 7974 686f 6e0a 7b25 2066 6f72  ```python.{% for
-000006e0: 2066 696c 7465 725f 6e61 6d65 2c20 6669   filter_name, fi
-000006f0: 6c74 6572 5f6f 626a 6563 7473 2c20 636c  lter_objects, cl
-00000700: 6561 725f 6672 6167 6d65 6e74 2069 6e20  ear_fragment in 
-00000710: 6669 6c74 6572 5f6c 6973 7420 257d 0a20  filter_list %}. 
-00000720: 2020 203c 6469 763e 0a20 2020 2020 2020     <div>.       
-00000730: 207b 7b20 6669 6c74 6572 5f6e 616d 657c   {{ filter_name|
-00000740: 7469 746c 6520 7d7d 0a20 2020 2020 2020  title }}.       
-00000750: 203c 6120 6872 6566 3d22 7b7b 2063 6c65   <a href="{{ cle
-00000760: 6172 5f66 7261 676d 656e 7420 7d7d 223e  ar_fragment }}">
-00000770: 636c 6561 7220 6669 6c74 6572 3c2f 613e  clear filter</a>
-00000780: 0a20 2020 203c 2f64 6976 3e0a 2020 2020  .    </div>.    
-00000790: 3c75 6c3e 0a20 2020 2020 2020 207b 2520  <ul>.        {% 
-000007a0: 7769 7468 2066 696c 7465 725f 6f62 6a65  with filter_obje
-000007b0: 6374 737c 6469 6374 736f 7274 3a22 6469  cts|dictsort:"di
-000007c0: 7370 6c61 7922 2061 7320 6469 7370 6c61  splay" as displa
-000007d0: 795f 6c69 7374 2025 7d0a 2020 2020 2020  y_list %}.      
-000007e0: 2020 2020 2020 7b25 2066 6f72 2069 7465        {% for ite
-000007f0: 6d20 696e 2064 6973 706c 6179 5f6c 6973  m in display_lis
-00000800: 7420 257d 0a20 2020 2020 2020 2020 2020  t %}.           
-00000810: 2020 2020 203c 6469 763e 0a20 2020 2020       <div>.     
-00000820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000830: 6120 6872 6566 3d22 7b7b 2069 7465 6d2e  a href="{{ item.
-00000840: 7175 6572 795f 7374 7269 6e67 207d 7d22  query_string }}"
-00000850: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000860: 2020 2020 2020 2020 2020 7b7b 2069 7465            {{ ite
-00000870: 6d2e 6469 7370 6c61 7920 7d7d 0a20 2020  m.display }}.   
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 203c 2f61 3e0a 2020 2020 2020 2020 2020   </a>.          
-000008a0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000008b0: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
-000008c0: 6f72 2025 7d0a 2020 2020 2020 2020 7b25  or %}.        {%
-000008d0: 2065 6e64 7769 7468 2025 7d0a 2020 2020   endwith %}.    
-000008e0: 3c2f 756c 3e0a 3c2f 6469 763e 0a60 6060  </ul>.</div>.```
-000008f0: 0a                                       .
+00000010: 7720 4669 6c74 6572 730d 0a0d 0a5b 215b  w Filters....[![
+00000020: 446f 6375 6d65 6e74 6174 696f 6e20 5374  Documentation St
+00000030: 6174 7573 5d28 6874 7470 733a 2f2f 7265  atus](https://re
+00000040: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000050: 6f6a 6563 7473 2f64 6a61 6e67 6f2d 6c69  ojects/django-li
+00000060: 7374 7669 6577 2d66 696c 7465 7273 2f62  stview-filters/b
+00000070: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00000080: 7465 7374 295d 2868 7474 7073 3a2f 2f64  test)](https://d
+00000090: 6a61 6e67 6f2d 6c69 7374 7669 6577 2d66  jango-listview-f
+000000a0: 696c 7465 7273 2e72 6561 6474 6865 646f  ilters.readthedo
+000000b0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+000000c0: 3f62 6164 6765 3d6c 6174 6573 7429 0d0a  ?badge=latest)..
+000000d0: 0d0a 4164 6420 636f 6e74 6578 7420 746f  ..Add context to
+000000e0: 206c 6973 7420 7669 6577 7320 666f 7220   list views for 
+000000f0: 7369 6465 6261 7220 6c69 6e6b 7320 616e  sidebar links an
+00000100: 6420 6d6f 6469 6679 696e 6720 7175 6572  d modifying quer
+00000110: 7973 6574 7320 7769 7468 2074 686f 7365  ysets with those
+00000120: 206c 696e 6b73 2e0d 0a0d 0a23 2320 5075   links.....## Pu
+00000130: 7270 6f73 650d 0a0d 0a41 7474 656d 7074  rpose....Attempt
+00000140: 696e 6720 746f 2064 7570 6c69 6361 7465  ing to duplicate
+00000150: 2074 6865 2066 756e 6374 696f 6e61 6c69   the functionali
+00000160: 7479 206f 6620 7468 6520 5b60 4d6f 6465  ty of the [`Mode
+00000170: 6c41 646d 696e 6020 4c69 7374 2046 696c  lAdmin` List Fil
+00000180: 7465 725d 2868 7474 7073 3a2f 2f64 6f63  ter](https://doc
+00000190: 732e 646a 616e 676f 7072 6f6a 6563 742e  s.djangoproject.
+000001a0: 636f 6d2f 656e 2f73 7461 626c 652f 7265  com/en/stable/re
+000001b0: 662f 636f 6e74 7269 622f 6164 6d69 6e2f  f/contrib/admin/
+000001c0: 6669 6c74 6572 732f 2920 6361 7061 6269  filters/) capabi
+000001d0: 6c69 7469 6573 2e0d 0a0d 0a54 6869 7320  lities.....This 
+000001e0: 6973 206c 6172 6765 6c79 2061 2063 6f70  is largely a cop
+000001f0: 792d 7061 7374 6520 6f66 2074 6865 2073  y-paste of the s
+00000200: 6f75 7263 6520 636f 6465 2066 6f72 2074  ource code for t
+00000210: 6861 7420 6d6f 6469 6669 6564 2074 6f20  hat modified to 
+00000220: 776f 726b 206f 7574 7369 6465 206f 6620  work outside of 
+00000230: 7468 6520 6164 6d69 6e20 696e 7465 7266  the admin interf
+00000240: 6163 652e 2046 6f72 2065 7861 6d70 6c65  ace. For example
+00000250: 2c20 7265 6665 7265 6e63 6573 2074 6f20  , references to 
+00000260: 606d 6f64 656c 5f61 646d 696e 6020 6861  `model_admin` ha
+00000270: 7665 2062 6565 6e20 7265 6d6f 7665 642e  ve been removed.
+00000280: 0d0a 0d0a 2323 2041 6464 6974 696f 6e61  ....## Additiona
+00000290: 6c20 4675 6e63 7469 6f6e 616c 6974 790d  l Functionality.
+000002a0: 0a0d 0a41 2066 6577 2063 7573 746f 6d69  ...A few customi
+000002b0: 7a61 7469 6f6e 7320 6172 6520 6164 6465  zations are adde
+000002c0: 642e 0d0a 0d0a 2323 2320 4164 6420 2743  d.....### Add 'C
+000002d0: 6c65 6172 2046 696c 7465 7227 2043 6f6e  lear Filter' Con
+000002e0: 7465 7874 0d0a 0d0a 416c 6c6f 7720 666f  text....Allow fo
+000002f0: 7220 7265 706c 6163 696e 6720 7468 6520  r replacing the 
+00000300: 2741 6c6c 2720 6c69 6e6b 2077 6974 6820  'All' link with 
+00000310: 6120 6275 7474 6f6e 2074 6861 7420 636c  a button that cl
+00000320: 6561 7273 2074 6865 2070 6172 616d 6574  ears the paramet
+00000330: 6572 2066 726f 6d20 7468 6520 7175 6572  er from the quer
+00000340: 792e 0d0a 0d0a 2323 2320 4f6e 6c79 204c  y.....### Only L
+00000350: 6973 7420 4c6f 6f6b 7570 7320 5769 7468  ist Lookups With
+00000360: 204d 6174 6368 6573 0d0a 0d0a 416c 6c6f   Matches....Allo
+00000370: 7720 666f 7220 6669 6c74 6572 696e 6720  w for filtering 
+00000380: 6f66 206c 6973 7420 666f 7220 7369 6465  of list for side
+00000390: 6261 7220 746f 206f 6e6c 7920 7468 6f73  bar to only thos
+000003a0: 6520 7769 7468 206d 6174 6368 6573 2e20  e with matches. 
+000003b0: 5468 6174 2077 6179 2065 6d70 7479 206c  That way empty l
+000003c0: 696e 6b73 2061 7265 6e27 7420 7461 6b69  inks aren't taki
+000003d0: 6e67 2075 7020 7661 6c75 6162 6c65 2073  ng up valuable s
+000003e0: 7061 6365 2e0d 0a0d 0a23 2323 2041 6464  pace.....### Add
+000003f0: 2043 6f75 6e74 2074 6f20 436f 6e74 6578   Count to Contex
+00000400: 740d 0a0d 0a41 6464 2074 6865 2063 6f75  t....Add the cou
+00000410: 6e74 206f 6620 6e75 6d62 6572 206f 6620  nt of number of 
+00000420: 6f62 6a65 6374 7320 746f 2065 6163 6820  objects to each 
+00000430: 6c69 6e6b 2074 6861 7420 6361 6e20 6265  link that can be
+00000440: 2073 686f 776e 2069 6e20 7468 6520 7465   shown in the te
+00000450: 6d70 6c61 7465 2e0d 0a0d 0a23 2320 436f  mplate.....## Co
+00000460: 6e66 6967 7572 6174 696f 6e0d 0a0d 0a23  nfiguration....#
+00000470: 2323 204d 6f64 656c 0d0a 0d0a 6060 6070  ## Model....```p
+00000480: 7974 686f 6e0d 0a66 726f 6d20 646a 616e  ython..from djan
+00000490: 676f 2e64 6220 696d 706f 7274 206d 6f64  go.db import mod
+000004a0: 656c 730d 0a0d 0a63 6c61 7373 2041 7574  els....class Aut
+000004b0: 686f 7228 6d6f 6465 6c73 2e4d 6f64 656c  hor(models.Model
+000004c0: 293a 0d0a 2020 2020 6e61 6d65 203d 206d  ):..    name = m
+000004d0: 6f64 656c 732e 4368 6172 4669 656c 6428  odels.CharField(
+000004e0: 2241 7574 686f 7227 7320 4e61 6d65 222c  "Author's Name",
+000004f0: 206d 6178 5f6c 656e 6774 683d 3130 3029   max_length=100)
+00000500: 0d0a 2020 2020 6269 7274 6864 6179 203d  ..    birthday =
+00000510: 206d 6f64 656c 732e 4461 7465 4669 656c   models.DateFiel
+00000520: 6428 2241 7574 686f 7227 7320 4269 7274  d("Author's Birt
+00000530: 6864 6179 222c 2062 6c61 6e6b 3d54 7275  hday", blank=Tru
+00000540: 6529 0d0a 0d0a 636c 6173 7320 426f 6f6b  e)....class Book
+00000550: 286d 6f64 656c 732e 4d6f 6465 6c29 3a0d  (models.Model):.
+00000560: 0a20 2020 2074 6974 6c65 203d 206d 6f64  .    title = mod
+00000570: 656c 732e 4368 6172 4669 656c 6428 2242  els.CharField("B
+00000580: 6f6f 6b20 5469 746c 6522 2c20 6d61 785f  ook Title", max_
+00000590: 6c65 6e67 7468 3d31 3530 290d 0a20 2020  length=150)..   
+000005a0: 2061 7574 686f 7220 3d20 6d6f 6465 6c73   author = models
+000005b0: 2e46 6f72 6569 676e 4b65 7928 4175 7468  .ForeignKey(Auth
+000005c0: 6f72 2c20 6f6e 5f64 656c 6574 653d 6d6f  or, on_delete=mo
+000005d0: 6465 6c73 2e50 524f 5445 4354 290d 0a60  dels.PROTECT)..`
+000005e0: 6060 0d0a 0d0a 2323 2320 436c 6173 732d  ``....### Class-
+000005f0: 6261 7365 6420 5669 6577 0d0a 0d0a 6060  based View....``
+00000600: 6070 7974 686f 6e0d 0a66 726f 6d20 646a  `python..from dj
+00000610: 616e 676f 2e76 6965 772e 6765 6e65 7269  ango.view.generi
+00000620: 6320 696d 706f 7274 204c 6973 7456 6965  c import ListVie
+00000630: 770d 0a0d 0a66 726f 6d20 646a 616e 676f  w....from django
+00000640: 2d6c 6973 7476 6965 772d 6669 6c74 6572  -listview-filter
+00000650: 7320 696d 706f 7274 2052 656c 6174 6564  s import Related
+00000660: 4669 656c 644c 6973 7456 6965 7746 696c  FieldListViewFil
+00000670: 7465 720d 0a0d 0a63 6c61 7373 2041 7574  ter....class Aut
+00000680: 686f 724c 6973 7456 6965 7728 4c69 7374  horListView(List
+00000690: 5669 6577 293a 0d0a 2020 2020 636f 6e74  View):..    cont
+000006a0: 6578 745f 6f62 6a65 6374 5f6e 616d 6520  ext_object_name 
+000006b0: 3d20 2261 7574 686f 7222 0d0a 2020 2020  = "author"..    
+000006c0: 7175 6572 7973 6574 203d 2041 7574 686f  queryset = Autho
+000006d0: 722e 6f62 6a65 6374 732e 6f72 6465 725f  r.objects.order_
+000006e0: 6279 2822 6e61 6d65 2229 0d0a 0d0a 636c  by("name")....cl
+000006f0: 6173 7320 426f 6f6b 4c69 7374 5669 6577  ass BookListView
+00000700: 284c 6973 7456 6965 7729 3a0d 0a20 2020  (ListView):..   
+00000710: 2063 6f6e 7465 7874 5f6f 626a 6563 745f   context_object_
+00000720: 6e61 6d65 203d 2022 626f 6f6b 220d 0a20  name = "book".. 
+00000730: 2020 2071 7565 7279 7365 7420 3d20 4175     queryset = Au
+00000740: 7468 6f72 2e6f 626a 6563 7473 2e6f 7264  thor.objects.ord
+00000750: 6572 5f62 7928 2274 6974 6c65 2229 0d0a  er_by("title")..
+00000760: 0d0a 2020 2020 6c69 7374 5f66 696c 7465  ..    list_filte
+00000770: 7220 3d20 5b0d 0a20 2020 2020 2020 2028  r = [..        (
+00000780: 2761 7574 686f 7227 2c20 5265 6c61 7465  'author', Relate
+00000790: 6446 6965 6c64 4c69 7374 5669 6577 4669  dFieldListViewFi
+000007a0: 6c74 6572 290d 0a20 2020 205d 0d0a 6060  lter)..    ]..``
+000007b0: 600d 0a0d 0a23 2323 2054 656d 706c 6174  `....### Templat
+000007c0: 650d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  e....```python..
+000007d0: 7b25 2066 6f72 2066 696c 7465 725f 6e61  {% for filter_na
+000007e0: 6d65 2c20 6669 6c74 6572 5f6f 626a 6563  me, filter_objec
+000007f0: 7473 2c20 636c 6561 725f 6672 6167 6d65  ts, clear_fragme
+00000800: 6e74 2069 6e20 6669 6c74 6572 5f6c 6973  nt in filter_lis
+00000810: 7420 257d 0d0a 2020 2020 3c64 6976 3e0d  t %}..    <div>.
+00000820: 0a20 2020 2020 2020 207b 7b20 6669 6c74  .        {{ filt
+00000830: 6572 5f6e 616d 657c 7469 746c 6520 7d7d  er_name|title }}
+00000840: 0d0a 2020 2020 2020 2020 3c61 2068 7265  ..        <a hre
+00000850: 663d 227b 7b20 636c 6561 725f 6672 6167  f="{{ clear_frag
+00000860: 6d65 6e74 207d 7d22 3e63 6c65 6172 2066  ment }}">clear f
+00000870: 696c 7465 723c 2f61 3e0d 0a20 2020 203c  ilter</a>..    <
+00000880: 2f64 6976 3e0d 0a20 2020 203c 756c 3e0d  /div>..    <ul>.
+00000890: 0a20 2020 2020 2020 207b 2520 7769 7468  .        {% with
+000008a0: 2066 696c 7465 725f 6f62 6a65 6374 737c   filter_objects|
+000008b0: 6469 6374 736f 7274 3a22 6469 7370 6c61  dictsort:"displa
+000008c0: 7922 2061 7320 6469 7370 6c61 795f 6c69  y" as display_li
+000008d0: 7374 2025 7d0d 0a20 2020 2020 2020 2020  st %}..         
+000008e0: 2020 207b 2520 666f 7220 6974 656d 2069     {% for item i
+000008f0: 6e20 6469 7370 6c61 795f 6c69 7374 2025  n display_list %
+00000900: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00000910: 2020 203c 6469 763e 0d0a 2020 2020 2020     <div>..      
+00000920: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
+00000930: 2068 7265 663d 227b 7b20 6974 656d 2e71   href="{{ item.q
+00000940: 7565 7279 5f73 7472 696e 6720 7d7d 223e  uery_string }}">
+00000950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000960: 2020 2020 2020 2020 2020 7b7b 2069 7465            {{ ite
+00000970: 6d2e 6469 7370 6c61 7920 7d7d 0d0a 2020  m.display }}..  
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 3c2f 613e 0d0a 2020 2020 2020 2020    </a>..        
+000009a0: 2020 2020 2020 2020 3c2f 6469 763e 0d0a          </div>..
+000009b0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000009c0: 6e64 666f 7220 257d 0d0a 2020 2020 2020  ndfor %}..      
+000009d0: 2020 7b25 2065 6e64 7769 7468 2025 7d0d    {% endwith %}.
+000009e0: 0a20 2020 203c 2f75 6c3e 0d0a 3c2f 6469  .    </ul>..</di
+000009f0: 763e 0d0a 6060 600d 0a                   v>..```..
```

### Comparing `django_listview_filters-0.0.1b1.dev1/pyproject.toml` & `django_listview_filters-0.0.1b1.dev2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "django_listview_filters"
-dynamic = ["version"]
-# version = "0.0.2"
-authors = [
-    { name="Karl Wooster", email="karl.wooster@wsu.edu" },
-]
-description = "Add context to list views for sidebar links and modifying querysets with those links."
-readme = "README.md"
-license.file = "LICENSE"
-dependencies = [
-    'django',
-    'furl',
-]
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/wsutc/django-listview-filters"
-"Bug Tracker" = "https://github.com/wsutc/django-listview-filters/issues"
-
-# [tool]
-# [tool.hatch]
-[tool.hatch.version]
-path="src/django_listview_filters/__init__.py"
-
-# [tool.hatch.build.targets.sdist]
-# exclude = [
-#     "/.github",
-#     "/docs",
-# ]
-
-# [tool.hatch.guild.targets.wheel]
-# packages = ["src/django-listview-filters"]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "django_listview_filters"
+dynamic = ["version"]
+# version = "0.0.2"
+authors = [{ name = "Karl Wooster", email = "karl.wooster@wsu.edu" }]
+description = "Add context to list views for sidebar links and modifying querysets with those links."
+readme = "README.md"
+license.file = "LICENSE"
+dependencies = ['django', 'furl']
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/wsutc/django-listview-filters"
+"Bug Tracker" = "https://github.com/wsutc/django-listview-filters/issues"
+
+# [tool]
+# [tool.hatch]
+[tool.hatch.version]
+path = "src/django_listview_filters/__init__.py"
+
+[tool.hatch.build.targets.sdist]
+exclude = ["/.github", "/docs"]
+
+[tool.hatch.guild.targets.wheel]
+packages = ["src/django-listview-filters"]
+
+# [tool.hatch.publish.index.repos.private]
+# url = "https://pypi.org/project/django-listview-filters/"
```

### Comparing `django_listview_filters-0.0.1b1.dev1/PKG-INFO` & `django_listview_filters-0.0.1b1.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_listview_filters
-Version: 0.0.1b1.dev1
+Version: 0.0.1b1.dev2
 Summary: Add context to list views for sidebar links and modifying querysets with those links.
 Project-URL: Homepage, https://github.com/wsutc/django-listview-filters
 Project-URL: Bug Tracker, https://github.com/wsutc/django-listview-filters/issues
 Author-email: Karl Wooster <karl.wooster@wsu.edu>
 License: MIT License
         
         Copyright (c) 2022 Washington State University - Tri-Cities
@@ -33,14 +33,16 @@
 Requires-Python: >=3.10
 Requires-Dist: django
 Requires-Dist: furl
 Description-Content-Type: text/markdown
 
 # Django ListView Filters
 
+[![Documentation Status](https://readthedocs.org/projects/django-listview-filters/badge/?version=latest)](https://django-listview-filters.readthedocs.io/en/latest/?badge=latest)
+
 Add context to list views for sidebar links and modifying querysets with those links.
 
 ## Purpose
 
 Attempting to duplicate the functionality of the [`ModelAdmin` List Filter](https://docs.djangoproject.com/en/stable/ref/contrib/admin/filters/) capabilities.
 
 This is largely a copy-paste of the source code for that modified to work outside of the admin interface. For example, references to `model_admin` have been removed.
```

