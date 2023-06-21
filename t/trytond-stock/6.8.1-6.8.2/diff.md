# Comparing `tmp/trytond_stock-6.8.1.tar.gz` & `tmp/trytond_stock-6.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock-6.8.1.tar", last modified: Wed May 17 20:44:28 2023, max compression
+gzip compressed data, was "trytond_stock-6.8.2.tar", last modified: Wed Jun 21 17:11:56 2023, max compression
```

## Comparing `trytond_stock-6.8.1.tar` & `trytond_stock-6.8.2.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.538167 trytond_stock-6.8.1/
--rw-r--r--   0 ced       (1000) ced       (1000)    10448 2023-05-17 20:44:25.000000 trytond_stock-6.8.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-05-17 20:44:24.000000 trytond_stock-6.8.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-05-17 20:44:28.538167 trytond_stock-6.8.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2614 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9561 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    46098 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/customer_return_restocking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    48755 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/delivery_note.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.511500 trytond_stock-6.8.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/conf.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.518166 trytond_stock-6.8.1/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/location.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2037 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1102 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3305 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7779 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/design/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2311 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.524833 trytond_stock-6.8.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/usage/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4193 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/usage/quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4669 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/usage/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/doc/usage/value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      825 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.524833 trytond_stock-6.8.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/icons/tryton-shipment-in.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/icons/tryton-shipment-out.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/icons/tryton-stock.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    49542 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/internal_shipment.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    23444 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/inventory.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8965 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/inventory.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.414832 trytond_stock-6.8.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    91409 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96063 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82156 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98088 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96959 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81052 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89803 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102088 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82130 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97445 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92393 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    80321 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    84327 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89189 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86477 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96348 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85105 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87027 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93899 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    91532 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85855 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82049 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    77247 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90483 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    28636 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10457 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7746 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    68212 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8526 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6302 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4507 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6992 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6018 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45875 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/picking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    50018 2023-05-13 22:24:13.000000 trytond_stock-6.8.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22458 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:44:28.538167 trytond_stock-6.8.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   115590 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    53918 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2918 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23733 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    32870 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/stock_reporting_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45402 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/supplier_restocking_list.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.441499 trytond_stock-6.8.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8304 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7532 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3365 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_inventory_count.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2675 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_inventory_empty_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_move_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_product_quantities_by_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5199 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_recompute_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_recompute_average_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5077 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7934 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_reporting_margin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2376 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_in_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2441 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_in_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4539 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_internal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3350 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_internal_transit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8630 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2487 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_out_return_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2528 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/scenario_stock_shipment_out_same_storage_output.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    69197 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:18:02.000000 trytond_stock-6.8.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.531500 trytond_stock-6.8.1/trytond_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     9605 2023-05-17 20:44:28.000000 trytond_stock-6.8.1/trytond_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:44:27.000000 trytond_stock-6.8.1/trytond_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:44:28.504833 trytond_stock-6.8.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1128 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_count_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_count_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_line_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/inventory_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_quantity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/location_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/move_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/party_address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/party_address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/party_contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/party_contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      903 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/period_cache_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/period_cache_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_cost_price_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_cost_price_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_modify_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_quantities_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_quantities_warehouse_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_quantities_warehouse_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/product_quantities_warehouse_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/products_by_locations_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/products_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/recompute_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_category_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_category_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_category_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_time_series_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_time_series_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_product_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_product_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_product_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/reporting_margin_product_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_assign_partial_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_in_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_in_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_internal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      590 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_internal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_out_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_out_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/shipment_out_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-05-01 12:17:31.000000 trytond_stock-6.8.1/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.538437 trytond_stock-6.8.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10549 2023-06-21 17:11:52.000000 trytond_stock-6.8.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-06-21 17:11:52.000000 trytond_stock-6.8.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-06-21 17:11:56.538437 trytond_stock-6.8.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2614 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9561 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    46098 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/customer_return_restocking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    48755 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/delivery_note.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.528436 trytond_stock-6.8.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/conf.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.528436 trytond_stock-6.8.2/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/location.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2037 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1102 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3305 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7779 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/design/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2311 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.531770 trytond_stock-6.8.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/usage/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4193 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/usage/quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4669 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/usage/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/doc/usage/value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      825 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.531770 trytond_stock-6.8.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/icons/tryton-shipment-in.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/icons/tryton-shipment-out.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/icons/tryton-stock.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    49542 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/internal_shipment.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    23444 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/inventory.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8965 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/inventory.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.488436 trytond_stock-6.8.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    91409 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96063 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82156 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98088 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96959 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81052 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89803 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   102088 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82130 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97445 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92393 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    80321 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    84327 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89189 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86477 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96348 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85105 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87027 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93899 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    91532 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85855 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82049 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    77247 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90483 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    28654 2023-06-10 09:36:59.000000 trytond_stock-6.8.2/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10457 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7746 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    68212 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8526 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6302 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4507 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6992 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6018 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45875 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/picking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    50018 2023-05-13 22:24:13.000000 trytond_stock-6.8.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22458 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:11:56.538437 trytond_stock-6.8.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   115590 2023-06-05 16:15:37.000000 trytond_stock-6.8.2/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    53918 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2918 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23733 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32870 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/stock_reporting_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45402 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/supplier_restocking_list.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.498436 trytond_stock-6.8.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8304 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7532 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3365 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_inventory_count.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2675 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_inventory_empty_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_move_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_product_quantities_by_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5199 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_recompute_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_recompute_average_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5077 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7934 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_reporting_margin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2376 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_in_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2441 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_in_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4539 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_internal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3350 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_internal_transit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8630 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2487 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_out_return_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2528 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/scenario_stock_shipment_out_same_storage_output.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    69197 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-17 20:44:38.000000 trytond_stock-6.8.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.535103 trytond_stock-6.8.2/trytond_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-06-21 17:11:55.000000 trytond_stock-6.8.2/trytond_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     9605 2023-06-21 17:11:56.000000 trytond_stock-6.8.2/trytond_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:11:55.000000 trytond_stock-6.8.2/trytond_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-06-21 17:11:55.000000 trytond_stock-6.8.2/trytond_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:44:27.000000 trytond_stock-6.8.2/trytond_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-06-21 17:11:55.000000 trytond_stock-6.8.2/trytond_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:11:55.000000 trytond_stock-6.8.2/trytond_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:11:56.525103 trytond_stock-6.8.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1128 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_count_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_count_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_line_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/inventory_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_quantity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/location_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/move_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/party_address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/party_address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/party_contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/party_contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      903 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/period_cache_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/period_cache_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_cost_price_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_cost_price_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_modify_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_quantities_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_quantities_warehouse_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_quantities_warehouse_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/product_quantities_warehouse_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/products_by_locations_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/products_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/recompute_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_category_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_category_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_category_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_time_series_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_time_series_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_product_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_product_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_product_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/reporting_margin_product_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_assign_partial_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      611 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_in_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_in_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_internal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      590 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_internal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_out_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_out_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/shipment_out_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-05-01 12:17:31.000000 trytond_stock-6.8.2/view/user_form_preferences.xml
```

### Comparing `trytond_stock-6.8.1/CHANGELOG` & `trytond_stock-6.8.2/CHANGELOG`

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

### Comparing `trytond_stock-6.8.1/COPYRIGHT` & `trytond_stock-6.8.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/LICENSE` & `trytond_stock-6.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/PKG-INFO` & `trytond_stock-6.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock-6.8.1/__init__.py` & `trytond_stock-6.8.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/configuration.py` & `trytond_stock-6.8.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/configuration.xml` & `trytond_stock-6.8.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/customer_return_restocking_list.fodt` & `trytond_stock-6.8.2/customer_return_restocking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/delivery_note.fodt` & `trytond_stock-6.8.2/delivery_note.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/conf.py` & `trytond_stock-6.8.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/configuration.rst` & `trytond_stock-6.8.2/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/inventory.rst` & `trytond_stock-6.8.2/doc/design/inventory.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/location.rst` & `trytond_stock-6.8.2/doc/design/location.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/move.rst` & `trytond_stock-6.8.2/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/period.rst` & `trytond_stock-6.8.2/doc/design/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/product.rst` & `trytond_stock-6.8.2/doc/design/product.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/design/shipment.rst` & `trytond_stock-6.8.2/doc/design/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/setup.rst` & `trytond_stock-6.8.2/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/usage/period.rst` & `trytond_stock-6.8.2/doc/usage/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/usage/quantity.rst` & `trytond_stock-6.8.2/doc/usage/quantity.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/usage/shipment.rst` & `trytond_stock-6.8.2/doc/usage/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/doc/usage/value.rst` & `trytond_stock-6.8.2/doc/usage/value.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/exceptions.py` & `trytond_stock-6.8.2/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/icons/LICENSE` & `trytond_stock-6.8.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/internal_shipment.fodt` & `trytond_stock-6.8.2/internal_shipment.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/inventory.py` & `trytond_stock-6.8.2/inventory.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/inventory.xml` & `trytond_stock-6.8.2/inventory.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/ir.py` & `trytond_stock-6.8.2/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/bg.po` & `trytond_stock-6.8.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/ca.po` & `trytond_stock-6.8.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/cs.po` & `trytond_stock-6.8.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/de.po` & `trytond_stock-6.8.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/es.po` & `trytond_stock-6.8.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/es_419.po` & `trytond_stock-6.8.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/et.po` & `trytond_stock-6.8.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/fa.po` & `trytond_stock-6.8.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/fi.po` & `trytond_stock-6.8.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/fr.po` & `trytond_stock-6.8.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/hu.po` & `trytond_stock-6.8.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/id.po` & `trytond_stock-6.8.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/it.po` & `trytond_stock-6.8.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/lo.po` & `trytond_stock-6.8.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/lt.po` & `trytond_stock-6.8.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/nl.po` & `trytond_stock-6.8.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/pl.po` & `trytond_stock-6.8.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/pt.po` & `trytond_stock-6.8.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/ro.po` & `trytond_stock-6.8.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/ru.po` & `trytond_stock-6.8.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/sl.po` & `trytond_stock-6.8.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/tr.po` & `trytond_stock-6.8.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/uk.po` & `trytond_stock-6.8.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/locale/zh_CN.po` & `trytond_stock-6.8.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/location.py` & `trytond_stock-6.8.2/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 
         def valid_context(name):
             return (trans_context.get(name) is not None
                 and isinstance(trans_context[name], int))
 
         context = {}
         if (name == 'quantity'
-                and (trans_context.get('stock_date_end', datetime.date.max)
+                and ((trans_context.get('stock_date_end') or datetime.date.max)
                     > Date_.today())):
             context['stock_date_end'] = Date_.today()
 
         if name == 'forecast_quantity':
             context['forecast'] = True
             if not trans_context.get('stock_date_end'):
                 context['stock_date_end'] = datetime.date.max
@@ -490,15 +490,15 @@
         def get_record():
             if trans_context.get('product') is not None:
                 return Product(trans_context['product'])
             else:
                 return Template(trans_context['product_template'])
 
         context = {}
-        if 'stock_date_end' in trans_context:
+        if trans_context.get('stock_date_end') is not None:
             # Use the last cost_price of the day
             context['_datetime'] = datetime.datetime.combine(
                 trans_context['stock_date_end'], datetime.time.max)
             # The date could be before the product creation
             record = get_record()
             if record.create_date > context['_datetime']:
                 return cost_values
```

### Comparing `trytond_stock-6.8.1/location.xml` & `trytond_stock-6.8.2/location.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/message.xml` & `trytond_stock-6.8.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/move.py` & `trytond_stock-6.8.2/move.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/move.xml` & `trytond_stock-6.8.2/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/party.py` & `trytond_stock-6.8.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/party.xml` & `trytond_stock-6.8.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/period.py` & `trytond_stock-6.8.2/period.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/period.xml` & `trytond_stock-6.8.2/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/picking_list.fodt` & `trytond_stock-6.8.2/picking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/product.py` & `trytond_stock-6.8.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/product.xml` & `trytond_stock-6.8.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/res.py` & `trytond_stock-6.8.2/res.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/res.xml` & `trytond_stock-6.8.2/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/setup.py` & `trytond_stock-6.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/shipment.py` & `trytond_stock-6.8.2/shipment.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/shipment.xml` & `trytond_stock-6.8.2/shipment.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/stock.xml` & `trytond_stock-6.8.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/stock_reporting_margin.py` & `trytond_stock-6.8.2/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/stock_reporting_margin.xml` & `trytond_stock-6.8.2/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/supplier_restocking_list.fodt` & `trytond_stock-6.8.2/supplier_restocking_list.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_average_cost_price.rst` & `trytond_stock-6.8.2/tests/scenario_stock_average_cost_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_inventory.rst` & `trytond_stock-6.8.2/tests/scenario_stock_inventory.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_inventory_count.rst` & `trytond_stock-6.8.2/tests/scenario_stock_inventory_count.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_inventory_empty_quantity.rst` & `trytond_stock-6.8.2/tests/scenario_stock_inventory_empty_quantity.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_move_in_future.rst` & `trytond_stock-6.8.2/tests/scenario_stock_move_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_product_quantities_by_warehouse.rst` & `trytond_stock-6.8.2/tests/scenario_stock_product_quantities_by_warehouse.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_recompute_average_cost_price.rst` & `trytond_stock-6.8.2/tests/scenario_stock_recompute_average_cost_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_recompute_average_cost_price_production.rst` & `trytond_stock-6.8.2/tests/scenario_stock_recompute_average_cost_price_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_reporting.rst` & `trytond_stock-6.8.2/tests/scenario_stock_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_reporting_margin.rst` & `trytond_stock-6.8.2/tests/scenario_stock_reporting_margin.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_in_return.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_in_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_in_same_storage_input.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_in_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_internal.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_internal.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_internal_transit.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_internal_transit.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_out.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_out.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_out_return_same_storage_input.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_out_return_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/scenario_stock_shipment_out_same_storage_output.rst` & `trytond_stock-6.8.2/tests/scenario_stock_shipment_out_same_storage_output.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tests/test_module.py` & `trytond_stock-6.8.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/tox.ini` & `trytond_stock-6.8.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/trytond_stock.egg-info/PKG-INFO` & `trytond_stock-6.8.2/trytond_stock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-stock
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock-6.8.1/trytond_stock.egg-info/SOURCES.txt` & `trytond_stock-6.8.2/trytond_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/configuration_form.xml` & `trytond_stock-6.8.2/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/inventory_form.xml` & `trytond_stock-6.8.2/view/inventory_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/inventory_line_form.xml` & `trytond_stock-6.8.2/view/inventory_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/location_form.xml` & `trytond_stock-6.8.2/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/location_quantity_form.xml` & `trytond_stock-6.8.2/view/location_quantity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/move_form.xml` & `trytond_stock-6.8.2/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/move_tree.xml` & `trytond_stock-6.8.2/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/party_form.xml` & `trytond_stock-6.8.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/reporting_margin_category_list.xml` & `trytond_stock-6.8.2/view/reporting_margin_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/reporting_margin_context_form.xml` & `trytond_stock-6.8.2/view/reporting_margin_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_in_form.xml` & `trytond_stock-6.8.2/view/shipment_in_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_in_return_form.xml` & `trytond_stock-6.8.2/view/shipment_in_return_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_in_return_tree.xml` & `trytond_stock-6.8.2/view/shipment_in_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_in_tree.xml` & `trytond_stock-6.8.2/view/shipment_in_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_internal_form.xml` & `trytond_stock-6.8.2/view/shipment_internal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_internal_tree.xml` & `trytond_stock-6.8.2/view/shipment_internal_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_out_form.xml` & `trytond_stock-6.8.2/view/shipment_out_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_out_return_form.xml` & `trytond_stock-6.8.2/view/shipment_out_return_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_out_return_tree.xml` & `trytond_stock-6.8.2/view/shipment_out_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.8.1/view/shipment_out_tree.xml` & `trytond_stock-6.8.2/view/shipment_out_tree.xml`

 * *Files identical despite different names*

