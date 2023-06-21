# Comparing `tmp/trytond_purchase-6.8.1.tar.gz` & `tmp/trytond_purchase-6.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-6.8.1.tar", last modified: Wed May 17 20:47:59 2023, max compression
+gzip compressed data, was "trytond_purchase-6.8.2.tar", last modified: Wed Jun 21 17:16:16 2023, max compression
```

## Comparing `trytond_purchase-6.8.1.tar` & `trytond_purchase-6.8.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     6684 2023-05-17 20:47:56.000000 trytond_purchase-6.8.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-17 20:47:55.000000 trytond_purchase-6.8.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.507377 trytond_purchase-6.8.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.514043 trytond_purchase-6.8.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/prepurchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4855 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.514043 trytond_purchase-6.8.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.397375 trytond_purchase-6.8.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37513 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32682 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38008 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37693 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32179 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34342 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39508 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32669 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37860 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36612 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33346 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37467 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35472 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37911 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33939 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35630 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31956 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37996 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35318 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32660 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30987 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35757 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    82961 2023-05-13 22:06:18.000000 trytond_purchase-6.8.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    32163 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11720 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9634 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.424042 trytond_purchase-6.8.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19171 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3009 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3025 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-05-01 12:18:02.000000 trytond_purchase-6.8.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.524043 trytond_purchase-6.8.1/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4760 2023-05-17 20:47:59.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.504043 trytond_purchase-6.8.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.568490 trytond_purchase-6.8.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6785 2023-06-21 17:16:13.000000 trytond_purchase-6.8.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-06-21 17:16:13.000000 trytond_purchase-6.8.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-06-21 17:16:16.565157 trytond_purchase-6.8.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.551823 trytond_purchase-6.8.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.555156 trytond_purchase-6.8.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/usage/prepurchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4855 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.558490 trytond_purchase-6.8.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.508488 trytond_purchase-6.8.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37513 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32682 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38008 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37693 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32179 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34342 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39508 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32669 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37860 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36612 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33346 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37467 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35472 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37911 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33939 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35630 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31956 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37996 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35318 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32660 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30987 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35757 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    82962 2023-06-10 09:50:05.000000 trytond_purchase-6.8.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32163 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11720 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:16:16.568490 trytond_purchase-6.8.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9634 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.515155 trytond_purchase-6.8.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19171 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1676 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3009 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3025 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-05-17 20:48:08.000000 trytond_purchase-6.8.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.565157 trytond_purchase-6.8.2/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-06-21 17:16:15.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4760 2023-06-21 17:16:16.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:16:15.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-06-21 17:16:15.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:58.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-06-21 17:16:15.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:16:15.000000 trytond_purchase-6.8.2/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:16:16.548489 trytond_purchase-6.8.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_purchase-6.8.2/view/template_tree.xml
```

### Comparing `trytond_purchase-6.8.1/CHANGELOG` & `trytond_purchase-6.8.2/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.2 - 2023-06-21
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.1 - 2023-05-17
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_purchase-6.8.1/COPYRIGHT` & `trytond_purchase-6.8.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/LICENSE` & `trytond_purchase-6.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/PKG-INFO` & `trytond_purchase-6.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-6.8.1/__init__.py` & `trytond_purchase-6.8.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/configuration.py` & `trytond_purchase-6.8.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/configuration.xml` & `trytond_purchase-6.8.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/doc/conf.py` & `trytond_purchase-6.8.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/doc/design.rst` & `trytond_purchase-6.8.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/doc/usage/prepurchase.rst` & `trytond_purchase-6.8.2/doc/usage/prepurchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/doc/usage/process.rst` & `trytond_purchase-6.8.2/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/doc/usage/returns.rst` & `trytond_purchase-6.8.2/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/icons/LICENSE` & `trytond_purchase-6.8.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/invoice.py` & `trytond_purchase-6.8.2/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/invoice.xml` & `trytond_purchase-6.8.2/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/bg.po` & `trytond_purchase-6.8.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/ca.po` & `trytond_purchase-6.8.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/cs.po` & `trytond_purchase-6.8.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/de.po` & `trytond_purchase-6.8.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/es.po` & `trytond_purchase-6.8.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/es_419.po` & `trytond_purchase-6.8.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/et.po` & `trytond_purchase-6.8.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/fa.po` & `trytond_purchase-6.8.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/fi.po` & `trytond_purchase-6.8.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/fr.po` & `trytond_purchase-6.8.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/hu.po` & `trytond_purchase-6.8.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/id.po` & `trytond_purchase-6.8.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/it.po` & `trytond_purchase-6.8.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/lo.po` & `trytond_purchase-6.8.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/lt.po` & `trytond_purchase-6.8.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/nl.po` & `trytond_purchase-6.8.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/pl.po` & `trytond_purchase-6.8.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/pt.po` & `trytond_purchase-6.8.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/ro.po` & `trytond_purchase-6.8.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/ru.po` & `trytond_purchase-6.8.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/sl.po` & `trytond_purchase-6.8.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/tr.po` & `trytond_purchase-6.8.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/uk.po` & `trytond_purchase-6.8.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/locale/zh_CN.po` & `trytond_purchase-6.8.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/message.xml` & `trytond_purchase-6.8.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/party.py` & `trytond_purchase-6.8.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/party.xml` & `trytond_purchase-6.8.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/product.py` & `trytond_purchase-6.8.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/product.xml` & `trytond_purchase-6.8.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/purchase.fodt` & `trytond_purchase-6.8.2/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/purchase.py` & `trytond_purchase-6.8.2/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1249,15 +1249,15 @@
                     | ~Eval('delivery_date_edit', False)),
                 }),
         'on_change_with_delivery_date', setter='set_delivery_date')
     delivery_date_edit = fields.Boolean(
         "Edit Delivery Date",
         domain=[
             If(Eval('type') != 'line',
-                ('delivery_date_edit', '=', None),
+                ('delivery_date_edit', '=', False),
                 ()),
             ],
         states={
             'invisible': (
                 (Eval('type') != 'line')
                 | Eval('purchase_state').in_(
                     ['processing', 'done', 'cancelled'])),
```

### Comparing `trytond_purchase-6.8.1/purchase.xml` & `trytond_purchase-6.8.2/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/purchase_reporting.py` & `trytond_purchase-6.8.2/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/purchase_reporting.xml` & `trytond_purchase-6.8.2/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/setup.py` & `trytond_purchase-6.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/stock.py` & `trytond_purchase-6.8.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/stock.xml` & `trytond_purchase-6.8.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase_empty.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase_reporting.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-6.8.2/tests/scenario_purchase_return_wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tests/test_module.py` & `trytond_purchase-6.8.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/tox.ini` & `trytond_purchase-6.8.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-6.8.2/trytond_purchase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-purchase
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-6.8.1/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-6.8.2/trytond_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/party_form.xml` & `trytond_purchase-6.8.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/product_supplier_form.xml` & `trytond_purchase-6.8.2/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_form.xml` & `trytond_purchase-6.8.2/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_line_form.xml` & `trytond_purchase-6.8.2/view/purchase_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_line_tree.xml` & `trytond_purchase-6.8.2/view/purchase_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_line_tree_sequence.xml` & `trytond_purchase-6.8.2/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_reporting_context_form.xml` & `trytond_purchase-6.8.2/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/purchase_tree.xml` & `trytond_purchase-6.8.2/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.1/view/template_form.xml` & `trytond_purchase-6.8.2/view/template_form.xml`

 * *Files identical despite different names*

