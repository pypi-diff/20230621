# Comparing `tmp/motor-3.1.2.tar.gz` & `tmp/motor-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motor-3.1.2.tar", last modified: Mon Apr  3 17:25:18 2023, max compression
+gzip compressed data, was "motor-3.2.0.tar", last modified: Wed Jun 21 21:23:24 2023, max compression
```

## Comparing `motor-3.1.2.tar` & `motor-3.2.0.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.459303 motor-3.1.2/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    11357 2023-04-03 17:14:52.000000 motor-3.1.2/LICENSE
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      642 2023-04-03 17:14:52.000000 motor-3.1.2/MANIFEST.in
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6827 2023-04-03 17:25:18.459128 motor-3.1.2/PKG-INFO
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     5467 2023-04-03 17:14:52.000000 motor-3.1.2/README.rst
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.437292 motor-3.1.2/doc/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3124 2023-04-03 17:14:52.000000 motor-3.1.2/doc/Makefile
--rw-r--r--   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:14:52.000000 motor-3.1.2/doc/__init__.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.437495 motor-3.1.2/doc/_static/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    57234 2023-04-03 17:14:52.000000 motor-3.1.2/doc/_static/motor.png
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.439832 motor-3.1.2/doc/api-asyncio/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      244 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/aiohttp.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      462 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_gridfs.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      203 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_change_stream.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      448 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_client.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      215 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_client_encryption.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      238 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_client_session.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      524 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_collection.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      447 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/asyncio_motor_database.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      436 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/cursors.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      422 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-asyncio/index.rst
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.441508 motor-3.1.2/doc/api-tornado/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      394 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/cursors.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      455 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/gridfs.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      362 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/index.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      182 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_change_stream.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      433 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_client.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      194 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_client_encryption.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      257 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_client_session.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      482 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_collection.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      412 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/motor_database.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      228 2023-04-03 17:14:52.000000 motor-3.1.2/doc/api-tornado/web.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    57478 2023-04-03 17:22:58.000000 motor-3.1.2/doc/changelog.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6688 2023-04-03 17:14:52.000000 motor-3.1.2/doc/conf.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1896 2023-04-03 17:14:52.000000 motor-3.1.2/doc/configuration.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      430 2023-04-03 17:14:52.000000 motor-3.1.2/doc/contributors.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      914 2023-04-03 17:14:52.000000 motor-3.1.2/doc/coroutine_annotation.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4531 2023-04-03 17:14:52.000000 motor-3.1.2/doc/developer-guide.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4422 2023-04-03 17:14:52.000000 motor-3.1.2/doc/differences.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)       81 2023-04-03 17:14:52.000000 motor-3.1.2/doc/docs-requirements.txt
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.444001 motor-3.1.2/doc/examples/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1293 2023-04-03 17:16:22.000000 motor-3.1.2/doc/examples/aiohttp_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1545 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/aiohttp_gridfs_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      552 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/aiohttp_gridfs_example.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      899 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/authentication.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3872 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/auto_csfle_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6449 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/bulk.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     5197 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/encryption.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2796 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/explicit_encryption_automatic_decryption_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2397 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/explicit_encryption_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      269 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/index.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4649 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/monitoring.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4474 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/monitoring_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3895 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/server_fle_enforcement_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1991 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/tailable-cursors.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3460 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/tornado_change_stream_example.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1517 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/tornado_change_stream_example.rst
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.444160 motor-3.1.2/doc/examples/tornado_change_stream_templates/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1236 2023-04-03 17:14:52.000000 motor-3.1.2/doc/examples/tornado_change_stream_templates/index.html
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1399 2023-04-03 17:14:52.000000 motor-3.1.2/doc/features.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3049 2023-04-03 17:14:52.000000 motor-3.1.2/doc/index.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2054 2023-04-03 17:14:52.000000 motor-3.1.2/doc/installation.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3069 2023-04-03 17:14:52.000000 motor-3.1.2/doc/make.bat
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     7508 2023-04-03 17:14:52.000000 motor-3.1.2/doc/migrate-to-motor-2.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    18425 2023-04-03 17:14:52.000000 motor-3.1.2/doc/migrate-to-motor-3.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2951 2023-04-03 17:14:52.000000 motor-3.1.2/doc/mongo_extensions.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6774 2023-04-03 17:14:52.000000 motor-3.1.2/doc/motor_extensions.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.444313 motor-3.1.2/doc/pydoctheme/
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.444660 motor-3.1.2/doc/pydoctheme/static/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2980 2023-04-03 17:14:52.000000 motor-3.1.2/doc/pydoctheme/static/pydoctheme.css
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      531 2023-04-03 17:14:52.000000 motor-3.1.2/doc/pydoctheme/theme.conf
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     9375 2023-04-03 17:14:52.000000 motor-3.1.2/doc/requirements.rst
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.444822 motor-3.1.2/doc/static/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6284 2023-04-03 17:14:52.000000 motor-3.1.2/doc/static/sidebar.js
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    17317 2023-04-03 17:14:52.000000 motor-3.1.2/doc/tutorial-asyncio.rst
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    17303 2023-04-03 17:14:52.000000 motor-3.1.2/doc/tutorial-tornado.rst
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.446990 motor-3.1.2/motor/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1087 2023-04-03 17:25:13.000000 motor-3.1.2/motor/__init__.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.449571 motor-3.1.2/motor/aiohttp/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     9311 2023-04-03 17:14:52.000000 motor-3.1.2/motor/aiohttp/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    74169 2023-04-03 17:16:22.000000 motor-3.1.2/motor/core.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    59713 2023-04-03 17:14:52.000000 motor-3.1.2/motor/docstrings.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.449742 motor-3.1.2/motor/frameworks/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:14:52.000000 motor-3.1.2/motor/frameworks/__init__.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.449913 motor-3.1.2/motor/frameworks/asyncio/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4645 2023-04-03 17:18:32.000000 motor-3.1.2/motor/frameworks/asyncio/__init__.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.450104 motor-3.1.2/motor/frameworks/tornado/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4203 2023-04-03 17:18:32.000000 motor-3.1.2/motor/frameworks/tornado/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     9810 2023-04-03 17:14:52.000000 motor-3.1.2/motor/metaprogramming.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2294 2023-04-03 17:14:52.000000 motor-3.1.2/motor/motor_asyncio.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      694 2023-04-03 17:14:52.000000 motor-3.1.2/motor/motor_common.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    18840 2023-04-03 17:14:52.000000 motor-3.1.2/motor/motor_gridfs.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2091 2023-04-03 17:14:52.000000 motor-3.1.2/motor/motor_tornado.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6922 2023-04-03 17:14:52.000000 motor-3.1.2/motor/web.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.449380 motor-3.1.2/motor.egg-info/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6827 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/PKG-INFO
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4176 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/SOURCES.txt
--rw-r--r--   0 steve.silvester   (502) wheel        (0)        1 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/dependency_links.txt
--rw-r--r--   0 steve.silvester   (502) wheel        (0)        1 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/not-zip-safe
--rw-r--r--   0 steve.silvester   (502) wheel        (0)      242 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/requires.txt
--rw-r--r--   0 steve.silvester   (502) wheel        (0)        6 2023-04-03 17:25:18.000000 motor-3.1.2/motor.egg-info/top_level.txt
--rw-r--r--   0 steve.silvester   (502) wheel        (0)       38 2023-04-03 17:25:18.459348 motor-3.1.2/setup.cfg
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     5885 2023-04-03 17:25:13.000000 motor-3.1.2/setup.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.450432 motor-3.1.2/synchro/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    25650 2023-04-03 17:16:22.000000 motor-3.1.2/synchro/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    13056 2023-04-03 17:16:22.000000 motor-3.1.2/synchro/synchrotest.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.451418 motor-3.1.2/test/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2566 2023-04-03 17:14:52.000000 motor-3.1.2/test/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2666 2023-04-03 17:14:52.000000 motor-3.1.2/test/assert_logs_backport.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.454439 motor-3.1.2/test/asyncio_tests/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     8632 2023-04-03 17:16:22.000000 motor-3.1.2/test/asyncio_tests/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    10568 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_aiohttp_gridfs.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     7592 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_await.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6106 2023-04-03 17:18:54.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_basic.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    10540 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_change_stream.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    10625 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_client.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     9908 2023-04-03 17:16:22.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_collection.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    25940 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_cursor.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6316 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_database.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     8046 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_encryption.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    13021 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_grid_file.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3212 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_gridfsbucket.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1972 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_ipv6.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2274 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_replica_set.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     7528 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_session.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6227 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_ssl.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6328 2023-04-03 17:14:52.000000 motor-3.1.2/test/asyncio_tests/test_asyncio_tests.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    53012 2023-04-03 17:16:22.000000 motor-3.1.2/test/asyncio_tests/test_examples.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.455343 motor-3.1.2/test/certificates/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     1273 2023-04-03 17:14:52.000000 motor-3.1.2/test/certificates/ca.pem
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2956 2023-04-03 17:14:52.000000 motor-3.1.2/test/certificates/client.pem
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2977 2023-04-03 17:14:52.000000 motor-3.1.2/test/certificates/server.pem
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    12060 2023-04-03 17:14:52.000000 motor-3.1.2/test/test_environment.py
-drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-04-03 17:25:18.458896 motor-3.1.2/test/tornado_tests/
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4714 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/__init__.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3189 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_auth.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     7570 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_await.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     5929 2023-04-03 17:18:54.000000 motor-3.1.2/test/tornado_tests/test_motor_basic.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     8745 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_change_stream.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    11336 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_client.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     9943 2023-04-03 17:16:22.000000 motor-3.1.2/test/tornado_tests/test_motor_collection.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4993 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_core.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    22867 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_cursor.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6586 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_database.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)    12769 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_grid_file.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2246 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_gridfsbucket.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2039 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_ipv6.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     2615 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_replica_set.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     8121 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_session.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     5556 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_ssl.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     6766 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_transaction.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     8699 2023-04-03 17:14:52.000000 motor-3.1.2/test/tornado_tests/test_motor_web.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4668 2023-04-03 17:14:52.000000 motor-3.1.2/test/utils.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     3071 2023-04-03 17:14:52.000000 motor-3.1.2/test/version.py
--rw-r--r--   0 steve.silvester   (502) wheel        (0)     4631 2023-04-03 17:16:22.000000 motor-3.1.2/tox.ini
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.294335 motor-3.2.0/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    11357 2023-06-21 21:19:30.000000 motor-3.2.0/LICENSE
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      642 2023-06-21 21:19:30.000000 motor-3.2.0/MANIFEST.in
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7086 2023-06-21 21:23:24.294183 motor-3.2.0/PKG-INFO
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     5726 2023-06-21 21:19:30.000000 motor-3.2.0/README.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.275903 motor-3.2.0/doc/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3124 2023-06-21 21:19:30.000000 motor-3.2.0/doc/Makefile
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:19:30.000000 motor-3.2.0/doc/__init__.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.276101 motor-3.2.0/doc/_static/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    57234 2023-06-21 21:19:30.000000 motor-3.2.0/doc/_static/motor.png
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.277806 motor-3.2.0/doc/api-asyncio/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      244 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/aiohttp.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      462 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_gridfs.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      203 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_change_stream.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      448 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_client.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      215 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_client_encryption.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      238 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_client_session.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      524 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_collection.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      447 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/asyncio_motor_database.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      436 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/cursors.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      422 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-asyncio/index.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.279319 motor-3.2.0/doc/api-tornado/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      394 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/cursors.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      455 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/gridfs.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      362 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/index.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      182 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_change_stream.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      433 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_client.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      194 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_client_encryption.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      257 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_client_session.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      482 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_collection.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      412 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/motor_database.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      228 2023-06-21 21:19:30.000000 motor-3.2.0/doc/api-tornado/web.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    58007 2023-06-21 21:19:30.000000 motor-3.2.0/doc/changelog.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6688 2023-06-21 21:19:30.000000 motor-3.2.0/doc/conf.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1896 2023-06-21 21:19:30.000000 motor-3.2.0/doc/configuration.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      430 2023-06-21 21:19:30.000000 motor-3.2.0/doc/contributors.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      914 2023-06-21 21:19:30.000000 motor-3.2.0/doc/coroutine_annotation.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4531 2023-06-21 21:19:30.000000 motor-3.2.0/doc/developer-guide.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4422 2023-06-21 21:19:30.000000 motor-3.2.0/doc/differences.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)       81 2023-06-21 21:19:30.000000 motor-3.2.0/doc/docs-requirements.txt
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.282408 motor-3.2.0/doc/examples/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1420 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/aiohttp_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1545 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/aiohttp_gridfs_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      552 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/aiohttp_gridfs_example.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      899 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/authentication.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3872 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/auto_csfle_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6449 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/bulk.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     5197 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/encryption.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2796 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/explicit_encryption_automatic_decryption_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2397 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/explicit_encryption_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      269 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/index.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4649 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/monitoring.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4474 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/monitoring_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3895 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/server_fle_enforcement_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1991 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/tailable-cursors.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3460 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/tornado_change_stream_example.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1517 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/tornado_change_stream_example.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.282574 motor-3.2.0/doc/examples/tornado_change_stream_templates/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1236 2023-06-21 21:19:30.000000 motor-3.2.0/doc/examples/tornado_change_stream_templates/index.html
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1399 2023-06-21 21:19:30.000000 motor-3.2.0/doc/features.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3049 2023-06-21 21:19:30.000000 motor-3.2.0/doc/index.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2054 2023-06-21 21:19:30.000000 motor-3.2.0/doc/installation.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3069 2023-06-21 21:19:30.000000 motor-3.2.0/doc/make.bat
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7508 2023-06-21 21:19:30.000000 motor-3.2.0/doc/migrate-to-motor-2.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    18425 2023-06-21 21:19:30.000000 motor-3.2.0/doc/migrate-to-motor-3.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2951 2023-06-21 21:19:30.000000 motor-3.2.0/doc/mongo_extensions.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6774 2023-06-21 21:19:30.000000 motor-3.2.0/doc/motor_extensions.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.282758 motor-3.2.0/doc/pydoctheme/
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.282941 motor-3.2.0/doc/pydoctheme/static/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2980 2023-06-21 21:19:30.000000 motor-3.2.0/doc/pydoctheme/static/pydoctheme.css
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      531 2023-06-21 21:19:30.000000 motor-3.2.0/doc/pydoctheme/theme.conf
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10291 2023-06-21 21:19:30.000000 motor-3.2.0/doc/requirements.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.283092 motor-3.2.0/doc/static/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6284 2023-06-21 21:19:30.000000 motor-3.2.0/doc/static/sidebar.js
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    17317 2023-06-21 21:19:30.000000 motor-3.2.0/doc/tutorial-asyncio.rst
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    17303 2023-06-21 21:19:30.000000 motor-3.2.0/doc/tutorial-tornado.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.284814 motor-3.2.0/motor/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1029 2023-06-21 21:19:30.000000 motor-3.2.0/motor/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      877 2023-06-21 21:23:19.000000 motor-3.2.0/motor/_version.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.285946 motor-3.2.0/motor/aiohttp/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     9311 2023-06-21 21:19:30.000000 motor-3.2.0/motor/aiohttp/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    78476 2023-06-21 21:19:30.000000 motor-3.2.0/motor/core.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    59705 2023-06-21 21:19:30.000000 motor-3.2.0/motor/docstrings.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.286091 motor-3.2.0/motor/frameworks/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:19:30.000000 motor-3.2.0/motor/frameworks/__init__.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.286232 motor-3.2.0/motor/frameworks/asyncio/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4645 2023-06-21 21:19:30.000000 motor-3.2.0/motor/frameworks/asyncio/__init__.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.286414 motor-3.2.0/motor/frameworks/tornado/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4203 2023-06-21 21:19:30.000000 motor-3.2.0/motor/frameworks/tornado/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     9810 2023-06-21 21:19:30.000000 motor-3.2.0/motor/metaprogramming.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2294 2023-06-21 21:19:30.000000 motor-3.2.0/motor/motor_asyncio.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      694 2023-06-21 21:19:30.000000 motor-3.2.0/motor/motor_common.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    18840 2023-06-21 21:19:30.000000 motor-3.2.0/motor/motor_gridfs.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2091 2023-06-21 21:19:30.000000 motor-3.2.0/motor/motor_tornado.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6922 2023-06-21 21:19:30.000000 motor-3.2.0/motor/web.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.285774 motor-3.2.0/motor.egg-info/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7086 2023-06-21 21:23:24.000000 motor-3.2.0/motor.egg-info/PKG-INFO
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4194 2023-06-21 21:23:24.000000 motor-3.2.0/motor.egg-info/SOURCES.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        1 2023-06-21 21:23:24.000000 motor-3.2.0/motor.egg-info/dependency_links.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        1 2023-06-21 21:21:40.000000 motor-3.2.0/motor.egg-info/not-zip-safe
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      242 2023-06-21 21:23:24.000000 motor-3.2.0/motor.egg-info/requires.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        6 2023-06-21 21:23:24.000000 motor-3.2.0/motor.egg-info/top_level.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)       38 2023-06-21 21:23:24.294380 motor-3.2.0/setup.cfg
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6005 2023-06-21 21:19:30.000000 motor-3.2.0/setup.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.286720 motor-3.2.0/synchro/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    26482 2023-06-21 21:19:30.000000 motor-3.2.0/synchro/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    13491 2023-06-21 21:19:30.000000 motor-3.2.0/synchro/synchrotest.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.287501 motor-3.2.0/test/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2566 2023-06-21 21:19:30.000000 motor-3.2.0/test/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2666 2023-06-21 21:19:30.000000 motor-3.2.0/test/assert_logs_backport.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.290594 motor-3.2.0/test/asyncio_tests/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8756 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10568 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_aiohttp_gridfs.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7592 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_await.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6106 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_basic.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10540 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_change_stream.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10625 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_client.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    13322 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_collection.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    25940 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_cursor.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6316 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_database.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8046 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_encryption.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    13021 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_grid_file.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3212 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_gridfsbucket.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1972 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_ipv6.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2274 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_replica_set.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7528 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_session.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6227 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_ssl.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6328 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_asyncio_tests.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    54827 2023-06-21 21:19:30.000000 motor-3.2.0/test/asyncio_tests/test_examples.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.291268 motor-3.2.0/test/certificates/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1273 2023-06-21 21:19:30.000000 motor-3.2.0/test/certificates/ca.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2956 2023-06-21 21:19:30.000000 motor-3.2.0/test/certificates/client.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2977 2023-06-21 21:19:30.000000 motor-3.2.0/test/certificates/server.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    12282 2023-06-21 21:19:30.000000 motor-3.2.0/test/test_environment.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-06-21 21:23:24.293979 motor-3.2.0/test/tornado_tests/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4714 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3189 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_auth.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     7570 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_await.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     5929 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_basic.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8745 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_change_stream.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    11336 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_client.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    13381 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_collection.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4993 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_core.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    22867 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_cursor.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6586 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_database.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    12769 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_grid_file.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2246 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_gridfsbucket.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2039 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_ipv6.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2615 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_replica_set.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8121 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_session.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     5556 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_ssl.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6766 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_transaction.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8699 2023-06-21 21:19:30.000000 motor-3.2.0/test/tornado_tests/test_motor_web.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4668 2023-06-21 21:19:30.000000 motor-3.2.0/test/utils.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3071 2023-06-21 21:19:30.000000 motor-3.2.0/test/version.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4701 2023-06-21 21:19:30.000000 motor-3.2.0/tox.ini
```

### Comparing `motor-3.1.2/LICENSE` & `motor-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/MANIFEST.in` & `motor-3.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/PKG-INFO` & `motor-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor
-Version: 3.1.2
+Version: 3.2.0
 Summary: Non-blocking MongoDB driver for Tornado or asyncio
 Home-page: https://github.com/mongodb/motor/
 Author: A. Jesse Jiryu Davis
 Author-email: jesse@mongodb.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: mongo,mongodb,pymongo,gridfs,bson,motor,tornado,asyncio
 Classifier: Intended Audience :: Developers
