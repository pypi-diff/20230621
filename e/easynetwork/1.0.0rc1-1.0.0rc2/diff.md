# Comparing `tmp/easynetwork-1.0.0rc1.tar.gz` & `tmp/easynetwork-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jun 18 16:42:45 2023, max compression
+gzip compressed data, last modified: Tue Jun 20 22:19:47 2023, max compression
```

## Comparing `easynetwork-1.0.0rc1.tar` & `easynetwork-1.0.0rc2.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0      847 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.flake8
--rw-r--r--   0        0        0     1939 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0   123771 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/pdm.lock
--rw-r--r--   0        0        0     3673 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tox.ini
--rw-r--r--   0        0        0     1260 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.vscode/settings.example.json
--rw-r--r--   0        0        0      637 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/converter.py
--rw-r--r--   0        0        0     2120 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/exceptions.py
--rw-r--r--   0        0        0     5291 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/protocol.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/py.typed
--rw-r--r--   0        0        0      206 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/__init__.py
--rw-r--r--   0        0        0      206 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/__init__.py
--rw-r--r--   0        0        0    11364 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/abc.py
--rw-r--r--   0        0        0     6289 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/factory.py
--rw-r--r--   0        0        0     2002 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/futures.py
--rw-r--r--   0        0        0      708 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/sniffio.py
--rw-r--r--   0        0        0     1918 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/tasks.py
--rw-r--r--   0        0        0      368 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/__init__.py
--rw-r--r--   0        0        0     2407 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/abc.py
--rw-r--r--   0        0        0    13391 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/tcp.py
--rw-r--r--   0        0        0    13060 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/udp.py
--rw-r--r--   0        0        0      585 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/__init__.py
--rw-r--r--   0        0        0     1428 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/abc.py
--rw-r--r--   0        0        0     2798 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/handler.py
--rw-r--r--   0        0        0     8043 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/standalone.py
--rw-r--r--   0        0        0    22757 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/tcp.py
--rw-r--r--   0        0        0    18880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/udp.py
--rw-r--r--   0        0        0      205 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/__init__.py
--rw-r--r--   0        0        0      335 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/__init__.py
--rw-r--r--   0        0        0     2146 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/abc.py
--rw-r--r--   0        0        0    14942 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/tcp.py
--rw-r--r--   0        0        0    12195 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/udp.py
--rw-r--r--   0        0        0     1164 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/__init__.py
--rw-r--r--   0        0        0     2264 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/abc.py
--rw-r--r--   0        0        0     7602 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/base_stream.py
--rw-r--r--   0        0        0     2897 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/cbor.py
--rw-r--r--   0        0        0     8165 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/json.py
--rw-r--r--   0        0        0     2313 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/line.py
--rw-r--r--   0        0        0     3794 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/msgpack.py
--rw-r--r--   0        0        0     3297 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/pickle.py
--rw-r--r--   0        0        0     5084 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/struct.py
--rw-r--r--   0        0        0      422 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/__init__.py
--rw-r--r--   0        0        0     2881 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/base64.py
--rw-r--r--   0        0        0     6344 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/compressor.py
--rw-r--r--   0        0        0     2246 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/encryptor.py
--rw-r--r--   0        0        0      195 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/__init__.py
--rw-r--r--   0        0        0    10880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/_utils.py
--rw-r--r--   0        0        0     1196 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/lock.py
--rw-r--r--   0        0        0     7948 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/socket.py
--rw-r--r--   0        0        0     5533 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/stream.py
--rw-r--r--   0        0        0      288 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/__init__.py
--rw-r--r--   0        0        0     6217 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/_utils.py
--rw-r--r--   0        0        0    17671 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/backend.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/py.typed
--rw-r--r--   0        0        0     5395 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/socket.py
--rw-r--r--   0        0        0     4696 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/tasks.py
--rw-r--r--   0        0        0     4186 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/threads.py
--rw-r--r--   0        0        0      208 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/__init__.py
--rw-r--r--   0        0        0     8604 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/endpoint.py
--rw-r--r--   0        0        0     3694 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/socket.py
--rw-r--r--   0        0        0      208 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/__init__.py
--rw-r--r--   0        0        0     5423 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/listener.py
--rw-r--r--   0        0        0     4113 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/socket.py
--rw-r--r--   0        0        0      131 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      551 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/conftest.py
--rw-r--r--   0        0        0     1113 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/tools.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/__init__.py
--rw-r--r--   0        0        0      355 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/__init__.py
--rw-r--r--   0        0        0    19654 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_asyncio_backend.py
--rw-r--r--   0        0        0     1288 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_backend_factory.py
--rw-r--r--   0        0        0     3201 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_futures.py
--rw-r--r--   0        0        0     2424 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_tasks.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/__init__.py
--rw-r--r--   0        0        0     4173 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/conftest.py
--rw-r--r--   0        0        0     1781 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/serializer.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/__init__.py
--rw-r--r--   0        0        0      289 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/_utils.py
--rw-r--r--   0        0        0      527 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/__init__.py
--rw-r--r--   0        0        0    19354 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_tcp.py
--rw-r--r--   0        0        0    31112 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/base.py
--rw-r--r--   0        0        0     4666 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_standalone.py
--rw-r--r--   0        0        0    31268 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_tcp.py
--rw-r--r--   0        0        0    18286 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/__init__.py
--rw-r--r--   0        0        0     1279 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/__init__.py
--rw-r--r--   0        0        0    12790 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py
--rw-r--r--   0        0        0    16039 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_udp.py
--rw-r--r--   0        0        0      130 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/__init__.py
--rw-r--r--   0        0        0     9118 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/base.py
--rw-r--r--   0        0        0      424 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/conftest.py
--rw-r--r--   0        0        0     6240 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     2233 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0     4069 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_compressors.py
--rw-r--r--   0        0        0     3572 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0     2639 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     3440 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_line.py
--rw-r--r--   0        0        0     1926 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_msgpack.py
--rw-r--r--   0        0        0     2747 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_namedtuple.py
--rw-r--r--   0        0        0     3609 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/__init__.py
--rw-r--r--   0        0        0    10664 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/json.py
--rw-r--r--   0        0        0     2356 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/pickle.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/__init__.py
--rw-r--r--   0        0        0     4925 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/test_import.py
--rw-r--r--   0        0        0      578 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/test_project_metadata.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/__init__.py
--rw-r--r--   0        0        0     3866 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/asyncio_event_loop.py
--rw-r--r--   0        0        0     1792 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/extra_features.py
--rw-r--r--   0        0        0      620 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/session_exit_code.py
--rw-r--r--   0        0        0     2671 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/scripts/async_server_test.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/__init__.py
--rw-r--r--   0        0        0     1795 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/_utils.py
--rw-r--r--   0        0        0     1808 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/base.py
--rw-r--r--   0        0        0     5555 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/conftest.py
--rw-r--r--   0        0        0     5098 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_converter.py
--rw-r--r--   0        0        0    15717 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_protocol.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/__init__.py
--rw-r--r--   0        0        0     1114 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/base.py
--rw-r--r--   0        0        0     2340 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/__init__.py
--rw-r--r--   0        0        0      425 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py
--rw-r--r--   0        0        0    17863 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/test_backend.py
--rw-r--r--   0        0        0     5327 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/test_futures.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/__init__.py
--rw-r--r--   0        0        0      169 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/base.py
--rw-r--r--   0        0        0     2682 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_abc.py
--rw-r--r--   0        0        0    51599 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_tcp.py
--rw-r--r--   0        0        0    41442 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_server/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_server/test_handler.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/__init__.py
--rw-r--r--   0        0        0     1679 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/conftest.py
--rw-r--r--   0        0        0    46304 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_backend.py
--rw-r--r--   0        0        0    32981 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py
--rw-r--r--   0        0        0    14186 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_socket.py
--rw-r--r--   0        0        0    27018 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_stream.py
--rw-r--r--   0        0        0     9534 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py
--rw-r--r--   0        0        0     4898 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_threads.py
--rw-r--r--   0        0        0    30962 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_utils.py
--rw-r--r--   0        0        0      130 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/__init__.py
--rw-r--r--   0        0        0      612 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/base.py
--rw-r--r--   0        0        0      355 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/conftest.py
--rw-r--r--   0        0        0    30904 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_abc.py
--rw-r--r--   0        0        0     3514 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     5880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0    20502 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_compressor.py
--rw-r--r--   0        0        0     4351 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0    15194 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     7216 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_line.py
--rw-r--r--   0        0        0     7146 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_msgpack.py
--rw-r--r--   0        0        0     9953 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0    16647 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_struct.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/__init__.py
--rw-r--r--   0        0        0      456 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/conftest.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/__init__.py
--rw-r--r--   0        0        0      526 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/base.py
--rw-r--r--   0        0        0     1019 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/conftest.py
--rw-r--r--   0        0        0     3294 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_abc.py
--rw-r--r--   0        0        0    67599 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_tcp.py
--rw-r--r--   0        0        0    44378 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/__init__.py
--rw-r--r--   0        0        0     2153 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_lock.py
--rw-r--r--   0        0        0     7763 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_socket.py
--rw-r--r--   0        0        0    14621 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_stream.py
--rw-r--r--   0        0        0    22406 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_utils.py
--rw-r--r--   0        0        0     1915 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1097 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0       55 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/README.md
--rw-r--r--   0        0        0     5202 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1429 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/.flake8
+-rw-r--r--   0        0        0     1939 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   123771 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/pdm.lock
+-rw-r--r--   0        0        0     3673 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tox.ini
+-rw-r--r--   0        0        0     1260 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/.vscode/settings.example.json
+-rw-r--r--   0        0        0      637 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/converter.py
+-rw-r--r--   0        0        0     2120 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/exceptions.py
+-rw-r--r--   0        0        0     5291 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/protocol.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/py.typed
+-rw-r--r--   0        0        0      206 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/__init__.py
+-rw-r--r--   0        0        0    11208 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/abc.py
+-rw-r--r--   0        0        0     6289 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/factory.py
+-rw-r--r--   0        0        0     2808 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/futures.py
+-rw-r--r--   0        0        0      708 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/sniffio.py
+-rw-r--r--   0        0        0     1918 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/tasks.py
+-rw-r--r--   0        0        0      368 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/client/__init__.py
+-rw-r--r--   0        0        0     2407 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/client/abc.py
+-rw-r--r--   0        0        0    13391 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/client/tcp.py
+-rw-r--r--   0        0        0    13060 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/client/udp.py
+-rw-r--r--   0        0        0      585 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/__init__.py
+-rw-r--r--   0        0        0     1428 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/abc.py
+-rw-r--r--   0        0        0     2798 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/handler.py
+-rw-r--r--   0        0        0     8043 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/standalone.py
+-rw-r--r--   0        0        0    22757 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/tcp.py
+-rw-r--r--   0        0        0    18880 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_async/server/udp.py
+-rw-r--r--   0        0        0      205 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_sync/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/__init__.py
+-rw-r--r--   0        0        0     2146 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/abc.py
+-rw-r--r--   0        0        0    14942 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/tcp.py
+-rw-r--r--   0        0        0    12195 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/udp.py
+-rw-r--r--   0        0        0     1164 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/__init__.py
+-rw-r--r--   0        0        0     2264 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/abc.py
+-rw-r--r--   0        0        0     7602 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/base_stream.py
+-rw-r--r--   0        0        0     2897 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/cbor.py
+-rw-r--r--   0        0        0     8165 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/json.py
+-rw-r--r--   0        0        0     2313 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/line.py
+-rw-r--r--   0        0        0     3794 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/msgpack.py
+-rw-r--r--   0        0        0     3297 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/pickle.py
+-rw-r--r--   0        0        0     5084 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/struct.py
+-rw-r--r--   0        0        0      422 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/__init__.py
+-rw-r--r--   0        0        0     2881 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/base64.py
+-rw-r--r--   0        0        0     6344 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/compressor.py
+-rw-r--r--   0        0        0     2246 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/encryptor.py
+-rw-r--r--   0        0        0      195 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/tools/__init__.py
+-rw-r--r--   0        0        0    10880 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/tools/_utils.py
+-rw-r--r--   0        0        0     1196 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/tools/lock.py
+-rw-r--r--   0        0        0     7948 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/tools/socket.py
+-rw-r--r--   0        0        0     5533 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork/tools/stream.py
+-rw-r--r--   0        0        0      288 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/__init__.py
+-rw-r--r--   0        0        0     6217 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/_utils.py
+-rw-r--r--   0        0        0    17411 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/backend.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/py.typed
+-rw-r--r--   0        0        0     5389 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/socket.py
+-rw-r--r--   0        0        0     4439 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/tasks.py
+-rw-r--r--   0        0        0     4072 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/threads.py
+-rw-r--r--   0        0        0      208 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/datagram/__init__.py
+-rw-r--r--   0        0        0     8604 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/datagram/endpoint.py
+-rw-r--r--   0        0        0     3694 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/datagram/socket.py
+-rw-r--r--   0        0        0      208 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/stream/__init__.py
+-rw-r--r--   0        0        0     5423 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/stream/listener.py
+-rw-r--r--   0        0        0     4113 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/src/easynetwork_asyncio/stream/socket.py
+-rw-r--r--   0        0        0      131 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0     1113 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/tools.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/__init__.py
+-rw-r--r--   0        0        0    18706 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_asyncio_backend.py
+-rw-r--r--   0        0        0     1288 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_backend_factory.py
+-rw-r--r--   0        0        0     3217 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_futures.py
+-rw-r--r--   0        0        0     2424 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_tasks.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/conftest.py
+-rw-r--r--   0        0        0     1781 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/serializer.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/_utils.py
+-rw-r--r--   0        0        0      527 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_client/__init__.py
+-rw-r--r--   0        0        0    19354 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_client/test_tcp.py
+-rw-r--r--   0        0        0    31112 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/base.py
+-rw-r--r--   0        0        0     4666 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_standalone.py
+-rw-r--r--   0        0        0    31268 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_tcp.py
+-rw-r--r--   0        0        0    18286 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/__init__.py
+-rw-r--r--   0        0        0     1279 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0    12790 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    16039 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0      130 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0     9118 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/base.py
+-rw-r--r--   0        0        0      424 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0     6240 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     2233 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0     4069 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_compressors.py
+-rw-r--r--   0        0        0     3572 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0     2639 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     3440 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     1926 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     2747 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_namedtuple.py
+-rw-r--r--   0        0        0     3609 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/samples/__init__.py
+-rw-r--r--   0        0        0    10664 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/samples/json.py
+-rw-r--r--   0        0        0     2356 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/functional_test/test_serializers/samples/pickle.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/other_test/__init__.py
+-rw-r--r--   0        0        0     4925 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/other_test/test_import.py
+-rw-r--r--   0        0        0      578 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/other_test/test_project_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/pytest_plugins/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/pytest_plugins/asyncio_event_loop.py
+-rw-r--r--   0        0        0     1792 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/pytest_plugins/extra_features.py
+-rw-r--r--   0        0        0      620 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/pytest_plugins/session_exit_code.py
+-rw-r--r--   0        0        0     2671 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/scripts/async_server_test.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/__init__.py
+-rw-r--r--   0        0        0     1795 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/_utils.py
+-rw-r--r--   0        0        0     1808 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/base.py
+-rw-r--r--   0        0        0     5555 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/conftest.py
+-rw-r--r--   0        0        0     5098 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_converter.py
+-rw-r--r--   0        0        0    15717 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_protocol.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/__init__.py
+-rw-r--r--   0        0        0     1114 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/base.py
+-rw-r--r--   0        0        0     2340 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/__init__.py
+-rw-r--r--   0        0        0     3083 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py
+-rw-r--r--   0        0        0    17863 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/test_backend.py
+-rw-r--r--   0        0        0     7956 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/test_futures.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/base.py
+-rw-r--r--   0        0        0     2682 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_abc.py
+-rw-r--r--   0        0        0    51599 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_tcp.py
+-rw-r--r--   0        0        0    41442 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_server/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_server/test_handler.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/__init__.py
+-rw-r--r--   0        0        0     1679 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/conftest.py
+-rw-r--r--   0        0        0    46304 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_backend.py
+-rw-r--r--   0        0        0    32981 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py
+-rw-r--r--   0        0        0    14174 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_socket.py
+-rw-r--r--   0        0        0    27018 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_stream.py
+-rw-r--r--   0        0        0     9534 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py
+-rw-r--r--   0        0        0     4898 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_threads.py
+-rw-r--r--   0        0        0    30962 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_utils.py
+-rw-r--r--   0        0        0      130 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0      612 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/base.py
+-rw-r--r--   0        0        0      355 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0    30904 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_abc.py
+-rw-r--r--   0        0        0     3514 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     5880 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0    20502 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_compressor.py
+-rw-r--r--   0        0        0     4351 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0    15194 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     7216 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     7146 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     9953 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0    16647 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_struct.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0      526 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/base.py
+-rw-r--r--   0        0        0     1019 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/conftest.py
+-rw-r--r--   0        0        0     3294 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_abc.py
+-rw-r--r--   0        0        0    67599 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    44378 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_tools/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_lock.py
+-rw-r--r--   0        0        0     7763 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_socket.py
+-rw-r--r--   0        0        0    14621 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_stream.py
+-rw-r--r--   0        0        0    22406 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_utils.py
+-rw-r--r--   0        0        0     1915 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1097 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0       55 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     5197 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-06-20 22:19:47.000000 easynetwork-1.0.0rc2/PKG-INFO
```

### Comparing `easynetwork-1.0.0rc1/.flake8` & `easynetwork-1.0.0rc2/.flake8`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/.pre-commit-config.yaml` & `easynetwork-1.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/pdm.lock` & `easynetwork-1.0.0rc2/pdm.lock`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/tox.ini` & `easynetwork-1.0.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/.vscode/settings.example.json` & `easynetwork-1.0.0rc2/.vscode/settings.example.json`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/__init__.py` & `easynetwork-1.0.0rc2/src/easynetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """The easiest way to use sockets in Python
 
 EasyNetwork is a high-level interface for networking in Python
 """
@@ -16,8 +16,8 @@
 __copyright__ = "Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine"
 __credits__ = ["FrankySnow9"]
 __deprecated__ = False
 __email__ = "clairicia.rcj.francis@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "FrankySnow9"
 __status__ = "Development"
-__version__ = "1.0.0rc1"
+__version__ = "1.0.0rc2"
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/converter.py` & `easynetwork-1.0.0rc2/src/easynetwork/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network packet converter module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/exceptions.py` & `easynetwork-1.0.0rc2/src/easynetwork/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Exceptions definition module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/protocol.py` & `easynetwork-1.0.0rc2/src/easynetwork/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network protocol module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/abc.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Asynchronous client/server module
 """
 
@@ -294,18 +294,14 @@
         raise NotImplementedError
 
     @abstractmethod
     async def ignore_cancellation(self, coroutine: Coroutine[Any, Any, _T_co]) -> _T_co:
         raise NotImplementedError
 
     @abstractmethod
-    async def wait_for(self, coroutine: Coroutine[Any, Any, _T_co], timeout: float | None) -> _T_co:
-        raise NotImplementedError
-
-    @abstractmethod
     def timeout(self, delay: float) -> AsyncContextManager[AbstractTimeoutHandle]:
         raise NotImplementedError
 
     @abstractmethod
     def timeout_at(self, deadline: float) -> AsyncContextManager[AbstractTimeoutHandle]:
         raise NotImplementedError
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/factory.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Asynchronous client/server module
 """
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/futures.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/futures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Asynchronous client/server module
 """
 
 from __future__ import annotations
 
-__all__ = ["AsyncPoolExecutor"]
+__all__ = ["AsyncExecutor", "AsyncThreadPoolExecutor"]
 
 import concurrent.futures
 import contextvars
-from typing import TYPE_CHECKING, Callable, ParamSpec, Self, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, ParamSpec, Self, TypeVar, overload
 
 from .sniffio import current_async_library_cvar as _sniffio_current_async_library_cvar
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from .abc import AbstractAsyncBackend
 
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
 
 
-class AsyncPoolExecutor:
+class AsyncExecutor:
     __slots__ = ("__backend", "__executor", "__weakref__")
 
     def __init__(self, backend: AbstractAsyncBackend, executor: concurrent.futures.Executor) -> None:
         self.__backend: AbstractAsyncBackend = backend
         self.__executor: concurrent.futures.Executor = executor
 
     async def __aenter__(self) -> Self:
@@ -40,24 +40,51 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         await self.shutdown()
 
     async def run(self, __func: Callable[_P, _T], /, *args: _P.args, **kwargs: _P.kwargs) -> _T:
-        ctx = contextvars.copy_context()
-
-        if _sniffio_current_async_library_cvar is not None:
-            ctx.run(_sniffio_current_async_library_cvar.set, None)
-
-        future: concurrent.futures.Future[_T] = self.__executor.submit(ctx.run, __func, *args, **kwargs)  # type: ignore[arg-type]
-        del __func, args, kwargs
         try:
-            return await self.__backend.wait_future(future)
+            return await self.__backend.wait_future(self.__executor.submit(__func, *args, **kwargs))
         finally:
-            del future
+            del __func, args, kwargs
 
     def shutdown_nowait(self, *, cancel_futures: bool = False) -> None:
         self.__executor.shutdown(wait=False, cancel_futures=cancel_futures)
 
     async def shutdown(self, *, cancel_futures: bool = False) -> None:
         await self.__backend.run_in_thread(self.__executor.shutdown, wait=True, cancel_futures=cancel_futures)
+
+
+class AsyncThreadPoolExecutor(AsyncExecutor):
+    __slots__ = ()
+
+    @overload
+    def __init__(self, backend: AbstractAsyncBackend) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self,
+        backend: AbstractAsyncBackend,
+        *,
+        max_workers: int | None = ...,
+        thread_name_prefix: str = ...,
+        initializer: Callable[..., object] | None = ...,
+        initargs: tuple[Any, ...] = ...,
+    ) -> None:
+        ...
+
+    def __init__(self, backend: AbstractAsyncBackend, **kwargs: Any) -> None:
+        super().__init__(backend, concurrent.futures.ThreadPoolExecutor(**kwargs))
+
+    async def run(self, __func: Callable[_P, _T], /, *args: _P.args, **kwargs: _P.kwargs) -> _T:
+        ctx = contextvars.copy_context()
+
+        if _sniffio_current_async_library_cvar is not None:
+            ctx.run(_sniffio_current_async_library_cvar.set, None)
+
+        try:
+            return await super().run(ctx.run, __func, *args, **kwargs)  # type: ignore[arg-type]
+        finally:
+            del __func, args, kwargs
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/sniffio.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/sniffio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Asynchronous client/server module
 """
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/tasks.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/backend/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Asynchronous client/server module
 """
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/client/abc.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/client/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/client/tcp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/client/tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/client/udp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/client/udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/__init__.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network server module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/abc.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network server module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/handler.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network servers' request handler base classes module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/standalone.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/standalone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network server module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/tcp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network server module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/udp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_async/server/udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Asynchronous network server module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/abc.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/tcp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/udp.py` & `easynetwork-1.0.0rc2/src/easynetwork/api_sync/client/udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network client module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/__init__.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """EasyNetwork's packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/abc.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Abstract base network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/base_stream.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/base_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Stream network packet serializer handler module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/cbor.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/cbor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """cbor-based network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/json.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """json-based network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/line.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """string line network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/msgpack.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/msgpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """msgpack-based network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/pickle.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/pickle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """pickle-based network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/struct.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """struct.Struct-based network packet serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/base64.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/base64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """base64 encoding serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/compressor.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/compressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Data compressor serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/encryptor.py` & `easynetwork-1.0.0rc2/src/easynetwork/serializers/wrapper/encryptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """encrypted data serializer module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/tools/_utils.py` & `easynetwork-1.0.0rc2/src/easynetwork/tools/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 __all__ = [
     "check_real_socket_state",
     "check_socket_family",
     "check_socket_no_ssl",
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/tools/lock.py` & `easynetwork-1.0.0rc2/src/easynetwork/tools/lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """
 Synchronization primitive extension module
 """
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/tools/socket.py` & `easynetwork-1.0.0rc2/src/easynetwork/tools/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network socket module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork/tools/stream.py` & `easynetwork-1.0.0rc2/src/easynetwork/tools/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Stream network packet serializer handler module"""
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/_utils.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.api_async
 """
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/backend.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.api_async
 """
 
 from __future__ import annotations
@@ -84,20 +84,14 @@
         asyncio._unregister_task(task)
 
         try:
             return await self._cancel_shielded_wait_asyncio_future(task)
         finally:
             del task
 
-    async def wait_for(self, coroutine: Coroutine[Any, Any, _T_co], timeout: float | None) -> _T_co:
-        assert asyncio.iscoroutine(coroutine), "Expected a coroutine object"
-
-        async with asyncio.timeout(timeout):
-            return await coroutine
-
     def timeout(self, delay: float) -> AsyncContextManager[AbstractTimeoutHandle]:
         from .tasks import timeout
 
         return timeout(delay)
 
     def timeout_at(self, deadline: float) -> AsyncContextManager[AbstractTimeoutHandle]:
         from .tasks import timeout_at
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/socket.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.async
 """
 
 from __future__ import annotations
@@ -115,15 +115,15 @@
 
     @contextlib.contextmanager
     def __conflict_detection(self, task_id: _SocketTaskId, *, abort_errno: int | None = None) -> Iterator[_socket.socket]:
         if (socket := self.__socket if not self.__closing else None) is None:
             raise _error_from_errno(_errno.ENOTSOCK)
 
         if task_id in self.__waiters:
-            raise _error_from_errno(_errno.EINPROGRESS)
+            raise _error_from_errno(_errno.EBUSY)
 
         if abort_errno is None:
             abort_errno = _errno.EINTR
 
         task = asyncio.current_task()
         if task is None:  # pragma: no cover
             raise RuntimeError("This function should be called within a task.")
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/tasks.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.api_async
 """
 
 from __future__ import annotations
@@ -105,49 +105,41 @@
 class TimeoutHandle(AbstractTimeoutHandle):
     __slots__ = ("__handle",)
 
     def __init__(self, handle: asyncio.Timeout) -> None:
         super().__init__()
         self.__handle: asyncio.Timeout = handle
 
-    def when(self) -> float:
-        deadline: float | None = self.__handle.when()
-        return deadline if deadline is not None else float("+inf")
-
-    def reschedule(self, when: float) -> None:
-        return self.__handle.reschedule(float(when) if when != float("+inf") else None)
-
-    def expired(self) -> bool:
-        return self.__handle.expired()
-
-
-class _TimeoutContextManager:
-    __slots__ = ("__handle",)
-
-    def __init__(self, handle: asyncio.Timeout) -> None:
-        super().__init__()
-        self.__handle: asyncio.Timeout = handle
-
-    async def __aenter__(self) -> TimeoutHandle:
+    async def __aenter__(self) -> Self:
         handle: asyncio.Timeout = self.__handle
         await type(handle).__aenter__(handle)
-        return TimeoutHandle(handle)
+        return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         handle: asyncio.Timeout = self.__handle
         try:
             return await type(handle).__aexit__(handle, exc_type, exc_val, exc_tb)
         finally:
             del exc_val, exc_tb, self
 
+    def when(self) -> float:
+        deadline: float | None = self.__handle.when()
+        return deadline if deadline is not None else float("+inf")
+
+    def reschedule(self, when: float) -> None:
+        return self.__handle.reschedule(float(when) if when != float("+inf") else None)
+
+    def expired(self) -> bool:
+        return self.__handle.expired()
+
 
-def timeout(delay: float) -> _TimeoutContextManager:
-    return _TimeoutContextManager(asyncio.timeout(float(delay) if delay != float("+inf") else None))
+def timeout(delay: float) -> TimeoutHandle:
+    return TimeoutHandle(asyncio.timeout(float(delay) if delay != float("+inf") else None))
 
 
-def timeout_at(deadline: float) -> _TimeoutContextManager:
-    return _TimeoutContextManager(asyncio.timeout_at(float(deadline) if deadline != float("+inf") else None))
+def timeout_at(deadline: float) -> TimeoutHandle:
+    return TimeoutHandle(asyncio.timeout_at(float(deadline) if deadline != float("+inf") else None))
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/threads.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/threads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.api_async
 """
 
 from __future__ import annotations
@@ -89,20 +89,18 @@
         self.__loop.call_soon_threadsafe(callback, future, context=ctx)
         return future
 
     @staticmethod
     def __get_result(future: concurrent.futures.Future[_T]) -> _T:
         try:
             return future.result()
-        except asyncio.CancelledError:
-            raise concurrent.futures.CancelledError() from None
         except concurrent.futures.CancelledError as exc:
             if not future.cancelled():  # raised from future.exception()
                 raise
-            raise RuntimeError("Operation cancelled") from exc
+            raise asyncio.CancelledError() from exc
         finally:
             del future
 
     def __check_running_loop(self) -> None:
         try:
             running_loop = asyncio.get_running_loop()
         except RuntimeError:
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/endpoint.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/datagram/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.async
 """
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/socket.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/datagram/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.async
 """
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/listener.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/stream/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.async
 """
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/socket.py` & `easynetwork-1.0.0rc2/src/easynetwork_asyncio/stream/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """asyncio engine for easynetwork.async
 """
 
 from __future__ import annotations
```

