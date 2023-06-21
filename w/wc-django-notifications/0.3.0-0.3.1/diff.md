# Comparing `tmp/wc-django-notifications-0.3.0.tar.gz` & `tmp/wc-django-notifications-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-notifications-0.3.0.tar", last modified: Wed Jun 21 13:52:07 2023, max compression
+gzip compressed data, was "wc-django-notifications-0.3.1.tar", last modified: Wed Jun 21 15:27:24 2023, max compression
```

## Comparing `wc-django-notifications-0.3.0.tar` & `wc-django-notifications-0.3.1.tar`

### file list

```diff
@@ -1,401 +1,402 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      695 2023-06-21 12:56:26.000000 wc-django-notifications-0.3.0/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)    11197 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     9862 2023-06-21 13:30:58.000000 wc-django-notifications-0.3.0/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1885 2023-06-16 13:01:55.000000 wc-django-notifications-0.3.0/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/tests/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1434 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tests/test_clear_view.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3536 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tests/test_flags_set_view.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     6113 2023-06-16 11:44:04.000000 wc-django-notifications-0.3.0/tests/test_list_view.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      993 2023-06-16 11:49:38.000000 wc-django-notifications-0.3.0/tests/test_sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2667 2023-06-16 11:49:45.000000 wc-django-notifications-0.3.0/tests/test_stats_collector.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)    11197 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)    10144 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-06-21 13:52:07.000000 wc-django-notifications-0.3.0/wc_django_notifications.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-06-21 13:31:35.000000 wc-django-notifications-0.3.0/wcd_notifications/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1615 2023-06-21 07:57:03.000000 wc-django-notifications-0.3.0/wcd_notifications/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.3.0/wcd_notifications/compat.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2023-06-16 12:05:13.000000 wc-django-notifications-0.3.0/wcd_notifications/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7747 2023-06-21 12:22:03.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/filters.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5190 2023-06-21 11:58:02.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4466 2023-06-21 13:30:10.000000 wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/views.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3791 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4008 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3788 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3753 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.737786 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3746 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3769 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3802 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3780 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3727 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3842 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3743 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3735 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3658 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.741786 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.729786 wc-django-notifications-0.3.0/wcd_notifications/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3857 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3749 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3783 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3936 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.733786 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/management/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.0/wcd_notifications/management/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/management/commands/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.0/wcd_notifications/management/commands/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      972 2023-06-21 12:49:40.000000 wc-django-notifications-0.3.0/wcd_notifications/management/commands/notifications_collect_stats.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      928 2023-06-21 13:09:19.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0002_auto_20230616_1153.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      255 2023-06-21 07:07:29.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0003_delete_stats.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3131 2023-06-21 13:14:01.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0004_auto_20230621_1414.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      451 2023-06-21 12:53:11.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/0005_stats_recollect.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9860 2023-06-21 13:08:15.000000 wc-django-notifications-0.3.0/wcd_notifications/models/notifications.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4003 2023-06-21 13:13:44.000000 wc-django-notifications-0.3.0/wcd_notifications/models/stats.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 13:52:07.745786 wc-django-notifications-0.3.0/wcd_notifications/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.0/wcd_notifications/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4777 2023-06-21 11:20:00.000000 wc-django-notifications-0.3.0/wcd_notifications/services/manager.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2103 2023-06-21 12:26:45.000000 wc-django-notifications-0.3.0/wcd_notifications/services/notifier.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      227 2023-06-16 11:46:27.000000 wc-django-notifications-0.3.0/wcd_notifications/signals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      449 2023-06-21 06:33:53.000000 wc-django-notifications-0.3.0/wcd_notifications/subscriptions.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     4378 2023-06-21 13:03:39.000000 wc-django-notifications-0.3.0/wcd_notifications/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      833 2023-06-21 15:27:17.000000 wc-django-notifications-0.3.1/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    11335 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     9862 2023-06-21 13:30:58.000000 wc-django-notifications-0.3.1/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1885 2023-06-16 13:01:55.000000 wc-django-notifications-0.3.1/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1434 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/tests/test_clear_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3536 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/tests/test_flags_set_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     6113 2023-06-16 11:44:04.000000 wc-django-notifications-0.3.1/tests/test_list_view.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      993 2023-06-16 11:49:38.000000 wc-django-notifications-0.3.1/tests/test_sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2667 2023-06-16 11:49:45.000000 wc-django-notifications-0.3.1/tests/test_stats_collector.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    11335 2023-06-21 15:27:24.000000 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    10224 2023-06-21 15:27:24.000000 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-21 15:27:24.000000 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2023-06-21 15:27:24.000000 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-06-21 15:27:24.000000 wc-django-notifications-0.3.1/wc_django_notifications.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-06-21 15:25:46.000000 wc-django-notifications-0.3.1/wcd_notifications/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1645 2023-06-21 15:15:16.000000 wc-django-notifications-0.3.1/wcd_notifications/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.3.1/wcd_notifications/compat.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2023-06-16 12:05:13.000000 wc-django-notifications-0.3.1/wcd_notifications/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7747 2023-06-21 12:22:03.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/filters.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5190 2023-06-21 11:58:02.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/serializers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4466 2023-06-21 13:30:10.000000 wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/views.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3791 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4008 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.280887 wc-django-notifications-0.3.1/wcd_notifications/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3788 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3753 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3746 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3769 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.284886 wc-django-notifications-0.3.1/wcd_notifications/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3802 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3780 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3727 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3703 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.288886 wc-django-notifications-0.3.1/wcd_notifications/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3842 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3743 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3735 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.272887 wc-django-notifications-0.3.1/wcd_notifications/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3658 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3857 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.292886 wc-django-notifications-0.3.1/wcd_notifications/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3749 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3849 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3783 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3760 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3782 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:16.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.296886 wc-django-notifications-0.3.1/wcd_notifications/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3704 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3936 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3705 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.276887 wc-django-notifications-0.3.1/wcd_notifications/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-21 13:32:19.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3698 2023-06-21 13:32:17.000000 wc-django-notifications-0.3.1/wcd_notifications/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/management/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.1/wcd_notifications/management/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/management/commands/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-06-21 12:28:09.000000 wc-django-notifications-0.3.1/wcd_notifications/management/commands/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      737 2023-06-21 15:25:32.000000 wc-django-notifications-0.3.1/wcd_notifications/management/commands/notifications_clear_removed_recipients.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      972 2023-06-21 12:49:40.000000 wc-django-notifications-0.3.1/wcd_notifications/management/commands/notifications_collect_stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      928 2023-06-21 13:09:19.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/0002_auto_20230616_1153.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      255 2023-06-21 07:07:29.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/0003_delete_stats.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3131 2023-06-21 13:14:01.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/0004_auto_20230621_1414.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      451 2023-06-21 12:53:11.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/0005_stats_recollect.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9875 2023-06-21 15:16:50.000000 wc-django-notifications-0.3.1/wcd_notifications/models/notifications.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4003 2023-06-21 13:13:44.000000 wc-django-notifications-0.3.1/wcd_notifications/models/stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-21 15:27:24.300886 wc-django-notifications-0.3.1/wcd_notifications/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.3.1/wcd_notifications/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4777 2023-06-21 15:17:26.000000 wc-django-notifications-0.3.1/wcd_notifications/services/manager.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2103 2023-06-21 12:26:45.000000 wc-django-notifications-0.3.1/wcd_notifications/services/notifier.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      227 2023-06-16 11:46:27.000000 wc-django-notifications-0.3.1/wcd_notifications/signals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      458 2023-06-21 15:15:36.000000 wc-django-notifications-0.3.1/wcd_notifications/subscriptions.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     4378 2023-06-21 13:03:39.000000 wc-django-notifications-0.3.1/wcd_notifications/utils.py
```

### Comparing `wc-django-notifications-0.3.0/CHANGELOG.md` & `wc-django-notifications-0.3.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1]
+### Fixed
+- Attempts to collect stats for `None` recipients.
+### Added
+- Management command to clear notifications and stats.
+
 ## [0.3.0]
 ### Changed
 - Internal stats collect implementation.
 ### Added
 - Management command to recollect stats.
 - Notification stats filtering.
