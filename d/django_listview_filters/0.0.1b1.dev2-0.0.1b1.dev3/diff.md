# Comparing `tmp/django_listview_filters-0.0.1b1.dev2.tar.gz` & `tmp/django_listview_filters-0.0.1b1.dev3.tar.gz`

## Comparing `django_listview_filters-0.0.1b1.dev2.tar` & `django_listview_filters-0.0.1b1.dev3.tar`

### file list

```diff
@@ -1,13 +1,25 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.readthedocs.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.vscode/settings.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/_helpers.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/_settings.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/filters.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/mixins.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/LICENSE
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/README.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/pyproject.toml
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev2/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/.readthedocs.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/requirements.txt
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/.vscode/settings.json
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/Makefile
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/classes.rst
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/conf.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/make.bat
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/miscellaneous.rst
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/requirements.txt
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/settings.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/custom_extensions/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/docs/custom_extensions/extensions.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/_helpers.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/_settings.py
+-rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/filters.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/mixins.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/LICENSE
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/README.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 django_listview_filters-0.0.1b1.dev3/PKG-INFO
```

### Comparing `django_listview_filters-0.0.1b1.dev2/.readthedocs.yaml` & `django_listview_filters-0.0.1b1.dev3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/filters.py` & `django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/filters.py`

 * *Files identical despite different names*

### Comparing `django_listview_filters-0.0.1b1.dev2/src/django_listview_filters/mixins.py` & `django_listview_filters-0.0.1b1.dev3/src/django_listview_filters/mixins.py`

 * *Files identical despite different names*

