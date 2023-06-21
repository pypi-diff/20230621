# Comparing `tmp/wc-django-notifications-0.2.0.tar.gz` & `tmp/wc-django-notifications-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-notifications-0.2.0.tar", last modified: Fri Jun 16 13:55:23 2023, max compression
+gzip compressed data, was "wc-django-notifications-0.3.0.tar", last modified: Wed Jun 21 13:52:07 2023, max compression
```

## Comparing `wc-django-notifications-0.2.0.tar` & `wc-django-notifications-0.3.0.tar`

### file list

```diff
@@ -1,387 +1,401 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      523 2023-06-16 13:54:32.000000 wc-django-notifications-0.2.0/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9730 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     8567 2023-06-16 13:50:14.000000 wc-django-notifications-0.2.0/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1885 2023-06-16 13:01:55.000000 wc-django-notifications-0.2.0/setup.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9730 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9696 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-06-16 12:15:26.000000 wc-django-notifications-0.2.0/wcd_notifications/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1350 2023-06-16 13:46:38.000000 wc-django-notifications-0.2.0/wcd_notifications/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.2.0/wcd_notifications/compat.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2023-06-16 12:05:13.000000 wc-django-notifications-0.2.0/wcd_notifications/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7048 2023-06-16 11:45:20.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/filters.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5207 2023-06-16 11:46:40.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4067 2023-06-16 12:10:37.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/views.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3556 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3614 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3773 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3547 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3511 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3534 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3567 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3545 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3492 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3468 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3468 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3607 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3508 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3500 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3423 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3622 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3514 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3614 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3548 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3547 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3701 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      928 2023-06-16 11:53:31.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/0002_auto_20230616_1153.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9341 2023-06-16 12:51:42.000000 wc-django-notifications-0.2.0/wcd_notifications/models/notifications.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1801 2023-04-14 08:43:15.000000 wc-django-notifications-0.2.0/wcd_notifications/models/stats.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4371 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/services/manager.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2103 2023-06-16 11:47:54.000000 wc-django-notifications-0.2.0/wcd_notifications/services/notifier.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      227 2023-06-16 11:46:27.000000 wc-django-notifications-0.2.0/wcd_notifications/signals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      449 2023-06-16 11:46:34.000000 wc-django-notifications-0.2.0/wcd_notifications/subscriptions.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3927 2023-04-14 08:34:36.000000 wc-django-notifications-0.2.0/wcd_notifications/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      695 2023-06-21 12:56:26.000000 wc-django-notifications-0.3.0/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    11197 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     9862 2023-06-21 13:30:58.000000 wc-django-notifications-0.3.0/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1885 2023-06-16 13:01:55.000000 wc-django-notifications-0.3.0/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1434 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tests/test_clear_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3536 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tests/test_flags_set_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     6113 2023-06-16 11:44:04.000000 wc-django-notifications-0.3.0/tests/test_list_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      993 2023-06-16 11:49:38.000000 wc-django-notifications-0.3.0/tests/test_sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2667 2023-06-16 11:49:45.000000 wc-django-notifications-0.3.0/tests/test_stats_collector.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    11197 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    10144 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-06-21 13:31:35.000000 wc-django-notifications-0.3.0/wcd_notifications/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1615 2023-06-21 07:57:03.000000 wc-django-notifications-0.3.0/wcd_notifications/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.3.0/wcd_notifications/compat.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2023-06-16 12:05:13.000000 wc-django-notifications-0.3.0/wcd_notifications/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7747 2023-06-21 12:22:03.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/filters.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5190 2023-06-21 11:58:02.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/serializers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4466 2023-06-21 13:30:10.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/views.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3791 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4008 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3788 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3753 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3746 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3769 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3802 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3780 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3727 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3842 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3743 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3735 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3658 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3857 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3749 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3783 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3936 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/management/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.0/wcd_notifications/management/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/management/commands/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.0/wcd_notifications/management/commands/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      972 2023-06-21 12:49:40.000000 wc-django-notifications-0.3.0/wcd_notifications/management/commands/notifications_collect_stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      928 2023-06-21 13:09:19.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0002_auto_20230616_1153.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      255 2023-06-21 07:07:29.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0003_delete_stats.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3131 2023-06-21 13:14:01.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0004_auto_20230621_1414.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      451 2023-06-21 12:53:11.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0005_stats_recollect.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9860 2023-06-21 13:08:15.000000 wc-django-notifications-0.3.0/wcd_notifications/models/notifications.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4003 2023-06-21 13:13:44.000000 wc-django-notifications-0.3.0/wcd_notifications/models/stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4777 2023-06-21 11:20:00.000000 wc-django-notifications-0.3.0/wcd_notifications/services/manager.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2103 2023-06-21 12:26:45.000000 wc-django-notifications-0.3.0/wcd_notifications/services/notifier.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      227 2023-06-16 11:46:27.000000 wc-django-notifications-0.3.0/wcd_notifications/signals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      449 2023-06-21 06:33:53.000000 wc-django-notifications-0.3.0/wcd_notifications/subscriptions.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     4378 2023-06-21 13:03:39.000000 wc-django-notifications-0.3.0/wcd_notifications/utils.py
```

### Comparing `wc-django-notifications-0.2.0/LICENSE` & `wc-django-notifications-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/Makefile` & `wc-django-notifications-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/PKG-INFO` & `wc-django-notifications-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: wc-django-notifications
-Version: 0.2.0
-Summary: Modular notifications system for your django applications.
-Home-page: UNKNOWN
-Author: WebCase
-Author-email: info@webcase.studio
-License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: drf
-License-File: LICENSE
-
 # Django notifications
 
 Modular notifications system for your django applications.
 
 ## Installation
 
 ```sh
@@ -129,15 +108,15 @@
 
 
 class OtherOptions(int, Enum):
   ONE = 1
   TWO = 2
 
 
-# Bu running this command you register your flags:
+# By running this command you register your flags:
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
@@ -231,14 +210,39 @@
 
 Returns list of all available flags.
 
 #### `GET[/api/v1/notifications/notifications/list/]`
 
 Paginatable list of notifications.
 
+To be able to display related objects in more detailed manner you may also register serializers that will be used for each object of a particular model:
+
+```python
+from wcd_notifications.contrib.drf.serializers import FIELD_SERIALIZERS
+
+from .models import SomeModel
+from .serializers import SomeModelSerializer
+
+
+# So for any object of `SomeModel` `SomeModelSerializer` will be used to
+# display `props` in notifications list view.
+FIELD_SERIALIZERS.add(SomeModel, SomeModelSerializer)
+```
+
+Also notifications messages can have shortcodes from `wc-shortcodes` and will be transformed during render. You only need to register your custom shortodes:
+
+```python
+from wcd_notifications.contrib.drf.serializers import SHORTCODES_REGISTRY
+
+
+@SHORTCODES_REGISTRY.register()
+def shortcode(entity, context={}):
+  return entity.content
+```
+
 Filters that can be applied:
 
 - **ids**: List of identifiers to filter over:
 
   `&ids=1,2,3&ids=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **actors**: List of actors to filter on:
