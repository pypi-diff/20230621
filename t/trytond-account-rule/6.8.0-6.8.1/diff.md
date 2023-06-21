# Comparing `tmp/trytond_account_rule-6.8.0.tar.gz` & `tmp/trytond_account_rule-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_rule-6.8.0.tar", last modified: Mon May  1 11:53:06 2023, max compression
+gzip compressed data, was "trytond_account_rule-6.8.1.tar", last modified: Wed Jun 21 17:18:26 2023, max compression
```

## Comparing `trytond_account_rule-6.8.0.tar` & `trytond_account_rule-6.8.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.610981 trytond_account_rule-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      497 2023-05-01 11:08:52.000000 trytond_account_rule-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:08:52.000000 trytond_account_rule-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2435 2023-05-01 11:53:06.610981 trytond_account_rule-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5523 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3756 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.607648 trytond_account_rule-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.604315 trytond_account_rule-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1855 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1635 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1648 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1851 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-04-29 08:02:46.000000 trytond_account_rule-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:06.610981 trytond_account_rule-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5127 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.607648 trytond_account_rule-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/tests/scenario_account_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-05-01 11:08:47.000000 trytond_account_rule-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.610981 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2435 2023-05-01 11:53:05.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2023-05-01 11:53:06.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:05.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-01 11:53:05.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-05-01 11:53:05.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:05.000000 trytond_account_rule-6.8.0/trytond_account_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:06.607648 trytond_account_rule-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/view/account_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/view/account_rule_form_stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/view/account_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_account_rule-6.8.0/view/account_rule_list_stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.776901 trytond_account_rule-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-06-21 17:18:23.000000 trytond_account_rule-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-06-21 17:18:23.000000 trytond_account_rule-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2023-06-21 17:18:26.776901 trytond_account_rule-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5523 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3756 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.773567 trytond_account_rule-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.763567 trytond_account_rule-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1864 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1855 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1635 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1648 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1851 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-06-10 09:43:13.000000 trytond_account_rule-6.8.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-06-10 09:43:13.000000 trytond_account_rule-6.8.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:18:26.776901 trytond_account_rule-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5127 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.766900 trytond_account_rule-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3186 2023-06-10 09:43:13.000000 trytond_account_rule-6.8.1/tests/scenario_account_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-05-01 12:18:02.000000 trytond_account_rule-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.776901 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1772 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:20.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:18:26.000000 trytond_account_rule-6.8.1/trytond_account_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:18:26.770234 trytond_account_rule-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/view/account_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/view/account_rule_form_stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/view/account_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:30.000000 trytond_account_rule-6.8.1/view/account_rule_list_stock.xml
```

### Comparing `trytond_account_rule-6.8.0/COPYRIGHT` & `trytond_account_rule-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/LICENSE` & `trytond_account_rule-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/PKG-INFO` & `trytond_account_rule-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_rule
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to change account used with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_rule-6.8.0/__init__.py` & `trytond_account_rule-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/account.py` & `trytond_account_rule-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/account.xml` & `trytond_account_rule-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/doc/conf.py` & `trytond_account_rule-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/doc/design.rst` & `trytond_account_rule-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/bg.po` & `trytond_account_rule-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/ca.po` & `trytond_account_rule-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/cs.po` & `trytond_account_rule-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/de.po` & `trytond_account_rule-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/es.po` & `trytond_account_rule-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/es_419.po` & `trytond_account_rule-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/et.po` & `trytond_account_rule-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/fa.po` & `trytond_account_rule-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/fi.po` & `trytond_account_rule-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/fr.po` & `trytond_account_rule-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/hu.po` & `trytond_account_rule-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/id.po` & `trytond_account_rule-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/it.po` & `trytond_account_rule-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/lo.po` & `trytond_account_rule-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/lt.po` & `trytond_account_rule-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/nl.po` & `trytond_account_rule-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/pl.po` & `trytond_account_rule-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/pt.po` & `trytond_account_rule-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/ro.po` & `trytond_account_rule-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/ru.po` & `trytond_account_rule-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/sl.po` & `trytond_account_rule-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/tr.po` & `trytond_account_rule-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/uk.po` & `trytond_account_rule-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/locale/zh_CN.po` & `trytond_account_rule-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/party.py` & `trytond_account_rule-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/product.py` & `trytond_account_rule-6.8.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/setup.py` & `trytond_account_rule-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/stock.py` & `trytond_account_rule-6.8.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/tests/scenario_account_rule.rst` & `trytond_account_rule-6.8.1/tests/scenario_account_rule.rst`

 * *Files 9% similar despite different names*

```diff
@@ -91,14 +91,17 @@
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.taxes.append(Tax(tax.id))
     >>> line.quantity = 2
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.quantity = -1
+    >>> line = sale.lines.new()
+    >>> line.type = 'comment'
+    >>> line.description = 'Sample'
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
 
     >>> invoice, = sale.invoices
     >>> invoice.lines[0].account == account_revenue1
```

### Comparing `trytond_account_rule-6.8.0/tests/test_module.py` & `trytond_account_rule-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/tox.ini` & `trytond_account_rule-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/trytond_account_rule.egg-info/PKG-INFO` & `trytond_account_rule-6.8.1/trytond_account_rule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-rule
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to change account used with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_rule-6.8.0/trytond_account_rule.egg-info/SOURCES.txt` & `trytond_account_rule-6.8.1/trytond_account_rule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/view/account_rule_form.xml` & `trytond_account_rule-6.8.1/view/account_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-6.8.0/view/account_rule_list.xml` & `trytond_account_rule-6.8.1/view/account_rule_list.xml`

 * *Files identical despite different names*

