# Comparing `tmp/django-mass-migration-0.1.0.tar.gz` & `tmp/django-mass-migration-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.1.0.tar", last modified: Thu Jun 15 09:40:05 2023, max compression
+gzip compressed data, was "django-mass-migration-0.1.2.tar", last modified: Wed Jun 21 16:10:12 2023, max compression
```

## Comparing `django-mass-migration-0.1.0.tar` & `django-mass-migration-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.650892 django-mass-migration-0.1.0/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-15 09:40:05.000000 django-mass-migration-0.1.0/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-15 09:40:05.000000 django-mass-migration-0.1.0/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:40:05.000000 django-mass-migration-0.1.0/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:40:05.000000 django-mass-migration-0.1.0/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:40:05.000000 django-mass-migration-0.1.0/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.646892 django-mass-migration-0.1.0/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.646892 django-mass-migration-0.1.0/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.646892 django-mass-migration-0.1.0/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/templates/massmigration/run_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-15 09:39:59.000000 django-mass-migration-0.1.0/massmigration/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:40:05.654892 django-mass-migration-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-15 09:40:03.000000 django-mass-migration-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.887647 django-mass-migration-0.1.2/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.887647 django-mass-migration-0.1.2/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.887647 django-mass-migration-0.1.2/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.887647 django-mass-migration-0.1.2/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.883647 django-mass-migration-0.1.2/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.883647 django-mass-migration-0.1.2/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.883647 django-mass-migration-0.1.2/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/templates/migration_templates/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-21 16:10:10.000000 django-mass-migration-0.1.2/massmigration/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:10:12.891647 django-mass-migration-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-21 16:10:12.000000 django-mass-migration-0.1.2/setup.py
```

### Comparing `django-mass-migration-0.1.0/LICENSE` & `django-mass-migration-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/PKG-INFO` & `django-mass-migration-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.0
+Version: 0.1.2
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django Mass Migration
 =====================
 
-This is a Django app which provides utilities for performing data operations on (optionally) large datasets.
+A Django app which provides utilities for performing data operations on (optionally) large datasets.
 
 Similar to Django's built-in migration system, it allows you to define data migrations to be performed on the database,
 and to apply those migration operations to your database, and it tracks which migrations have been applied and which haven't.
 
 Unlike Django's built-in migration system, it is designed for performing long-running data modification tasks
 where there could be a significant amount of time between when the migration is started and when it's finished.
 See [Concepts](#concepts).
@@ -55,15 +55,15 @@
 This command has two required, positional arguments:
 
 1. `app_label` - this should be the name of an installed app in your project.
 2. `migration_name` - this should be the name that you want to give you migration.
 
 The command also takes the following optional arguments:
 
-* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types).
+* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types). The default is `mapper`.
 
 A file will be created inside a folder called 'massmigrations' in your app, using the supplied migration name.
 E.g. `myapp/massmigrations/001_my_migration.py`.
 This is a blank slate for you to write your migration code in.
 
 
 Migration Types
@@ -167,14 +167,15 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.0/README.md` & `django-mass-migration-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django Mass Migration
 =====================
 
-This is a Django app which provides utilities for performing data operations on (optionally) large datasets.
+A Django app which provides utilities for performing data operations on (optionally) large datasets.
 
 Similar to Django's built-in migration system, it allows you to define data migrations to be performed on the database,
 and to apply those migration operations to your database, and it tracks which migrations have been applied and which haven't.
 
 Unlike Django's built-in migration system, it is designed for performing long-running data modification tasks
 where there could be a significant amount of time between when the migration is started and when it's finished.
 See [Concepts](#concepts).
@@ -36,15 +36,15 @@
 This command has two required, positional arguments:
 
 1. `app_label` - this should be the name of an installed app in your project.
 2. `migration_name` - this should be the name that you want to give you migration.
 
 The command also takes the following optional arguments:
 
-* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types).
+* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types). The default is `mapper`.
 
 A file will be created inside a folder called 'massmigrations' in your app, using the supplied migration name.
 E.g. `myapp/massmigrations/001_my_migration.py`.
 This is a blank slate for you to write your migration code in.
 
 
 Migration Types
@@ -148,14 +148,15 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.0/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.1.2/django_mass_migration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.0
+Version: 0.1.2
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django Mass Migration
 =====================
 