@@ -68,16 +68,15 @@
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongo, please look into
 our `support channels <https://support.mongodb.com/welcome>`_. Please
 do not email any of the Motor developers directly with issues or
-questions - you're more likely to get an answer on the `MongoDB Community
-Forums <https://developer.mongodb.com/community/forums/tag/motor-driver>`_.
+questions - you're more likely to get an answer on the `StackOverflow <https://stackoverflow.com/questions/tagged/mongodb>`_ (using a "mongodb" tag).
 
 Bugs / Feature Requests
 =======================
 
 Think you've found a bug? Want to see a new feature in Motor? Please open a
 case in our issue management tool, JIRA:
 
@@ -189,14 +188,20 @@
 =============
 
 Motor's documentation is on ReadTheDocs_.
 
 Build the documentation with Python 3.7+. Install sphinx_, Tornado_, and aiohttp_,
 and do ``cd doc; make html``.
 
+Learning Resources
+==================
+
+MongoDB Learn - `Python courses <https://learn.mongodb.com/catalog?labels=%5B%22Language%22%5D&values=%5B%22Python%22%5D>`_.
+`Python Articles on Developer Center <https://www.mongodb.com/developer/languages/python/>`_.
+
 Testing
 =======
 
 Run ``python setup.py test``.
 Tests are located in the ``test/`` directory.
 
 .. _PyMongo: http://pypi.python.org/pypi/pymongo/
```

### Comparing `motor-3.1.2/README.rst` & `motor-3.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongo, please look into
 our `support channels <https://support.mongodb.com/welcome>`_. Please
 do not email any of the Motor developers directly with issues or
-questions - you're more likely to get an answer on the `MongoDB Community
-Forums <https://developer.mongodb.com/community/forums/tag/motor-driver>`_.
+questions - you're more likely to get an answer on the `StackOverflow <https://stackoverflow.com/questions/tagged/mongodb>`_ (using a "mongodb" tag).
 
 Bugs / Feature Requests
 =======================
 
 Think you've found a bug? Want to see a new feature in Motor? Please open a
 case in our issue management tool, JIRA:
 
@@ -154,14 +153,20 @@
 =============
 
 Motor's documentation is on ReadTheDocs_.
 
 Build the documentation with Python 3.7+. Install sphinx_, Tornado_, and aiohttp_,
 and do ``cd doc; make html``.
 
+Learning Resources
+==================
+
+MongoDB Learn - `Python courses <https://learn.mongodb.com/catalog?labels=%5B%22Language%22%5D&values=%5B%22Python%22%5D>`_.
+`Python Articles on Developer Center <https://www.mongodb.com/developer/languages/python/>`_.
+
 Testing
 =======
 
 Run ``python setup.py test``.
 Tests are located in the ``test/`` directory.
 
 .. _PyMongo: http://pypi.python.org/pypi/pymongo/
```

### Comparing `motor-3.1.2/doc/Makefile` & `motor-3.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/_static/motor.png` & `motor-3.2.0/doc/_static/motor.png`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/api-asyncio/asyncio_motor_collection.rst` & `motor-3.2.0/doc/api-asyncio/asyncio_motor_collection.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/changelog.rst` & `motor-3.2.0/doc/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Changelog
 =========
 
 .. currentmodule:: motor.motor_tornado
 
-
-Motor 3.1.2
+Motor 3.2.0
 -----------
 
-Motor 3.1.2 fixes a bug when using Motor with ``multiprocessing``.
-
+- Add support for MongoDB 7.0 and PyMongo 4.4+.
+- Add support for Queryable Encryption helpers :meth:`~motor.core.MotorClientEncryption.create_encrypted_collection` and
+  :meth:`~motor.core.MotorClientEncryption.encrypt_expression`.
+  Backwards-breaking changes may be made before the final release.
+- pymongocrypt 1.6.0 or later is now required for Client Side Field Level
+  Encryption (CSFLE) and Queryable Encryption (QE) support. MongoDB Server 7.0
+  introduced a backwards breaking change to the QE protocol. Users taking
+  advantage of the QE must now upgrade to MongoDB 7.0+ and Motor 3.2+.
 
 Motor 3.1.1
 -----------
 
 Motor 3.1.1 adds support for Python 3.11 and fixes a bug that caused an
 ``ImportError`` in Python 3.11.0.
```

