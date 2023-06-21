# Comparing `tmp/bk-iam-1.3.2.tar.gz` & `tmp/bk-iam-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk-iam-1.3.2.tar", last modified: Wed Jun 14 09:23:09 2023, max compression
+gzip compressed data, was "dist/bk-iam-1.3.3.tar", last modified: Wed Jun 21 09:42:43 2023, max compression
```

## Comparing `bk-iam-1.3.2.tar` & `bk-iam-1.3.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-14 09:22:24.000000 bk-iam-1.3.2/iam/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/api/
--rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.2/iam/api/client.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/api/http.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/meta.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/objects.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/dummy_iam.py
--rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.2/iam/iam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/apply/
--rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/apply/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/apply/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/eval/
--rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/eval/constants.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/eval/object.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/eval/expression.py
--rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/eval/operators.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/model/
--rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/model/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/
--rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/apps.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/templates/
--rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/templates/migration.tmpl
--rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/utils/
--rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/utils/do_migrate.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/migrator.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/management/commands/
--rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/iam_migration/migrations/
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/iam_migration/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/django/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/django/dispatcher/
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/django/dispatcher/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9922 2023-06-14 09:22:24.000000 bk-iam-1.3.2/iam/contrib/django/dispatcher/dispatchers.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/django/dispatcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/django/middlewares.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/django/response.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/converter/
--rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/converter/base.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/converter/queryset.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/converter/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/contrib/tastypie/
--rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/tastypie/resource.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/tastypie/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/tastypie/authorization.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/tastypie/shortcuts.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/contrib/http.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/resource/
--rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/resource/provider.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/resource/constants.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/resource/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/resource/utils.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/resource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/iam/auth/
--rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/auth/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.2/iam/cache.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-14 09:23:09.000000 bk-iam-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-14 09:22:24.000000 bk-iam-1.3.2/readme_en.md
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-14 09:23:09.000000 bk-iam-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1244 2023-03-07 02:07:52.000000 bk-iam-1.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:23:09.000000 bk-iam-1.3.2/bk_iam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-14 09:23:09.000000 bk-iam-1.3.2/bk_iam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:23:09.000000 bk-iam-1.3.2/bk_iam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-14 09:23:08.000000 bk-iam-1.3.2/bk_iam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-14 09:23:09.000000 bk-iam-1.3.2/bk_iam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-14 09:23:08.000000 bk-iam-1.3.2/bk_iam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-14 09:22:24.000000 bk-iam-1.3.2/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-21 09:42:03.000000 bk-iam-1.3.3/iam/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/api/
+-rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.3/iam/api/client.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/api/http.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/objects.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/dummy_iam.py
+-rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.3/iam/iam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/apply/
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/apply/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/apply/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/eval/
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/object.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/expression.py
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/operators.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/model/
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/model/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/
+-rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/apps.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/templates/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/templates/migration.tmpl
+-rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/
+-rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/do_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrator.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrations/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/django/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9942 2023-06-21 09:42:03.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/dispatchers.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/response.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/converter/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/base.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/queryset.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/tastypie/
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/resource.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/http.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/resource/
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/provider.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/constants.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/utils.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/auth/
+-rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/auth/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/cache.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-21 09:42:43.000000 bk-iam-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-14 09:22:24.000000 bk-iam-1.3.3/readme_en.md
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 09:42:43.000000 bk-iam-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-03-07 02:07:52.000000 bk-iam-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-06-14 09:22:24.000000 bk-iam-1.3.3/readme.md
```

### Comparing `bk-iam-1.3.2/iam/api/client.py` & `bk-iam-1.3.3/iam/api/client.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/api/__init__.py` & `bk-iam-1.3.3/iam/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/api/http.py` & `bk-iam-1.3.3/iam/api/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/meta.py` & `bk-iam-1.3.3/iam/meta.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/exceptions.py` & `bk-iam-1.3.3/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/objects.py` & `bk-iam-1.3.3/iam/objects.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/dummy_iam.py` & `bk-iam-1.3.3/iam/dummy_iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/iam.py` & `bk-iam-1.3.3/iam/iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/apply/models.py` & `bk-iam-1.3.3/iam/apply/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/apply/__init__.py` & `bk-iam-1.3.3/iam/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/utils.py` & `bk-iam-1.3.3/iam/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/eval/constants.py` & `bk-iam-1.3.3/iam/eval/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/eval/object.py` & `bk-iam-1.3.3/iam/eval/object.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/eval/expression.py` & `bk-iam-1.3.3/iam/eval/expression.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/eval/operators.py` & `bk-iam-1.3.3/iam/eval/operators.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/eval/__init__.py` & `bk-iam-1.3.3/iam/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/model/models.py` & `bk-iam-1.3.3/iam/model/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/model/__init__.py` & `bk-iam-1.3.3/iam/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/collection.py` & `bk-iam-1.3.3/iam/collection.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/apps.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/apps.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/constants.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/templates/migration.tmpl` & `bk-iam-1.3.3/iam/contrib/iam_migration/templates/migration.tmpl`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/exceptions.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/template.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/template.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/utils/do_migrate.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/utils/do_migrate.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/utils/__init__.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/migrator.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/__init__.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/management/commands/iam_makemigrations.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/iam_makemigrations.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/management/commands/__init__.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/management/__init__.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/migrations/__init__.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/iam_migration/conf.py` & `bk-iam-1.3.3/iam/contrib/iam_migration/conf.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/django/dispatcher/exceptions.py` & `bk-iam-1.3.3/iam/contrib/django/dispatcher/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/django/dispatcher/dispatchers.py` & `bk-iam-1.3.3/iam/contrib/django/dispatcher/dispatchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         result = provider.list_attr_value(filter_obj, page_obj, **options)
 
         return success_response(result.to_dict(), request_id)
 
     def _dispatch_list_instance(self, request, data, request_id):
         options = self._get_options(request)
 
-        filter_obj = get_filter_obj(data.get("filter"), ["parent", "search", "resource_type_chain"])
+        filter_obj = get_filter_obj(data.get("filter"), ["parent", "search", "action", "resource_type_chain"])
         page_obj = get_page_obj(data.get("page"))
 
         provider = self._provider[data["type"]]
 
         pre_process = getattr(provider, "pre_list_instance", None)
         if pre_process and callable(pre_process):
             pre_process(filter_obj, page_obj, **options)
@@ -194,15 +194,15 @@
         result = provider.list_instance_by_policy(filter_obj, page_obj, **options)
 
         return success_response(result.to_list(), request_id)
 
     def _dispatch_search_instance(self, request, data, request_id):
         options = self._get_options(request)
 
-        filter_obj = get_filter_obj(data.get("filter"), ["parent", "keyword"])
+        filter_obj = get_filter_obj(data.get("filter"), ["parent", "action", "keyword"])
 
         if filter_obj.keyword is None or len(filter_obj.keyword) < 2:
             raise KeywordTooShortException("the length of keyword should be greater than or equals to 2")
 
         page_obj = get_page_obj(data.get("page"))
 
         provider = self._provider[data["type"]]
```

