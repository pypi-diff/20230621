# Comparing `tmp/pymodbus-3.3.1.tar.gz` & `tmp/pymodbus-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.3.1.tar", last modified: Mon Jun  5 18:50:48 2023, max compression
+gzip compressed data, was "pymodbus-3.3.2.tar", last modified: Wed Jun 21 15:05:43 2023, max compression
```

## Comparing `pymodbus-3.3.1.tar` & `pymodbus-3.3.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.994661 pymodbus-3.3.1/
--rw-r--r--   0 jan        (501) staff       (20)    26536 2023-06-05 18:50:02.000000 pymodbus-3.3.1/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-04 13:17:31.000000 pymodbus-3.3.1/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-04 13:17:31.000000 pymodbus-3.3.1/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-05 18:50:48.994750 pymodbus-3.3.1/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    16791 2023-06-05 18:50:02.000000 pymodbus-3.3.1/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.980409 pymodbus-3.3.1/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-05 18:50:02.000000 pymodbus-3.3.1/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9369 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9267 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.982099 pymodbus-3.3.1/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    11845 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/serial.py
--rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.982755 pymodbus-3.3.1/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4851 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/remote.py
--rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.983717 pymodbus-3.3.1/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/base.py
--rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/mei_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14021 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12160 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.983852 pymodbus-3.3.1/pymodbus/repl/
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.984692 pymodbus-3.3.1/pymodbus/repl/client/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/completer.py
--rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/helper.py
--rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/main.py
--rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/mclient.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.985113 pymodbus-3.3.1/pymodbus/repl/server/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/server/cli.py
--rw-r--r--   0 jan        (501) staff       (20)     6421 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/server/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.985391 pymodbus-3.3.1/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    47906 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.986152 pymodbus-3.3.1/pymodbus/server/reactive/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/server/reactive/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/reactive/default_config.py
--rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/reactive/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.987063 pymodbus-3.3.1/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/setup.json
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.988409 pymodbus-3.3.1/pymodbus/server/simulator/web/
--rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple120.png
--rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple152.png
--rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple60.png
--rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple76.png
--rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/favicon.ico
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989202 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/
--rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/calls
--rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/log
--rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
--rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/registers
--rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/server
--rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/index.html
--rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/pymodbus.css
--rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/welcome.html
--rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/transaction.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989458 pymodbus-3.3.1/pymodbus/transport/
--rw-r--r--   0 jan        (501) staff       (20)       17 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/transport/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989576 pymodbus-3.3.1/pymodbus/transport/serial_asyncio/
--rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/transport/serial_asyncio/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    14940 2023-06-05 18:50:02.000000 pymodbus-3.3.1/pymodbus/transport/transport.py
--rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/utilities.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.981166 pymodbus-3.3.1/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.1/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-04 13:17:31.000000 pymodbus-3.3.1/requirements.txt
--rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-05 18:50:48.995351 pymodbus-3.3.1/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-04 13:17:31.000000 pymodbus-3.3.1/setup.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.994544 pymodbus-3.3.1/test/
--rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_all_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_bit_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_bit_write_messages.py
--rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client.py
--rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client_faulty_response.py
--rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client_sync.py
--rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_diag_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_events.py
--rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_example_client_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     7225 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_examples.py
--rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_mei_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_other_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_register_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_register_write_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2448 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_remote_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_repl_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_asyncio.py
--rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_context.py
--rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_multidrop.py
--rwxr-xr-x   0 jan        (501) staff       (20)    10930 2023-06-05 18:30:16.000000 pymodbus-3.3.1/test/test_server_task.py
--rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_simulator.py
--rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_sparse_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_transaction.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_unix_socket.py
--rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.915977 pymodbus-3.3.2/
+-rw-r--r--   0 jan        (501) staff       (20)    26849 2023-06-21 13:55:50.000000 pymodbus-3.3.2/CHANGELOG.rst
+-rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-09 17:19:30.000000 pymodbus-3.3.2/LICENSE
+-rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-09 17:19:30.000000 pymodbus-3.3.2/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)    18292 2023-06-21 15:05:43.916066 pymodbus-3.3.2/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    16798 2023-06-21 15:05:31.000000 pymodbus-3.3.2/README.rst
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.904849 pymodbus-3.3.2/pymodbus/
+-rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     9540 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/bit_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     9532 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/bit_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.906506 pymodbus-3.3.2/pymodbus/client/
+-rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    11845 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/base.py
+-rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/client/mixin.py
+-rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/tcp.py
+-rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/tls.py
+-rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/udp.py
+-rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/constants.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907039 pymodbus-3.3.2/pymodbus/datastore/
+-rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/datastore/context.py
+-rw-r--r--   0 jan        (501) staff       (20)     4796 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/datastore/remote.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/store.py
+-rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/device.py
+-rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/diag_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/events.py
+-rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/file_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907738 pymodbus-3.3.2/pymodbus/framer/
+-rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/base.py
+-rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/mei_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/other_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/py.typed
+-rw-r--r--   0 jan        (501) staff       (20)    14300 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/register_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    12510 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/register_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907845 pymodbus-3.3.2/pymodbus/repl/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908309 pymodbus-3.3.2/pymodbus/repl/client/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/client/completer.py
+-rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/client/helper.py
+-rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/repl/client/main.py
+-rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/repl/client/mclient.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908645 pymodbus-3.3.2/pymodbus/repl/server/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/server/cli.py
+-rw-r--r--   0 jan        (501) staff       (20)     6417 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/repl/server/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908888 pymodbus-3.3.2/pymodbus/server/
+-rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    47906 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/server/async_io.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.909250 pymodbus-3.3.2/pymodbus/server/reactive/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/server/reactive/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/reactive/default_config.py
+-rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/server/reactive/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.909843 pymodbus-3.3.2/pymodbus/server/simulator/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/main.py
+-rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.911462 pymodbus-3.3.2/pymodbus/server/simulator/web/
+-rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912192 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/transaction.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912420 pymodbus-3.3.2/pymodbus/transport/
+-rw-r--r--   0 jan        (501) staff       (20)       17 2023-06-14 11:10:10.000000 pymodbus-3.3.2/pymodbus/transport/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912529 pymodbus-3.3.2/pymodbus/transport/serial_asyncio/
+-rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/transport/serial_asyncio/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    14940 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/transport/transport.py
+-rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.905601 pymodbus-3.3.2/pymodbus.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    18292 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.2/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-21 15:05:31.000000 pymodbus-3.3.2/requirements.txt
+-rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-21 15:05:43.916674 pymodbus-3.3.2/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-09 17:19:30.000000 pymodbus-3.3.2/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.915874 pymodbus-3.3.2/test/
+-rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_all_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_bit_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_bit_write_messages.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_client.py
+-rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_client_faulty_response.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_client_sync.py
+-rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_device.py
+-rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_diag_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_events.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_example_client_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     7228 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_examples.py
+-rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_file_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_framers.py
+-rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_mei_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_other_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_register_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_register_write_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2661 2023-06-21 13:55:50.000000 pymodbus-3.3.2/test/test_remote_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_repl_client.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_server_asyncio.py
+-rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_server_context.py
+-rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_server_multidrop.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    10930 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_server_task.py
+-rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_sparse_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_transaction.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_unix_socket.py
+-rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_utilities.py
```

### Comparing `pymodbus-3.3.1/CHANGELOG.rst` & `pymodbus-3.3.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+version 3.3.2
+----------------------------------------------------------
+* Fix RemoteSlaveContext (#1599)
+* Change version follow PEP 440. (#1609)
+* Fix regression with REPL server not listening (#1604)
+* Fix write function codes (#1598)
+* Release corrections. (#1586)
+
+Thanks to:
+  Alex
+  Fredo70
+  jan iversen
+
 version 3.3.1
 ----------------------------------------------------------
 * transport fixes and 100% test coverage. (#1580)
 * Delay self.loop until connect(). (#1579)
 * Added mechanism to determine if server did not start cleanly (#1539)
 * Proof transport reconnect works. (#1577)
 * Fix non-shared block doc in config.rst. (#1573)
```

### Comparing `pymodbus-3.3.1/LICENSE` & `pymodbus-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/PKG-INFO` & `pymodbus-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.3.1
+Version: 3.3.2
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -36,16 +36,16 @@
 Provides-Extra: documentation
 Provides-Extra: development
 License-File: LICENSE
 
 ================================
 PyModbus - A Python Modbus Stack
 ================================
-We are happy to announce that we have a new home: pymodbus-dev, which is pure 100% FOSS.
-The move from a company organization to pymodbus-dev was done to allow a 100% openness in the spirit of FOSS.
+We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
+There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
  .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
@@ -55,17 +55,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.2>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.1/README.rst` & `pymodbus-3.3.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ================================
 PyModbus - A Python Modbus Stack
 ================================
-We are happy to announce that we have a new home: pymodbus-dev, which is pure 100% FOSS.
-The move from a company organization to pymodbus-dev was done to allow a 100% openness in the spirit of FOSS.
+We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
+There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
  .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
@@ -16,17 +16,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.2>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.1/pymodbus/bit_read_message.py` & `pymodbus-3.3.2/pymodbus/bit_read_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "ReadDiscreteInputsResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.constants import Defaults
+from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
-from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.utilities import pack_bitstring, unpack_bitstring
 
 
 class ReadBitsRequestBase(ModbusRequest):
     """Base class for Messages Requesting bit values."""
 
     _rtu_frame_size = 8
@@ -167,14 +167,16 @@
         :returns: An initialized :py:class:`~pymodbus.register_read_message.ReadCoilsResponse`, or an :py:class:`~pymodbus.pdu.ExceptionResponse` if an error occurred
         """
         if not (1 <= self.count <= 0x7D0):
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, self.count):
             return self.doException(merror.IllegalAddress)
         values = context.getValues(self.function_code, self.address, self.count)
+        if isinstance(values, ExceptionResponse):
+            return values
         return ReadCoilsResponse(values)
 
 
 class ReadCoilsResponse(ReadBitsResponseBase):
     """The coils in the response message are packed as one coil per bit of the data field.
 
     Status is indicated as 1= ON and 0= OFF. The LSB of the
@@ -233,14 +235,16 @@
         :returns: An initialized :py:class:`~pymodbus.register_read_message.ReadDiscreteInputsResponse`, or an :py:class:`~pymodbus.pdu.ExceptionResponse` if an error occurred
         """
         if not (1 <= self.count <= 0x7D0):
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, self.count):
             return self.doException(merror.IllegalAddress)
         values = context.getValues(self.function_code, self.address, self.count)
+        if isinstance(values, ExceptionResponse):
+            return values
         return ReadDiscreteInputsResponse(values)
 
 
 class ReadDiscreteInputsResponse(ReadBitsResponseBase):
     """The discrete inputs in the response message are packed as one input per bit of the data field.
 
     Status is indicated as 1= ON; 0= OFF. The LSB of
```

### Comparing `pymodbus-3.3.1/pymodbus/bit_write_message.py` & `pymodbus-3.3.2/pymodbus/bit_write_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     "WriteMultipleCoilsResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.constants import ModbusStatus
+from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
-from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.utilities import pack_bitstring, unpack_bitstring
 
 
 # ---------------------------------------------------------------------------#
 #  Local Constants
 # ---------------------------------------------------------------------------#
 #  These are defined in the spec to turn a coil on/off
@@ -86,16 +86,20 @@
         :returns: The populated response or exception message
         """
         # if self.value not in [ModbusStatus.Off, ModbusStatus.On]:
         #    return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, 1):
             return self.doException(merror.IllegalAddress)
 
-        context.setValues(self.function_code, self.address, [self.value])
+        result = context.setValues(self.function_code, self.address, [self.value])
+        if isinstance(result, ExceptionResponse):
+            return result
         values = context.getValues(self.function_code, self.address, 1)
+        if isinstance(values, ExceptionResponse):
+            return values
         return WriteSingleCoilResponse(self.address, values[0])
 
     def get_response_pdu_size(self):
         """Get response pdu size.
 
         Func_code (1 byte) + Output Address (2 byte) + Output Value  (2 Bytes)
         :return:
@@ -218,15 +222,17 @@
         if not 1 <= count <= 0x07B0:
             return self.doException(merror.IllegalValue)
         if self.byte_count != (count + 7) // 8:
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, count):
             return self.doException(merror.IllegalAddress)
 
-        context.setValues(self.function_code, self.address, self.values)
+        result = context.setValues(self.function_code, self.address, self.values)
+        if isinstance(result, ExceptionResponse):
+            return result
         return WriteMultipleCoilsResponse(self.address, count)
 
     def __str__(self):
         """Return a string representation of the instance.
 
         :returns: A string representation of the instance
         """
```

### Comparing `pymodbus-3.3.1/pymodbus/client/__init__.py` & `pymodbus-3.3.2/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/base.py` & `pymodbus-3.3.2/pymodbus/client/base.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/mixin.py` & `pymodbus-3.3.2/pymodbus/client/mixin.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/serial.py` & `pymodbus-3.3.2/pymodbus/client/serial.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/tcp.py` & `pymodbus-3.3.2/pymodbus/client/tcp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/tls.py` & `pymodbus-3.3.2/pymodbus/client/tls.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/client/udp.py` & `pymodbus-3.3.2/pymodbus/client/udp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/constants.py` & `pymodbus-3.3.2/pymodbus/constants.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/datastore/context.py` & `pymodbus-3.3.2/pymodbus/datastore/context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/datastore/remote.py` & `pymodbus-3.3.2/pymodbus/datastore/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,42 +28,42 @@
         if not self.__set_callbacks:
             Log.error("Init went wrong.")
 
     def reset(self):
         """Reset all the datastores to their default values."""
         raise NotImplementedException()
 
-    def validate(self, fc_as_hex, address, count=1):
+    def validate(self, _fc_as_hex, _address, _count):
         """Validate the request to make sure it is in range.
 
-        :param fc_as_hex: The function we are working with
-        :param address: The starting address
-        :param count: The number of values to test
-        :returns: True if the request in within range, False otherwise
+        :returns: True
         """
-        Log.debug("validate[{}] {}:{}", fc_as_hex, address, count)
-        group_fx = self.decode(fc_as_hex)
-        if fc_as_hex in self._write_fc:
-            func_fc = self.__set_callbacks[f"{group_fx}{fc_as_hex}"]
-        else:
-            func_fc = self.__get_callbacks[group_fx]
-        self.result = func_fc(address, count)
-        return not self.result.isError()
+        return True
 
     def getValues(self, fc_as_hex, _address, _count=1):
         """Get values from real call in validate"""
         if fc_as_hex in self._write_fc:
             return [0]
+        group_fx = self.decode(fc_as_hex)
+        func_fc = self.__get_callbacks[group_fx]
+        self.result = func_fc(_address, _count)
         return self.__extract_result(self.decode(fc_as_hex), self.result)
 
     def setValues(self, fc_as_hex, address, values):
-        """Set the datastore with the supplied values.
-
-        Already done in validate
-        """
+        """Set the datastore with the supplied values."""
+        group_fx = self.decode(fc_as_hex)
+        if fc_as_hex in self._write_fc:
+            func_fc = self.__set_callbacks[f"{group_fx}{fc_as_hex}"]
+            if fc_as_hex in {0x0F, 0x10}:
+                self.result = func_fc(address, values)
+            else:
+                self.result = func_fc(address, values[0])
+        if self.result.isError():
+            return self.result
+        return None
 
     def __str__(self):
         """Return a string representation of the context.
 
         :returns: A string representation of the context
         """
         return f"Remote Slave Context({self._client})"
@@ -109,15 +109,15 @@
             "i6": lambda a, v: self._client.write_register(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
             "i16": lambda a, v: self._client.write_registers(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
         }
-        self._write_fc = (0x05, 0x06, 0x15, 0x16, 0x17)
+        self._write_fc = (0x05, 0x06, 0x0F, 0x10)
 
     def __extract_result(self, fc_as_hex, result):
         """Extract the values out of a response.
 
         TODO make this consistent (values?)
         """
         if not result.isError():
```

### Comparing `pymodbus-3.3.1/pymodbus/datastore/simulator.py` & `pymodbus-3.3.2/pymodbus/datastore/simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/datastore/store.py` & `pymodbus-3.3.2/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/device.py` & `pymodbus-3.3.2/pymodbus/device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/diag_message.py` & `pymodbus-3.3.2/pymodbus/diag_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/events.py` & `pymodbus-3.3.2/pymodbus/events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/exceptions.py` & `pymodbus-3.3.2/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/factory.py` & `pymodbus-3.3.2/pymodbus/factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/file_message.py` & `pymodbus-3.3.2/pymodbus/file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/ascii_framer.py` & `pymodbus-3.3.2/pymodbus/framer/ascii_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/base.py` & `pymodbus-3.3.2/pymodbus/framer/base.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/binary_framer.py` & `pymodbus-3.3.2/pymodbus/framer/binary_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/rtu_framer.py` & `pymodbus-3.3.2/pymodbus/framer/rtu_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/socket_framer.py` & `pymodbus-3.3.2/pymodbus/framer/socket_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/framer/tls_framer.py` & `pymodbus-3.3.2/pymodbus/framer/tls_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/logging.py` & `pymodbus-3.3.2/pymodbus/logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/mei_message.py` & `pymodbus-3.3.2/pymodbus/mei_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/other_message.py` & `pymodbus-3.3.2/pymodbus/other_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/payload.py` & `pymodbus-3.3.2/pymodbus/payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/pdu.py` & `pymodbus-3.3.2/pymodbus/pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/register_read_message.py` & `pymodbus-3.3.2/pymodbus/register_read_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     "ReadWriteMultipleRegistersResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.constants import Defaults
+from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
-from pymodbus.pdu import ModbusRequest, ModbusResponse
 
 
 class ReadRegistersRequestBase(ModbusRequest):
     """Base class for reading a modbus register."""
 
     _rtu_frame_size = 8
 
@@ -147,14 +147,17 @@
         :returns: An initialized :py:class:`~pymodbus.register_read_message.ReadHoldingRegistersResponse`, or an :py:class:`~pymodbus.pdu.ExceptionResponse` if an error occurred
         """
         if not (1 <= self.count <= 0x7D):
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, self.count):
             return self.doException(merror.IllegalAddress)
         values = context.getValues(self.function_code, self.address, self.count)
+        if isinstance(values, ExceptionResponse):
+            return values
+
         return ReadHoldingRegistersResponse(values)
 
 
 class ReadHoldingRegistersResponse(ReadRegistersResponseBase):
     """Read holding registers.
 
     This function code is used to read the contents of a contiguous block
@@ -205,14 +208,16 @@
         :returns: An initialized :py:class:`~pymodbus.register_read_message.ReadInputRegistersResponse`, or an :py:class:`~pymodbus.pdu.ExceptionResponse` if an error occurred
         """
         if not (1 <= self.count <= 0x7D):
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, self.count):
             return self.doException(merror.IllegalAddress)
         values = context.getValues(self.function_code, self.address, self.count)
+        if isinstance(values, ExceptionResponse):
+            return values
         return ReadInputRegistersResponse(values)
 
 
 class ReadInputRegistersResponse(ReadRegistersResponseBase):
     """Read/write input registers.
 
     This function code is used to read from 1 to approx. 125 contiguous
@@ -320,15 +325,19 @@
             return self.doException(merror.IllegalValue)
         if not context.validate(
             self.function_code, self.write_address, self.write_count
         ):
             return self.doException(merror.IllegalAddress)
         if not context.validate(self.function_code, self.read_address, self.read_count):
             return self.doException(merror.IllegalAddress)
-        context.setValues(self.function_code, self.write_address, self.write_registers)
+        result = context.setValues(
+            self.function_code, self.write_address, self.write_registers
+        )
+        if isinstance(result, ExceptionResponse):
+            return result
         registers = context.getValues(
             self.function_code, self.read_address, self.read_count
         )
         return ReadWriteMultipleRegistersResponse(registers)
 
     def get_response_pdu_size(self):
         """Get response pdu size.
```

### Comparing `pymodbus-3.3.1/pymodbus/register_write_message.py` & `pymodbus-3.3.2/pymodbus/register_write_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     "MaskWriteRegisterRequest",
     "MaskWriteRegisterResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
+from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
-from pymodbus.pdu import ModbusRequest, ModbusResponse
 
 
 class WriteSingleRegisterRequest(ModbusRequest):
     """This function code is used to write a single holding register in a remote device.
 
     The Request PDU specifies the address of the register to
     be written. Registers are addressed starting at zero. Therefore register
@@ -64,15 +64,17 @@
         :returns: An initialized response, exception message otherwise
         """
         if not 0 <= self.value <= 0xFFFF:
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, 1):
             return self.doException(merror.IllegalAddress)
 
-        context.setValues(self.function_code, self.address, [self.value])
+        result = context.setValues(self.function_code, self.address, [self.value])
+        if isinstance(result, ExceptionResponse):
+            return result
         values = context.getValues(self.function_code, self.address, 1)
         return WriteSingleRegisterResponse(self.address, values[0])
 
     def get_response_pdu_size(self):
         """Get response pdu size.
 
         Func_code (1 byte) + Register Address(2 byte) + Register Value (2 bytes)
@@ -207,15 +209,17 @@
         if not 1 <= self.count <= 0x07B:
             return self.doException(merror.IllegalValue)
         if self.byte_count != self.count * 2:
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, self.count):
             return self.doException(merror.IllegalAddress)
 
-        context.setValues(self.function_code, self.address, self.values)
+        result = context.setValues(self.function_code, self.address, self.values)
+        if isinstance(result, ExceptionResponse):
+            return result
         return WriteMultipleRegistersResponse(self.address, self.count)
 
     def get_response_pdu_size(self):
         """Get response pdu size.
 
         Func_code (1 byte) + Starting Address (2 byte) + Quantity of Registers  (2 Bytes)
         :return:
@@ -326,16 +330,20 @@
         if not 0x0000 <= self.and_mask <= 0xFFFF:
             return self.doException(merror.IllegalValue)
         if not 0x0000 <= self.or_mask <= 0xFFFF:
             return self.doException(merror.IllegalValue)
         if not context.validate(self.function_code, self.address, 1):
             return self.doException(merror.IllegalAddress)
         values = context.getValues(self.function_code, self.address, 1)[0]
+        if isinstance(values, ExceptionResponse):
+            return values
         values = (values & self.and_mask) | (self.or_mask & ~self.and_mask)
-        context.setValues(self.function_code, self.address, [values])
+        result = context.setValues(self.function_code, self.address, [values])
+        if isinstance(result, ExceptionResponse):
+            return result
         return MaskWriteRegisterResponse(self.address, self.and_mask, self.or_mask)
 
 
 class MaskWriteRegisterResponse(ModbusResponse):
     """The normal response is an echo of the request.
 
     The response is returned after the register has been written.
```

### Comparing `pymodbus-3.3.1/pymodbus/repl/client/completer.py` & `pymodbus-3.3.2/pymodbus/repl/client/completer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/repl/client/helper.py` & `pymodbus-3.3.2/pymodbus/repl/client/helper.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/repl/client/main.py` & `pymodbus-3.3.2/pymodbus/repl/client/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/repl/client/mclient.py` & `pymodbus-3.3.2/pymodbus/repl/client/mclient.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/repl/server/cli.py` & `pymodbus-3.3.2/pymodbus/repl/server/cli.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/repl/server/main.py` & `pymodbus-3.3.2/pymodbus/repl/server/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,16 +194,16 @@
         slave=modbus_slave_id,
         loop=loop,
         single=False,
         data_block_settings=data_block_settings,
         **web_app_config,
         **modbus_config,
     )
+    loop.run_until_complete(app.run_async(repl))
     if repl:
         loop.run_until_complete(run_repl(app))
     else:
-        loop.run_until_complete(app.run_async(repl))
         loop.run_forever()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pymodbus-3.3.1/pymodbus/server/__init__.py` & `pymodbus-3.3.2/pymodbus/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/async_io.py` & `pymodbus-3.3.2/pymodbus/server/async_io.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/reactive/default_config.py` & `pymodbus-3.3.2/pymodbus/server/reactive/default_config.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/reactive/main.py` & `pymodbus-3.3.2/pymodbus/server/reactive/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/http_server.py` & `pymodbus-3.3.2/pymodbus/server/simulator/http_server.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/main.py` & `pymodbus-3.3.2/pymodbus/server/simulator/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/setup.json` & `pymodbus-3.3.2/pymodbus/server/simulator/setup.json`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/apple120.png` & `pymodbus-3.3.2/pymodbus/server/simulator/web/apple120.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/apple152.png` & `pymodbus-3.3.2/pymodbus/server/simulator/web/apple152.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/apple60.png` & `pymodbus-3.3.2/pymodbus/server/simulator/web/apple60.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/apple76.png` & `pymodbus-3.3.2/pymodbus/server/simulator/web/apple76.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/favicon.ico` & `pymodbus-3.3.2/pymodbus/server/simulator/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/calls` & `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/calls`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/log` & `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/log`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png` & `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/registers` & `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/registers`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/server` & `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/server`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/index.html` & `pymodbus-3.3.2/pymodbus/server/simulator/web/index.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/pymodbus.css` & `pymodbus-3.3.2/pymodbus/server/simulator/web/pymodbus.css`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/server/simulator/web/welcome.html` & `pymodbus-3.3.2/pymodbus/server/simulator/web/welcome.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/transaction.py` & `pymodbus-3.3.2/pymodbus/transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/transport/serial_asyncio/__init__.py` & `pymodbus-3.3.2/pymodbus/transport/serial_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/transport/transport.py` & `pymodbus-3.3.2/pymodbus/transport/transport.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus/utilities.py` & `pymodbus-3.3.2/pymodbus/utilities.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/pymodbus.egg-info/PKG-INFO` & `pymodbus-3.3.2/pymodbus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.3.1
+Version: 3.3.2
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -36,16 +36,16 @@
 Provides-Extra: documentation
 Provides-Extra: development
 License-File: LICENSE
 
 ================================
 PyModbus - A Python Modbus Stack
 ================================
-We are happy to announce that we have a new home: pymodbus-dev, which is pure 100% FOSS.
-The move from a company organization to pymodbus-dev was done to allow a 100% openness in the spirit of FOSS.
+We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
+There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
  .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
@@ -55,17 +55,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.2>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.1/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.3.2/pymodbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/requirements.txt` & `pymodbus-3.3.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/setup.cfg` & `pymodbus-3.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/setup.py` & `pymodbus-3.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_all_messages.py` & `pymodbus-3.3.2/test/test_all_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_bit_read_messages.py` & `pymodbus-3.3.2/test/test_bit_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_bit_write_messages.py` & `pymodbus-3.3.2/test/test_bit_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_client.py` & `pymodbus-3.3.2/test/test_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_client_faulty_response.py` & `pymodbus-3.3.2/test/test_client_faulty_response.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_client_sync.py` & `pymodbus-3.3.2/test/test_client_sync.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_device.py` & `pymodbus-3.3.2/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_diag_messages.py` & `pymodbus-3.3.2/test/test_diag_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_events.py` & `pymodbus-3.3.2/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_example_client_server.py` & `pymodbus-3.3.2/test/test_example_client_server.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_examples.py` & `pymodbus-3.3.2/test/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 import pytest_asyncio
 
 from examples.build_bcd_payload import BcdPayloadBuilder, BcdPayloadDecoder
 from examples.client_async import run_async_client, setup_async_client
 from examples.client_custom_msg import run_custom_client
 from examples.client_payload import run_payload_calls
 from examples.client_test import run_async_calls as run_client_test
+from examples.datastore_simulator import run_server_simulator, setup_simulator
 from examples.message_generator import generate_messages
 from examples.message_parser import parse_messages
 from examples.server_async import run_async_server, setup_server
 from examples.server_callback import run_callback_server
 from examples.server_payload import setup_payload_server
-from examples.server_simulator import run_server_simulator, setup_simulator
 from examples.server_updating import run_updating_server, setup_updating_server
 from pymodbus import pymodbus_apply_logging_config
 from pymodbus.server import ServerAsyncStop
 
 
 # from examples.serial_forwarder import run_forwarder
```

### Comparing `pymodbus-3.3.1/test/test_exceptions.py` & `pymodbus-3.3.2/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_factory.py` & `pymodbus-3.3.2/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_file_message.py` & `pymodbus-3.3.2/test/test_file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_framers.py` & `pymodbus-3.3.2/test/test_framers.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_logging.py` & `pymodbus-3.3.2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_mei_messages.py` & `pymodbus-3.3.2/test/test_mei_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_other_messages.py` & `pymodbus-3.3.2/test/test_other_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_payload.py` & `pymodbus-3.3.2/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_pdu.py` & `pymodbus-3.3.2/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_register_read_messages.py` & `pymodbus-3.3.2/test/test_register_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_register_write_messages.py` & `pymodbus-3.3.2/test/test_register_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_remote_datastore.py` & `pymodbus-3.3.2/test/test_remote_datastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,21 @@
         with pytest.raises(NotImplementedException):
             context.reset()
 
     def test_remote_slave_set_values(self):
         """Test setting values against a remote slave context"""
         client = mock.MagicMock()
         client.write_coils = lambda a, b: WriteMultipleCoilsResponse()
+        client.write_registers = lambda a, b: ExceptionResponse(0x10, 0x02)
 
         context = RemoteSlaveContext(client)
-        context.setValues(1, 0, [1])
+        context.setValues(0x0F, 0, [1])
+        result = context.setValues(0x10, 1, [1])
+        assert result.exception_code == 0x02
+        assert result.function_code == 0x90
 
     def test_remote_slave_get_values(self):
         """Test getting values from a remote slave context"""
         client = mock.MagicMock()
         client.read_coils = lambda a, b: ReadCoilsResponse([1] * 10)
         client.read_input_registers = lambda a, b: ReadInputRegistersResponse([10] * 10)
         client.read_holding_registers = lambda a, b: ExceptionResponse(0x15)
@@ -60,8 +64,8 @@
         result = context.validate(1, 0, 10)
         assert result
 
         result = context.validate(4, 0, 10)
         assert result
 
         result = context.validate(3, 0, 10)
-        assert not result
+        assert result
```

### Comparing `pymodbus-3.3.1/test/test_repl_client.py` & `pymodbus-3.3.2/test/test_repl_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_server_asyncio.py` & `pymodbus-3.3.2/test/test_server_asyncio.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_server_context.py` & `pymodbus-3.3.2/test/test_server_context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_server_multidrop.py` & `pymodbus-3.3.2/test/test_server_multidrop.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_server_task.py` & `pymodbus-3.3.2/test/test_server_task.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_simulator.py` & `pymodbus-3.3.2/test/test_simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_sparse_datastore.py` & `pymodbus-3.3.2/test/test_sparse_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_transaction.py` & `pymodbus-3.3.2/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_unix_socket.py` & `pymodbus-3.3.2/test/test_unix_socket.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.1/test/test_utilities.py` & `pymodbus-3.3.2/test/test_utilities.py`

 * *Files identical despite different names*