@@ -291,29 +295,18 @@
 #### `GET[/api/v1/notifications/notifications/stats/]`
 
 Here user can get a notifications statistics. There will be a list for each recipient that current authorization resolves in.
 
 Each recipient stats contains total count of notifications and notification counts for every flag exists in their notifications.
 
 So this way you will find all read/unread messages for example.
-# Changelog
-All notable changes to this project will be documented in this file.
-
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+Filters that can be applied:
 
-## [0.2.0]
-### Fixed
-- Past form of verb "send" changed everywhere from "sended" to "sent".
-- Removed explicit `pagination_class` from notifications list view.
-- Small fixes.
-
-## [0.1.3]
-### Fixed
-- Django 2.2 compatibility.
+- **actor_types**: List of types for filter on:
 
-## [0.1.1]
-Initial version.
+  `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
+- **action_types**: Same as **actor_types**.
+- **target_types**: Same as **actor_types**.
 
+By applying filters you receive statistics data only for affected notifications.
```

### Comparing `wc-django-notifications-0.2.0/README.md` & `wc-django-notifications-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: wc-django-notifications
+Version: 0.3.0
+Summary: Modular notifications system for your django applications.
+Home-page: UNKNOWN
+Author: WebCase
+Author-email: info@webcase.studio
+License: MIT License
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: drf
+License-File: LICENSE
+
 # Django notifications
 
 Modular notifications system for your django applications.
 
 ## Installation
 
 ```sh
@@ -108,15 +129,15 @@
 
 
 class OtherOptions(int, Enum):
   ONE = 1
   TWO = 2
 
 
-# Bu running this command you register your flags:
+# By running this command you register your flags:
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
@@ -210,14 +231,39 @@
 
 Returns list of all available flags.
 
 #### `GET[/api/v1/notifications/notifications/list/]`
 
 Paginatable list of notifications.
 
+To be able to display related objects in more detailed manner you may also register serializers that will be used for each object of a particular model:
+
+```python
+from wcd_notifications.contrib.drf.serializers import FIELD_SERIALIZERS
+
+from .models import SomeModel
+from .serializers import SomeModelSerializer
+
+
+# So for any object of `SomeModel` `SomeModelSerializer` will be used to
+# display `props` in notifications list view.
+FIELD_SERIALIZERS.add(SomeModel, SomeModelSerializer)
+```
+
+Also notifications messages can have shortcodes from `wc-shortcodes` and will be transformed during render. You only need to register your custom shortodes:
+
+```python
+from wcd_notifications.contrib.drf.serializers import SHORTCODES_REGISTRY
+
+
+@SHORTCODES_REGISTRY.register()
+def shortcode(entity, context={}):
+  return entity.content
+```
+
 Filters that can be applied:
 
 - **ids**: List of identifiers to filter over:
 
   `&ids=1,2,3&ids=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **actors**: List of actors to filter on:
