# Comparing `tmp/trytond_currency-6.8.0.tar.gz` & `tmp/trytond_currency-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency-6.8.0.tar", last modified: Mon May  1 11:37:17 2023, max compression
+gzip compressed data, was "trytond_currency-6.8.1.tar", last modified: Wed Jun 21 17:16:50 2023, max compression
```

## Comparing `trytond_currency-6.8.0.tar` & `trytond_currency-6.8.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3753 2023-05-01 10:58:17.000000 trytond_currency-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 10:58:17.000000 trytond_currency-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15851 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6572 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.299201 trytond_currency-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-21 08:36:08.000000 trytond_currency-6.8.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/ecb.py
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.299201 trytond_currency-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/icons/tryton-currency.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.292534 trytond_currency-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5977 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4810 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5914 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5185 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5949 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5901 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5480 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5615 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5369 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5853 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5806 2023-04-30 10:46:36.000000 trytond_currency-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5015 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6453 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5390 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/message.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.292534 trytond_currency-6.8.0/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3316 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/scripts/import_currencies.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4760 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.295868 trytond_currency-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_compute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_rate_update.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14824 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-05-01 10:58:12.000000 trytond_currency-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/trytond_currency.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-05-01 11:37:17.000000 trytond_currency-6.8.0/trytond_currency.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_currency-6.8.0/trytond_currency.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.295868 trytond_currency-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_rate_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/currency_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/currency_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.308967 trytond_currency-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3854 2023-06-21 17:16:47.000000 trytond_currency-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-06-21 17:16:47.000000 trytond_currency-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-06-21 17:16:50.308967 trytond_currency-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15851 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6572 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.302300 trytond_currency-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/ecb.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.305634 trytond_currency-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/icons/tryton-currency.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.292300 trytond_currency-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5012 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5977 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4810 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5914 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5185 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5949 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5901 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5480 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5615 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5369 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5853 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5806 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5015 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6453 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5390 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/message.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.292300 trytond_currency-6.8.1/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3316 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/scripts/import_currencies.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:16:50.308967 trytond_currency-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4760 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.295633 trytond_currency-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/scenario_currency_compute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/scenario_currency_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/scenario_currency_rate_update.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14824 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-05-01 12:18:02.000000 trytond_currency-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.308967 trytond_currency-6.8.1/trytond_currency.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-06-21 17:16:49.000000 trytond_currency-6.8.1/trytond_currency.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-06-21 17:16:50.000000 trytond_currency-6.8.1/trytond_currency.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:16:49.000000 trytond_currency-6.8.1/trytond_currency.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-06-21 17:16:49.000000 trytond_currency-6.8.1/trytond_currency.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:15.000000 trytond_currency-6.8.1/trytond_currency.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-06-21 17:16:49.000000 trytond_currency-6.8.1/trytond_currency.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:16:49.000000 trytond_currency-6.8.1/trytond_currency.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:50.298967 trytond_currency-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-06-10 09:41:43.000000 trytond_currency-6.8.1/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/currency_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/currency_rate_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/currency_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-05-01 12:17:31.000000 trytond_currency-6.8.1/view/currency_tree.xml
```

### Comparing `trytond_currency-6.8.0/CHANGELOG` & `trytond_currency-6.8.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.1 - 2023-06-21
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Make symbol of currency optional
 * Remove support for Python 3.7
 * Add support for Python 3.11
 * Allow rounding with opposite method
```

### Comparing `trytond_currency-6.8.0/COPYRIGHT` & `trytond_currency-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/LICENSE` & `trytond_currency-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/PKG-INFO` & `trytond_currency-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-6.8.0/currency.py` & `trytond_currency-6.8.1/currency.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/currency.xml` & `trytond_currency-6.8.1/currency.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/doc/conf.py` & `trytond_currency-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/doc/configuration.rst` & `trytond_currency-6.8.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/doc/design.rst` & `trytond_currency-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/doc/usage.rst` & `trytond_currency-6.8.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/ecb.py` & `trytond_currency-6.8.1/ecb.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/fields.py` & `trytond_currency-6.8.1/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/icons/LICENSE` & `trytond_currency-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/ir.py` & `trytond_currency-6.8.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/bg.po` & `trytond_currency-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/ca.po` & `trytond_currency-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/cs.po` & `trytond_currency-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/de.po` & `trytond_currency-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/es.po` & `trytond_currency-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/es_419.po` & `trytond_currency-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/et.po` & `trytond_currency-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/fa.po` & `trytond_currency-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/fi.po` & `trytond_currency-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/fr.po` & `trytond_currency-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/hu.po` & `trytond_currency-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/id.po` & `trytond_currency-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/it.po` & `trytond_currency-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/lo.po` & `trytond_currency-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/lt.po` & `trytond_currency-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/nl.po` & `trytond_currency-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/pl.po` & `trytond_currency-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/pt.po` & `trytond_currency-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/ro.po` & `trytond_currency-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/ru.po` & `trytond_currency-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/sl.po` & `trytond_currency-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/tr.po` & `trytond_currency-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/uk.po` & `trytond_currency-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/locale/zh_CN.po` & `trytond_currency-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/message.xml` & `trytond_currency-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/scripts/import_currencies.py` & `trytond_currency-6.8.1/scripts/import_currencies.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/setup.py` & `trytond_currency-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/tests/scenario_currency_compute.rst` & `trytond_currency-6.8.1/tests/scenario_currency_compute.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/tests/scenario_currency_rate_update.rst` & `trytond_currency-6.8.1/tests/scenario_currency_rate_update.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/tests/test_module.py` & `trytond_currency-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/tests/tools.py` & `trytond_currency-6.8.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/tox.ini` & `trytond_currency-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/trytond_currency.egg-info/PKG-INFO` & `trytond_currency-6.8.1/trytond_currency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-currency
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-6.8.0/trytond_currency.egg-info/SOURCES.txt` & `trytond_currency-6.8.1/trytond_currency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.8.0/view/cron_form.xml` & `trytond_currency-6.8.1/view/cron_form.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_currency-6.8.0/view/cron_form.xml` & `trytond_currency-6.8.1/view/cron_form.xml`

```diff
@@ -4,15 +4,15 @@
 <form>
   <label name="source"/>
   <field name="source"/>
   <label name="frequency"/>
   <group id="frequency" col="-1">
     <field name="frequency"/>
     <label name="weekday"/>
-    <field name="weekday"/>
+    <field name="weekday" widget="selection"/>
     <label name="day"/>
     <field name="day"/>
   </group>
   <label name="currency"/>
   <field name="currency"/>
   <label name="last_update"/>
   <group id="run">
```

### Comparing `trytond_currency-6.8.0/view/currency_form.xml` & `trytond_currency-6.8.1/view/currency_form.xml`

 * *Files identical despite different names*

