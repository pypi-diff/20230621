# Comparing `tmp/mizdb-tomselect-0.3.0.tar.gz` & `tmp/mizdb-tomselect-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb-tomselect-0.3.0.tar", last modified: Tue Jun 20 09:57:27 2023, max compression
+gzip compressed data, was "mizdb-tomselect-0.3.1.tar", last modified: Wed Jun 21 08:29:35 2023, max compression
```

## Comparing `mizdb-tomselect-0.3.0.tar` & `mizdb-tomselect-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.057971 mizdb-tomselect-0.3.0/
--rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.0/LICENSE
--rw-r--r--   0 philip    (1000) philip    (1000)    10012 2023-06-20 09:57:27.057971 mizdb-tomselect-0.3.0/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)     9674 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.0/README.md
--rw-r--r--   0 philip    (1000) philip    (1000)     1530 2023-06-20 09:56:54.000000 mizdb-tomselect-0.3.0/pyproject.toml
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-06-20 09:57:27.057971 mizdb-tomselect-0.3.0/setup.cfg
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.053971 mizdb-tomselect-0.3.0/src/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.055971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/
--rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/__init__.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.053971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.053971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.056971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/css/
--rw-r--r--   0 philip    (1000) philip    (1000)      430 2023-06-15 10:00:33.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.056971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/js/
--rw-r--r--   0 philip    (1000) philip    (1000)   145680 2023-06-20 09:57:24.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.053971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.053971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.056971 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/css/
--rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-r--r--   0 philip    (1000) philip    (1000)     3827 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     5743 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect/widgets.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.056971 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)    10012 2023-06-20 09:57:27.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      672 2023-06-20 09:57:27.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-06-20 09:57:27.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-06-20 09:57:27.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/requires.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-06-20 09:57:27.000000 mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/top_level.txt
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-20 09:57:27.057971 mizdb-tomselect-0.3.0/tests/
--rw-r--r--   0 philip    (1000) philip    (1000)    13937 2023-06-20 06:55:07.000000 mizdb-tomselect-0.3.0/tests/test_e2e.py
--rw-r--r--   0 philip    (1000) philip    (1000)     6615 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.0/tests/test_views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2718 2023-06-15 09:59:55.000000 mizdb-tomselect-0.3.0/tests/test_widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.469478 mizdb-tomselect-0.3.1/
+-rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.1/LICENSE
+-rw-r--r--   0 philip    (1000) philip    (1000)    10466 2023-06-21 08:29:35.468477 mizdb-tomselect-0.3.1/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)    10128 2023-06-20 11:54:49.000000 mizdb-tomselect-0.3.1/README.md
+-rw-r--r--   0 philip    (1000) philip    (1000)     1530 2023-06-20 11:43:52.000000 mizdb-tomselect-0.3.1/pyproject.toml
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-06-21 08:29:35.469478 mizdb-tomselect-0.3.1/setup.cfg
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.406476 mizdb-tomselect-0.3.1/src/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.408476 mizdb-tomselect-0.3.1/src/mizdb_tomselect/
+-rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/__init__.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.407476 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.407476 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.463477 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)      430 2023-06-15 10:00:33.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.463477 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/js/
+-rw-r--r--   0 philip    (1000) philip    (1000)   145680 2023-06-21 08:29:32.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.407476 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.407476 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.465477 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/css/
+-rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-r--r--   0 philip    (1000) philip    (1000)     3827 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     5743 2023-06-20 11:43:52.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect/widgets.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.463477 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)    10466 2023-06-21 08:29:35.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      672 2023-06-21 08:29:35.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-06-21 08:29:35.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-06-21 08:29:35.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/requires.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-06-21 08:29:35.000000 mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/top_level.txt
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-21 08:29:35.468477 mizdb-tomselect-0.3.1/tests/
+-rw-r--r--   0 philip    (1000) philip    (1000)    13937 2023-06-20 06:55:07.000000 mizdb-tomselect-0.3.1/tests/test_e2e.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     6615 2023-06-20 09:53:41.000000 mizdb-tomselect-0.3.1/tests/test_views.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     2718 2023-06-15 09:59:55.000000 mizdb-tomselect-0.3.1/tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.3.0/LICENSE` & `mizdb-tomselect-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/PKG-INFO` & `mizdb-tomselect-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: mizdb-tomselect
-Version: 0.3.0
-Summary: Django autocomplete widgets and views using TomSelect
-Author-email: Philip Becker <yummytea1@gmail.com>
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
-Note that this library was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
@@ -63,39 +52,35 @@
 
 Use the widgets in a form.
 
 ```python
 from django import forms
 
 from mizdb_tomselect.widgets import MIZSelect, MIZSelectTabular
-from .models import MyModel
+from .models import City, Person
 
 
 class MyForm(forms.Form):
-    mizselect = forms.ModelChoiceField(
-        MyModel.objects.all(),
-        widget=MIZSelect(
-            MyModel,
-            url='my_autocomplete_view',
-            search_lookup="name__icontains",
-        ),
+    city = forms.ModelChoiceField(
+        City.objects.all(),
+        widget=MIZSelect(City, url='my_autocomplete_view'),
     )
 
-    # Display results in a table, optionally with additional columns:
-    mizselect_tabular = forms.ModelChoiceField(
-        MyModel.objects.all(),
+    # Display results in a table, with additional columns for fields 
+    # 'first_name' and 'last_name':
+    person = forms.ModelChoiceField(
+        Person.objects.all(),
         widget=MIZSelectTabular(
-            MyModel,
+            Person,
             url='my_autocomplete_view',
-            search_lookup="name__icontains",
-            # extra_columns is a mapping of model field: column header label for extra columns
-            # (columns for valueField and labelField are always included)
-            extra_columns={'name': 'Name', 'something_else': 'Something Else'},
+            search_lookup="full_name__icontains",
+            # for extra columns pass a mapping of model field: column header label
+            extra_columns={'first_name': "First Name", "last_name": "Last Name"},
             # The column header label for the labelField column
-            label_field_label='My Model Objects',
+            label_field_label='Full Name',
         ),
     )
 ``` 
 
 NOTE: Make sure to include [bootstrap](https://getbootstrap.com/docs/5.2/getting-started/download/) somewhere. For example in the template:
 ```html
 <!DOCTYPE html>
@@ -135,38 +120,51 @@
 | url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
 | search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
 | value_field    | `"id"`              | model field that provides the value of an option                                               |
 | label_field    | `"name"`            | model field that provides the label of an option                                               |
 | create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False               | if True, allow selecting multiple options                                                      |
 | changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name for the add view of this model([see below](#option-creation))                         |
+| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
 | filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
+
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-To add more columns, pass an `extra_columns` parameter to the widget. This must
-be a mapping `model field name: column label`. The field name tells TomSelect 
-what values to look up on a model object result for a given column. The label is
-the table header label for a given column
+![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value | Description                         |
 |--------------------|---------------|-------------------------------------|
 | extra_columns      |               | a mapping for additional columns    |
 | value_field_label  | `"ID"`        | table header for the value column   |
 | label_field_label  | `"Object"`    | table header for the label column   |
 
+#### Adding more columns 
+
+To add more columns, pass a `result attribute name: column label` mapping to the widget
+argument `extra_columns`.
+
+The column label is the table header label for a given column.  
+
+The attribute name tells TomSelect what value to look up on a result for the column.
+
+**Important**: that means that the result visible to TomSelect must have an attribute
+or property with that name or the column will remain empty. 
+The results for TomSelect are created by the view calling `values()` on the 
+result queryset, so you must make sure that the attribute name is available
+on the view's root queryset as either a model field or as an annotation.
+
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -178,28 +176,28 @@
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
 ----
 ### Option creation
 
-To enable option creation in the dropdown, pass the URL pattern name for the 
+To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/add', MyModelAddView.as_view(), name='my_model_add'),
+    path('city/add/', CityAddView.as_view(), name='city_add'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', add_url='my_model_add')
+widget = MIZSelect(City, url='my_autocomplete_view', add_url='city_add')
 ```
 
 Clicking on that button sends the user to the add page of the model.
 
 #### AJAX request
 
 If `create_field` was also passed to the widget, clicking on the button will
@@ -217,54 +215,56 @@
 
 Override the view's `create_object` method to change the creation process.
 
 ----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
-pass in the URL pattern name for the changelist.
+pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/change', MyModelChangelistView.as_view(), name='my_model_changelist'),
+    path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', changelist_url='my_model_changelist')
+widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 ----
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
-class Pizza(models.Model):
-    best_topping = models.ForeignKey("Topping", on_delete=models.SET_NULL)
+class Person(models.Model):
+    name = models.CharField(max_length=50)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
     
-class Topping(models.Model):
-    ...
+class City(models.Model):
+    name = models.CharField(max_length=50)
+    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class MyForm(forms.Form):
-    topping = forms.ModelChoiceField(queryset=Toppings.objects.all())
-    pizza = forms.ModelChoiceField(
-        queryset=Pizza.objects.all(),
-        wiget=MIZSelect(
-            Pizza,
-            filter_by=("topping", "best_topping_id")
+class PersonsFromCapitolsForm(forms.Form):
+    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+    person = forms.ModelChoiceField(
+        queryset=Person.objects.all(),
+        widget=MIZSelect(
+            Person,
+            filter_by=("capitol", "city_id")
         )
     )
 ```
-This will result in the Pizza result queryset to be filtered against 
-`best_topping_id` with the current value of the `topping` formfield.
-NOTE: When using `filter_by`, the element now **requires** that the other field 
+This will result in the Person result queryset to be filtered against 
+`city_id` with the current value of the `capitol` formfield.  
+NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
```

### Comparing `mizdb-tomselect-0.3.0/README.md` & `mizdb-tomselect-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+Metadata-Version: 2.1
+Name: mizdb-tomselect
+Version: 0.3.1
+Summary: Django autocomplete widgets and views using TomSelect
+Author-email: Philip Becker <yummytea1@gmail.com>
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
-Note that this library was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
@@ -52,39 +63,35 @@
 
 Use the widgets in a form.
 
 ```python
 from django import forms
 
 from mizdb_tomselect.widgets import MIZSelect, MIZSelectTabular
-from .models import MyModel
+from .models import City, Person
 
 
 class MyForm(forms.Form):
-    mizselect = forms.ModelChoiceField(
-        MyModel.objects.all(),
-        widget=MIZSelect(
-            MyModel,
-            url='my_autocomplete_view',
-            search_lookup="name__icontains",
-        ),
+    city = forms.ModelChoiceField(
+        City.objects.all(),
+        widget=MIZSelect(City, url='my_autocomplete_view'),
     )
 
-    # Display results in a table, optionally with additional columns:
-    mizselect_tabular = forms.ModelChoiceField(
-        MyModel.objects.all(),
+    # Display results in a table, with additional columns for fields 
+    # 'first_name' and 'last_name':
+    person = forms.ModelChoiceField(
+        Person.objects.all(),
         widget=MIZSelectTabular(
-            MyModel,
+            Person,
             url='my_autocomplete_view',
-            search_lookup="name__icontains",
-            # extra_columns is a mapping of model field: column header label for extra columns
-            # (columns for valueField and labelField are always included)
-            extra_columns={'name': 'Name', 'something_else': 'Something Else'},
+            search_lookup="full_name__icontains",
+            # for extra columns pass a mapping of model field: column header label
+            extra_columns={'first_name': "First Name", "last_name": "Last Name"},
             # The column header label for the labelField column
-            label_field_label='My Model Objects',
+            label_field_label='Full Name',
         ),
     )
 ``` 
 
 NOTE: Make sure to include [bootstrap](https://getbootstrap.com/docs/5.2/getting-started/download/) somewhere. For example in the template:
 ```html
 <!DOCTYPE html>
@@ -124,38 +131,51 @@
 | url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
 | search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
 | value_field    | `"id"`              | model field that provides the value of an option                                               |
 | label_field    | `"name"`            | model field that provides the label of an option                                               |
 | create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False               | if True, allow selecting multiple options                                                      |
 | changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name for the add view of this model([see below](#option-creation))                         |
+| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
 | filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
+
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-To add more columns, pass an `extra_columns` parameter to the widget. This must
-be a mapping `model field name: column label`. The field name tells TomSelect 
-what values to look up on a model object result for a given column. The label is
-the table header label for a given column
+![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value | Description                         |
 |--------------------|---------------|-------------------------------------|
 | extra_columns      |               | a mapping for additional columns    |
 | value_field_label  | `"ID"`        | table header for the value column   |
 | label_field_label  | `"Object"`    | table header for the label column   |
 
+#### Adding more columns 
+
+To add more columns, pass a `result attribute name: column label` mapping to the widget
+argument `extra_columns`.
+
+The column label is the table header label for a given column.  
+
+The attribute name tells TomSelect what value to look up on a result for the column.
+
+**Important**: that means that the result visible to TomSelect must have an attribute
+or property with that name or the column will remain empty. 
+The results for TomSelect are created by the view calling `values()` on the 
+result queryset, so you must make sure that the attribute name is available
+on the view's root queryset as either a model field or as an annotation.
+
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -167,28 +187,28 @@
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
 ----
 ### Option creation
 
-To enable option creation in the dropdown, pass the URL pattern name for the 
+To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/add', MyModelAddView.as_view(), name='my_model_add'),
+    path('city/add/', CityAddView.as_view(), name='city_add'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', add_url='my_model_add')
+widget = MIZSelect(City, url='my_autocomplete_view', add_url='city_add')
 ```
 
 Clicking on that button sends the user to the add page of the model.
 
 #### AJAX request
 
 If `create_field` was also passed to the widget, clicking on the button will
@@ -206,54 +226,56 @@
 
 Override the view's `create_object` method to change the creation process.
 
 ----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
-pass in the URL pattern name for the changelist.
+pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/change', MyModelChangelistView.as_view(), name='my_model_changelist'),
+    path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', changelist_url='my_model_changelist')
+widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 ----
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
-class Pizza(models.Model):
-    best_topping = models.ForeignKey("Topping", on_delete=models.SET_NULL)
+class Person(models.Model):
+    name = models.CharField(max_length=50)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
     
-class Topping(models.Model):
-    ...
+class City(models.Model):
+    name = models.CharField(max_length=50)
+    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class MyForm(forms.Form):
-    topping = forms.ModelChoiceField(queryset=Toppings.objects.all())
-    pizza = forms.ModelChoiceField(
-        queryset=Pizza.objects.all(),
-        wiget=MIZSelect(
-            Pizza,
-            filter_by=("topping", "best_topping_id")
+class PersonsFromCapitolsForm(forms.Form):
+    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+    person = forms.ModelChoiceField(
+        queryset=Person.objects.all(),
+        widget=MIZSelect(
+            Person,
+            filter_by=("capitol", "city_id")
         )
     )
 ```
-This will result in the Pizza result queryset to be filtered against 
-`best_topping_id` with the current value of the `topping` formfield.
-NOTE: When using `filter_by`, the element now **requires** that the other field 
+This will result in the Person result queryset to be filtered against 
+`city_id` with the current value of the `capitol` formfield.  
+NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
```

### Comparing `mizdb-tomselect-0.3.0/pyproject.toml` & `mizdb-tomselect-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mizdb-tomselect"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using TomSelect"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4409,15 +4409,15 @@
             }
         };
         if (elem.hasAttribute("is-tabular")) {
             templates.option = function(data, escape) {
                 let columns = `<div class="col-1">${data[this.settings.valueField]}</div>
                      <div class="${this.settings.labelColClass}">${data[this.settings.labelField]}</div>`;
                 for (const c of this.settings.extraColumns) {
-                    columns += `<div class="col">${escape(data[c]) || ""}</div>`;
+                    columns += `<div class="col">${escape(data[c] || "")}</div>`;
                 }
                 return `<div class="row">${columns}</div>`;
             };
         }
         return templates;
     }
```

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect/views.py` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect/widgets.py` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
               choice value of an option (f.ex. 'id')
             label_field: the name of the model field that corresponds to the
               human-readable value of an option (f.ex. 'name')
             create_field: the name of the model field used to create new
               model objects with
             multiple: if True, allow selecting multiple options
             changelist_url: URL name of the changelist view for this model
-            add_url: URL name for the add view of this model
+            add_url: URL name of the add view for this model
             filter_by: a 2-tuple (form_field_name, field_lookup) to filter the
               results against the value of the form field using the given
               Django field lookup. For example:
                ('foo', 'bar__id') => results.filter(bar__id=data['foo'])
             kwargs: additional keyword arguments passed to forms.Select
         """
         self.model = model
```

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/PKG-INFO` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.0
+Version: 0.3.1
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TomSelect for Django (MIZDB)
 
 Django autocomplete widgets and views using [TomSelect](https://tom-select.js.org/).
 
-Note that this library was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
+Note that this was written specifically with the [MIZDB](https://github.com/Actionb/MIZDB) app in mind - it may not apply to your app.
 <!-- TOC -->
 * [TomSelect for Django (MIZDB)](#tomselect-for-django-mizdb)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Widgets](#widgets)
     * [MIZSelect](#mizselect)
     * [MIZSelectTabular](#mizselecttabular)
@@ -63,39 +63,35 @@
 
 Use the widgets in a form.
 
 ```python
 from django import forms
 
 from mizdb_tomselect.widgets import MIZSelect, MIZSelectTabular
-from .models import MyModel
+from .models import City, Person
 
 
 class MyForm(forms.Form):
-    mizselect = forms.ModelChoiceField(
-        MyModel.objects.all(),
-        widget=MIZSelect(
-            MyModel,
-            url='my_autocomplete_view',
-            search_lookup="name__icontains",
-        ),
+    city = forms.ModelChoiceField(
+        City.objects.all(),
+        widget=MIZSelect(City, url='my_autocomplete_view'),
     )
 
-    # Display results in a table, optionally with additional columns:
-    mizselect_tabular = forms.ModelChoiceField(
-        MyModel.objects.all(),
+    # Display results in a table, with additional columns for fields 
+    # 'first_name' and 'last_name':
+    person = forms.ModelChoiceField(
+        Person.objects.all(),
         widget=MIZSelectTabular(
-            MyModel,
+            Person,
             url='my_autocomplete_view',
-            search_lookup="name__icontains",
-            # extra_columns is a mapping of model field: column header label for extra columns
-            # (columns for valueField and labelField are always included)
-            extra_columns={'name': 'Name', 'something_else': 'Something Else'},
+            search_lookup="full_name__icontains",
+            # for extra columns pass a mapping of model field: column header label
+            extra_columns={'first_name': "First Name", "last_name": "Last Name"},
             # The column header label for the labelField column
-            label_field_label='My Model Objects',
+            label_field_label='Full Name',
         ),
     )
 ``` 
 
 NOTE: Make sure to include [bootstrap](https://getbootstrap.com/docs/5.2/getting-started/download/) somewhere. For example in the template:
 ```html
 <!DOCTYPE html>
@@ -135,38 +131,51 @@
 | url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
 | search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
 | value_field    | `"id"`              | model field that provides the value of an option                                               |
 | label_field    | `"name"`            | model field that provides the label of an option                                               |
 | create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
 | multiple       | False               | if True, allow selecting multiple options                                                      |
 | changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name for the add view of this model([see below](#option-creation))                         |
+| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
 | filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
+
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
-To add more columns, pass an `extra_columns` parameter to the widget. This must
-be a mapping `model field name: column label`. The field name tells TomSelect 
-what values to look up on a model object result for a given column. The label is
-the table header label for a given column
+![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
 | Argument           | Default value | Description                         |
 |--------------------|---------------|-------------------------------------|
 | extra_columns      |               | a mapping for additional columns    |
 | value_field_label  | `"ID"`        | table header for the value column   |
 | label_field_label  | `"Object"`    | table header for the label column   |
 
+#### Adding more columns 
+
+To add more columns, pass a `result attribute name: column label` mapping to the widget
+argument `extra_columns`.
+
+The column label is the table header label for a given column.  
+
+The attribute name tells TomSelect what value to look up on a result for the column.
+
+**Important**: that means that the result visible to TomSelect must have an attribute
+or property with that name or the column will remain empty. 
+The results for TomSelect are created by the view calling `values()` on the 
+result queryset, so you must make sure that the attribute name is available
+on the view's root queryset as either a model field or as an annotation.
+
 
 ## Function & Features
 
 ### Searching
 
 The AutocompleteView filters the result queryset against the `search_lookup`
 passed to the widget. The default value for the lookup is `name__icontains`.
@@ -178,28 +187,28 @@
         # Filter using your own queryset method:
         return queryset.search(q)
 ```
 
 ----
 ### Option creation
 
-To enable option creation in the dropdown, pass the URL pattern name for the 
+To enable option creation in the dropdown, pass the URL pattern name of the 
 add page of the given model to the widget. This will add an 'Add' button to the
 bottom of the dropdown.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/add', MyModelAddView.as_view(), name='my_model_add'),
+    path('city/add/', CityAddView.as_view(), name='city_add'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', add_url='my_model_add')
+widget = MIZSelect(City, url='my_autocomplete_view', add_url='city_add')
 ```
 
 Clicking on that button sends the user to the add page of the model.
 
 #### AJAX request
 
 If `create_field` was also passed to the widget, clicking on the button will
@@ -217,54 +226,56 @@
 
 Override the view's `create_object` method to change the creation process.
 
 ----
 ### Changelist link
 
 The dropdown will include a link to the changelist of the given model if you
-pass in the URL pattern name for the changelist.
+pass in the URL pattern name of the changelist view.
 
 ```python
 # urls.py
 urlpatterns = [
     ...
     path('autocomplete/', AutocompleteView.as_view(), name='my_autocomplete_view'),
-    path('my_model/change', MyModelChangelistView.as_view(), name='my_model_changelist'),
+    path('city/change/', CityChangelistView.as_view(), name='city_changelist'),
 ]
 
 # forms.py
-widget = MIZSelect(MyModel, url='my_autocomplete_view', changelist_url='my_model_changelist')
+widget = MIZSelect(City, url='my_autocomplete_view', changelist_url='city_changelist')
 ```
 ----
 ### Filter against values of another field
 
 Use the `filter_by` argument to restrict the available options to the value of 
 another field. The parameter must be a 2-tuple: `(name_of_the_other_form_field, django_field_lookup)`
 ```python
 # models.py
-class Pizza(models.Model):
-    best_topping = models.ForeignKey("Topping", on_delete=models.SET_NULL)
+class Person(models.Model):
+    name = models.CharField(max_length=50)
+    city = models.ForeignKey("City", on_delete=models.SET_NULL, blank=True, null=True)
     
-class Topping(models.Model):
-    ...
+class City(models.Model):
+    name = models.CharField(max_length=50)
+    is_capitol = models.BooleanField(default=False)
 
 # forms.py
-class MyForm(forms.Form):
-    topping = forms.ModelChoiceField(queryset=Toppings.objects.all())
-    pizza = forms.ModelChoiceField(
-        queryset=Pizza.objects.all(),
-        wiget=MIZSelect(
-            Pizza,
-            filter_by=("topping", "best_topping_id")
+class PersonsFromCapitolsForm(forms.Form):
+    capitol = forms.ModelChoiceField(queryset=City.objects.filter(is_capitol=True))
+    person = forms.ModelChoiceField(
+        queryset=Person.objects.all(),
+        widget=MIZSelect(
+            Person,
+            filter_by=("capitol", "city_id")
         )
     )
 ```
-This will result in the Pizza result queryset to be filtered against 
-`best_topping_id` with the current value of the `topping` formfield.
-NOTE: When using `filter_by`, the element now **requires** that the other field 
+This will result in the Person result queryset to be filtered against 
+`city_id` with the current value of the `capitol` formfield.  
+NOTE: When using `filter_by`, the declaring element now **requires** that the other field 
 provides a value. If the other field does not have a value, the search will not 
 return any results.
 
 ## Development & Demo
 
 ```bash
 python3 -m venv venv
```

### Comparing `mizdb-tomselect-0.3.0/src/mizdb_tomselect.egg-info/SOURCES.txt` & `mizdb-tomselect-0.3.1/src/mizdb_tomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/tests/test_e2e.py` & `mizdb-tomselect-0.3.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/tests/test_views.py` & `mizdb-tomselect-0.3.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.0/tests/test_widgets.py` & `mizdb-tomselect-0.3.1/tests/test_widgets.py`

 * *Files identical despite different names*