@@ -270,7 +316,49 @@
 #### `GET[/api/v1/notifications/notifications/stats/]`
 
 Here user can get a notifications statistics. There will be a list for each recipient that current authorization resolves in.
 
 Each recipient stats contains total count of notifications and notification counts for every flag exists in their notifications.
 
 So this way you will find all read/unread messages for example.
+
+Filters that can be applied:
+
+- **actor_types**: List of types for filter on:
+
+  `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
+
+- **action_types**: Same as **actor_types**.
+- **target_types**: Same as **actor_types**.
+
+By applying filters you receive statistics data only for affected notifications.
+# Changelog
+All notable changes to this project will be documented in this file.
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
+and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+## [Unreleased]
+
+## [0.3.0]
+### Changed
+- Internal stats collect implementation.
+### Added
+- Management command to recollect stats.
+- Notification stats filtering.
+
+## [0.2.0]
+### Changed
+- Past form of verb "send" changed everywhere from "sended" to "sent".
+### Removed
+- Removed explicit `pagination_class` from notifications list view.
+### Fixed
+- Small fixes.
+
+## [0.1.3]
+### Fixed
+- Django 2.2 compatibility.
+
+## [0.1.1]
+Initial version.
+
+
```

### Comparing `wc-django-notifications-0.2.0/setup.py` & `wc-django-notifications-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/tox.ini` & `wc-django-notifications-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wc_django_notifications.egg-info/PKG-INFO` & `wc-django-notifications-0.3.0/wc_django_notifications.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -129,15 +129,15 @@
 
 
 class OtherOptions(int, Enum):
   ONE = 1
   TWO = 2
 
 
-# Bu running this command you register your flags:
+# By running this command you register your flags:
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
@@ -231,14 +231,39 @@
 
 Returns list of all available flags.
 
 #### `GET[/api/v1/notifications/notifications/list/]`
 
 Paginatable list of notifications.
 
