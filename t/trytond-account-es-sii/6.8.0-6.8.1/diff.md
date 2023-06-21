# Comparing `tmp/trytond_account_es_sii-6.8.0.tar.gz` & `tmp/trytond_account_es_sii-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es_sii-6.8.0.tar", last modified: Mon May  1 11:42:26 2023, max compression
+gzip compressed data, was "trytond_account_es_sii-6.8.1.tar", last modified: Wed Jun 21 17:19:37 2023, max compression
```

## Comparing `trytond_account_es_sii-6.8.0.tar` & `trytond_account_es_sii-6.8.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-05-01 11:01:46.000000 trytond_account_es_sii-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 11:01:45.000000 trytond_account_es_sii-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23865 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5887 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.029699 trytond_account_es_sii-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1085 2023-04-30 10:46:36.000000 trytond_account_es_sii-6.8.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.026365 trytond_account_es_sii-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5430 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5476 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5566 2023-04-30 10:46:36.000000 trytond_account_es_sii-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4430 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5484 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4582 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12629 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.026365 trytond_account_es_sii-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2039 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    21334 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-05-01 11:01:40.000000 trytond_account_es_sii-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1938 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.029699 trytond_account_es_sii-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/invoice_sii_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/invoice_sii_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/tax_template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.717815 trytond_account_es_sii-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-06-21 17:19:34.000000 trytond_account_es_sii-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-06-21 17:19:34.000000 trytond_account_es_sii-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-06-21 17:19:37.717815 trytond_account_es_sii-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23869 2023-06-10 09:34:27.000000 trytond_account_es_sii-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5887 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.714481 trytond_account_es_sii-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1085 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.704481 trytond_account_es_sii-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5430 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5476 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5566 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4430 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5484 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:19:37.717815 trytond_account_es_sii-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4582 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12629 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.707814 trytond_account_es_sii-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2039 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    22155 2023-06-10 09:34:27.000000 trytond_account_es_sii-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-05-01 12:18:02.000000 trytond_account_es_sii-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.717815 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1938 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:17.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:19:37.000000 trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:19:37.711148 trytond_account_es_sii-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/invoice_sii_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/invoice_sii_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-05-01 12:17:30.000000 trytond_account_es_sii-6.8.1/view/tax_template_form.xml
```

### Comparing `trytond_account_es_sii-6.8.0/COPYRIGHT` & `trytond_account_es_sii-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/LICENSE` & `trytond_account_es_sii-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/PKG-INFO` & `trytond_account_es_sii-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_es_sii
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module that sends invoices to the Spanish SII webservice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es_sii-6.8.0/__init__.py` & `trytond_account_es_sii-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/account.py` & `trytond_account_es_sii-6.8.1/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 SII_URL = [
     (None, ""),
     ('aeat', "AEAT"),
     ('guipuzkoa', "Guipuzkoa"),
     # XXX: URLs for basque country and navarra should be added
     ]
 WS_URL = {
-    'aeat': ('https://www2.agenciatributaria.gob.es/static_files/'
-        'common/internet/dep/aplicaciones/es/aeat/ssii_1_1/fact/ws/'),
+    'aeat': ('https://www2.agenciatributaria.gob.es/static_files/common/'
+        'internet/dep/aplicaciones/es/aeat/ssii_1_1_bis/fact/ws/'),
     'guipuzkoa': (
         'https://egoitza.gipuzkoa.eus/ogasuna/sii/ficheros/v1.1/'),
     }
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'account.configuration'
```

### Comparing `trytond_account_es_sii-6.8.0/account.xml` & `trytond_account_es_sii-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/doc/conf.py` & `trytond_account_es_sii-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/doc/configuration.rst` & `trytond_account_es_sii-6.8.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/doc/design.rst` & `trytond_account_es_sii-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/bg.po` & `trytond_account_es_sii-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/ca.po` & `trytond_account_es_sii-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/cs.po` & `trytond_account_es_sii-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/de.po` & `trytond_account_es_sii-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/es.po` & `trytond_account_es_sii-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/es_419.po` & `trytond_account_es_sii-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/et.po` & `trytond_account_es_sii-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/fa.po` & `trytond_account_es_sii-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/fi.po` & `trytond_account_es_sii-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/fr.po` & `trytond_account_es_sii-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/hu.po` & `trytond_account_es_sii-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/id.po` & `trytond_account_es_sii-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/it.po` & `trytond_account_es_sii-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/lo.po` & `trytond_account_es_sii-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/lt.po` & `trytond_account_es_sii-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/nl.po` & `trytond_account_es_sii-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/pl.po` & `trytond_account_es_sii-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/pt.po` & `trytond_account_es_sii-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/ro.po` & `trytond_account_es_sii-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/ru.po` & `trytond_account_es_sii-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/sl.po` & `trytond_account_es_sii-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/tr.po` & `trytond_account_es_sii-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/uk.po` & `trytond_account_es_sii-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/locale/zh_CN.po` & `trytond_account_es_sii-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/message.xml` & `trytond_account_es_sii-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/party.py` & `trytond_account_es_sii-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/setup.py` & `trytond_account_es_sii-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/tax.xml` & `trytond_account_es_sii-6.8.1/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account_es_sii-6.8.1/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/tests/test_module.py` & `trytond_account_es_sii-6.8.1/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from decimal import Decimal
 
 from trytond.modules.account.tests import create_chart, get_fiscalyear
+from trytond.modules.account_es_sii.account import SII_URL
 from trytond.modules.account_invoice.tests import set_invoice_sequences
 from trytond.modules.company.tests import create_company, set_company
 from trytond.modules.currency.tests import add_currency_rate, create_currency
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 
 today = datetime.date.today()
@@ -523,9 +524,29 @@
                     ])
             self.assertTrue(tax.es_exclude_from_sii)
 
             sii_invoice = create_invoice('in', company, party, [tax])
 
             self.assertEqual(sii_invoice, [])
 
+    @with_transaction()
+    def test_get_client(self):
+        "Test client can be initialized for all environments"
+        pool = Pool()
+        Config = pool.get('account.configuration')
+        Credential = pool.get('account.credential.sii')
+
+        company = create_company()
+        with set_company(company):
+            config = Config(1)
+            for key, _ in SII_URL:
+                if not key:
+                    continue
+                for environment in ['staging', 'production']:
+                    config.es_sii_url = key
+                    config.es_sii_environment = environment
+                    config.save()
+                    client = Credential.get_client('SuministroFactEmitidas')
+                    self.assertTrue(client)
+
 
 del ModuleTestCase
```

### Comparing `trytond_account_es_sii-6.8.0/tox.ini` & `trytond_account_es_sii-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/PKG-INFO` & `trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-es-sii
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module that sends invoices to the Spanish SII webservice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/SOURCES.txt` & `trytond_account_es_sii-6.8.1/trytond_account_es_sii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/view/tax_form.xml` & `trytond_account_es_sii-6.8.1/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.8.0/view/tax_template_form.xml` & `trytond_account_es_sii-6.8.1/view/tax_template_form.xml`

 * *Files identical despite different names*