### Comparing `motor-3.1.2/doc/conf.py` & `motor-3.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/configuration.rst` & `motor-3.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/coroutine_annotation.py` & `motor-3.2.0/doc/coroutine_annotation.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/developer-guide.rst` & `motor-3.2.0/doc/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/differences.rst` & `motor-3.2.0/doc/differences.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/aiohttp_example.py` & `motor-3.2.0/doc/examples/aiohttp_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # These comments let tutorial-asyncio.rst include this code in sections.
 # -- setup-start --
-import asyncio
-
 from aiohttp import web
 
 from motor.motor_asyncio import AsyncIOMotorClient
 
 
 async def setup_db():
     db = AsyncIOMotorClient().test
@@ -37,14 +35,24 @@
 
     return web.Response(body=document["body"].encode(), content_type="text/html")
 
 
 # -- handler-end --
 
 # -- main-start --
-db = asyncio.run(setup_db())
-app = web.Application()
-app["db"] = db
-# Route requests to the page_handler() coroutine.
-app.router.add_get("/pages/{page_name}", page_handler)
-web.run_app(app)
+async def init_connection():
+    db = await setup_db()
+    app = web.Application()
+    app["db"] = db
+    # Route requests to the page_handler() coroutine.
+    app.router.add_get("/pages/{page_name}", page_handler)
+    return app
+
+
+def main():
+    app = init_connection()
+    web.run_app(app)
+
+
+if __name__ == "__main__":
+    main()
 # -- main-end --
```

### Comparing `motor-3.1.2/doc/examples/aiohttp_gridfs_example.py` & `motor-3.2.0/doc/examples/aiohttp_gridfs_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/aiohttp_gridfs_example.rst` & `motor-3.2.0/doc/examples/aiohttp_gridfs_example.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/authentication.rst` & `motor-3.2.0/doc/examples/authentication.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/auto_csfle_example.py` & `motor-3.2.0/doc/examples/auto_csfle_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/bulk.rst` & `motor-3.2.0/doc/examples/bulk.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/encryption.rst` & `motor-3.2.0/doc/examples/encryption.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/explicit_encryption_automatic_decryption_example.py` & `motor-3.2.0/doc/examples/explicit_encryption_automatic_decryption_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/explicit_encryption_example.py` & `motor-3.2.0/doc/examples/explicit_encryption_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/monitoring.rst` & `motor-3.2.0/doc/examples/monitoring.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/monitoring_example.py` & `motor-3.2.0/doc/examples/monitoring_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/server_fle_enforcement_example.py` & `motor-3.2.0/doc/examples/server_fle_enforcement_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/tailable-cursors.rst` & `motor-3.2.0/doc/examples/tailable-cursors.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/tornado_change_stream_example.py` & `motor-3.2.0/doc/examples/tornado_change_stream_example.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/tornado_change_stream_example.rst` & `motor-3.2.0/doc/examples/tornado_change_stream_example.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/examples/tornado_change_stream_templates/index.html` & `motor-3.2.0/doc/examples/tornado_change_stream_templates/index.html`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/features.rst` & `motor-3.2.0/doc/features.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/index.rst` & `motor-3.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/installation.rst` & `motor-3.2.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/make.bat` & `motor-3.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/migrate-to-motor-2.rst` & `motor-3.2.0/doc/migrate-to-motor-2.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/migrate-to-motor-3.rst` & `motor-3.2.0/doc/migrate-to-motor-3.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/mongo_extensions.py` & `motor-3.2.0/doc/mongo_extensions.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/motor_extensions.py` & `motor-3.2.0/doc/motor_extensions.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/pydoctheme/static/pydoctheme.css` & `motor-3.2.0/doc/pydoctheme/static/pydoctheme.css`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/pydoctheme/theme.conf` & `motor-3.2.0/doc/pydoctheme/theme.conf`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/requirements.rst` & `motor-3.2.0/doc/requirements.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Requirements
 ============
 
 The current version of Motor requires:
 
 * CPython 3.7 and later.
-* PyMongo_ 4.2 and later.
+* PyMongo_ 4.4 and later.
 
 Motor can integrate with either Tornado or asyncio.
 
 The default authentication mechanism for MongoDB 3.0+ is SCRAM-SHA-1.
 
 Building the docs requires `sphinx`_.
 
@@ -47,47 +47,51 @@
 +-------------------+-----------------+
 | 2.5               | 3.12+           |
 +-------------------+-----------------+
 | 3.0               | 4.1+            |
 +-------------------+-----------------+
 | 3.1               | 4.2+            |
 +-------------------+-----------------+
+| 3.2               | 4.4+            |
++-------------------+-----------------+
 
 Motor and MongoDB
 `````````````````
 
-+---------------------------------------------------------------------------------------+
-|                                  MongoDB Version                                      |
-+=====================+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+
-|                     | 2.2 | 2.4 | 2.6 | 3.0 | 3.2 | 3.4 | 3.6 | 4.0 | 4.2 | 4.4 | 5.0 |
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-| Motor Version | 1.0 |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 1.1 |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 1.2 |**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 1.3 |**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.0 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.1 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.2 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.3 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.4 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 2.5 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 3.0 |**N**|**N**|**N**|**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
-|               | 3.1 |**N**|**N**|**N**|**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |
-+---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
++---------------------------------------------------------------------------------------------------+
+|                                  MongoDB Version                                                  |
++=====================+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+=====+
+|                     | 2.2 | 2.4 | 2.6 | 3.0 | 3.2 | 3.4 | 3.6 | 4.0 | 4.2 | 4.4 | 5.0 | 6.0 | 7.0 |
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+| Motor Version | 1.0 |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 1.1 |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 1.2 |**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 1.3 |**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.0 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.1 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.2 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.3 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.4 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 2.5 |**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 3.0 |**N**|**N**|**N**|**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |**N**|**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 3.1 |**N**|**N**|**N**|**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
+|               | 3.2 |**N**|**N**|**N**|**N**|**N**|**N**|  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |  Y  |
++---------------+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+-----+
 
 There is no relationship between PyMongo and MongoDB version numbers, although
 the numbers happen to be close or equal in recent releases of PyMongo and MongoDB.
 Use `the PyMongo compatibility matrix`_ to determine what MongoDB version is
 supported by PyMongo. Use the compatibility matrix above to determine what
 MongoDB version Motor supports.
 
@@ -120,14 +124,16 @@
 +---------------+-----+-----+-----+-----+-----+
 |               | 2.3 |**N**|**N**|  Y  |  Y  |
 +---------------+-----+-----+-----+-----+-----+
 |               | 3.0 |**N**|**N**|**N**|  Y  |
 +---------------+-----+-----+-----+-----+-----+
 |               | 3.1 |**N**|**N**|**N**|  Y  |
 +---------------+-----+-----+-----+-----+-----+
+|               | 3.2 |**N**|**N**|**N**|  Y  |
++---------------+-----+-----+-----+-----+-----+
 
 Motor and Python
 ````````````````
 
 Motor 1.2 dropped support for the short-lived version of
 the "async for" protocol implemented in Python 3.5.0 and 3.5.1. Motor continues
 to work with "async for" loops in Python 3.5.2 and later.
@@ -168,12 +174,14 @@
 +---------------+-----+-----+-----+-----+-------+-------+-----+-----+-----+-----+-----+-----+
 |               | 2.5 |**N**|**N**|**N**|**N**  |  Y    |  Y  |  Y  |  Y  |  Y  |  Y  |**N**|
 +---------------+-----+-----+-----+-----+-------+-------+-----+-----+-----+-----+-----+-----+
 |               | 3.0 |**N**|**N**|**N**|**N**  |**N**  |**N**|  Y  |  Y  |  Y  |  Y  |**N**|
 +---------------+-----+-----+-----+-----+-------+-------+-----+-----+-----+-----+-----+-----+
 |               | 3.1 |**N**|**N**|**N**|**N**  |**N**  |**N**|  Y  |  Y  |  Y  |  Y  |**Y**|
 +---------------+-----+-----+-----+-----+-------+-------+-----+-----+-----+-----+-----+-----+
+|               | 3.2 |**N**|**N**|**N**|**N**  |**N**  |**N**|  Y  |  Y  |  Y  |  Y  |**Y**|
++---------------+-----+-----+-----+-----+-------+-------+-----+-----+-----+-----+-----+-----+
 
 Not Supported
 -------------
 
 Motor does not support Jython or IronPython.
```

### Comparing `motor-3.1.2/doc/static/sidebar.js` & `motor-3.2.0/doc/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/tutorial-asyncio.rst` & `motor-3.2.0/doc/tutorial-asyncio.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/doc/tutorial-tornado.rst` & `motor-3.2.0/doc/tutorial-tornado.rst`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/__init__.py` & `motor-3.2.0/motor/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Motor, an asynchronous driver for MongoDB."""
 
-version_tuple = (3, 1, 2)
+from ._version import get_version_string, version, version_tuple  # noqa
 
-
-def get_version_string():
-    return ".".join(map(str, version_tuple))
-
-
-version = get_version_string()
 """Current version of Motor."""
 
 
 try:
     import tornado
 except ImportError:
     tornado = None
```

### Comparing `motor-3.1.2/motor/aiohttp/__init__.py` & `motor-3.2.0/motor/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/core.py` & `motor-3.2.0/motor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         batch_size=None,
         collation=None,
         start_at_operation_time=None,
         session=None,
         start_after=None,
         comment=None,
         full_document_before_change=None,
+        show_expanded_events=None,
     ):
         """Watch changes on this cluster.
 
         Returns a :class:`~MotorChangeStream` cursor which iterates over changes
         on all databases in this cluster. Introduced in MongoDB 4.0.
 
         See the documentation for :meth:`MotorCollection.watch` for more
@@ -210,18 +211,22 @@
           - `start_after` (optional): The same as `resume_after` except that
             `start_after` can resume notifications after an invalidate event.
             This option and `resume_after` are mutually exclusive.
           - `comment` (optional): A user-provided comment to attach to this
             command.
           - `full_document_before_change`: Allowed values: `whenAvailable` and `required`. Change events
              may now result in a `fullDocumentBeforeChange` response field.
+          - `show_expanded_events` (optional): Include expanded events such as DDL events like `dropIndexes`.
 
         :Returns:
           A :class:`~MotorChangeStream`.
 
+        .. versionchanged:: 3.2
+           Added ``show_expanded_events`` parameter.
+
         .. versionchanged:: 3.1
            Added ``full_document_before_change`` parameter.
 
         .. versionchanged:: 3.0
            Added ``comment`` parameter.
 
         .. versionchanged:: 2.1
@@ -245,14 +250,15 @@
             batch_size,
             collation,
             start_at_operation_time,
             session,
             start_after,
             comment,
             full_document_before_change,
+            show_expanded_events,
         )
 
     def __getattr__(self, name):
         if name.startswith("_"):
             raise AttributeError(
                 "%s has no attribute %r. To access the %s"
                 " database, use client['%s']." % (self.__class__.__name__, name, name, name)
@@ -609,15 +615,15 @@
 
         # Latent cursor that will send initial command on first "async for".
         return cursor_class(
             self["$cmd.aggregate"],
             self._async_aggregate,
             pipeline,
             *unwrap_args_session(args),
-            **unwrap_kwargs_session(kwargs)
+            **unwrap_kwargs_session(kwargs),
         )
 
     def watch(
         self,
         pipeline=None,
         full_document=None,
         resume_after=None,
@@ -625,14 +631,15 @@
         batch_size=None,
         collation=None,
         start_at_operation_time=None,
         session=None,
         start_after=None,
         comment=None,
         full_document_before_change=None,
+        show_expanded_events=None,
     ):
         """Watch changes on this database.
 
         Returns a :class:`~MotorChangeStream` cursor which iterates over changes
         on this database. Introduced in MongoDB 4.0.
 
         See the documentation for :meth:`MotorCollection.watch` for more