+To be able to display related objects in more detailed manner you may also register serializers that will be used for each object of a particular model:
+
+```python
+from wcd_notifications.contrib.drf.serializers import FIELD_SERIALIZERS
+
+from .models import SomeModel
+from .serializers import SomeModelSerializer
+
+
+# So for any object of `SomeModel` `SomeModelSerializer` will be used to
+# display `props` in notifications list view.
+FIELD_SERIALIZERS.add(SomeModel, SomeModelSerializer)
+```
+
+Also notifications messages can have shortcodes from `wc-shortcodes` and will be transformed during render. You only need to register your custom shortodes:
+
+```python
+from wcd_notifications.contrib.drf.serializers import SHORTCODES_REGISTRY
+
+
+@SHORTCODES_REGISTRY.register()
+def shortcode(entity, context={}):
+  return entity.content
+```
+
 Filters that can be applied:
 
 - **ids**: List of identifiers to filter over:
 
   `&ids=1,2,3&ids=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **actors**: List of actors to filter on:
@@ -291,26 +316,46 @@
 #### `GET[/api/v1/notifications/notifications/stats/]`
 
 Here user can get a notifications statistics. There will be a list for each recipient that current authorization resolves in.
 
 Each recipient stats contains total count of notifications and notification counts for every flag exists in their notifications.
 
 So this way you will find all read/unread messages for example.
+
+Filters that can be applied:
+
+- **actor_types**: List of types for filter on:
+
+  `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
+
+- **action_types**: Same as **actor_types**.
+- **target_types**: Same as **actor_types**.
+
+By applying filters you receive statistics data only for affected notifications.
 # Changelog
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.0]
+### Changed
+- Internal stats collect implementation.
+### Added
+- Management command to recollect stats.
+- Notification stats filtering.
+
 ## [0.2.0]
-### Fixed
+### Changed
 - Past form of verb "send" changed everywhere from "sended" to "sent".
+### Removed
 - Removed explicit `pagination_class` from notifications list view.
+### Fixed
 - Small fixes.
 
 ## [0.1.3]
 ### Fixed
 - Django 2.2 compatibility.
 
 ## [0.1.1]
```

### Comparing `wc-django-notifications-0.2.0/wc_django_notifications.egg-info/SOURCES.txt` & `wc-django-notifications-0.3.0/wc_django_notifications.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 setup.cfg
 setup.py
 tox.ini
+tests/test_clear_view.py
+tests/test_flags_set_view.py
+tests/test_list_view.py
+tests/test_sender.py
+tests/test_stats_collector.py
 wc_django_notifications.egg-info/PKG-INFO
 wc_django_notifications.egg-info/SOURCES.txt
 wc_django_notifications.egg-info/dependency_links.txt
 wc_django_notifications.egg-info/requires.txt
 wc_django_notifications.egg-info/top_level.txt
 wcd_notifications/__init__.py
 wcd_notifications/admin.py
@@ -192,16 +197,22 @@
 wcd_notifications/locale/uk/LC_MESSAGES/django.po
 wcd_notifications/locale/ur/LC_MESSAGES/django.mo
 wcd_notifications/locale/ur/LC_MESSAGES/django.po
 wcd_notifications/locale/uz/LC_MESSAGES/django.mo
 wcd_notifications/locale/uz/LC_MESSAGES/django.po
 wcd_notifications/locale/vi/LC_MESSAGES/django.mo
 wcd_notifications/locale/vi/LC_MESSAGES/django.po
+wcd_notifications/management/__init__.py
+wcd_notifications/management/commands/__init__.py
+wcd_notifications/management/commands/notifications_collect_stats.py
 wcd_notifications/migrations/0001_initial.py
 wcd_notifications/migrations/0002_auto_20230616_1153.py
+wcd_notifications/migrations/0003_delete_stats.py
+wcd_notifications/migrations/0004_auto_20230621_1414.py
+wcd_notifications/migrations/0005_stats_recollect.py
 wcd_notifications/migrations/__init__.py
 wcd_notifications/models/__init__.py
 wcd_notifications/models/notifications.py
 wcd_notifications/models/stats.py
 wcd_notifications/services/__init__.py
 wcd_notifications/services/manager.py
 wcd_notifications/services/notifier.py
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/admin.py` & `wc-django-notifications-0.3.0/wcd_notifications/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,13 +37,21 @@
         manager.collect_stats([obj.recipient])
 
         return result
 
 
 @admin.register(Stats)
 class StatsAdmin(admin.ModelAdmin):
-    list_display = 'id', 'recipient', 'total',
-    list_filter = 'recipient_content_type',
+    list_display = (
+        'id', 'recipient', 'flag', 'amount',
+        'recipient_content_type', 'actor_content_type',
+        'action_content_type', 'target_content_type',
+    )
+    list_filter = (
+        'recipient_content_type', 'actor_content_type',
+        'action_content_type', 'target_content_type',
+    )
+    list_select_related = list_filter
     search_fields = (
         'recipient_content_type', 'recipient_object_id',
-        'flags', 'total',
+        'flag', 'amount',
     )
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/compat.py` & `wc-django-notifications-0.3.0/wcd_notifications/compat.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/conf.py` & `wc-django-notifications-0.3.0/wcd_notifications/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/filters.py` & `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.db import models
 
 from django_filters import rest_framework as filters
 from django_filters import fields
 from django_filters import widgets
 from django_filters.constants import EMPTY_VALUES
 