### Comparing `easynetwork-1.0.0rc1/tests/conftest.py` & `easynetwork-1.0.0rc2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import os
 import random
 
 random.seed(42)  # Fully deterministic random output
```

### Comparing `easynetwork-1.0.0rc1/tests/tools.py` & `easynetwork-1.0.0rc2/tests/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import time
 from typing import Any, Generator, TypeVar, final
 
 import pytest
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_asyncio_backend.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_asyncio_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from concurrent.futures import CancelledError as FutureCancelledError, Future
 
 from easynetwork.api_async.backend.factory import AsyncBackendFactory
@@ -80,44 +80,14 @@
 
         task = event_loop.create_task(backend.ignore_cancellation(self_cancellation()))
 
         with pytest.raises(asyncio.CancelledError):
             await task
         assert task.cancelled()
 
-    async def test____wait_for____without_timeout(
-        self,
-        backend: AsyncioBackend,
-    ) -> None:
-        assert (await backend.wait_for(asyncio.sleep(0.5, 42), None)) == 42
-
-    async def test____wait_for____with_timeout____respected(
-        self,
-        backend: AsyncioBackend,
-    ) -> None:
-        assert (await backend.wait_for(asyncio.sleep(0.5, 42), 1)) == 42
-
-    async def test____wait_for____with_timeout____timeout_error(
-        self,
-        backend: AsyncioBackend,
-    ) -> None:
-        with pytest.raises(TimeoutError):
-            await backend.wait_for(asyncio.sleep(0.5, 42), 0.25)
-
-    async def test____wait_for____with_timeout____cancellation(
-        self,
-        event_loop: asyncio.AbstractEventLoop,
-        backend: AsyncioBackend,
-    ) -> None:
-        task = event_loop.create_task(backend.wait_for(asyncio.sleep(0.5, 42), 0.25))
-        event_loop.call_later(0.10, task.cancel)
-
-        await asyncio.wait({task})
-        assert task.cancelled()
-
     async def test____timeout____respected(
         self,
         backend: AsyncioBackend,
     ) -> None:
         async with backend.timeout(1):
             assert await asyncio.sleep(0.5, 42) == 42
 
