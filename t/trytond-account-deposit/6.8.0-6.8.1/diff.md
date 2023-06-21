# Comparing `tmp/trytond_account_deposit-6.8.0.tar.gz` & `tmp/trytond_account_deposit-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_deposit-6.8.0.tar", last modified: Mon May  1 11:52:37 2023, max compression
+gzip compressed data, was "trytond_account_deposit-6.8.1.tar", last modified: Wed Jun 21 17:20:40 2023, max compression
```

## Comparing `trytond_account_deposit-6.8.0.tar` & `trytond_account_deposit-6.8.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-05-01 11:08:32.000000 trytond_account_deposit-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:08:32.000000 trytond_account_deposit-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1762 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2495 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.290618 trytond_account_deposit-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5174 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1567 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.283951 trytond_account_deposit-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1928 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1895 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1700 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2003 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1905 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1630 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1575 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1631 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1707 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1655 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1671 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1627 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1593 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2081 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5917 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4449 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.287284 trytond_account_deposit-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2971 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/tests/scenario_deposit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3367 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/tests/scenario_deposit_second_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      648 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-05-01 11:08:25.000000 trytond_account_deposit-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-05-01 11:52:37.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.290618 trytond_account_deposit-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/move_line_list_deposit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/recall_deposit_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.188619 trytond_account_deposit-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1897 2023-06-21 17:20:36.000000 trytond_account_deposit-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-06-21 17:20:36.000000 trytond_account_deposit-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-06-21 17:20:40.188619 trytond_account_deposit-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1765 2023-06-10 09:44:41.000000 trytond_account_deposit-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2495 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.185286 trytond_account_deposit-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5174 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1567 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.178619 trytond_account_deposit-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1928 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1895 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1700 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2003 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1905 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1630 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1575 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1631 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1707 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1655 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1671 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1627 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1593 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2081 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5917 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:20:40.188619 trytond_account_deposit-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4449 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.181953 trytond_account_deposit-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2971 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/scenario_deposit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3367 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/scenario_deposit_second_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      648 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-05-01 12:18:02.000000 trytond_account_deposit-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.185286 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-06-21 17:20:39.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-06-21 17:20:40.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:20:39.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-06-21 17:20:39.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:20.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-06-21 17:20:39.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:20:39.000000 trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:20:40.181953 trytond_account_deposit-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/move_line_list_deposit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-05-01 12:17:30.000000 trytond_account_deposit-6.8.1/view/recall_deposit_form.xml
```

### Comparing `trytond_account_deposit-6.8.0/CHANGELOG` & `trytond_account_deposit-6.8.1/CHANGELOG`

 * *Files 5% similar despite different names*

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
 * Support deposit in second currency
 * Remove support for Python 3.7
 * Add support for Python 3.11
```

### Comparing `trytond_account_deposit-6.8.0/COPYRIGHT` & `trytond_account_deposit-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/LICENSE` & `trytond_account_deposit-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/PKG-INFO` & `trytond_account_deposit-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_deposit
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for accounting deposit
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_deposit-6.8.0/__init__.py` & `trytond_account_deposit-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/account.py` & `trytond_account_deposit-6.8.1/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 
 class Reconcile(metaclass=PoolMeta):
     __name__ = 'account.reconcile'
 
     def get_currencies(self, account, party, currency=None, _balanced=False):
         if account.type.deposit:
             _balanced = True
-        return super().get_parties(
+        return super().get_currencies(
             account, party, currency=None, _balanced=_balanced)
```

### Comparing `trytond_account_deposit-6.8.0/account.xml` & `trytond_account_deposit-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/doc/conf.py` & `trytond_account_deposit-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/invoice.py` & `trytond_account_deposit-6.8.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/invoice.xml` & `trytond_account_deposit-6.8.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/bg.po` & `trytond_account_deposit-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/ca.po` & `trytond_account_deposit-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/cs.po` & `trytond_account_deposit-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/de.po` & `trytond_account_deposit-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/es.po` & `trytond_account_deposit-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/es_419.po` & `trytond_account_deposit-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/et.po` & `trytond_account_deposit-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/fa.po` & `trytond_account_deposit-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/fi.po` & `trytond_account_deposit-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/fr.po` & `trytond_account_deposit-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/hu.po` & `trytond_account_deposit-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/id.po` & `trytond_account_deposit-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/it.po` & `trytond_account_deposit-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/lo.po` & `trytond_account_deposit-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/lt.po` & `trytond_account_deposit-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/nl.po` & `trytond_account_deposit-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/pl.po` & `trytond_account_deposit-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/pt.po` & `trytond_account_deposit-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/ro.po` & `trytond_account_deposit-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/ru.po` & `trytond_account_deposit-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/sl.po` & `trytond_account_deposit-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/tr.po` & `trytond_account_deposit-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/uk.po` & `trytond_account_deposit-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/locale/zh_CN.po` & `trytond_account_deposit-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/message.xml` & `trytond_account_deposit-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart.xml` & `trytond_account_deposit-6.8.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_bg.xml` & `trytond_account_deposit-6.8.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_ca.xml` & `trytond_account_deposit-6.8.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_de.xml` & `trytond_account_deposit-6.8.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_en.xml` & `trytond_account_deposit-6.8.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_es.xml` & `trytond_account_deposit-6.8.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_fr.xml` & `trytond_account_deposit-6.8.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_nl.xml` & `trytond_account_deposit-6.8.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_pt.xml` & `trytond_account_deposit-6.8.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_ru.xml` & `trytond_account_deposit-6.8.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/minimal_chart_sl.xml` & `trytond_account_deposit-6.8.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/party.py` & `trytond_account_deposit-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/party.xml` & `trytond_account_deposit-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/setup.py` & `trytond_account_deposit-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/tests/scenario_deposit.rst` & `trytond_account_deposit-6.8.1/tests/scenario_deposit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/tests/scenario_deposit_second_currency.rst` & `trytond_account_deposit-6.8.1/tests/scenario_deposit_second_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/tests/tools.py` & `trytond_account_deposit-6.8.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/tox.ini` & `trytond_account_deposit-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/PKG-INFO` & `trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-deposit
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for accounting deposit
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/SOURCES.txt` & `trytond_account_deposit-6.8.1/trytond_account_deposit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