@@ -669,18 +676,22 @@
           - `start_after` (optional): The same as `resume_after` except that
             `start_after` can resume notifications after an invalidate event.
             This option and `resume_after` are mutually exclusive.
           - `comment` (optional): A user-provided comment to attach to this
             command.
           - `full_document_before_change`: Allowed values: `whenAvailable` and `required`. Change events
              may now result in a `fullDocumentBeforeChange` response field.
+          - `show_expanded_events` (optional): Include expanded events such as DDL events like `dropIndexes`.
 
         :Returns:
           A :class:`~MotorChangeStream`.
 
+        .. versionchanged:: 3.2
+           Added ``show_expanded_events`` parameter.
+
         .. versionchanged:: 3.1
            Added ``full_document_before_change`` parameter.
 
         .. versionchanged:: 3.0
            Added ``comment`` parameter.
 
         .. versionchanged:: 2.1
@@ -704,14 +715,15 @@
             batch_size,
             collation,
             start_at_operation_time,
             session,
             start_after,
             comment,
             full_document_before_change,
+            show_expanded_events,
         )
 
     @property
     def client(self):
         """This MotorDatabase's :class:`MotorClient`."""
         return self._client
 
@@ -997,15 +1009,15 @@
 
         # Latent cursor that will send initial command on first "async for".
         return cursor_class(
             self,
             self._async_aggregate,
             pipeline,
             *unwrap_args_session(args),
-            **unwrap_kwargs_session(kwargs)
+            **unwrap_kwargs_session(kwargs),
         )
 
     def aggregate_raw_batches(self, pipeline, **kwargs):
         """Perform an aggregation and retrieve batches of raw BSON.
 
         Similar to the :meth:`aggregate` method but returns each batch as bytes.
 
@@ -1043,14 +1055,15 @@
         batch_size=None,
         collation=None,
         start_at_operation_time=None,
         session=None,
         start_after=None,
         comment=None,
         full_document_before_change=None,
+        show_expanded_events=None,
     ):
         """Watch changes on this collection.
 
         Performs an aggregation with an implicit initial ``$changeStream``
         stage and returns a :class:`~MotorChangeStream` cursor which
         iterates over changes on this collection.
 
@@ -1142,20 +1155,24 @@
           - `start_after` (optional): The same as `resume_after` except that
             `start_after` can resume notifications after an invalidate event.
             This option and `resume_after` are mutually exclusive.
           - `comment` (optional): A user-provided comment to attach to this
             command.
           - `full_document_before_change`: Allowed values: `whenAvailable` and `required`. Change events
              may now result in a `fullDocumentBeforeChange` response field.
+          - `show_expanded_events` (optional): Include expanded events such as DDL events like `dropIndexes`.
 
         :Returns:
           A :class:`~MotorChangeStream`.
 
         See the :ref:`tornado_change_stream_example`.
 
+        .. versionchanged:: 3.2
+           Added ``show_expanded_events`` parameter.
+
         .. versionchanged:: 3.1
            Added ``full_document_before_change`` parameter.
 
         .. versionchanged:: 3.0
            Added ``comment`` parameter.
 
         .. versionchanged:: 2.1
@@ -1182,14 +1199,15 @@
             batch_size,
             collation,
             start_at_operation_time,
             session,
             start_after,
             comment,
             full_document_before_change,
+            show_expanded_events,
         )
 
     def list_indexes(self, session=None, **kwargs):
         """Get a cursor over the index documents for this collection. ::
 
           async def print_indexes():
               async for index in db.test.list_indexes():
@@ -1782,14 +1800,15 @@
         batch_size,
         collation,
         start_at_operation_time,
         session,
         start_after,
         comment,
         full_document_before_change,
+        show_expanded_events,
     ):
         super().__init__(delegate=None)
         # The "target" object is a client, database, or collection.
         self._target = target
         self._kwargs = {
             "pipeline": pipeline,
             "full_document": full_document,
@@ -1798,14 +1817,15 @@
             "batch_size": batch_size,
             "collation": collation,
             "start_at_operation_time": start_at_operation_time,
             "session": session,
             "start_after": start_after,
             "comment": comment,
             "full_document_before_change": full_document_before_change,
+            "show_expanded_events": show_expanded_events,
         }
 
     def _lazy_init(self):
         if not self.delegate:
             self.delegate = self._target.delegate.watch(**unwrap_kwargs_session(self._kwargs))
 
     def _try_next(self):
@@ -1955,14 +1975,16 @@
     # Key Management API
     rewrap_many_data_key = AsyncCommand()
     delete_key = AsyncCommand()
     get_key = AsyncCommand()
     add_key_alt_name = AsyncCommand()
     get_key_by_alt_name = AsyncCommand()
     remove_key_alt_name = AsyncCommand()
+    if hasattr(ClientEncryption, "encrypt_expression"):
+        encrypt_expression = AsyncCommand()
 
     def __init__(
         self,
         kms_providers,
         key_vault_namespace,
         key_vault_client,
         codec_options,
@@ -2010,7 +2032,88 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     async def get_keys(self):
         cursor_class = create_class_with_framework(AgnosticCursor, self._framework, self.__module__)
         return cursor_class(self.delegate.get_keys(), self)
+
+    async def create_encrypted_collection(
+        self,
+        database,
+        name,
+        encrypted_fields,
+        kms_provider=None,
+        master_key=None,
+        **kwargs,
+    ):
+        """Create a collection with encryptedFields.
+
+        .. warning::
+            This function does not update the encryptedFieldsMap in the client's
+            AutoEncryptionOpts, thus the user must create a new client after calling this function with
+            the encryptedFields returned.
+
+        Normally collection creation is automatic. This method should
+        only be used to specify options on
+        creation. :class:`~pymongo.errors.EncryptionError` will be
+        raised if the collection already exists.
+
+        :Parameters:
+          - `database`: the database in which to create a collection
+          - `name`: the name of the collection to create
+          - `encrypted_fields` (dict): Document that describes the encrypted fields for
+            Queryable Encryption. For example::
+
+              {
+                "escCollection": "enxcol_.encryptedCollection.esc",
+                "ecocCollection": "enxcol_.encryptedCollection.ecoc",
+                "fields": [
+                    {
+                        "path": "firstName",
+                        "keyId": Binary.from_uuid(UUID('00000000-0000-0000-0000-000000000000')),
+                        "bsonType": "string",
+                        "queries": {"queryType": "equality"}
+                    },
+                    {
+                        "path": "ssn",
+                        "keyId": Binary.from_uuid(UUID('04104104-1041-0410-4104-104104104104')),
+                        "bsonType": "string"
+                    }
+                  ]
+              }
+
+            The "keyId" may be set to ``None`` to auto-generate the data keys.
+          - `kms_provider` (optional): the KMS provider to be used
+          - `master_key` (optional): Identifies a KMS-specific key used to encrypt the
+            new data key. If the kmsProvider is "local" the `master_key` is
+            not applicable and may be omitted.
+          - `**kwargs` (optional): additional keyword arguments are the same as "create_collection".
+
+        All optional `create collection command`_ parameters should be passed
+        as keyword arguments to this method.
+        See the documentation for :meth:`~pymongo.database.Database.create_collection` for all valid options.
+
+        :Raises:
+          - :class:`~pymongo.errors.EncryptedCollectionError`: When either data-key creation or creating the collection fails.
+
+        .. versionadded:: 3.2
+
+        .. _create collection command:
+            https://mongodb.com/docs/manual/reference/command/create
+
+        """
+        collection_class = create_class_with_framework(
+            AgnosticCollection, self._framework, self.__module__
+        )
+        loop = self.get_io_loop()
+        coll, ef = await self._framework.run_on_executor(
+            loop,
+            self.delegate.create_encrypted_collection,
+            database=database.delegate,
+            name=name,
+            encrypted_fields=encrypted_fields,
+            kms_provider=kms_provider,
+            master_key=master_key,
+            **kwargs,
+        )
+        return collection_class(database, coll.name, _delegate=coll), ef
```

### Comparing `motor-3.1.2/motor/docstrings.py` & `motor-3.2.0/motor/docstrings.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,18 +325,18 @@
 command document before it is sent.
 
 For example, a command like ``{buildinfo: 1}`` can be sent
 using::
 
     result = await db.command("buildinfo")
 
-For a command where the value matters, like ``{collstats:
+For a command where the value matters, like ``{count:
 collection_name}`` we can do::
 
-    result = await db.command("collstats", collection_name)
+    result = await db.command("count", collection_name)
 
 For commands that take additional arguments we can use
 kwargs. So ``{filemd5: object_id, root: file_root}`` becomes::
 
     result = await db.command("filemd5", object_id, root=file_root)
 
 :Parameters:
```

### Comparing `motor-3.1.2/motor/frameworks/asyncio/__init__.py` & `motor-3.2.0/motor/frameworks/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/frameworks/tornado/__init__.py` & `motor-3.2.0/motor/frameworks/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/metaprogramming.py` & `motor-3.2.0/motor/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/motor_asyncio.py` & `motor-3.2.0/motor/motor_asyncio.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/motor_common.py` & `motor-3.2.0/motor/motor_common.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/motor_gridfs.py` & `motor-3.2.0/motor/motor_gridfs.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/motor_tornado.py` & `motor-3.2.0/motor/motor_tornado.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor/web.py` & `motor-3.2.0/motor/web.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/motor.egg-info/PKG-INFO` & `motor-3.2.0/motor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motor
-Version: 3.1.2
+Version: 3.2.0
 Summary: Non-blocking MongoDB driver for Tornado or asyncio
 Home-page: https://github.com/mongodb/motor/
 Author: A. Jesse Jiryu Davis
 Author-email: jesse@mongodb.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: mongo,mongodb,pymongo,gridfs,bson,motor,tornado,asyncio
 Classifier: Intended Audience :: Developers
@@ -68,16 +68,15 @@
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongo, please look into
 our `support channels <https://support.mongodb.com/welcome>`_. Please
 do not email any of the Motor developers directly with issues or
-questions - you're more likely to get an answer on the `MongoDB Community
-Forums <https://developer.mongodb.com/community/forums/tag/motor-driver>`_.
+questions - you're more likely to get an answer on the `StackOverflow <https://stackoverflow.com/questions/tagged/mongodb>`_ (using a "mongodb" tag).
 
 Bugs / Feature Requests
 =======================
 
 Think you've found a bug? Want to see a new feature in Motor? Please open a
 case in our issue management tool, JIRA:
 
@@ -189,14 +188,20 @@
 =============
 
 Motor's documentation is on ReadTheDocs_.
 
 Build the documentation with Python 3.7+. Install sphinx_, Tornado_, and aiohttp_,
 and do ``cd doc; make html``.
 
+Learning Resources
+==================
+
+MongoDB Learn - `Python courses <https://learn.mongodb.com/catalog?labels=%5B%22Language%22%5D&values=%5B%22Python%22%5D>`_.
+`Python Articles on Developer Center <https://www.mongodb.com/developer/languages/python/>`_.
+
 Testing
 =======
 
 Run ``python setup.py test``.
 Tests are located in the ``test/`` directory.
 
 .. _PyMongo: http://pypi.python.org/pypi/pymongo/
```

### Comparing `motor-3.1.2/motor.egg-info/SOURCES.txt` & `motor-3.2.0/motor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 doc/examples/tornado_change_stream_example.py
 doc/examples/tornado_change_stream_example.rst
 doc/examples/tornado_change_stream_templates/index.html
 doc/pydoctheme/theme.conf
 doc/pydoctheme/static/pydoctheme.css
 doc/static/sidebar.js
 motor/__init__.py
+motor/_version.py
 motor/core.py
 motor/docstrings.py
 motor/metaprogramming.py
 motor/motor_asyncio.py
 motor/motor_common.py
 motor/motor_gridfs.py
 motor/motor_tornado.py
```

### Comparing `motor-3.1.2/setup.py` & `motor-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 """
 
 description = "Non-blocking MongoDB driver for Tornado or asyncio"
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
-pymongo_ver = ">=4.1,<5"
+pymongo_ver = ">=4.4,<5"
 
 install_requires = ["pymongo" + pymongo_ver]
 
 extras_require = {
     "encryption": ["pymongo[encryption]" + pymongo_ver],
     "ocsp": ["pymongo[ocsp]" + pymongo_ver],
     "snappy": ["pymongo[snappy]" + pymongo_ver],
@@ -145,17 +145,23 @@
     "motor.frameworks",
     "motor.frameworks.tornado",
     "motor.frameworks.asyncio",
     "motor.aiohttp",
 ]
 
 