@@ -448,28 +418,28 @@
             task.get_loop().call_later(0.5, task.cancel)
             await task.get_loop().create_future()
             raise AssertionError("Not cancelled")
 
         def thread() -> int:
             return threads_portal.run_coroutine(coroutine, 42)
 
-        with pytest.raises(RuntimeError, match=r"^Operation cancelled$"):
+        with pytest.raises(asyncio.CancelledError):
             await backend.run_in_thread(thread)
 
     async def test____create_threads_portal____run_coroutine_from_thread____explicit_concurrent_future_Cancelled(
         self,
         backend: AsyncioBackend,
     ) -> None:
         threads_portal = backend.create_threads_portal()
 
         async def coroutine(value: int) -> int:
             raise FutureCancelledError()
 
         def thread() -> int:
-            with pytest.raises(FutureCancelledError):
+            with pytest.raises(asyncio.CancelledError):  # asyncio do the job to convert the concurrent.futures.CancelledError
                 return threads_portal.run_coroutine(coroutine, 42)
             return 54
 
         assert await backend.run_in_thread(thread) == 54
 
     @pytest.mark.feature_sniffio
     async def test____create_threads_portal____run_coroutine_from_thread____sniffio_contextvar_reset(
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_backend_factory.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_backend_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import Iterator
 
 from easynetwork.api_async.backend.factory import AsyncBackendFactory
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_futures.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_futures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 import time
 from typing import AsyncIterator
 
 from easynetwork.api_async.backend.abc import AbstractAsyncBackend
 from easynetwork.api_async.backend.factory import AsyncBackendFactory
-from easynetwork.api_async.backend.futures import AsyncPoolExecutor
+from easynetwork.api_async.backend.futures import AsyncThreadPoolExecutor
 
 import pytest
 import pytest_asyncio
 
 
 @pytest.mark.asyncio
-class TestSingleTaskRunner:
+class TestAsyncThreadPoolExecutor:
     @pytest.fixture
     @staticmethod
     def backend() -> AbstractAsyncBackend:
         return AsyncBackendFactory.new("asyncio")
 
     @pytest.fixture
     @staticmethod
     def max_workers(request: pytest.FixtureRequest) -> int | None:
         return getattr(request, "param", None)
 
     @pytest_asyncio.fixture
     @staticmethod
-    async def executor(backend: AbstractAsyncBackend, max_workers: int | None) -> AsyncIterator[AsyncPoolExecutor]:
-        async with AsyncPoolExecutor(backend, concurrent.futures.ThreadPoolExecutor(max_workers=max_workers)) as executor:
+    async def executor(backend: AbstractAsyncBackend, max_workers: int | None) -> AsyncIterator[AsyncThreadPoolExecutor]:
+        async with AsyncThreadPoolExecutor(backend, max_workers=max_workers) as executor:
             yield executor
 
     async def test____run____submit_and_wait(
         self,
-        executor: AsyncPoolExecutor,
+        executor: AsyncThreadPoolExecutor,
     ) -> None:
         def thread_fn(value: int) -> int:
             return value
 
         assert await executor.run(thread_fn, 42) == 42
 
     async def test____run____ignore_cancellation(
         self,
         event_loop: asyncio.AbstractEventLoop,
-        executor: AsyncPoolExecutor,
+        executor: AsyncThreadPoolExecutor,
     ) -> None:
         task = event_loop.create_task(executor.run(time.sleep, 0.5))
 
         for i in range(5):
             for _ in range(3):
                 event_loop.call_later(0.1 * i, task.cancel)
 
         await task
         assert not task.cancelled()
 
     @pytest.mark.feature_sniffio
     async def test____run____sniffio_contextvar_reset(
         self,
-        executor: AsyncPoolExecutor,
+        executor: AsyncThreadPoolExecutor,
     ) -> None:
         import sniffio
 
         sniffio.current_async_library_cvar.set("asyncio")
 
         def callback() -> str | None:
             return sniffio.current_async_library_cvar.get()
@@ -72,24 +72,24 @@
         cvar_outer = sniffio.current_async_library_cvar.get()
 
         assert cvar_inner is None
         assert cvar_outer == "asyncio"
 
     async def test____shutdown____idempotent(
         self,
-        executor: AsyncPoolExecutor,
+        executor: AsyncThreadPoolExecutor,
     ) -> None:
         await executor.shutdown()
         await executor.shutdown()
 
     @pytest.mark.parametrize("max_workers", [1], indirect=True, ids=lambda nb: f"max_workers=={nb}")
     async def test____shutdown____cancel_futures(
         self,
         event_loop: asyncio.AbstractEventLoop,
-        executor: AsyncPoolExecutor,
+        executor: AsyncThreadPoolExecutor,
     ) -> None:
         busy_task = event_loop.create_task(executor.run(time.sleep, 1))
 
         await asyncio.sleep(0.2)
         future_cancelled_tasks = [event_loop.create_task(executor.run(time.sleep, 0.1)) for _ in range(10)]
 
         await asyncio.sleep(0.1)
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_tasks.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_async/test_backend/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.api_async.backend.abc import AbstractAsyncBackend
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/conftest.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import ssl
 from contextlib import ExitStack
 from functools import partial
 from socket import AF_INET, AF_INET6, SOCK_DGRAM, SOCK_STREAM, has_ipv6 as HAS_IPV6, socket as Socket
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/serializer.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/serializer.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/conftest.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_tcp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_client/test_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import ssl
 from socket import AF_INET, IPPROTO_TCP, SHUT_WR, TCP_NODELAY, socket as Socket
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_udp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_client/test_udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 from socket import AF_INET, socket as Socket
 from typing import Any, AsyncIterator, Awaitable, Callable
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/base.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import AsyncIterator
 
 from easynetwork.api_async.server.abc import AbstractAsyncNetworkServer
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_standalone.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_standalone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import threading
 import time
 from typing import AsyncGenerator, Callable, Iterator
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_tcp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import collections
 import contextlib
 import logging
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_udp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_async/test_server/test_udp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import collections
 import contextlib
 import logging
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/conftest.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import time
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import Any, Callable, Iterator
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import socketserver
 import ssl
 from concurrent.futures import Future
 from socket import AF_INET, IPPROTO_TCP, SHUT_WR, TCP_NODELAY, socket as Socket
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_udp.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_communication/test_sync/test_client/test_udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET, socket as Socket
 from typing import Any, Callable, Iterator
 
 from easynetwork.api_sync.client.udp import UDPNetworkClient, UDPNetworkEndpoint
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/base.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 import random
 from abc import ABCMeta
 from typing import Any, Callable, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_base64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import random
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_cbor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_compressors.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_compressors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import random
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_encryptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 from typing import Any, Callable, final
 
 from easynetwork.serializers.wrapper.encryptor import EncryptorSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable-error-code=override
 
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_line.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 from typing import Literal, final
 
 from easynetwork.serializers.line import StringLineSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_msgpack.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_msgpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_namedtuple.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_namedtuple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 from typing import Any, NamedTuple, final
 
 from easynetwork.serializers.struct import NamedTupleStructSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_pickle.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/test_pickle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 import dataclasses
 import pickle
 import pickletools
 from typing import Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/json.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/samples/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import Any
 
 SAMPLES: list[tuple[Any, str]] = [
     (5, "positive integer"),
```

### Comparing `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/pickle.py` & `easynetwork-1.0.0rc2/tests/functional_test/test_serializers/samples/pickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from pickle import STOP as STOP_OPCODE
 
 
 class Dummy:
```

### Comparing `easynetwork-1.0.0rc1/tests/other_test/test_import.py` & `easynetwork-1.0.0rc2/tests/other_test/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from functools import cache
 from importlib import import_module
 from itertools import combinations
 from typing import TYPE_CHECKING
```

### Comparing `easynetwork-1.0.0rc1/tests/other_test/test_project_metadata.py` & `easynetwork-1.0.0rc2/tests/other_test/test_project_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import importlib.metadata as importlib_metadata
 
 import pytest
 import trove_classifiers
```

### Comparing `easynetwork-1.0.0rc1/tests/pytest_plugins/asyncio_event_loop.py` & `easynetwork-1.0.0rc2/tests/pytest_plugins/asyncio_event_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import enum
 import importlib
 from typing import TYPE_CHECKING, Any, assert_never
```

### Comparing `easynetwork-1.0.0rc1/tests/pytest_plugins/extra_features.py` & `easynetwork-1.0.0rc2/tests/pytest_plugins/extra_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import functools
 import sys
 
 import pytest
```

### Comparing `easynetwork-1.0.0rc1/tests/pytest_plugins/session_exit_code.py` & `easynetwork-1.0.0rc2/tests/pytest_plugins/session_exit_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import pytest
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
```

### Comparing `easynetwork-1.0.0rc1/tests/scripts/async_server_test.py` & `easynetwork-1.0.0rc2/tests/scripts/async_server_test.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/_utils.py` & `easynetwork-1.0.0rc2/tests/unit_test/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import functools
 from types import TracebackType
 from typing import Any
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/base.py` & `easynetwork-1.0.0rc2/tests/unit_test/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET6
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.tools.socket import AddressFamily
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/conftest.py` & `easynetwork-1.0.0rc2/tests/unit_test/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import pathlib
 from socket import AF_INET, IPPROTO_TCP, IPPROTO_UDP, SOCK_DGRAM, SOCK_STREAM, socket as Socket
 from ssl import SSLContext, SSLSocket
 from typing import TYPE_CHECKING, Any, Callable
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_converter.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable
 
 from easynetwork.converter import AbstractPacketConverterComposite, PacketConverterComposite, RequestResponseConverterBuilder
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_protocol.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generator
 
 from easynetwork.exceptions import (
     DatagramProtocolParseError,
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/base.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET6
 from typing import TYPE_CHECKING
 
 from easynetwork.tools.socket import new_socket_address
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/conftest.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Callable
 
 from easynetwork.api_async.backend.abc import (
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from socket import socket as Socket
 from typing import Any, AsyncContextManager, Callable, Coroutine, NoReturn, Sequence, final
 
 from easynetwork.api_async.backend.abc import (
@@ -37,17 +37,14 @@
 
     async def cancel_shielded_coro_yield(self) -> None:
         raise NotImplementedError
 
     async def ignore_cancellation(self, coroutine: Coroutine[Any, Any, Any]) -> Any:
         raise NotImplementedError
 
-    async def wait_for(self, coroutine: Coroutine[Any, Any, Any], timeout: float | None) -> Any:
-        raise NotImplementedError
-
     def timeout(self, delay: Any) -> AsyncContextManager[AbstractTimeoutHandle]:
         raise NotImplementedError
 
     def timeout_at(self, deadline: Any) -> AsyncContextManager[AbstractTimeoutHandle]:
         raise NotImplementedError
 
     def get_cancelled_exc_class(self) -> type[BaseException]:
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/test_backend.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_backend/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from socket import socket as Socket
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any, Coroutine, Iterator, Literal, assert_never, final
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_abc.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.api_async.client.abc import AbstractAsyncNetworkClient
 from easynetwork.tools.socket import SocketAddress
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_tcp.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import errno
 import os
 from socket import AF_INET6, IPPROTO_TCP, SO_KEEPALIVE, SOL_SOCKET, TCP_NODELAY
 from typing import TYPE_CHECKING, Any
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_udp.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_client/test_udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET6
 from typing import TYPE_CHECKING, Any, cast
 
 from easynetwork.api_async.client.udp import AsyncUDPNetworkClient, AsyncUDPNetworkEndpoint
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_server/test_handler.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_api/test_server/test_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=func-returns-value
 
 from __future__ import annotations
 
 import inspect
 from typing import TYPE_CHECKING, Any, AsyncGenerator
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/conftest.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Callable
 
 from easynetwork_asyncio.datagram.endpoint import DatagramEndpoint
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_backend.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import contextvars
 from typing import TYPE_CHECKING, Any, Callable, Sequence, cast
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any, Callable
 
 from easynetwork_asyncio.datagram.endpoint import DatagramEndpoint, DatagramEndpointProtocol, create_datagram_endpoint
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_socket.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 from socket import socket as Socket
@@ -78,25 +78,25 @@
     async def test____method____busy(
         self,
         socket_method: Callable[[], Coroutine[Any, Any, Any]],
         event_loop: asyncio.AbstractEventLoop,
         mock_socket_method: MagicMock,
     ) -> None:
         # Arrange
-        from errno import EINPROGRESS
+        from errno import EBUSY
 
         with self._set_sock_method_in_blocking_state(mock_socket_method):
             _ = await self._busy_socket_task(socket_method(), event_loop, mock_socket_method)
 
         # Act
         with pytest.raises(OSError) as exc_info:
             await socket_method()
 
         # Assert
-        assert exc_info.value.errno == EINPROGRESS
+        assert exc_info.value.errno == EBUSY
         mock_socket_method.assert_not_called()
 
     async def test____method____closed_socket____before_attempt(
         self,
         socket: AsyncSocket,
         socket_method: Callable[[], Coroutine[Any, Any, Any]],
         mock_socket_method: MagicMock,
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_stream.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 # mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import asyncio
 import asyncio.trsock
 from typing import TYPE_CHECKING, Any, Callable
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import math
 from typing import TYPE_CHECKING, Any
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_threads.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_threads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any
 
 from easynetwork_asyncio.threads import ThreadsPortal
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_utils.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_async/test_asyncio_backend/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import asyncio
 import asyncio.trsock
 import errno
 from socket import (
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/base.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 from typing import Any, Callable
 
 import pytest
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_abc.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 import random
 from typing import IO, TYPE_CHECKING, Any, Generator, final
 
 from easynetwork.exceptions import DeserializeError, IncrementalDeserializeError
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_base64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.exceptions import DeserializeError
 from easynetwork.serializers.wrapper.base64 import Base64EncodedSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_cbor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.serializers.cbor import CBORDecoderConfig, CBOREncoderConfig, CBORSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_compressor.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_compressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Iterator
 
 from easynetwork.exceptions import DeserializeError, IncrementalDeserializeError
 from easynetwork.serializers.wrapper.compressor import (
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_encryptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.exceptions import DeserializeError
 from easynetwork.serializers.wrapper.encryptor import EncryptorSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generator
 
 from easynetwork.exceptions import DeserializeError, IncrementalDeserializeError
 from easynetwork.serializers.json import JSONDecoderConfig, JSONEncoderConfig, JSONSerializer, _JSONParser
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_line.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 from typing import Literal
 
 from easynetwork.exceptions import DeserializeError
 from easynetwork.serializers.line import StringLineSerializer
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_msgpack.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_msgpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.exceptions import DeserializeError
 from easynetwork.serializers.msgpack import MessagePackerConfig, MessagePackSerializer, MessageUnpackerConfig
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_pickle.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_pickle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*
+# -*- coding: utf-8 -*
 
 from __future__ import annotations
 
 import pickle
 from io import BytesIO
 from pickle import DEFAULT_PROTOCOL, Pickler, Unpickler
 from typing import TYPE_CHECKING, Any, final
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_struct.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_serializers/test_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import collections
 from typing import TYPE_CHECKING, Any, Iterable, final
 
 from easynetwork.exceptions import DeserializeError
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/base.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ...base import BaseTestSocket
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/conftest.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from selectors import BaseSelector
 from typing import TYPE_CHECKING
 
 import pytest
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_abc.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from collections import deque
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.api_sync.client.abc import AbstractNetworkClient
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_tcp.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import contextlib
 import errno
 import os
 from selectors import EVENT_READ, EVENT_WRITE
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_udp.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_sync/test_client/test_udp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from selectors import EVENT_READ, EVENT_WRITE
 from socket import AF_INET6, SOCK_DGRAM
 from typing import TYPE_CHECKING, Any
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_lock.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import os
 import random
 import threading
 from typing import TYPE_CHECKING
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_socket.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import socket
 from typing import TYPE_CHECKING, Any, Callable
 
 from easynetwork.tools.socket import (
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_stream.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generator
 
 from easynetwork.tools.stream import StreamDataConsumer, StreamDataProducer
```

### Comparing `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_utils.py` & `easynetwork-1.0.0rc2/tests/unit_test/test_tools/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: Utf-8 -*-
+# -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import os
 import selectors
 from socket import (
     AF_INET,
```

### Comparing `easynetwork-1.0.0rc1/.gitignore` & `easynetwork-1.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/LICENSE` & `easynetwork-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc1/pyproject.toml` & `easynetwork-1.0.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = "FrankySnow9", email = "clairicia.rcj.francis@gmail.com"}
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
```

### Comparing `easynetwork-1.0.0rc1/PKG-INFO` & `easynetwork-1.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: easynetwork
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: The easiest way to use sockets in Python
 Project-URL: Homepage, https://github.com/francis-clairicia/EasyNetwork
 Author-email: FrankySnow9 <clairicia.rcj.francis@gmail.com>
 License-File: LICENSE
 Keywords: async,asynchronous,client,communication,networking,serialization,server,socket
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
```