-from wcd_notifications.models import Notification
+from wcd_notifications.models import Notification, Stats
 from wcd_notifications.utils import from_content_type_key
 
 
 class SplitterWidget(widgets.BaseCSVWidget):
     delimiter = ','
 
     def __init__(self, *args, **kwargs):
@@ -117,14 +117,22 @@
     }
 
     def clean(self, values):
         values = super().clean(values)
         result = []
 
         for value in values:
+            if not value or value.isspace():
+                if self.required:
+                    raise forms.ValidationError(
+                        self.error_messages['required'],
+                        code='required',
+                    )
+                continue
+
             try:
                 content_type = from_content_type_key(value)
             except ContentType.DoesNotExist:
                 raise forms.ValidationError(
                     self.error_messages['no_content_type'],
                     code='no_content_type',
                 )
@@ -230,7 +238,17 @@
         return qs.sent()
 
     def filter_roots(self, qs, value):
         if value is not True:
             return qs
 
         return qs.filter(parent_id__isnull=True)
+
+
+class StatsFilterSet(filters.FilterSet):
+    actor_types = ContentTypeInFilter(field_name='actor_content_type', lookup_expr='in')
+    action_types = ContentTypeInFilter(field_name='action_content_type', lookup_expr='in')
+    target_types = ContentTypeInFilter(field_name='target_content_type', lookup_expr='in')
+
+    class Meta:
+        model = Stats
+        fields = ['actor_types', 'action_types', 'target_types']
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/serializers.py` & `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,16 +161,14 @@
 class NotificationClearSerializer(serializers.Serializer):
     def commit(self, queryset):
         cleared = manager.clear(queryset)
 
         self._data = {'cleared': cleared}
 
 
-class StatsReadSerializer(DisplayRelatedFieldMixin, serializers.ModelSerializer):
-    class Meta:
-        model = Stats
-        fields = 'recipient', 'flags', 'total',
-
+class StatsReadSerializer(DisplayRelatedFieldMixin, serializers.Serializer):
     recipient = serializers.SerializerMethodField()
+    flags = serializers.JSONField()
+    total = serializers.IntegerField()
 
     def get_recipient(self, obj):
         return self._display_related_field(obj, 'recipient')
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/views.py` & `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rest_framework.response import Response
 from rest_framework.generics import ListAPIView, GenericAPIView
 from django_filters import rest_framework as filters
 
 from wcd_notifications.models import Notification, Stats
 from wcd_notifications.utils import resolve_recipients
 
-from .filters import NotificationsFilterSet
+from .filters import NotificationsFilterSet, StatsFilterSet
 from .serializers import (
     FlagReadSerializer,
     NotificationReadSerializer, NotificationChangeFlagSerializer,
     NotificationClearSerializer,
     StatsReadSerializer,
 )
 
@@ -71,14 +71,16 @@
         queryset = self.filter_queryset(self.get_queryset())
         serializer.commit(queryset)
 
 
 class FlagsList(ListAPIView):
     serializer_class = FlagReadSerializer
     flags_registry = property(lambda self: Notification.flags_registry)
+    # HACK: This is for different api analyzers.
+    queryset = Notification.objects.none()
 
     def list(self, request, *args, **kwargs):
         serializer = self.get_serializer(self.flags_registry.values(), many=True)
         return Response(serializer.data)
 
 
 class NotificationsList(NotificationsMixin, ListAPIView):
@@ -92,14 +94,22 @@
 class NotificationsChangeFlags(MultiNotificationsActionView):
     serializer_class = NotificationChangeFlagSerializer
 
 
 class StatsList(RecipientsResolverMixin, ListAPIView):
     serializer_class = StatsReadSerializer
     queryset = Stats.objects.all().prefetch_related('recipient')
