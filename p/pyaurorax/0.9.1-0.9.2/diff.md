# Comparing `tmp/pyaurorax-0.9.1.tar.gz` & `tmp/pyaurorax-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaurorax-0.9.1.tar", max compression
+gzip compressed data, was "pyaurorax-0.9.2.tar", max compression
```

## Comparing `pyaurorax-0.9.1.tar` & `pyaurorax-0.9.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1078 2021-12-20 21:54:30.147983 pyaurorax-0.9.1/LICENSE
--rw-r--r--   0        0        0     7705 2022-01-26 20:16:19.460203 pyaurorax-0.9.1/README.md
--rw-r--r--   0        0        0     3177 2022-02-11 17:28:12.527946 pyaurorax-0.9.1/pyaurorax/__init__.py
--rw-r--r--   0        0        0        0 2021-12-20 21:54:49.231749 pyaurorax-0.9.1/pyaurorax/_internal/__init__.py
--rw-r--r--   0        0        0      126 2021-12-20 21:54:49.231749 pyaurorax-0.9.1/pyaurorax/_internal/util.py
--rw-r--r--   0        0        0     1536 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/api/__init__.py
--rw-r--r--   0        0        0     1238 2022-02-07 00:46:17.269999 pyaurorax-0.9.1/pyaurorax/api/api.py
--rw-r--r--   0        0        0      243 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/api/classes/__init__.py
--rw-r--r--   0        0        0     8037 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/api/classes/request.py
--rw-r--r--   0        0        0      871 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/api/classes/response.py
--rw-r--r--   0        0        0     4962 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/api/classes/urls.py
--rw-r--r--   0        0        0      818 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/availability/__init__.py
--rw-r--r--   0        0        0     5045 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/availability/availability.py
--rw-r--r--   0        0        0      261 2022-01-16 22:10:34.939274 pyaurorax-0.9.1/pyaurorax/availability/classes/__init__.py
--rw-r--r--   0        0        0      848 2022-01-16 22:10:34.943274 pyaurorax-0.9.1/pyaurorax/availability/classes/availability_result.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.1/pyaurorax/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.1/pyaurorax/cli/availability/__init__.py
--rw-r--r--   0        0        0     8376 2022-01-16 22:10:34.943274 pyaurorax-0.9.1/pyaurorax/cli/availability/commands.py
--rw-r--r--   0        0        0     2895 2022-02-11 17:28:12.527946 pyaurorax-0.9.1/pyaurorax/cli/cli.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.1/pyaurorax/cli/conjunctions/__init__.py
--rw-r--r--   0        0        0    13049 2022-01-26 20:15:40.040230 pyaurorax-0.9.1/pyaurorax/cli/conjunctions/commands.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/data_products/__init__.py
--rw-r--r--   0        0        0    14089 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/data_products/commands.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/ephemeris/__init__.py
--rw-r--r--   0        0        0    13476 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/ephemeris/commands.py
--rw-r--r--   0        0        0    11465 2022-01-26 20:15:38.668231 pyaurorax-0.9.1/pyaurorax/cli/helpers.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/sources/__init__.py
--rw-r--r--   0        0        0    21345 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/sources/commands.py
--rw-r--r--   0        0        0     3705 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/templates.py
--rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/util/__init__.py
--rw-r--r--   0        0        0     3418 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/cli/util/commands.py
--rw-r--r--   0        0        0     1422 2022-01-16 22:10:34.947274 pyaurorax-0.9.1/pyaurorax/conjunctions/__init__.py
--rw-r--r--   0        0        0      261 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/conjunctions/classes/__init__.py
--rw-r--r--   0        0        0     1602 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/conjunctions/classes/conjunction.py
--rw-r--r--   0        0        0    14988 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/conjunctions/classes/search.py
--rw-r--r--   0        0        0    11531 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/conjunctions/conjunctions.py
--rw-r--r--   0        0        0     3184 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/data_products/__init__.py
--rw-r--r--   0        0        0      263 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/data_products/classes/__init__.py
--rw-r--r--   0        0        0     3028 2022-01-16 22:10:34.951274 pyaurorax-0.9.1/pyaurorax/data_products/classes/data_product.py
--rw-r--r--   0        0        0    10204 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/data_products/classes/search.py
--rw-r--r--   0        0        0    16935 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/data_products/data_products.py
--rw-r--r--   0        0        0     1034 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/ephemeris/__init__.py
--rw-r--r--   0        0        0      255 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/ephemeris/classes/__init__.py
--rw-r--r--   0        0        0     3554 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/ephemeris/classes/ephemeris.py
--rw-r--r--   0        0        0    10280 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/ephemeris/classes/search.py
--rw-r--r--   0        0        0    13984 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/ephemeris/ephemeris.py
--rw-r--r--   0        0        0     1906 2022-01-16 22:10:34.955274 pyaurorax-0.9.1/pyaurorax/exceptions.py
--rw-r--r--   0        0        0     1585 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/location.py
--rw-r--r--   0        0        0      733 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/metadata/__init__.py
--rw-r--r--   0        0        0     2133 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/metadata/metadata.py
--rw-r--r--   0        0        0      864 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/requests/__init__.py
--rw-r--r--   0        0        0     6776 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/requests/requests.py
--rw-r--r--   0        0        0     3349 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/sources/__init__.py
--rw-r--r--   0        0        0      251 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/sources/classes/__init__.py
--rw-r--r--   0        0        0     6589 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/sources/classes/data_source.py
--rw-r--r--   0        0        0     1392 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/sources/classes/data_source_stats.py
--rw-r--r--   0        0        0    20282 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/sources/sources.py
--rw-r--r--   0        0        0      651 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/util/__init__.py
--rw-r--r--   0        0        0     4354 2022-01-16 22:10:34.959274 pyaurorax-0.9.1/pyaurorax/util/calculate_btrace.py
--rw-r--r--   0        0        0     1974 2022-02-11 17:28:12.527946 pyaurorax-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     9559 2022-02-11 17:28:45.163161 pyaurorax-0.9.1/setup.py
--rw-r--r--   0        0        0     9596 2022-02-11 17:28:45.163549 pyaurorax-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-12-20 21:54:30.147983 pyaurorax-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7671 2022-02-11 17:29:45.423958 pyaurorax-0.9.2/README.md
+-rw-r--r--   0        0        0     3177 2022-02-11 17:30:07.147961 pyaurorax-0.9.2/pyaurorax/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-20 21:54:49.231749 pyaurorax-0.9.2/pyaurorax/_internal/__init__.py
+-rw-r--r--   0        0        0      126 2021-12-20 21:54:49.231749 pyaurorax-0.9.2/pyaurorax/_internal/util.py
+-rw-r--r--   0        0        0     1536 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/api/__init__.py
+-rw-r--r--   0        0        0     1238 2022-02-07 00:46:17.269999 pyaurorax-0.9.2/pyaurorax/api/api.py
+-rw-r--r--   0        0        0      243 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/api/classes/__init__.py
+-rw-r--r--   0        0        0     8037 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/api/classes/request.py
+-rw-r--r--   0        0        0      871 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/api/classes/response.py
+-rw-r--r--   0        0        0     4962 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/api/classes/urls.py
+-rw-r--r--   0        0        0      818 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/availability/__init__.py
+-rw-r--r--   0        0        0     5045 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/availability/availability.py
+-rw-r--r--   0        0        0      261 2022-01-16 22:10:34.939274 pyaurorax-0.9.2/pyaurorax/availability/classes/__init__.py
+-rw-r--r--   0        0        0      848 2022-01-16 22:10:34.943274 pyaurorax-0.9.2/pyaurorax/availability/classes/availability_result.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.2/pyaurorax/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.2/pyaurorax/cli/availability/__init__.py
+-rw-r--r--   0        0        0     8376 2022-01-16 22:10:34.943274 pyaurorax-0.9.2/pyaurorax/cli/availability/commands.py
+-rw-r--r--   0        0        0     2895 2022-02-11 17:30:07.147961 pyaurorax-0.9.2/pyaurorax/cli/cli.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.943274 pyaurorax-0.9.2/pyaurorax/cli/conjunctions/__init__.py
+-rw-r--r--   0        0        0    13049 2022-01-26 20:15:40.040230 pyaurorax-0.9.2/pyaurorax/cli/conjunctions/commands.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/data_products/__init__.py
+-rw-r--r--   0        0        0    14089 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/data_products/commands.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/ephemeris/__init__.py
+-rw-r--r--   0        0        0    13476 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/ephemeris/commands.py
+-rw-r--r--   0        0        0    11465 2022-01-26 20:15:38.668231 pyaurorax-0.9.2/pyaurorax/cli/helpers.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/sources/__init__.py
+-rw-r--r--   0        0        0    21345 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/sources/commands.py
+-rw-r--r--   0        0        0     3705 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/templates.py
+-rw-r--r--   0        0        0        0 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/util/__init__.py
+-rw-r--r--   0        0        0     3418 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/cli/util/commands.py
+-rw-r--r--   0        0        0     1422 2022-01-16 22:10:34.947274 pyaurorax-0.9.2/pyaurorax/conjunctions/__init__.py
+-rw-r--r--   0        0        0      261 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/conjunctions/classes/__init__.py
+-rw-r--r--   0        0        0     1602 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/conjunctions/classes/conjunction.py
+-rw-r--r--   0        0        0    14988 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/conjunctions/classes/search.py
+-rw-r--r--   0        0        0    11531 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/conjunctions/conjunctions.py
+-rw-r--r--   0        0        0     3184 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/data_products/__init__.py
+-rw-r--r--   0        0        0      263 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/data_products/classes/__init__.py
+-rw-r--r--   0        0        0     3028 2022-01-16 22:10:34.951274 pyaurorax-0.9.2/pyaurorax/data_products/classes/data_product.py
+-rw-r--r--   0        0        0    10204 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/data_products/classes/search.py
+-rw-r--r--   0        0        0    16935 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/data_products/data_products.py
+-rw-r--r--   0        0        0     1034 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/ephemeris/__init__.py
+-rw-r--r--   0        0        0      255 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/ephemeris/classes/__init__.py
+-rw-r--r--   0        0        0     3554 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/ephemeris/classes/ephemeris.py
+-rw-r--r--   0        0        0    10280 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/ephemeris/classes/search.py
+-rw-r--r--   0        0        0    13984 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/ephemeris/ephemeris.py
+-rw-r--r--   0        0        0     1906 2022-01-16 22:10:34.955274 pyaurorax-0.9.2/pyaurorax/exceptions.py
+-rw-r--r--   0        0        0     1585 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/location.py
+-rw-r--r--   0        0        0      733 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/metadata/__init__.py
+-rw-r--r--   0        0        0     2133 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/metadata/metadata.py
+-rw-r--r--   0        0        0      864 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/requests/__init__.py
+-rw-r--r--   0        0        0     6776 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/requests/requests.py
+-rw-r--r--   0        0        0     3349 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/sources/__init__.py
+-rw-r--r--   0        0        0      251 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/sources/classes/__init__.py
+-rw-r--r--   0        0        0     6589 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/sources/classes/data_source.py
+-rw-r--r--   0        0        0     1392 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/sources/classes/data_source_stats.py
+-rw-r--r--   0        0        0    20282 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/sources/sources.py
+-rw-r--r--   0        0        0      651 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/util/__init__.py
+-rw-r--r--   0        0        0     4354 2022-01-16 22:10:34.959274 pyaurorax-0.9.2/pyaurorax/util/calculate_btrace.py
+-rw-r--r--   0        0        0     1974 2022-02-11 17:30:07.103961 pyaurorax-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     9525 2022-02-11 17:30:49.677647 pyaurorax-0.9.2/setup.py
+-rw-r--r--   0        0        0     9562 2022-02-11 17:30:49.677980 pyaurorax-0.9.2/PKG-INFO
```

### Comparing `pyaurorax-0.9.1/LICENSE` & `pyaurorax-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/README.md` & `pyaurorax-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 PyAuroraX is a Python library for interacting with [AuroraX](https://aurorax.space), a project working to be the world's first and foremost data platform for auroral science. The primary objective of AuroraX is to enable mining and exploration of existing and future auroral data, enabling key science and enhancing the benefits of the world's investment in auroral instrumentation. This will be accomplished with the development of key systems/standards for uniform metadata generation and search, image content analysis, interfaces to leading international tools, and a community involvement that includes more than 80% of the world's data providers.
 
 PyAuroraX officially supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).
 
 Some links to help:
 - [AuroraX main website](https://aurorax.space)
-- [PyAuroraX documentation](https://docs.aurorax.space/python_libraries/pyaurorax/overview)
-- [PyAuroraX API Reference](https://docs.aurorax.space/python_libraries/pyaurorax/api_reference/pyaurorax)
+- [PyAuroraX documentation](https://docs.aurorax.space/code/overview)
+- [PyAuroraX API Reference](https://docs.aurorax.space/code/pyaurorax_api_reference/pyaurorax)
 
 ## Installation
 
 PyAuroraX is available on PyPI so pip can be used to install it:
 
 ```console
 $ pip install pyaurorax
```

#### html2text {}

```diff
@@ -13,27 +13,27 @@
 key science and enhancing the benefits of the world's investment in auroral
 instrumentation. This will be accomplished with the development of key systems/
 standards for uniform metadata generation and search, image content analysis,
 interfaces to leading international tools, and a community involvement that
 includes more than 80% of the world's data providers. PyAuroraX officially
 supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).
 Some links to help: - [AuroraX main website](https://aurorax.space) -
-[PyAuroraX documentation](https://docs.aurorax.space/python_libraries/
-pyaurorax/overview) - [PyAuroraX API Reference](https://docs.aurorax.space/
-python_libraries/pyaurorax/api_reference/pyaurorax) ## Installation PyAuroraX
-is available on PyPI so pip can be used to install it: ```console $ pip install
-pyaurorax ``` To get full functionality, you can install PyAuroraX with the
-aacgmv2 dependency. Note that without this, the calculate_btrace methods in the
-util module will show warning messages. All other functionality will work
-without this dependency. ```console $ pip install pyaurorax[aacgmv2] ```
-Futhermore, if you want the most bleeding edge version of PyAuroraX, you can
-install it directly from the Github repository: ```console $ git clone https://
-github.com/aurorax-space/pyaurorax.git $ cd pyaurorax $ pip install . [ or with
-the aacgmv2 extra ] $ pip install .[aacgmv2] ``` ## Usage There are two things
-you can use as part of the PyAuroraX library: the main library, and the command
+[PyAuroraX documentation](https://docs.aurorax.space/code/overview) -
+[PyAuroraX API Reference](https://docs.aurorax.space/code/
+pyaurorax_api_reference/pyaurorax) ## Installation PyAuroraX is available on
+PyPI so pip can be used to install it: ```console $ pip install pyaurorax ```
+To get full functionality, you can install PyAuroraX with the aacgmv2
+dependency. Note that without this, the calculate_btrace methods in the util
+module will show warning messages. All other functionality will work without
+this dependency. ```console $ pip install pyaurorax[aacgmv2] ``` Futhermore, if
+you want the most bleeding edge version of PyAuroraX, you can install it
+directly from the Github repository: ```console $ git clone https://github.com/
+aurorax-space/pyaurorax.git $ cd pyaurorax $ pip install . [ or with the
+aacgmv2 extra ] $ pip install .[aacgmv2] ``` ## Usage There are two things you
+can use as part of the PyAuroraX library: the main library, and the command
 line tool. ### Library import You can import the library using the following
 statement: ```python >>> import pyaurorax ``` ### CLI program The program
 `aurorax-cli` is included in the PyAuroraX package as a command line tool. Try
 it out using: ``` $ aurorax-cli --help ``` ## Development Some common things
 you can do: - `make update` Update the Python dependency libraries - `tools/
 bump_version.py` Bump the version number - `make test-pytest-unauthorized-
 access` Only run the authorization tests - `make test-pytest-read` Only run the
```

### Comparing `pyaurorax-0.9.1/pyaurorax/__init__.py` & `pyaurorax-0.9.2/pyaurorax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Basic usage:
 ```python
 > import pyaurorax
 ```
 """
 
 # versioning info
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # documentation excludes
 __pdoc__ = {"cli": False}
 
 # pull in top level functions
 from .api import (AuroraXRequest,
                   authenticate,
```

### Comparing `pyaurorax-0.9.1/pyaurorax/api/__init__.py` & `pyaurorax-0.9.2/pyaurorax/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/api/api.py` & `pyaurorax-0.9.2/pyaurorax/api/api.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/api/classes/request.py` & `pyaurorax-0.9.2/pyaurorax/api/classes/request.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/api/classes/response.py` & `pyaurorax-0.9.2/pyaurorax/api/classes/response.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/api/classes/urls.py` & `pyaurorax-0.9.2/pyaurorax/api/classes/urls.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/availability/__init__.py` & `pyaurorax-0.9.2/pyaurorax/availability/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/availability/availability.py` & `pyaurorax-0.9.2/pyaurorax/availability/availability.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/availability/classes/availability_result.py` & `pyaurorax-0.9.2/pyaurorax/availability/classes/availability_result.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/availability/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/availability/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/cli.py` & `pyaurorax-0.9.2/pyaurorax/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if (return_json is True):
             return r.json()
     else:
         click.echo("Error connecting to AuroraX API, got a %d response" % (r.status_code))
 
 
 @click.group(invoke_without_command=True)
-@click.version_option(version="0.9.1")
+@click.version_option(version="0.9.2")
 @click.option("--api-key", type=str, help="Specify an API key")
 @click.option("--api-base-url", type=str, help="Set the AuroraX API base URL")
 @click.option("--verbose", "-v", is_flag=True, help="Enable verbose output")
 @click.option("--test-connectivity", is_flag=True, help="Test connectivity to AuroraX API")
 @click.pass_context
 def cli(ctx, api_key, api_base_url, verbose, test_connectivity):
     """
```

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/conjunctions/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/conjunctions/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/data_products/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/data_products/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/ephemeris/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/ephemeris/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/helpers.py` & `pyaurorax-0.9.2/pyaurorax/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/sources/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/sources/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/templates.py` & `pyaurorax-0.9.2/pyaurorax/cli/templates.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/cli/util/commands.py` & `pyaurorax-0.9.2/pyaurorax/cli/util/commands.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/conjunctions/__init__.py` & `pyaurorax-0.9.2/pyaurorax/conjunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/conjunctions/classes/conjunction.py` & `pyaurorax-0.9.2/pyaurorax/conjunctions/classes/conjunction.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/conjunctions/classes/search.py` & `pyaurorax-0.9.2/pyaurorax/conjunctions/classes/search.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/conjunctions/conjunctions.py` & `pyaurorax-0.9.2/pyaurorax/conjunctions/conjunctions.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/data_products/__init__.py` & `pyaurorax-0.9.2/pyaurorax/data_products/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/data_products/classes/data_product.py` & `pyaurorax-0.9.2/pyaurorax/data_products/classes/data_product.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/data_products/classes/search.py` & `pyaurorax-0.9.2/pyaurorax/data_products/classes/search.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/data_products/data_products.py` & `pyaurorax-0.9.2/pyaurorax/data_products/data_products.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/ephemeris/__init__.py` & `pyaurorax-0.9.2/pyaurorax/ephemeris/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/ephemeris/classes/ephemeris.py` & `pyaurorax-0.9.2/pyaurorax/ephemeris/classes/ephemeris.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/ephemeris/classes/search.py` & `pyaurorax-0.9.2/pyaurorax/ephemeris/classes/search.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/ephemeris/ephemeris.py` & `pyaurorax-0.9.2/pyaurorax/ephemeris/ephemeris.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/exceptions.py` & `pyaurorax-0.9.2/pyaurorax/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/location.py` & `pyaurorax-0.9.2/pyaurorax/location.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/metadata/__init__.py` & `pyaurorax-0.9.2/pyaurorax/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/metadata/metadata.py` & `pyaurorax-0.9.2/pyaurorax/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/requests/__init__.py` & `pyaurorax-0.9.2/pyaurorax/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/requests/requests.py` & `pyaurorax-0.9.2/pyaurorax/requests/requests.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/sources/__init__.py` & `pyaurorax-0.9.2/pyaurorax/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/sources/classes/data_source.py` & `pyaurorax-0.9.2/pyaurorax/sources/classes/data_source.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/sources/classes/data_source_stats.py` & `pyaurorax-0.9.2/pyaurorax/sources/classes/data_source_stats.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/sources/sources.py` & `pyaurorax-0.9.2/pyaurorax/sources/sources.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/util/__init__.py` & `pyaurorax-0.9.2/pyaurorax/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyaurorax/util/calculate_btrace.py` & `pyaurorax-0.9.2/pyaurorax/util/calculate_btrace.py`

 * *Files identical despite different names*

### Comparing `pyaurorax-0.9.1/pyproject.toml` & `pyaurorax-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyaurorax"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python library for interacting with the AuroraX API"
 readme = "README.md"
 homepage = "https://github.com/aurorax-space/pyaurorax"
 repository = "https://github.com/aurorax-space/pyaurorax"
 authors = [
     "Maryam Sohrabi <sohrabm@ucalgary.ca>", 
     "Darren Chaddock <dchaddoc@ucalgary.ca>"
```

### Comparing `pyaurorax-0.9.1/setup.py` & `pyaurorax-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 {'aacgmv2': ['aacgmv2>=2.6.2,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['aurorax-cli = pyaurorax.cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'pyaurorax',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Python library for interacting with the AuroraX API',
-    'long_description': '<a href="https://aurorax.space/"><img alt="AuroraX" src="logo.svg" height="60"></a>\n\n[![Github Actions - Tests](https://github.com/aurorax-space/pyaurorax/workflows/tests/badge.svg)](https://github.com/aurorax-space/pyaurorax/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/pyaurorax.svg)](https://pypi.python.org/pypi/pyaurorax/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://img.shields.io/pypi/pyversions/pyaurorax.svg)](https://pypi.python.org/pypi/pyaurorax/)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5815985.svg)](https://doi.org/10.5281/zenodo.5815985)\n\nPyAuroraX is a Python library for interacting with [AuroraX](https://aurorax.space), a project working to be the world\'s first and foremost data platform for auroral science. The primary objective of AuroraX is to enable mining and exploration of existing and future auroral data, enabling key science and enhancing the benefits of the world\'s investment in auroral instrumentation. This will be accomplished with the development of key systems/standards for uniform metadata generation and search, image content analysis, interfaces to leading international tools, and a community involvement that includes more than 80% of the world\'s data providers.\n\nPyAuroraX officially supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).\n\nSome links to help:\n- [AuroraX main website](https://aurorax.space)\n- [PyAuroraX documentation](https://docs.aurorax.space/python_libraries/pyaurorax/overview)\n- [PyAuroraX API Reference](https://docs.aurorax.space/python_libraries/pyaurorax/api_reference/pyaurorax)\n\n## Installation\n\nPyAuroraX is available on PyPI so pip can be used to install it:\n\n```console\n$ pip install pyaurorax\n```\n\nTo get full functionality, you can install PyAuroraX with the aacgmv2 dependency. Note that without this, the calculate_btrace methods in the util module will show warning messages. All other functionality will work without this dependency.\n\n```console\n$ pip install pyaurorax[aacgmv2]\n```\n\nFuthermore, if you want the most bleeding edge version of PyAuroraX, you can install it directly from the Github repository:\n\n```console\n$ git clone https://github.com/aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ pip install .\n[ or with the aacgmv2 extra ]\n$ pip install .[aacgmv2]\n```\n\n## Usage\n\nThere are two things you can use as part of the PyAuroraX library: the main library, and the command line tool.\n\n### Library import\n\nYou can import the library using the following statement:\n\n```python\n>>> import pyaurorax\n```\n\n### CLI program\n\nThe program `aurorax-cli` is included in the PyAuroraX package as a command line tool. Try it out using:\n\n```\n$ aurorax-cli --help\n```\n\n## Development\n\nSome common things you can do:\n- `make update` Update the Python dependency libraries\n- `tools/bump_version.py` Bump the version number\n- `make test-pytest-unauthorized-access` Only run the authorization tests\n- `make test-pytest-read` Only run the read-based tests\n- `make test-pytest-create-update-delete` Only run the write-based tests\n- `make docs` Generate pdoc documentation\n\n### Setup\n\nClone the repository and install primary and development dependencies using Poetry.\n\n```console\n$ git clone git@github.com:aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ make install\n```\n\n### Documentation\n\nDocumentation for the PyAuroraX project is managed by a separate repository [here](https://github.com/aurorax-space/docs). However, you are still able to generate the documentation for this repo for testing/development purposes. To generate the docs, run the following:\n\n```console\n$ make docs\n```\n\n### Testing\n\nPyAuroraX includes several test evaluations bundled into two groups: linting and functionality tests. The linting includes looking through the codebase using tools such as Flake8, PyLint, Pycodestyle, Bandit, and MyPy. The functionality tests use PyTest to test modules in the library.\n\nWhen running the functionality tests using PyTest, you must have the environment variable `AURORAX_APIKEY_STAGING` set to your API key on the staging API system. Alternatively, you can specifiy your API key using the command line (see example at the bottom of this section).\n\nThere exist several makefile targets to help run these tests quicker/easier. Below are the available commands:\n\n- `make test-linting` Run all linting tests\n- `make test-pytest` Run all automated functional tests\n- `make test-flake8` Run Flake8 styling tests\n- `make test-pylint` Run PyLint styling tests\n- `make test-pycodestyle` Run pycodestyle styling tests\n- `make test-bandit` Run Bandit security test\n- `make test-mypy` Run mypy type checking test\n- `make test-coverage` View test coverage report (must be done after `make test-pytest` or other coverage command)\n\nThe PyTest functionality tests include several categories of tests. You can run each category separately if you want using the "markers" feature of PyTest. All markers are found in the pytest.ini file at the root of the repository.\n\n- `poetry run pytest --markers` List all markers\n- `poetry run pytest -v -m accounts` Perform only the tests for the "accounts" marker\n- `poetry run pytest -v -m availability` Perform only the tests for the "availability" marker\n- `poetry run pytest -v -m conjunctions` Perform only the tests for the "conjunctions" marker\n- `poetry run pytest -v -m ephemeris` Perform only the tests for the "ephemeris" marker\n- `poetry run pytest -v -m exceptions` Perform only the tests for the "exceptions" marker\n- `poetry run pytest -v -m location` Perform only the tests for the "location" marker\n- `poetry run pytest -v -m metadata` Perform only the tests for the "metadata" marker\n- `poetry run pytest -v -m requests` Perform only the tests for the "request" marker\n- `poetry run pytest -v -m sources` Perform only the tests for the "sources" marker\n- `poetry run pytest -v -m util` Perform only the tests for the "util" marker\n\nBelow are some more commands for advanced usages of PyTest.\n\n- `poetry run pytest -v` Run all tests in verbose mode\n- `poetry run pytest --collect-only` List all available tests\n- `poetry run pytest --markers` List all markers (includes builtin, plugin and per-project ones)\n- `cat pytest.ini` List custom markers\n\nYou can also run Pytest against a different API. By default, it runs agains the staging API, but you can alternatively tell it to run against the production API, or a local instance.\n\n- `poetry run pytest -v --env=production` Run all tests against production API, using the AURORAX_APIKEY_PRODUCTION environment variable\n- `poetry run pytest --env=local --host=http://localhost:3000` Run all tests against a local instance of the API, using the AURORAX_APIKEY_LOCAL environment variable\n- `poetry run pytest -v --api-key=SOME_API_KEY` Run all tests with the specified API key (will run against the staging API since that\'s the default)\n- `poetry run pytest --help` View usage for pytest, including the usage for custom options (see the \'custom options\' section of the output)\n\nBelow are some more commands for evaluating the PyTest coverage.\n\n- `poetry run coverage report` View test coverage report\n- `poetry run coverage html` Generate an HTML page of the coverage report\n- `poetry run coverage report --show-missing` View the test coverage report and include the lines deemed to be not covered by tests\n\nNote that the coverage report only gets updated when using the Makefile pytest targets, or when running coverage manually like `coverage run -m pytest -v`. More information about usage of the `coverage` command can be found [here](https://coverage.readthedocs.io).\n',
+    'long_description': '<a href="https://aurorax.space/"><img alt="AuroraX" src="logo.svg" height="60"></a>\n\n[![Github Actions - Tests](https://github.com/aurorax-space/pyaurorax/workflows/tests/badge.svg)](https://github.com/aurorax-space/pyaurorax/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/pyaurorax.svg)](https://pypi.python.org/pypi/pyaurorax/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://img.shields.io/pypi/pyversions/pyaurorax.svg)](https://pypi.python.org/pypi/pyaurorax/)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5815985.svg)](https://doi.org/10.5281/zenodo.5815985)\n\nPyAuroraX is a Python library for interacting with [AuroraX](https://aurorax.space), a project working to be the world\'s first and foremost data platform for auroral science. The primary objective of AuroraX is to enable mining and exploration of existing and future auroral data, enabling key science and enhancing the benefits of the world\'s investment in auroral instrumentation. This will be accomplished with the development of key systems/standards for uniform metadata generation and search, image content analysis, interfaces to leading international tools, and a community involvement that includes more than 80% of the world\'s data providers.\n\nPyAuroraX officially supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).\n\nSome links to help:\n- [AuroraX main website](https://aurorax.space)\n- [PyAuroraX documentation](https://docs.aurorax.space/code/overview)\n- [PyAuroraX API Reference](https://docs.aurorax.space/code/pyaurorax_api_reference/pyaurorax)\n\n## Installation\n\nPyAuroraX is available on PyPI so pip can be used to install it:\n\n```console\n$ pip install pyaurorax\n```\n\nTo get full functionality, you can install PyAuroraX with the aacgmv2 dependency. Note that without this, the calculate_btrace methods in the util module will show warning messages. All other functionality will work without this dependency.\n\n```console\n$ pip install pyaurorax[aacgmv2]\n```\n\nFuthermore, if you want the most bleeding edge version of PyAuroraX, you can install it directly from the Github repository:\n\n```console\n$ git clone https://github.com/aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ pip install .\n[ or with the aacgmv2 extra ]\n$ pip install .[aacgmv2]\n```\n\n## Usage\n\nThere are two things you can use as part of the PyAuroraX library: the main library, and the command line tool.\n\n### Library import\n\nYou can import the library using the following statement:\n\n```python\n>>> import pyaurorax\n```\n\n### CLI program\n\nThe program `aurorax-cli` is included in the PyAuroraX package as a command line tool. Try it out using:\n\n```\n$ aurorax-cli --help\n```\n\n## Development\n\nSome common things you can do:\n- `make update` Update the Python dependency libraries\n- `tools/bump_version.py` Bump the version number\n- `make test-pytest-unauthorized-access` Only run the authorization tests\n- `make test-pytest-read` Only run the read-based tests\n- `make test-pytest-create-update-delete` Only run the write-based tests\n- `make docs` Generate pdoc documentation\n\n### Setup\n\nClone the repository and install primary and development dependencies using Poetry.\n\n```console\n$ git clone git@github.com:aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ make install\n```\n\n### Documentation\n\nDocumentation for the PyAuroraX project is managed by a separate repository [here](https://github.com/aurorax-space/docs). However, you are still able to generate the documentation for this repo for testing/development purposes. To generate the docs, run the following:\n\n```console\n$ make docs\n```\n\n### Testing\n\nPyAuroraX includes several test evaluations bundled into two groups: linting and functionality tests. The linting includes looking through the codebase using tools such as Flake8, PyLint, Pycodestyle, Bandit, and MyPy. The functionality tests use PyTest to test modules in the library.\n\nWhen running the functionality tests using PyTest, you must have the environment variable `AURORAX_APIKEY_STAGING` set to your API key on the staging API system. Alternatively, you can specifiy your API key using the command line (see example at the bottom of this section).\n\nThere exist several makefile targets to help run these tests quicker/easier. Below are the available commands:\n\n- `make test-linting` Run all linting tests\n- `make test-pytest` Run all automated functional tests\n- `make test-flake8` Run Flake8 styling tests\n- `make test-pylint` Run PyLint styling tests\n- `make test-pycodestyle` Run pycodestyle styling tests\n- `make test-bandit` Run Bandit security test\n- `make test-mypy` Run mypy type checking test\n- `make test-coverage` View test coverage report (must be done after `make test-pytest` or other coverage command)\n\nThe PyTest functionality tests include several categories of tests. You can run each category separately if you want using the "markers" feature of PyTest. All markers are found in the pytest.ini file at the root of the repository.\n\n- `poetry run pytest --markers` List all markers\n- `poetry run pytest -v -m accounts` Perform only the tests for the "accounts" marker\n- `poetry run pytest -v -m availability` Perform only the tests for the "availability" marker\n- `poetry run pytest -v -m conjunctions` Perform only the tests for the "conjunctions" marker\n- `poetry run pytest -v -m ephemeris` Perform only the tests for the "ephemeris" marker\n- `poetry run pytest -v -m exceptions` Perform only the tests for the "exceptions" marker\n- `poetry run pytest -v -m location` Perform only the tests for the "location" marker\n- `poetry run pytest -v -m metadata` Perform only the tests for the "metadata" marker\n- `poetry run pytest -v -m requests` Perform only the tests for the "request" marker\n- `poetry run pytest -v -m sources` Perform only the tests for the "sources" marker\n- `poetry run pytest -v -m util` Perform only the tests for the "util" marker\n\nBelow are some more commands for advanced usages of PyTest.\n\n- `poetry run pytest -v` Run all tests in verbose mode\n- `poetry run pytest --collect-only` List all available tests\n- `poetry run pytest --markers` List all markers (includes builtin, plugin and per-project ones)\n- `cat pytest.ini` List custom markers\n\nYou can also run Pytest against a different API. By default, it runs agains the staging API, but you can alternatively tell it to run against the production API, or a local instance.\n\n- `poetry run pytest -v --env=production` Run all tests against production API, using the AURORAX_APIKEY_PRODUCTION environment variable\n- `poetry run pytest --env=local --host=http://localhost:3000` Run all tests against a local instance of the API, using the AURORAX_APIKEY_LOCAL environment variable\n- `poetry run pytest -v --api-key=SOME_API_KEY` Run all tests with the specified API key (will run against the staging API since that\'s the default)\n- `poetry run pytest --help` View usage for pytest, including the usage for custom options (see the \'custom options\' section of the output)\n\nBelow are some more commands for evaluating the PyTest coverage.\n\n- `poetry run coverage report` View test coverage report\n- `poetry run coverage html` Generate an HTML page of the coverage report\n- `poetry run coverage report --show-missing` View the test coverage report and include the lines deemed to be not covered by tests\n\nNote that the coverage report only gets updated when using the Makefile pytest targets, or when running coverage manually like `coverage run -m pytest -v`. More information about usage of the `coverage` command can be found [here](https://coverage.readthedocs.io).\n',
     'author': 'Maryam Sohrabi',
     'author_email': 'sohrabm@ucalgary.ca',
     'maintainer': 'Maryam Sohrabi',
     'maintainer_email': 'sohrabm@ucalgary.ca',
     'url': 'https://github.com/aurorax-space/pyaurorax',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 'pyaurorax.sources', 'pyaurorax.sources.classes', 'pyaurorax.util']
 package_data = \ {'': ['*']} install_requires = \ ['click>=8.0.3,<9.0.0',
 'humanize>=3.2.0,<4.0.0', 'pydantic>=1.7.3,<2.0.0', 'python-
 dateutil>=2.8.2,<3.0.0', 'requests>=2.25.1,<3.0.0', 'termcolor>=1.1.0,<2.0.0',
 'texttable>=1.6.4,<2.0.0'] extras_require = \ {'aacgmv2':
 ['aacgmv2>=2.6.2,<3.0.0']} entry_points = \ {'console_scripts': ['aurorax-cli =
 pyaurorax.cli.cli:cli']} setup_kwargs = { 'name': 'pyaurorax', 'version':
-'0.9.1', 'description': 'Python library for interacting with the AuroraX API',
+'0.9.2', 'description': 'Python library for interacting with the AuroraX API',
 'long_description': '[AuroraX]\n\n[![Github Actions - Tests](https://
 github.com/aurorax-space/pyaurorax/workflows/tests/badge.svg)](https://
 github.com/aurorax-space/pyaurorax/actions?query=workflow%3Atests)\n[![PyPI
 version](https://img.shields.io/pypi/v/pyaurorax.svg)](https://pypi.python.org/
 pypi/pyaurorax/)\n[![MIT license](https://img.shields.io/badge/License-MIT-
 blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://
 img.shields.io/pypi/pyversions/pyaurorax.svg)](https://pypi.python.org/pypi/
@@ -31,39 +31,39 @@
 investment in auroral instrumentation. This will be accomplished with the
 development of key systems/standards for uniform metadata generation and
 search, image content analysis, interfaces to leading international tools, and
 a community involvement that includes more than 80% of the world\'s data
 providers.\n\nPyAuroraX officially supports Python 3.6, 3.7, 3.8, and 3.9
 (Python 3.10 not currently supported).\n\nSome links to help:\n- [AuroraX main
 website](https://aurorax.space)\n- [PyAuroraX documentation](https://
-docs.aurorax.space/python_libraries/pyaurorax/overview)\n- [PyAuroraX API
-Reference](https://docs.aurorax.space/python_libraries/pyaurorax/api_reference/
-pyaurorax)\n\n## Installation\n\nPyAuroraX is available on PyPI so pip can be
-used to install it:\n\n```console\n$ pip install pyaurorax\n```\n\nTo get full
-functionality, you can install PyAuroraX with the aacgmv2 dependency. Note that
-without this, the calculate_btrace methods in the util module will show warning
-messages. All other functionality will work without this
-dependency.\n\n```console\n$ pip install pyaurorax[aacgmv2]\n```\n\nFuthermore,
-if you want the most bleeding edge version of PyAuroraX, you can install it
-directly from the Github repository:\n\n```console\n$ git clone https://
-github.com/aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ pip install .\n[ or
-with the aacgmv2 extra ]\n$ pip install .[aacgmv2]\n```\n\n## Usage\n\nThere
-are two things you can use as part of the PyAuroraX library: the main library,
-and the command line tool.\n\n### Library import\n\nYou can import the library
-using the following statement:\n\n```python\n>>> import pyaurorax\n```\n\n###
-CLI program\n\nThe program `aurorax-cli` is included in the PyAuroraX package
-as a command line tool. Try it out using:\n\n```\n$ aurorax-cli --
-help\n```\n\n## Development\n\nSome common things you can do:\n- `make update`
-Update the Python dependency libraries\n- `tools/bump_version.py` Bump the
-version number\n- `make test-pytest-unauthorized-access` Only run the
-authorization tests\n- `make test-pytest-read` Only run the read-based tests\n-
-`make test-pytest-create-update-delete` Only run the write-based tests\n- `make
-docs` Generate pdoc documentation\n\n### Setup\n\nClone the repository and
-install primary and development dependencies using Poetry.\n\n```console\n$ git
-clone git@github.com:aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ make
+docs.aurorax.space/code/overview)\n- [PyAuroraX API Reference](https://
+docs.aurorax.space/code/pyaurorax_api_reference/pyaurorax)\n\n##
+Installation\n\nPyAuroraX is available on PyPI so pip can be used to install
+it:\n\n```console\n$ pip install pyaurorax\n```\n\nTo get full functionality,
+you can install PyAuroraX with the aacgmv2 dependency. Note that without this,
+the calculate_btrace methods in the util module will show warning messages. All
+other functionality will work without this dependency.\n\n```console\n$ pip
+install pyaurorax[aacgmv2]\n```\n\nFuthermore, if you want the most bleeding
+edge version of PyAuroraX, you can install it directly from the Github
+repository:\n\n```console\n$ git clone https://github.com/aurorax-space/
+pyaurorax.git\n$ cd pyaurorax\n$ pip install .\n[ or with the aacgmv2 extra
+]\n$ pip install .[aacgmv2]\n```\n\n## Usage\n\nThere are two things you can
+use as part of the PyAuroraX library: the main library, and the command line
+tool.\n\n### Library import\n\nYou can import the library using the following
+statement:\n\n```python\n>>> import pyaurorax\n```\n\n### CLI program\n\nThe
+program `aurorax-cli` is included in the PyAuroraX package as a command line
+tool. Try it out using:\n\n```\n$ aurorax-cli --help\n```\n\n##
+Development\n\nSome common things you can do:\n- `make update` Update the
+Python dependency libraries\n- `tools/bump_version.py` Bump the version
+number\n- `make test-pytest-unauthorized-access` Only run the authorization
+tests\n- `make test-pytest-read` Only run the read-based tests\n- `make test-
+pytest-create-update-delete` Only run the write-based tests\n- `make docs`
+Generate pdoc documentation\n\n### Setup\n\nClone the repository and install
+primary and development dependencies using Poetry.\n\n```console\n$ git clone
+git@github.com:aurorax-space/pyaurorax.git\n$ cd pyaurorax\n$ make
 install\n```\n\n### Documentation\n\nDocumentation for the PyAuroraX project is
 managed by a separate repository [here](https://github.com/aurorax-space/docs).
 However, you are still able to generate the documentation for this repo for
 testing/development purposes. To generate the docs, run the following:
 \n\n```console\n$ make docs\n```\n\n### Testing\n\nPyAuroraX includes several
 test evaluations bundled into two groups: linting and functionality tests. The
 linting includes looking through the codebase using tools such as Flake8,
```

### Comparing `pyaurorax-0.9.1/PKG-INFO` & `pyaurorax-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaurorax
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library for interacting with the AuroraX API
 Home-page: https://github.com/aurorax-space/pyaurorax
 License: MIT
 Keywords: aurorax,space physics,aurora,aurora borealis,northern lights,southern lights
 Author: Maryam Sohrabi
 Author-email: sohrabm@ucalgary.ca
 Maintainer: Maryam Sohrabi
@@ -50,16 +50,16 @@
 
 PyAuroraX is a Python library for interacting with [AuroraX](https://aurorax.space), a project working to be the world's first and foremost data platform for auroral science. The primary objective of AuroraX is to enable mining and exploration of existing and future auroral data, enabling key science and enhancing the benefits of the world's investment in auroral instrumentation. This will be accomplished with the development of key systems/standards for uniform metadata generation and search, image content analysis, interfaces to leading international tools, and a community involvement that includes more than 80% of the world's data providers.
 
 PyAuroraX officially supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).
 
 Some links to help:
 - [AuroraX main website](https://aurorax.space)
-- [PyAuroraX documentation](https://docs.aurorax.space/python_libraries/pyaurorax/overview)
-- [PyAuroraX API Reference](https://docs.aurorax.space/python_libraries/pyaurorax/api_reference/pyaurorax)
+- [PyAuroraX documentation](https://docs.aurorax.space/code/overview)
+- [PyAuroraX API Reference](https://docs.aurorax.space/code/pyaurorax_api_reference/pyaurorax)
 
 ## Installation
 
 PyAuroraX is available on PyPI so pip can be used to install it:
 
 ```console
 $ pip install pyaurorax
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyaurorax Version: 0.9.1 Summary: Python library
+Metadata-Version: 2.1 Name: pyaurorax Version: 0.9.2 Summary: Python library
 for interacting with the AuroraX API Home-page: https://github.com/aurorax-
 space/pyaurorax License: MIT Keywords: aurorax,space physics,aurora,aurora
 borealis,northern lights,southern lights Author: Maryam Sohrabi Author-email:
 sohrabm@ucalgary.ca Maintainer: Maryam Sohrabi Maintainer-email:
 sohrabm@ucalgary.ca Requires-Python: >=3.6,<3.10 Classifier: Intended Audience
 :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
@@ -38,27 +38,27 @@
 key science and enhancing the benefits of the world's investment in auroral
 instrumentation. This will be accomplished with the development of key systems/
 standards for uniform metadata generation and search, image content analysis,
 interfaces to leading international tools, and a community involvement that
 includes more than 80% of the world's data providers. PyAuroraX officially
 supports Python 3.6, 3.7, 3.8, and 3.9 (Python 3.10 not currently supported).
 Some links to help: - [AuroraX main website](https://aurorax.space) -
-[PyAuroraX documentation](https://docs.aurorax.space/python_libraries/
-pyaurorax/overview) - [PyAuroraX API Reference](https://docs.aurorax.space/
-python_libraries/pyaurorax/api_reference/pyaurorax) ## Installation PyAuroraX
-is available on PyPI so pip can be used to install it: ```console $ pip install
-pyaurorax ``` To get full functionality, you can install PyAuroraX with the
-aacgmv2 dependency. Note that without this, the calculate_btrace methods in the
-util module will show warning messages. All other functionality will work
-without this dependency. ```console $ pip install pyaurorax[aacgmv2] ```
-Futhermore, if you want the most bleeding edge version of PyAuroraX, you can
-install it directly from the Github repository: ```console $ git clone https://
-github.com/aurorax-space/pyaurorax.git $ cd pyaurorax $ pip install . [ or with
-the aacgmv2 extra ] $ pip install .[aacgmv2] ``` ## Usage There are two things
-you can use as part of the PyAuroraX library: the main library, and the command
+[PyAuroraX documentation](https://docs.aurorax.space/code/overview) -
+[PyAuroraX API Reference](https://docs.aurorax.space/code/
+pyaurorax_api_reference/pyaurorax) ## Installation PyAuroraX is available on
+PyPI so pip can be used to install it: ```console $ pip install pyaurorax ```
+To get full functionality, you can install PyAuroraX with the aacgmv2
+dependency. Note that without this, the calculate_btrace methods in the util
+module will show warning messages. All other functionality will work without
+this dependency. ```console $ pip install pyaurorax[aacgmv2] ``` Futhermore, if
+you want the most bleeding edge version of PyAuroraX, you can install it
+directly from the Github repository: ```console $ git clone https://github.com/
+aurorax-space/pyaurorax.git $ cd pyaurorax $ pip install . [ or with the
+aacgmv2 extra ] $ pip install .[aacgmv2] ``` ## Usage There are two things you
+can use as part of the PyAuroraX library: the main library, and the command
 line tool. ### Library import You can import the library using the following
 statement: ```python >>> import pyaurorax ``` ### CLI program The program
 `aurorax-cli` is included in the PyAuroraX package as a command line tool. Try
 it out using: ``` $ aurorax-cli --help ``` ## Development Some common things
 you can do: - `make update` Update the Python dependency libraries - `tools/
 bump_version.py` Bump the version number - `make test-pytest-unauthorized-
 access` Only run the authorization tests - `make test-pytest-read` Only run the
```