```

### Comparing `wc-django-notifications-0.3.0/LICENSE` & `wc-django-notifications-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/Makefile` & `wc-django-notifications-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/PKG-INFO` & `wc-django-notifications-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -335,14 +335,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1]
+### Fixed
+- Attempts to collect stats for `None` recipients.
+### Added
+- Management command to clear notifications and stats.
+
 ## [0.3.0]
 ### Changed
 - Internal stats collect implementation.
 ### Added
 - Management command to recollect stats.
 - Notification stats filtering.
```

### Comparing `wc-django-notifications-0.3.0/README.md` & `wc-django-notifications-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/setup.py` & `wc-django-notifications-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tests/test_clear_view.py` & `wc-django-notifications-0.3.1/tests/test_clear_view.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tests/test_flags_set_view.py` & `wc-django-notifications-0.3.1/tests/test_flags_set_view.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tests/test_list_view.py` & `wc-django-notifications-0.3.1/tests/test_list_view.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tests/test_sender.py` & `wc-django-notifications-0.3.1/tests/test_sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tests/test_stats_collector.py` & `wc-django-notifications-0.3.1/tests/test_stats_collector.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/tox.ini` & `wc-django-notifications-0.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wc_django_notifications.egg-info/PKG-INFO` & `wc-django-notifications-0.3.1/wc_django_notifications.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -335,14 +335,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1]
+### Fixed
+- Attempts to collect stats for `None` recipients.
+### Added
+- Management command to clear notifications and stats.
+
 ## [0.3.0]
 ### Changed
 - Internal stats collect implementation.
 ### Added
 - Management command to recollect stats.
 - Notification stats filtering.
