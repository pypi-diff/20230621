# Comparing `tmp/trytond_sale_supply-6.8.0.tar.gz` & `tmp/trytond_sale_supply-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply-6.8.0.tar", last modified: Mon May  1 11:47:47 2023, max compression
+gzip compressed data, was "trytond_sale_supply-6.8.1.tar", last modified: Wed Jun 21 17:14:33 2023, max compression
```

## Comparing `trytond_sale_supply-6.8.0.tar` & `trytond_sale_supply-6.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2103 2023-05-01 11:05:13.000000 trytond_sale_supply-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:05:13.000000 trytond_sale_supply-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.187018 trytond_sale_supply-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2629 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3494 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11814 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3849 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3356 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_stock_first.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-05-01 11:05:07.000000 trytond_sale_supply-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-05-01 11:47:47.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2204 2023-06-21 17:14:30.000000 trytond_sale_supply-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-06-21 17:14:29.000000 trytond_sale_supply-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.137121 trytond_sale_supply-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3438 2023-06-10 09:48:45.000000 trytond_sale_supply-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3494 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11814 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3849 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3356 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-05-01 12:18:02.000000 trytond_sale_supply-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-06-21 17:14:33.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:18.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/view/template_form.xml
```

### Comparing `trytond_sale_supply-6.8.0/CHANGELOG` & `trytond_sale_supply-6.8.1/CHANGELOG`

 * *Files 2% similar despite different names*

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
 * Add stock_first option to supply_on_sale
 * Change supply_on_sale into selection
 * Remove support for Python 3.7
 * Add support for Python 3.11
```

### Comparing `trytond_sale_supply-6.8.0/COPYRIGHT` & `trytond_sale_supply-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/LICENSE` & `trytond_sale_supply-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/PKG-INFO` & `trytond_sale_supply-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-6.8.0/README.rst` & `trytond_sale_supply-6.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/__init__.py` & `trytond_sale_supply-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/doc/conf.py` & `trytond_sale_supply-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/doc/index.rst` & `trytond_sale_supply-6.8.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/bg.po` & `trytond_sale_supply-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/ca.po` & `trytond_sale_supply-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/cs.po` & `trytond_sale_supply-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/de.po` & `trytond_sale_supply-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/es.po` & `trytond_sale_supply-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/es_419.po` & `trytond_sale_supply-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/et.po` & `trytond_sale_supply-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/fa.po` & `trytond_sale_supply-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/fi.po` & `trytond_sale_supply-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/fr.po` & `trytond_sale_supply-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/hu.po` & `trytond_sale_supply-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/id.po` & `trytond_sale_supply-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/it.po` & `trytond_sale_supply-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/lo.po` & `trytond_sale_supply-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/lt.po` & `trytond_sale_supply-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/nl.po` & `trytond_sale_supply-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/pl.po` & `trytond_sale_supply-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/pt.po` & `trytond_sale_supply-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/ro.po` & `trytond_sale_supply-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/ru.po` & `trytond_sale_supply-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/sl.po` & `trytond_sale_supply-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/tr.po` & `trytond_sale_supply-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/uk.po` & `trytond_sale_supply-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/locale/zh_CN.po` & `trytond_sale_supply-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/message.xml` & `trytond_sale_supply-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/product.py` & `trytond_sale_supply-6.8.1/stock.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-
-from sql import Literal
+from collections import defaultdict
 
 from trytond.i18n import gettext
-from trytond.model import fields
+from trytond.model import Model, ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval
-from trytond.transaction import Transaction
-
 
-class Template(metaclass=PoolMeta):
-    __name__ = 'product.template'
 
-    supply_on_sale = fields.Selection([
-            (None, "Never"),
-            ('stock_first', "Stock First"),
-            ('always', "Always"),
-            ], "Supply On Sale",
-        states={
-            'invisible': ~Eval('purchasable') | ~Eval('salable'),
-            })
+class ShipmentIn(metaclass=PoolMeta):
+    __name__ = 'stock.shipment.in'
 
     @classmethod