+version_ns = {}
+with open("motor/_version.py") as fp:
+    exec(fp.read(), version_ns)
+version = version_ns["version"]
+
+
 setup(
     name="motor",
-    version="3.1.2",
+    version=version,
     packages=packages,
     description=description,
     long_description=long_description,
     author="A. Jesse Jiryu Davis",
     author_email="jesse@mongodb.com",
     url="https://github.com/mongodb/motor/",
     python_requires=">=3.7",
```

### Comparing `motor-3.1.2/synchro/__init__.py` & `motor-3.2.0/synchro/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 DO NOT USE THIS MODULE.
 """
 
 import functools
 import inspect
 import unittest
+from typing import Generic, TypeVar
 
 # Make e.g. "from pymongo.errors import AutoReconnect" work. Note that
 # importing * won't pick up underscore-prefixed attrs.
 from gridfs import *
 from gridfs import _disallow_transactions
 from gridfs.errors import *
 from gridfs.grid_file import (
@@ -49,23 +50,25 @@
     event_loggers,
     message,
     operations,
     read_preferences,
     saslprep,
     server_selectors,
     server_type,
+    srv_resolver,
     ssl_support,
     write_concern,
 )
 
 # Added for API compat with pymongo.
 try:
     from pymongo import _csot
 except ImportError:
     pass
+from pymongo import client_session
 from pymongo.auth import *
 from pymongo.auth import _build_credentials_tuple, _password_digest
 from pymongo.client_session import TransactionOptions, _TxnState
 from pymongo.collation import *
 from pymongo.common import *
 from pymongo.common import _MAX_END_SESSIONS, _UUID_REPRESENTATIONS
 from pymongo.compression_support import _HAVE_SNAPPY, _HAVE_ZLIB, _HAVE_ZSTD
@@ -99,14 +102,15 @@
 from pymongo.read_preferences import _ServerMode
 from pymongo.results import *
 from pymongo.results import _WriteResult
 from pymongo.saslprep import *
 from pymongo.server import *
 from pymongo.server_selectors import *
 from pymongo.settings import *
+from pymongo.srv_resolver import _resolve, _SrvResolver
 from pymongo.ssl_support import *
 from pymongo.topology import *
 from pymongo.topology_description import *
 from pymongo.uri_parser import *
 from pymongo.uri_parser import _HAVE_DNSPYTHON
 from pymongo.write_concern import *
 from tornado.ioloop import IOLoop
@@ -334,15 +338,18 @@
                 return async_method(*args, **kwargs)
 
             return IOLoop.current().run_sync(partial)
 
         return synchronized_method
 
 
-class MongoClient(Synchro):
+_T = TypeVar("_T")
+
+
+class MongoClient(Synchro, Generic[_T]):
     __delegate_class__ = motor.MotorClient
     HOST = "localhost"
     PORT = 27017
 
     get_database = WrapOutgoing()
     max_pool_size = SynchroProperty()
     start_session = Sync()
@@ -764,14 +771,17 @@
             kms_providers, key_vault_namespace, key_vault_client=key_vault_client, **kwargs
         )
 
 
 class ClientEncryption(Synchro):
     __delegate_class__ = motor.MotorClientEncryption
 
+    _enc_col = Sync("create_encrypted_collection")
+    encrypt_expression = Sync("encrypt_expression")
+
     def __init__(
         self,
         kms_providers,
         key_vault_namespace,
         key_vault_client,
         codec_options,
         kms_tls_options=None,
@@ -788,7 +798,26 @@
         return self
 
     def __exit__(self, *args):
         return self.synchronize(self.delegate.__aexit__)(*args)
 
     def get_keys(self):
         return Cursor(self.synchronize(self.delegate.get_keys)())
+
+    def create_encrypted_collection(
+        self,
+        database,
+        name,
+        encrypted_fields,
+        kms_provider=None,
+        master_key=None,
+        **kwargs,
+    ):
+        coll, ef = self.synchronize(self.delegate.create_encrypted_collection)(
+            database=database.delegate,
+            name=name,
+            encrypted_fields=encrypted_fields,
+            kms_provider=kms_provider,
+            master_key=master_key,
+            **kwargs,
+        )
+        return Collection(database, coll.name, delegate=coll), ef
```

### Comparing `motor-3.1.2/synchro/synchrotest.py` & `motor-3.2.0/synchro/synchrotest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 This program monkey-patches sys.modules, so run it alone, rather than as part
 of a larger test suite.
 """
 
 import importlib
 import importlib.abc
 import importlib.machinery
+import re
 import sys
 
 import nose
 from nose.config import Config
 from nose.plugins import Plugin
 from nose.plugins.manager import PluginManager
 from nose.plugins.skip import Skip
@@ -44,16 +45,16 @@
     "test.test_replica_set_reconfig",
     # Accesses PyMongo internals.
     "test.test_retryable_writes",
     # Accesses PyMongo internals. Tested directly in Motor.
     "test.test_session",
     # Deprecated in PyMongo, removed in Motor 2.0.
     "test.test_gridfs",
-    # Skip mypy tests.
-    "test.test_mypy",
+    # Skip mypy/typing tests.
+    "test.test_typing",
 ]
 
 
 excluded_tests = [
     # Motor's reprs aren't the same as PyMongo's.
     "*.test_repr",
     "TestClient.test_unix_socket",
@@ -122,14 +123,15 @@
     "TestCollation.*",
     "TestCollection.test_find_one_and_write_concern",
     "TestCollection.test_write_error_text_handling",
     "TestBinary.test_uuid_queries",
     "TestCursor.test_comment",
     "TestCursor.test_where",
     "TestGridfs.test_gridfs_find",
+    "TestKmsTLSOptions.test_05_tlsDisableOCSPEndpointCheck_is_permitted",
     # Tests that use "authenticate" or "logoout", removed in Motor 2.0.
     "TestSASLPlain.test_sasl_plain_bad_credentials",
     "TestSCRAM.test_scram",
     "TestSCRAMSHA1.test_scram_sha1",
     # Uses "collection_names", deprecated in PyMongo, removed in Motor 2.0.
     "TestSingleSecondaryOk.test_reads_from_secondary",
     # Slow.
@@ -168,24 +170,28 @@
     "*.test_iteration",
     # MD5 is deprecated
     "*.test_md5",
     # Causes a deadlock.
     "TestFork.*",
     # Also causes a deadlock.
     "TestClientSimple.test_fork",
+    # This method requires credentials.
+    "TestOnDemandAWSCredentials.test_02_success",
     # These methods are picked up by nose despite not being a unittest.
     "TestRewrapWithSeparateClientEncryption.run_test",
     "TestCustomEndpoint.run_test_expected_success",
     "TestDataKeyDoubleEncryption.run_test",
     # Motor does not support CSOT.
     "TestCsotGridfsFind.*",
     # These tests are failing right now.
     "TestUnifiedFindShutdownError.test_Concurrent_shutdown_error_on_find",
     "TestUnifiedInsertShutdownError.test_Concurrent_shutdown_error_on_insert",
     "TestUnifiedPoolClearedError.test_PoolClearedError_does_not_mark_server_unknown",
+    # These tests have hard-coded values that differ from motor.
+    "TestClient.test_handshake.*",
 ]
 
 
 excluded_modules_matched = set()
 excluded_tests_matched = set()
 
 
@@ -251,19 +257,23 @@
         if method.__name__ in ("run_test_ops", "maybe_skip_test"):
             return False
 
         for excluded_name in excluded_tests:
             classname = method.__self__.__class__.__name__
 
             # Should we exclude this method's whole TestCase?
-            suite_name, method_name = excluded_name.split(".")
+            suite_name, _, method_name = excluded_name.partition(".")
             suite_matches = suite_name in [classname, "*"]
 
             # Should we exclude this particular method?
-            method_matches = method.__name__ == method_name or method_name == "*"
+            method_matches = (
+                method.__name__ == method_name
+                or method_name == "*"
+                or re.match(f"^{method_name}$", method.__name__)
+            )
 
             if suite_matches and method_matches:
                 excluded_tests_matched.add(excluded_name)
                 return False
 
         return True
 
@@ -330,14 +340,15 @@
         "pymongo.command_cursor",
         "pymongo.change_stream",
         "pymongo.cursor",
         "pymongo.encryption",
         "pymongo.encryption_options",
         "pymongo.mongo_client",
         "pymongo.database",
+        "pymongo.srv_resolver",
         "gridfs",
         "gridfs.grid_file",
     ]:
         sys.modules.pop(n)
 
     if "--check-exclude-patterns" in sys.argv:
         check_exclude_patterns = True
```

### Comparing `motor-3.1.2/test/__init__.py` & `motor-3.2.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/assert_logs_backport.py` & `motor-3.2.0/test/assert_logs_backport.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/__init__.py` & `motor-3.2.0/test/asyncio_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,31 +91,32 @@
             raise SkipTest("mongod doesn't support SSL, or is down")
 
         self.cx = self.asyncio_client()
         self.db = self.cx.motor_test
         self.collection = self.db.test_collection
         self.loop.run_until_complete(self.collection.drop())
 
-    def get_client_kwargs(self, **kwargs):
+    def get_client_kwargs(self, set_loop=True, **kwargs):
+        if set_loop:
+            kwargs.setdefault("io_loop", self.loop)
         if env.mongod_started_with_ssl:
             kwargs.setdefault("tlsCAFile", CA_PEM)
             kwargs.setdefault("tlsCertificateKeyFile", CLIENT_PEM)
-
         kwargs.setdefault("tls", env.mongod_started_with_ssl)
-        kwargs.setdefault("io_loop", self.loop)
-
         return kwargs
 
-    def asyncio_client(self, uri=None, *args, **kwargs):
+    def asyncio_client(self, uri=None, *args, set_loop=True, **kwargs):
         """Get an AsyncIOMotorClient.
 
         Ignores self.ssl, you must pass 'ssl' argument.
         """
         return motor_asyncio.AsyncIOMotorClient(
-            uri or env.uri, *args, **self.get_client_kwargs(**kwargs)
+            kwargs.pop("host", None) or uri or env.uri,
+            *args,
+            **self.get_client_kwargs(**kwargs, set_loop=set_loop)
         )
 
     def asyncio_rsc(self, uri=None, *args, **kwargs):
         """Get an open MotorClient for replica set.
 
         Ignores self.ssl, you must pass 'ssl' argument.
         """
```

### Comparing `motor-3.1.2/test/asyncio_tests/test_aiohttp_gridfs.py` & `motor-3.2.0/test/asyncio_tests/test_aiohttp_gridfs.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_await.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_await.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_basic.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_basic.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_change_stream.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_change_stream.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_client.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_client.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_collection.py` & `motor-3.2.0/test/tornado_tests/test_motor_collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,132 @@
-# Copyright 2014 MongoDB, Inc.
+# Copyright 2012-2015 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Test AsyncIOMotorCollection."""
+"""Test Motor, an asynchronous driver for MongoDB and Tornado."""
 