+    filter_backends = (filters.DjangoFilterBackend,)
+    filterset_class = StatsFilterSet
+
+    def combine_results(self, queryset):
+        return queryset.resolve_total_flags()
+
+    def filter_queryset(self, queryset):
+        return self.combine_results(super().filter_queryset(queryset))
 
 
 flags_list_view = FlagsList.as_view()
 notifications_list_view = NotificationsList.as_view()
 notifications_change_flags_view = NotificationsChangeFlags.as_view()
 notifications_clear_view = NotificationsClear.as_view()
 stats_list_view = StatsList.as_view()
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
+"2);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
+"4);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -44,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=5; plural=((n%10 == 1) && (n%100 != 11) && (n%100 !"
 "=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && "
 "(n%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 "
 "> 19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != "
 "0 && n % 1000000 == 0) ? 3 : 4);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -46,103 +46,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
+"11) ? 2 : 3;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
-"11) ? 2 : 3;\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
+"2:1));\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
-"4);\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
+"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
+"1 : n % 1 != 0 ? 2: 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +44,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
-"(n > 2 && n < 20) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
+"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
+"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +44,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
+"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
-"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
-"1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
+"(n > 2 && n < 20) ? 2 : 3;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -44,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
-"2);\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -41,103 +43,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
-"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
-"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -44,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -44,103 +44,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -43,103 +44,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -45,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +42,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +41,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-16 15:14+0300\n"
+"POT-Creation-Date: 2023-06-21 16:32+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:136
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
 #: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
@@ -42,103 +45,111 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:37
+#: wcd_notifications/models/notifications.py:38
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:116
+#: wcd_notifications/models/notifications.py:135
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:132
+#: wcd_notifications/models/notifications.py:151
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:138
-#: wcd_notifications/models/stats.py:35
+#: wcd_notifications/models/notifications.py:157
+#: wcd_notifications/models/stats.py:82
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:142
-#: wcd_notifications/models/stats.py:39
+#: wcd_notifications/models/notifications.py:161
+#: wcd_notifications/models/stats.py:86
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:149
+#: wcd_notifications/models/notifications.py:168
+#: wcd_notifications/models/stats.py:93
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:153
+#: wcd_notifications/models/notifications.py:172
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:160
+#: wcd_notifications/models/notifications.py:179
+#: wcd_notifications/models/stats.py:98
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:164
+#: wcd_notifications/models/notifications.py:183
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:171
+#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/stats.py:103
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:175
+#: wcd_notifications/models/notifications.py:194
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:182
+#: wcd_notifications/models/notifications.py:201
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:186
+#: wcd_notifications/models/notifications.py:205
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:191
+#: wcd_notifications/models/notifications.py:210
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:24
+#: wcd_notifications/models/stats.py:71
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:26
+#: wcd_notifications/models/stats.py:73
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:44
+#: wcd_notifications/models/stats.py:108
+msgctxt "wcd_notifications"
+msgid "Flag"
+msgstr ""
+
+#: wcd_notifications/models/stats.py:112
 msgctxt "wcd_notifications"
-msgid "Flags stats"
+msgid "Amount"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:48
+#: wcd_notifications/utils.py:50
 msgctxt "wcd_notifications"
-msgid "Total"
+msgid "No content type found for \"{}\" key."
 msgstr ""
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/migrations/0001_initial.py` & `wc-django-notifications-0.3.0/wcd_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/migrations/0002_auto_20230616_1153.py` & `wc-django-notifications-0.3.0/wcd_notifications/migrations/0002_auto_20230616_1153.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/models/notifications.py` & `wc-django-notifications-0.3.0/wcd_notifications/models/notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
-from json import JSONEncoder
-from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Type, TypedDict
-from itertools import groupby
+from typing import *
 from enum import Enum
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.postgres.fields import ArrayField
 from django.contrib.contenttypes.models import ContentType
 from django.utils import timezone
 from django.utils.translation import pgettext_lazy
 from django.db import models
 from django.contrib.postgres.indexes import GinIndex, BTreeIndex
 from px_pipeline import Filter
 