### Comparing `bk-iam-1.3.2/iam/contrib/django/dispatcher/__init__.py` & `bk-iam-1.3.3/iam/contrib/django/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/django/middlewares.py` & `bk-iam-1.3.3/iam/contrib/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/django/response.py` & `bk-iam-1.3.3/iam/contrib/django/response.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/django/__init__.py` & `bk-iam-1.3.3/iam/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/converter/base.py` & `bk-iam-1.3.3/iam/contrib/converter/base.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/converter/queryset.py` & `bk-iam-1.3.3/iam/contrib/converter/queryset.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/converter/__init__.py` & `bk-iam-1.3.3/iam/contrib/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/converter/sql.py` & `bk-iam-1.3.3/iam/contrib/converter/sql.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/tastypie/resource.py` & `bk-iam-1.3.3/iam/contrib/tastypie/resource.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/tastypie/__init__.py` & `bk-iam-1.3.3/iam/contrib/tastypie/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/tastypie/authorization.py` & `bk-iam-1.3.3/iam/contrib/tastypie/authorization.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/tastypie/shortcuts.py` & `bk-iam-1.3.3/iam/contrib/tastypie/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/__init__.py` & `bk-iam-1.3.3/iam/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/contrib/http.py` & `bk-iam-1.3.3/iam/contrib/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/__init__.py` & `bk-iam-1.3.3/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/resource/provider.py` & `bk-iam-1.3.3/iam/resource/provider.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/resource/constants.py` & `bk-iam-1.3.3/iam/resource/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/resource/dispatcher.py` & `bk-iam-1.3.3/iam/resource/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/resource/utils.py` & `bk-iam-1.3.3/iam/resource/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/resource/__init__.py` & `bk-iam-1.3.3/iam/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/shortcuts.py` & `bk-iam-1.3.3/iam/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/auth/models.py` & `bk-iam-1.3.3/iam/auth/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/auth/__init__.py` & `bk-iam-1.3.3/iam/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/iam/cache.py` & `bk-iam-1.3.3/iam/cache.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/readme_en.md` & `bk-iam-1.3.3/readme_en.md`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/PKG-INFO` & `bk-iam-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bk-iam
-Version: 1.3.2
+Version: 1.3.3
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Description: bk-iam python sdk
 Platform: UNKNOWN
```

### Comparing `bk-iam-1.3.2/setup.py` & `bk-iam-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/bk_iam.egg-info/SOURCES.txt` & `bk-iam-1.3.3/bk_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.2/bk_iam.egg-info/PKG-INFO` & `bk-iam-1.3.3/bk_iam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bk-iam
-Version: 1.3.2
+Version: 1.3.3
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Description: bk-iam python sdk
 Platform: UNKNOWN
```

### Comparing `bk-iam-1.3.2/readme.md` & `bk-iam-1.3.3/readme.md`

 * *Files identical despite different names*