-import asyncio
 import sys
 import traceback
 import unittest
-from test.asyncio_tests import AsyncIOTestCase, asyncio_test
+from test.test_environment import env
+from test.tornado_tests import MotorTest
 from test.utils import ignore_deprecations
 
+import pymongo.errors
 from bson import CodecOptions
 from bson.binary import JAVA_LEGACY
 from pymongo import ReadPreference, WriteConcern
+from pymongo.encryption import Algorithm, QueryType
 from pymongo.errors import BulkWriteError, DuplicateKeyError, OperationFailure
 from pymongo.read_concern import ReadConcern
 from pymongo.read_preferences import Secondary
+from tornado import gen
+from tornado.testing import gen_test
 
-from motor.motor_asyncio import AsyncIOMotorCollection
+import motor
+import motor.motor_tornado
 
+if pymongo.version_tuple >= (4, 4, 0):
+    from pymongo.encryption_options import RangeOpts
 
-class TestAsyncIOCollection(AsyncIOTestCase):
-    @asyncio_test
+
+class MotorCollectionTest(MotorTest):
+    @gen_test
     async def test_collection(self):
         # Test that we can create a collection directly, not just from
-        # database accessors.
-        collection = AsyncIOMotorCollection(self.db, "test_collection")
+        # MotorClient's accessors
+        collection = motor.MotorCollection(self.db, "test_collection")
 
         # Make sure we got the right collection and it can do an operation
         self.assertEqual("test_collection", collection.name)
-        await collection.delete_many({})
         await collection.insert_one({"_id": 1})
         doc = await collection.find_one({"_id": 1})
         self.assertEqual(1, doc["_id"])
 
         # If you pass kwargs to PyMongo's Collection(), it calls
         # db.create_collection(). Motor can't do I/O in a constructor
         # so this is prohibited.
-        self.assertRaises(
-            TypeError, AsyncIOMotorCollection, self.db, "test_collection", capped=True
-        )
+        self.assertRaises(TypeError, motor.MotorCollection, self.db, "test_collection", capped=True)
 
-    @asyncio_test
+    @gen_test
     async def test_dotted_collection_name(self):
         # Ensure that remove, insert, and find work on collections with dots
         # in their names.
         for coll in (self.db.foo.bar, self.db.foo.bar.baz):
             await coll.delete_many({})
             result = await coll.insert_one({"_id": "xyzzy"})
             self.assertEqual("xyzzy", result.inserted_id)
             result = await coll.find_one({"_id": "xyzzy"})
             self.assertEqual(result["_id"], "xyzzy")
             await coll.delete_many({})
-            resp = await coll.find_one({"_id": "xyzzy"})
-            self.assertEqual(None, resp)
+            self.assertEqual(None, (await coll.find_one({"_id": "xyzzy"})))
 
     def test_call(self):
         # Prevents user error with nice message.
         try:
             self.db.foo()
         except TypeError as e:
             self.assertTrue("no such method exists" in str(e))
         else:
             self.fail("Expected TypeError")
 
     @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_update(self):
         await self.collection.insert_one({"_id": 1})
         result = await self.collection.update_one({"_id": 1}, {"$set": {"foo": "bar"}})
 
         self.assertIsNone(result.upserted_id)
         self.assertEqual(1, result.modified_count)
 
     @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_update_bad(self):
         # Violate a unique index, make sure we handle error well
         coll = self.db.unique_collection
         await coll.create_index("s", unique=True)
 
         try:
             await coll.insert_many([{"s": 1}, {"s": 2}])
             with self.assertRaises(DuplicateKeyError):
                 await coll.update_one({"s": 2}, {"$set": {"s": 1}})
 
         finally:
             await coll.drop()
 
-    @asyncio_test
+    @gen_test
     async def test_insert_one(self):
         collection = self.collection
         result = await collection.insert_one({"_id": 201})
         self.assertEqual(201, result.inserted_id)
 
     @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_insert_many_one_bad(self):
         collection = self.collection
         await collection.insert_one({"_id": 2})
 
         # Violate a unique index in one of many updates, handle error.
         with self.assertRaises(BulkWriteError):
             await collection.insert_many([{"_id": 1}, {"_id": 2}, {"_id": 3}])  # Already exists
 
         # First insert should have succeeded, but not second or third.
         self.assertEqual(set([1, 2]), set((await collection.distinct("_id"))))
 
-    @asyncio_test
+    @gen_test
     async def test_delete_one(self):
         # Remove a document twice, check that we get a success responses
         # and n = 0 for the second time.
         await self.collection.insert_one({"_id": 1})
         result = await self.collection.delete_one({"_id": 1})
 
         # First time we remove, n = 1
@@ -133,70 +137,73 @@
         result = await self.collection.delete_one({"_id": 1})
 
         # Second time, document is already gone, n = 0
         self.assertEqual(0, result.raw_result["n"])
         self.assertEqual(1, result.raw_result["ok"])
         self.assertEqual(None, result.raw_result.get("err"))
 
-    @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_unacknowledged_insert(self):
+        # Test that unacknowledged inserts complete eventually.
+
         coll = self.db.test_unacknowledged_insert
         await coll.with_options(write_concern=WriteConcern(0)).insert_one({"_id": 1})
 
         # The insert is eventually executed.
         while not (await coll.count_documents({})):
-            await asyncio.sleep(0.1)
+            await gen.sleep(0.1)
 
-    @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_unacknowledged_update(self):
+        # Test that unacknowledged updates complete eventually.
         coll = self.collection
 
         await coll.insert_one({"_id": 1})
         await coll.with_options(write_concern=WriteConcern(0)).update_one(
             {"_id": 1}, {"$set": {"a": 1}}
         )
 
         while not (await coll.find_one({"a": 1})):
-            await asyncio.sleep(0.1)
+            await gen.sleep(0.1)
 
     @ignore_deprecations
-    @asyncio_test
+    @gen_test
     async def test_indexes(self):
         test_collection = self.collection
 
         # Create an index
         idx_name = await test_collection.create_index([("foo", 1)])
         index_info = await test_collection.index_information()
         self.assertEqual([("foo", 1)], index_info[idx_name]["key"])
 
         # Don't test drop_index or drop_indexes -- Synchro tests them
 
     async def _make_test_data(self, n):
         await self.db.drop_collection("test")
         await self.db.test.insert_many([{"_id": i} for i in range(n)])
-        expected_sum = sum(range(n))
-        return expected_sum
+        return sum(range(n))
 
     pipeline = [{"$project": {"_id": "$_id"}}]
 
-    @asyncio_test(timeout=30)
+    def assertAllDocs(self, expected_sum, docs):
+        self.assertEqual(expected_sum, sum(doc["_id"] for doc in docs))
+
+    @gen_test(timeout=30)
     async def test_aggregation_cursor(self):
         db = self.db
 
         # A small collection which returns only an initial batch,
         # and a larger one that requires a getMore.
         for collection_size in (10, 1000):
             expected_sum = await self._make_test_data(collection_size)
             cursor = db.test.aggregate(self.pipeline)
             docs = await cursor.to_list(collection_size)
-            self.assertEqual(expected_sum, sum(doc["_id"] for doc in docs))
+            self.assertAllDocs(expected_sum, docs)
 
-    @asyncio_test
+    @gen_test
     async def test_aggregation_cursor_exc_info(self):
         await self._make_test_data(200)
         cursor = self.db.test.aggregate(self.pipeline)
         await cursor.to_list(length=10)
         await self.db.test.drop()
         try:
             await cursor.to_list(length=None)
@@ -205,30 +212,30 @@
 
             # The call tree should include PyMongo code we ran on a thread.
             formatted = "\n".join(traceback.format_tb(tb))
             self.assertTrue(
                 "_unpack_response" in formatted or "_check_command_response" in formatted
             )
 
-    @asyncio_test
+    @gen_test
     async def test_aggregate_cursor_del(self):
         cursor = self.db.test.aggregate(self.pipeline)
         del cursor
         cursor = self.db.test.aggregate(self.pipeline)
         await cursor.close()
         del cursor
 
     def test_with_options(self):
         coll = self.db.test
         codec_options = CodecOptions(tz_aware=True, uuid_representation=JAVA_LEGACY)
 
         write_concern = WriteConcern(w=2, j=True)
         coll2 = coll.with_options(codec_options, ReadPreference.SECONDARY, write_concern)
 
-        self.assertTrue(isinstance(coll2, AsyncIOMotorCollection))
+        self.assertTrue(isinstance(coll2, motor.MotorCollection))
         self.assertEqual(codec_options, coll2.codec_options)
         self.assertEqual(Secondary(), coll2.read_preference)
         self.assertEqual(write_concern, coll2.write_concern)
 
         pref = Secondary([{"dc": "sf"}])
         coll2 = coll.with_options(read_preference=pref)
         self.assertEqual(pref, coll2.read_preference)
@@ -256,10 +263,85 @@
 
         for c in [coll1, coll2, coll3]:
             self.assertEqual(write_concern, c.write_concern)
             self.assertEqual(read_concern, c.read_concern)
             self.assertEqual(read_preference, c.read_preference)
             self.assertEqual(codec_options, c.codec_options)
 
+    @env.require_version_min(7, 0, -1, -1)
+    @env.require_no_standalone
+    @gen_test
+    async def test_async_create_encrypted_collection(self):
+        if pymongo.version_tuple < (4, 4, 0):
+            raise unittest.SkipTest("Requires PyMongo 4.4+")
+        await self.db.drop_collection("test_collection")
+        c = self.collection
+        KMS_PROVIDERS = {"local": {"key": b"\x00" * 96}}
+        self.cx.drop_database("db")
+        async with motor.MotorClientEncryption(
+            KMS_PROVIDERS, "keyvault.datakeys", c, CodecOptions()
+        ) as client_encryption:
+            coll, ef = await client_encryption.create_encrypted_collection(
+                database=self.db,
+                name="testing1",
+                encrypted_fields={"fields": [{"path": "ssn", "bsonType": "string", "keyId": None}]},
+                kms_provider="local",
+            )
+            with self.assertRaises(pymongo.errors.WriteError) as exc:
+                await coll.insert_one({"ssn": "123-45-6789"})
+            self.assertEqual(exc.exception.code, 121)
+            await self.db.drop_collection("testing1", encrypted_fields=ef)
+
+    @gen_test
+    async def test_async_encrypt_expression(self):
+        if pymongo.version_tuple < (4, 4, 0):
+            raise unittest.SkipTest("Requires PyMongo 4.4+")
+        c = self.collection
+        KMS_PROVIDERS = {"local": {"key": b"\x00" * 96}}
+        self.cx.drop_database("db")
+        async with motor.MotorClientEncryption(
+            KMS_PROVIDERS, "keyvault.datakeys", c, CodecOptions()
+        ) as client_encryption:
+            data_key = await client_encryption.create_data_key(
+                "local", key_alt_names=["pymongo_encryption_example_1"]
+            )
+            name = "DoubleNoPrecision"
+            range_opts = RangeOpts(sparsity=1)
+            for i in [6.0, 30.0, 200.0]:
+                insert_payload = await client_encryption.encrypt(
+                    float(i),
+                    key_id=data_key,
+                    algorithm=Algorithm.RANGEPREVIEW,
+                    contention_factor=0,
+                    range_opts=range_opts,
+                )
+                self.collection.insert_one(
+                    {
+                        f"encrypted{name}": insert_payload,
+                    }
+                )
+                self.assertEqual(await client_encryption.decrypt(insert_payload), i)
+
+            find_payload = await client_encryption.encrypt_expression(
+                expression={
+                    "$and": [
+                        {f"encrypted{name}": {"$gte": 6.0}},
+                        {f"encrypted{name}": {"$lte": 200.0}},
+                    ]
+                },
+                key_id=data_key,
+                algorithm=Algorithm.RANGEPREVIEW,
+                query_type=QueryType.RANGEPREVIEW,
+                contention_factor=0,
+                range_opts=range_opts,
+            )
+
+            sorted_find = sorted(
+                await self.collection.explicit_encryption.find(find_payload).to_list(3),
+                key=lambda x: x["_id"],
+            )
+            for elem, expected in zip(sorted_find, [6.0, 30.0, 200.0]):
+                self.assertEqual(elem[f"encrypted{name}"], expected)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_cursor.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_cursor.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_database.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_database.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_encryption.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_encryption.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_grid_file.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_grid_file.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_gridfsbucket.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_gridfsbucket.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_ipv6.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_ipv6.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_replica_set.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_replica_set.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_session.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_session.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_ssl.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_ssl.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_asyncio_tests.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_tests.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/asyncio_tests/test_examples.py` & `motor-3.2.0/test/asyncio_tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 """MongoDB documentation examples with Motor and asyncio."""
 
 import asyncio
 import base64
 import datetime
 import unittest
 from io import StringIO