### Comparing `django_listview_filters-0.0.1b1.dev2/.gitignore` & `django_listview_filters-0.0.1b1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_listview_filters-0.0.1b1.dev2/LICENSE` & `django_listview_filters-0.0.1b1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_listview_filters-0.0.1b1.dev2/README.md` & `django_listview_filters-0.0.1b1.dev3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Django ListView Filters
 
 [![Documentation Status](https://readthedocs.org/projects/django-listview-filters/badge/?version=latest)](https://django-listview-filters.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/django-listview-filters.svg)](https://badge.fury.io/py/django-listview-filters)
+
+## Description
 
 Add context to list views for sidebar links and modifying querysets with those links.
 
 ## Purpose
 
 Attempting to duplicate the functionality of the [`ModelAdmin` List Filter](https://docs.djangoproject.com/en/stable/ref/contrib/admin/filters/) capabilities.
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
 # Django ListView Filters [![Documentation Status](https://readthedocs.org/
 projects/django-listview-filters/badge/?version=latest)](https://django-
-listview-filters.readthedocs.io/en/latest/?badge=latest) Add context to list
-views for sidebar links and modifying querysets with those links. ## Purpose
-Attempting to duplicate the functionality of the [`ModelAdmin` List Filter]
-(https://docs.djangoproject.com/en/stable/ref/contrib/admin/filters/
-) capabilities. This is largely a copy-paste of the source code for that
-modified to work outside of the admin interface. For example, references to
-`model_admin` have been removed. ## Additional Functionality A few
-customizations are added. ### Add 'Clear Filter' Context Allow for replacing
-the 'All' link with a button that clears the parameter from the query. ### Only
-List Lookups With Matches Allow for filtering of list for sidebar to only those
-with matches. That way empty links aren't taking up valuable space. ### Add
-Count to Context Add the count of number of objects to each link that can be
-shown in the template. ## Configuration ### Model ```python from django.db
-import models class Author(models.Model): name = models.CharField("Author's
-Name", max_length=100) birthday = models.DateField("Author's Birthday",
-blank=True) class Book(models.Model): title = models.CharField("Book Title",
-max_length=150) author = models.ForeignKey(Author, on_delete=models.PROTECT)
-``` ### Class-based View ```python from django.view.generic import ListView
-from django-listview-filters import RelatedFieldListViewFilter class
-AuthorListView(ListView): context_object_name = "author" queryset =
-Author.objects.order_by("name") class BookListView(ListView):
-context_object_name = "book" queryset = Author.objects.order_by("title")
-list_filter = [ ('author', RelatedFieldListViewFilter) ] ``` ### Template
-```python {% for filter_name, filter_objects, clear_fragment in filter_list %}
+listview-filters.readthedocs.io/en/latest/?badge=latest) [![PyPI version]
+(https://badge.fury.io/py/django-listview-filters.svg)](https://badge.fury.io/
+py/django-listview-filters) ## Description Add context to list views for
+sidebar links and modifying querysets with those links. ## Purpose Attempting
+to duplicate the functionality of the [`ModelAdmin` List Filter](https://
+docs.djangoproject.com/en/stable/ref/contrib/admin/filters/) capabilities. This
+is largely a copy-paste of the source code for that modified to work outside of
+the admin interface. For example, references to `model_admin` have been
+removed. ## Additional Functionality A few customizations are added. ### Add
+'Clear Filter' Context Allow for replacing the 'All' link with a button that
+clears the parameter from the query. ### Only List Lookups With Matches Allow
+for filtering of list for sidebar to only those with matches. That way empty
+links aren't taking up valuable space. ### Add Count to Context Add the count
+of number of objects to each link that can be shown in the template. ##
+Configuration ### Model ```python from django.db import models class Author
+(models.Model): name = models.CharField("Author's Name", max_length=100)
+birthday = models.DateField("Author's Birthday", blank=True) class Book
+(models.Model): title = models.CharField("Book Title", max_length=150) author =
+models.ForeignKey(Author, on_delete=models.PROTECT) ``` ### Class-based View
+```python from django.view.generic import ListView from django-listview-filters
+import RelatedFieldListViewFilter class AuthorListView(ListView):
+context_object_name = "author" queryset = Author.objects.order_by("name") class
+BookListView(ListView): context_object_name = "book" queryset =
+Author.objects.order_by("title") list_filter = [ ('author',
+RelatedFieldListViewFilter) ] ``` ### Template ```python {% for filter_name,
+filter_objects, clear_fragment in filter_list %}
 {{ filter_name|title }} clear_filter
     * {% with filter_objects|dictsort:"display" as display_list %} {% for item
       in display_list %}
       {{_item.display_}}
     * {% endfor %} {% endwith %}
 ```
```

### Comparing `django_listview_filters-0.0.1b1.dev2/pyproject.toml` & `django_listview_filters-0.0.1b1.dev3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/wsutc/django-listview-filters"
-"Bug Tracker" = "https://github.com/wsutc/django-listview-filters/issues"
+"Homepage" = "https://git.tricity.wsu.edu/karl.wooster/django-listview-filters"
+"Bug Tracker" = "https://git.tricity.wsu.edu/karl.wooster/django-listview-filters/-/issues"
+"Documentation" = "https://django-listview-filters.readthedocs.io/en/latest/"
+
 
 # [tool]
 # [tool.hatch]
 [tool.hatch.version]
 path = "src/django_listview_filters/__init__.py"
 
-[tool.hatch.build.targets.sdist]
-exclude = ["/.github", "/docs"]
-
-[tool.hatch.guild.targets.wheel]
-packages = ["src/django-listview-filters"]
+# [tool.hatch.build.targets.sdist]
+# exclude = [
+#     "/.github",
+#     "/docs",
+# ]
 
-# [tool.hatch.publish.index.repos.private]
-# url = "https://pypi.org/project/django-listview-filters/"
+# [tool.hatch.guild.targets.wheel]
+# packages = ["src/django-listview-filters"]
```

### Comparing `django_listview_filters-0.0.1b1.dev2/PKG-INFO` & `django_listview_filters-0.0.1b1.dev3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: django_listview_filters
-Version: 0.0.1b1.dev2
+Version: 0.0.1b1.dev3
 Summary: Add context to list views for sidebar links and modifying querysets with those links.
-Project-URL: Homepage, https://github.com/wsutc/django-listview-filters
-Project-URL: Bug Tracker, https://github.com/wsutc/django-listview-filters/issues
+Project-URL: Homepage, https://git.tricity.wsu.edu/karl.wooster/django-listview-filters
+Project-URL: Bug Tracker, https://git.tricity.wsu.edu/karl.wooster/django-listview-filters/-/issues
+Project-URL: Documentation, https://django-listview-filters.readthedocs.io/en/latest/
 Author-email: Karl Wooster <karl.wooster@wsu.edu>
 License: MIT License
         
         Copyright (c) 2022 Washington State University - Tri-Cities
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,14 +35,17 @@
 Requires-Dist: django
 Requires-Dist: furl
 Description-Content-Type: text/markdown
 
 # Django ListView Filters
 
 [![Documentation Status](https://readthedocs.org/projects/django-listview-filters/badge/?version=latest)](https://django-listview-filters.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/django-listview-filters.svg)](https://badge.fury.io/py/django-listview-filters)
+
+## Description
 
 Add context to list views for sidebar links and modifying querysets with those links.
 
 ## Purpose
 
 Attempting to duplicate the functionality of the [`ModelAdmin` List Filter](https://docs.djangoproject.com/en/stable/ref/contrib/admin/filters/) capabilities.
```