```

### Comparing `wc-django-notifications-0.3.0/wc_django_notifications.egg-info/SOURCES.txt` & `wc-django-notifications-0.3.1/wc_django_notifications.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 wcd_notifications/locale/ur/LC_MESSAGES/django.po
 wcd_notifications/locale/uz/LC_MESSAGES/django.mo
 wcd_notifications/locale/uz/LC_MESSAGES/django.po
 wcd_notifications/locale/vi/LC_MESSAGES/django.mo
 wcd_notifications/locale/vi/LC_MESSAGES/django.po
 wcd_notifications/management/__init__.py
 wcd_notifications/management/commands/__init__.py
+wcd_notifications/management/commands/notifications_clear_removed_recipients.py
 wcd_notifications/management/commands/notifications_collect_stats.py
 wcd_notifications/migrations/0001_initial.py
 wcd_notifications/migrations/0002_auto_20230616_1153.py
 wcd_notifications/migrations/0003_delete_stats.py
 wcd_notifications/migrations/0004_auto_20230621_1414.py
 wcd_notifications/migrations/0005_stats_recollect.py
 wcd_notifications/migrations/__init__.py
```

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/admin.py` & `wc-django-notifications-0.3.1/wcd_notifications/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         'flags', 'message', 'data',
     )
     formfield_overrides = formfield_overrides
 
     def save_model(self, request, obj, form, change) -> None:
         result = super().save_model(request, obj, form, change)
 
-        manager.collect_stats([obj.recipient])
+        if obj.recipient:
+            manager.collect_stats([obj.recipient])
 
         return result
 
 
 @admin.register(Stats)
 class StatsAdmin(admin.ModelAdmin):
     list_display = (
```

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/compat.py` & `wc-django-notifications-0.3.1/wcd_notifications/compat.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/conf.py` & `wc-django-notifications-0.3.1/wcd_notifications/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/filters.py` & `wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/filters.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/serializers.py` & `wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/contrib/drf/views.py` & `wc-django-notifications-0.3.1/wcd_notifications/contrib/drf/views.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/af/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/az/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.1/wcd_notifications/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/be/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.1/wcd_notifications/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/br/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/bs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/da/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/de/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/dsb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/el/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/en/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/es/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/et/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/fy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/gd/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/he/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/hsb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ia/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/id/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ig/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/io/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/io/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/is/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/it/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/kab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/km/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/kn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ky/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/lb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/mk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ml/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/my/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ne/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/os/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/os/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/pa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.1/wcd_notifications/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/te/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/te/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/tg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/th/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/tk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/tt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/udm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo` & `wc-django-notifications-0.3.1/wcd_notifications/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/uz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po` & `wc-django-notifications-0.3.1/wcd_notifications/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/management/commands/notifications_collect_stats.py` & `wc-django-notifications-0.3.1/wcd_notifications/management/commands/notifications_collect_stats.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/migrations/0001_initial.py` & `wc-django-notifications-0.3.1/wcd_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/migrations/0002_auto_20230616_1153.py` & `wc-django-notifications-0.3.1/wcd_notifications/migrations/0002_auto_20230616_1153.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/migrations/0004_auto_20230621_1414.py` & `wc-django-notifications-0.3.1/wcd_notifications/migrations/0004_auto_20230621_1414.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/models/notifications.py` & `wc-django-notifications-0.3.1/wcd_notifications/models/notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         query = (
             self
             .only(*fields)
             .order_by(*fields)
             .distinct(*fields)
             .prefetch_related('recipient')
         )
-        return [x.recipient for x in query]
+        return [x.recipient for x in query if x.recipient]
 
     def collect_total_stats(self) -> Dict[RecipientDef, int]:
         fields = (
             'recipient_content_type', 'recipient_object_id',
             'actor_content_type', 'action_content_type', 'target_content_type',
         )
         records = (
```

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/models/stats.py` & `wc-django-notifications-0.3.1/wcd_notifications/models/stats.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/services/manager.py` & `wc-django-notifications-0.3.1/wcd_notifications/services/manager.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/services/notifier.py` & `wc-django-notifications-0.3.1/wcd_notifications/services/notifier.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.3.0/wcd_notifications/utils.py` & `wc-django-notifications-0.3.1/wcd_notifications/utils.py`

 * *Files identical despite different names*