+from os import environ
 from test import env
 from test.asyncio_tests import AsyncIOTestCase, asyncio_test
 from test.utils import wait_until
+from threading import Thread
 from unittest.mock import patch
 
 import pymongo
 from bson import Binary
 from bson.codec_options import CodecOptions
 from pymongo import WriteConcern
 from pymongo.encryption_options import AutoEncryptionOpts
@@ -897,15 +899,15 @@
         await db.restaurants.insert_one({})
 
         # Start runCommand Example 1
         info = await db.command("buildInfo")
         # End runCommand Example 1
 
         # Start runCommand Example 2
-        stats = await db.command("collStats", "restaurants")
+        count = await db.command("count", "restaurants")
         # End runCommand Example 2
 
     @asyncio_test
     async def test_index_management(self):
         db = self.db
 
         # Start Index Example 1
@@ -1391,16 +1393,17 @@
         """Wait for snapshot reads to become available to prevent this error:
         [246:SnapshotUnavailable]: Unable to read from a snapshot due to pending collection catalog changes; please retry the operation. Snapshot timestamp is Timestamp(1646666892, 4). Collection minimum is Timestamp(1646666892, 5) (on localhost:27017, modern retry, attempt 1)
         From https://github.com/mongodb/mongo-ruby-driver/commit/7c4117b58e3d12e237f7536f7521e18fc15f79ac
         """
         client = collection.database.client
         async with await client.start_session(snapshot=True) as s:
             try:
-                await collection.aggregate([], session=s).to_list(None)
-                return True
+                if await collection.find_one(session=s):
+                    return True
+                return False
             except OperationFailure as e:
                 # Retry them as the server demands...
                 if e.code == 246:  # SnapshotUnavailable
                     return False
                 raise
 
 
@@ -1410,15 +1413,15 @@
 )
 
 
 class TestQueryableEncryptionDocsExample(AsyncIOTestCase):
 
     # Queryable Encryption is not supported on Standalone topology.
 
-    @env.require_version_min(6, 0)
+    @env.require_version_min(7, 0, -1)
     @asyncio_test
     @env.require_replica_set
     async def test_queryable_encryption(self):
         client = self.cx
 
         # MongoClient to use in testing that handles auth/tls/etc,
         # and cleanup.
@@ -1499,7 +1502,60 @@
         unencrypted_coll = unencrypted_client.docs_examples.encrypted
         res = await unencrypted_coll.find_one({"_id": 1})
         assert res is not None
         assert isinstance(res["encrypted_indexed"], Binary)
         assert isinstance(res["encrypted_unindexed"], Binary)
 
         await client_encryption.close()
+
+
+class MotorAWSLambdaExamples(AsyncIOTestCase):
+    def test_shared_client(self):
+        environ.setdefault("MONGODB_URI", "localhost")
+        AsyncIOMotorClient = lambda *args, **kwargs: self.asyncio_client(
+            *args, **kwargs, set_loop=False
+        )
+        # Start AWS Lambda Example 1
+        import asyncio
+        import os
+
+        event_loop = asyncio.new_event_loop()
+        client = AsyncIOMotorClient(host=os.environ["MONGODB_URI"])
+
+        async def async_handler(event, context):
+            return await client.db.command("ping")
+
+        def lambda_handler(event, context):
+            return event_loop.run_until_complete(async_handler(event, context))
+
+        # End AWS Lambda Example 1
+        lambda_handler("event", {})
+        lambda_handler("event", {})
+        lambda_handler("event", {})
+        t = Thread(target=lambda_handler, args=("event", {}))
+        t.start()
+        t.join()
+
+    @unittest.skip("This test needs to be run with valid IAM credentials.")
+    def test_IAM_auth(self):
+        environ.setdefault("MONGODB_URI", "localhost")
+        # Start AWS Lambda Example 2
+        import asyncio
+        import os
+
+        from motor.motor_asyncio import AsyncIOMotorClient
+
+        event_loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(event_loop)
+        client = AsyncIOMotorClient(
+            host=os.environ["MONGODB_URI"],
+            authSource="$external",
+            authMechanism="MONGODB-AWS",
+        )
+
+        async def async_handler(event, context):
+            return await client.db.command("ping")
+
+        def lambda_handler(event, context):
+            return event_loop.run_until_complete(async_handler(event, context))
+
+        # End AWS Lambda Example 2
```

### Comparing `motor-3.1.2/test/certificates/ca.pem` & `motor-3.2.0/test/certificates/ca.pem`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/certificates/client.pem` & `motor-3.2.0/test/certificates/client.pem`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/certificates/server.pem` & `motor-3.2.0/test/certificates/server.pem`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/test_environment.py` & `motor-3.2.0/test/test_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,18 @@
         """Run a test only if the server version is at most ``version``."""
         other_version = Version(*ver)
         return self.require(
             lambda: self.version <= other_version,
             "Server version must be at most %s" % str(other_version),
         )
 
+    def require_no_standalone(self, func):
+        """Run a test only if the client is not connected to a standalone."""
+        return self.require(lambda: not self.is_standalone, "Connected to a standalone", func=func)
+
     def require_replica_set(self, func):
         """Run a test only if the client is connected to a replica set."""
         return self.require(
             lambda: self.is_replica_set, "Not connected to a replica set", func=func
         )
 
     def require_transactions(self, func):
```

### Comparing `motor-3.1.2/test/tornado_tests/__init__.py` & `motor-3.2.0/test/tornado_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_auth.py` & `motor-3.2.0/test/tornado_tests/test_motor_auth.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_await.py` & `motor-3.2.0/test/tornado_tests/test_motor_await.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_basic.py` & `motor-3.2.0/test/tornado_tests/test_motor_basic.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_change_stream.py` & `motor-3.2.0/test/tornado_tests/test_motor_change_stream.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_client.py` & `motor-3.2.0/test/tornado_tests/test_motor_client.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_collection.py` & `motor-3.2.0/test/asyncio_tests/test_asyncio_collection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,134 @@
-# Copyright 2012-2015 MongoDB, Inc.
+# Copyright 2014 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Test Motor, an asynchronous driver for MongoDB and Tornado."""
+"""Test AsyncIOMotorCollection."""
 
+import asyncio
 import sys
 import traceback
 import unittest
-from test.tornado_tests import MotorTest
+from test.asyncio_tests import AsyncIOTestCase, asyncio_test
+from test.test_environment import env
 from test.utils import ignore_deprecations
 
+import pymongo
 from bson import CodecOptions
 from bson.binary import JAVA_LEGACY
 from pymongo import ReadPreference, WriteConcern
+from pymongo.encryption import Algorithm, QueryType
 from pymongo.errors import BulkWriteError, DuplicateKeyError, OperationFailure
 from pymongo.read_concern import ReadConcern
 from pymongo.read_preferences import Secondary
-from tornado import gen
-from tornado.testing import gen_test
 
-import motor
-import motor.motor_tornado
+from motor.motor_asyncio import AsyncIOMotorClientEncryption, AsyncIOMotorCollection
 
+if pymongo.version_tuple >= (4, 4, 0):
+    from pymongo.encryption_options import RangeOpts
 
-class MotorCollectionTest(MotorTest):
-    @gen_test
+
+class TestAsyncIOCollection(AsyncIOTestCase):
+    @asyncio_test
     async def test_collection(self):
         # Test that we can create a collection directly, not just from
-        # MotorClient's accessors
-        collection = motor.MotorCollection(self.db, "test_collection")
+        # database accessors.
+        collection = AsyncIOMotorCollection(self.db, "test_collection")
 
         # Make sure we got the right collection and it can do an operation
         self.assertEqual("test_collection", collection.name)
+        await collection.delete_many({})
         await collection.insert_one({"_id": 1})
         doc = await collection.find_one({"_id": 1})
         self.assertEqual(1, doc["_id"])
 
         # If you pass kwargs to PyMongo's Collection(), it calls
         # db.create_collection(). Motor can't do I/O in a constructor
         # so this is prohibited.
-        self.assertRaises(TypeError, motor.MotorCollection, self.db, "test_collection", capped=True)
+        self.assertRaises(
+            TypeError, AsyncIOMotorCollection, self.db, "test_collection", capped=True
+        )
 
-    @gen_test
+    @asyncio_test
     async def test_dotted_collection_name(self):
         # Ensure that remove, insert, and find work on collections with dots
         # in their names.
         for coll in (self.db.foo.bar, self.db.foo.bar.baz):
             await coll.delete_many({})
             result = await coll.insert_one({"_id": "xyzzy"})
             self.assertEqual("xyzzy", result.inserted_id)
             result = await coll.find_one({"_id": "xyzzy"})
             self.assertEqual(result["_id"], "xyzzy")
             await coll.delete_many({})
-            self.assertEqual(None, (await coll.find_one({"_id": "xyzzy"})))
+            resp = await coll.find_one({"_id": "xyzzy"})
+            self.assertEqual(None, resp)
 
     def test_call(self):
         # Prevents user error with nice message.
         try:
             self.db.foo()
         except TypeError as e:
             self.assertTrue("no such method exists" in str(e))
         else:
             self.fail("Expected TypeError")
 
     @ignore_deprecations
-    @gen_test
+    @asyncio_test
     async def test_update(self):
         await self.collection.insert_one({"_id": 1})
         result = await self.collection.update_one({"_id": 1}, {"$set": {"foo": "bar"}})
 
         self.assertIsNone(result.upserted_id)
         self.assertEqual(1, result.modified_count)
 
     @ignore_deprecations
-    @gen_test
+    @asyncio_test
     async def test_update_bad(self):
         # Violate a unique index, make sure we handle error well
         coll = self.db.unique_collection
         await coll.create_index("s", unique=True)
 
         try:
             await coll.insert_many([{"s": 1}, {"s": 2}])
             with self.assertRaises(DuplicateKeyError):
                 await coll.update_one({"s": 2}, {"$set": {"s": 1}})
 
         finally:
             await coll.drop()
 
-    @gen_test
+    @asyncio_test
     async def test_insert_one(self):
         collection = self.collection
         result = await collection.insert_one({"_id": 201})
         self.assertEqual(201, result.inserted_id)
 
     @ignore_deprecations
-    @gen_test
+    @asyncio_test
     async def test_insert_many_one_bad(self):
         collection = self.collection
         await collection.insert_one({"_id": 2})
 
         # Violate a unique index in one of many updates, handle error.
         with self.assertRaises(BulkWriteError):
             await collection.insert_many([{"_id": 1}, {"_id": 2}, {"_id": 3}])  # Already exists
 
         # First insert should have succeeded, but not second or third.
         self.assertEqual(set([1, 2]), set((await collection.distinct("_id"))))
 
-    @gen_test
+    @asyncio_test
     async def test_delete_one(self):
         # Remove a document twice, check that we get a success responses
         # and n = 0 for the second time.
         await self.collection.insert_one({"_id": 1})
         result = await self.collection.delete_one({"_id": 1})
 
         # First time we remove, n = 1