-This is a Django app which provides utilities for performing data operations on (optionally) large datasets.
+A Django app which provides utilities for performing data operations on (optionally) large datasets.
 
 Similar to Django's built-in migration system, it allows you to define data migrations to be performed on the database,
 and to apply those migration operations to your database, and it tracks which migrations have been applied and which haven't.
 
 Unlike Django's built-in migration system, it is designed for performing long-running data modification tasks
 where there could be a significant amount of time between when the migration is started and when it's finished.
 See [Concepts](#concepts).
@@ -55,15 +55,15 @@
 This command has two required, positional arguments:
 
 1. `app_label` - this should be the name of an installed app in your project.
 2. `migration_name` - this should be the name that you want to give you migration.
 
 The command also takes the following optional arguments:
 
-* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types).
+* `--template` - this should be the name of one of the supplied templates in `massmigration/templates/migration_templates`, without the extension, e.g. `--template=mapper`. See [Migration Types](#migration-types). The default is `mapper`.
 
 A file will be created inside a folder called 'massmigrations' in your app, using the supplied migration name.
 E.g. `myapp/massmigrations/001_my_migration.py`.
 This is a blank slate for you to write your migration code in.
 
 
 Migration Types
@@ -167,14 +167,15 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.0/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.1.2/django_mass_migration.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,11 +27,14 @@
 massmigration/management/commands/__init__.py
 massmigration/management/commands/makemassmigration.py
 massmigration/templates/admin/massmigration/migrationrecord/change_list.html
 massmigration/templates/massmigration/base.html
 massmigration/templates/massmigration/delete_migration.html
 massmigration/templates/massmigration/manage_migrations.html
 massmigration/templates/massmigration/run_migration.html
+massmigration/templates/migration_templates/custom.py
+massmigration/templates/migration_templates/mapper.py
+massmigration/templates/migration_templates/simple.py
 massmigration/utils/__init__.py
 massmigration/utils/apps.py
 massmigration/utils/functional.py
 massmigration/utils/permissions.py
```

### Comparing `django-mass-migration-0.1.0/massmigration/admin.py` & `django-mass-migration-0.1.2/massmigration/admin.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/backends/base.py` & `django-mass-migration-0.1.2/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/backends/djangae.py` & `django-mass-migration-0.1.2/massmigration/backends/djangae.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/enforcement.py` & `django-mass-migration-0.1.2/massmigration/enforcement.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/exceptions.py` & `django-mass-migration-0.1.2/massmigration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/loader.py` & `django-mass-migration-0.1.2/massmigration/loader.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.1.2/massmigration/management/commands/makemassmigration.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             help=(
                 "Name to give the migration file. "
                 "This can only contain letters, numbers and underscores."
             ),
         )
         parser.add_argument(
             "--template",
-            default="simple",
+            default="mapper",
             help=(
                 "Which mapper template to use as the base. "
                 "Must exist as a python file in massmigration/templates/migration_templates."
             ),
         )
 
     def handle(self, *args, **options):
```

### Comparing `django-mass-migration-0.1.0/massmigration/migrations.py` & `django-mass-migration-0.1.2/massmigration/migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,31 @@
 import logging
 
 # Third party
 from gcloudc.db import transaction
 from djangae.utils import retry_on_error
 from django.conf import settings
 from django.db import models
-from django.utils import timezone
 from django.utils.module_loading import import_string
 
 # Djangae Migrations
 from . import record_cache
+from .constants import DEFAULT_BACKEND
 from .exceptions import DependentMigrationNotApplied, MigrationAlreadyStarted
 from .models import MigrationRecord
 
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_BACKEND = "massmigration.backends.djangae.DjangaeBackend"
-
 
 class BaseMigration:
     """ An operation to be performed on the database. """
 
     dependencies = []  # A list of (app_label, migration_name) pairs
 
-    # This is for use for migrations which are not stored in a folder called 'migrations' inside
-    # an installed app.
-    app_label: str = None
-
     # This can be set to make a migration run on a specific backend, rather than the one that's
     # that's specified in the Django settings
     backend: str = None
 
     # This specifies the name of the method on the backend class which should be called to run this
     # migration. Custom migration types can be run on custom backends which support them by using
     # this attribute.
```

### Comparing `django-mass-migration-0.1.0/massmigration/models.py` & `django-mass-migration-0.1.2/massmigration/models.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/record_cache.py` & `django-mass-migration-0.1.2/massmigration/record_cache.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.1.2/massmigration/templates/massmigration/base.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.1.2/massmigration/templates/massmigration/delete_migration.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.1.2/massmigration/templates/massmigration/manage_migrations.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/utils/functional.py` & `django-mass-migration-0.1.2/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/massmigration/views.py` & `django-mass-migration-0.1.2/massmigration/views.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.0/setup.py` & `django-mass-migration-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # TODO: possibly make the dependency on djangae optional
 EXTRAS = {}
 
 
 setup(
     name=NAME,
-    version="v0.1.0",
+    version="v0.1.2",
     packages=PACKAGES,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=["django", "djangae", "django-gcloud-connectors", "Google App Engine"],
     url=URL,
@@ -33,12 +33,12 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
     include_package_data=True,
     install_requires=[
         "django>=3.2,<5.0",
         "djangae>=1.1.0",
-        "django-gcloud-connectors>=0.3.7",
+        "django-gcloud-connectors>=0.3.6",
     ],
     extras_require=EXTRAS,
     # tests_require=EXTRAS["test"],
 )
```