-    def __resgister__(cls, module):
-        table_h = cls.__table_handler__(module)
-        table = cls.__table__()
-        cursor = Transaction().connection.cursor()
-
-        migrate_supply_on_sale = table_h.column_is_type(
-            'supply_on_sale', 'BOOL')
-        if migrate_supply_on_sale:
-            table_h.column_rename('supply_on_sale', '_temp_supply_on_sale')
-
-        super().__register__(module)
-
-        # Migration from 6.6: convert supply_on_sale from boolean to selection
-        if migrate_supply_on_sale:
-            cursor.execute(*table.update(
-                    [table.supply_on_sale],
-                    ['always'],
-                    where=table._temp_supply_on_sale == Literal(True)))
-            table_h.drop_column('_temp_supply_on_sale')
+    @ModelView.button
+    @Workflow.transition('done')
+    def done(cls, shipments):
+        super(ShipmentIn, cls).done(shipments)
+
+        # Assigned sale move lines
+        for shipment in shipments:
+            shipment.assign_supplied()
+
+    def assign_supplied(self, grouping=('product',), filter_=None):
+        pool = Pool()
+        SaleLine = pool.get('sale.line')
+
+        def filter_func(move):
+            if filter_ is None:
+                return True
+            for fieldname, values in filter_:
+                value = getattr(move, fieldname)
+                if isinstance(value, Model):
+                    value = value.id
+                if value not in values:
+                    return False
+
+        def get_key(move):
+            key = (move.to_location.id,)
+            for field in grouping:
+                value = getattr(move, field)
+                if isinstance(value, Model):
+                    value = value.id
+                key += (value,)
+            return key
+        move_ids = [m.id for m in filter(filter_func, self.incoming_moves)]
+        sale_lines = SaleLine.search([
+                ('purchase_request.purchase_line.moves', 'in', move_ids),
+                ('purchase_request.origin', 'like', 'sale.sale,%'),
+                ])
+        pbl = defaultdict(lambda: defaultdict(int))
+        if self.warehouse_storage == self.warehouse_input:
+            inventory_moves = self.incoming_moves
+        else:
+            inventory_moves = self.inventory_moves
+        for move in filter(filter_func, inventory_moves):
+            pbl[move.product][get_key(move)] += move.internal_quantity
+        for sale_line in sale_lines:
+            sale_line.assign_supplied(
+                pbl[sale_line.product], grouping=grouping)
 
-    @fields.depends(methods=['_notify_order_point'])
+
+class OrderPoint(metaclass=PoolMeta):
+    __name__ = 'stock.order_point'
+
+    @fields.depends(methods=['_notify_product_supply_on_sale'])
     def on_change_notify(self):
         notifications = super().on_change_notify()
-        notifications.extend(self._notify_order_point())
+        notifications.extend(self._notify_product_supply_on_sale())
         return notifications
 
-    @fields.depends('id', 'supply_on_sale')
-    def _notify_order_point(self):
-        pool = Pool()
-        try:
-            OrderPoint = pool.get('stock.order_point')
-        except KeyError:
-            return
-        if self.supply_on_sale and self.id is not None and self.id >= 0:
-            order_points = OrderPoint.search([
-                    ('product.template.id', '=', self.id),
-                    ('type', '=', 'purchase'),
-                    ], limit=6)
-            if order_points:
-                names = ', '.join(o.rec_name for o in order_points[:5])
-                if len(order_points) > 5:
-                    names + '...'
-                yield ('warning', gettext(
-                        'sale_supply'
-                        '.msg_template_supply_on_sale_order_point',
-                        order_points=names))
-
-
-class Product(metaclass=PoolMeta):
-    __name__ = 'product.product'
+    @fields.depends('type', 'product')
+    def _notify_product_supply_on_sale(self):
+        if (self.type == 'purchase'
+                and self.product and self.product.supply_on_sale):
+            yield ('warning', gettext(
+                    'sale_supply'
+                    '.msg_order_point_product_supply_on_sale',
+                    product=self.product.rec_name))
```

### Comparing `trytond_sale_supply-6.8.0/purchase.py` & `trytond_sale_supply-6.8.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/sale.py` & `trytond_sale_supply-6.8.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/sale.xml` & `trytond_sale_supply-6.8.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/setup.py` & `trytond_sale_supply-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/tests/scenario_sale_supply.rst` & `trytond_sale_supply-6.8.1/tests/scenario_sale_supply.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/tests/scenario_sale_supply_notifications.rst` & `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/tests/scenario_sale_supply_shipment_on_invoice.rst` & `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_shipment_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/tests/scenario_sale_supply_stock_first.rst` & `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_stock_first.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/tox.ini` & `trytond_sale_supply-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/PKG-INFO` & `trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-sale-supply
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/SOURCES.txt` & `trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