-from ..utils import Registry, make_generic_Q, to_intarray, ModelDef
+from ..utils import (
+    Registry, make_generic_Q, to_intarray, ModelDef, content_type_from_id as ctfid
+)
 from ..compat import IntegerChoices, JSONField
 
 
 __all__ = (
     'Readability',
     'NotificationQuerySet', 'Notification',
     'make_generic_Q',
@@ -38,16 +38,19 @@
     READ = READABILITY_BASE_NUMBER + 6, pgettext_lazy('wcd_notifications', 'Read')
 
 
 class FlagsRegistry(Registry):
     def add(self, choices: Type[Enum]):
         for item in choices:
             assert item.value not in self, (
-                f'Value {item.value} already registered, check '
-                'your flags for consistency.'
+                f'Value {item.value} already registered as {self[item.value]}, '
+                'check your flags for consistency.'
+            )
+            assert item.value > 9, (
+                f'Value {item.value} is reserved for internal use.'
             )
 
             self[item.value] = item
 
     register = add
 
 
@@ -69,53 +72,68 @@
 
     def targets(self, targets: Sequence[ModelDef]):
         return self.filter(make_generic_Q('target', targets))
 
     def sent(self, now: Optional[datetime] = None):
         return self.filter(sent_at=now if now is not None else timezone.now())
 
+    def collect_recipients(self):
+        fields = 'recipient_content_type', 'recipient_object_id',
+        query = (
+            self
+            .only(*fields)
+            .order_by(*fields)
+            .distinct(*fields)
+            .prefetch_related('recipient')
+        )
+        return [x.recipient for x in query]
+
     def collect_total_stats(self) -> Dict[RecipientDef, int]:
+        fields = (
+            'recipient_content_type', 'recipient_object_id',
+            'actor_content_type', 'action_content_type', 'target_content_type',
+        )
         records = (
             self
-            .values('recipient_content_type', 'recipient_object_id')
+            .values(*fields)
             .order_by()
-            .annotate(total=models.Count('pk'))
-            .values_list('recipient_content_type', 'recipient_object_id', 'total')
+            .annotate(count=models.Count('pk'))
+            .values_list(*fields, 'count')
         )
-        return {
-            (ContentType.objects.get_for_id(ct), oid): total
-            for (ct, oid, total) in records
-        }
+        return [
+            (ctfid(ct), oid, ctfid(actor), ctfid(action), ctfid(target), count)
+            for (ct, oid, actor, action, target, count) in records
+        ]
 
     def collect_flag_stats(self) -> List[FlagStats]:
-        flat_records = list(
+        fields = (
+            'recipient_content_type', 'recipient_object_id', 'flag',
+            'actor_content_type', 'action_content_type', 'target_content_type',
+        )
+        records = (
             self
             .annotate(flag=models.Func('flags', function='unnest'))
-            .values('flag', 'recipient_content_type', 'recipient_object_id')
+            .values(*fields)
             .order_by()
-            .annotate(count=models.Count('*'))
+            .annotate(count=models.Count('pk'))
+            .values_list(*fields, 'count')
         )
-        key = lambda x: (x['recipient_content_type'], x['recipient_object_id'])
-        stats_map = groupby(sorted(flat_records, key=key), key=key)
 
         return [
-            {
-                'recipient': (ContentType.objects.get_for_id(ct), oid),
-                'stats': {x['flag']: x['count'] for x in items}
-            }
-            for (ct, oid), items in stats_map
+            (ctfid(ct), oid, ctfid(actor), ctfid(action), ctfid(target), fl, count)
+            for (ct, oid, fl, actor, action, target, count) in records
         ]
 
 
 class Notification(models.Model):
     Readability = Readability
 
     preparator = Filter()
     flags_registry = FlagsRegistry()
-    objects = NotificationQuerySet.as_manager()
+    objects: Union[NotificationQuerySet, models.Manager] = NotificationQuerySet.as_manager()
 
     class Meta:
         verbose_name = pgettext_lazy('wcd_notifications', 'Notification')
         verbose_name_plural = pgettext_lazy('wcd_notifications', 'Notifications')
         ordering = ('-ordering_field', '-sent_at', '-created_at', '-pk',)
         indexes = [
             GinIndex(
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/services/manager.py` & `wc-django-notifications-0.3.0/wcd_notifications/services/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional, Sequence, Set
+from itertools import chain
 
 from django.db import models
 from px_pipeline import StraightPipeline
 
-from ..models import Notification, NotificationQuerySet, Stats
+from ..models import Notification, NotificationQuerySet, Stats, TOTAL_FLAG
 from ..signals import (
     notifications_flags_changed, notifications_updated, notifications_cleared,
     stats_updated,
 )
 from ..utils import model_bulk_update_or_create, to_intarray, ModelDef
 from ..conf import settings
 
@@ -112,34 +113,42 @@
 
 
 def collect_stats(recipients: Optional[Sequence[ModelDef]]) -> List[Stats]:
     qs: NotificationQuerySet = Notification.objects.all()
 
     if recipients is not None:
         assert len(recipients) != 0, (
-            'Cant collect statistics for empty recipients list.'
+            'Can\'t collect statistics for empty recipients list.'
         )
         qs = qs.recipients(recipients)
 
     flag_stats = qs.collect_flag_stats()
     total_stats = qs.collect_total_stats()
+    stats = chain(flag_stats, (
+        (ct, oid, actor, action, target, TOTAL_FLAG, count)
+        for (ct, oid, actor, action, target, count) in total_stats
+    ))
 
     instances = model_bulk_update_or_create(Stats, [
         (
             {
-                'recipient_content_type': stat['recipient'][0],
-                'recipient_object_id': stat['recipient'][1],
+                'recipient_content_type': ct,
+                'recipient_object_id': oid,
+                'actor_content_type': actor,
+                'action_content_type': action,
+                'target_content_type': target,
+                'flag': flag,
             },
             {
-                'flags': stat['stats'],
-                'total': total_stats[stat['recipient']],
+                'amount': count,
             }
         )
-        for stat in flag_stats
+        for (ct, oid, actor, action, target, flag, count) in stats
     ])
+    Stats.objects.recipients(recipients).exclude(pk__in=[x.pk for x in instances]).delete()
 
     stats_updated.send(Stats, instances=instances)
 
     return instances
 
 
 def clear(queryset) -> int:
```

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/services/notifier.py` & `wc-django-notifications-0.3.0/wcd_notifications/services/notifier.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.2.0/wcd_notifications/utils.py` & `wc-django-notifications-0.3.0/wcd_notifications/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from itertools import groupby
 from operator import attrgetter
 from operator import or_
 from django.db import models
 from django.contrib.contenttypes.models import ContentType
+from django.utils.translation import pgettext_lazy
 from functools import lru_cache
 from collections import OrderedDict
 from typing import Callable, List, Optional, Sequence, Tuple, Type, TypeVar, Union
 from django.utils.module_loading import import_string
-from django.db.models import prefetch_related_objects
 
 from .conf import settings
 
 
 NATURAL_KEY_DELIMITER = '.'
 M = TypeVar('M', bound=models.Model)
 TypePkPair = Tuple[ContentType, Union[str, int]]
@@ -18,27 +19,42 @@
 
 
 @lru_cache
 def cached_import_string(path: str):
     return import_string(path)
 
 
+def group_and_sort(items, key=lambda x: x, **kwargs):
+    return groupby(sorted(items, key=key, **kwargs), key=key)
+
+
 def get_type_pk_pair(instance: Optional[models.Model] = None):
     if instance is None:
         return None, None
 
     return ContentType.objects.get_for_model(instance.__class__), instance.pk
 
 
+def content_type_from_id(id):
+    return ContentType.objects.get_for_id(id)if id is not None else None
+
+
 def to_content_type_key(ct: ContentType):
     return NATURAL_KEY_DELIMITER.join(ct.natural_key())
 
 
 def from_content_type_key(key: str) -> ContentType:
-    return ContentType.objects.get_by_natural_key(*key.split(NATURAL_KEY_DELIMITER))
+    splitted = key.split(NATURAL_KEY_DELIMITER)
+
+    if len(splitted) != 2:
+        raise ContentType.DoesNotExist(pgettext_lazy(
+            'wcd_notifications', 'No content type found for "{}" key.'
+        ).format(key))
+
+    return ContentType.objects.get_by_natural_key(*splitted)
 
 
 def to_intarray(ints: Sequence[int]) -> str:
     return '{' + ','.join(map(str, ints)) + '}'
 
 
 class Registry(OrderedDict):
```