@@ -131,73 +139,70 @@
         result = await self.collection.delete_one({"_id": 1})
 
         # Second time, document is already gone, n = 0
         self.assertEqual(0, result.raw_result["n"])
         self.assertEqual(1, result.raw_result["ok"])
         self.assertEqual(None, result.raw_result.get("err"))
 
-    @gen_test
+    @ignore_deprecations
+    @asyncio_test
     async def test_unacknowledged_insert(self):
-        # Test that unacknowledged inserts complete eventually.
-
         coll = self.db.test_unacknowledged_insert
         await coll.with_options(write_concern=WriteConcern(0)).insert_one({"_id": 1})
 
         # The insert is eventually executed.
         while not (await coll.count_documents({})):
-            await gen.sleep(0.1)
+            await asyncio.sleep(0.1)
 
-    @gen_test
+    @ignore_deprecations
+    @asyncio_test
     async def test_unacknowledged_update(self):
-        # Test that unacknowledged updates complete eventually.
         coll = self.collection
 
         await coll.insert_one({"_id": 1})
         await coll.with_options(write_concern=WriteConcern(0)).update_one(
             {"_id": 1}, {"$set": {"a": 1}}
         )
 
         while not (await coll.find_one({"a": 1})):
-            await gen.sleep(0.1)
+            await asyncio.sleep(0.1)
 
     @ignore_deprecations
-    @gen_test
+    @asyncio_test
     async def test_indexes(self):
         test_collection = self.collection
 
         # Create an index
         idx_name = await test_collection.create_index([("foo", 1)])
         index_info = await test_collection.index_information()
         self.assertEqual([("foo", 1)], index_info[idx_name]["key"])
 
         # Don't test drop_index or drop_indexes -- Synchro tests them
 
     async def _make_test_data(self, n):
         await self.db.drop_collection("test")
         await self.db.test.insert_many([{"_id": i} for i in range(n)])
-        return sum(range(n))
+        expected_sum = sum(range(n))
+        return expected_sum
 
     pipeline = [{"$project": {"_id": "$_id"}}]
 
-    def assertAllDocs(self, expected_sum, docs):
-        self.assertEqual(expected_sum, sum(doc["_id"] for doc in docs))
-
-    @gen_test(timeout=30)
+    @asyncio_test(timeout=30)
     async def test_aggregation_cursor(self):
         db = self.db
 
         # A small collection which returns only an initial batch,
         # and a larger one that requires a getMore.
         for collection_size in (10, 1000):
             expected_sum = await self._make_test_data(collection_size)
             cursor = db.test.aggregate(self.pipeline)
             docs = await cursor.to_list(collection_size)
-            self.assertAllDocs(expected_sum, docs)
+            self.assertEqual(expected_sum, sum(doc["_id"] for doc in docs))
 
-    @gen_test
+    @asyncio_test
     async def test_aggregation_cursor_exc_info(self):
         await self._make_test_data(200)
         cursor = self.db.test.aggregate(self.pipeline)
         await cursor.to_list(length=10)
         await self.db.test.drop()
         try:
             await cursor.to_list(length=None)
@@ -206,30 +211,30 @@
 
             # The call tree should include PyMongo code we ran on a thread.
             formatted = "\n".join(traceback.format_tb(tb))
             self.assertTrue(
                 "_unpack_response" in formatted or "_check_command_response" in formatted
             )
 
-    @gen_test
+    @asyncio_test
     async def test_aggregate_cursor_del(self):
         cursor = self.db.test.aggregate(self.pipeline)
         del cursor
         cursor = self.db.test.aggregate(self.pipeline)
         await cursor.close()
         del cursor
 
     def test_with_options(self):
         coll = self.db.test
         codec_options = CodecOptions(tz_aware=True, uuid_representation=JAVA_LEGACY)
 
         write_concern = WriteConcern(w=2, j=True)
         coll2 = coll.with_options(codec_options, ReadPreference.SECONDARY, write_concern)
 
-        self.assertTrue(isinstance(coll2, motor.MotorCollection))
+        self.assertTrue(isinstance(coll2, AsyncIOMotorCollection))
         self.assertEqual(codec_options, coll2.codec_options)
         self.assertEqual(Secondary(), coll2.read_preference)
         self.assertEqual(write_concern, coll2.write_concern)
 
         pref = Secondary([{"dc": "sf"}])
         coll2 = coll.with_options(read_preference=pref)
         self.assertEqual(pref, coll2.read_preference)
@@ -257,10 +262,84 @@
 
         for c in [coll1, coll2, coll3]:
             self.assertEqual(write_concern, c.write_concern)
             self.assertEqual(read_concern, c.read_concern)
             self.assertEqual(read_preference, c.read_preference)
             self.assertEqual(codec_options, c.codec_options)
 
+    @env.require_version_min(7, 0, -1, -1)
+    @env.require_no_standalone
+    @asyncio_test
+    async def test_async_create_encrypted_collection(self):
+        if pymongo.version_tuple < (4, 4, 0):
+            raise unittest.SkipTest("Requires PyMongo 4.4+")
+        c = self.collection
+        KMS_PROVIDERS = {"local": {"key": b"\x00" * 96}}
+        self.cx.drop_database("db")
+        async with AsyncIOMotorClientEncryption(
+            KMS_PROVIDERS, "keyvault.datakeys", c, CodecOptions()
+        ) as client_encryption:
+            coll, ef = await client_encryption.create_encrypted_collection(
+                database=self.db,
+                name="testing1",
+                encrypted_fields={"fields": [{"path": "ssn", "bsonType": "string", "keyId": None}]},
+                kms_provider="local",
+            )
+            with self.assertRaises(pymongo.errors.WriteError) as exc:
+                await coll.insert_one({"ssn": "123-45-6789"})
+            self.assertEqual(exc.exception.code, 121)
+            await self.db.drop_collection("testing1", encrypted_fields=ef)
+
+    @asyncio_test
+    async def test_async_encrypt_expression(self):
+        if pymongo.version_tuple < (4, 4, 0):
+            raise unittest.SkipTest("Requires PyMongo 4.4+")
+        c = self.collection
+        KMS_PROVIDERS = {"local": {"key": b"\x00" * 96}}
+        self.cx.drop_database("db")
+        async with AsyncIOMotorClientEncryption(
+            KMS_PROVIDERS, "keyvault.datakeys", c, CodecOptions()
+        ) as client_encryption:
+            data_key = await client_encryption.create_data_key(
+                "local", key_alt_names=["pymongo_encryption_example_1"]
+            )
+            name = "DoubleNoPrecision"
+            range_opts = RangeOpts(sparsity=1)
+            for i in [6.0, 30.0, 200.0]:
+                insert_payload = await client_encryption.encrypt(
+                    float(i),
+                    key_id=data_key,
+                    algorithm=Algorithm.RANGEPREVIEW,
+                    contention_factor=0,
+                    range_opts=range_opts,
+                )
+                self.collection.insert_one(
+                    {
+                        f"encrypted{name}": insert_payload,
+                    }
+                )
+                self.assertEqual(await client_encryption.decrypt(insert_payload), i)
+
+            find_payload = await client_encryption.encrypt_expression(
+                expression={
+                    "$and": [
+                        {f"encrypted{name}": {"$gte": 6.0}},
+                        {f"encrypted{name}": {"$lte": 200.0}},
+                    ]
+                },
+                key_id=data_key,
+                algorithm=Algorithm.RANGEPREVIEW,
+                query_type=QueryType.RANGEPREVIEW,
+                contention_factor=0,
+                range_opts=range_opts,
+            )
+
+            sorted_find = sorted(
+                await self.collection.explicit_encryption.find(find_payload).to_list(3),
+                key=lambda x: x["_id"],
+            )
+            for elem, expected in zip(sorted_find, [6.0, 30.0, 200.0]):
+                self.assertEqual(elem[f"encrypted{name}"], expected)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_core.py` & `motor-3.2.0/test/tornado_tests/test_motor_core.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_cursor.py` & `motor-3.2.0/test/tornado_tests/test_motor_cursor.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_database.py` & `motor-3.2.0/test/tornado_tests/test_motor_database.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_grid_file.py` & `motor-3.2.0/test/tornado_tests/test_motor_grid_file.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_gridfsbucket.py` & `motor-3.2.0/test/tornado_tests/test_motor_gridfsbucket.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_ipv6.py` & `motor-3.2.0/test/tornado_tests/test_motor_ipv6.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_replica_set.py` & `motor-3.2.0/test/tornado_tests/test_motor_replica_set.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_session.py` & `motor-3.2.0/test/tornado_tests/test_motor_session.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_ssl.py` & `motor-3.2.0/test/tornado_tests/test_motor_ssl.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_transaction.py` & `motor-3.2.0/test/tornado_tests/test_motor_transaction.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/tornado_tests/test_motor_web.py` & `motor-3.2.0/test/tornado_tests/test_motor_web.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/utils.py` & `motor-3.2.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/test/version.py` & `motor-3.2.0/test/version.py`

 * *Files identical despite different names*

### Comparing `motor-3.1.2/tox.ini` & `motor-3.2.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # Tornado 5 supports Python 3.4+.
     tornado5-{py37},
 
     # Tornado 6 supports Python 3.5+.
     tornado6-{pypy37,py37,py38,py39,py310,py311},
 
     # Test Tornado's dev version in a few configurations.
-    tornado_git-{py37,py38},
+    tornado_git-{py38},
 
     # Ensure the sphinx build has no errors or warnings.
     py3-sphinx-docs,
 
     # Run the doctests, include examples and tutorial, via Sphinx.
     py3-sphinx-doctest,
 
@@ -49,21 +49,23 @@
     FLE_AZURE_TENANTID
     FLE_AZURE_CLIENTSECRET
     FLE_GCP_EMAIL
     FLE_GCP_PRIVATEKEY
 
 
 basepython =
-    py37,synchro37: {env:PYTHON_BINARY:python3.7}
+    py37: {env:PYTHON_BINARY:python3.7}
     py38: {env:PYTHON_BINARY:python3.8}
     py39: {env:PYTHON_BINARY:python3.9}
     py310: {env:PYTHON_BINARY:python3.10}
     py311: {env:PYTHON_BINARY:python3.11}
     pypy37: {env:PYTHON_BINARY:pypy3}
 
+    synchro37: {env:PYTHON_BINARY:python3.7}
+
     # Default Python 3 when we don't care about minor version.
     py3,lint,manifest: {env:PYTHON_BINARY:python3}
 
 deps =
     tornado5: tornado>=5,<6
     tornado6: tornado>=6,<7
     tornado_git: git+https://github.com/tornadoweb/tornado.git
@@ -75,14 +77,16 @@
     sphinx: tornado
 
     py3-pymongo-latest: tornado>=5,<6
 
     synchro37: tornado>=6,<7
     synchro37: nose
 
+    pypy37: cryptography<3
+
 setenv =
     PYTHONWARNINGS="error,ignore:The distutils package is deprecated:DeprecationWarning"
 commands =
     python --version
     python setup.py test --xunit-output=xunit-results {posargs}
 
 extras =
@@ -104,15 +108,16 @@
 setenv = PYTHONHASHSEED=0
 changedir = doc
 commands =
     sphinx-build -q -E -b linkcheck . {envtmpdir}/linkcheck {posargs}
 
 [testenv:py3-pymongo-latest]
 commands =
-    pip install git+https://github.com/mongodb/mongo-python-driver.git@master#egg=pymongo[encryption]
+    pip install git+https://github.com/mongodb/mongo-python-driver.git@master
+    pip install --pre pymongocrypt
     python --version
     python -c "import pymongo; print('PyMongo %s' % (pymongo.version,))"
     python setup.py test --xunit-output=xunit-results {posargs}
 
 [testenv:synchro37]
 allowlist_externals =
     git
```

