# Comparing `tmp/wc-django-envoyer-0.2.4.tar.gz` & `tmp/wc-django-envoyer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-envoyer-0.2.4.tar", last modified: Mon Jun 19 09:46:43 2023, max compression
+gzip compressed data, was "wc-django-envoyer-0.2.5.tar", last modified: Wed Jun 21 13:53:23 2023, max compression
```

## Comparing `wc-django-envoyer-0.2.4.tar` & `wc-django-envoyer-0.2.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      487 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6431 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-06-19 09:44:56.000000 wc-django-envoyer-0.2.4/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/tests/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/tests/test_celery.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/tests/test_run.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-06-19 09:46:43.000000 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1919 2023-06-19 09:46:43.000000 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-19 09:46:43.000000 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-06-19 09:46:43.000000 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-06-19 09:46:43.000000 wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-06-19 09:46:19.000000 wc-django-envoyer-0.2.4/wcd_envoyer/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1779 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/templates.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/admin/utils.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/apps.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/channels/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5692 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/backend.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/console.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4478 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/django_sendmail.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/registry_base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/channels/renderers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      560 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.196701 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/tasks.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       89 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      393 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      386 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1261 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/events.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/migrations/0002_auto_20230505_0852.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/models/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/models/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/models/utils.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     8672 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/services/templates_resolver.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/signals.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-19 09:46:43.200701 wc-django-envoyer-0.2.4/wcd_envoyer/utils/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/utils/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/utils/functional.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/utils/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/utils/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      855 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.4/wcd_envoyer/utils/types.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      487 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6431 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-06-21 13:52:48.000000 wc-django-envoyer-0.2.5/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.056581 wc-django-envoyer-0.2.5/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/tests/test_celery.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/tests/test_run.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.056581 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7472 2023-06-21 13:53:23.000000 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1919 2023-06-21 13:53:23.000000 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-21 13:53:23.000000 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-06-21 13:53:23.000000 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-06-21 13:53:23.000000 wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.056581 wc-django-envoyer-0.2.5/wcd_envoyer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-06-21 13:53:02.000000 wc-django-envoyer-0.2.5/wcd_envoyer/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.056581 wc-django-envoyer-0.2.5/wcd_envoyer/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1779 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/templates.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/admin/utils.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/apps.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/channels/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5692 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/backend.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/console.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4478 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/django_sendmail.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/registry_base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/channels/renderers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      560 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/tasks.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       89 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      393 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      386 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1261 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/events.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/migrations/0002_auto_20230505_0852.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/models/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/models/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/models/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8672 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/services/templates_resolver.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/signals.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:53:23.060581 wc-django-envoyer-0.2.5/wcd_envoyer/utils/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/utils/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/utils/functional.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/utils/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/utils/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      855 2023-06-07 12:35:50.000000 wc-django-envoyer-0.2.5/wcd_envoyer/utils/types.py
```

### Comparing `wc-django-envoyer-0.2.4/LICENSE` & `wc-django-envoyer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/Makefile` & `wc-django-envoyer-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/PKG-INFO` & `wc-django-envoyer-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `wc-django-envoyer-0.2.4/README.md` & `wc-django-envoyer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/setup.py` & `wc-django-envoyer-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     author_email='info@webcase.studio',
     license='MIT License',
     description='Message sender to different channels.',
     install_requires=[
         'django-entangled>=0.5.4,<0.6.0',
         'django-jsonfield>=1.4.1,<2.0.0',
         'px-django-lingua>=0.1.7,<0.2.0',
-        'wc-django-notifications>=0.1.3,<0.3.0',
+        'wc-django-notifications>=0.1.3,<0.4.0',
     ],
     include_package_data=True,
     extras_require={
         'dev': [
             'pytest>=6.0,<7.0',
             'pytest-mock>=3.10.0,<4.0.0',
             'pytest-watch>=4.2,<5.0',
```

### Comparing `wc-django-envoyer-0.2.4/tests/test_celery.py` & `wc-django-envoyer-0.2.5/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/tests/test_run.py` & `wc-django-envoyer-0.2.5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/tox.ini` & `wc-django-envoyer-0.2.5/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/PKG-INFO` & `wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `wc-django-envoyer-0.2.4/wc_django_envoyer.egg-info/SOURCES.txt` & `wc-django-envoyer-0.2.5/wc_django_envoyer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/admin/messages.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/admin/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/admin/templates.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/admin/templates.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/admin/utils.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/admin/utils.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/channels/backend.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/channels/backend.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/console.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/console.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/channels/backends/django_sendmail.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/channels/backends/django_sendmail.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/channels/forms.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/channels/forms.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/channels/registry_base.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/channels/registry_base.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/conf.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/services/sender.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/services/sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/shortcuts.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/contrib/celery/tasks.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/contrib/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/events.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/events.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/migrations/0001_initial.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/migrations/0002_auto_20230505_0852.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/migrations/0002_auto_20230505_0852.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/models/channels.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/models/channels.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/models/messages.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/models/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/services/sender.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/services/sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/services/templates_resolver.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/services/templates_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/shortcuts.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/utils/functional.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/utils/functional.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/utils/models.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/utils/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.4/wcd_envoyer/utils/types.py` & `wc-django-envoyer-0.2.5/wcd_envoyer/utils/types.py`

 * *Files identical despite different names*

